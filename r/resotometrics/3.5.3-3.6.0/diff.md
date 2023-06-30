# Comparing `tmp/resotometrics-3.5.3.tar.gz` & `tmp/resotometrics-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotometrics-3.5.3.tar", last modified: Wed Jun 21 14:22:25 2023, max compression
+gzip compressed data, was "resotometrics-3.6.0.tar", last modified: Fri Jun 30 19:21:23 2023, max compression
```

## Comparing `resotometrics-3.5.3.tar` & `resotometrics-3.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:25.465724 resotometrics-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 14:19:46.000000 resotometrics-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-21 14:22:25.465724 resotometrics-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-21 14:19:46.000000 resotometrics-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-21 14:19:46.000000 resotometrics-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:25.465724 resotometrics-3.5.3/resotometrics/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-21 14:19:46.000000 resotometrics-3.5.3/resotometrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-21 14:19:46.000000 resotometrics-3.5.3/resotometrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-21 14:19:46.000000 resotometrics-3.5.3/resotometrics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-06-21 14:19:46.000000 resotometrics-3.5.3/resotometrics/default_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-21 14:19:46.000000 resotometrics-3.5.3/resotometrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-21 14:19:46.000000 resotometrics-3.5.3/resotometrics/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:25.465724 resotometrics-3.5.3/resotometrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-21 14:22:25.000000 resotometrics-3.5.3/resotometrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 14:22:25.000000 resotometrics-3.5.3/resotometrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:22:25.000000 resotometrics-3.5.3/resotometrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 14:22:25.000000 resotometrics-3.5.3/resotometrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:20:50.000000 resotometrics-3.5.3/resotometrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 14:22:25.000000 resotometrics-3.5.3/resotometrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 14:22:25.000000 resotometrics-3.5.3/resotometrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:22:25.465724 resotometrics-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:25.465724 resotometrics-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 14:19:46.000000 resotometrics-3.5.3/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:23.156855 resotometrics-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 19:17:36.000000 resotometrics-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-30 19:21:23.156855 resotometrics-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-30 19:17:36.000000 resotometrics-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-30 19:17:36.000000 resotometrics-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:23.156855 resotometrics-3.6.0/resotometrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-30 19:17:36.000000 resotometrics-3.6.0/resotometrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-30 19:17:36.000000 resotometrics-3.6.0/resotometrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-30 19:17:36.000000 resotometrics-3.6.0/resotometrics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-06-30 19:17:36.000000 resotometrics-3.6.0/resotometrics/default_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-30 19:17:36.000000 resotometrics-3.6.0/resotometrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-30 19:17:36.000000 resotometrics-3.6.0/resotometrics/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:23.156855 resotometrics-3.6.0/resotometrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-30 19:21:23.000000 resotometrics-3.6.0/resotometrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-30 19:21:23.000000 resotometrics-3.6.0/resotometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:23.000000 resotometrics-3.6.0/resotometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 19:21:23.000000 resotometrics-3.6.0/resotometrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:19:15.000000 resotometrics-3.6.0/resotometrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 19:21:23.000000 resotometrics-3.6.0/resotometrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 19:21:23.000000 resotometrics-3.6.0/resotometrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:21:23.156855 resotometrics-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:23.156855 resotometrics-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-30 19:17:36.000000 resotometrics-3.6.0/test/test_args.py
```

### Comparing `resotometrics-3.5.3/PKG-INFO` & `resotometrics-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.5.3
+Version: 3.6.0
 Summary: Exports Resoto metrics in Prometheus format.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotometrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.5.3/README.md` & `resotometrics-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.3/pyproject.toml` & `resotometrics-3.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotometrics"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 description = "Exports Resoto metrics in Prometheus format."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3"
+    "resotolib==3.6.0"
 ]
 
 [pyproject.optional-dependencies]
 test = ["pytest"]
 
 [project.scripts]
 resotometrics = "resotometrics.__main__:main"
```

### Comparing `resotometrics-3.5.3/resotometrics/__main__.py` & `resotometrics-3.6.0/resotometrics/__main__.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.3/resotometrics/config.py` & `resotometrics-3.6.0/resotometrics/config.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.3/resotometrics/default_metrics.yaml` & `resotometrics-3.6.0/resotometrics/default_metrics.yaml`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.3/resotometrics/metrics.py` & `resotometrics-3.6.0/resotometrics/metrics.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.3/resotometrics/search.py` & `resotometrics-3.6.0/resotometrics/search.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.3/resotometrics.egg-info/PKG-INFO` & `resotometrics-3.6.0/resotometrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.5.3
+Version: 3.6.0
 Summary: Exports Resoto metrics in Prometheus format.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotometrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.5.3/test/test_args.py` & `resotometrics-3.6.0/test/test_args.py`

 * *Files identical despite different names*

