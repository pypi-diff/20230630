# Comparing `tmp/resoto-plugin-cleanup-volumes-3.5.3.tar.gz` & `tmp/resoto-plugin-cleanup-volumes-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-volumes-3.5.3.tar", last modified: Wed Jun 21 14:20:00 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-volumes-3.6.0.tar", last modified: Fri Jun 30 19:28:22 2023, max compression
```

## Comparing `resoto-plugin-cleanup-volumes-3.5.3.tar` & `resoto-plugin-cleanup-volumes-3.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:00.845930 resoto-plugin-cleanup-volumes-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:17:24.000000 resoto-plugin-cleanup-volumes-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-21 14:20:00.845930 resoto-plugin-cleanup-volumes-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-21 14:17:24.000000 resoto-plugin-cleanup-volumes-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-21 14:17:24.000000 resoto-plugin-cleanup-volumes-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:00.845930 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-21 14:17:24.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-21 14:17:24.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:00.845930 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-21 14:20:00.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 14:20:00.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:20:00.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 14:20:00.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:18:28.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 14:20:00.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 14:20:00.000000 resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:20:00.845930 resoto-plugin-cleanup-volumes-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:00.845930 resoto-plugin-cleanup-volumes-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-21 14:17:24.000000 resoto-plugin-cleanup-volumes-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:22.804365 resoto-plugin-cleanup-volumes-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:25:10.000000 resoto-plugin-cleanup-volumes-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-30 19:28:22.804365 resoto-plugin-cleanup-volumes-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-30 19:25:10.000000 resoto-plugin-cleanup-volumes-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-30 19:25:10.000000 resoto-plugin-cleanup-volumes-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:22.800365 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-30 19:25:10.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-30 19:25:10.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:22.804365 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-30 19:28:22.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 19:28:22.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:28:22.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 19:28:22.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:26:25.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 19:28:22.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-30 19:28:22.000000 resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:28:22.804365 resoto-plugin-cleanup-volumes-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:22.804365 resoto-plugin-cleanup-volumes-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 19:25:10.000000 resoto-plugin-cleanup-volumes-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-volumes-3.5.3/PKG-INFO` & `resoto-plugin-cleanup-volumes-3.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-volumes
-Version: 3.5.3
+Version: 3.6.0
 Summary: Volume Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-volumes-3.5.3/README.md` & `resoto-plugin-cleanup-volumes-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.5.3/pyproject.toml` & `resoto-plugin-cleanup-volumes-3.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-volumes"
 description = "Volume Cleaner Plugin"
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
 cleanup_volumes = "resoto_plugin_cleanup_volumes:CleanupVolumesPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes/__init__.py` & `resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes/config.py` & `resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO` & `resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-volumes
-Version: 3.5.3
+Version: 3.6.0
 Summary: Volume Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-volumes-3.5.3/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-volumes-3.6.0/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

