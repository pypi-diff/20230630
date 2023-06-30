# Comparing `tmp/quri_parts_circuit-0.9.1.tar.gz` & `tmp/quri_parts_circuit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_circuit-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts_circuit-0.9.2.tar", max compression
```

## Comparing `quri_parts_circuit-0.9.1.tar` & `quri_parts_circuit-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.757528 quri_parts_circuit-0.9.1/LICENSE
--rw-r--r--   0        0        0      259 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/README.md
--rw-r--r--   0        0        0     1022 2023-03-29 06:14:03.809508 quri_parts_circuit-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      201 2023-03-29 06:14:02.961511 quri_parts_circuit-0.9.1/quri_parts/circuit/NOTICE
--rw-r--r--   0        0        0     3636 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/__init__.py
--rw-r--r--   0        0        0    11742 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/circuit.py
--rw-r--r--   0        0        0     9067 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/circuit_linear_mapped.py
--rw-r--r--   0        0        0    14569 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/circuit_parametric.py
--rw-r--r--   0        0        0     2324 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/clifford_gate.py
--rw-r--r--   0        0        0     1496 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/gate.py
--rw-r--r--   0        0        0     5263 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/gate_names.py
--rw-r--r--   0        0        0    14467 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/gates.py
--rw-r--r--   0        0        0     2167 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/inverse_gate.py
--rw-r--r--   0        0        0     1880 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/noise/__init__.py
--rw-r--r--   0        0        0    35663 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/noise/noise_instruction.py
--rw-r--r--   0        0        0    14041 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/noise/noise_model.py
--rw-r--r--   0        0        0     1250 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/parameter.py
--rw-r--r--   0        0        0    11601 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/parameter_mapping.py
--rw-r--r--   0        0        0     5514 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/parameter_shift.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/py.typed
--rw-r--r--   0        0        0      702 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/topology/__init__.py
--rw-r--r--   0        0        0     5227 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/topology/square_lattice.py
--rw-r--r--   0        0        0     5759 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/__init__.py
--rw-r--r--   0        0        0     3289 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/clifford_approximation.py
--rw-r--r--   0        0        0    16837 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/gate_kind_decomposer.py
--rw-r--r--   0        0        0     1518 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/identity_insertion.py
--rw-r--r--   0        0        0     2845 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/multi_pauli_decomposer.py
--rw-r--r--   0        0        0     2358 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/qubit_remapping.py
--rw-r--r--   0        0        0     5221 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/transpiler.py
--rw-r--r--   0        0        0     3835 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/unitary_matrix_decomposer.py
--rw-r--r--   0        0        0     2387 2023-03-29 06:13:57.761528 quri_parts_circuit-0.9.1/quri_parts/circuit/utils/controlled_rotations.py
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 quri_parts_circuit-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/LICENSE
+-rw-r--r--   0        0        0      259 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/README.md
+-rw-r--r--   0        0        0     1022 2023-03-29 07:37:25.310975 quri_parts_circuit-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      201 2023-03-29 07:37:24.538971 quri_parts_circuit-0.9.2/quri_parts/circuit/NOTICE
+-rw-r--r--   0        0        0     3636 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/__init__.py
+-rw-r--r--   0        0        0    11742 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/circuit.py
+-rw-r--r--   0        0        0     9067 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/circuit_linear_mapped.py
+-rw-r--r--   0        0        0    14569 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/circuit_parametric.py
+-rw-r--r--   0        0        0     2324 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/clifford_gate.py
+-rw-r--r--   0        0        0     1496 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/gate.py
+-rw-r--r--   0        0        0     5263 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/gate_names.py
+-rw-r--r--   0        0        0    14467 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/gates.py
+-rw-r--r--   0        0        0     2167 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/inverse_gate.py
+-rw-r--r--   0        0        0     1880 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/noise/__init__.py
+-rw-r--r--   0        0        0    35663 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/noise/noise_instruction.py
+-rw-r--r--   0        0        0    14041 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/noise/noise_model.py
+-rw-r--r--   0        0        0     1250 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/parameter.py
+-rw-r--r--   0        0        0    11601 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/parameter_mapping.py
+-rw-r--r--   0        0        0     5514 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/parameter_shift.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/py.typed
+-rw-r--r--   0        0        0      702 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/topology/__init__.py
+-rw-r--r--   0        0        0     5227 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/topology/square_lattice.py
+-rw-r--r--   0        0        0     5759 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/__init__.py
+-rw-r--r--   0        0        0     3289 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/clifford_approximation.py
+-rw-r--r--   0        0        0    16837 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/gate_kind_decomposer.py
+-rw-r--r--   0        0        0     1518 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/identity_insertion.py
+-rw-r--r--   0        0        0     2845 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/multi_pauli_decomposer.py
+-rw-r--r--   0        0        0     2358 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/qubit_remapping.py
+-rw-r--r--   0        0        0     5221 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/transpiler.py
+-rw-r--r--   0        0        0     3835 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/unitary_matrix_decomposer.py
+-rw-r--r--   0        0        0     2387 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/utils/controlled_rotations.py
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 quri_parts_circuit-0.9.2/PKG-INFO
```

### Comparing `quri_parts_circuit-0.9.1/LICENSE` & `quri_parts_circuit-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/pyproject.toml` & `quri_parts_circuit-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-circuit"
-version = "0.9.1"
+version = "0.9.2"
 description = "Platform-independent quantum circuit library"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/__init__.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/circuit.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/circuit.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/circuit_linear_mapped.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/circuit_linear_mapped.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/circuit_parametric.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/circuit_parametric.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/clifford_gate.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/clifford_gate.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/gate.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/gate.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/gate_names.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/gate_names.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/gates.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/gates.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/inverse_gate.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/inverse_gate.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/noise/__init__.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/noise/noise_instruction.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/noise/noise_instruction.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/noise/noise_model.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/noise/noise_model.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/parameter.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/parameter.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/parameter_mapping.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/parameter_mapping.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/parameter_shift.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/parameter_shift.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/topology/__init__.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/topology/square_lattice.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/topology/square_lattice.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/__init__.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/clifford_approximation.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/clifford_approximation.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/gate_kind_decomposer.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/gate_kind_decomposer.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/identity_insertion.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/identity_insertion.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/multi_pauli_decomposer.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/multi_pauli_decomposer.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/qubit_remapping.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/qubit_remapping.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/transpiler.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/transpiler.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/transpile/unitary_matrix_decomposer.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/unitary_matrix_decomposer.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/quri_parts/circuit/utils/controlled_rotations.py` & `quri_parts_circuit-0.9.2/quri_parts/circuit/utils/controlled_rotations.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.1/PKG-INFO` & `quri_parts_circuit-0.9.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-circuit
-Version: 0.9.1
+Version: 0.9.2
 Summary: Platform-independent quantum circuit library
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

