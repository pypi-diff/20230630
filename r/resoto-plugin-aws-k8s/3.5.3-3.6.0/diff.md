# Comparing `tmp/resoto-plugin-aws-k8s-3.5.3.tar.gz` & `tmp/resoto-plugin-aws-k8s-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-k8s-3.5.3.tar", last modified: Wed Jun 21 14:19:40 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-k8s-3.6.0.tar", last modified: Fri Jun 30 19:23:13 2023, max compression
```

## Comparing `resoto-plugin-aws-k8s-3.5.3.tar` & `resoto-plugin-aws-k8s-3.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:19:40.111903 resoto-plugin-aws-k8s-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:16:06.000000 resoto-plugin-aws-k8s-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-21 14:19:40.111903 resoto-plugin-aws-k8s-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 14:16:06.000000 resoto-plugin-aws-k8s-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-21 14:16:06.000000 resoto-plugin-aws-k8s-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:19:40.111903 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-21 14:16:06.000000 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:19:40.111903 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-21 14:19:40.000000 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-21 14:19:40.000000 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:19:40.000000 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 14:19:40.000000 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:17:09.000000 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 14:19:40.000000 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 14:19:40.000000 resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:19:40.111903 resoto-plugin-aws-k8s-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:19:40.111903 resoto-plugin-aws-k8s-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:06.000000 resoto-plugin-aws-k8s-3.5.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 14:16:06.000000 resoto-plugin-aws-k8s-3.5.3/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:13.233087 resoto-plugin-aws-k8s-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:18:52.000000 resoto-plugin-aws-k8s-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-30 19:23:13.233087 resoto-plugin-aws-k8s-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 19:18:52.000000 resoto-plugin-aws-k8s-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-30 19:18:52.000000 resoto-plugin-aws-k8s-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:13.229087 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-30 19:18:52.000000 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:13.233087 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-30 19:23:13.000000 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 19:23:13.000000 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:23:13.000000 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 19:23:13.000000 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:20:09.000000 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-30 19:23:13.000000 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 19:23:13.000000 resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:23:13.233087 resoto-plugin-aws-k8s-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:13.233087 resoto-plugin-aws-k8s-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:18:52.000000 resoto-plugin-aws-k8s-3.6.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 19:18:52.000000 resoto-plugin-aws-k8s-3.6.0/test/test_collector.py
```

### Comparing `resoto-plugin-aws-k8s-3.5.3/PKG-INFO` & `resoto-plugin-aws-k8s-3.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto AWS-K8s Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
 Keywords: aws,k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,12 +15,12 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: test
 
 # resoto-plugin-aws-k8s
 AWS - K8s Collector Plugin for Resoto: link together your AWS and k8s cluster resources.
```

### Comparing `resoto-plugin-aws-k8s-3.5.3/pyproject.toml` & `resoto-plugin-aws-k8s-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-aws-k8s"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 description = "Resoto AWS-K8s Collector Plugin"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,18 +23,18 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["aws", "k8s"]
 
-dependencies = [ "resotolib==3.5.3" ]
+dependencies = [ "resotolib==3.6.0" ]
 
 [project.optional-dependencies]
-dev = [ "mypy" ]
+test = [ "mypy" ]
 
 [project.entry-points."resoto.plugins"]
 aws_k8s_collector = "resoto_plugin_aws_k8s:AWSK8sCollectorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
 Source = "https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s"
```

### Comparing `resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s/__init__.py` & `resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-k8s-3.5.3/resoto_plugin_aws_k8s.egg-info/PKG-INFO` & `resoto-plugin-aws-k8s-3.6.0/resoto_plugin_aws_k8s.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto AWS-K8s Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
 Keywords: aws,k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,12 +15,12 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: test
 
 # resoto-plugin-aws-k8s
 AWS - K8s Collector Plugin for Resoto: link together your AWS and k8s cluster resources.
```

### Comparing `resoto-plugin-aws-k8s-3.5.3/test/test_collector.py` & `resoto-plugin-aws-k8s-3.6.0/test/test_collector.py`

 * *Files identical despite different names*

