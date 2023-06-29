# Comparing `tmp/hypha-0.15.7.tar.gz` & `tmp/hypha-0.15.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypha-0.15.7.tar", last modified: Tue Jul 19 03:43:57 2022, max compression
+gzip compressed data, was "hypha-0.15.8.tar", last modified: Tue Jul 19 05:11:34 2022, max compression
```

## Comparing `hypha-0.15.7.tar` & `hypha-0.15.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.462769 hypha-0.15.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-07-19 03:43:45.000000 hypha-0.15.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-07-19 03:43:45.000000 hypha-0.15.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-07-19 03:43:57.462769 hypha-0.15.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-07-19 03:43:45.000000 hypha-0.15.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.454769 hypha-0.15.7/hypha/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-19 03:43:55.000000 hypha-0.15.7/hypha/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35092 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6847 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.454769 hypha-0.15.7/hypha/built-in/
--rw-r--r--   0 runner    (1001) docker     (121)     7303 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/built-in/account-manager.html
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-19 03:43:55.000000 hypha-0.15.7/hypha/built-in/echo-service.html
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-07-19 03:43:55.000000 hypha-0.15.7/hypha/built-in/imjoy-plugin-parser.html
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-07-19 03:43:55.000000 hypha-0.15.7/hypha/built-in/playground.html
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-07-19 03:43:55.000000 hypha-0.15.7/hypha/built-in/test.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.458769 hypha-0.15.7/hypha/core/
--rw-r--r--   0 runner    (1001) docker     (121)     8310 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11068 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    16497 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/core/store.py
--rw-r--r--   0 runner    (1001) docker     (121)    41862 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/core/workspace.py
--rw-r--r--   0 runner    (1001) docker     (121)     8653 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/http.py
--rw-r--r--   0 runner    (1001) docker     (121)    14362 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/minio.py
--rw-r--r--   0 runner    (1001) docker     (121)     5068 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.458769 hypha-0.15.7/hypha/runner/
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6380 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/runner/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)    27690 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     9425 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.458769 hypha-0.15.7/hypha/static_files/
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/static_files/lite.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.458769 hypha-0.15.7/hypha/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-07-19 03:43:55.000000 hypha-0.15.7/hypha/templates/web-python-plugin.html
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-07-19 03:43:55.000000 hypha-0.15.7/hypha/templates/web-worker-plugin.html
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-07-19 03:43:55.000000 hypha-0.15.7/hypha/templates/window-plugin.html
--rw-r--r--   0 runner    (1001) docker     (121)     4278 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/triton.py
--rw-r--r--   0 runner    (1001) docker     (121)    13624 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8696 2022-07-19 03:43:45.000000 hypha-0.15.7/hypha/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.454769 hypha-0.15.7/hypha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-07-19 03:43:57.000000 hypha-0.15.7/hypha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-07-19 03:43:57.000000 hypha-0.15.7/hypha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 03:43:57.000000 hypha-0.15.7/hypha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-19 03:43:57.000000 hypha-0.15.7/hypha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 03:43:57.000000 hypha-0.15.7/hypha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-07-19 03:43:57.000000 hypha-0.15.7/hypha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-19 03:43:57.000000 hypha-0.15.7/hypha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-07-19 03:43:57.462769 hypha-0.15.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-19 03:43:55.000000 hypha-0.15.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 03:43:57.462769 hypha-0.15.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6017 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/example_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_asgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     6459 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (121)     3755 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_minio_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8243 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     6383 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (121)    12301 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     8112 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_server_apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-07-19 03:43:45.000000 hypha-0.15.7/tests/test_triton.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.074471 hypha-0.15.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-07-19 05:11:24.000000 hypha-0.15.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-07-19 05:11:24.000000 hypha-0.15.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-07-19 05:11:34.074471 hypha-0.15.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-07-19 05:11:24.000000 hypha-0.15.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.070471 hypha-0.15.8/hypha/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-19 05:11:32.000000 hypha-0.15.8/hypha/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35092 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6847 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.074471 hypha-0.15.8/hypha/built-in/
+-rw-r--r--   0 runner    (1001) docker     (121)     7303 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/built-in/account-manager.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-19 05:11:32.000000 hypha-0.15.8/hypha/built-in/echo-service.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-07-19 05:11:32.000000 hypha-0.15.8/hypha/built-in/imjoy-plugin-parser.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-07-19 05:11:32.000000 hypha-0.15.8/hypha/built-in/playground.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-07-19 05:11:32.000000 hypha-0.15.8/hypha/built-in/test.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.074471 hypha-0.15.8/hypha/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     8310 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11068 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16497 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/core/store.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41862 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/core/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8653 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14362 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/minio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5068 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.074471 hypha-0.15.8/hypha/runner/
+-rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6380 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/runner/browser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27690 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9425 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.074471 hypha-0.15.8/hypha/static_files/
+-rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/static_files/lite.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.074471 hypha-0.15.8/hypha/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-07-19 05:11:32.000000 hypha-0.15.8/hypha/templates/web-python-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-07-19 05:11:32.000000 hypha-0.15.8/hypha/templates/web-worker-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-07-19 05:11:32.000000 hypha-0.15.8/hypha/templates/window-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4278 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/triton.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13624 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8696 2022-07-19 05:11:24.000000 hypha-0.15.8/hypha/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.074471 hypha-0.15.8/hypha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-07-19 05:11:34.000000 hypha-0.15.8/hypha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-07-19 05:11:34.000000 hypha-0.15.8/hypha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 05:11:34.000000 hypha-0.15.8/hypha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-19 05:11:34.000000 hypha-0.15.8/hypha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 05:11:34.000000 hypha-0.15.8/hypha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-07-19 05:11:34.000000 hypha-0.15.8/hypha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-19 05:11:34.000000 hypha-0.15.8/hypha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-07-19 05:11:34.074471 hypha-0.15.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-19 05:11:32.000000 hypha-0.15.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 05:11:34.074471 hypha-0.15.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6017 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/example_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6459 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3755 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_minio_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8243 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6383 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12301 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8112 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_server_apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-07-19 05:11:24.000000 hypha-0.15.8/tests/test_triton.py
```

### Comparing `hypha-0.15.7/LICENSE` & `hypha-0.15.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/PKG-INFO` & `hypha-0.15.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypha
-Version: 0.15.7
+Version: 0.15.8
 Summary: A serverless application framework for large-scale data management and AI model serving.
 Home-page: http://github.com/imjoy-team/hypha
 Author: ImJoy Team
 Author-email: imjoy.team@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `hypha-0.15.7/README.md` & `hypha-0.15.8/README.md`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/apps.py` & `hypha-0.15.8/hypha/apps.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/asgi.py` & `hypha-0.15.8/hypha/asgi.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/built-in/account-manager.html` & `hypha-0.15.8/hypha/built-in/account-manager.html`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/built-in/echo-service.html` & `hypha-0.15.8/hypha/built-in/echo-service.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
 <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>ImJoy Plugin Template</title>
    <meta name="description" content="Template for ImJoy plugin">
    <meta name="author" content="ImJoy-Team">
-   <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.14/dist/hypha-rpc-websocket.min.js"></script>
+   <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.15/dist/hypha-rpc-websocket.min.js"></script>
 </head>
 
 <body>
     <script>
         const config = Object.fromEntries(new URLSearchParams(window.location.search))
         if(!config.server_url) config.server_url = window.location.origin;
         hyphaWebsocketClient.connectToServer(config).then(async (api)=>{
```

### Comparing `hypha-0.15.7/hypha/built-in/imjoy-plugin-parser.html` & `hypha-0.15.8/hypha/built-in/imjoy-plugin-parser.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
 <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>ImJoy Plugin Template</title>
    <meta name="description" content="Template for ImJoy plugin">
    <meta name="author" content="ImJoy-Team">
-   <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.14/dist/hypha-rpc-websocket.min.js"></script>
+   <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.15/dist/hypha-rpc-websocket.min.js"></script>
    <scrpt src="https://cdn.jsdelivr.net/npm/imjoy-core@0.13.82/src/pluginParser.js"></scrpt>
 </head>
 
 <body>
     <script>
         function randId() {
             return (
```

### Comparing `hypha-0.15.7/hypha/built-in/playground.html` & `hypha-0.15.8/hypha/built-in/playground.html`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>ImJoy Playground</title>
    <meta name="description" content="A playground for developing ImJoy plugins">
    <meta name="author" content="ImJoy-Team">
    <link rel="stylesheet" data-name="vs/editor/editor.main" href="https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.20.0/min/vs/editor/editor.main.min.css">
-   <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.14/dist/hypha-rpc-websocket.min.js"></script>
+   <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.15/dist/hypha-rpc-websocket.min.js"></script>
    <scrpt src="https://cdn.jsdelivr.net/npm/imjoy-core@0.13.82/src/pluginParser.js"></scrpt>
 <script>
 window.default_plugin = `
 <docs lang="markdown">
 [TODO: write documentation for this plugin.]
 </docs>
```

### Comparing `hypha-0.15.7/hypha/built-in/test.html` & `hypha-0.15.8/hypha/built-in/test.html`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <title>ImJoy Plugin Template</title>
   <meta name="description" content="Template for ImJoy plugin">
   <meta name="author" content="ImJoy-Team">
-  <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.14/dist/hypha-rpc-websocket.min.js"></script>
+  <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.15/dist/hypha-rpc-websocket.min.js"></script>
 </head>
 
 <body>
 <script>
 window.onload = function() {
   const cfg = {
   "local_base_url": "http://127.0.0.1:38283",
```

### Comparing `hypha-0.15.7/hypha/core/__init__.py` & `hypha-0.15.8/hypha/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/core/auth.py` & `hypha-0.15.8/hypha/core/auth.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/core/store.py` & `hypha-0.15.8/hypha/core/store.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/core/workspace.py` & `hypha-0.15.8/hypha/core/workspace.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/http.py` & `hypha-0.15.8/hypha/http.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/minio.py` & `hypha-0.15.8/hypha/minio.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/plugin_parser.py` & `hypha-0.15.8/hypha/plugin_parser.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/rdf.py` & `hypha-0.15.8/hypha/rdf.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/runner/__init__.py` & `hypha-0.15.8/hypha/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/runner/__main__.py` & `hypha-0.15.8/hypha/runner/__main__.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/runner/browser.py` & `hypha-0.15.8/hypha/runner/browser.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/s3.py` & `hypha-0.15.8/hypha/s3.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/server.py` & `hypha-0.15.8/hypha/server.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/static_files/lite.html` & `hypha-0.15.8/hypha/static_files/lite.html`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/templates/web-python-plugin.html` & `hypha-0.15.8/hypha/templates/web-python-plugin.html`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 m.MemoryBIO = None
 m.SSLContext = None
 sys.modules["ssl"] = m
 del m
 
 async def run():
     try:
-        await micropip.install(["imjoy-rpc==0.5.14", {% for req in requirements %}"{{req}}", {% endfor %}])
+        await micropip.install(["imjoy-rpc==0.5.15", {% for req in requirements %}"{{req}}", {% endfor %}])
         js.__resolve()
     except Exception as e:
         js.__reject(traceback.format_exc())
 
 asyncio.get_event_loop().run_until_complete(run())
 `
```

### Comparing `hypha-0.15.7/hypha/templates/web-worker-plugin.html` & `hypha-0.15.8/hypha/templates/web-worker-plugin.html`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 <body>
 <script id="worker" type="javascript/worker">
 window = self;
 
 self.onmessage = function(e) {
 const config = e.data
 
-importScripts("https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.14/dist/hypha-rpc-websocket.min.js")
+importScripts("https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.15/dist/hypha-rpc-websocket.min.js")
 
 hyphaWebsocketClient.connectToServer(config).then(async (api)=>{
 await hyphaWebsocketClient.loadRequirements([{% for req in requirements %}"{{req}}", {% endfor %}])
 {{ script | safe }}
 }).catch(console.error)
 }
 </script>
```

### Comparing `hypha-0.15.7/hypha/templates/window-plugin.html` & `hypha-0.15.8/hypha/templates/window-plugin.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <title>ImJoy Plugin (window)</title>
   <meta name="description" content="Template for ImJoy plugin">
   <meta name="author" content="ImJoy-Team">
-  <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.14/dist/hypha-rpc-websocket.min.js"></script>
+  <script src="https://cdn.jsdelivr.net/npm/imjoy-rpc@0.5.15/dist/hypha-rpc-websocket.min.js"></script>
 </head>
 
 <body>
 <script>
 window.onload = function() {
   const cfg = {{ config | tojson(indent=2) }}
   const config = Object.assign(cfg, Object.fromEntries(new URLSearchParams(window.location.search)));
```

### Comparing `hypha-0.15.7/hypha/triton.py` & `hypha-0.15.8/hypha/triton.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/utils.py` & `hypha-0.15.8/hypha/utils.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha/websocket.py` & `hypha-0.15.8/hypha/websocket.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/hypha.egg-info/PKG-INFO` & `hypha-0.15.8/hypha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypha
-Version: 0.15.7
+Version: 0.15.8
 Summary: A serverless application framework for large-scale data management and AI model serving.
 Home-page: http://github.com/imjoy-team/hypha
 Author: ImJoy Team
 Author-email: imjoy.team@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `hypha-0.15.7/hypha.egg-info/SOURCES.txt` & `hypha-0.15.8/hypha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/setup.py` & `hypha-0.15.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     " data management and AI model serving."
 )
 
 REQUIREMENTS = [
     "aiobotocore>=2.1.0",
     "aiofiles",
     "fastapi>=0.70.0",
-    "imjoy-rpc==0.5.14",
+    "imjoy-rpc==0.5.15",
     "msgpack>=1.0.2",
     "numpy",
     "pydantic[email]>=1.8.2",
     "typing-extensions>=3.7.4.3",  # required by pydantic
     "jinja2>=3",
     "lxml",
     "python-dotenv>=0.19.0",
```

### Comparing `hypha-0.15.7/tests/__init__.py` & `hypha-0.15.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/conftest.py` & `hypha-0.15.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/example_plugin.py` & `hypha-0.15.8/tests/example_plugin.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_asgi.py` & `hypha-0.15.8/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_http.py` & `hypha-0.15.8/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_minio_client.py` & `hypha-0.15.8/tests/test_minio_client.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_plugin_parser.py` & `hypha-0.15.8/tests/test_plugin_parser.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_rdf.py` & `hypha-0.15.8/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_redis.py` & `hypha-0.15.8/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_s3.py` & `hypha-0.15.8/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_server.py` & `hypha-0.15.8/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_server_apps.py` & `hypha-0.15.8/tests/test_server_apps.py`

 * *Files identical despite different names*

### Comparing `hypha-0.15.7/tests/test_triton.py` & `hypha-0.15.8/tests/test_triton.py`

 * *Files identical despite different names*

