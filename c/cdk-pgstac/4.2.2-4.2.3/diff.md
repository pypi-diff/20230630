# Comparing `tmp/cdk-pgstac-4.2.2.tar.gz` & `tmp/cdk-pgstac-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-pgstac-4.2.2.tar", last modified: Fri Jun 16 06:25:00 2023, max compression
+gzip compressed data, was "cdk-pgstac-4.2.3.tar", last modified: Fri Jun 30 10:58:34 2023, max compression
```

## Comparing `cdk-pgstac-4.2.2.tar` & `cdk-pgstac-4.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/src/cdk_pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)   136966 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/src/cdk_pgstac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/src/cdk_pgstac/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/src/cdk_pgstac/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   172634 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/src/cdk_pgstac/_jsii/cdk-pgstac@4.2.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/src/cdk_pgstac/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:58:34.205497 cdk-pgstac-4.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-30 10:58:34.205497 cdk-pgstac-4.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:58:34.205497 cdk-pgstac-4.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:58:34.205497 cdk-pgstac-4.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:58:34.205497 cdk-pgstac-4.2.3/src/cdk_pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)   136966 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/src/cdk_pgstac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:58:34.205497 cdk-pgstac-4.2.3/src/cdk_pgstac/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/src/cdk_pgstac/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172601 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/src/cdk_pgstac/_jsii/cdk-pgstac@4.2.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:58:25.000000 cdk-pgstac-4.2.3/src/cdk_pgstac/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:58:34.205497 cdk-pgstac-4.2.3/src/cdk_pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-30 10:58:33.000000 cdk-pgstac-4.2.3/src/cdk_pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-30 10:58:34.000000 cdk-pgstac-4.2.3/src/cdk_pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:58:33.000000 cdk-pgstac-4.2.3/src/cdk_pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 10:58:34.000000 cdk-pgstac-4.2.3/src/cdk_pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 10:58:34.000000 cdk-pgstac-4.2.3/src/cdk_pgstac.egg-info/top_level.txt
```

### Comparing `cdk-pgstac-4.2.2/LICENSE` & `cdk-pgstac-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.2.2/PKG-INFO` & `cdk-pgstac-4.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 4.2.2
+Version: 4.2.3
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-pgstac-4.2.2/README.md` & `cdk-pgstac-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.2.2/setup.py` & `cdk-pgstac-4.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-pgstac",
-    "version": "4.2.2",
+    "version": "4.2.3",
     "description": "A set of constructs deploying pgSTAC with CDK",
     "license": "ISC",
     "url": "https://github.com/developmentseed/cdk-pgstac.git",
     "long_description_content_type": "text/markdown",
     "author": "Anthony Lukach<anthony@developmentseed.org>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_pgstac",
         "cdk_pgstac._jsii"
     ],
     "package_data": {
         "cdk_pgstac._jsii": [
-            "cdk-pgstac@4.2.2.jsii.tgz"
+            "cdk-pgstac@4.2.3.jsii.tgz"
         ],
         "cdk_pgstac": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-pgstac-4.2.2/src/cdk_pgstac/__init__.py` & `cdk-pgstac-4.2.3/src/cdk_pgstac/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/PKG-INFO` & `cdk-pgstac-4.2.3/src/cdk_pgstac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 4.2.2
+Version: 4.2.3
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

