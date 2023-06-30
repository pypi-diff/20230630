# Comparing `tmp/resoto-plugin-posthog-3.5.3.tar.gz` & `tmp/resoto-plugin-posthog-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-posthog-3.5.3.tar", last modified: Wed Jun 21 14:23:00 2023, max compression
+gzip compressed data, was "resoto-plugin-posthog-3.6.0.tar", last modified: Fri Jun 30 19:23:33 2023, max compression
```

## Comparing `resoto-plugin-posthog-3.5.3.tar` & `resoto-plugin-posthog-3.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:00.761735 resoto-plugin-posthog-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:20:05.000000 resoto-plugin-posthog-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-21 14:23:00.761735 resoto-plugin-posthog-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-21 14:20:05.000000 resoto-plugin-posthog-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-21 14:20:05.000000 resoto-plugin-posthog-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:00.761735 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-21 14:20:05.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 14:20:05.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-21 14:20:05.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-21 14:20:05.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:00.761735 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-21 14:23:00.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-21 14:23:00.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:00.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 14:23:00.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:21.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 14:23:00.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 14:23:00.000000 resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:23:00.761735 resoto-plugin-posthog-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:00.761735 resoto-plugin-posthog-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 14:20:05.000000 resoto-plugin-posthog-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:33.108103 resoto-plugin-posthog-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:20:19.000000 resoto-plugin-posthog-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-30 19:23:33.108103 resoto-plugin-posthog-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 19:20:19.000000 resoto-plugin-posthog-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 19:20:19.000000 resoto-plugin-posthog-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:33.104103 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-30 19:20:19.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 19:20:19.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-30 19:20:19.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-30 19:20:19.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:33.108103 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-30 19:23:33.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-30 19:23:33.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:23:33.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 19:23:33.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:35.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 19:23:33.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 19:23:33.000000 resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:23:33.108103 resoto-plugin-posthog-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:33.108103 resoto-plugin-posthog-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-30 19:20:19.000000 resoto-plugin-posthog-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-posthog-3.5.3/PKG-INFO` & `resoto-plugin-posthog-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Posthog Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/posthog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.5.3/README.md` & `resoto-plugin-posthog-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.5.3/pyproject.toml` & `resoto-plugin-posthog-3.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-posthog"
 description = "Resoto Posthog Collector Plugin"
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
     "requests",
 ]
 
 [project.entry-points."resoto.plugins"]
 posthog = "resoto_plugin_posthog:PosthogCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-posthog-3.5.3/resoto_plugin_posthog/__init__.py` & `resoto-plugin-posthog-3.6.0/resoto_plugin_posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.5.3/resoto_plugin_posthog/posthog.py` & `resoto-plugin-posthog-3.6.0/resoto_plugin_posthog/posthog.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.5.3/resoto_plugin_posthog/resources.py` & `resoto-plugin-posthog-3.6.0/resoto_plugin_posthog/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/PKG-INFO` & `resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Posthog Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/posthog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.5.3/resoto_plugin_posthog.egg-info/SOURCES.txt` & `resoto-plugin-posthog-3.6.0/resoto_plugin_posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

