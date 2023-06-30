# Comparing `tmp/resoto-plugin-github-3.5.3.tar.gz` & `tmp/resoto-plugin-github-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-github-3.5.3.tar", last modified: Wed Jun 21 14:23:11 2023, max compression
+gzip compressed data, was "resoto-plugin-github-3.6.0.tar", last modified: Fri Jun 30 19:27:56 2023, max compression
```

## Comparing `resoto-plugin-github-3.5.3.tar` & `resoto-plugin-github-3.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:11.942977 resoto-plugin-github-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:20:35.000000 resoto-plugin-github-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-21 14:23:11.942977 resoto-plugin-github-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 14:20:35.000000 resoto-plugin-github-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-21 14:20:35.000000 resoto-plugin-github-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:11.942977 resoto-plugin-github-3.5.3/resoto_plugin_github/
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-21 14:20:35.000000 resoto-plugin-github-3.5.3/resoto_plugin_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-21 14:20:35.000000 resoto-plugin-github-3.5.3/resoto_plugin_github/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-21 14:20:35.000000 resoto-plugin-github-3.5.3/resoto_plugin_github/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:11.942977 resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-21 14:23:11.000000 resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 14:23:11.000000 resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:11.000000 resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 14:23:11.000000 resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:37.000000 resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 14:23:11.000000 resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 14:23:11.000000 resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:23:11.942977 resoto-plugin-github-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:11.942977 resoto-plugin-github-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 14:20:35.000000 resoto-plugin-github-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:56.918284 resoto-plugin-github-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:23.000000 resoto-plugin-github-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-30 19:27:56.918284 resoto-plugin-github-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 19:24:23.000000 resoto-plugin-github-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-30 19:24:23.000000 resoto-plugin-github-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:56.918284 resoto-plugin-github-3.6.0/resoto_plugin_github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-30 19:24:23.000000 resoto-plugin-github-3.6.0/resoto_plugin_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-30 19:24:23.000000 resoto-plugin-github-3.6.0/resoto_plugin_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-30 19:24:23.000000 resoto-plugin-github-3.6.0/resoto_plugin_github/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:56.918284 resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-30 19:27:56.000000 resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-30 19:27:56.000000 resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:27:56.000000 resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 19:27:56.000000 resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:25:46.000000 resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 19:27:56.000000 resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 19:27:56.000000 resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:27:56.918284 resoto-plugin-github-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:56.918284 resoto-plugin-github-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-30 19:24:23.000000 resoto-plugin-github-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-github-3.5.3/PKG-INFO` & `resoto-plugin-github-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Github Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/github
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-github-3.5.3/pyproject.toml` & `resoto-plugin-github-3.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-github"
 description = "Resoto Github Collector Plugin"
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
     "PyGithub",
 ]
 
 [project.entry-points."resoto.plugins"]
 github = "resoto_plugin_github:GithubCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-github-3.5.3/resoto_plugin_github/__init__.py` & `resoto-plugin-github-3.6.0/resoto_plugin_github/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.5.3/resoto_plugin_github/config.py` & `resoto-plugin-github-3.6.0/resoto_plugin_github/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.5.3/resoto_plugin_github/resources.py` & `resoto-plugin-github-3.6.0/resoto_plugin_github/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.5.3/resoto_plugin_github.egg-info/PKG-INFO` & `resoto-plugin-github-3.6.0/resoto_plugin_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Github Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/github
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

