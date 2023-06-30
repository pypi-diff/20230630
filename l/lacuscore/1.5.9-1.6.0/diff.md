# Comparing `tmp/lacuscore-1.5.9.tar.gz` & `tmp/lacuscore-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.5.9.tar", max compression
+gzip compressed data, was "lacuscore-1.6.0.tar", max compression
```

## Comparing `lacuscore-1.5.9.tar` & `lacuscore-1.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.9/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.9/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.9/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.9/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    30838 2023-06-18 13:51:13.388781 lacuscore-1.5.9/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.9/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-06-18 13:51:46.400929 lacuscore-1.5.9/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.6.0/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.6.0/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.6.0/lacuscore/__init__.py
+-rw-r--r--   0        0        0     2138 2023-06-27 10:03:30.510884 lacuscore-1.6.0/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    33491 2023-06-27 10:02:06.046544 lacuscore-1.6.0/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.6.0/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-06-30 14:22:29.631600 lacuscore-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.6.0/PKG-INFO
```

### Comparing `lacuscore-1.5.9/LICENSE` & `lacuscore-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.9/README.md` & `lacuscore-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.9/lacuscore/lacuscore.py` & `lacuscore-1.6.0/lacuscore/lacuscore.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import sys
 import time
 import unicodedata
 import zlib
 
 from asyncio import Task
 from base64 import b64decode, b64encode
+from datetime import date, timedelta
 from enum import IntEnum, unique
 from logging import LoggerAdapter
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Literal, Optional, Union, Dict, List, Any, TypedDict, overload, Tuple, cast, MutableMapping, Iterator
 from uuid import uuid4
 from urllib.parse import urlsplit
@@ -334,17 +335,17 @@
         p.hset(f'lacus:capture_settings:{perma_uuid}', mapping=mapping_capture)  # type: ignore
         p.zadd('lacus:to_capture', {perma_uuid: priority})
         p.execute()
         return perma_uuid
 
     def _encode_response(self, capture: CaptureResponse) -> CaptureResponseJson:
         encoded_capture = cast(CaptureResponseJson, capture)
-        if capture.get('png') is not None:
+        if capture.get('png') is not None and capture['png'] is not None:  # the second part is not needed, but makes mypy happy
             encoded_capture['png'] = b64encode(capture['png']).decode()
-        if capture.get('downloaded_file') is not None:
+        if capture.get('downloaded_file') is not None and capture['downloaded_file'] is not None:  # the second part is not needed, but makes mypy happy
             encoded_capture['downloaded_file'] = b64encode(capture['downloaded_file']).decode()
         if capture.get('children') and capture['children']:
             for child in capture['children']:
                 child = self._encode_response(child)
         return encoded_capture
 
     @overload
@@ -420,14 +421,16 @@
         """
         if self.redis.zscore('lacus:ongoing', uuid) is not None:
             # the capture is ongoing
             return
 
         logger = LacusCoreLogAdapter(self.master_logger, {'uuid': uuid})
         self.redis.zadd('lacus:ongoing', {uuid: time.time()})
+        stats_pipeline = self.redis.pipeline()
+        today = date.today().isoformat()
 
         retry = False
         try:
             setting_keys = ['depth', 'rendered_hostname_only', 'url', 'document_name',
                             'document', 'browser', 'device_name', 'user_agent', 'proxy',
                             'general_timeout_in_sec', 'cookies', 'headers', 'http_credentials',
                             'viewport', 'referer', 'geolocation', 'timezone_id', 'locale',
@@ -465,15 +468,16 @@
                         raise LacusCoreException(f'Unexpected setting: {k}: {v}')
             except LacusCoreException as e:
                 raise e
             except Exception as e:
                 raise LacusCoreException(f'Error while preparing settings: {e}')
 
             if not to_capture:
-                result = {'error': f'No capture settings for {uuid}.'}
+                all_entries = self.redis.hgetall(f'lacus:capture_settings:{uuid}')
+                result = {'error': f'No capture settings for {uuid} - {all_entries}'}
                 raise CaptureError
 
             if document_as_bytes:
                 # we do not have a URL yet.
                 name = to_capture.pop('document_name', None)
                 if not name:
                     raise LacusCoreException('No document name provided, settings are invalid')
@@ -541,14 +545,15 @@
                 else:
                     browser_engine = 'webkit'
             try:
                 logger.debug(f'Capturing {url}')
                 # NOTE: starting with python 3.11, we can use asyncio.timeout
                 # async with asyncio.timeout(self.max_capture_time):
                 general_timeout = to_capture.get('general_timeout_in_sec')
+                stats_pipeline.sadd(f'stats:{today}:captures', url)
                 async with Capture(
                         browser=browser_engine,
                         device_name=to_capture.get('device_name'),
                         proxy=proxy,
                         general_timeout_in_sec=general_timeout) as capture:
                     # required by Mypy: https://github.com/python/mypy/issues/3004
                     capture.headers = to_capture.get('headers')  # type: ignore
@@ -568,14 +573,18 @@
                     playwright_result = await asyncio.wait_for(
                         capture.capture_page(
                             url, referer=to_capture.get('referer'),
                             depth=to_capture.get('depth', 0),
                             rendered_hostname_only=to_capture.get('rendered_hostname_only', True),
                             max_depth_capture_time=self.max_capture_time),
                         timeout=self.max_capture_time)
+                    if 'error' in playwright_result and 'error_name' in playwright_result:
+                        # generate stats
+                        if playwright_result['error_name'] is not None:
+                            stats_pipeline.zincrby(f'stats:{today}:errors', 1, playwright_result['error_name'])
             except PlaywrightCaptureException as e:
                 logger.exception(f'Invalid parameters for the capture of {url} - {e}')
                 result = {'error': f'Invalid parameters for the capture of {url} - {e}'}
                 raise CaptureError
             except asyncio.CancelledError:
                 logger.warning(f'The capture of {url} has been cancelled.')
                 result = {'error': f'The capture of {url} has been cancelled.'}
@@ -589,29 +598,37 @@
                 result = {'error': f'Something went poorly {url} - {e}'}
                 raise CaptureError
 
             if capture.should_retry:
                 # PlaywrightCapture considers this capture elligible for a retry
                 logger.info('PlaywrightCapture considers it elligible for a retry.')
                 raise RetryCapture
+            elif self.redis.exists(f'lacus:capture_retry:{uuid}'):
+                # this is a retry that worked
+                stats_pipeline.sadd(f'stats:{today}:retry_success', url)
         except RetryCapture:
             # Check if we already re-tried this capture
-            if (current_retry := self.redis.get(f'lacus:capture_retry:{uuid}')) is None:
-                self.redis.setex(f'lacus:capture_retry:{uuid}', self.max_capture_time * (self.max_retries + 1), self.max_retries)
-            else:
-                self.redis.decr(f'lacus:capture_retry:{uuid}')
-            if current_retry is None or int(current_retry.decode()) > 0:
-                logger.debug(f'Retrying {url}.')
-                # Just wait a little bit before retrying, expecially if it is the only capture in the queue
-                await asyncio.sleep(random.randint(5, 10))
+            _current_retry = self.redis.get(f'lacus:capture_retry:{uuid}')
+            if _current_retry is None:
+                # No retry yet
+                logger.debug(f'Retrying {url} for the first time.')
                 retry = True
+                self.redis.setex(f'lacus:capture_retry:{uuid}',
+                                 self.max_capture_time * (self.max_retries + 1),
+                                 self.max_retries)
             else:
-                error_msg = result['error'] if result.get('error') else 'Unknown error'
-                logger.info(f'Retried too many times {url}: {error_msg}')
-
+                current_retry = int(_current_retry.decode())
+                if current_retry > 0:
+                    logger.debug(f'Retrying {url} for the {self.max_retries-current_retry+1}th time.')
+                    self.redis.decr(f'lacus:capture_retry:{uuid}')
+                    retry = True
+                else:
+                    error_msg = result['error'] if result.get('error') else 'Unknown error'
+                    logger.info(f'Retried too many times {url}: {error_msg}')
+                    stats_pipeline.sadd(f'stats:{today}:retry_failed', url)
         except CaptureError:
             if not result:
                 result = {'error': "No result key, shouldn't happen"}
                 logger.exception(f'Unable to capture: {result["error"]}')
             if url:
                 logger.warning(f'Unable to capture {url}: {result["error"]}')
             else:
@@ -620,46 +637,69 @@
             msg = f'Something unexpected happened with {url}: {e}'
             result = {'error': msg}
             logger.exception(msg)
         else:
             result = cast(CaptureResponse, playwright_result)
             if start_time := self.redis.zscore('lacus:ongoing', uuid):
                 runtime = time.time() - start_time
-                logger.info(f'Successfully captured {url} - Runtime: {runtime}s')
+                logger.info(f'Capture of {url} finished - Runtime: {runtime}s')
                 result['runtime'] = runtime
             else:
-                logger.info(f'Successfully captured {url} - No Runtime.')
+                logger.info(f'Capture of {url} finished - No Runtime.')
         finally:
+            # NOTE: in this block, we absolutely have to make sure the UUID is removed
+            #       from the lacus:ongoing sorted set (it is definitely not ongoing anymore)
+            #       and optionally re-added to lacus:to_capture if re want to retry it
 
             if to_capture.get('document'):
                 os.unlink(tmp_f.name)
 
-            retry_redis_error = 3
-            while retry_redis_error > 0:
-                try:
-                    to_store = b''
-                    p = self.redis.pipeline()
-                    if retry:
-                        p.zadd('lacus:to_capture', {uuid: priority - 1})
-                    else:
-                        to_store = zlib.compress(pickle.dumps(result))
-                        p.setex(f'lacus:capture_results:{uuid}', 36000, to_store)
-                        p.delete(f'lacus:capture_settings:{uuid}')
-                    p.zrem('lacus:ongoing', uuid)
-                    p.execute()
-                    break
-                except RedisConnectionError as e:
-                    logger.warning(f'Unable to store capture result (size: {sys.getsizeof(to_store)} - Redis Connection Error: {e}')
-                    retry_redis_error -= 1
+            if retry:
+                if self.redis.zcard('lacus:to_capture') == 0:
+                    # Just wait a little bit before retrying
                     await asyncio.sleep(random.randint(5, 10))
+                p = self.redis.pipeline()
+                p.zrem('lacus:ongoing', uuid)
+                p.zadd('lacus:to_capture', {uuid: priority - 1})
+                p.execute()
             else:
-                logger.critical('Unable to connect to redis and to push the result of the capture.')
+                to_store = zlib.compress(pickle.dumps(result))
+                retry_redis_error = 3
+                while retry_redis_error > 0:
+                    try:
+                        p = self.redis.pipeline()
+                        p.setex(f'lacus:capture_results:{uuid}', 36000, to_store)
+                        p.delete(f'lacus:capture_settings:{uuid}')
+                        p.zrem('lacus:ongoing', uuid)
+                        p.execute()
+                        break
+                    except RedisConnectionError as e:
+                        logger.warning(f'Unable to store capture result (size: {sys.getsizeof(to_store)} - Redis Connection Error: {e}')
+                        retry_redis_error -= 1
+                        await asyncio.sleep(random.randint(5, 10))
+                else:
+                    self.redis.zrem('lacus:ongoing', uuid)
+                    stats_pipeline.zincrby(f'stats:{today}:errors', 1, 'Redis Connection')
+                    logger.critical('Unable to connect to redis and to push the result of the capture.')
+
+            # Expire stats in 10 days
+            expire_time = timedelta(days=10)
+            stats_pipeline.expire(f'stats:{today}:errors', expire_time)
+            stats_pipeline.expire(f'stats:{today}:retry_failed', expire_time)
+            stats_pipeline.expire(f'stats:{today}:retry_success', expire_time)
+            stats_pipeline.expire(f'stats:{today}:captures', expire_time)
+            stats_pipeline.execute()
 
     def clear_capture(self, uuid: str, reason: str):
         '''Remove a capture from the list, shouldn't happen unless it is in error'''
+        logger = LacusCoreLogAdapter(self.master_logger, {'uuid': uuid})
+        if self.get_capture_status(uuid) in [CaptureStatus.ONGOING, CaptureStatus.QUEUED]:
+            logger.warning('Attempted to clear capture that is still being processed.')
+            return
+        logger.warning(f'Clearing capture: {reason}')
         result = {'error': reason}
         p = self.redis.pipeline()
         to_store = zlib.compress(pickle.dumps(result))
         p.setex(f'lacus:capture_results:{uuid}', 36000, to_store)
         p.delete(f'lacus:capture_settings:{uuid}')
         p.zrem('lacus:ongoing', uuid)
         p.execute()
```

### Comparing `lacuscore-1.5.9/pyproject.toml` & `lacuscore-1.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.5.9"
+version = "1.6.0"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -28,28 +28,28 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 Sphinx = { version = "^7.0.1", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.20.5"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.21.0"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
-redis = {version = "^4.5.5", extras = ["hiredis"]}
+redis = {version = "^4.6.0", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
-types-redis = {version = "^4.5.5.2"}
-mypy = "^1.3.0"
+types-redis = {version = "^4.6.0.0"}
+mypy = "^1.4.1"
 types-requests = "^2.31.0.1"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.13.0", python = ">=3.9"}
 ]
-pytest = "^7.3.2"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lacuscore-1.5.9/PKG-INFO` & `lacuscore-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.5.9
+Version: 1.6.0
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.20.5,<2.0.0)
-Requires-Dist: redis[hiredis] (>=4.5.5,<5.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.21.0,<2.0.0)
+Requires-Dist: redis[hiredis] (>=4.6.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/lacuscore/badge/?version=latest)](https://lacuscore.readthedocs.io/en/latest/?badge=latest)
```

