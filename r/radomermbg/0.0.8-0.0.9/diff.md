# Comparing `tmp/radomermbg-0.0.8.tar.gz` & `tmp/radomermbg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\radomermbg-0.0.8.tar", last modified: Fri Jun 30 11:53:30 2023, max compression
+gzip compressed data, was "dist\radomermbg-0.0.9.tar", last modified: Fri Jun 30 11:58:19 2023, max compression
```

## Comparing `radomermbg-0.0.8.tar` & `radomermbg-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 11:53:30.000000 radomermbg-0.0.8/
--rw-rw-rw-   0        0        0     1088 2023-06-30 10:03:26.000000 radomermbg-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-06-30 10:00:42.000000 radomermbg-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      494 2023-06-30 11:53:30.000000 radomermbg-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-06-30 09:59:40.000000 radomermbg-0.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 11:53:30.000000 radomermbg-0.0.8/radomermbg/
--rw-rw-rw-   0        0        0       94 2023-06-30 11:38:05.000000 radomermbg-0.0.8/radomermbg/__init__.py
--rw-rw-rw-   0        0        0     1929 2023-06-30 11:52:24.000000 radomermbg-0.0.8/radomermbg/radomer.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:53:30.000000 radomermbg-0.0.8/radomermbg.egg-info/
--rw-rw-rw-   0        0        0      494 2023-06-30 11:53:29.000000 radomermbg-0.0.8/radomermbg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-30 11:53:29.000000 radomermbg-0.0.8/radomermbg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 11:53:29.000000 radomermbg-0.0.8/radomermbg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 11:53:29.000000 radomermbg-0.0.8/radomermbg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 11:53:29.000000 radomermbg-0.0.8/radomermbg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 11:53:30.000000 radomermbg-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1316 2023-06-30 11:53:23.000000 radomermbg-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:58:19.000000 radomermbg-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2023-06-30 10:03:26.000000 radomermbg-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-06-30 10:00:42.000000 radomermbg-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      494 2023-06-30 11:58:19.000000 radomermbg-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-06-30 09:59:40.000000 radomermbg-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 11:58:19.000000 radomermbg-0.0.9/radomermbg/
+-rw-rw-rw-   0        0        0       94 2023-06-30 11:38:05.000000 radomermbg-0.0.9/radomermbg/__init__.py
+-rw-rw-rw-   0        0        0     2034 2023-06-30 11:57:52.000000 radomermbg-0.0.9/radomermbg/radomer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:58:19.000000 radomermbg-0.0.9/radomermbg.egg-info/
+-rw-rw-rw-   0        0        0      494 2023-06-30 11:58:18.000000 radomermbg-0.0.9/radomermbg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-30 11:58:19.000000 radomermbg-0.0.9/radomermbg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:58:18.000000 radomermbg-0.0.9/radomermbg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 11:58:18.000000 radomermbg-0.0.9/radomermbg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 11:58:18.000000 radomermbg-0.0.9/radomermbg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 11:58:19.000000 radomermbg-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1316 2023-06-30 11:58:00.000000 radomermbg-0.0.9/setup.py
```

### Comparing `radomermbg-0.0.8/LICENSE.txt` & `radomermbg-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `radomermbg-0.0.8/radomermbg/radomer.py` & `radomermbg-0.0.9/radomermbg/radomer.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 import torch
 import  cv2
 import numpy as np
 from ultralytics import YOLO
 
 import os 
 import gdown
+from os.path import exists as file_exists
 
-
-gdown.download('https://drive.google.com/file/d/1DXFI6oY8087JlgVN2JkHKAki9tevCiVt/view?usp=drive_link','best_test_platform_elas.pt',
-    quiet=False,fuzzy=True)
+if file_exists('best_test_platform_elas.pt'):
+	pass 
+else:
+	gdown.download('https://drive.google.com/file/d/1DXFI6oY8087JlgVN2JkHKAki9tevCiVt/view?usp=drive_link','best_test_platform_elas.pt',
+	    quiet=False,fuzzy=True)
 
 # Load a model
 model = YOLO('best_test_platform_elas.pt')  # load a custom model
 
 # Predict with the model
 
 def background(img):
```

### Comparing `radomermbg-0.0.8/setup.py` & `radomermbg-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 from setuptools import setup, find_packages
 setup(
   name = 'radomermbg',         # How you named your package folder (MyLib)
   packages = find_packages(),   # Chose the same as "name"
-  version = '0.0.8',      # Start with a small number and increase it with every change you make
+  version = '0.0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'background removal',   # Give a short description about your library
   author = 'SARVESH,SRIDHARAN,PRIYANKA', 
   url = '',                  # Type in your name
   author_email = 'cvradome@gmail.com',      # Type in your E-Mail
   keywords = ['background', 'subtraction'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
```

