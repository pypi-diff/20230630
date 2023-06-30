# Comparing `tmp/vit-b16-keras-0.0.8.tar.gz` & `tmp/vit-b16-keras-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-b16-keras-0.0.8.tar", last modified: Fri Jun 30 14:07:56 2023, max compression
+gzip compressed data, was "vit-b16-keras-0.0.9.tar", last modified: Fri Jun 30 14:57:59 2023, max compression
```

## Comparing `vit-b16-keras-0.0.8.tar` & `vit-b16-keras-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 14:07:56.537482 vit-b16-keras-0.0.8/
--rw-rw-rw-   0        0        0      618 2023-06-30 14:07:56.535478 vit-b16-keras-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-30 14:07:56.538484 vit-b16-keras-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      878 2023-06-30 13:52:24.000000 vit-b16-keras-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:07:56.512968 vit-b16-keras-0.0.8/vit-b16-keras/
--rw-rw-rw-   0        0        0       40 2023-06-30 13:48:14.000000 vit-b16-keras-0.0.8/vit-b16-keras/__init__.py
--rw-rw-rw-   0        0        0      340 2023-06-30 14:03:16.000000 vit-b16-keras-0.0.8/vit-b16-keras/vit_b16.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:07:56.533481 vit-b16-keras-0.0.8/vit_b16_keras.egg-info/
--rw-rw-rw-   0        0        0      618 2023-06-30 14:07:56.000000 vit-b16-keras-0.0.8/vit_b16_keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-30 14:07:56.000000 vit-b16-keras-0.0.8/vit_b16_keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:07:56.000000 vit-b16-keras-0.0.8/vit_b16_keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 14:07:56.000000 vit-b16-keras-0.0.8/vit_b16_keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 14:07:56.000000 vit-b16-keras-0.0.8/vit_b16_keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 14:57:59.311003 vit-b16-keras-0.0.9/
+-rw-rw-rw-   0        0        0      618 2023-06-30 14:57:59.310002 vit-b16-keras-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-30 14:57:59.312002 vit-b16-keras-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      878 2023-06-30 14:51:16.000000 vit-b16-keras-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:57:59.279006 vit-b16-keras-0.0.9/vit-b16-keras/
+-rw-rw-rw-   0        0        0       40 2023-06-30 13:48:14.000000 vit-b16-keras-0.0.9/vit-b16-keras/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-06-30 14:51:05.000000 vit-b16-keras-0.0.9/vit-b16-keras/vit_b16.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:57:59.307003 vit-b16-keras-0.0.9/vit_b16_keras.egg-info/
+-rw-rw-rw-   0        0        0      618 2023-06-30 14:57:59.000000 vit-b16-keras-0.0.9/vit_b16_keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-30 14:57:59.000000 vit-b16-keras-0.0.9/vit_b16_keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:57:59.000000 vit-b16-keras-0.0.9/vit_b16_keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 14:57:59.000000 vit-b16-keras-0.0.9/vit_b16_keras.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 14:57:59.000000 vit-b16-keras-0.0.9/vit_b16_keras.egg-info/top_level.txt
```

### Comparing `vit-b16-keras-0.0.8/PKG-INFO` & `vit-b16-keras-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-b16-keras
-Version: 0.0.8
+Version: 0.0.9
 Summary: vit-b16-keras
 Home-page: UNKNOWN
 Author: Elena Paul
 Author-email: wohani7266@dotvilla.com
 License: UNKNOWN
 Description: A package to install vision transformer
 Keywords: arithmetic,math,mathematics
```

### Comparing `vit-b16-keras-0.0.8/setup.py` & `vit-b16-keras-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'vit-b16-keras'
 LONG_DESCRIPTION = 'A package to install vision transformer'
 
 # Setting up
 setup(
     name="vit-b16-keras",
     version=VERSION,
```

### Comparing `vit-b16-keras-0.0.8/vit_b16_keras.egg-info/PKG-INFO` & `vit-b16-keras-0.0.9/vit_b16_keras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-b16-keras
-Version: 0.0.8
+Version: 0.0.9
 Summary: vit-b16-keras
 Home-page: UNKNOWN
 Author: Elena Paul
 Author-email: wohani7266@dotvilla.com
 License: UNKNOWN
 Description: A package to install vision transformer
 Keywords: arithmetic,math,mathematics
```

