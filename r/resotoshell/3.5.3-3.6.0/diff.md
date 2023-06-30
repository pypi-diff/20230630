# Comparing `tmp/resotoshell-3.5.3.tar.gz` & `tmp/resotoshell-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.5.3.tar", last modified: Wed Jun 21 14:21:48 2023, max compression
+gzip compressed data, was "resotoshell-3.6.0.tar", last modified: Fri Jun 30 19:29:51 2023, max compression
```

## Comparing `resotoshell-3.5.3.tar` & `resotoshell-3.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:48.309282 resotoshell-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:17:48.000000 resotoshell-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-21 14:21:48.309282 resotoshell-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-21 14:17:48.000000 resotoshell-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-21 14:17:48.000000 resotoshell-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:48.305282 resotoshell-3.5.3/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/authorized_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37345 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-21 14:17:48.000000 resotoshell-3.5.3/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:48.309282 resotoshell-3.5.3/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:19:00.000000 resotoshell-3.5.3/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 14:21:48.000000 resotoshell-3.5.3/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 14:21:48.309282 resotoshell-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:48.309282 resotoshell-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-21 14:17:48.000000 resotoshell-3.5.3/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-06-21 14:17:48.000000 resotoshell-3.5.3/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-21 14:17:48.000000 resotoshell-3.5.3/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:51.858892 resotoshell-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:48.000000 resotoshell-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-30 19:29:51.858892 resotoshell-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-30 19:24:48.000000 resotoshell-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-30 19:24:48.000000 resotoshell-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:51.858892 resotoshell-3.6.0/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37345 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:51.858892 resotoshell-3.6.0/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:26:19.000000 resotoshell-3.6.0/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 19:29:51.858892 resotoshell-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:51.858892 resotoshell-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 19:24:48.000000 resotoshell-3.6.0/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-06-30 19:24:48.000000 resotoshell-3.6.0/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-30 19:24:48.000000 resotoshell-3.6.0/test/test_protected_files.py
```

### Comparing `resotoshell-3.5.3/PKG-INFO` & `resotoshell-3.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.5.3
+Version: 3.6.0
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.5.3/README.md` & `resotoshell-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.3/pyproject.toml` & `resotoshell-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotoshell"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 description = "Commandline interpreter to interact with Resoto."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -24,15 +24,15 @@
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["cloud security"]
 
 dependencies = [
-    "resotolib==3.5.3",
+    "resotolib==3.6.0",
     "prompt-toolkit",
     "rich",
     "resotoclient",
     "aiohttp[speedups]",
 ]
 
 [project.scripts]
```

### Comparing `resotoshell-3.5.3/resotoshell/__main__.py` & `resotoshell-3.6.0/resotoshell/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.3/resotoshell/authorized_client.py` & `resotoshell-3.6.0/resotoshell/authorized_client.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.3/resotoshell/promptsession.py` & `resotoshell-3.6.0/resotoshell/promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.3/resotoshell/protected_files.py` & `resotoshell-3.6.0/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.3/resotoshell/shell.py` & `resotoshell-3.6.0/resotoshell/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os.path
 import re
 import shutil
 import sys
+from pathlib import Path
 from subprocess import call
 from tempfile import TemporaryDirectory
 from typing import Dict, Union, Optional, Tuple
 from urllib import parse
 from urllib.parse import urlsplit
 
 import aiohttp
@@ -131,20 +132,26 @@
     async def handle_result(
         self,
         response: Union[HttpResponse, aiohttp.BodyPartReader, aiohttp.MultipartReader],
         first: bool = True,
     ) -> None:
         # store the file from the part inside the given directory
         async def store_file(response: Union[HttpResponse, aiohttp.BodyPartReader], directory: str) -> Tuple[str, str]:
-            disposition = response.headers.get("Content-Disposition", "")
-            match = re.findall('filename="([^"]+)"', disposition)
-            filename = parse.unquote(match[0]) if match else "out"
-            if "/" in filename:
-                raise ValueError(f"Invalid filename: {filename}")
-            filepath = os.path.join(directory, filename)
+            if (filepath := response.headers.get("file-path")) is not None:
+                path = Path(filepath).expanduser().absolute()
+                filepath = str(path)
+                filename = path.name
+            else:  # fall back to content-disposition
+                disposition = response.headers.get("Content-Disposition", "")
+                match = re.findall('filename="([^"]+)"', disposition)
+                filename = parse.unquote(match[0]) if match else "out"
+                if "/" in filename:
+                    raise ValueError(f"Invalid filename: {filename}")
+                filepath = os.path.join(directory, filename)
+            Path(filepath).parent.mkdir(parents=True, exist_ok=True)
             with open(filepath, "wb+") as fh:
                 if isinstance(response, HttpResponse):
                     content = await response.payload_bytes()
                 else:
                     content = await response.read()
                 fh.write(content)
             return filename, filepath
```

### Comparing `resotoshell-3.5.3/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.6.0/resotoshell.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.5.3
+Version: 3.6.0
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.5.3/resotoshell.egg-info/SOURCES.txt` & `resotoshell-3.6.0/resotoshell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.3/test/test_promptsession.py` & `resotoshell-3.6.0/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.3/test/test_protected_files.py` & `resotoshell-3.6.0/test/test_protected_files.py`

 * *Files identical despite different names*

