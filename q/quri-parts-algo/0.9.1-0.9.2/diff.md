# Comparing `tmp/quri_parts_algo-0.9.1.tar.gz` & `tmp/quri_parts_algo-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_algo-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts_algo-0.9.2.tar", max compression
```

## Comparing `quri_parts_algo-0.9.1.tar` & `quri_parts_algo-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/LICENSE
--rw-r--r--   0        0        0      276 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/README.md
--rw-r--r--   0        0        0     1229 2023-03-29 06:14:00.665519 quri_parts_algo-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 06:13:59.733522 quri_parts_algo-0.9.1/quri_parts/algo/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/__init__.py
--rw-r--r--   0        0        0     1333 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/ansatz/__init__.py
--rw-r--r--   0        0        0     5711 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/ansatz/hardware_efficient.py
--rw-r--r--   0        0        0     4236 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/ansatz/symmetry_preserving.py
--rw-r--r--   0        0        0     8908 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/ansatz/two_local.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/mitigation/__init__.py
--rw-r--r--   0        0        0     1000 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/mitigation/cdr/__init__.py
--rw-r--r--   0        0        0    11773 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/mitigation/cdr/cdr.py
--rw-r--r--   0        0        0      879 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/mitigation/readout_mitigation/__init__.py
--rw-r--r--   0        0        0     4348 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/mitigation/readout_mitigation/readout_mitigation.py
--rw-r--r--   0        0        0     1234 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/mitigation/zne/__init__.py
--rw-r--r--   0        0        0    12086 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/mitigation/zne/zne.py
--rw-r--r--   0        0        0     1272 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/optimizer/__init__.py
--rw-r--r--   0        0        0     6547 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/optimizer/adam.py
--rw-r--r--   0        0        0     2563 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/optimizer/interface.py
--rw-r--r--   0        0        0    10573 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/optimizer/lbfgs.py
--rw-r--r--   0        0        0     8689 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/optimizer/nft.py
--rw-r--r--   0        0        0     6270 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/optimizer/spsa.py
--rw-r--r--   0        0        0     1495 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/optimizer/tolerance.py
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/py.typed
--rw-r--r--   0        0        0      792 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/utils/__init__.py
--rw-r--r--   0        0        0     6380 2023-03-29 06:13:57.753528 quri_parts_algo-0.9.1/quri_parts/algo/utils/fitting.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 quri_parts_algo-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.850951 quri_parts_algo-0.9.2/LICENSE
+-rw-r--r--   0        0        0      276 2023-03-29 07:37:19.850951 quri_parts_algo-0.9.2/README.md
+-rw-r--r--   0        0        0     1229 2023-03-29 07:37:22.450959 quri_parts_algo-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-03-29 07:37:21.634956 quri_parts_algo-0.9.2/quri_parts/algo/NOTICE
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/__init__.py
+-rw-r--r--   0        0        0     1333 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/ansatz/__init__.py
+-rw-r--r--   0        0        0     5711 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/ansatz/hardware_efficient.py
+-rw-r--r--   0        0        0     4236 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/ansatz/symmetry_preserving.py
+-rw-r--r--   0        0        0     8908 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/ansatz/two_local.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/__init__.py
+-rw-r--r--   0        0        0     1000 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/cdr/__init__.py
+-rw-r--r--   0        0        0    11773 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/cdr/cdr.py
+-rw-r--r--   0        0        0      879 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/readout_mitigation/__init__.py
+-rw-r--r--   0        0        0     4348 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/readout_mitigation/readout_mitigation.py
+-rw-r--r--   0        0        0     1234 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/zne/__init__.py
+-rw-r--r--   0        0        0    12086 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/zne/zne.py
+-rw-r--r--   0        0        0     1272 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/__init__.py
+-rw-r--r--   0        0        0     6547 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/adam.py
+-rw-r--r--   0        0        0     2563 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/interface.py
+-rw-r--r--   0        0        0    10573 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/lbfgs.py
+-rw-r--r--   0        0        0     8689 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/nft.py
+-rw-r--r--   0        0        0     6270 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/spsa.py
+-rw-r--r--   0        0        0     1495 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/tolerance.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/py.typed
+-rw-r--r--   0        0        0      792 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/utils/__init__.py
+-rw-r--r--   0        0        0     6380 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/utils/fitting.py
+-rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 quri_parts_algo-0.9.2/PKG-INFO
```

### Comparing `quri_parts_algo-0.9.1/LICENSE` & `quri_parts_algo-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/pyproject.toml` & `quri_parts_algo-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-algo"
-version = "0.9.1"
+version = "0.9.2"
 description = "Algorithms for quantum computers"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/ansatz/__init__.py` & `quri_parts_algo-0.9.2/quri_parts/algo/ansatz/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/ansatz/hardware_efficient.py` & `quri_parts_algo-0.9.2/quri_parts/algo/ansatz/hardware_efficient.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/ansatz/symmetry_preserving.py` & `quri_parts_algo-0.9.2/quri_parts/algo/ansatz/symmetry_preserving.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/ansatz/two_local.py` & `quri_parts_algo-0.9.2/quri_parts/algo/ansatz/two_local.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/mitigation/cdr/__init__.py` & `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/cdr/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/mitigation/cdr/cdr.py` & `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/cdr/cdr.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/mitigation/readout_mitigation/__init__.py` & `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/readout_mitigation/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/mitigation/readout_mitigation/readout_mitigation.py` & `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/readout_mitigation/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/mitigation/zne/__init__.py` & `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/zne/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/mitigation/zne/zne.py` & `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/zne/zne.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/optimizer/__init__.py` & `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/optimizer/adam.py` & `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/adam.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/optimizer/interface.py` & `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/interface.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/optimizer/lbfgs.py` & `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/lbfgs.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/optimizer/nft.py` & `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/nft.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/optimizer/spsa.py` & `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/spsa.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/optimizer/tolerance.py` & `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/tolerance.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/utils/__init__.py` & `quri_parts_algo-0.9.2/quri_parts/algo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/quri_parts/algo/utils/fitting.py` & `quri_parts_algo-0.9.2/quri_parts/algo/utils/fitting.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.1/PKG-INFO` & `quri_parts_algo-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-algo
-Version: 0.9.1
+Version: 0.9.2
 Summary: Algorithms for quantum computers
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<3.12
```

