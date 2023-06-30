# Comparing `tmp/ens_normalize-3.0.2.tar.gz` & `tmp/ens_normalize-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ens_normalize-3.0.2.tar", max compression
+gzip compressed data, was "ens_normalize-3.0.3.tar", max compression
```

## Comparing `ens_normalize-3.0.2.tar` & `ens_normalize-3.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1110 2023-05-20 09:14:31.129166 ens_normalize-3.0.2/LICENSE
--rw-r--r--   0        0        0    17112 2023-05-20 09:14:31.129166 ens_normalize-3.0.2/README.md
--rw-r--r--   0        0        0      571 2023-05-20 09:14:31.129166 ens_normalize-3.0.2/ens_normalize/__init__.py
--rw-r--r--   0        0        0    36598 2023-05-20 09:14:31.129166 ens_normalize-3.0.2/ens_normalize/normalization.py
--rw-r--r--   0        0        0  5153418 2023-05-20 09:14:31.153167 ens_normalize-3.0.2/ens_normalize/spec.pickle
--rw-r--r--   0        0        0      678 2023-05-20 09:14:31.153167 ens_normalize-3.0.2/pyproject.toml
--rw-r--r--   0        0        0    17856 1970-01-01 00:00:00.000000 ens_normalize-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1110 2023-06-30 21:00:57.971680 ens_normalize-3.0.3/LICENSE
+-rw-r--r--   0        0        0    17112 2023-06-30 21:00:57.971680 ens_normalize-3.0.3/README.md
+-rw-r--r--   0        0        0      571 2023-06-30 21:00:57.975680 ens_normalize-3.0.3/ens_normalize/__init__.py
+-rw-r--r--   0        0        0    36598 2023-06-30 21:00:57.975680 ens_normalize-3.0.3/ens_normalize/normalization.py
+-rw-r--r--   0        0        0  5153418 2023-06-30 21:00:57.995680 ens_normalize-3.0.3/ens_normalize/spec.pickle
+-rw-r--r--   0        0        0      678 2023-06-30 21:00:57.995680 ens_normalize-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0    17906 1970-01-01 00:00:00.000000 ens_normalize-3.0.3/PKG-INFO
```

### Comparing `ens_normalize-3.0.2/LICENSE` & `ens_normalize-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ens_normalize-3.0.2/README.md` & `ens_normalize-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ens_normalize-3.0.2/ens_normalize/__init__.py` & `ens_normalize-3.0.3/ens_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `ens_normalize-3.0.2/ens_normalize/normalization.py` & `ens_normalize-3.0.3/ens_normalize/normalization.py`

 * *Files identical despite different names*

### Comparing `ens_normalize-3.0.2/ens_normalize/spec.pickle` & `ens_normalize-3.0.3/ens_normalize/spec.pickle`

 * *Files identical despite different names*

### Comparing `ens_normalize-3.0.2/pyproject.toml` & `ens_normalize-3.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ens-normalize"
-version = "3.0.2"
+version = "3.0.3"
 description = "Ethereum Name Service (ENS) Name Normalizer"
 license = "MIT"
 authors = ["Jakub Karbowski <jakub@namehash.io>"]
 maintainers = ["NameHash Team <devops@namehash.io>"]
 homepage = "https://github.com/namehash/ens-normalize-python"
 repository = "https://github.com/namehash/ens-normalize-python"
 readme = "README.md"
 packages = [{include = "ens_normalize"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 pyunormalize = "^15.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
```

### Comparing `ens_normalize-3.0.2/PKG-INFO` & `ens_normalize-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ens-normalize
-Version: 3.0.2
+Version: 3.0.3
 Summary: Ethereum Name Service (ENS) Name Normalizer
 Home-page: https://github.com/namehash/ens-normalize-python
 License: MIT
 Author: Jakub Karbowski
 Author-email: jakub@namehash.io
 Maintainer: NameHash Team
 Maintainer-email: devops@namehash.io
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyunormalize (>=15.0.0,<16.0.0)
 Project-URL: Repository, https://github.com/namehash/ens-normalize-python
 Description-Content-Type: text/markdown
```

