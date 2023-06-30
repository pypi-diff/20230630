# Comparing `tmp/helloworld-rayaq-0.0.1.tar.gz` & `tmp/helloworld-rayaq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helloworld-rayaq-0.0.1.tar", last modified: Fri Jun 30 04:04:06 2023, max compression
+gzip compressed data, was "helloworld-rayaq-0.0.2.tar", last modified: Fri Jun 30 20:23:25 2023, max compression
```

## Comparing `helloworld-rayaq-0.0.1.tar` & `helloworld-rayaq-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 rayaq      (501) staff       (20)        0 2023-06-30 04:04:06.462102 helloworld-rayaq-0.0.1/
--rw-r--r--   0 rayaq      (501) staff       (20)      570 2023-06-30 04:04:06.461931 helloworld-rayaq-0.0.1/PKG-INFO
-drwxr-xr-x   0 rayaq      (501) staff       (20)        0 2023-06-30 04:04:06.459294 helloworld-rayaq-0.0.1/helloworld-rayaq/
--rw-r--r--   0 rayaq      (501) staff       (20)       41 2023-06-30 03:35:52.000000 helloworld-rayaq-0.0.1/helloworld-rayaq/__init__.py
--rw-r--r--   0 rayaq      (501) staff       (20)       54 2023-06-30 03:29:57.000000 helloworld-rayaq-0.0.1/helloworld-rayaq/helloworld.py
-drwxr-xr-x   0 rayaq      (501) staff       (20)        0 2023-06-30 04:04:06.461677 helloworld-rayaq-0.0.1/helloworld_rayaq.egg-info/
--rw-r--r--   0 rayaq      (501) staff       (20)      570 2023-06-30 04:04:06.000000 helloworld-rayaq-0.0.1/helloworld_rayaq.egg-info/PKG-INFO
--rw-r--r--   0 rayaq      (501) staff       (20)      228 2023-06-30 04:04:06.000000 helloworld-rayaq-0.0.1/helloworld_rayaq.egg-info/SOURCES.txt
--rw-r--r--   0 rayaq      (501) staff       (20)        1 2023-06-30 04:04:06.000000 helloworld-rayaq-0.0.1/helloworld_rayaq.egg-info/dependency_links.txt
--rw-r--r--   0 rayaq      (501) staff       (20)       17 2023-06-30 04:04:06.000000 helloworld-rayaq-0.0.1/helloworld_rayaq.egg-info/top_level.txt
--rw-r--r--   0 rayaq      (501) staff       (20)       38 2023-06-30 04:04:06.462152 helloworld-rayaq-0.0.1/setup.cfg
--rw-r--r--   0 rayaq      (501) staff       (20)     1029 2023-06-30 03:57:00.000000 helloworld-rayaq-0.0.1/setup.py
+drwxr-xr-x   0 rayaq      (501) staff       (20)        0 2023-06-30 20:23:25.935096 helloworld-rayaq-0.0.2/
+-rw-r--r--   0 rayaq      (501) staff       (20)      570 2023-06-30 20:23:25.934802 helloworld-rayaq-0.0.2/PKG-INFO
+drwxr-xr-x   0 rayaq      (501) staff       (20)        0 2023-06-30 20:23:25.932040 helloworld-rayaq-0.0.2/helloworld-rayaq/
+-rw-r--r--   0 rayaq      (501) staff       (20)       41 2023-06-30 03:35:52.000000 helloworld-rayaq-0.0.2/helloworld-rayaq/__init__.py
+-rw-r--r--   0 rayaq      (501) staff       (20)       54 2023-06-30 03:29:57.000000 helloworld-rayaq-0.0.2/helloworld-rayaq/helloworld.py
+drwxr-xr-x   0 rayaq      (501) staff       (20)        0 2023-06-30 20:23:25.934506 helloworld-rayaq-0.0.2/helloworld_rayaq.egg-info/
+-rw-r--r--   0 rayaq      (501) staff       (20)      570 2023-06-30 20:23:25.000000 helloworld-rayaq-0.0.2/helloworld_rayaq.egg-info/PKG-INFO
+-rw-r--r--   0 rayaq      (501) staff       (20)      228 2023-06-30 20:23:25.000000 helloworld-rayaq-0.0.2/helloworld_rayaq.egg-info/SOURCES.txt
+-rw-r--r--   0 rayaq      (501) staff       (20)        1 2023-06-30 20:23:25.000000 helloworld-rayaq-0.0.2/helloworld_rayaq.egg-info/dependency_links.txt
+-rw-r--r--   0 rayaq      (501) staff       (20)       17 2023-06-30 20:23:25.000000 helloworld-rayaq-0.0.2/helloworld_rayaq.egg-info/top_level.txt
+-rw-r--r--   0 rayaq      (501) staff       (20)       38 2023-06-30 20:23:25.935155 helloworld-rayaq-0.0.2/setup.cfg
+-rw-r--r--   0 rayaq      (501) staff       (20)     1029 2023-06-30 04:09:13.000000 helloworld-rayaq-0.0.2/setup.py
```

### Comparing `helloworld-rayaq-0.0.1/PKG-INFO` & `helloworld-rayaq-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helloworld-rayaq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Hello World Package
 Home-page: UNKNOWN
 Author: Rayaq Siddiqui
 Author-email: rayaq05@hotmail.com
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `helloworld-rayaq-0.0.1/helloworld_rayaq.egg-info/PKG-INFO` & `helloworld-rayaq-0.0.2/helloworld_rayaq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helloworld-rayaq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Hello World Package
 Home-page: UNKNOWN
 Author: Rayaq Siddiqui
 Author-email: rayaq05@hotmail.com
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `helloworld-rayaq-0.0.1/setup.py` & `helloworld-rayaq-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Python Hello World Package'
 LONG_DESCRIPTION = 'A Python Package that can print Hello, World'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="helloworld-rayaq",
```

