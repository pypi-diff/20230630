# Comparing `tmp/ns_asphalt9-0.0.1.tar.gz` & `tmp/ns_asphalt9-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.0.1.tar", last modified: Fri Jun 30 07:14:15 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.0.2.tar", last modified: Fri Jun 30 07:19:51 2023, max compression
```

## Comparing `ns_asphalt9-0.0.1.tar` & `ns_asphalt9-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:14:15.175400 ns_asphalt9-0.0.1/
--rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.1/LICENSE
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:14:15.175472 ns_asphalt9-0.0.1/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.1/README.md
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:14:15.173762 ns_asphalt9-0.0.1/ns_asphalt9/
--rw-r--r--   0 neo.sun    (502) staff       (20)     5062 2023-06-29 06:51:56.000000 ns_asphalt9-0.0.1/ns_asphalt9/main.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:14:15.175055 ns_asphalt9-0.0.1/ns_asphalt9.egg-info/
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:14:15.000000 ns_asphalt9-0.0.1/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)      320 2023-06-30 07:14:15.000000 ns_asphalt9-0.0.1/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:14:15.000000 ns_asphalt9-0.0.1/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       47 2023-06-30 07:14:15.000000 ns_asphalt9-0.0.1/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.1/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-06-30 07:14:15.000000 ns_asphalt9-0.0.1/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-06-30 07:14:15.000000 ns_asphalt9-0.0.1/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)     1292 2023-06-30 07:14:15.175791 ns_asphalt9-0.0.1/setup.cfg
--rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.1/setup.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:14:15.175169 ns_asphalt9-0.0.1/tests/
--rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.1/tests/test_ocr.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:19:51.689252 ns_asphalt9-0.0.2/
+-rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.2/LICENSE
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:19:51.689398 ns_asphalt9-0.0.2/PKG-INFO
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.2/README.md
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:19:51.687257 ns_asphalt9-0.0.2/ns_asphalt9/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     5062 2023-06-29 06:51:56.000000 ns_asphalt9-0.0.2/ns_asphalt9/main.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:19:51.688745 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 neo.sun    (502) staff       (20)      320 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)       54 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1299 2023-06-30 07:19:51.689788 ns_asphalt9-0.0.2/setup.cfg
+-rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.2/setup.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:19:51.688883 ns_asphalt9-0.0.2/tests/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.2/tests/test_ocr.py
```

### Comparing `ns_asphalt9-0.0.1/LICENSE` & `ns_asphalt9-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.1/PKG-INFO` & `ns_asphalt9-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.0.1/README.md` & `ns_asphalt9-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.1/ns_asphalt9/main.py` & `ns_asphalt9-0.0.2/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.1/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.0.2/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.0.1/setup.cfg` & `ns_asphalt9-0.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.0.1
+version = 0.0.2
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
@@ -28,15 +28,15 @@
 packages = ns_asphalt9
 include_package_data = true
 python_requires = >= 3.6
 zip_safe = False
 
 [options.entry_points]
 console_scripts = 
-	nxbt = ns_asphalt9.main:main
+	ns_asphalt9 = ns_asphalt9.main:main
 
 [aliases]
 test = pytest
 
 [tool:pytest]
 testpaths = tests
 filterwarnings =
```

### Comparing `ns_asphalt9-0.0.1/tests/test_ocr.py` & `ns_asphalt9-0.0.2/tests/test_ocr.py`

 * *Files identical despite different names*

