# Comparing `tmp/plemmy-0.2.4.tar.gz` & `tmp/plemmy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.2.4.tar", last modified: Sat Jun 24 16:58:04 2023, max compression
+gzip compressed data, was "plemmy-0.2.5.tar", last modified: Fri Jun 30 20:44:48 2023, max compression
```

## Comparing `plemmy-0.2.4.tar` & `plemmy-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-24 16:58:04.570548 plemmy-0.2.4/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.4/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-24 16:58:04.570384 plemmy-0.2.4/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.4/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-24 16:58:04.569120 plemmy-0.2.4/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.4/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    70949 2023-06-24 16:56:44.000000 plemmy-0.2.4/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2803 2023-06-23 18:44:09.000000 plemmy-0.2.4/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-24 16:57:12.000000 plemmy-0.2.4/plemmy/version.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-24 16:58:04.570175 plemmy-0.2.4/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-24 16:58:04.570595 plemmy-0.2.4/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.4/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-30 20:44:48.100899 plemmy-0.2.5/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.5/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-30 20:44:48.100728 plemmy-0.2.5/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.5/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-30 20:44:48.099532 plemmy-0.2.5/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.5/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    70949 2023-06-24 16:56:44.000000 plemmy-0.2.5/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-06-30 20:43:38.000000 plemmy-0.2.5/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-30 20:43:24.000000 plemmy-0.2.5/plemmy/version.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-30 20:44:48.100495 plemmy-0.2.5/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-30 20:44:48.000000 plemmy-0.2.5/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-30 20:44:48.100948 plemmy-0.2.5/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.5/setup.py
```

### Comparing `plemmy-0.2.4/LICENSE` & `plemmy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.4/PKG-INFO` & `plemmy-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.2.4/README.md` & `plemmy-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.4/plemmy/lemmyhttp.py` & `plemmy-0.2.5/plemmy/lemmyhttp.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.4/plemmy/utils.py` & `plemmy-0.2.5/plemmy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     Returns:
         requests.Response: server response for POST operation
     """
 
     logger = logging.getLogger(__name__)
     try:
-        re = requests.post(url, headers=headers, json=json)
+        re = requests.post(url, headers=headers, json=json, timeout=30)
         logger.debug(f"Code: {re.status_code}")
     except requests.exceptions.RequestException as ex:
         logger.error(f"POST error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
 
@@ -35,15 +35,15 @@
 
     Returns:
         requests.Response: server response for PUT operation
     """
 
     logger = logging.getLogger(__name__)
     try:
-        re = requests.put(url, headers=headers, json=json)
+        re = requests.put(url, headers=headers, json=json, timeout=30)
         logger.debug(f"Code: {re.status_code}")
     except requests.exceptions.RequestException as ex:
         logger.error(f"PUT error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
 
@@ -60,15 +60,16 @@
 
     Returns:
         requests.Response: server response for GET operation
     """
 
     logger = logging.getLogger(__name__)
     try:
-        re = requests.get(url, headers=headers, json=json, params=params)
+        re = requests.get(url, headers=headers, json=json, params=params,
+                          timeout=30)
         logger.debug(f"Code: {re.status_code}")
     except requests.exceptions.RequestException as ex:
         logger.error(f"GET error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
```

### Comparing `plemmy-0.2.4/plemmy.egg-info/PKG-INFO` & `plemmy-0.2.5/plemmy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.2.4/setup.py` & `plemmy-0.2.5/setup.py`

 * *Files identical despite different names*

