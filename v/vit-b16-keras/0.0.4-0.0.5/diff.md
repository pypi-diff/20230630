# Comparing `tmp/vit-b16-keras-0.0.4.tar.gz` & `tmp/vit-b16-keras-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-b16-keras-0.0.4.tar", last modified: Fri Jun 30 13:40:59 2023, max compression
+gzip compressed data, was "vit-b16-keras-0.0.5.tar", last modified: Wed Jun 28 11:04:18 2023, max compression
```

## Comparing `vit-b16-keras-0.0.4.tar` & `vit-b16-keras-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 13:40:59.036574 vit-b16-keras-0.0.4/
--rw-rw-rw-   0        0        0      612 2023-06-30 13:40:59.035576 vit-b16-keras-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-30 13:40:59.037572 vit-b16-keras-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      872 2023-06-30 13:39:34.000000 vit-b16-keras-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:40:59.004573 vit-b16-keras-0.0.4/vit-b16/
--rw-rw-rw-   0        0        0       40 2023-06-30 13:27:36.000000 vit-b16-keras-0.0.4/vit-b16/__init__.py
--rw-rw-rw-   0        0        0      385 2023-06-30 13:31:43.000000 vit-b16-keras-0.0.4/vit-b16/vit_b16.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:40:59.032570 vit-b16-keras-0.0.4/vit_b16_keras.egg-info/
--rw-rw-rw-   0        0        0      612 2023-06-30 13:40:58.000000 vit-b16-keras-0.0.4/vit_b16_keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-30 13:40:58.000000 vit-b16-keras-0.0.4/vit_b16_keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 13:40:58.000000 vit-b16-keras-0.0.4/vit_b16_keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 13:40:58.000000 vit-b16-keras-0.0.4/vit_b16_keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 13:40:58.000000 vit-b16-keras-0.0.4/vit_b16_keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-28 11:04:18.851382 vit-b16-keras-0.0.5/
+-rw-rw-rw-   0        0        0      618 2023-06-28 11:04:18.844870 vit-b16-keras-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-28 11:04:18.851382 vit-b16-keras-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      878 2023-06-28 11:02:13.000000 vit-b16-keras-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-28 11:04:18.795314 vit-b16-keras-0.0.5/vit-b16-keras/
+-rw-rw-rw-   0        0        0       33 2023-06-28 08:25:05.000000 vit-b16-keras-0.0.5/vit-b16-keras/__init__.py
+-rw-rw-rw-   0        0        0      336 2023-06-28 10:58:36.000000 vit-b16-keras-0.0.5/vit-b16-keras/vit.py
+drwxrwxrwx   0        0        0        0 2023-06-28 11:04:18.844870 vit-b16-keras-0.0.5/vit_b16_keras.egg-info/
+-rw-rw-rw-   0        0        0      618 2023-06-28 11:04:18.000000 vit-b16-keras-0.0.5/vit_b16_keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-06-28 11:04:18.000000 vit-b16-keras-0.0.5/vit_b16_keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-28 11:04:18.000000 vit-b16-keras-0.0.5/vit_b16_keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-28 11:04:18.000000 vit-b16-keras-0.0.5/vit_b16_keras.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-28 11:04:18.000000 vit-b16-keras-0.0.5/vit_b16_keras.egg-info/top_level.txt
```

### Comparing `vit-b16-keras-0.0.4/PKG-INFO` & `vit-b16-keras-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vit-b16-keras
-Version: 0.0.4
-Summary: vitb-16
+Version: 0.0.5
+Summary: vit-b16-keras
 Home-page: UNKNOWN
 Author: Elena Paul
 Author-email: wohani7266@dotvilla.com
 License: UNKNOWN
 Description: A package to install vision transformer
 Keywords: arithmetic,math,mathematics
 Platform: UNKNOWN
```

### Comparing `vit-b16-keras-0.0.4/setup.py` & `vit-b16-keras-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
-DESCRIPTION = 'vitb-16'
+VERSION = '0.0.5'
+DESCRIPTION = 'vit-b16-keras'
 LONG_DESCRIPTION = 'A package to install vision transformer'
 
 # Setting up
 setup(
     name="vit-b16-keras",
     version=VERSION,
     author="Elena Paul",
```

### Comparing `vit-b16-keras-0.0.4/vit_b16_keras.egg-info/PKG-INFO` & `vit-b16-keras-0.0.5/vit_b16_keras.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vit-b16-keras
-Version: 0.0.4
-Summary: vitb-16
+Version: 0.0.5
+Summary: vit-b16-keras
 Home-page: UNKNOWN
 Author: Elena Paul
 Author-email: wohani7266@dotvilla.com
 License: UNKNOWN
 Description: A package to install vision transformer
 Keywords: arithmetic,math,mathematics
 Platform: UNKNOWN
```

