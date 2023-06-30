# Comparing `tmp/tychos-0.0.1.tar.gz` & `tmp/tychos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.0.1.tar", last modified: Thu Jun 29 20:39:33 2023, max compression
+gzip compressed data, was "tychos-0.0.2.tar", last modified: Fri Jun 30 20:18:24 2023, max compression
```

## Comparing `tychos-0.0.1.tar` & `tychos-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-29 20:39:33.321531 tychos-0.0.1/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.1/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)       72 2023-06-29 20:39:33.321416 tychos-0.0.1/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)       19 2023-06-27 16:59:52.000000 tychos-0.0.1/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-06-29 20:39:33.321579 tychos-0.0.1/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)       58 2023-06-29 20:39:02.000000 tychos-0.0.1/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-29 20:39:33.320662 tychos-0.0.1/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)       47 2023-06-29 19:17:21.000000 tychos-0.0.1/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-26 15:20:14.000000 tychos-0.0.1/tychos/api.py
--rw-r--r--   0 abe732     (501) staff       (20)      748 2023-06-29 20:37:31.000000 tychos-0.0.1/tychos/vector_data_store.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-29 20:39:33.321274 tychos-0.0.1/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)       72 2023-06-29 20:39:33.000000 tychos-0.0.1/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      207 2023-06-29 20:39:33.000000 tychos-0.0.1/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-06-29 20:39:33.000000 tychos-0.0.1/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-06-29 20:39:33.000000 tychos-0.0.1/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-30 20:18:24.844036 tychos-0.0.2/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.2/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)       95 2023-06-30 20:18:24.843918 tychos-0.0.2/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)       19 2023-06-27 16:59:52.000000 tychos-0.0.2/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-06-30 20:18:24.844067 tychos-0.0.2/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)      138 2023-06-30 20:16:58.000000 tychos-0.0.2/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-30 20:18:24.842991 tychos-0.0.2/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)       74 2023-06-30 15:48:02.000000 tychos-0.0.2/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-26 15:20:14.000000 tychos-0.0.2/tychos/api.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-30 20:18:24.843786 tychos-0.0.2/tychos/helpers/
+-rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.2/tychos/helpers/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1296 2023-06-30 20:02:27.000000 tychos-0.0.2/tychos/vector.py
+-rw-r--r--   0 abe732     (501) staff       (20)      996 2023-06-30 20:02:19.000000 tychos-0.0.2/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-30 20:18:24.843678 tychos-0.0.2/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)       95 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      280 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        9 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/requires.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.0.1/LICENSE` & `tychos-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tychos-0.0.1/tychos/vector_data_store.py` & `tychos-0.0.2/tychos/vector_data_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import requests
+from .vector import Vector
 
 class VectorDataStore:
     def __init__(self, api_key):
         self.api_key = api_key
         self.base_url = 'https://www.tychos.ai/api/'
         # self.base_url = 'http://localhost:3000/api/'
+        self.vector = Vector(api_key)
 
-    def query(self, index_name, query_string, limit):
+    def query(self, name, query_string, limit):
+        # vectorize query string
+        query_vector = self.vector.create(
+            type="text_embedding",
+            input_text=query_string,
+            model="text-embedding-ada-002"
+        )
 
         # send query request to vector data store
         url = f'{self.base_url}/query-vector-store'
         headers = {'api_key': self.api_key}
         payload = {
-                    'index_name': index_name,
-                    'query_string': query_string,
+                    'name': name,
+                    'query_vector': query_vector,
                     'top': limit,
                 }
         response = requests.post(url=url, headers=headers, json=payload)
 
         # error handling
         response.raise_for_status()
```

