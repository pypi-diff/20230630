# Comparing `tmp/quri_parts_braket-0.9.1.tar.gz` & `tmp/quri_parts_braket-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_braket-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts_braket-0.9.2.tar", max compression
```

## Comparing `quri_parts_braket-0.9.1.tar` & `quri_parts_braket-0.9.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/LICENSE
--rw-r--r--   0        0        0      369 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/README.md
--rw-r--r--   0        0        0     1197 2023-03-29 06:14:01.753515 quri_parts_braket-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 06:14:00.853518 quri_parts_braket-0.9.1/quri_parts/braket/NOTICE
--rw-r--r--   0        0        0      541 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/quri_parts/braket/__init__.py
--rw-r--r--   0        0        0      803 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/quri_parts/braket/backend/__init__.py
--rw-r--r--   0        0        0     1452 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/quri_parts/braket/backend/device.py
--rw-r--r--   0        0        0     7359 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/quri_parts/braket/backend/sampling.py
--rw-r--r--   0        0        0     1310 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/quri_parts/braket/backend/transpiler.py
--rw-r--r--   0        0        0     6576 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/quri_parts/braket/circuit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.757528 quri_parts_braket-0.9.1/quri_parts/braket/py.typed
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 quri_parts_braket-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/LICENSE
+-rw-r--r--   0        0        0      369 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/README.md
+-rw-r--r--   0        0        0     1197 2023-03-29 07:37:23.482965 quri_parts_braket-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-03-29 07:37:22.614960 quri_parts_braket-0.9.2/quri_parts/braket/NOTICE
+-rw-r--r--   0        0        0      541 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/__init__.py
+-rw-r--r--   0        0        0      803 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/backend/__init__.py
+-rw-r--r--   0        0        0     1452 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/backend/device.py
+-rw-r--r--   0        0        0     7359 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/backend/sampling.py
+-rw-r--r--   0        0        0     1310 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/backend/transpiler.py
+-rw-r--r--   0        0        0     6576 2023-03-29 07:37:19.858951 quri_parts_braket-0.9.2/quri_parts/braket/circuit/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.858951 quri_parts_braket-0.9.2/quri_parts/braket/py.typed
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 quri_parts_braket-0.9.2/PKG-INFO
```

### Comparing `quri_parts_braket-0.9.1/LICENSE` & `quri_parts_braket-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.1/pyproject.toml` & `quri_parts_braket-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-braket"
-version = "0.9.1"
+version = "0.9.2"
 description = "A plugin to use Amazon Braket SDK with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_braket-0.9.1/quri_parts/braket/__init__.py` & `quri_parts_braket-0.9.2/quri_parts/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.1/quri_parts/braket/backend/__init__.py` & `quri_parts_braket-0.9.2/quri_parts/braket/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.1/quri_parts/braket/backend/device.py` & `quri_parts_braket-0.9.2/quri_parts/braket/backend/device.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.1/quri_parts/braket/backend/sampling.py` & `quri_parts_braket-0.9.2/quri_parts/braket/backend/sampling.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.1/quri_parts/braket/backend/transpiler.py` & `quri_parts_braket-0.9.2/quri_parts/braket/backend/transpiler.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.1/quri_parts/braket/circuit/__init__.py` & `quri_parts_braket-0.9.2/quri_parts/braket/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.1/PKG-INFO` & `quri_parts_braket-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-braket
-Version: 0.9.1
+Version: 0.9.2
 Summary: A plugin to use Amazon Braket SDK with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

