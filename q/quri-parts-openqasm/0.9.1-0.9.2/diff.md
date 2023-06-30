# Comparing `tmp/quri_parts_openqasm-0.9.1.tar.gz` & `tmp/quri_parts_openqasm-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_openqasm-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts_openqasm-0.9.2.tar", max compression
```

## Comparing `quri_parts_openqasm-0.9.1.tar` & `quri_parts_openqasm-0.9.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.773528 quri_parts_openqasm-0.9.1/LICENSE
--rw-r--r--   0        0        0      351 2023-03-29 06:13:57.773528 quri_parts_openqasm-0.9.1/README.md
--rw-r--r--   0        0        0     1015 2023-03-29 06:14:11.545507 quri_parts_openqasm-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 06:14:10.649507 quri_parts_openqasm-0.9.1/quri_parts/openqasm/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.773528 quri_parts_openqasm-0.9.1/quri_parts/openqasm/__init__.py
--rw-r--r--   0        0        0     5512 2023-03-29 06:13:57.773528 quri_parts_openqasm-0.9.1/quri_parts/openqasm/circuit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.773528 quri_parts_openqasm-0.9.1/quri_parts/openqasm/py.typed
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 quri_parts_openqasm-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/LICENSE
+-rw-r--r--   0        0        0      351 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/README.md
+-rw-r--r--   0        0        0     1015 2023-03-29 07:37:31.955011 quri_parts_openqasm-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-03-29 07:37:31.159007 quri_parts_openqasm-0.9.2/quri_parts/openqasm/NOTICE
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/quri_parts/openqasm/__init__.py
+-rw-r--r--   0        0        0     5518 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/quri_parts/openqasm/circuit/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/quri_parts/openqasm/py.typed
+-rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 quri_parts_openqasm-0.9.2/PKG-INFO
```

### Comparing `quri_parts_openqasm-0.9.1/LICENSE` & `quri_parts_openqasm-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_openqasm-0.9.1/pyproject.toml` & `quri_parts_openqasm-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "quri-parts-openqasm"
-version = "0.9.1"
+version = "0.9.2"
 description = "A support library for using OpenQASM 3 with QURI Parts"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
 classifiers = [
```

### Comparing `quri_parts_openqasm-0.9.1/quri_parts/openqasm/circuit/__init__.py` & `quri_parts_openqasm-0.9.2/quri_parts/openqasm/circuit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 _single_qubit_gate_stdgates_symbol: Mapping["SingleQubitGateNameType", str] = {
     gate_names.Identity: "id",
     gate_names.X: "x",
     gate_names.Y: "y",
     gate_names.Z: "z",
     gate_names.H: "h",
     gate_names.S: "s",
+    gate_names.SqrtX: "sx",
     gate_names.Sdag: "sdg",
     gate_names.T: "t",
     gate_names.Tdag: "tdg",
 }
 
 _single_qubit_rotation_gate_stdgates_symbol: Mapping["SingleQubitGateNameType", str] = {
     gate_names.RX: "rx",
@@ -73,15 +74,14 @@
 _U_gate_stdgates_symbol: Mapping["SingleQubitGateNameType", str] = {
     gate_names.U1: "u1",
     gate_names.U2: "u2",
     gate_names.U3: "u3",
 }
 
 _not_implemented_gates: set["SingleQubitGateNameType"] = {
-    gate_names.SqrtX,
     gate_names.SqrtXdag,
     gate_names.SqrtY,
     gate_names.SqrtYdag,
 }
 
 
 def convert_to_qasm(
```

### Comparing `quri_parts_openqasm-0.9.1/PKG-INFO` & `quri_parts_openqasm-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-openqasm
-Version: 0.9.1
+Version: 0.9.2
 Summary: A support library for using OpenQASM 3 with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<3.12
 Classifier: Programming Language :: Python :: 3
```

