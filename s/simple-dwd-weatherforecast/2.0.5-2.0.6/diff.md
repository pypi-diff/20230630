# Comparing `tmp/simple_dwd_weatherforecast-2.0.5.tar.gz` & `tmp/simple_dwd_weatherforecast-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_dwd_weatherforecast-2.0.5.tar", last modified: Fri Jun 30 15:05:47 2023, max compression
+gzip compressed data, was "simple_dwd_weatherforecast-2.0.6.tar", last modified: Fri Jun 30 15:26:59 2023, max compression
```

## Comparing `simple_dwd_weatherforecast-2.0.5.tar` & `simple_dwd_weatherforecast-2.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/dwdforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 15:05:36.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/dwdmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:47.779399 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 15:05:47.000000 simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:26:59.643264 simple_dwd_weatherforecast-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 15:26:59.643264 simple_dwd_weatherforecast-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:26:59.643264 simple_dwd_weatherforecast-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:26:59.639264 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/dwdforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/dwdmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   861420 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/stations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:26:59.643264 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/top_level.txt
```

### Comparing `simple_dwd_weatherforecast-2.0.5/LICENCE` & `simple_dwd_weatherforecast-2.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.5/PKG-INFO` & `simple_dwd_weatherforecast-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_dwd_weatherforecast
-Version: 2.0.5
+Version: 2.0.6
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `simple_dwd_weatherforecast-2.0.5/README.md` & `simple_dwd_weatherforecast-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/dwdforecast.py` & `simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/dwdforecast.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast/dwdmap.py` & `simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/dwdmap.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.5/simple_dwd_weatherforecast.egg-info/PKG-INFO` & `simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-dwd-weatherforecast
-Version: 2.0.5
+Version: 2.0.6
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

