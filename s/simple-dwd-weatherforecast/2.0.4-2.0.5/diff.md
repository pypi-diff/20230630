# Comparing `tmp/simple_dwd_weatherforecast-2.0.4.tar.gz` & `tmp/simple_dwd_weatherforecast-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_dwd_weatherforecast-2.0.4.tar", last modified: Fri Jun 30 14:22:19 2023, max compression
+gzip compressed data, was "simple_dwd_weatherforecast-2.0.5.tar", last modified: Fri Jun 30 15:05:47 2023, max compression
```

## Comparing `simple_dwd_weatherforecast-2.0.4.tar` & `simple_dwd_weatherforecast-2.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:19.668050 simple_dwd_weatherforecast-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 14:22:10.000000 simple_dwd_weatherforecast-2.0.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 14:22:19.668050 simple_dwd_weatherforecast-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 14:22:10.000000 simple_dwd_weatherforecast-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:22:19.668050 simple_dwd_weatherforecast-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 14:22:10.000000 simple_dwd_weatherforecast-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:19.664049 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:10.000000 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-30 14:22:10.000000 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast/dwdforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 14:22:10.000000 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast/dwdmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:19.668050 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 14:22:19.000000 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 14:22:19.000000 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:19.000000 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 14:22:19.000000 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 14:22:19.000000 simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/dwdforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/dwdmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/top_level.txt
```

### Comparing `simple_dwd_weatherforecast-2.0.4/LICENCE` & `simple_dwd_weatherforecast-2.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.4/PKG-INFO` & `simple_dwd_weatherforecast-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_dwd_weatherforecast
-Version: 2.0.4
+Version: 2.0.5
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `simple_dwd_weatherforecast-2.0.4/README.md` & `simple_dwd_weatherforecast-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.4/setup.py` & `simple_dwd_weatherforecast-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_dwd_weatherforecast",
-    version="2.0.4",
+    version="2.0.5",
     author="Max Fermor",
     description="A simple tool to retrieve a weather forecast from DWD OpenData",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FL550/simple_dwd_weatherforecast.git",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast/dwdforecast.py` & `simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/dwdforecast.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast/dwdmap.py` & `simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/dwdmap.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.4/simple_dwd_weatherforecast.egg-info/PKG-INFO` & `simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-dwd-weatherforecast
-Version: 2.0.4
+Version: 2.0.5
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

