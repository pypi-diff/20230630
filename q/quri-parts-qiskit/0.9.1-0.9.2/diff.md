# Comparing `tmp/quri_parts_qiskit-0.9.1.tar.gz` & `tmp/quri_parts_qiskit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_qiskit-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts_qiskit-0.9.2.tar", max compression
```

## Comparing `quri_parts_qiskit-0.9.1.tar` & `quri_parts_qiskit-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.777528 quri_parts_qiskit-0.9.1/LICENSE
--rw-r--r--   0        0        0      260 2023-03-29 06:13:57.777528 quri_parts_qiskit-0.9.1/README.md
--rw-r--r--   0        0        0     1090 2023-03-29 06:14:13.661507 quri_parts_qiskit-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 06:14:12.757507 quri_parts_qiskit-0.9.1/quri_parts/qiskit/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.777528 quri_parts_qiskit-0.9.1/quri_parts/qiskit/__init__.py
--rw-r--r--   0        0        0      724 2023-03-29 06:13:57.777528 quri_parts_qiskit-0.9.1/quri_parts/qiskit/backend/__init__.py
--rw-r--r--   0        0        0     7241 2023-03-29 06:13:57.777528 quri_parts_qiskit-0.9.1/quri_parts/qiskit/backend/sampling.py
--rw-r--r--   0        0        0     6341 2023-03-29 06:13:57.777528 quri_parts_qiskit-0.9.1/quri_parts/qiskit/circuit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.777528 quri_parts_qiskit-0.9.1/quri_parts/qiskit/py.typed
--rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 quri_parts_qiskit-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/LICENSE
+-rw-r--r--   0        0        0      260 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/README.md
+-rw-r--r--   0        0        0     1090 2023-03-29 07:37:33.795022 quri_parts_qiskit-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-03-29 07:37:33.011017 quri_parts_qiskit-0.9.2/quri_parts/qiskit/NOTICE
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/__init__.py
+-rw-r--r--   0        0        0      724 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/backend/__init__.py
+-rw-r--r--   0        0        0     7241 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/backend/sampling.py
+-rw-r--r--   0        0        0     6341 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/circuit/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/py.typed
+-rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 quri_parts_qiskit-0.9.2/PKG-INFO
```

### Comparing `quri_parts_qiskit-0.9.1/LICENSE` & `quri_parts_qiskit-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_qiskit-0.9.1/pyproject.toml` & `quri_parts_qiskit-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-qiskit"
-version = "0.9.1"
+version = "0.9.2"
 description = "A plugin to use Qiskit with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_qiskit-0.9.1/quri_parts/qiskit/backend/__init__.py` & `quri_parts_qiskit-0.9.2/quri_parts/qiskit/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_qiskit-0.9.1/quri_parts/qiskit/backend/sampling.py` & `quri_parts_qiskit-0.9.2/quri_parts/qiskit/backend/sampling.py`

 * *Files identical despite different names*

### Comparing `quri_parts_qiskit-0.9.1/quri_parts/qiskit/circuit/__init__.py` & `quri_parts_qiskit-0.9.2/quri_parts/qiskit/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_qiskit-0.9.1/PKG-INFO` & `quri_parts_qiskit-0.9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-qiskit
-Version: 0.9.1
+Version: 0.9.2
 Summary: A plugin to use Qiskit with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

