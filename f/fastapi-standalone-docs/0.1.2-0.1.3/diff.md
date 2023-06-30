# Comparing `tmp/fastapi_standalone_docs-0.1.2.tar.gz` & `tmp/fastapi_standalone_docs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_standalone_docs-0.1.2.tar", max compression
+gzip compressed data, was "fastapi_standalone_docs-0.1.3.tar", max compression
```

## Comparing `fastapi_standalone_docs-0.1.2.tar` & `fastapi_standalone_docs-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/LICENSE
--rw-r--r--   0        0        0     4618 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/README.md
--rw-r--r--   0        0        0       82 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/__init__.py
--rw-r--r--   0        0        0     1828 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/scripts.py
--rw-r--r--   0        0        0     2759 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/standalone_docs.py
--rw-r--r--   0        0        0     1086 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/fastapi/LICENSE
--rw-r--r--   0        0        0      412 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/fastapi/favicon.png
--rw-r--r--   0        0        0     1174 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/logo-mini.svg
--rw-r--r--   0        0        0  1042510 2023-06-26 07:12:36.528958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/redoc.standalone.js
--rw-r--r--   0        0        0     2628 2023-06-26 07:12:36.528958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt
--rw-r--r--   0        0        0    11358 2023-06-26 07:12:36.528958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/LICENSE
--rw-r--r--   0        0        0  1048219 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js
--rw-r--r--   0        0        0   145206 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/swagger-ui.css
--rw-r--r--   0        0        0        0 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/tests/conftests.py
--rw-r--r--   0        0        0     6131 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/tests/test_standalone_docs.py
--rw-r--r--   0        0        0      852 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 fastapi_standalone_docs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4609 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/README.md
+-rw-r--r--   0        0        0       82 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/__init__.py
+-rw-r--r--   0        0        0     1828 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/scripts.py
+-rw-r--r--   0        0        0     2759 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/standalone_docs.py
+-rw-r--r--   0        0        0     1086 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/fastapi/LICENSE
+-rw-r--r--   0        0        0      412 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/fastapi/favicon.png
+-rw-r--r--   0        0        0     1174 2023-06-30 12:21:39.140591 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/logo-mini.svg
+-rw-r--r--   0        0        0  1042510 2023-06-30 12:21:39.148592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/redoc.standalone.js
+-rw-r--r--   0        0        0     2628 2023-06-30 12:21:39.148592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0        0        0    11358 2023-06-30 12:21:39.148592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/LICENSE
+-rw-r--r--   0        0        0  1048219 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   145206 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/swagger-ui.css
+-rw-r--r--   0        0        0        0 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/tests/conftests.py
+-rw-r--r--   0        0        0     6131 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/tests/test_standalone_docs.py
+-rw-r--r--   0        0        0      852 2023-06-30 12:21:39.156592 fastapi_standalone_docs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 fastapi_standalone_docs-0.1.3/PKG-INFO
```

### Comparing `fastapi_standalone_docs-0.1.2/LICENSE` & `fastapi_standalone_docs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/README.md` & `fastapi_standalone_docs-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # FastAPI Standalone Docs
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ioxiocom/fastapi-standalone-docs/publish.yaml)](https://github.com/ioxiocom/fastapi-standalone-docs/actions/workflows/publish.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/fastapi-standalone-docs)](https://pypi.org/project/fastapi-standalone-docs/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-standalone-docs)](https://pypi.org/project/fastapi-standalone-docs/)
-[![License: BSD 3-Clause](https://img.shields.io/pypi/l/fastapi-standalone-docs)](https://opensource.org/license/mit/)
+[![License: MIT](https://img.shields.io/pypi/l/fastapi-standalone-docs)](https://opensource.org/license/mit/)
 
 Host FastAPI Swagger UI and ReDoc without any third party CDNs. Handy if you want to be
 able to use the docs offline or want to avoid loading content from 3rd party CDNs due to
 privacy reasons.
 
 This library was heavily inspired by
 [fastapi-offline-swagger-ui](https://github.com/ahmetoner/fastapi-offline-swagger-ui),
```

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/scripts.py` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/scripts.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/standalone_docs.py` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/standalone_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/fastapi/LICENSE` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/fastapi/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/logo-mini.svg` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/logo-mini.svg`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/redoc.standalone.js` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/LICENSE` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/swagger-ui.css` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/static/swagger/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/tests/test_standalone_docs.py` & `fastapi_standalone_docs-0.1.3/fastapi_standalone_docs/tests/test_standalone_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.2/pyproject.toml` & `fastapi_standalone_docs-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-standalone-docs"
-version = "0.1.2"
+version = "0.1.3"
 description = "Host FastAPI Swagger UI and ReDoc without third party CDNs"
 authors = ["IOXIO Ltd"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ioxiocom/fastapi-standalone-docs"
 packages = [{include = "fastapi_standalone_docs"}]
```

### Comparing `fastapi_standalone_docs-0.1.2/PKG-INFO` & `fastapi_standalone_docs-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-standalone-docs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Host FastAPI Swagger UI and ReDoc without third party CDNs
 Home-page: https://github.com/ioxiocom/fastapi-standalone-docs
 License: MIT
 Author: IOXIO Ltd
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 
 # FastAPI Standalone Docs
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ioxiocom/fastapi-standalone-docs/publish.yaml)](https://github.com/ioxiocom/fastapi-standalone-docs/actions/workflows/publish.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/fastapi-standalone-docs)](https://pypi.org/project/fastapi-standalone-docs/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-standalone-docs)](https://pypi.org/project/fastapi-standalone-docs/)
-[![License: BSD 3-Clause](https://img.shields.io/pypi/l/fastapi-standalone-docs)](https://opensource.org/license/mit/)
+[![License: MIT](https://img.shields.io/pypi/l/fastapi-standalone-docs)](https://opensource.org/license/mit/)
 
 Host FastAPI Swagger UI and ReDoc without any third party CDNs. Handy if you want to be
 able to use the docs offline or want to avoid loading content from 3rd party CDNs due to
 privacy reasons.
 
 This library was heavily inspired by
 [fastapi-offline-swagger-ui](https://github.com/ahmetoner/fastapi-offline-swagger-ui),
```

