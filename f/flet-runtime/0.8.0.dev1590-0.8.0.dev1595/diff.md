# Comparing `tmp/flet_runtime-0.8.0.dev1590.tar.gz` & `tmp/flet_runtime-0.8.0.dev1595.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_runtime-0.8.0.dev1590.tar", max compression
+gzip compressed data, was "flet_runtime-0.8.0.dev1595.tar", max compression
```

## Comparing `flet_runtime-0.8.0.dev1590.tar` & `flet_runtime-0.8.0.dev1595.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      204 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/README.md
--rw-r--r--   0        0        0      747 2023-06-27 03:22:07.455315 flet_runtime-0.8.0.dev1590/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/__init__.py
--rw-r--r--   0        0        0    23672 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/app.py
--rw-r--r--   0        0        0     6309 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/async_local_socket_connection.py
--rw-r--r--   0        0        0      252 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/__init__.py
--rw-r--r--   0        0        0     9107 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/group.py
--rw-r--r--   0        0        0     1515 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/oauth_token.py
--rw-r--r--   0        0        0      324 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/__init__.py
--rw-r--r--   0        0        0      743 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      848 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3683 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      807 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      146 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/user.py
--rw-r--r--   0        0        0    10255 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/pubsub.py
--rw-r--r--   0        0        0     6934 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/sync_local_socket_connection.py
--rw-r--r--   0        0        0     3593 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/utils.py
--rw-r--r--   0        0        0      103 2023-06-27 03:21:36.038613 flet_runtime-0.8.0.dev1590/src/flet_runtime/version.py
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 flet_runtime-0.8.0.dev1590/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/README.md
+-rw-r--r--   0        0        0      747 2023-06-30 16:42:55.895799 flet_runtime-0.8.0.dev1595/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/__init__.py
+-rw-r--r--   0        0        0    23719 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/app.py
+-rw-r--r--   0        0        0     6309 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/async_local_socket_connection.py
+-rw-r--r--   0        0        0      252 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/__init__.py
+-rw-r--r--   0        0        0     9107 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/group.py
+-rw-r--r--   0        0        0     1515 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/oauth_token.py
+-rw-r--r--   0        0        0      324 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      848 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3683 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      807 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      146 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/user.py
+-rw-r--r--   0        0        0    10255 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/pubsub.py
+-rw-r--r--   0        0        0     6934 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     3593 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/utils.py
+-rw-r--r--   0        0        0      103 2023-06-30 16:42:22.691901 flet_runtime-0.8.0.dev1595/src/flet_runtime/version.py
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 flet_runtime-0.8.0.dev1595/PKG-INFO
```

### Comparing `flet_runtime-0.8.0.dev1590/pyproject.toml` & `flet_runtime-0.8.0.dev1595/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-runtime"
-version = "0.8.0.dev1590"
+version = "0.8.0.dev1595"
 description = "Flet Runtime - a base package for Flet desktop and Flet mobile."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_runtime", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.8.0.dev1590"
+flet-core = "0.8.0.dev1595"
 python = "^3.7"
 oauthlib = "^3.2.2"
 httpx = "^0.24.1"
 typing-extensions = { version = "^4.6.2", python = "<3.8" }
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/app.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,23 +314,26 @@
 ):
     env_port = os.getenv("FLET_SERVER_PORT")
     if env_port is not None and env_port:
         port = int(env_port)
 
     uds_path = os.getenv("FLET_SERVER_UDS_PATH")
 
+    env_assets_dir = os.getenv("FLET_ASSETS_PATH")
+    if env_assets_dir:
+        assets_dir = env_assets_dir
+
     is_socket_server = server is None and (
         is_mobile() or view == AppView.FLET_APP or view == AppView.FLET_APP_HIDDEN
     )
 
     if not is_socket_server:
         server = __start_flet_server(
             host,
             port,
-            assets_dir,
             upload_dir,
             web_renderer,
             use_color_emoji,
             route_url_strategy,
         )
 
     def on_event(conn, e):
@@ -369,14 +372,15 @@
             on_session_created=on_session_created,
         )
     else:
         assert server
         conn = SyncWebSocketConnection(
             server_address=server,
             page_name=env_page_name if not page_name and env_page_name else page_name,
+            assets_dir=assets_dir,
             token=auth_token,
             on_event=on_event,
             on_session_created=on_session_created,
         )
     conn.connect()
     return conn
 
@@ -397,22 +401,25 @@
 ):
     env_port = os.getenv("FLET_SERVER_PORT")
     if env_port is not None and env_port:
         port = int(env_port)
 
     uds_path = os.getenv("FLET_SERVER_UDS_PATH")
 
+    env_assets_dir = os.getenv("FLET_ASSETS_PATH")
+    if env_assets_dir:
+        assets_dir = env_assets_dir
+
     is_socket_server = server is None and (
         is_mobile() or view == AppView.FLET_APP or view == AppView.FLET_APP_HIDDEN
     )
     if not is_socket_server:
         server = __start_flet_server(
             host,
             port,
-            assets_dir,
             upload_dir,
             web_renderer,
             use_color_emoji,
             route_url_strategy,
         )
 
     async def on_event(e):
@@ -453,26 +460,26 @@
             on_session_created=on_session_created,
         )
     else:
         assert server
         conn = AsyncWebSocketConnection(
             server_address=server,
             page_name=env_page_name if not page_name and env_page_name else page_name,
+            assets_dir=assets_dir,
             auth_token=auth_token,
             on_event=on_event,
             on_session_created=on_session_created,
         )
     await conn.connect()
     return conn
 
 
 def __start_flet_server(
     host,
     port,
-    assets_dir,
     upload_dir,
     web_renderer: Optional[WebRenderer],
     use_color_emoji,
     route_url_strategy,
 ):
     server_ip = host if host not in [None, "", "*"] else "127.0.0.1"
 
@@ -527,21 +534,14 @@
     web_root_dir = get_package_web_dir()
 
     if not os.path.exists(web_root_dir):
         raise Exception(f"Web root path not found: {web_root_dir}")
 
     args = [fletd_path, "--content-dir", web_root_dir, "--port", str(port)]
 
-    env_assets_dir = os.getenv("FLET_ASSETS_PATH")
-    if env_assets_dir:
-        assets_dir = env_assets_dir
-
-    if assets_dir:
-        args.extend(["--assets-dir", assets_dir])
-
     creationflags = 0
     start_new_session = False
 
     if os.getenv("FLET_DETACH_FLETD") is None:
         args.append("--attached")
     else:
         if is_windows():
```

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/async_local_socket_connection.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/async_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/authorization.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/oauth_provider.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/oauth_token.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/auth0_oauth_provider.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/azure_oauth_provider.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/github_oauth_provider.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/auth/providers/google_oauth_provider.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/pubsub.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/pubsub.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/sync_local_socket_connection.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/sync_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/src/flet_runtime/utils.py` & `flet_runtime-0.8.0.dev1595/src/flet_runtime/utils.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.8.0.dev1590/PKG-INFO` & `flet_runtime-0.8.0.dev1595/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-runtime
-Version: 0.8.0.dev1590
+Version: 0.8.0.dev1595
 Summary: Flet Runtime - a base package for Flet desktop and Flet mobile.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.8.0.dev1590)
+Requires-Dist: flet-core (==0.8.0.dev1595)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
```

