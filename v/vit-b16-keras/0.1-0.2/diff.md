# Comparing `tmp/vit-b16-keras-0.1.tar.gz` & `tmp/vit-b16-keras-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-b16-keras-0.1.tar", last modified: Fri Jun 30 15:34:04 2023, max compression
+gzip compressed data, was "vit-b16-keras-0.2.tar", last modified: Fri Jun 30 17:48:26 2023, max compression
```

## Comparing `vit-b16-keras-0.1.tar` & `vit-b16-keras-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:34:04.907882 vit-b16-keras-0.1/
--rw-rw-rw-   0        0        0      616 2023-06-30 15:34:04.906895 vit-b16-keras-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-30 15:34:04.908889 vit-b16-keras-0.1/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-06-30 15:32:55.000000 vit-b16-keras-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:34:04.879025 vit-b16-keras-0.1/vit-b16-keras/
--rw-rw-rw-   0        0        0       40 2023-06-30 13:48:14.000000 vit-b16-keras-0.1/vit-b16-keras/__init__.py
--rw-rw-rw-   0        0        0      438 2023-06-30 15:33:57.000000 vit-b16-keras-0.1/vit-b16-keras/vit_b16.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:34:04.903883 vit-b16-keras-0.1/vit_b16_keras.egg-info/
--rw-rw-rw-   0        0        0      616 2023-06-30 15:34:04.000000 vit-b16-keras-0.1/vit_b16_keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-30 15:34:04.000000 vit-b16-keras-0.1/vit_b16_keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:34:04.000000 vit-b16-keras-0.1/vit_b16_keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 15:34:04.000000 vit-b16-keras-0.1/vit_b16_keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 15:34:04.000000 vit-b16-keras-0.1/vit_b16_keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 17:48:26.603072 vit-b16-keras-0.2/
+-rw-rw-rw-   0        0        0      616 2023-06-30 17:48:26.602079 vit-b16-keras-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-30 17:48:26.604073 vit-b16-keras-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-06-30 17:48:09.000000 vit-b16-keras-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:48:26.566076 vit-b16-keras-0.2/vit_b16_keras/
+-rw-rw-rw-   0        0        0       40 2023-06-30 17:45:23.000000 vit-b16-keras-0.2/vit_b16_keras/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-06-30 17:41:31.000000 vit-b16-keras-0.2/vit_b16_keras/vit_b16.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:48:26.600069 vit-b16-keras-0.2/vit_b16_keras.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-06-30 17:48:26.000000 vit-b16-keras-0.2/vit_b16_keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-30 17:48:26.000000 vit-b16-keras-0.2/vit_b16_keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 17:48:26.000000 vit-b16-keras-0.2/vit_b16_keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 17:48:26.000000 vit-b16-keras-0.2/vit_b16_keras.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 17:48:26.000000 vit-b16-keras-0.2/vit_b16_keras.egg-info/top_level.txt
```

### Comparing `vit-b16-keras-0.1/PKG-INFO` & `vit-b16-keras-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-b16-keras
-Version: 0.1
+Version: 0.2
 Summary: vit-b16-keras
 Home-page: UNKNOWN
 Author: Elena Paul
 Author-email: wohani7266@dotvilla.com
 License: UNKNOWN
 Description: A package to install vision transformer
 Keywords: arithmetic,math,mathematics
```

### Comparing `vit-b16-keras-0.1/setup.py` & `vit-b16-keras-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1'
+VERSION = '0.2'
 DESCRIPTION = 'vit-b16-keras'
 LONG_DESCRIPTION = 'A package to install vision transformer'
 
 # Setting up
 setup(
     name="vit-b16-keras",
     version=VERSION,
```

### Comparing `vit-b16-keras-0.1/vit_b16_keras.egg-info/PKG-INFO` & `vit-b16-keras-0.2/vit_b16_keras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-b16-keras
-Version: 0.1
+Version: 0.2
 Summary: vit-b16-keras
 Home-page: UNKNOWN
 Author: Elena Paul
 Author-email: wohani7266@dotvilla.com
 License: UNKNOWN
 Description: A package to install vision transformer
 Keywords: arithmetic,math,mathematics
```

