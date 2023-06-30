# Comparing `tmp/PersianConverter-1.0.2.tar.gz` & `tmp/PersianConverter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PersianConverter-1.0.2.tar", last modified: Fri Jun 30 13:32:33 2023, max compression
+gzip compressed data, was "PersianConverter-1.0.3.tar", last modified: Fri Jun 30 13:40:12 2023, max compression
```

## Comparing `PersianConverter-1.0.2.tar` & `PersianConverter-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 13:32:33.617403 PersianConverter-1.0.2/
--rw-rw-rw-   0        0        0      865 2023-06-30 13:32:33.616407 PersianConverter-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 13:32:33.610414 PersianConverter-1.0.2/PersianConverter.egg-info/
--rw-rw-rw-   0        0        0      865 2023-06-30 13:32:33.000000 PersianConverter-1.0.2/PersianConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-30 13:32:33.000000 PersianConverter-1.0.2/PersianConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 13:32:33.000000 PersianConverter-1.0.2/PersianConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-30 13:32:33.000000 PersianConverter-1.0.2/PersianConverter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-30 13:32:33.000000 PersianConverter-1.0.2/PersianConverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-30 13:32:33.000000 PersianConverter-1.0.2/PersianConverter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 13:32:33.614408 PersianConverter-1.0.2/persian_converter/
--rw-rw-rw-   0        0        0        0 2023-06-30 13:30:34.000000 PersianConverter-1.0.2/persian_converter/__init__.py
--rw-rw-rw-   0        0        0      369 2023-06-30 13:14:23.000000 PersianConverter-1.0.2/persian_converter/converter.py
--rw-rw-rw-   0        0        0       42 2023-06-30 13:32:33.617403 PersianConverter-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1312 2023-06-30 13:32:09.000000 PersianConverter-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:40:12.984400 PersianConverter-1.0.3/
+-rw-rw-rw-   0        0        0      865 2023-06-30 13:40:12.980894 PersianConverter-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 13:40:12.965283 PersianConverter-1.0.3/PersianConverter.egg-info/
+-rw-rw-rw-   0        0        0      865 2023-06-30 13:40:12.000000 PersianConverter-1.0.3/PersianConverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-30 13:40:12.000000 PersianConverter-1.0.3/PersianConverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 13:40:12.000000 PersianConverter-1.0.3/PersianConverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-30 13:40:12.000000 PersianConverter-1.0.3/PersianConverter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-30 13:40:12.000000 PersianConverter-1.0.3/PersianConverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-30 13:40:12.000000 PersianConverter-1.0.3/PersianConverter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 13:40:12.980894 PersianConverter-1.0.3/persian_converter/
+-rw-rw-rw-   0        0        0      298 2023-06-30 13:39:29.000000 PersianConverter-1.0.3/persian_converter/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-06-30 13:14:23.000000 PersianConverter-1.0.3/persian_converter/converter.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 13:40:12.984400 PersianConverter-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1312 2023-06-30 13:39:55.000000 PersianConverter-1.0.3/setup.py
```

### Comparing `PersianConverter-1.0.2/PKG-INFO` & `PersianConverter-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PersianConverter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for converting Persian text
 Home-page: https://github.com/komeylian/PersianConverter
 Author: Hamidreza Komeylian
 Author-email: komeylian@gmail.com
 License: MIT
 Keywords: Persian,text conversion
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PersianConverter-1.0.2/PersianConverter.egg-info/PKG-INFO` & `PersianConverter-1.0.3/PersianConverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PersianConverter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for converting Persian text
 Home-page: https://github.com/komeylian/PersianConverter
 Author: Hamidreza Komeylian
 Author-email: komeylian@gmail.com
 License: MIT
 Keywords: Persian,text conversion
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PersianConverter-1.0.2/setup.py` & `PersianConverter-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PersianConverter',
-    version='1.0.2',
+    version='1.0.3',
     packages=['persian_converter'],
     install_requires=[
         'arabic_reshaper',
         'python-bidi'
     ],
     author='Hamidreza Komeylian',
     author_email='komeylian@gmail.com',
```

