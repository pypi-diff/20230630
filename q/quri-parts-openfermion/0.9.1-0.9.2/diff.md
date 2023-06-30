# Comparing `tmp/quri_parts_openfermion-0.9.1.tar.gz` & `tmp/quri_parts_openfermion-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_openfermion-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts_openfermion-0.9.2.tar", max compression
```

## Comparing `quri_parts_openfermion-0.9.1.tar` & `quri_parts_openfermion-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/LICENSE
--rw-r--r--   0        0        0      280 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/README.md
--rw-r--r--   0        0        0     1315 2023-03-29 06:14:10.489507 quri_parts_openfermion-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      259 2023-03-29 06:14:09.545508 quri_parts_openfermion-0.9.1/quri_parts/openfermion/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/__init__.py
--rw-r--r--   0        0        0      659 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/ansatz/__init__.py
--rw-r--r--   0        0        0     4333 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/ansatz/kupccgsd.py
--rw-r--r--   0        0        0     3661 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/ansatz/uccsd.py
--rw-r--r--   0        0        0      881 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/operator/__init__.py
--rw-r--r--   0        0        0     1435 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/operator/conversions.py
--rw-r--r--   0        0        0     2245 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/operator/fermion_operator.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/py.typed
--rw-r--r--   0        0        0    11715 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/transforms/__init__.py
--rw-r--r--   0        0        0      720 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/utils/__init__.py
--rw-r--r--   0        0        0     2915 2023-03-29 06:13:57.773528 quri_parts_openfermion-0.9.1/quri_parts/openfermion/utils/add_exp_excitation_gates_trotter_decomposition.py
--rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 quri_parts_openfermion-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.870951 quri_parts_openfermion-0.9.2/LICENSE
+-rw-r--r--   0        0        0      280 2023-03-29 07:37:19.870951 quri_parts_openfermion-0.9.2/README.md
+-rw-r--r--   0        0        0     1315 2023-03-29 07:37:31.019006 quri_parts_openfermion-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-03-29 07:37:30.195002 quri_parts_openfermion-0.9.2/quri_parts/openfermion/NOTICE
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/__init__.py
+-rw-r--r--   0        0        0      659 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/__init__.py
+-rw-r--r--   0        0        0     4333 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/kupccgsd.py
+-rw-r--r--   0        0        0     3661 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/uccsd.py
+-rw-r--r--   0        0        0      881 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/__init__.py
+-rw-r--r--   0        0        0     1435 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/conversions.py
+-rw-r--r--   0        0        0     2245 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/fermion_operator.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/py.typed
+-rw-r--r--   0        0        0    11715 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/transforms/__init__.py
+-rw-r--r--   0        0        0      720 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/utils/__init__.py
+-rw-r--r--   0        0        0     2915 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/utils/add_exp_excitation_gates_trotter_decomposition.py
+-rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 quri_parts_openfermion-0.9.2/PKG-INFO
```

### Comparing `quri_parts_openfermion-0.9.1/LICENSE` & `quri_parts_openfermion-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/pyproject.toml` & `quri_parts_openfermion-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-openfermion"
-version = "0.9.1"
+version = "0.9.2"
 description = "A support library for using OpenFermion with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/ansatz/__init__.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/ansatz/kupccgsd.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/kupccgsd.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/ansatz/uccsd.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/uccsd.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/operator/__init__.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/operator/conversions.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/conversions.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/operator/fermion_operator.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/fermion_operator.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/transforms/__init__.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/utils/__init__.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/quri_parts/openfermion/utils/add_exp_excitation_gates_trotter_decomposition.py` & `quri_parts_openfermion-0.9.2/quri_parts/openfermion/utils/add_exp_excitation_gates_trotter_decomposition.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.1/PKG-INFO` & `quri_parts_openfermion-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-openfermion
-Version: 0.9.1
+Version: 0.9.2
 Summary: A support library for using OpenFermion with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<3.12
```

