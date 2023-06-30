# Comparing `tmp/resoto-plugin-digitalocean-k8s-3.5.3.tar.gz` & `tmp/resoto-plugin-digitalocean-k8s-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.5.3.tar", last modified: Wed Jun 21 14:20:56 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.6.0.tar", last modified: Fri Jun 30 19:27:26 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-k8s-3.5.3.tar` & `resoto-plugin-digitalocean-k8s-3.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:56.545241 resoto-plugin-digitalocean-k8s-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:17:13.000000 resoto-plugin-digitalocean-k8s-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-21 14:20:56.545241 resoto-plugin-digitalocean-k8s-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 14:17:13.000000 resoto-plugin-digitalocean-k8s-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-21 14:17:13.000000 resoto-plugin-digitalocean-k8s-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:56.541242 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-21 14:17:13.000000 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:56.545241 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-21 14:20:56.000000 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-21 14:20:56.000000 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:20:56.000000 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 14:20:56.000000 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:18:19.000000 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 14:20:56.000000 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 14:20:56.000000 resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:20:56.545241 resoto-plugin-digitalocean-k8s-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:56.545241 resoto-plugin-digitalocean-k8s-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:17:13.000000 resoto-plugin-digitalocean-k8s-3.5.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-21 14:17:13.000000 resoto-plugin-digitalocean-k8s-3.5.3/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:26.413824 resoto-plugin-digitalocean-k8s-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:22:21.000000 resoto-plugin-digitalocean-k8s-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-30 19:27:26.413824 resoto-plugin-digitalocean-k8s-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-30 19:22:21.000000 resoto-plugin-digitalocean-k8s-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-30 19:22:21.000000 resoto-plugin-digitalocean-k8s-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:26.409824 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-30 19:22:21.000000 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:26.413824 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-30 19:27:26.000000 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-30 19:27:26.000000 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:27:26.000000 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 19:27:26.000000 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:23:53.000000 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-30 19:27:26.000000 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-30 19:27:26.000000 resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:27:26.413824 resoto-plugin-digitalocean-k8s-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:26.413824 resoto-plugin-digitalocean-k8s-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:21.000000 resoto-plugin-digitalocean-k8s-3.6.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-30 19:22:21.000000 resoto-plugin-digitalocean-k8s-3.6.0/test/test_collector.py
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.3/PKG-INFO` & `resoto-plugin-digitalocean-k8s-3.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean-k8s
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto DigitalOcean-K8s Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean_k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -14,12 +14,12 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: test
 
 # resoto-plugin-digitalocean-k8s
 DigitalOcean - K8s Collector Plugin for Resoto: link together your k8s cluster resources with DigitalOcean.
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.3/pyproject.toml` & `resoto-plugin-digitalocean-k8s-3.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-digitalocean-k8s"
 description = "Resoto DigitalOcean-K8s Collector Plugin"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,21 +23,19 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3",
+    "resotolib==3.6.0",
 ]
 
 [project.optional-dependencies]
-dev = [
-    "mypy",
-]
+test = [ "mypy" ]
 
 [project.entry-points."resoto.plugins"]
 digitalocean_k8s_collector = "resoto_plugin_digitalocean_k8s:DigitalOceanK8sCollectorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
 Source = "https://github.com/someengineering/resoto/tree/main/plugins/digitalocean_k8s"
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s/__init__.py` & `resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-k8s-3.5.3/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-k8s-3.6.0/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean-k8s
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto DigitalOcean-K8s Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean_k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -14,12 +14,12 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: test
 
 # resoto-plugin-digitalocean-k8s
 DigitalOcean - K8s Collector Plugin for Resoto: link together your k8s cluster resources with DigitalOcean.
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.3/test/test_collector.py` & `resoto-plugin-digitalocean-k8s-3.6.0/test/test_collector.py`

 * *Files identical despite different names*

