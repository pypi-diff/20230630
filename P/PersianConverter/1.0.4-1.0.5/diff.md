# Comparing `tmp/PersianConverter-1.0.4.tar.gz` & `tmp/PersianConverter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PersianConverter-1.0.4.tar", last modified: Fri Jun 30 16:19:07 2023, max compression
+gzip compressed data, was "PersianConverter-1.0.5.tar", last modified: Fri Jun 30 16:23:15 2023, max compression
```

## Comparing `PersianConverter-1.0.4.tar` & `PersianConverter-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 16:19:07.182030 PersianConverter-1.0.4/
--rw-rw-rw-   0        0        0      865 2023-06-30 16:19:07.181030 PersianConverter-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 16:19:07.177034 PersianConverter-1.0.4/PersianConverter.egg-info/
--rw-rw-rw-   0        0        0      865 2023-06-30 16:19:06.000000 PersianConverter-1.0.4/PersianConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-30 16:19:07.000000 PersianConverter-1.0.4/PersianConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 16:19:06.000000 PersianConverter-1.0.4/PersianConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-30 16:19:06.000000 PersianConverter-1.0.4/PersianConverter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-30 16:19:06.000000 PersianConverter-1.0.4/PersianConverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-30 16:19:06.000000 PersianConverter-1.0.4/PersianConverter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 16:19:07.180030 PersianConverter-1.0.4/persian_converter/
--rw-rw-rw-   0        0        0      298 2023-06-30 13:39:29.000000 PersianConverter-1.0.4/persian_converter/__init__.py
--rw-rw-rw-   0        0        0      369 2023-06-30 13:14:23.000000 PersianConverter-1.0.4/persian_converter/converter.py
--rw-rw-rw-   0        0        0       42 2023-06-30 16:19:07.182030 PersianConverter-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1312 2023-06-30 16:18:36.000000 PersianConverter-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:23:15.492541 PersianConverter-1.0.5/
+-rw-rw-rw-   0        0        0      865 2023-06-30 16:23:15.492541 PersianConverter-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 16:23:15.492541 PersianConverter-1.0.5/PersianConverter.egg-info/
+-rw-rw-rw-   0        0        0      865 2023-06-30 16:23:15.000000 PersianConverter-1.0.5/PersianConverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-30 16:23:15.000000 PersianConverter-1.0.5/PersianConverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 16:23:15.000000 PersianConverter-1.0.5/PersianConverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-30 16:23:15.000000 PersianConverter-1.0.5/PersianConverter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-30 16:23:15.000000 PersianConverter-1.0.5/PersianConverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-30 16:23:15.000000 PersianConverter-1.0.5/PersianConverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3155 2023-06-30 16:17:55.000000 PersianConverter-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 16:23:15.492541 PersianConverter-1.0.5/persian_converter/
+-rw-rw-rw-   0        0        0      298 2023-06-30 13:39:29.000000 PersianConverter-1.0.5/persian_converter/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-06-30 13:14:23.000000 PersianConverter-1.0.5/persian_converter/converter.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 16:23:15.492541 PersianConverter-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1312 2023-06-30 16:22:57.000000 PersianConverter-1.0.5/setup.py
```

### Comparing `PersianConverter-1.0.4/PKG-INFO` & `PersianConverter-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PersianConverter
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for converting Persian text
 Home-page: https://github.com/komeylian/PersianConverter
 Author: Hamidreza Komeylian
 Author-email: komeylian@gmail.com
 License: MIT
 Keywords: Persian,text conversion
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PersianConverter-1.0.4/PersianConverter.egg-info/PKG-INFO` & `PersianConverter-1.0.5/PersianConverter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PersianConverter
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for converting Persian text
 Home-page: https://github.com/komeylian/PersianConverter
 Author: Hamidreza Komeylian
 Author-email: komeylian@gmail.com
 License: MIT
 Keywords: Persian,text conversion
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PersianConverter-1.0.4/setup.py` & `PersianConverter-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PersianConverter',
-    version='1.0.4',
+    version='1.0.5',
     packages=['persian_converter'],
     install_requires=[
         'arabic_reshaper',
         'python-bidi'
     ],
     author='Hamidreza Komeylian',
     author_email='komeylian@gmail.com',
```

