# Comparing `tmp/CNUfof_utils-1.0.0.tar.gz` & `tmp/CNUfof_utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CNUfof_utils-1.0.0.tar", last modified: Thu Jun 29 21:42:13 2023, max compression
+gzip compressed data, was "dist/CNUfof_utils-1.0.1.tar", last modified: Fri Jun 30 02:16:04 2023, max compression
```

## Comparing `CNUfof_utils-1.0.0.tar` & `CNUfof_utils-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ehddbs98  (1005) ehddbs98  (1006)        0 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/
-drwxrwxr-x   0 ehddbs98  (1005) ehddbs98  (1006)        0 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/CNUfof_utils.egg-info/
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)     1898 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/CNUfof_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)      194 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/CNUfof_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)        1 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/CNUfof_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)        5 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/CNUfof_utils.egg-info/top_level.txt
-drwxrwxr-x   0 ehddbs98  (1005) ehddbs98  (1006)        0 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/PFOF/
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)       50 2023-06-28 22:14:03.000000 CNUfof_utils-1.0.0/PFOF/__init__.py
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)     9063 2023-06-28 20:25:46.000000 CNUfof_utils-1.0.0/PFOF/functions.py
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)     1432 2023-06-29 21:42:04.000000 CNUfof_utils-1.0.0/README
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)      713 2023-06-29 21:41:57.000000 CNUfof_utils-1.0.0/setup.py
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)     1898 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/PKG-INFO
--rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)       38 2023-06-29 21:42:13.000000 CNUfof_utils-1.0.0/setup.cfg
+drwxrwxr-x   0 ehddbs98  (1005) ehddbs98  (1006)        0 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/
+drwxrwxr-x   0 ehddbs98  (1005) ehddbs98  (1006)        0 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/CNUfof_utils.egg-info/
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)     1898 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/CNUfof_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)      194 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/CNUfof_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)        1 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/CNUfof_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)        5 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/CNUfof_utils.egg-info/top_level.txt
+drwxrwxr-x   0 ehddbs98  (1005) ehddbs98  (1006)        0 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/PFOF/
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)       72 2023-06-30 02:14:18.000000 CNUfof_utils-1.0.1/PFOF/__init__.py
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)     9075 2023-06-30 02:12:15.000000 CNUfof_utils-1.0.1/PFOF/functions.py
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)     1432 2023-06-30 02:15:07.000000 CNUfof_utils-1.0.1/README
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)      713 2023-06-30 02:15:15.000000 CNUfof_utils-1.0.1/setup.py
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)     1898 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/PKG-INFO
+-rw-rw-r--   0 ehddbs98  (1005) ehddbs98  (1006)       38 2023-06-30 02:16:04.000000 CNUfof_utils-1.0.1/setup.cfg
```

### Comparing `CNUfof_utils-1.0.0/CNUfof_utils.egg-info/PKG-INFO` & `CNUfof_utils-1.0.1/CNUfof_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNUfof-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for Galaxy Group finding algorithm using Mutliprocessing package
 Home-page: https://github.com/Dong-yunkwak/KDY.git
 Author: Dong Yun Kwak
 Author-email: 98ehddbs@naver.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 * Pydl
 * Ray (Multiprocessing Package)
 * astropy
 * Pandas 
 
 
 
-Version 1.0.0 2023.06.22 
+Version 1.0.1 2023.06.22 
 Version of packages used. (Please check these versions)
 python  3.10.3
 numpy   1.21.4
 astropy 5.1.1
 pandas  1.3.5
 pydl    1.0.0
 ray     2.2.9
```

### Comparing `CNUfof_utils-1.0.0/PFOF/functions.py` & `CNUfof_utils-1.0.1/PFOF/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import astropy.units as u
 import pandas as pd
 from astropy.cosmology import FlatLambdaCDM , Planck18
 from pydl.goddard.astro import gcirc
 import astropy.units as u
 import ray
 import sys
+import time
 sys.setrecursionlimit(10**6)
 
 
 # In[ ]:
 
 
 class fofradecV():
```

### Comparing `CNUfof_utils-1.0.0/README` & `CNUfof_utils-1.0.1/README`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * Pydl
 * Ray (Multiprocessing Package)
 * astropy
 * Pandas 
 
 
 
-Version 1.0.0 2023.06.22 
+Version 1.0.1 2023.06.22 
 Version of packages used. (Please check these versions)
 python  3.10.3
 numpy   1.21.4
 astropy 5.1.1
 pandas  1.3.5
 pydl    1.0.0
 ray     2.2.9
```

### Comparing `CNUfof_utils-1.0.0/setup.py` & `CNUfof_utils-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # In[3]:
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CNUfof_utils",
-    version = '1.0.0',
+    version = '1.0.1',
     author = "Dong Yun Kwak",
     author_email = '98ehddbs@naver.com',
     description = "Python package for Galaxy Group finding algorithm using Mutliprocessing package",
     long_description = long_description,
     long_description_content_type = "text",
     url="https://github.com/Dong-yunkwak/KDY.git",
     packages=['PFOF'],
```

### Comparing `CNUfof_utils-1.0.0/PKG-INFO` & `CNUfof_utils-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNUfof_utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for Galaxy Group finding algorithm using Mutliprocessing package
 Home-page: https://github.com/Dong-yunkwak/KDY.git
 Author: Dong Yun Kwak
 Author-email: 98ehddbs@naver.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 * Pydl
 * Ray (Multiprocessing Package)
 * astropy
 * Pandas 
 
 
 
-Version 1.0.0 2023.06.22 
+Version 1.0.1 2023.06.22 
 Version of packages used. (Please check these versions)
 python  3.10.3
 numpy   1.21.4
 astropy 5.1.1
 pandas  1.3.5
 pydl    1.0.0
 ray     2.2.9
```

