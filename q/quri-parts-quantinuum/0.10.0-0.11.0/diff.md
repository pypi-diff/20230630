# Comparing `tmp/quri_parts_quantinuum-0.10.0.tar.gz` & `tmp/quri_parts_quantinuum-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_quantinuum-0.10.0.tar", max compression
+gzip compressed data, was "quri_parts_quantinuum-0.11.0.tar", max compression
```

## Comparing `quri_parts_quantinuum-0.10.0.tar` & `quri_parts_quantinuum-0.11.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/LICENSE
--rw-r--r--   0        0        0      276 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/README.md
--rw-r--r--   0        0        0     1134 2023-04-28 01:51:47.068525 quri_parts_quantinuum-0.10.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-28 01:51:46.448532 quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/NOTICE
--rw-r--r--   0        0        0        0 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/__init__.py
--rw-r--r--   0        0        0      621 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/__init__.py
--rw-r--r--   0        0        0      651 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/gate_names.py
--rw-r--r--   0        0        0     2867 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/gates.py
--rw-r--r--   0        0        0     1794 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/transpile/__init__.py
--rw-r--r--   0        0        0     6901 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/transpile/quantinuum_native_transpiler.py
--rw-r--r--   0        0        0        0 2023-04-28 01:51:36.420632 quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/py.typed
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 quri_parts_quantinuum-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/LICENSE
+-rw-r--r--   0        0        0      276 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/README.md
+-rw-r--r--   0        0        0     1134 2023-05-30 10:40:29.815918 quri_parts_quantinuum-0.11.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-30 10:40:28.983893 quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/NOTICE
+-rw-r--r--   0        0        0        0 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/__init__.py
+-rw-r--r--   0        0        0      621 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/__init__.py
+-rw-r--r--   0        0        0      651 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/gate_names.py
+-rw-r--r--   0        0        0     2867 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/gates.py
+-rw-r--r--   0        0        0     1794 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/transpile/__init__.py
+-rw-r--r--   0        0        0     6901 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/transpile/quantinuum_native_transpiler.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:40:14.639340 quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/py.typed
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 quri_parts_quantinuum-0.11.0/PKG-INFO
```

### Comparing `quri_parts_quantinuum-0.10.0/LICENSE` & `quri_parts_quantinuum-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.10.0/pyproject.toml` & `quri_parts_quantinuum-0.11.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-quantinuum"
-version = "0.10.0"
+version = "0.11.0"
 description = "A plugin to use Quantinuum with QIRI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <support@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/__init__.py` & `quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/gate_names.py` & `quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/gate_names.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/gates.py` & `quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/gates.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/transpile/__init__.py` & `quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.10.0/quri_parts/quantinuum/circuit/transpile/quantinuum_native_transpiler.py` & `quri_parts_quantinuum-0.11.0/quri_parts/quantinuum/circuit/transpile/quantinuum_native_transpiler.py`

 * *Files identical despite different names*

### Comparing `quri_parts_quantinuum-0.10.0/PKG-INFO` & `quri_parts_quantinuum-0.11.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-quantinuum
-Version: 0.10.0
+Version: 0.11.0
 Summary: A plugin to use Quantinuum with QIRI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: support@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

