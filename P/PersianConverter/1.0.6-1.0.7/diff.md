# Comparing `tmp/PersianConverter-1.0.6.tar.gz` & `tmp/PersianConverter-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PersianConverter-1.0.6.tar", last modified: Fri Jun 30 16:31:07 2023, max compression
+gzip compressed data, was "PersianConverter-1.0.7.tar", last modified: Fri Jun 30 16:33:39 2023, max compression
```

## Comparing `PersianConverter-1.0.6.tar` & `PersianConverter-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 16:31:07.204955 PersianConverter-1.0.6/
--rw-rw-rw-   0        0        0     4044 2023-06-30 16:31:07.204955 PersianConverter-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 16:31:07.189331 PersianConverter-1.0.6/PersianConverter.egg-info/
--rw-rw-rw-   0        0        0     4044 2023-06-30 16:31:07.000000 PersianConverter-1.0.6/PersianConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-30 16:31:07.000000 PersianConverter-1.0.6/PersianConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 16:31:07.000000 PersianConverter-1.0.6/PersianConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-30 16:31:07.000000 PersianConverter-1.0.6/PersianConverter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-30 16:31:07.000000 PersianConverter-1.0.6/PersianConverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-30 16:31:07.000000 PersianConverter-1.0.6/PersianConverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3155 2023-06-30 16:17:55.000000 PersianConverter-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 16:31:07.204955 PersianConverter-1.0.6/persian_converter/
--rw-rw-rw-   0        0        0      298 2023-06-30 13:39:29.000000 PersianConverter-1.0.6/persian_converter/__init__.py
--rw-rw-rw-   0        0        0      369 2023-06-30 13:14:23.000000 PersianConverter-1.0.6/persian_converter/converter.py
--rw-rw-rw-   0        0        0       42 2023-06-30 16:31:07.204955 PersianConverter-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     4495 2023-06-30 16:30:48.000000 PersianConverter-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:33:39.852956 PersianConverter-1.0.7/
+-rw-rw-rw-   0        0        0     4050 2023-06-30 16:33:39.852956 PersianConverter-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 16:33:39.852956 PersianConverter-1.0.7/PersianConverter.egg-info/
+-rw-rw-rw-   0        0        0     4050 2023-06-30 16:33:39.000000 PersianConverter-1.0.7/PersianConverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-30 16:33:39.000000 PersianConverter-1.0.7/PersianConverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 16:33:39.000000 PersianConverter-1.0.7/PersianConverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-30 16:33:39.000000 PersianConverter-1.0.7/PersianConverter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-30 16:33:39.000000 PersianConverter-1.0.7/PersianConverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-30 16:33:39.000000 PersianConverter-1.0.7/PersianConverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3155 2023-06-30 16:17:55.000000 PersianConverter-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 16:33:39.852956 PersianConverter-1.0.7/persian_converter/
+-rw-rw-rw-   0        0        0      298 2023-06-30 13:39:29.000000 PersianConverter-1.0.7/persian_converter/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-06-30 13:14:23.000000 PersianConverter-1.0.7/persian_converter/converter.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 16:33:39.852956 PersianConverter-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     4501 2023-06-30 16:33:12.000000 PersianConverter-1.0.7/setup.py
```

### Comparing `PersianConverter-1.0.6/PKG-INFO` & `PersianConverter-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PersianConverter
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for converting Persian text
 Home-page: https://github.com/komeylian/PersianConverter
 Author: Hamidreza Komeylian
 Author-email: komeylian@gmail.com
 License: MIT
 Keywords: Persian,text conversion
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 A package for converting Persian text. This package provides functions to reshape and display Persian text.
+    
     # PersianConverter
 
 [![PyPI version](https://img.shields.io/pypi/v/PersianConverter.svg)](https://pypi.org/project/PersianConverter/)
 [![License](https://img.shields.io/pypi/l/PersianConverter.svg)](https://github.com/your_username/PersianConverter/blob/main/LICENSE)
 
 PersianConverter is a Python package for converting Persian text. It provides functions to reshape Persian text, apply the bidirectional algorithm, and display Persian text using proper presentation forms.
```

### Comparing `PersianConverter-1.0.6/PersianConverter.egg-info/PKG-INFO` & `PersianConverter-1.0.7/PersianConverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PersianConverter
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for converting Persian text
 Home-page: https://github.com/komeylian/PersianConverter
 Author: Hamidreza Komeylian
 Author-email: komeylian@gmail.com
 License: MIT
 Keywords: Persian,text conversion
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 A package for converting Persian text. This package provides functions to reshape and display Persian text.
+    
     # PersianConverter
 
 [![PyPI version](https://img.shields.io/pypi/v/PersianConverter.svg)](https://pypi.org/project/PersianConverter/)
 [![License](https://img.shields.io/pypi/l/PersianConverter.svg)](https://github.com/your_username/PersianConverter/blob/main/LICENSE)
 
 PersianConverter is a Python package for converting Persian text. It provides functions to reshape Persian text, apply the bidirectional algorithm, and display Persian text using proper presentation forms.
```

### Comparing `PersianConverter-1.0.6/README.md` & `PersianConverter-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PersianConverter-1.0.6/setup.py` & `PersianConverter-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PersianConverter',
-    version='1.0.6',
+    version='1.0.7',
     packages=['persian_converter'],
     install_requires=[
         'arabic_reshaper',
         'python-bidi'
     ],
     author='Hamidreza Komeylian',
     author_email='komeylian@gmail.com',
@@ -22,14 +22,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     long_description='''A package for converting Persian text. This package provides functions to reshape and display Persian text.
+    
     # PersianConverter
 
 [![PyPI version](https://img.shields.io/pypi/v/PersianConverter.svg)](https://pypi.org/project/PersianConverter/)
 [![License](https://img.shields.io/pypi/l/PersianConverter.svg)](https://github.com/your_username/PersianConverter/blob/main/LICENSE)
 
 PersianConverter is a Python package for converting Persian text. It provides functions to reshape Persian text, apply the bidirectional algorithm, and display Persian text using proper presentation forms.
```

