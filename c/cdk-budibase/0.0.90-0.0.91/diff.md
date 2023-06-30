# Comparing `tmp/cdk-budibase-0.0.90.tar.gz` & `tmp/cdk-budibase-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-budibase-0.0.90.tar", last modified: Thu Jun 29 00:20:52 2023, max compression
+gzip compressed data, was "cdk-budibase-0.0.91.tar", last modified: Fri Jun 30 00:21:00 2023, max compression
```

## Comparing `cdk-budibase-0.0.90.tar` & `cdk-budibase-0.0.91.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:52.433154 cdk-budibase-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-29 00:20:52.433154 cdk-budibase-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 00:20:52.433154 cdk-budibase-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:52.429154 cdk-budibase-0.0.90/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:52.433154 cdk-budibase-0.0.90/src/cdk_budibase/
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/src/cdk_budibase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:52.433154 cdk-budibase-0.0.90/src/cdk_budibase/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/src/cdk_budibase/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   486657 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/src/cdk_budibase/_jsii/cdk-budibase@0.0.90.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:20:33.000000 cdk-budibase-0.0.90/src/cdk_budibase/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:52.433154 cdk-budibase-0.0.90/src/cdk_budibase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-29 00:20:52.000000 cdk-budibase-0.0.90/src/cdk_budibase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 00:20:52.000000 cdk-budibase-0.0.90/src/cdk_budibase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:20:52.000000 cdk-budibase-0.0.90/src/cdk_budibase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 00:20:52.000000 cdk-budibase-0.0.90/src/cdk_budibase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 00:20:52.000000 cdk-budibase-0.0.90/src/cdk_budibase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:21:00.460042 cdk-budibase-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-30 00:21:00.460042 cdk-budibase-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 00:21:00.460042 cdk-budibase-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:21:00.456042 cdk-budibase-0.0.91/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:21:00.460042 cdk-budibase-0.0.91/src/cdk_budibase/
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/src/cdk_budibase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:21:00.460042 cdk-budibase-0.0.91/src/cdk_budibase/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/src/cdk_budibase/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   486659 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/src/cdk_budibase/_jsii/cdk-budibase@0.0.91.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:20:44.000000 cdk-budibase-0.0.91/src/cdk_budibase/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:21:00.460042 cdk-budibase-0.0.91/src/cdk_budibase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-30 00:21:00.000000 cdk-budibase-0.0.91/src/cdk_budibase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-30 00:21:00.000000 cdk-budibase-0.0.91/src/cdk_budibase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:21:00.000000 cdk-budibase-0.0.91/src/cdk_budibase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 00:21:00.000000 cdk-budibase-0.0.91/src/cdk_budibase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 00:21:00.000000 cdk-budibase-0.0.91/src/cdk_budibase.egg-info/top_level.txt
```

### Comparing `cdk-budibase-0.0.90/LICENSE` & `cdk-budibase-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-budibase-0.0.90/PKG-INFO` & `cdk-budibase-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-budibase
-Version: 0.0.90
+Version: 0.0.91
 Summary: Use AWS CDK to create budibase server
 Home-page: https://github.com/neilkuan/cdk-budibase.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-budibase.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-budibase-0.0.90/README.md` & `cdk-budibase-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `cdk-budibase-0.0.90/setup.py` & `cdk-budibase-0.0.91/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-budibase",
-    "version": "0.0.90",
+    "version": "0.0.91",
     "description": "Use AWS CDK to create budibase server",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-budibase.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_budibase",
         "cdk_budibase._jsii"
     ],
     "package_data": {
         "cdk_budibase._jsii": [
-            "cdk-budibase@0.0.90.jsii.tgz"
+            "cdk-budibase@0.0.91.jsii.tgz"
         ],
         "cdk_budibase": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-budibase-0.0.90/src/cdk_budibase/__init__.py` & `cdk-budibase-0.0.91/src/cdk_budibase/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-budibase-0.0.90/src/cdk_budibase.egg-info/PKG-INFO` & `cdk-budibase-0.0.91/src/cdk_budibase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-budibase
-Version: 0.0.90
+Version: 0.0.91
 Summary: Use AWS CDK to create budibase server
 Home-page: https://github.com/neilkuan/cdk-budibase.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-budibase.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

