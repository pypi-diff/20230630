# Comparing `tmp/resoto-plugin-cleanup-untagged-3.5.3.tar.gz` & `tmp/resoto-plugin-cleanup-untagged-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-untagged-3.5.3.tar", last modified: Wed Jun 21 14:23:20 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-untagged-3.6.0.tar", last modified: Fri Jun 30 19:28:01 2023, max compression
```

## Comparing `resoto-plugin-cleanup-untagged-3.5.3.tar` & `resoto-plugin-cleanup-untagged-3.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.961998 resoto-plugin-cleanup-untagged-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:18:00.000000 resoto-plugin-cleanup-untagged-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-21 14:23:20.961998 resoto-plugin-cleanup-untagged-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-21 14:18:00.000000 resoto-plugin-cleanup-untagged-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-21 14:18:00.000000 resoto-plugin-cleanup-untagged-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.957998 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-21 14:18:00.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-21 14:18:00.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.961998 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-21 14:23:20.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 14:23:20.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:20.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 14:23:20.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:19:39.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 14:23:20.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 14:23:20.000000 resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:23:20.961998 resoto-plugin-cleanup-untagged-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.961998 resoto-plugin-cleanup-untagged-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-21 14:18:00.000000 resoto-plugin-cleanup-untagged-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:01.255336 resoto-plugin-cleanup-untagged-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:23:42.000000 resoto-plugin-cleanup-untagged-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-30 19:28:01.255336 resoto-plugin-cleanup-untagged-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-30 19:23:42.000000 resoto-plugin-cleanup-untagged-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 19:23:42.000000 resoto-plugin-cleanup-untagged-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:01.255336 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-30 19:23:42.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-30 19:23:42.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:01.255336 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-30 19:28:01.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-30 19:28:01.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:28:01.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 19:28:01.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:25:00.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 19:28:01.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 19:28:01.000000 resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:28:01.255336 resoto-plugin-cleanup-untagged-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:01.255336 resoto-plugin-cleanup-untagged-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-30 19:23:42.000000 resoto-plugin-cleanup-untagged-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-untagged-3.5.3/PKG-INFO` & `resoto-plugin-cleanup-untagged-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-untagged
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Cleanup Untagged Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_untagged
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-untagged-3.5.3/README.md` & `resoto-plugin-cleanup-untagged-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.5.3/pyproject.toml` & `resoto-plugin-cleanup-untagged-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-untagged"
 description = "Resoto Cleanup Untagged Plugin"
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
 cleanup_untagged = "resoto_plugin_cleanup_untagged:CleanupUntaggedPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged/__init__.py` & `resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged/config.py` & `resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO` & `resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-untagged
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Cleanup Untagged Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_untagged
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-untagged-3.5.3/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-untagged-3.6.0/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.5.3/test/test_config.py` & `resoto-plugin-cleanup-untagged-3.6.0/test/test_config.py`

 * *Files identical despite different names*

