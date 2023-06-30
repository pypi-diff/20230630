# Comparing `tmp/watchmen_rest-16.5.8.tar.gz` & `tmp/watchmen_rest-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_rest-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_rest-16.5.9.tar", max compression
```

## Comparing `watchmen_rest-16.5.8.tar` & `watchmen_rest-16.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/LICENSE
--rw-r--r--   0        0        0      658 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/pyproject.toml
--rw-r--r--   0        0        0      668 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/__init__.py
--rw-r--r--   0        0        0     2089 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/auth_helper.py
--rw-r--r--   0        0        0     5801 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/authentication.py
--rw-r--r--   0        0        0      419 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/cors.py
--rw-r--r--   0        0        0       98 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/exceptions.py
--rw-r--r--   0        0        0      295 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/prometheus.py
--rw-r--r--   0        0        0     2492 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/rest_app.py
--rw-r--r--   0        0        0      938 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/settings.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/system/__init__.py
--rw-r--r--   0        0        0      139 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/system/health_router.py
--rw-r--r--   0        0        0      130 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/util/__init__.py
--rw-r--r--   0        0        0     1467 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/util/raise_http_exception.py
--rw-r--r--   0        0        0      949 2023-06-08 03:33:39.215631 watchmen_rest-16.5.8/src/watchmen_rest/util/validator.py
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 watchmen_rest-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.895968 watchmen_rest-16.5.9/LICENSE
+-rw-r--r--   0        0        0      658 2023-06-10 16:48:37.895968 watchmen_rest-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0      668 2023-06-10 16:48:37.895968 watchmen_rest-16.5.9/src/watchmen_rest/__init__.py
+-rw-r--r--   0        0        0     2089 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/auth_helper.py
+-rw-r--r--   0        0        0     5801 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/authentication.py
+-rw-r--r--   0        0        0      419 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/cors.py
+-rw-r--r--   0        0        0       98 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/exceptions.py
+-rw-r--r--   0        0        0      295 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/prometheus.py
+-rw-r--r--   0        0        0     2494 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/rest_app.py
+-rw-r--r--   0        0        0      938 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/settings.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/system/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/system/health_router.py
+-rw-r--r--   0        0        0      130 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/util/__init__.py
+-rw-r--r--   0        0        0     1467 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/util/raise_http_exception.py
+-rw-r--r--   0        0        0      949 2023-06-10 16:48:37.899968 watchmen_rest-16.5.9/src/watchmen_rest/util/validator.py
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 watchmen_rest-16.5.9/PKG-INFO
```

### Comparing `watchmen_rest-16.5.8/LICENSE` & `watchmen_rest-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.8/pyproject.toml` & `watchmen_rest-16.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "watchmen-rest"
-version = "16.5.8"
+version = "16.5.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_rest", from = "src" }
 ]
 
@@ -13,16 +13,16 @@
 fastapi = "^0.75.1"
 uvicorn = "^0.17.6"
 jsonschema = "^4.4.0"
 python-jose = "^3.3.0"
 # jose = "^1.0.0"
 python-dotenv = "^0.20.0"
 starlette-prometheus = { version = "^0.9.0", optional = true }
-watchmen-auth = "16.5.8"
-watchmen-storage = "16.5.8"
+watchmen-auth = "16.5.9"
+watchmen-storage = "16.5.9"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `watchmen_rest-16.5.8/src/watchmen_rest/__init__.py` & `watchmen_rest-16.5.9/src/watchmen_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.8/src/watchmen_rest/auth_helper.py` & `watchmen_rest-16.5.9/src/watchmen_rest/auth_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.8/src/watchmen_rest/authentication.py` & `watchmen_rest-16.5.9/src/watchmen_rest/authentication.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.8/src/watchmen_rest/rest_app.py` & `watchmen_rest-16.5.9/src/watchmen_rest/rest_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 logger = getLogger(f'app.{__name__}')
 
 
 class RestApp:
 	def __init__(self, settings: RestSettings):
 		self.settings = settings
-		logger.info(f'Application settings[{settings.dict()}].')
+		# logger.info(f'Application settings[{settings.dict()}].')
 
 	def get_settings(self) -> RestSettings:
 		return self.settings
 
 	def construct(self) -> FastAPI:
 		app = FastAPI(
 			title=self.settings.APP_NAME,
```

### Comparing `watchmen_rest-16.5.8/src/watchmen_rest/settings.py` & `watchmen_rest-16.5.9/src/watchmen_rest/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.8/src/watchmen_rest/util/raise_http_exception.py` & `watchmen_rest-16.5.9/src/watchmen_rest/util/raise_http_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.8/src/watchmen_rest/util/validator.py` & `watchmen_rest-16.5.9/src/watchmen_rest/util/validator.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.8/PKG-INFO` & `watchmen_rest-16.5.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-rest
-Version: 16.5.8
+Version: 16.5.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,9 +13,9 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.75.1,<0.76.0)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: starlette-prometheus (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn (>=0.17.6,<0.18.0)
-Requires-Dist: watchmen-auth (==16.5.8)
-Requires-Dist: watchmen-storage (==16.5.8)
+Requires-Dist: watchmen-auth (==16.5.9)
+Requires-Dist: watchmen-storage (==16.5.9)
```

