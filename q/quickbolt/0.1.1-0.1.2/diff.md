# Comparing `tmp/quickbolt-0.1.1.tar.gz` & `tmp/quickbolt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbolt-0.1.1.tar", max compression
+gzip compressed data, was "quickbolt-0.1.2.tar", max compression
```

## Comparing `quickbolt-0.1.1.tar` & `quickbolt-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.1/LICENSE
--rw-r--r--   0        0        0     3947 2023-06-25 21:46:08.497591 quickbolt-0.1.1/README.md
--rw-r--r--   0        0        0     1238 2023-06-29 03:21:24.065633 quickbolt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.1/quickbolt/__init__.py
--rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.1/quickbolt/batch_generation/__init__.py
--rw-r--r--   0        0        0    10231 2023-06-28 14:58:27.760352 quickbolt-0.1.1/quickbolt/batch_generation/batch_generation.py
--rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.1/quickbolt/clients/__init__.py
--rw-r--r--   0        0        0     9806 2023-06-29 02:36:13.536989 quickbolt-0.1.1/quickbolt/clients/aio_requests.py
--rw-r--r--   0        0        0    10021 2023-06-29 02:36:13.537220 quickbolt-0.1.1/quickbolt/clients/httpx_requests.py
--rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.1/quickbolt/logging/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-29 02:36:13.537441 quickbolt-0.1.1/quickbolt/logging/async_logger.py
--rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.1/quickbolt/pytest/__init__.py
--rw-r--r--   0        0        0     4628 2023-06-29 02:36:13.537663 quickbolt-0.1.1/quickbolt/pytest/core_pytest_base.py
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.1/quickbolt/reporting/__init__.py
--rw-r--r--   0        0        0     6776 2023-06-29 02:36:13.537886 quickbolt-0.1.1/quickbolt/reporting/response_csv.py
--rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.1/quickbolt/utils/__init__.py
--rw-r--r--   0        0        0     3859 2023-06-24 00:16:27.310243 quickbolt-0.1.1/quickbolt/utils/dictionary.py
--rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.1/quickbolt/utils/directory.py
--rw-r--r--   0        0        0     1763 2023-06-27 06:26:52.439989 quickbolt-0.1.1/quickbolt/utils/json.py
--rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.1/quickbolt/utils/sync_async.py
--rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.1/quickbolt/validations/__init__.py
--rw-r--r--   0        0        0     4866 2023-06-28 14:58:27.760715 quickbolt-0.1.1/quickbolt/validations/validations.py
--rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 quickbolt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3947 2023-06-25 21:46:08.497591 quickbolt-0.1.2/README.md
+-rw-r--r--   0        0        0     1238 2023-06-29 23:02:31.932187 quickbolt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.2/quickbolt/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.2/quickbolt/batch_generation/__init__.py
+-rw-r--r--   0        0        0    10231 2023-06-29 16:19:50.859017 quickbolt-0.1.2/quickbolt/batch_generation/batch_generation.py
+-rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.2/quickbolt/clients/__init__.py
+-rw-r--r--   0        0        0     9806 2023-06-29 16:19:54.925810 quickbolt-0.1.2/quickbolt/clients/aio_requests.py
+-rw-r--r--   0        0        0    10021 2023-06-29 16:19:54.926154 quickbolt-0.1.2/quickbolt/clients/httpx_requests.py
+-rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.2/quickbolt/logging/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.1.2/quickbolt/logging/async_logger.py
+-rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.2/quickbolt/pytest/__init__.py
+-rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.1.2/quickbolt/pytest/core_pytest_base.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.2/quickbolt/reporting/__init__.py
+-rw-r--r--   0        0        0     7244 2023-06-29 21:59:20.300359 quickbolt-0.1.2/quickbolt/reporting/response_csv.py
+-rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.2/quickbolt/utils/__init__.py
+-rw-r--r--   0        0        0     3859 2023-06-24 00:16:27.310243 quickbolt-0.1.2/quickbolt/utils/dictionary.py
+-rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.2/quickbolt/utils/directory.py
+-rw-r--r--   0        0        0     1763 2023-06-27 06:26:52.439989 quickbolt-0.1.2/quickbolt/utils/json.py
+-rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.2/quickbolt/utils/sync_async.py
+-rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.2/quickbolt/validations/__init__.py
+-rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.1.2/quickbolt/validations/validations.py
+-rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 quickbolt-0.1.2/PKG-INFO
```

### Comparing `quickbolt-0.1.1/LICENSE` & `quickbolt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/README.md` & `quickbolt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/pyproject.toml` & `quickbolt-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbolt"
-version = "0.1.1"
+version = "0.1.2"
 description = "Asynchronously make and validate requests!"
 authors = ["Ashton Szabo <aszabo00@gmail.com>"]
 repository = "https://github.com/aszabo00/quickbolt"
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Intended Audience :: Information Technology",
```

### Comparing `quickbolt-0.1.1/quickbolt/batch_generation/batch_generation.py` & `quickbolt-0.1.2/quickbolt/batch_generation/batch_generation.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/quickbolt/clients/aio_requests.py` & `quickbolt-0.1.2/quickbolt/clients/aio_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/quickbolt/clients/httpx_requests.py` & `quickbolt-0.1.2/quickbolt/clients/httpx_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/quickbolt/logging/async_logger.py` & `quickbolt-0.1.2/quickbolt/logging/async_logger.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/quickbolt/pytest/core_pytest_base.py` & `quickbolt-0.1.2/quickbolt/pytest/core_pytest_base.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/quickbolt/reporting/response_csv.py` & `quickbolt-0.1.2/quickbolt/reporting/response_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from copy import deepcopy
 
 import aiofiles.os as aos
 import numpy as np
 from aiocsv import AsyncDictReader, AsyncReader, AsyncWriter
 from aiofiles import open as aopen
 
+import quickbolt.utils.dictionary as dh
 import quickbolt.utils.json as jh
 
 
 async def read_csv(csv_path: None | str) -> list[list]:
     """
     This reads a csv.
 
@@ -44,15 +45,23 @@
 
     Args:
         text: The text to scrub.
 
     Returns:
         scrubbed_text: The scrubbed text.
     """
-    scrubbed_text = text
+    # need to do better here
+    text_dict = jh.deserialize(text)
+    flat_scrubbed_text = dh.flatten(text_dict)
+    for key, value in flat_scrubbed_text.items():
+        if not isinstance(value, str):
+            val_type = type(value).__name__
+            flat_scrubbed_text[key] = f"{value} ({val_type})"
+    unflat_scrubbed_text = dh.unflatten(flat_scrubbed_text)
+    scrubbed_text = jh.serialize(unflat_scrubbed_text)
 
     targets = re.findall(
         r"([A-Za-z]+[\d@]+[\w@]*|[\d@]+[A-Za-z]+[\w@]*|\d+)", scrubbed_text
     )
     targets.sort(key=len, reverse=True)
 
     for t in targets:
@@ -123,15 +132,15 @@
 
     for r in responses:
         r["server_headers"] = {k: v for k, v in r["server_headers"].items()}
 
         kwargs = r.get("kwargs", {})
         r["body"] = kwargs.pop("message", {}) or kwargs.pop("data", {})
         if "FormData" in str(type(r["body"])):
-            r["body"] = r["body"]._fields
+            r["body"] = {f[0]["name"]: f[2] for f in r["body"]._fields}
         elif isinstance(r["body"], dict):
             update = {
                 k: v.name
                 for k, v in r["body"].items()
                 if "BufferedReader" in str(type(v))
             }
             r["body"].update(update)
```

### Comparing `quickbolt-0.1.1/quickbolt/utils/dictionary.py` & `quickbolt-0.1.2/quickbolt/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/quickbolt/utils/directory.py` & `quickbolt-0.1.2/quickbolt/utils/directory.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/quickbolt/utils/json.py` & `quickbolt-0.1.2/quickbolt/utils/json.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/quickbolt/validations/validations.py` & `quickbolt-0.1.2/quickbolt/validations/validations.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.1/PKG-INFO` & `quickbolt-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbolt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronously make and validate requests!
 Home-page: https://github.com/aszabo00/quickbolt
 License: MIT
 Author: Ashton Szabo
 Author-email: aszabo00@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
```

