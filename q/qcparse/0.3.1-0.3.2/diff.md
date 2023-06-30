# Comparing `tmp/qcparse-0.3.1.tar.gz` & `tmp/qcparse-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcparse-0.3.1.tar", max compression
+gzip compressed data, was "qcparse-0.3.2.tar", max compression
```

## Comparing `qcparse-0.3.1.tar` & `qcparse-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3993 2023-06-30 02:33:33.881337 qcparse-0.3.1/README.md
--rw-r--r--   0        0        0     1181 2023-06-30 02:33:33.881337 qcparse-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      312 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/__init__.py
--rw-r--r--   0        0        0      879 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/cli.py
--rw-r--r--   0        0        0      475 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/exceptions.py
--rw-r--r--   0        0        0     6793 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/main.py
--rw-r--r--   0        0        0     2418 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/models.py
--rw-r--r--   0        0        0       74 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/parsers/__init__.py
--rw-r--r--   0        0        0     9189 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/parsers/terachem.py
--rw-r--r--   0        0        0     2701 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/parsers/utils.py
--rw-r--r--   0        0        0     3995 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/registry.py
--rw-r--r--   0        0        0     1193 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/utils.py
--rw-r--r--   0        0        0     4615 1970-01-01 00:00:00.000000 qcparse-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3993 2023-06-30 03:20:35.137518 qcparse-0.3.2/README.md
+-rw-r--r--   0        0        0     1196 2023-06-30 03:20:35.141518 qcparse-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      312 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/__init__.py
+-rw-r--r--   0        0        0      879 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/cli.py
+-rw-r--r--   0        0        0      475 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/exceptions.py
+-rw-r--r--   0        0        0     6793 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/main.py
+-rw-r--r--   0        0        0     2418 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/models.py
+-rw-r--r--   0        0        0       74 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/parsers/__init__.py
+-rw-r--r--   0        0        0     9189 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/parsers/terachem.py
+-rw-r--r--   0        0        0     2701 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/parsers/utils.py
+-rw-r--r--   0        0        0     3995 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/registry.py
+-rw-r--r--   0        0        0     1193 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/utils.py
+-rw-r--r--   0        0        0     4630 1970-01-01 00:00:00.000000 qcparse-0.3.2/PKG-INFO
```

### Comparing `qcparse-0.3.1/README.md` & `qcparse-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.1/pyproject.toml` & `qcparse-0.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "qcparse"
-version = "0.3.1"
-description = "A package for parsing TeraChem file outputs into structured MolSSI data objects."
+version = "0.3.2"
+description = "A package for parsing Quantum Chemistry program file outputs into structured qcio data objects."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pydantic = ">=1.7.4,!=1.8,!=1.8.1,<2.0.0"
```

### Comparing `qcparse-0.3.1/qcparse/cli.py` & `qcparse-0.3.2/qcparse/cli.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.1/qcparse/main.py` & `qcparse-0.3.2/qcparse/main.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.1/qcparse/models.py` & `qcparse-0.3.2/qcparse/models.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.1/qcparse/parsers/terachem.py` & `qcparse-0.3.2/qcparse/parsers/terachem.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.1/qcparse/parsers/utils.py` & `qcparse-0.3.2/qcparse/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.1/qcparse/registry.py` & `qcparse-0.3.2/qcparse/registry.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.1/qcparse/utils.py` & `qcparse-0.3.2/qcparse/utils.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.1/PKG-INFO` & `qcparse-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qcparse
-Version: 0.3.1
-Summary: A package for parsing TeraChem file outputs into structured MolSSI data objects.
+Version: 0.3.2
+Summary: A package for parsing Quantum Chemistry program file outputs into structured qcio data objects.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

