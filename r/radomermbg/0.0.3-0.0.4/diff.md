# Comparing `tmp/radomermbg-0.0.3.tar.gz` & `tmp/radomermbg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\radomermbg-0.0.3.tar", last modified: Fri Jun 30 11:02:22 2023, max compression
+gzip compressed data, was "dist\radomermbg-0.0.4.tar", last modified: Fri Jun 30 11:04:09 2023, max compression
```

## Comparing `radomermbg-0.0.3.tar` & `radomermbg-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 11:02:22.000000 radomermbg-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-06-30 10:03:26.000000 radomermbg-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-06-30 10:00:42.000000 radomermbg-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      494 2023-06-30 11:02:22.000000 radomermbg-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-06-30 09:59:40.000000 radomermbg-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 11:02:22.000000 radomermbg-0.0.3/radomermbg.egg-info/
--rw-rw-rw-   0        0        0      494 2023-06-30 11:02:21.000000 radomermbg-0.0.3/radomermbg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-06-30 11:02:22.000000 radomermbg-0.0.3/radomermbg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 11:02:21.000000 radomermbg-0.0.3/radomermbg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 11:02:21.000000 radomermbg-0.0.3/radomermbg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 11:02:21.000000 radomermbg-0.0.3/radomermbg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 11:02:22.000000 radomermbg-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1316 2023-06-30 11:02:18.000000 radomermbg-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:04:09.000000 radomermbg-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-06-30 10:03:26.000000 radomermbg-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-06-30 10:00:42.000000 radomermbg-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      494 2023-06-30 11:04:09.000000 radomermbg-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-06-30 09:59:40.000000 radomermbg-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 11:04:09.000000 radomermbg-0.0.4/radomermbg.egg-info/
+-rw-rw-rw-   0        0        0      494 2023-06-30 11:04:09.000000 radomermbg-0.0.4/radomermbg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-06-30 11:04:09.000000 radomermbg-0.0.4/radomermbg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:04:09.000000 radomermbg-0.0.4/radomermbg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 11:04:09.000000 radomermbg-0.0.4/radomermbg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:04:09.000000 radomermbg-0.0.4/radomermbg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 11:04:09.000000 radomermbg-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1316 2023-06-30 11:04:01.000000 radomermbg-0.0.4/setup.py
```

### Comparing `radomermbg-0.0.3/LICENSE.txt` & `radomermbg-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `radomermbg-0.0.3/setup.py` & `radomermbg-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 from setuptools import setup, find_packages
 setup(
   name = 'radomermbg',         # How you named your package folder (MyLib)
   packages = find_packages(),   # Chose the same as "name"
-  version = '0.0.3',      # Start with a small number and increase it with every change you make
+  version = '0.0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'background removal',   # Give a short description about your library
   author = 'SARVESH,SRIDHARAN,PRIYANKA', 
   url = '',                  # Type in your name
   author_email = 'cvradome@gmail.com',      # Type in your E-Mail
   keywords = ['background', 'subtraction'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
```

