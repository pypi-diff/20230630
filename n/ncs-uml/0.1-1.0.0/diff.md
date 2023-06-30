# Comparing `tmp/ncs-uml-0.1.tar.gz` & `tmp/ncs-uml-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncs-uml-0.1.tar", last modified: Fri Jun 30 20:13:51 2023, max compression
+gzip compressed data, was "ncs-uml-1.0.0.tar", last modified: Fri Jun 30 20:25:06 2023, max compression
```

## Comparing `ncs-uml-0.1.tar` & `ncs-uml-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:13:51.386250 ncs-uml-0.1/
--rw-r--r--   0 kkotari    (501) staff       (20)        3 2023-06-23 13:30:52.000000 ncs-uml-0.1/.version
--rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-0.1/LICENSE
--rw-r--r--   0 kkotari    (501) staff       (20)       75 2023-06-23 13:29:14.000000 ncs-uml-0.1/MANIFEST.in
--rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 20:13:51.386083 ncs-uml-0.1/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)        9 2023-06-23 13:12:35.000000 ncs-uml-0.1/README.md
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:13:51.384784 ncs-uml-0.1/ncs_uml/
--rw-r--r--   0 kkotari    (501) staff       (20)      138 2023-06-30 18:42:48.000000 ncs-uml-0.1/ncs_uml/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5528 2023-06-30 20:12:43.000000 ncs-uml-0.1/ncs_uml/main.py
--rw-r--r--   0 kkotari    (501) staff       (20)      639 2023-06-24 00:35:50.000000 ncs-uml-0.1/ncs_uml/run.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5981 2023-06-30 20:08:47.000000 ncs-uml-0.1/ncs_uml/utils.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:13:51.385855 ncs-uml-0.1/ncs_uml.egg-info/
--rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 20:13:51.000000 ncs-uml-0.1/ncs_uml.egg-info/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)      320 2023-06-30 20:13:51.000000 ncs-uml-0.1/ncs_uml.egg-info/SOURCES.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-06-30 20:13:51.000000 ncs-uml-0.1/ncs_uml.egg-info/dependency_links.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       71 2023-06-30 20:13:51.000000 ncs-uml-0.1/ncs_uml.egg-info/entry_points.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-30 20:13:51.000000 ncs-uml-0.1/ncs_uml.egg-info/requires.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-06-30 20:13:51.000000 ncs-uml-0.1/ncs_uml.egg-info/top_level.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-0.1/requirements.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-06-30 20:13:51.386302 ncs-uml-0.1/setup.cfg
--rw-r--r--   0 kkotari    (501) staff       (20)     1784 2023-06-23 14:31:02.000000 ncs-uml-0.1/setup.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:25:06.832288 ncs-uml-1.0.0/
+-rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.0.0/LICENSE
+-rw-r--r--   0 kkotari    (501) staff       (20)       75 2023-06-23 13:29:14.000000 ncs-uml-1.0.0/MANIFEST.in
+-rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 20:25:06.832105 ncs-uml-1.0.0/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)        9 2023-06-23 13:12:35.000000 ncs-uml-1.0.0/README.md
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:25:06.830788 ncs-uml-1.0.0/ncs_uml/
+-rw-r--r--   0 kkotari    (501) staff       (20)      248 2023-06-30 20:23:43.000000 ncs-uml-1.0.0/ncs_uml/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5528 2023-06-30 20:12:43.000000 ncs-uml-1.0.0/ncs_uml/main.py
+-rw-r--r--   0 kkotari    (501) staff       (20)      639 2023-06-24 00:35:50.000000 ncs-uml-1.0.0/ncs_uml/run.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5981 2023-06-30 20:08:47.000000 ncs-uml-1.0.0/ncs_uml/utils.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:25:06.831870 ncs-uml-1.0.0/ncs_uml.egg-info/
+-rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)      311 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/SOURCES.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/dependency_links.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       71 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/entry_points.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/requires.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/top_level.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.0.0/requirements.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-06-30 20:25:06.832346 ncs-uml-1.0.0/setup.cfg
+-rw-r--r--   0 kkotari    (501) staff       (20)     1683 2023-06-30 20:23:16.000000 ncs-uml-1.0.0/setup.py
```

### Comparing `ncs-uml-0.1/LICENSE` & `ncs-uml-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ncs-uml-0.1/PKG-INFO` & `ncs-uml-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 0.1
-Summary: ncs-uml is the smartway to generate the plantuml code from yang file/s
+Version: 1.0.0
+Summary: ncs-uml is the smartway to generate the plantuml code from yang file
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ncs-uml-0.1/ncs_uml/main.py` & `ncs-uml-1.0.0/ncs_uml/main.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-0.1/ncs_uml/run.py` & `ncs-uml-1.0.0/ncs_uml/run.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-0.1/ncs_uml/utils.py` & `ncs-uml-1.0.0/ncs_uml/utils.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-0.1/ncs_uml.egg-info/PKG-INFO` & `ncs-uml-1.0.0/ncs_uml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 0.1
-Summary: ncs-uml is the smartway to generate the plantuml code from yang file/s
+Version: 1.0.0
+Summary: ncs-uml is the smartway to generate the plantuml code from yang file
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ncs-uml-0.1/setup.py` & `ncs-uml-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from setuptools import setup, find_packages
 from os import path
 from io import open
 
+import ncs_uml
+
 here = path.abspath(path.dirname(__file__))
 reqs = []
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-with open(path.join(here, '.version'), encoding='utf-8') as f:
-    version = f.read()
-
 with open(path.join(here, 'requirements.txt'), encoding='utf-8') as f:
     read_lines = f.readlines()
     reqs = [each.strip() for each in read_lines]
 
 setup(
-    name = 'ncs-uml',
-    version = version,
-    description = "ncs-uml is the smartway to generate the plantuml code from yang file/s",
+    name = ncs_uml.__name__,
+    version = ncs_uml.__version__,
+    description = ncs_uml.__description__,
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/kirankotari/ncs-uml.git',
     author = 'Kiran Kumar Kotari',
     author_email = 'kirankotari@live.com',
     entry_points={
         'console_scripts': [
```

