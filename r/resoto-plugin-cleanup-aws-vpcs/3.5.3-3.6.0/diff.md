# Comparing `tmp/resoto-plugin-cleanup-aws-vpcs-3.5.3.tar.gz` & `tmp/resoto-plugin-cleanup-aws-vpcs-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.5.3.tar", last modified: Wed Jun 21 14:23:29 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.6.0.tar", last modified: Fri Jun 30 19:22:47 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.3.tar` & `resoto-plugin-cleanup-aws-vpcs-3.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:29.336458 resoto-plugin-cleanup-aws-vpcs-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:20:24.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-21 14:23:29.336458 resoto-plugin-cleanup-aws-vpcs-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 14:20:24.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 14:20:24.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:29.332458 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-21 14:20:24.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-21 14:20:24.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:29.336458 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-21 14:23:29.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 14:23:29.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:29.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 14:23:29.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:21:42.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 14:23:29.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 14:23:29.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:23:29.336458 resoto-plugin-cleanup-aws-vpcs-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:29.336458 resoto-plugin-cleanup-aws-vpcs-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 14:20:24.000000 resoto-plugin-cleanup-aws-vpcs-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:47.121888 resoto-plugin-cleanup-aws-vpcs-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:19:09.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-30 19:22:47.121888 resoto-plugin-cleanup-aws-vpcs-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-30 19:19:09.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-30 19:19:09.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:47.121888 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-30 19:19:09.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-30 19:19:09.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:47.121888 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-30 19:22:47.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-30 19:22:47.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:22:47.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 19:22:47.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:20:39.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-30 19:22:47.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 19:22:47.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:22:47.121888 resoto-plugin-cleanup-aws-vpcs-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:47.121888 resoto-plugin-cleanup-aws-vpcs-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 19:19:09.000000 resoto-plugin-cleanup-aws-vpcs-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.3/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.5.3
+Version: 3.6.0
 Summary: AWS VPC Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.3/README.md` & `resoto-plugin-cleanup-aws-vpcs-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.3/pyproject.toml` & `resoto-plugin-cleanup-aws-vpcs-3.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-aws-vpcs"
 description = "AWS VPC Cleaner Plugin"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,16 +23,16 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3",
-    "resoto-plugin-aws==3.5.3"
+    "resotolib==3.6.0",
+    "resoto-plugin-aws==3.6.0"
 ]
 
 [project.entry-points."resoto.plugins"]
 cleanup_aws_vpcs = "resoto_plugin_cleanup_aws_vpcs:CleanupAWSVPCsPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs/__init__.py` & `resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs/config.py` & `resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.5.3
+Version: 3.6.0
 Summary: AWS VPC Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.5.3/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-vpcs-3.6.0/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

