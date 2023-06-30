# Comparing `tmp/PersianConverter-1.0.8.tar.gz` & `tmp/PersianConverter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PersianConverter-1.0.8.tar", last modified: Fri Jun 30 16:37:12 2023, max compression
+gzip compressed data, was "PersianConverter-1.0.9.tar", last modified: Fri Jun 30 16:39:05 2023, max compression
```

## Comparing `PersianConverter-1.0.8.tar` & `PersianConverter-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 16:37:12.335711 PersianConverter-1.0.8/
--rw-rw-rw-   0        0        0     4285 2023-06-30 16:37:12.335711 PersianConverter-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 16:37:12.335711 PersianConverter-1.0.8/PersianConverter.egg-info/
--rw-rw-rw-   0        0        0     4285 2023-06-30 16:37:12.000000 PersianConverter-1.0.8/PersianConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-30 16:37:12.000000 PersianConverter-1.0.8/PersianConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 16:37:12.000000 PersianConverter-1.0.8/PersianConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-30 16:37:12.000000 PersianConverter-1.0.8/PersianConverter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-30 16:37:12.000000 PersianConverter-1.0.8/PersianConverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-30 16:37:12.000000 PersianConverter-1.0.8/PersianConverter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 16:37:12.335711 PersianConverter-1.0.8/persian_converter/
--rw-rw-rw-   0        0        0      298 2023-06-30 13:39:29.000000 PersianConverter-1.0.8/persian_converter/__init__.py
--rw-rw-rw-   0        0        0      369 2023-06-30 13:14:23.000000 PersianConverter-1.0.8/persian_converter/converter.py
--rw-rw-rw-   0        0        0       42 2023-06-30 16:37:12.335711 PersianConverter-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     4739 2023-06-30 16:36:40.000000 PersianConverter-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:39:05.558900 PersianConverter-1.0.9/
+-rw-rw-rw-   0        0        0     4287 2023-06-30 16:39:05.558900 PersianConverter-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 16:39:05.558900 PersianConverter-1.0.9/PersianConverter.egg-info/
+-rw-rw-rw-   0        0        0     4287 2023-06-30 16:39:05.000000 PersianConverter-1.0.9/PersianConverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-30 16:39:05.000000 PersianConverter-1.0.9/PersianConverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 16:39:05.000000 PersianConverter-1.0.9/PersianConverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-30 16:39:05.000000 PersianConverter-1.0.9/PersianConverter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-30 16:39:05.000000 PersianConverter-1.0.9/PersianConverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-30 16:39:05.000000 PersianConverter-1.0.9/PersianConverter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 16:39:05.558900 PersianConverter-1.0.9/persian_converter/
+-rw-rw-rw-   0        0        0      298 2023-06-30 13:39:29.000000 PersianConverter-1.0.9/persian_converter/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-06-30 13:14:23.000000 PersianConverter-1.0.9/persian_converter/converter.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 16:39:05.558900 PersianConverter-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     4738 2023-06-30 16:38:46.000000 PersianConverter-1.0.9/setup.py
```

### Comparing `PersianConverter-1.0.8/PKG-INFO` & `PersianConverter-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PersianConverter
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for converting Persian text
 Home-page: https://github.com/komeylian/PersianConverter
 Author: Hamidreza Komeylian
 Author-email: komeylian@gmail.com
 License: MIT
 Keywords: Persian,text conversion
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
+
     A package for converting Persian text. This package provides functions to reshape and display Persian text.
     
     # PersianConverter
     
     [![PyPI version](https://img.shields.io/pypi/v/PersianConverter.svg)](https://pypi.org/project/PersianConverter/)
     [![License](https://img.shields.io/pypi/l/PersianConverter.svg)](https://github.com/your_username/PersianConverter/blob/main/LICENSE)
```

### Comparing `PersianConverter-1.0.8/PersianConverter.egg-info/PKG-INFO` & `PersianConverter-1.0.9/PersianConverter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PersianConverter
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for converting Persian text
 Home-page: https://github.com/komeylian/PersianConverter
 Author: Hamidreza Komeylian
 Author-email: komeylian@gmail.com
 License: MIT
 Keywords: Persian,text conversion
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
+
     A package for converting Persian text. This package provides functions to reshape and display Persian text.
     
     # PersianConverter
     
     [![PyPI version](https://img.shields.io/pypi/v/PersianConverter.svg)](https://pypi.org/project/PersianConverter/)
     [![License](https://img.shields.io/pypi/l/PersianConverter.svg)](https://github.com/your_username/PersianConverter/blob/main/LICENSE)
```

### Comparing `PersianConverter-1.0.8/setup.py` & `PersianConverter-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PersianConverter',
-    version='1.0.8',
+    version='1.0.9',
     packages=['persian_converter'],
     install_requires=[
         'arabic_reshaper',
         'python-bidi'
     ],
     author='Hamidreza Komeylian',
     author_email='komeylian@gmail.com',
@@ -21,15 +21,15 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    long_description='''\
+    long_description='''
     A package for converting Persian text. This package provides functions to reshape and display Persian text.
     
     # PersianConverter
     
     [![PyPI version](https://img.shields.io/pypi/v/PersianConverter.svg)](https://pypi.org/project/PersianConverter/)
     [![License](https://img.shields.io/pypi/l/PersianConverter.svg)](https://github.com/your_username/PersianConverter/blob/main/LICENSE)
```

