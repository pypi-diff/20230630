# Comparing `tmp/quri_parts_chem-0.9.1.tar.gz` & `tmp/quri_parts_chem-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_chem-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts_chem-0.9.2.tar", max compression
```

## Comparing `quri_parts_chem-0.9.1.tar` & `quri_parts_chem-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/LICENSE
--rw-r--r--   0        0        0      285 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/README.md
--rw-r--r--   0        0        0     1132 2023-03-29 06:14:02.801511 quri_parts_chem-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 06:14:01.901514 quri_parts_chem-0.9.1/quri_parts/chem/NOTICE
--rw-r--r--   0        0        0      315 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/ansatz/__init__.py
--rw-r--r--   0        0        0     2297 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/ansatz/all_singles_doubles.py
--rw-r--r--   0        0        0     3555 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/ansatz/gate_fabric.py
--rw-r--r--   0        0        0     3925 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/ansatz/particle_conserving_u1.py
--rw-r--r--   0        0        0     2814 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/ansatz/particle_conserving_u2.py
--rw-r--r--   0        0        0     1145 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/mol/__init__.py
--rw-r--r--   0        0        0     2989 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/mol/active_space.py
--rw-r--r--   0        0        0     6287 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/mol/models.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/py.typed
--rw-r--r--   0        0        0     4515 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/transforms/__init__.py
--rw-r--r--   0        0        0     6307 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/utils/excitations.py
--rw-r--r--   0        0        0     2076 2023-03-29 06:13:57.757528 quri_parts_chem-0.9.1/quri_parts/chem/utils/orbital_rotation.py
--rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 quri_parts_chem-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/LICENSE
+-rw-r--r--   0        0        0      285 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/README.md
+-rw-r--r--   0        0        0     1132 2023-03-29 07:37:24.406970 quri_parts_chem-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-03-29 07:37:23.610965 quri_parts_chem-0.9.2/quri_parts/chem/NOTICE
+-rw-r--r--   0        0        0      315 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/ansatz/__init__.py
+-rw-r--r--   0        0        0     2297 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/ansatz/all_singles_doubles.py
+-rw-r--r--   0        0        0     3555 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/ansatz/gate_fabric.py
+-rw-r--r--   0        0        0     3925 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/ansatz/particle_conserving_u1.py
+-rw-r--r--   0        0        0     2814 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/ansatz/particle_conserving_u2.py
+-rw-r--r--   0        0        0     1145 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/mol/__init__.py
+-rw-r--r--   0        0        0     2989 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/mol/active_space.py
+-rw-r--r--   0        0        0     6287 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/mol/models.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/py.typed
+-rw-r--r--   0        0        0     4515 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/transforms/__init__.py
+-rw-r--r--   0        0        0     6307 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/utils/excitations.py
+-rw-r--r--   0        0        0     2076 2023-03-29 07:37:19.858951 quri_parts_chem-0.9.2/quri_parts/chem/utils/orbital_rotation.py
+-rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 quri_parts_chem-0.9.2/PKG-INFO
```

### Comparing `quri_parts_chem-0.9.1/LICENSE` & `quri_parts_chem-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/pyproject.toml` & `quri_parts_chem-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-chem"
-version = "0.9.1"
+version = "0.9.2"
 description = "Quantum computer algorithms for chemistry"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/ansatz/all_singles_doubles.py` & `quri_parts_chem-0.9.2/quri_parts/chem/ansatz/all_singles_doubles.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/ansatz/gate_fabric.py` & `quri_parts_chem-0.9.2/quri_parts/chem/ansatz/gate_fabric.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/ansatz/particle_conserving_u1.py` & `quri_parts_chem-0.9.2/quri_parts/chem/ansatz/particle_conserving_u1.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/ansatz/particle_conserving_u2.py` & `quri_parts_chem-0.9.2/quri_parts/chem/ansatz/particle_conserving_u2.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/mol/__init__.py` & `quri_parts_chem-0.9.2/quri_parts/chem/mol/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/mol/active_space.py` & `quri_parts_chem-0.9.2/quri_parts/chem/mol/active_space.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/mol/models.py` & `quri_parts_chem-0.9.2/quri_parts/chem/mol/models.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/transforms/__init__.py` & `quri_parts_chem-0.9.2/quri_parts/chem/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/utils/excitations.py` & `quri_parts_chem-0.9.2/quri_parts/chem/utils/excitations.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/quri_parts/chem/utils/orbital_rotation.py` & `quri_parts_chem-0.9.2/quri_parts/chem/utils/orbital_rotation.py`

 * *Files identical despite different names*

### Comparing `quri_parts_chem-0.9.1/PKG-INFO` & `quri_parts_chem-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-chem
-Version: 0.9.1
+Version: 0.9.2
 Summary: Quantum computer algorithms for chemistry
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

