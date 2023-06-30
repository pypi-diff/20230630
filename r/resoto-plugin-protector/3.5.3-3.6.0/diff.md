# Comparing `tmp/resoto-plugin-protector-3.5.3.tar.gz` & `tmp/resoto-plugin-protector-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-protector-3.5.3.tar", last modified: Wed Jun 21 14:18:11 2023, max compression
+gzip compressed data, was "resoto-plugin-protector-3.6.0.tar", last modified: Fri Jun 30 19:23:25 2023, max compression
```

## Comparing `resoto-plugin-protector-3.5.3.tar` & `resoto-plugin-protector-3.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:11.706483 resoto-plugin-protector-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:15:34.000000 resoto-plugin-protector-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-21 14:18:11.706483 resoto-plugin-protector-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-21 14:15:34.000000 resoto-plugin-protector-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 14:15:34.000000 resoto-plugin-protector-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:11.706483 resoto-plugin-protector-3.5.3/resoto_plugin_protector/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-21 14:15:34.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-21 14:15:34.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:11.706483 resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-21 14:18:11.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-21 14:18:11.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:18:11.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 14:18:11.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:16:36.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 14:18:11.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 14:18:11.000000 resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:18:11.706483 resoto-plugin-protector-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:11.706483 resoto-plugin-protector-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-21 14:15:34.000000 resoto-plugin-protector-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/resoto_plugin_protector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-protector-3.5.3/PKG-INFO` & `resoto-plugin-protector-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Protector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/protector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-protector-3.5.3/README.md` & `resoto-plugin-protector-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.5.3/pyproject.toml` & `resoto-plugin-protector-3.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-protector"
 description = "Resoto Protector Plugin"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3",
+    "resotolib==3.6.0",
 ]
 
 [project.entry-points."resoto.plugins"]
 protector = "resoto_plugin_protector:ProtectorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-protector-3.5.3/resoto_plugin_protector/__init__.py` & `resoto-plugin-protector-3.6.0/resoto_plugin_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.5.3/resoto_plugin_protector/config.py` & `resoto-plugin-protector-3.6.0/resoto_plugin_protector/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.5.3/resoto_plugin_protector.egg-info/PKG-INFO` & `resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Protector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/protector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

