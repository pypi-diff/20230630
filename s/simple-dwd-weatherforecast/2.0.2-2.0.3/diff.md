# Comparing `tmp/simple_dwd_weatherforecast-2.0.2.tar.gz` & `tmp/simple_dwd_weatherforecast-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_dwd_weatherforecast-2.0.2.tar", last modified: Fri Jun 30 12:41:36 2023, max compression
+gzip compressed data, was "simple_dwd_weatherforecast-2.0.3.tar", last modified: Fri Jun 30 14:14:55 2023, max compression
```

## Comparing `simple_dwd_weatherforecast-2.0.2.tar` & `simple_dwd_weatherforecast-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:41:36.303895 simple_dwd_weatherforecast-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 12:41:36.303895 simple_dwd_weatherforecast-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:41:36.307895 simple_dwd_weatherforecast-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:41:36.303895 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/dwdforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/dwdmap.py
--rw-r--r--   0 runner    (1001) docker     (123)   386545 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/stations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:41:36.303895 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:14:55.527117 simple_dwd_weatherforecast-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 14:14:46.000000 simple_dwd_weatherforecast-2.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 14:14:55.527117 simple_dwd_weatherforecast-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 14:14:46.000000 simple_dwd_weatherforecast-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:14:55.527117 simple_dwd_weatherforecast-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 14:14:46.000000 simple_dwd_weatherforecast-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:14:55.523117 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:14:46.000000 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-06-30 14:14:46.000000 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast/dwdforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 14:14:46.000000 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast/dwdmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:14:55.523117 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 14:14:55.000000 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 14:14:55.000000 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:14:55.000000 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 14:14:55.000000 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 14:14:55.000000 simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast.egg-info/top_level.txt
```

### Comparing `simple_dwd_weatherforecast-2.0.2/LICENCE` & `simple_dwd_weatherforecast-2.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.2/PKG-INFO` & `simple_dwd_weatherforecast-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_dwd_weatherforecast
-Version: 2.0.2
+Version: 2.0.3
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `simple_dwd_weatherforecast-2.0.2/README.md` & `simple_dwd_weatherforecast-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.2/setup.py` & `simple_dwd_weatherforecast-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_dwd_weatherforecast",
-    version="2.0.2",
+    version="2.0.3",
     author="Max Fermor",
     description="A simple tool to retrieve a weather forecast from DWD OpenData",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FL550/simple_dwd_weatherforecast.git",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/dwdforecast.py` & `simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast/dwdforecast.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/dwdmap.py` & `simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast/dwdmap.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/PKG-INFO` & `simple_dwd_weatherforecast-2.0.3/simple_dwd_weatherforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-dwd-weatherforecast
-Version: 2.0.2
+Version: 2.0.3
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

