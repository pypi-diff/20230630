# Comparing `tmp/sphractal-0.4.0.tar.gz` & `tmp/sphractal-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.4.0.tar", max compression
+gzip compressed data, was "sphractal-0.4.2.tar", max compression
```

## Comparing `sphractal-0.4.0.tar` & `sphractal-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1082 2023-06-27 05:21:43.041389 sphractal-0.4.0/LICENSE
--rwxr-xr-x   0        0        0     2923 2023-06-29 14:18:09.647848 sphractal-0.4.0/README.md
--rwxr-xr-x   0        0        0     1428 2023-06-29 14:33:18.024655 sphractal-0.4.0/pyproject.toml
--rwxr-xr-x   0        0        0     1394 2023-06-29 02:30:46.436695 sphractal-0.4.0/src/sphractal/__init__.py
--rwxr-xr-x   0        0        0    21060 2023-06-29 09:48:04.563888 sphractal-0.4.0/src/sphractal/boxCnt.py
--rwxr-xr-x   0        0        0     3821 2023-06-29 07:36:35.379815 sphractal-0.4.0/src/sphractal/constants.py
--rwxr-xr-x   0        0        0        0 2023-06-28 06:39:13.904193 sphractal-0.4.0/src/sphractal/data/__init__.py
--rwxr-xr-x   0        0        0    20105 2023-06-28 13:54:13.190798 sphractal-0.4.0/src/sphractal/data/example.xyz
--rwxr-xr-x   0        0        0      279 2023-06-29 04:44:45.075987 sphractal-0.4.0/src/sphractal/datasets.py
--rwxr-xr-x   0        0        0     8813 2023-06-29 09:00:43.603121 sphractal-0.4.0/src/sphractal/surfExact.py
--rwxr-xr-x   0        0        0     7909 2023-06-29 07:30:04.760528 sphractal-0.4.0/src/sphractal/surfPointClouds.py
--rwxr-xr-x   0        0        0    11480 2023-06-29 12:21:19.032436 sphractal-0.4.0/src/sphractal/utils.py
--rwxr-xr-x   0        0        0    94223 2023-06-29 13:46:08.939952 sphractal-0.4.0/tests/fixtures.py
--rwxr-xr-x   0        0        0    10966 2023-06-29 14:06:17.192569 sphractal-0.4.0/tests/test_sphractal.py
--rw-r--r--   0        0        0     3687 1970-01-01 00:00:00.000000 sphractal-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-30 03:23:36.162883 sphractal-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2767 2023-06-30 03:23:36.162883 sphractal-0.4.2/README.md
+-rw-r--r--   0        0        0     1428 2023-06-30 03:24:30.958639 sphractal-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1394 2023-06-30 03:23:36.230883 sphractal-0.4.2/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    21060 2023-06-30 03:23:36.230883 sphractal-0.4.2/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     3821 2023-06-30 03:23:36.230883 sphractal-0.4.2/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-06-30 03:23:36.230883 sphractal-0.4.2/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      279 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8813 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     7909 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11480 2023-06-30 03:23:36.234883 sphractal-0.4.2/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94223 2023-06-30 03:23:36.234883 sphractal-0.4.2/tests/fixtures.py
+-rw-r--r--   0        0        0    10966 2023-06-30 03:23:36.234883 sphractal-0.4.2/tests/test_sphractal.py
+-rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 sphractal-0.4.2/PKG-INFO
```

### Comparing `sphractal-0.4.0/LICENSE` & `sphractal-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/README.md` & `sphractal-0.4.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Sphractal
 
-[![ci-cd](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml)
-
 ## Description
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
```

### Comparing `sphractal-0.4.0/pyproject.toml` & `sphractal-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.4.0"
+version = "0.4.2"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting"]
 license = "MIT"
 readme = "README.md"
 include = ["tests/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `sphractal-0.4.0/src/sphractal/__init__.py` & `sphractal-0.4.2/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/src/sphractal/boxCnt.py` & `sphractal-0.4.2/src/sphractal/boxCnt.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/src/sphractal/constants.py` & `sphractal-0.4.2/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/src/sphractal/data/example.xyz` & `sphractal-0.4.2/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/src/sphractal/surfExact.py` & `sphractal-0.4.2/src/sphractal/surfExact.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/src/sphractal/surfPointClouds.py` & `sphractal-0.4.2/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/src/sphractal/utils.py` & `sphractal-0.4.2/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/tests/fixtures.py` & `sphractal-0.4.2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/tests/test_sphractal.py` & `sphractal-0.4.2/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.0/PKG-INFO` & `sphractal-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.4.0
+Version: 0.4.2
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 License: MIT
 Author: Jonathan Yik Chang Ting
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,16 +15,14 @@
 Requires-Dist: numpy (>=1.22,<1.25)
 Requires-Dist: scipy (>=1.11.0) ; python_version >= "3.9" and python_version < "3.13"
 Requires-Dist: statsmodels (>=0.14.0)
 Description-Content-Type: text/markdown
 
 # Sphractal
 
-[![ci-cd](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml)
-
 ## Description
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
```

