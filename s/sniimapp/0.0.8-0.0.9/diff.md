# Comparing `tmp/sniimapp-0.0.8.tar.gz` & `tmp/sniimapp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp-0.0.8.tar", last modified: Fri Jun 30 07:13:54 2023, max compression
+gzip compressed data, was "sniimapp-0.0.9.tar", last modified: Fri Jun 30 07:24:38 2023, max compression
```

## Comparing `sniimapp-0.0.8.tar` & `sniimapp-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 07:13:54.522176 sniimapp-0.0.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.8/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1369 2023-06-30 07:13:54.522176 sniimapp-0.0.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2023-06-29 22:13:57.000000 sniimapp-0.0.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-06-30 07:13:37.000000 sniimapp-0.0.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-30 07:13:54.522176 sniimapp-0.0.8/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 07:13:54.522176 sniimapp-0.0.8/sniimapp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1369 2023-06-30 07:13:54.000000 sniimapp-0.0.8/sniimapp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-30 07:13:54.000000 sniimapp-0.0.8/sniimapp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-30 07:13:54.000000 sniimapp-0.0.8/sniimapp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-30 07:13:54.000000 sniimapp-0.0.8/sniimapp.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-06-30 07:12:51.000000 sniimapp-0.0.8/sniimapp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 07:24:38.347107 sniimapp-0.0.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.9/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1369 2023-06-30 07:24:38.347107 sniimapp-0.0.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2023-06-29 22:13:57.000000 sniimapp-0.0.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-06-30 07:24:18.000000 sniimapp-0.0.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-30 07:24:38.347107 sniimapp-0.0.9/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 07:24:38.347107 sniimapp-0.0.9/sniimapp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1369 2023-06-30 07:24:38.000000 sniimapp-0.0.9/sniimapp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-30 07:24:38.000000 sniimapp-0.0.9/sniimapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-30 07:24:38.000000 sniimapp-0.0.9/sniimapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-30 07:24:38.000000 sniimapp-0.0.9/sniimapp.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1969 2023-06-30 07:23:26.000000 sniimapp-0.0.9/sniimapp.py
```

### Comparing `sniimapp-0.0.8/LICENSE` & `sniimapp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.8/PKG-INFO` & `sniimapp-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.8/README.md` & `sniimapp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.8/pyproject.toml` & `sniimapp-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sniimapp"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Rodolfo Lopez", email="1803672F@umich.mx" },
 ]
 description = "Libreria para extraccion de precios SNIIM"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sniimapp-0.0.8/sniimapp.egg-info/PKG-INFO` & `sniimapp-0.0.9/sniimapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.8/sniimapp.py` & `sniimapp-0.0.9/sniimapp.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class SNIIM():
 
     def __init__(self, product, start_date, end_date):
         self.product = product
         self.start_date = start_date
         self.end_date   = end_date
         self.MONGO_HOST = '18.215.228.120' #os.environ.get('MONGO_HOST')
-        self.MONGO_PORT = '27017'          #os.environ.get('MONGO_PORT')
+        self.MONGO_PORT = 27017           #os.environ.get('MONGO_PORT')
         self.MONGO_USER = 'fcca_read_1'    #os.environ.get('MONGO_USER')
         self.MONGO_PASSW ='Fcc4_R3_d_1'    #os.environ.get('MONGO_PASSWORD')
         self.client = MongoClient(self._connection_string)
         self.MONGO_DB = 'sniim'            #os.environ.get('MONGO_DATABASE')
         if product == 'fyh':
             self.db_collection = 'sniim_fyh'
         if product == 'granos':
```

