# Comparing `tmp/atc_easy_desktop-1.0.1.tar.gz` & `tmp/atc_easy_desktop-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atc_easy_desktop-1.0.1.tar", last modified: Thu Jun 29 17:07:37 2023, max compression
+gzip compressed data, was "atc_easy_desktop-1.0.2.tar", last modified: Thu Jun 29 17:22:00 2023, max compression
```

## Comparing `atc_easy_desktop-1.0.1.tar` & `atc_easy_desktop-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 17:07:37.974242 atc_easy_desktop-1.0.1/
--rw-rw-rw-   0        0        0     1144 2023-06-29 17:07:37.974242 atc_easy_desktop-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-06-29 16:41:49.000000 atc_easy_desktop-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 17:07:37.958616 atc_easy_desktop-1.0.1/atc_easy_desktop/
--rw-rw-rw-   0        0        0     1535 2023-06-29 16:12:27.000000 atc_easy_desktop-1.0.1/atc_easy_desktop/atc_easy_desktop.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:07:37.974242 atc_easy_desktop-1.0.1/atc_easy_desktop.egg-info/
--rw-rw-rw-   0        0        0     1144 2023-06-29 17:07:37.000000 atc_easy_desktop-1.0.1/atc_easy_desktop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-29 17:07:37.000000 atc_easy_desktop-1.0.1/atc_easy_desktop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 17:07:37.000000 atc_easy_desktop-1.0.1/atc_easy_desktop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 17:07:37.000000 atc_easy_desktop-1.0.1/atc_easy_desktop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 17:07:37.000000 atc_easy_desktop-1.0.1/atc_easy_desktop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 17:07:37.974242 atc_easy_desktop-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-06-29 17:07:32.000000 atc_easy_desktop-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:22:00.244385 atc_easy_desktop-1.0.2/
+-rw-rw-rw-   0        0        0     1144 2023-06-29 17:22:00.244385 atc_easy_desktop-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-06-29 16:41:49.000000 atc_easy_desktop-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 17:22:00.228759 atc_easy_desktop-1.0.2/atc_easy_desktop/
+-rw-rw-rw-   0        0        0       43 2023-06-29 17:21:07.000000 atc_easy_desktop-1.0.2/atc_easy_desktop/__init__.py
+-rw-rw-rw-   0        0        0     1535 2023-06-29 16:12:27.000000 atc_easy_desktop-1.0.2/atc_easy_desktop/atc_easy_desktop.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:22:00.244385 atc_easy_desktop-1.0.2/atc_easy_desktop.egg-info/
+-rw-rw-rw-   0        0        0     1144 2023-06-29 17:22:00.000000 atc_easy_desktop-1.0.2/atc_easy_desktop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-29 17:22:00.000000 atc_easy_desktop-1.0.2/atc_easy_desktop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 17:22:00.000000 atc_easy_desktop-1.0.2/atc_easy_desktop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 17:22:00.000000 atc_easy_desktop-1.0.2/atc_easy_desktop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 17:22:00.000000 atc_easy_desktop-1.0.2/atc_easy_desktop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 17:22:00.244385 atc_easy_desktop-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-06-29 17:21:17.000000 atc_easy_desktop-1.0.2/setup.py
```

### Comparing `atc_easy_desktop-1.0.1/PKG-INFO` & `atc_easy_desktop-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atc_easy_desktop
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thư viện sử dụng để code game trên màn hình desktop
 Author: Chienbg200
 Author-email: chienbg200400@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `atc_easy_desktop-1.0.1/README.md` & `atc_easy_desktop-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `atc_easy_desktop-1.0.1/atc_easy_desktop/atc_easy_desktop.py` & `atc_easy_desktop-1.0.2/atc_easy_desktop/atc_easy_desktop.py`

 * *Files identical despite different names*

### Comparing `atc_easy_desktop-1.0.1/atc_easy_desktop.egg-info/PKG-INFO` & `atc_easy_desktop-1.0.2/atc_easy_desktop.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atc-easy-desktop
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thư viện sử dụng để code game trên màn hình desktop
 Author: Chienbg200
 Author-email: chienbg200400@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `atc_easy_desktop-1.0.1/setup.py` & `atc_easy_desktop-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='atc_easy_desktop',
-    version='1.0.1',
+    version='1.0.2',
     description='Thư viện sử dụng để code game trên màn hình desktop',
     long_description=long_description,
     author='Chienbg200',
     author_email='chienbg200400@gmail.com',
     packages=['atc_easy_desktop'],
     install_requires=[
         'pywin32',
```

