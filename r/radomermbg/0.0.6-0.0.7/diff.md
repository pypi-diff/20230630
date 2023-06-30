# Comparing `tmp/radomermbg-0.0.6.tar.gz` & `tmp/radomermbg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\radomermbg-0.0.6.tar", last modified: Fri Jun 30 11:45:58 2023, max compression
+gzip compressed data, was "dist\radomermbg-0.0.7.tar", last modified: Fri Jun 30 11:48:19 2023, max compression
```

## Comparing `radomermbg-0.0.6.tar` & `radomermbg-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 11:45:58.000000 radomermbg-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-06-30 10:03:26.000000 radomermbg-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-06-30 10:00:42.000000 radomermbg-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      494 2023-06-30 11:45:58.000000 radomermbg-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-06-30 09:59:40.000000 radomermbg-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 11:45:58.000000 radomermbg-0.0.6/radomermbg/
--rw-rw-rw-   0        0        0       94 2023-06-30 11:38:05.000000 radomermbg-0.0.6/radomermbg/__init__.py
--rw-rw-rw-   0        0        0      191 2023-06-30 09:36:56.000000 radomermbg-0.0.6/radomermbg/downloadweights.py
--rw-rw-rw-   0        0        0     1796 2023-06-30 11:41:05.000000 radomermbg-0.0.6/radomermbg/radomer.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:45:58.000000 radomermbg-0.0.6/radomermbg.egg-info/
--rw-rw-rw-   0        0        0      494 2023-06-30 11:45:58.000000 radomermbg-0.0.6/radomermbg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-30 11:45:58.000000 radomermbg-0.0.6/radomermbg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 11:45:58.000000 radomermbg-0.0.6/radomermbg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 11:45:58.000000 radomermbg-0.0.6/radomermbg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 11:45:58.000000 radomermbg-0.0.6/radomermbg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 11:45:58.000000 radomermbg-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1316 2023-06-30 11:45:48.000000 radomermbg-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:48:19.000000 radomermbg-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-06-30 10:03:26.000000 radomermbg-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-06-30 10:00:42.000000 radomermbg-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      494 2023-06-30 11:48:19.000000 radomermbg-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-06-30 09:59:40.000000 radomermbg-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 11:48:19.000000 radomermbg-0.0.7/radomermbg/
+-rw-rw-rw-   0        0        0       94 2023-06-30 11:38:05.000000 radomermbg-0.0.7/radomermbg/__init__.py
+-rw-rw-rw-   0        0        0     1965 2023-06-30 11:47:30.000000 radomermbg-0.0.7/radomermbg/radomer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:48:19.000000 radomermbg-0.0.7/radomermbg.egg-info/
+-rw-rw-rw-   0        0        0      494 2023-06-30 11:48:19.000000 radomermbg-0.0.7/radomermbg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-30 11:48:19.000000 radomermbg-0.0.7/radomermbg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:48:19.000000 radomermbg-0.0.7/radomermbg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 11:48:19.000000 radomermbg-0.0.7/radomermbg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 11:48:19.000000 radomermbg-0.0.7/radomermbg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 11:48:19.000000 radomermbg-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1316 2023-06-30 11:48:10.000000 radomermbg-0.0.7/setup.py
```

### Comparing `radomermbg-0.0.6/LICENSE.txt` & `radomermbg-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `radomermbg-0.0.6/radomermbg/radomer.py` & `radomermbg-0.0.7/radomermbg/radomer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import os
 import gdown
 import torch
 import  cv2
 import numpy as np
 from ultralytics import YOLO
 
-import downloadweights
+import os 
+import gdown
+
+
+gdown.download('https://drive.google.com/file/d/1DXFI6oY8087JlgVN2JkHKAki9tevCiVt/view?usp=drive_link','best_test_platform_elas.pt',
+    quiet=False,fuzzy=True)
 
 # Load a model
 model = YOLO('best_test_platform_elas.pt')  # load a custom model
 
 # Predict with the model
 
 def background(img):
```

### Comparing `radomermbg-0.0.6/setup.py` & `radomermbg-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 from setuptools import setup, find_packages
 setup(
   name = 'radomermbg',         # How you named your package folder (MyLib)
   packages = find_packages(),   # Chose the same as "name"
-  version = '0.0.6',      # Start with a small number and increase it with every change you make
+  version = '0.0.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'background removal',   # Give a short description about your library
   author = 'SARVESH,SRIDHARAN,PRIYANKA', 
   url = '',                  # Type in your name
   author_email = 'cvradome@gmail.com',      # Type in your E-Mail
   keywords = ['background', 'subtraction'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
```

