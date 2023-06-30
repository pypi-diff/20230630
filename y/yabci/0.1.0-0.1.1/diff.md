# Comparing `tmp/yabci-0.1.0.tar.gz` & `tmp/yabci-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yabci-0.1.0.tar", last modified: Fri Jun 30 20:23:29 2023, max compression
+gzip compressed data, was "yabci-0.1.1.tar", last modified: Fri Jun 30 20:52:07 2023, max compression
```

## Comparing `yabci-0.1.0.tar` & `yabci-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bob       (1000) bob       (1001)        0 2023-06-30 20:23:29.651971 yabci-0.1.0/
--rw-r--r--   0 bob       (1000) bob       (1001)    34523 2023-06-30 17:06:17.000000 yabci-0.1.0/LICENSE
--rw-r--r--   0 bob       (1000) bob       (1001)    47728 2023-06-30 20:23:29.651971 yabci-0.1.0/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1001)     7240 2023-06-30 19:52:28.000000 yabci-0.1.0/README.md
--rw-r--r--   0 bob       (1000) bob       (1001)      847 2023-06-30 20:19:20.000000 yabci-0.1.0/pyproject.toml
--rw-r--r--   0 bob       (1000) bob       (1001)       38 2023-06-30 20:23:29.651971 yabci-0.1.0/setup.cfg
-drwxr-xr-x   0 bob       (1000) bob       (1001)        0 2023-06-30 20:23:29.651971 yabci-0.1.0/src/
--rw-r--r--   0 bob       (1000) bob       (1001)        0 2023-06-27 21:12:36.000000 yabci-0.1.0/src/__init__.py
--rw-r--r--   0 bob       (1000) bob       (1001)     9386 2023-06-30 19:36:45.000000 yabci-0.1.0/src/importer.py
--rw-r--r--   0 bob       (1000) bob       (1001)      426 2023-06-29 15:54:04.000000 yabci-0.1.0/src/logger.py
--rw-r--r--   0 bob       (1000) bob       (1001)     4258 2023-06-29 16:14:58.000000 yabci-0.1.0/src/utils.py
-drwxr-xr-x   0 bob       (1000) bob       (1001)        0 2023-06-30 20:23:29.651971 yabci-0.1.0/src/yabci.egg-info/
--rw-r--r--   0 bob       (1000) bob       (1001)    47728 2023-06-30 20:23:29.000000 yabci-0.1.0/src/yabci.egg-info/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1001)      301 2023-06-30 20:23:29.000000 yabci-0.1.0/src/yabci.egg-info/SOURCES.txt
--rw-r--r--   0 bob       (1000) bob       (1001)        1 2023-06-30 20:23:29.000000 yabci-0.1.0/src/yabci.egg-info/dependency_links.txt
--rw-r--r--   0 bob       (1000) bob       (1001)       42 2023-06-30 20:23:29.000000 yabci-0.1.0/src/yabci.egg-info/requires.txt
--rw-r--r--   0 bob       (1000) bob       (1001)       31 2023-06-30 20:23:29.000000 yabci-0.1.0/src/yabci.egg-info/top_level.txt
-drwxr-xr-x   0 bob       (1000) bob       (1001)        0 2023-06-30 20:23:29.651971 yabci-0.1.0/tests/
--rw-r--r--   0 bob       (1000) bob       (1001)     2356 2023-06-30 16:10:49.000000 yabci-0.1.0/tests/test_examples.py
--rw-r--r--   0 bob       (1000) bob       (1001)     4413 2023-06-30 19:30:38.000000 yabci-0.1.0/tests/test_importer.py
+drwxr-xr-x   0 bob       (1000) bob       (1001)        0 2023-06-30 20:52:07.433999 yabci-0.1.1/
+-rw-r--r--   0 bob       (1000) bob       (1001)    34523 2023-06-30 17:06:17.000000 yabci-0.1.1/LICENSE
+-rw-r--r--   0 bob       (1000) bob       (1001)    47780 2023-06-30 20:52:07.433999 yabci-0.1.1/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1001)     7240 2023-06-30 19:52:28.000000 yabci-0.1.1/README.md
+-rw-r--r--   0 bob       (1000) bob       (1001)      899 2023-06-30 20:42:14.000000 yabci-0.1.1/pyproject.toml
+-rw-r--r--   0 bob       (1000) bob       (1001)       38 2023-06-30 20:52:07.433999 yabci-0.1.1/setup.cfg
+drwxr-xr-x   0 bob       (1000) bob       (1001)        0 2023-06-30 20:52:07.430666 yabci-0.1.1/src/
+-rw-r--r--   0 bob       (1000) bob       (1001)        0 2023-06-27 21:12:36.000000 yabci-0.1.1/src/__init__.py
+-rw-r--r--   0 bob       (1000) bob       (1001)     9386 2023-06-30 19:36:45.000000 yabci-0.1.1/src/importer.py
+-rw-r--r--   0 bob       (1000) bob       (1001)      426 2023-06-29 15:54:04.000000 yabci-0.1.1/src/logger.py
+-rw-r--r--   0 bob       (1000) bob       (1001)     4258 2023-06-29 16:14:58.000000 yabci-0.1.1/src/utils.py
+drwxr-xr-x   0 bob       (1000) bob       (1001)        0 2023-06-30 20:52:07.430666 yabci-0.1.1/src/yabci.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1001)    47780 2023-06-30 20:52:07.000000 yabci-0.1.1/src/yabci.egg-info/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1001)      301 2023-06-30 20:52:07.000000 yabci-0.1.1/src/yabci.egg-info/SOURCES.txt
+-rw-r--r--   0 bob       (1000) bob       (1001)        1 2023-06-30 20:52:07.000000 yabci-0.1.1/src/yabci.egg-info/dependency_links.txt
+-rw-r--r--   0 bob       (1000) bob       (1001)       42 2023-06-30 20:52:07.000000 yabci-0.1.1/src/yabci.egg-info/requires.txt
+-rw-r--r--   0 bob       (1000) bob       (1001)       31 2023-06-30 20:52:07.000000 yabci-0.1.1/src/yabci.egg-info/top_level.txt
+drwxr-xr-x   0 bob       (1000) bob       (1001)        0 2023-06-30 20:52:07.433999 yabci-0.1.1/tests/
+-rw-r--r--   0 bob       (1000) bob       (1001)     2356 2023-06-30 16:10:49.000000 yabci-0.1.1/tests/test_examples.py
+-rw-r--r--   0 bob       (1000) bob       (1001)     4413 2023-06-30 19:30:38.000000 yabci-0.1.1/tests/test_importer.py
```

### Comparing `yabci-0.1.0/LICENSE` & `yabci-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yabci-0.1.0/PKG-INFO` & `yabci-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yabci
-Version: 0.1.0
-Summary: Yet another beancount importer
+Version: 0.1.1
+Summary: Yet another beancount importer - import any file formats, with total customization
 Author: privatize-koala
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `yabci-0.1.0/README.md` & `yabci-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yabci-0.1.0/pyproject.toml` & `yabci-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "yabci"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="privatize-koala" },
 ]
-description = "Yet another beancount importer"
+description = "Yet another beancount importer - import any file formats, with total customization"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
```

### Comparing `yabci-0.1.0/src/importer.py` & `yabci-0.1.1/src/importer.py`

 * *Files identical despite different names*

### Comparing `yabci-0.1.0/src/utils.py` & `yabci-0.1.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `yabci-0.1.0/src/yabci.egg-info/PKG-INFO` & `yabci-0.1.1/src/yabci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yabci
-Version: 0.1.0
-Summary: Yet another beancount importer
+Version: 0.1.1
+Summary: Yet another beancount importer - import any file formats, with total customization
 Author: privatize-koala
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `yabci-0.1.0/tests/test_examples.py` & `yabci-0.1.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `yabci-0.1.0/tests/test_importer.py` & `yabci-0.1.1/tests/test_importer.py`

 * *Files identical despite different names*

