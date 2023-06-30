# Comparing `tmp/honeydew-0.1.8.tar.gz` & `tmp/honeydew-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeydew-0.1.8.tar", last modified: Tue Sep 20 02:59:10 2022, max compression
+gzip compressed data, was "honeydew-0.1.9.tar", last modified: Tue Sep 20 03:57:28 2022, max compression
```

## Comparing `honeydew-0.1.8.tar` & `honeydew-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2022-09-20 02:59:10.986608 honeydew-0.1.8/
--rw-r--r--   0 docker    (1000) docker    (1000)     1081 2022-09-20 02:59:10.986608 honeydew-0.1.8/PKG-INFO
--rwxrwxrwx   0 docker    (1000) docker    (1000)      204 2022-09-15 03:59:50.000000 honeydew-0.1.8/README.md
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2022-09-20 02:59:10.985608 honeydew-0.1.8/honeydew/
--rwxrwxrwx   0 docker    (1000) docker    (1000)      150 2022-09-15 05:04:36.000000 honeydew-0.1.8/honeydew/__init__.py
--rwxrwxrwx   0 docker    (1000) docker    (1000)     7411 2022-09-20 02:47:15.000000 honeydew-0.1.8/honeydew/gcp.py
--rwxrwxrwx   0 docker    (1000) docker    (1000)     4311 2022-09-15 05:44:13.000000 honeydew-0.1.8/honeydew/mysql.py
--rwxrwxrwx   0 docker    (1000) docker    (1000)     2102 2022-09-15 05:43:34.000000 honeydew-0.1.8/honeydew/ssh.py
--rwxrwxrwx   0 docker    (1000) docker    (1000)      806 2022-09-15 05:47:50.000000 honeydew-0.1.8/honeydew/utils.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2022-09-20 02:59:10.985608 honeydew-0.1.8/honeydew.egg-info/
--rw-r--r--   0 docker    (1000) docker    (1000)     1081 2022-09-20 02:59:10.000000 honeydew-0.1.8/honeydew.egg-info/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)      266 2022-09-20 02:59:10.000000 honeydew-0.1.8/honeydew.egg-info/SOURCES.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        1 2022-09-20 02:59:10.000000 honeydew-0.1.8/honeydew.egg-info/dependency_links.txt
--rw-r--r--   0 docker    (1000) docker    (1000)      163 2022-09-20 02:59:10.000000 honeydew-0.1.8/honeydew.egg-info/requires.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        9 2022-09-20 02:59:10.000000 honeydew-0.1.8/honeydew.egg-info/top_level.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       38 2022-09-20 02:59:10.986608 honeydew-0.1.8/setup.cfg
--rwxrwxrwx   0 docker    (1000) docker    (1000)     1587 2022-09-20 02:59:08.000000 honeydew-0.1.8/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2022-09-20 03:57:28.616497 honeydew-0.1.9/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1081 2022-09-20 03:57:28.616497 honeydew-0.1.9/PKG-INFO
+-rwxrwxrwx   0 docker    (1000) docker    (1000)      204 2022-09-15 03:59:50.000000 honeydew-0.1.9/README.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2022-09-20 03:57:28.616497 honeydew-0.1.9/honeydew/
+-rwxrwxrwx   0 docker    (1000) docker    (1000)      150 2022-09-15 05:04:36.000000 honeydew-0.1.9/honeydew/__init__.py
+-rwxrwxrwx   0 docker    (1000) docker    (1000)     7393 2022-09-20 03:56:41.000000 honeydew-0.1.9/honeydew/gcp.py
+-rwxrwxrwx   0 docker    (1000) docker    (1000)     4311 2022-09-15 05:44:13.000000 honeydew-0.1.9/honeydew/mysql.py
+-rwxrwxrwx   0 docker    (1000) docker    (1000)     2102 2022-09-15 05:43:34.000000 honeydew-0.1.9/honeydew/ssh.py
+-rwxrwxrwx   0 docker    (1000) docker    (1000)      806 2022-09-15 05:47:50.000000 honeydew-0.1.9/honeydew/utils.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2022-09-20 03:57:28.616497 honeydew-0.1.9/honeydew.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1081 2022-09-20 03:57:28.000000 honeydew-0.1.9/honeydew.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)      266 2022-09-20 03:57:28.000000 honeydew-0.1.9/honeydew.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2022-09-20 03:57:28.000000 honeydew-0.1.9/honeydew.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)      163 2022-09-20 03:57:28.000000 honeydew-0.1.9/honeydew.egg-info/requires.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        9 2022-09-20 03:57:28.000000 honeydew-0.1.9/honeydew.egg-info/top_level.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       38 2022-09-20 03:57:28.616497 honeydew-0.1.9/setup.cfg
+-rwxrwxrwx   0 docker    (1000) docker    (1000)     1587 2022-09-20 03:56:49.000000 honeydew-0.1.9/setup.py
```

### Comparing `honeydew-0.1.8/PKG-INFO` & `honeydew-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeydew
-Version: 0.1.8
+Version: 0.1.9
 Summary: Collection of connectors for ETL
 Home-page: https://honeydew-lib.github.io/
 Author: Poltak Jefferson
 Author-email: poltak.jefferson@gmail.com
 License: MIT
 Project-URL: Repository, https://github.com/honeydew-lib/honeydew
 Project-URL: Documentation, https://honeydew-lib.github.io/
```

### Comparing `honeydew-0.1.8/honeydew/gcp.py` & `honeydew-0.1.9/honeydew/gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 from google.cloud import bigquery
 from google.cloud import storage
 import pandas as pd
-import pandas_gbq
 
 class GcpConnector:
     """
     Instantiate a GCP connector.
     Args:
         credential_file (str): Credential json file
         proxy (str): Proxy address
```

### Comparing `honeydew-0.1.8/honeydew/mysql.py` & `honeydew-0.1.9/honeydew/mysql.py`

 * *Files identical despite different names*

### Comparing `honeydew-0.1.8/honeydew/ssh.py` & `honeydew-0.1.9/honeydew/ssh.py`

 * *Files identical despite different names*

### Comparing `honeydew-0.1.8/honeydew/utils.py` & `honeydew-0.1.9/honeydew/utils.py`

 * *Files identical despite different names*

### Comparing `honeydew-0.1.8/honeydew.egg-info/PKG-INFO` & `honeydew-0.1.9/honeydew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeydew
-Version: 0.1.8
+Version: 0.1.9
 Summary: Collection of connectors for ETL
 Home-page: https://honeydew-lib.github.io/
 Author: Poltak Jefferson
 Author-email: poltak.jefferson@gmail.com
 License: MIT
 Project-URL: Repository, https://github.com/honeydew-lib/honeydew
 Project-URL: Documentation, https://honeydew-lib.github.io/
```

### Comparing `honeydew-0.1.8/setup.py` & `honeydew-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="honeydew",
-    version="0.1.8",
+    version="0.1.9",
     description="Collection of connectors for ETL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://honeydew-lib.github.io/",
     project_urls = {
         'Repository': 'https://github.com/honeydew-lib/honeydew',
         'Documentation': 'https://honeydew-lib.github.io/'
```

