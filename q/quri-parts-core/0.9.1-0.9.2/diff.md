# Comparing `tmp/quri_parts_core-0.9.1.tar.gz` & `tmp/quri_parts_core-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_core-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts_core-0.9.2.tar", max compression
```

## Comparing `quri_parts_core-0.9.1.tar` & `quri_parts_core-0.9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/LICENSE
--rw-r--r--   0        0        0      288 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/README.md
--rw-r--r--   0        0        0     1169 2023-03-29 06:14:06.029509 quri_parts_core-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2691 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/backend/py.typed
--rw-r--r--   0        0        0     3382 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/backend/qubit_mapping.py
--rw-r--r--   0        0        0       34 2023-03-29 06:14:05.077509 quri_parts_core-0.9.1/quri_parts/core/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/__init__.py
--rw-r--r--   0        0        0     1215 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/circuit/exp_single_pauli_gate.py
--rw-r--r--   0        0        0     7710 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/estimator/__init__.py
--rw-r--r--   0        0        0     6657 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/estimator/gradient.py
--rw-r--r--   0        0        0     2343 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/estimator/sampling/__init__.py
--rw-r--r--   0        0        0     9705 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/estimator/sampling/estimator.py
--rw-r--r--   0        0        0     6287 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/estimator/sampling/pauli.py
--rw-r--r--   0        0        0     2228 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/measurement/__init__.py
--rw-r--r--   0        0        0     4929 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/measurement/bitwise_commuting_pauli.py
--rw-r--r--   0        0        0     2818 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/measurement/interface.py
--rw-r--r--   0        0        0     1329 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/__init__.py
--rw-r--r--   0        0        0     7257 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/conjugation.py
--rw-r--r--   0        0        0     1312 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/grouping/__init__.py
--rw-r--r--   0        0        0     5551 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/grouping/pauli_grouping.py
--rw-r--r--   0        0        0     5683 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/operator.py
--rw-r--r--   0        0        0    10528 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/pauli.py
--rw-r--r--   0        0        0     2325 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/representation/__init__.py
--rw-r--r--   0        0        0     1545 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/representation/bsf.py
--rw-r--r--   0        0        0     3597 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/operator/trotter_suzuki.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/py.typed
--rw-r--r--   0        0        0     3424 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/sampling/__init__.py
--rw-r--r--   0        0        0     6076 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/sampling/shots_allocator.py
--rw-r--r--   0        0        0     2617 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/state/__init__.py
--rw-r--r--   0        0        0     7057 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/state/comp_basis.py
--rw-r--r--   0        0        0     3399 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/state/state.py
--rw-r--r--   0        0        0     3604 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/state/state_parametric.py
--rw-r--r--   0        0        0     2927 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/state/state_vector.py
--rw-r--r--   0        0        0     3380 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/state/state_vector_parametric.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/utils/__init__.py
--rw-r--r--   0        0        0     1142 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/utils/array.py
--rw-r--r--   0        0        0     8991 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/utils/binary_field.py
--rw-r--r--   0        0        0     1403 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/utils/bit.py
--rw-r--r--   0        0        0     1936 2023-03-29 06:13:57.765528 quri_parts_core-0.9.1/quri_parts/core/utils/concurrent.py
--rw-r--r--   0        0        0     6161 2023-03-29 06:13:57.769528 quri_parts_core-0.9.1/quri_parts/core/utils/differentiation.py
--rw-r--r--   0        0        0     1458 2023-03-29 06:13:57.769528 quri_parts_core-0.9.1/quri_parts/core/utils/statistics.py
--rw-r--r--   0        0        0     1186 1970-01-01 00:00:00.000000 quri_parts_core-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/LICENSE
+-rw-r--r--   0        0        0      288 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/README.md
+-rw-r--r--   0        0        0     1169 2023-03-29 07:37:27.166985 quri_parts_core-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2691 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/backend/py.typed
+-rw-r--r--   0        0        0     3382 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/backend/qubit_mapping.py
+-rw-r--r--   0        0        0       34 2023-03-29 07:37:26.378981 quri_parts_core-0.9.2/quri_parts/core/NOTICE
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/__init__.py
+-rw-r--r--   0        0        0     1215 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/circuit/exp_single_pauli_gate.py
+-rw-r--r--   0        0        0     7710 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/__init__.py
+-rw-r--r--   0        0        0     6657 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/gradient.py
+-rw-r--r--   0        0        0     2343 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/__init__.py
+-rw-r--r--   0        0        0     9705 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/estimator.py
+-rw-r--r--   0        0        0     6287 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/pauli.py
+-rw-r--r--   0        0        0     2228 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/measurement/__init__.py
+-rw-r--r--   0        0        0     4929 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/measurement/bitwise_commuting_pauli.py
+-rw-r--r--   0        0        0     2818 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/measurement/interface.py
+-rw-r--r--   0        0        0     1329 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/__init__.py
+-rw-r--r--   0        0        0     7257 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/conjugation.py
+-rw-r--r--   0        0        0     1312 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/grouping/__init__.py
+-rw-r--r--   0        0        0     5551 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/grouping/pauli_grouping.py
+-rw-r--r--   0        0        0     5683 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/operator.py
+-rw-r--r--   0        0        0    10528 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/pauli.py
+-rw-r--r--   0        0        0     2325 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/representation/__init__.py
+-rw-r--r--   0        0        0     1545 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/representation/bsf.py
+-rw-r--r--   0        0        0     3597 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/trotter_suzuki.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/py.typed
+-rw-r--r--   0        0        0     3424 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/sampling/__init__.py
+-rw-r--r--   0        0        0     6076 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/sampling/shots_allocator.py
+-rw-r--r--   0        0        0     2617 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/__init__.py
+-rw-r--r--   0        0        0     7057 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/comp_basis.py
+-rw-r--r--   0        0        0     3399 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/state.py
+-rw-r--r--   0        0        0     3604 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/state_parametric.py
+-rw-r--r--   0        0        0     2927 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/state_vector.py
+-rw-r--r--   0        0        0     3380 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/state_vector_parametric.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/__init__.py
+-rw-r--r--   0        0        0     1142 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/array.py
+-rw-r--r--   0        0        0     8991 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/binary_field.py
+-rw-r--r--   0        0        0     1403 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/bit.py
+-rw-r--r--   0        0        0     1936 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/concurrent.py
+-rw-r--r--   0        0        0     6161 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/differentiation.py
+-rw-r--r--   0        0        0     1458 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/statistics.py
+-rw-r--r--   0        0        0     1186 1970-01-01 00:00:00.000000 quri_parts_core-0.9.2/PKG-INFO
```

### Comparing `quri_parts_core-0.9.1/LICENSE` & `quri_parts_core-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/pyproject.toml` & `quri_parts_core-0.9.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-core"
-version = "0.9.1"
+version = "0.9.2"
 description = "A platform-independent library for quantum computing"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_core-0.9.1/quri_parts/backend/__init__.py` & `quri_parts_core-0.9.2/quri_parts/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/backend/qubit_mapping.py` & `quri_parts_core-0.9.2/quri_parts/backend/qubit_mapping.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/circuit/exp_single_pauli_gate.py` & `quri_parts_core-0.9.2/quri_parts/core/circuit/exp_single_pauli_gate.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/estimator/__init__.py` & `quri_parts_core-0.9.2/quri_parts/core/estimator/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/estimator/gradient.py` & `quri_parts_core-0.9.2/quri_parts/core/estimator/gradient.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/estimator/sampling/__init__.py` & `quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/estimator/sampling/estimator.py` & `quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/estimator.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/estimator/sampling/pauli.py` & `quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/pauli.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/measurement/__init__.py` & `quri_parts_core-0.9.2/quri_parts/core/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/measurement/bitwise_commuting_pauli.py` & `quri_parts_core-0.9.2/quri_parts/core/measurement/bitwise_commuting_pauli.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/measurement/interface.py` & `quri_parts_core-0.9.2/quri_parts/core/measurement/interface.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/__init__.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/conjugation.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/conjugation.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/grouping/__init__.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/grouping/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/grouping/pauli_grouping.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/grouping/pauli_grouping.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/operator.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/operator.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/pauli.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/pauli.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/representation/__init__.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/representation/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/representation/bsf.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/representation/bsf.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/operator/trotter_suzuki.py` & `quri_parts_core-0.9.2/quri_parts/core/operator/trotter_suzuki.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/sampling/__init__.py` & `quri_parts_core-0.9.2/quri_parts/core/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/sampling/shots_allocator.py` & `quri_parts_core-0.9.2/quri_parts/core/sampling/shots_allocator.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/state/__init__.py` & `quri_parts_core-0.9.2/quri_parts/core/state/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/state/comp_basis.py` & `quri_parts_core-0.9.2/quri_parts/core/state/comp_basis.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/state/state.py` & `quri_parts_core-0.9.2/quri_parts/core/state/state.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/state/state_parametric.py` & `quri_parts_core-0.9.2/quri_parts/core/state/state_parametric.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/state/state_vector.py` & `quri_parts_core-0.9.2/quri_parts/core/state/state_vector.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/state/state_vector_parametric.py` & `quri_parts_core-0.9.2/quri_parts/core/state/state_vector_parametric.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/utils/array.py` & `quri_parts_core-0.9.2/quri_parts/core/utils/array.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/utils/binary_field.py` & `quri_parts_core-0.9.2/quri_parts/core/utils/binary_field.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/utils/bit.py` & `quri_parts_core-0.9.2/quri_parts/core/utils/bit.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/utils/concurrent.py` & `quri_parts_core-0.9.2/quri_parts/core/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/utils/differentiation.py` & `quri_parts_core-0.9.2/quri_parts/core/utils/differentiation.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/quri_parts/core/utils/statistics.py` & `quri_parts_core-0.9.2/quri_parts/core/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.1/PKG-INFO` & `quri_parts_core-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: A platform-independent library for quantum computing
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

