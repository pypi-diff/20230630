# Comparing `tmp/resoto-plugin-cleanup-expired-3.5.3.tar.gz` & `tmp/resoto-plugin-cleanup-expired-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-expired-3.5.3.tar", last modified: Wed Jun 21 14:21:53 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-expired-3.6.0.tar", last modified: Fri Jun 30 19:27:23 2023, max compression
```

## Comparing `resoto-plugin-cleanup-expired-3.5.3.tar` & `resoto-plugin-cleanup-expired-3.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:53.191947 resoto-plugin-cleanup-expired-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:19:14.000000 resoto-plugin-cleanup-expired-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-21 14:21:53.191947 resoto-plugin-cleanup-expired-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-21 14:19:14.000000 resoto-plugin-cleanup-expired-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-21 14:19:14.000000 resoto-plugin-cleanup-expired-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:53.191947 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-21 14:19:14.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 14:19:14.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:53.191947 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-21 14:21:53.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 14:21:53.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:53.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 14:21:53.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:20:17.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 14:21:53.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 14:21:53.000000 resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:21:53.191947 resoto-plugin-cleanup-expired-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:21:53.191947 resoto-plugin-cleanup-expired-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-21 14:19:14.000000 resoto-plugin-cleanup-expired-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:23.698681 resoto-plugin-cleanup-expired-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:04.000000 resoto-plugin-cleanup-expired-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-30 19:27:23.698681 resoto-plugin-cleanup-expired-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 19:24:04.000000 resoto-plugin-cleanup-expired-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-30 19:24:04.000000 resoto-plugin-cleanup-expired-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:23.698681 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-30 19:24:04.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-30 19:24:04.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:23.698681 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-30 19:27:23.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 19:27:23.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:27:23.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 19:27:23.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:25:21.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 19:27:23.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-30 19:27:23.000000 resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:27:23.698681 resoto-plugin-cleanup-expired-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:23.698681 resoto-plugin-cleanup-expired-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-30 19:24:04.000000 resoto-plugin-cleanup-expired-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-expired-3.5.3/PKG-INFO` & `resoto-plugin-cleanup-expired-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-expired
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Expired Resource Cleanup Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-expired-3.5.3/README.md` & `resoto-plugin-cleanup-expired-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.5.3/pyproject.toml` & `resoto-plugin-cleanup-expired-3.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-expired"
 description = "Resoto Expired Resource Cleanup Plugin"
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
 cleanup_expired = "resoto_plugin_cleanup_expired:CleanupExpiredPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired/__init__.py` & `resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/PKG-INFO` & `resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-expired
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Expired Resource Cleanup Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-expired-3.5.3/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-expired-3.6.0/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt`

 * *Files identical despite different names*

