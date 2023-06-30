# Comparing `tmp/resoto-plugin-vsphere-3.5.3.tar.gz` & `tmp/resoto-plugin-vsphere-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-vsphere-3.5.3.tar", last modified: Wed Jun 21 14:23:30 2023, max compression
+gzip compressed data, was "resoto-plugin-vsphere-3.6.0.tar", last modified: Fri Jun 30 19:28:33 2023, max compression
```

## Comparing `resoto-plugin-vsphere-3.5.3.tar` & `resoto-plugin-vsphere-3.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:30.375248 resoto-plugin-vsphere-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:20:54.000000 resoto-plugin-vsphere-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-21 14:23:30.375248 resoto-plugin-vsphere-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 14:20:54.000000 resoto-plugin-vsphere-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-21 14:20:54.000000 resoto-plugin-vsphere-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:30.375248 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-21 14:20:54.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-21 14:20:54.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-21 14:20:54.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-21 14:20:54.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/vsphere_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:30.375248 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-21 14:23:30.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-21 14:23:30.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:30.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 14:23:30.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:56.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 14:23:30.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 14:23:30.000000 resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:23:30.375248 resoto-plugin-vsphere-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:30.375248 resoto-plugin-vsphere-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 14:20:54.000000 resoto-plugin-vsphere-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:33.311132 resoto-plugin-vsphere-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:29.000000 resoto-plugin-vsphere-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-30 19:28:33.311132 resoto-plugin-vsphere-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 19:24:29.000000 resoto-plugin-vsphere-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-30 19:24:29.000000 resoto-plugin-vsphere-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:33.311132 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-30 19:24:29.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-30 19:24:29.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-30 19:24:29.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-30 19:24:29.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/vsphere_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:33.311132 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-30 19:28:33.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-30 19:28:33.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:28:33.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 19:28:33.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:26:04.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 19:28:33.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 19:28:33.000000 resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:28:33.315132 resoto-plugin-vsphere-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:28:33.311132 resoto-plugin-vsphere-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 19:24:29.000000 resoto-plugin-vsphere-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-vsphere-3.5.3/PKG-INFO` & `resoto-plugin-vsphere-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-vsphere
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto VSphere Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/vsphere
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-vsphere-3.5.3/pyproject.toml` & `resoto-plugin-vsphere-3.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-vsphere"
 description = "Resoto VSphere Collector Plugin"
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
     "pyvmomi",
 ]
 
 [project.entry-points."resoto.plugins"]
 vsphere = "resoto_plugin_vsphere:VSphereCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/__init__.py` & `resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/config.py` & `resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/resources.py` & `resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere/vsphere_client.py` & `resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere/vsphere_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/PKG-INFO` & `resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-vsphere
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto VSphere Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/vsphere
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-vsphere-3.5.3/resoto_plugin_vsphere.egg-info/SOURCES.txt` & `resoto-plugin-vsphere-3.6.0/resoto_plugin_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

