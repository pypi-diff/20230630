# Comparing `tmp/allure_combine-1.0.7.tar.gz` & `tmp/allure_combine-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/allure_combine-1.0.7.tar", last modified: Mon Aug 22 09:56:57 2022, max compression
+gzip compressed data, was "dist/allure_combine-1.0.8.tar", last modified: Mon Aug 22 10:22:46 2022, max compression
```

## Comparing `allure_combine-1.0.7.tar` & `allure_combine-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mihanentalpo  (1000) mihanentalpo  (1000)        0 2022-08-22 09:56:57.000000 allure_combine-1.0.7/
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)     5422 2022-08-22 09:56:57.000000 allure_combine-1.0.7/PKG-INFO
-drwxr-xr-x   0 mihanentalpo  (1000) mihanentalpo  (1000)        0 2022-08-22 09:56:57.000000 allure_combine-1.0.7/allure_combine/
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)  2510779 2022-06-20 05:58:39.000000 allure_combine-1.0.7/allure_combine/sinon-9.2.4.js
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)    11742 2022-08-22 09:53:14.000000 allure_combine-1.0.7/allure_combine/combine.py
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       73 2022-06-19 11:12:12.000000 allure_combine-1.0.7/allure_combine/__init__.py
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)     3290 2022-08-22 09:56:25.000000 allure_combine-1.0.7/README.md
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       38 2022-08-22 09:56:57.000000 allure_combine-1.0.7/setup.cfg
-drwxr-xr-x   0 mihanentalpo  (1000) mihanentalpo  (1000)        0 2022-08-22 09:56:57.000000 allure_combine-1.0.7/allure_combine.egg-info/
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)     5422 2022-08-22 09:56:57.000000 allure_combine-1.0.7/allure_combine.egg-info/PKG-INFO
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)      331 2022-08-22 09:56:57.000000 allure_combine-1.0.7/allure_combine.egg-info/SOURCES.txt
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       15 2022-08-22 09:56:57.000000 allure_combine-1.0.7/allure_combine.egg-info/top_level.txt
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       11 2022-08-22 09:56:57.000000 allure_combine-1.0.7/allure_combine.egg-info/requires.txt
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       97 2022-08-22 09:56:57.000000 allure_combine-1.0.7/allure_combine.egg-info/entry_points.txt
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)        1 2022-08-22 09:56:57.000000 allure_combine-1.0.7/allure_combine.egg-info/dependency_links.txt
--rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)     1992 2022-08-22 09:54:33.000000 allure_combine-1.0.7/setup.py
+drwxr-xr-x   0 mihanentalpo  (1000) mihanentalpo  (1000)        0 2022-08-22 10:22:46.000000 allure_combine-1.0.8/
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)     5422 2022-08-22 10:22:46.000000 allure_combine-1.0.8/PKG-INFO
+drwxr-xr-x   0 mihanentalpo  (1000) mihanentalpo  (1000)        0 2022-08-22 10:22:46.000000 allure_combine-1.0.8/allure_combine/
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)  2510779 2022-06-20 05:58:39.000000 allure_combine-1.0.8/allure_combine/sinon-9.2.4.js
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)    11769 2022-08-22 10:01:32.000000 allure_combine-1.0.8/allure_combine/combine.py
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       73 2022-06-19 11:12:12.000000 allure_combine-1.0.8/allure_combine/__init__.py
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)     3290 2022-08-22 10:20:15.000000 allure_combine-1.0.8/README.md
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       38 2022-08-22 10:22:46.000000 allure_combine-1.0.8/setup.cfg
+drwxr-xr-x   0 mihanentalpo  (1000) mihanentalpo  (1000)        0 2022-08-22 10:22:46.000000 allure_combine-1.0.8/allure_combine.egg-info/
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)     5422 2022-08-22 10:22:46.000000 allure_combine-1.0.8/allure_combine.egg-info/PKG-INFO
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)      331 2022-08-22 10:22:46.000000 allure_combine-1.0.8/allure_combine.egg-info/SOURCES.txt
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       15 2022-08-22 10:22:46.000000 allure_combine-1.0.8/allure_combine.egg-info/top_level.txt
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       11 2022-08-22 10:22:46.000000 allure_combine-1.0.8/allure_combine.egg-info/requires.txt
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)       97 2022-08-22 10:22:46.000000 allure_combine-1.0.8/allure_combine.egg-info/entry_points.txt
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)        1 2022-08-22 10:22:46.000000 allure_combine-1.0.8/allure_combine.egg-info/dependency_links.txt
+-rw-r--r--   0 mihanentalpo  (1000) mihanentalpo  (1000)     1992 2022-08-22 10:20:39.000000 allure_combine-1.0.8/setup.py
```

### Comparing `allure_combine-1.0.7/PKG-INFO` & `allure_combine-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure_combine
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generate single HTML file from allure report.
 Home-page: https://github.com/MihanEntalpo/allure-single-html-file
 Author: MihanEntalpo, Sine.wang
 Author-email: mihanentalpo@yandex.ru, sinecelia.wang@gmail.com
 Maintainer: Sine.wang
 Maintainer-email: sinecelia.wang@gmail.com
 License: MIT
@@ -19,15 +19,15 @@
         1. Reads contents of allure-generated folder
         2. Creates server.js file, which has all the data files inside and code to start fake XHR server
         3. Patches index.html file, so it's using server.js and sinon-9.2.4.js (Taken from [here](https://sinonjs.org/)), and could be run in any browser without --allow-file-access-from-files parameter of chrome browser
         4. Creates file complete.html with all files built-in in a single file
         
         ## Requirements
         
-        * Python 3.5+
+        * Python 3.6+
         * You need to have your allure report folder generated (`allure generate './some/path/to/allure/generated/folder'`)
         
         ## Installation
         
         
         ### Install with pip
```

### Comparing `allure_combine-1.0.7/allure_combine/sinon-9.2.4.js` & `allure_combine-1.0.8/allure_combine/sinon-9.2.4.js`

 * *Files identical despite different names*

### Comparing `allure_combine-1.0.7/allure_combine/combine.py` & `allure_combine-1.0.8/allure_combine/combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         "svg": "image/svg",
         "txt": "text/plain;charset=UTF-8",
         "js": "application/javascript",
         "json": "application/json",
         "csv": "text/csv",
         "css": "text/css",
         "html": "text/html",
+        "xml": "text/xml",
         "htm": "text/html",
         "png": "image/png",
         "jpeg": "image/jpeg",
         "jpg": "image/jpg",
         "gif": "image/gif",
         "mp4": "video/mp4",
         "avi": "video/avi",
```

### Comparing `allure_combine-1.0.7/README.md` & `allure_combine-1.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 1. Reads contents of allure-generated folder
 2. Creates server.js file, which has all the data files inside and code to start fake XHR server
 3. Patches index.html file, so it's using server.js and sinon-9.2.4.js (Taken from [here](https://sinonjs.org/)), and could be run in any browser without --allow-file-access-from-files parameter of chrome browser
 4. Creates file complete.html with all files built-in in a single file
 
 ## Requirements
 
-* Python 3.5+
+* Python 3.6+
 * You need to have your allure report folder generated (`allure generate './some/path/to/allure/generated/folder'`)
 
 ## Installation
 
 
 ### Install with pip
```

### Comparing `allure_combine-1.0.7/allure_combine.egg-info/PKG-INFO` & `allure_combine-1.0.8/allure_combine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-combine
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generate single HTML file from allure report.
 Home-page: https://github.com/MihanEntalpo/allure-single-html-file
 Author: MihanEntalpo, Sine.wang
 Author-email: mihanentalpo@yandex.ru, sinecelia.wang@gmail.com
 Maintainer: Sine.wang
 Maintainer-email: sinecelia.wang@gmail.com
 License: MIT
@@ -19,15 +19,15 @@
         1. Reads contents of allure-generated folder
         2. Creates server.js file, which has all the data files inside and code to start fake XHR server
         3. Patches index.html file, so it's using server.js and sinon-9.2.4.js (Taken from [here](https://sinonjs.org/)), and could be run in any browser without --allow-file-access-from-files parameter of chrome browser
         4. Creates file complete.html with all files built-in in a single file
         
         ## Requirements
         
-        * Python 3.5+
+        * Python 3.6+
         * You need to have your allure report folder generated (`allure generate './some/path/to/allure/generated/folder'`)
         
         ## Installation
         
         
         ### Install with pip
```

### Comparing `allure_combine-1.0.7/setup.py` & `allure_combine-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name=PACKAGE_NAME,
-    version='1.0.7',
+    version='1.0.8',
     author='MihanEntalpo, Sine.wang',
     author_email='mihanentalpo@yandex.ru, sinecelia.wang@gmail.com',
     maintainer='Sine.wang',
     maintainer_email='sinecelia.wang@gmail.com',
     license='MIT',
     url='https://github.com/MihanEntalpo/allure-single-html-file',
     description='Generate single HTML file from allure report.',
```

