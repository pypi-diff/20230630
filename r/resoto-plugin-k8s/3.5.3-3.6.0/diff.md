# Comparing `tmp/resoto-plugin-k8s-3.5.3.tar.gz` & `tmp/resoto-plugin-k8s-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-k8s-3.5.3.tar", last modified: Wed Jun 21 14:27:11 2023, max compression
+gzip compressed data, was "resoto-plugin-k8s-3.6.0.tar", last modified: Fri Jun 30 19:29:03 2023, max compression
```

## Comparing `resoto-plugin-k8s-3.5.3.tar` & `resoto-plugin-k8s-3.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:11.494304 resoto-plugin-k8s-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:22:16.000000 resoto-plugin-k8s-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-21 14:27:11.494304 resoto-plugin-k8s-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:22:16.000000 resoto-plugin-k8s-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-21 14:22:16.000000 resoto-plugin-k8s-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:11.494304 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-21 14:22:16.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-06-21 14:22:16.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-21 14:22:16.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-06-21 14:22:16.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:11.494304 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-21 14:27:11.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-21 14:27:11.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:27:11.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-21 14:27:11.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:40.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 14:27:11.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:27:11.000000 resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 14:27:11.494304 resoto-plugin-k8s-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:25:36.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/setup.cfg
```

### Comparing `resoto-plugin-k8s-3.5.3/PKG-INFO` & `resoto-plugin-k8s-3.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.5.3/pyproject.toml` & `resoto-plugin-k8s-3.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-k8s"
 description = "Resoto Kubernetes Collector Plugin"
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
     "kubernetes",
 ]
 
 [project.entry-points."resoto.plugins"]
 k8s_collector = "resoto_plugin_k8s:KubernetesCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/__init__.py` & `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/base.py` & `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/collector.py` & `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.3/resoto_plugin_k8s/resources.py` & `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.3/resoto_plugin_k8s.egg-info/PKG-INFO` & `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

