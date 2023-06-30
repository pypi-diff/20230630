# Comparing `tmp/atomcache-0.7.3.tar.gz` & `tmp/atomcache-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomcache-0.7.3.tar", max compression
+gzip compressed data, was "atomcache-0.7.4.tar", max compression
```

## Comparing `atomcache-0.7.3.tar` & `atomcache-0.7.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.3/LICENSE
--rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.3/README.md
--rw-r--r--   0        0        0      160 2023-06-29 14:56:27.625934 atomcache-0.7.3/atomcache/__init__.py
--rw-r--r--   0        0        0     1421 2023-06-29 14:55:22.713233 atomcache-0.7.3/atomcache/backend.py
--rw-r--r--   0        0        0    10452 2023-06-29 14:55:22.723234 atomcache-0.7.3/atomcache/base.py
--rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.3/atomcache/py.typed
--rw-r--r--   0        0        0     4962 2023-06-29 14:55:22.716234 atomcache-0.7.3/atomcache/redis.py
--rw-r--r--   0        0        0      951 2023-06-29 14:56:34.604009 atomcache-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 atomcache-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.4/LICENSE
+-rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.4/README.md
+-rw-r--r--   0        0        0      160 2023-06-30 10:08:19.292207 atomcache-0.7.4/atomcache/__init__.py
+-rw-r--r--   0        0        0     1421 2023-06-30 10:06:30.127745 atomcache-0.7.4/atomcache/backend.py
+-rw-r--r--   0        0        0     9790 2023-06-30 10:07:43.401727 atomcache-0.7.4/atomcache/base.py
+-rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.4/atomcache/py.typed
+-rw-r--r--   0        0        0     4962 2023-06-30 10:06:30.130746 atomcache-0.7.4/atomcache/redis.py
+-rw-r--r--   0        0        0      951 2023-06-30 10:08:24.766280 atomcache-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 atomcache-0.7.4/PKG-INFO
```

### Comparing `atomcache-0.7.3/LICENSE` & `atomcache-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.3/README.md` & `atomcache-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.3/atomcache/backend.py` & `atomcache-0.7.4/atomcache/backend.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.3/atomcache/base.py` & `atomcache-0.7.4/atomcache/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import inspect
 import json
+from contextlib import suppress
 from functools import partial
 from hashlib import sha256
 from typing import Any, Awaitable, Callable, Coroutine, Dict, Optional, TypeVar, Union
 
 from fastapi import FastAPI, Request, Response, params
 from fastapi.encoders import jsonable_encoder
 from fastapi.routing import APIRoute
@@ -66,24 +67,19 @@
         self.auto_refresh = auto_refresh
         self._expire = exp
         self.namespace = namespace
         self._lock_timeout = lock_timeout
         self._allow_cache_control = cache_control
         self._autorefresh_callback: Union[Callable, Awaitable, None] = None
         self._autorefresh_task: Optional[asyncio.Future] = None
-        self._refreshing: bool = False
         self._no_cache: bool = False
 
     async def __call__(self, request: Request):
         if self._allow_cache_control:
             self._no_cache = "no-cache" in CommaSeparatedStrings(request.headers.get("Cache-Control", ""))
-        if self._refreshing:
-            cached_content, ttl = await self.backend.get(self.get_key(), with_lock=False)
-            if cached_content is not None:
-                raise CachedResponse(content=cached_content, ttl=ttl)
         return self
 
     def set_namespace(self, namespace: str):  # noqa: WPS615 FIXME: unpythonic setter
         self.namespace = namespace
 
     def set_autorefresh_callback(self, endpoint: Union[Callable, Coroutine]):  # noqa: WPS231 WPS615
         kwargs = {}
@@ -154,15 +150,15 @@
             cache_id (str, optional): Cache identifier. Defaults to "".
             with_lock (bool, optional): Lock the cache if there is no response. Defaults to True.
             lockspace (str, optional): Key to use for lock
 
         Raises:
             CachedResponse: generate response from cache.
         """
-        if self._refreshing or self._no_cache:
+        if self._no_cache:
             return
         cached_content, ttl = await self.backend.get(
             self.get_key(cache_id),
             timeout=self._lock_timeout,
             with_lock=with_lock,
             lockspace=lockspace,
         )
@@ -202,29 +198,18 @@
                 cache = default.dependency
                 if cache.namespace is None:
                     cache.set_namespace(route.path)
                 if cache.auto_refresh:
                     cache.set_autorefresh_callback(route.endpoint)
 
     async def _autorefresh(self):
-        key = self.get_key()
-
-        ttl = await self.backend.ttl(key)
-
-        time_until_refresh = ttl - self._lock_timeout  # In case key is not setted ttl is -2
-
-        if time_until_refresh > 0:
-            await asyncio.sleep(time_until_refresh)
-        if await self.backend.lock(key, timeout=self._lock_timeout):
-            self._autorefresh_task = asyncio.ensure_future(self._autorefresh())
-            self._refreshing = True
-            try:  # noqa: WPS501
+        while True:  # noqa: WPS457
+            with suppress(CachedResponse):
                 await self._autorefresh_callback()
-            finally:
-                self._refreshing = False
+            await asyncio.sleep(self._expire - self._lock_timeout)
 
 
 def cached_response_handler(request: Request, exc: CachedResponse) -> Response:
     if_none_match = request.headers.get("if-none-match")
     etag = f"W/{hashsum(exc.content)}"
     if if_none_match == etag:
         response = Response(status_code=304, headers={"Cache-Control": f"max-age={exc.ttl}"})  # noqa:WPS432
```

### Comparing `atomcache-0.7.3/atomcache/redis.py` & `atomcache-0.7.4/atomcache/redis.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.3/pyproject.toml` & `atomcache-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atomcache"
-version = "0.7.3"
+version = "0.7.4"
 description = "Asynchronous cache manager designed for horizontally scaled web applications."
 authors = ["Serghei Ungurean <srg@intelbit.io>", "Nichita Morcotilo <nmorkotilo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pysergio/atomcache"
 repository = "https://github.com/pysergio/atomcache"
```

### Comparing `atomcache-0.7.3/PKG-INFO` & `atomcache-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomcache
-Version: 0.7.3
+Version: 0.7.4
 Summary: Asynchronous cache manager designed for horizontally scaled web applications.
 Home-page: https://github.com/pysergio/atomcache
 License: MIT
 Author: Serghei Ungurean
 Author-email: srg@intelbit.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: atomcache Version: 0.7.3 Summary: Asynchronous
+Metadata-Version: 2.1 Name: atomcache Version: 0.7.4 Summary: Asynchronous
 cache manager designed for horizontally scaled web applications. Home-page:
 https://github.com/pysergio/atomcache License: MIT Author: Serghei Ungurean
 Author-email: srg@intelbit.io Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: fastapi
```

