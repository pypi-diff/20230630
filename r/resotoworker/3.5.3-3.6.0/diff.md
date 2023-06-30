# Comparing `tmp/resotoworker-3.5.3.tar.gz` & `tmp/resotoworker-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.5.3.tar", last modified: Wed Jun 21 14:25:24 2023, max compression
+gzip compressed data, was "resotoworker-3.6.0.tar", last modified: Fri Jun 30 19:24:16 2023, max compression
```

## Comparing `resotoworker-3.5.3.tar` & `resotoworker-3.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:24.292047 resotoworker-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:21:54.000000 resotoworker-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-21 14:25:24.292047 resotoworker-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-21 14:21:54.000000 resotoworker-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 14:21:54.000000 resotoworker-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:24.288047 resotoworker-3.5.3/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-21 14:21:54.000000 resotoworker-3.5.3/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:24.288047 resotoworker-3.5.3/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:22:56.000000 resotoworker-3.5.3/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:25:24.000000 resotoworker-3.5.3/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:25:24.292047 resotoworker-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:24.292047 resotoworker-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-21 14:21:54.000000 resotoworker-3.5.3/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:16.857830 resotoworker-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:18:37.000000 resotoworker-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-30 19:24:16.857830 resotoworker-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-30 19:18:37.000000 resotoworker-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-30 19:18:37.000000 resotoworker-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:16.853830 resotoworker-3.6.0/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:16.857830 resotoworker-3.6.0/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:20:15.000000 resotoworker-3.6.0/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:24:16.857830 resotoworker-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:16.857830 resotoworker-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/test_utils.py
```

### Comparing `resotoworker-3.5.3/PKG-INFO` & `resotoworker-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.5.3
+Version: 3.6.0
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.5.3/README.md` & `resotoworker-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/pyproject.toml` & `resotoworker-3.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "resotoworker"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3",
+    "resotolib==3.6.0",
     "tenacity",
     "CherryPy",
 ]
 
 [project.scripts]
 resotoworker = "resotoworker.__main__:main"
```

### Comparing `resotoworker-3.5.3/resotoworker/__main__.py` & `resotoworker-3.6.0/resotoworker/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/resotoworker/cleanup.py` & `resotoworker-3.6.0/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/resotoworker/collect.py` & `resotoworker-3.6.0/resotoworker/collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/resotoworker/config.py` & `resotoworker-3.6.0/resotoworker/config.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/resotoworker/pluginloader.py` & `resotoworker-3.6.0/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/resotoworker/resotocore.py` & `resotoworker-3.6.0/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/resotoworker/tag.py` & `resotoworker-3.6.0/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/resotoworker/utils.py` & `resotoworker-3.6.0/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.6.0/resotoworker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.5.3
+Version: 3.6.0
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.5.3/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.6.0/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/test/test_args.py` & `resotoworker-3.6.0/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/test/test_collect.py` & `resotoworker-3.6.0/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/test/test_resotocore.py` & `resotoworker-3.6.0/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.3/test/test_utils.py` & `resotoworker-3.6.0/test/test_utils.py`

 * *Files identical despite different names*

