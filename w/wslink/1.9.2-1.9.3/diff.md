# Comparing `tmp/wslink-1.9.2.tar.gz` & `tmp/wslink-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../dist/wslink-1.9.2.tar", last modified: Thu Dec  8 20:48:05 2022, max compression
+gzip compressed data, was "../dist/wslink-1.9.3.tar", last modified: Mon Dec 19 17:53:11 2022, max compression
```

## Comparing `wslink-1.9.2.tar` & `wslink-1.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-08 20:48:05.000000 wslink-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-12-08 20:47:31.000000 wslink-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2463 2022-12-08 20:48:05.000000 wslink-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1448 2022-12-08 20:47:31.000000 wslink-1.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       66 2022-12-08 20:48:05.000000 wslink-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1587 2022-12-08 20:47:31.000000 wslink-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-08 20:48:05.000000 wslink-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink/
--rw-r--r--   0 runner    (1001) docker     (116)     1483 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2708 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink/backends/
--rw-r--r--   0 runner    (1001) docker     (116)      485 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink/backends/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (116)    23509 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/backends/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8427 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/backends/aiohttp/launcher.py
--rw-r--r--   0 runner    (1001) docker     (116)    13338 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/backends/aiohttp/relay.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    21137 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/launcher.py
--rw-r--r--   0 runner    (1001) docker     (116)     2573 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/publish.py
--rw-r--r--   0 runner    (1001) docker     (116)       86 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/relay.py
--rw-r--r--   0 runner    (1001) docker     (116)     9394 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/server.py
--rw-r--r--   0 runner    (1001) docker     (116)     2290 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/ssl_context.py
--rw-r--r--   0 runner    (1001) docker     (116)      384 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/uri.py
--rw-r--r--   0 runner    (1001) docker     (116)     4574 2022-12-08 20:47:31.000000 wslink-1.9.2/src/wslink/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2463 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      555 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-12-08 20:48:05.000000 wslink-1.9.2/src/wslink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2022-12-19 17:52:31.000000 wslink-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2463 2022-12-19 17:53:11.000000 wslink-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1448 2022-12-19 17:52:31.000000 wslink-1.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       66 2022-12-19 17:53:11.000000 wslink-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1587 2022-12-19 17:52:31.000000 wslink-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink/
+-rw-r--r--   0 runner    (1001) docker     (116)     1483 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     2708 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink/backends/
+-rw-r--r--   0 runner    (1001) docker     (116)      485 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink/backends/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (116)    23509 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/backends/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8445 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/backends/aiohttp/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13338 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/backends/aiohttp/relay.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    21137 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2573 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/publish.py
+-rw-r--r--   0 runner    (1001) docker     (116)       86 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/relay.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9394 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/server.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2290 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/ssl_context.py
+-rw-r--r--   0 runner    (1001) docker     (116)      384 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/uri.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4574 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2463 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      555 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/top_level.txt
```

### Comparing `wslink-1.9.2/PKG-INFO` & `wslink-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 1.9.2
+Version: 1.9.3
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wslink-1.9.2/README.rst` & `wslink-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/setup.py` & `wslink-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/LICENSE` & `wslink-1.9.3/src/wslink/LICENSE`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/__init__.py` & `wslink-1.9.3/src/wslink/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/backends/aiohttp/__init__.py` & `wslink-1.9.3/src/wslink/backends/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/backends/aiohttp/launcher.py` & `wslink-1.9.3/src/wslink/backends/aiohttp/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,16 @@
 
     if not endpoint.startswith("/"):
         endpoint = "/{0}/".format(endpoint)
 
     web_app.add_routes(
         [
             aiohttp_web.post(endpoint, launcher_resource.handle_post),
-            aiohttp_web.get(endpoint, launcher_resource.handle_get),
-            aiohttp_web.delete(endpoint, launcher_resource.handle_delete),
+            aiohttp_web.get(endpoint + "{id}", launcher_resource.handle_get),
+            aiohttp_web.delete(endpoint + "{id}", launcher_resource.handle_delete),
         ]
     )
 
     if len(content) > 0:
         web_app.router.add_route("GET", "/", _root_handler)
         web_app.add_routes([aiohttp_web.static("/", content)])
```

### Comparing `wslink-1.9.2/src/wslink/backends/aiohttp/relay.py` & `wslink-1.9.3/src/wslink/backends/aiohttp/relay.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/launcher.py` & `wslink-1.9.3/src/wslink/launcher.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/publish.py` & `wslink-1.9.3/src/wslink/publish.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/server.py` & `wslink-1.9.3/src/wslink/server.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/ssl_context.py` & `wslink-1.9.3/src/wslink/ssl_context.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink/websocket.py` & `wslink-1.9.3/src/wslink/websocket.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.2/src/wslink.egg-info/PKG-INFO` & `wslink-1.9.3/src/wslink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 1.9.2
+Version: 1.9.3
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wslink-1.9.2/src/wslink.egg-info/SOURCES.txt` & `wslink-1.9.3/src/wslink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

