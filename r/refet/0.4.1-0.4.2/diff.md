# Comparing `tmp/refet-0.4.1.tar.gz` & `tmp/refet-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refet-0.4.1.tar", last modified: Mon Nov 21 16:47:00 2022, max compression
+gzip compressed data, was "refet-0.4.2.tar", last modified: Fri Jun 30 14:46:52 2023, max compression
```

## Comparing `refet-0.4.1.tar` & `refet-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-11-21 16:47:00.681973 refet-0.4.1/
--rw-r--r--   0 mortonc  (11773) staff       (20)    11357 2018-05-02 15:36:20.000000 refet-0.4.1/LICENSE.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)     8988 2022-11-21 16:47:00.681437 refet-0.4.1/PKG-INFO
--rw-r--r--   0 mortonc  (11773) staff       (20)     8456 2022-10-12 16:27:25.000000 refet-0.4.1/README.rst
--rw-r--r--   0 mortonc  (11773) staff       (20)      916 2022-11-15 23:46:15.000000 refet-0.4.1/pyproject.toml
--rw-r--r--   0 mortonc  (11773) staff       (20)       38 2022-11-21 16:47:00.682074 refet-0.4.1/setup.cfg
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-11-21 16:47:00.674579 refet-0.4.1/src/
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-11-21 16:47:00.679249 refet-0.4.1/src/refet/
--rw-r--r--   0 mortonc  (11773) staff       (20)       52 2022-10-12 16:08:07.000000 refet-0.4.1/src/refet/__init__.py
--rw-r--r--   0 mortonc  (11773) staff       (20)    21885 2022-10-12 16:27:25.000000 refet-0.4.1/src/refet/calcs.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     7853 2022-10-12 16:27:25.000000 refet-0.4.1/src/refet/daily.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     7661 2022-11-15 23:46:15.000000 refet-0.4.1/src/refet/hourly.py
--rw-r--r--   0 mortonc  (11773) staff       (20)     3090 2022-11-21 16:46:36.000000 refet-0.4.1/src/refet/units.py
-drwxr-xr-x   0 mortonc  (11773) staff       (20)        0 2022-11-21 16:47:00.681002 refet-0.4.1/src/refet.egg-info/
--rw-r--r--   0 mortonc  (11773) staff       (20)     8988 2022-11-21 16:47:00.000000 refet-0.4.1/src/refet.egg-info/PKG-INFO
--rw-r--r--   0 mortonc  (11773) staff       (20)      300 2022-11-21 16:47:00.000000 refet-0.4.1/src/refet.egg-info/SOURCES.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)        1 2022-11-21 16:47:00.000000 refet-0.4.1/src/refet.egg-info/dependency_links.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)       14 2022-11-21 16:47:00.000000 refet-0.4.1/src/refet.egg-info/requires.txt
--rw-r--r--   0 mortonc  (11773) staff       (20)        6 2022-11-21 16:47:00.000000 refet-0.4.1/src/refet.egg-info/top_level.txt
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-30 14:46:52.023357 refet-0.4.2/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11357 2023-05-12 14:36:09.000000 refet-0.4.2/LICENSE.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9009 2023-06-30 14:46:52.023187 refet-0.4.2/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8456 2023-05-12 14:36:09.000000 refet-0.4.2/README.rst
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      888 2023-06-30 14:45:57.000000 refet-0.4.2/pyproject.toml
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2023-06-30 14:46:52.023398 refet-0.4.2/setup.cfg
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-30 14:46:52.020709 refet-0.4.2/src/
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-30 14:46:52.021723 refet-0.4.2/src/refet/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      214 2023-06-30 14:45:57.000000 refet-0.4.2/src/refet/__init__.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    21885 2023-05-12 14:36:09.000000 refet-0.4.2/src/refet/calcs.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     7853 2023-05-12 14:36:09.000000 refet-0.4.2/src/refet/daily.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     7661 2023-05-12 14:36:09.000000 refet-0.4.2/src/refet/hourly.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3090 2023-05-12 14:36:09.000000 refet-0.4.2/src/refet/units.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-30 14:46:52.022332 refet-0.4.2/src/refet.egg-info/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9009 2023-06-30 14:46:52.000000 refet-0.4.2/src/refet.egg-info/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      448 2023-06-30 14:46:52.000000 refet-0.4.2/src/refet.egg-info/SOURCES.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2023-06-30 14:46:52.000000 refet-0.4.2/src/refet.egg-info/dependency_links.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       41 2023-06-30 14:46:52.000000 refet-0.4.2/src/refet.egg-info/requires.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        6 2023-06-30 14:46:52.000000 refet-0.4.2/src/refet.egg-info/top_level.txt
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-30 14:46:52.023021 refet-0.4.2/tests/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    15904 2023-05-12 14:36:09.000000 refet-0.4.2/tests/test_calcs.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9324 2023-05-12 14:36:09.000000 refet-0.4.2/tests/test_daily.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     5982 2023-05-12 14:36:09.000000 refet-0.4.2/tests/test_daily_refet_output.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8750 2023-05-12 14:36:09.000000 refet-0.4.2/tests/test_hourly.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     7286 2023-05-12 14:36:09.000000 refet-0.4.2/tests/test_hourly_refet_output.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3240 2023-05-12 14:36:09.000000 refet-0.4.2/tests/test_units.py
```

### Comparing `refet-0.4.1/LICENSE.txt` & `refet-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `refet-0.4.1/PKG-INFO` & `refet-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: refet
-Version: 0.4.1
+Version: 0.4.2
 Summary: ASCE Standardized Reference Evapotranspiration Functions
 Author-email: Charles Morton <charles.morton@dri.edu>
 Project-URL: Homepage, https://github.com/WSWUP/RefET
 Project-URL: Bug Tracker, https://github.com/WSWUP/RefET/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE.txt
 
 ===================================================
 ASCE Standardized Reference Evapotranspiration (ET)
 ===================================================
 
 |version| |build|
```

### Comparing `refet-0.4.1/README.rst` & `refet-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `refet-0.4.1/pyproject.toml` & `refet-0.4.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "refet"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
-  { name="Charles Morton", email="charles.morton@dri.edu" },
+    { name="Charles Morton", email="charles.morton@dri.edu" },
 ]
 description = "ASCE Standardized Reference Evapotranspiration Functions"
 readme = "README.rst"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy >=1.10.0",
@@ -20,26 +20,24 @@
 "Homepage" = "https://github.com/WSWUP/RefET"
 "Bug Tracker" = "https://github.com/WSWUP/RefET/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
-# [project.optional-dependencies]
-# dev = [
-#     "pandas",
-#     "pytz",
-#     "pytest",
-#     "pytest-cov",
-# ]
+[project.optional-dependencies]
+test = [
+    "pandas",
+    "pytz",
+    "pytest",
+]
 
 # [tool.pytest.ini_options]
 # pythonpath = [
-#   "src"
+#     "src"
 # ]
 # addopts = [
 #     "--import-mode=importlib",
 # ]
 
 # [tool.coverage.run]
 # source = ["src"]
-
```

### Comparing `refet-0.4.1/src/refet/calcs.py` & `refet-0.4.2/src/refet/calcs.py`

 * *Files identical despite different names*

### Comparing `refet-0.4.1/src/refet/daily.py` & `refet-0.4.2/src/refet/daily.py`

 * *Files identical despite different names*

### Comparing `refet-0.4.1/src/refet/hourly.py` & `refet-0.4.2/src/refet/hourly.py`

 * *Files identical despite different names*

### Comparing `refet-0.4.1/src/refet/units.py` & `refet-0.4.2/src/refet/units.py`

 * *Files identical despite different names*

### Comparing `refet-0.4.1/src/refet.egg-info/PKG-INFO` & `refet-0.4.2/src/refet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: refet
-Version: 0.4.1
+Version: 0.4.2
 Summary: ASCE Standardized Reference Evapotranspiration Functions
 Author-email: Charles Morton <charles.morton@dri.edu>
 Project-URL: Homepage, https://github.com/WSWUP/RefET
 Project-URL: Bug Tracker, https://github.com/WSWUP/RefET/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE.txt
 
 ===================================================
 ASCE Standardized Reference Evapotranspiration (ET)
 ===================================================
 
 |version| |build|
```

