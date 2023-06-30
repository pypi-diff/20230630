# Comparing `tmp/quri_parts-0.9.1.tar.gz` & `tmp/quri_parts-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts-0.9.1.tar", max compression
+gzip compressed data, was "quri_parts-0.9.2.tar", max compression
```

## Comparing `quri_parts-0.9.1.tar` & `quri_parts-0.9.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11358 2023-03-29 06:13:57.749528 quri_parts-0.9.1/LICENSE
--rw-r--r--   0        0        0     4539 2023-03-29 06:13:57.749528 quri_parts-0.9.1/README.md
--rw-r--r--   0        0        0     3144 2023-03-29 06:13:59.557523 quri_parts-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 06:13:57.833528 quri_parts-0.9.1/quri_parts/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 06:13:57.785528 quri_parts-0.9.1/quri_parts/_quri_parts_meta.py
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 quri_parts-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.850951 quri_parts-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4539 2023-03-29 07:37:19.850951 quri_parts-0.9.2/README.md
+-rw-r--r--   0        0        0     3144 2023-03-29 07:37:21.486956 quri_parts-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-03-29 07:37:19.930951 quri_parts-0.9.2/quri_parts/NOTICE
+-rw-r--r--   0        0        0        0 2023-03-29 07:37:19.882951 quri_parts-0.9.2/quri_parts/_quri_parts_meta.py
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 quri_parts-0.9.2/PKG-INFO
```

### Comparing `quri_parts-0.9.1/LICENSE` & `quri_parts-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts-0.9.1/README.md` & `quri_parts-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `quri_parts-0.9.1/pyproject.toml` & `quri_parts-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts"
-version = "0.9.1"
+version = "0.9.2"
 description = "Platform-independent quantum computing library"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts-0.9.1/PKG-INFO` & `quri_parts-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts
-Version: 0.9.1
+Version: 0.9.2
 Summary: Platform-independent quantum computing library
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<3.12
```

