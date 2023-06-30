# Comparing `tmp/qcparse-0.3.0.tar.gz` & `tmp/qcparse-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcparse-0.3.0.tar", max compression
+gzip compressed data, was "qcparse-0.3.1.tar", max compression
```

## Comparing `qcparse-0.3.0.tar` & `qcparse-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3993 2023-06-28 18:22:01.752831 qcparse-0.3.0/README.md
--rw-r--r--   0        0        0     1181 2023-06-28 18:22:01.752831 qcparse-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      312 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/__init__.py
--rw-r--r--   0        0        0      879 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/cli.py
--rw-r--r--   0        0        0      475 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/exceptions.py
--rw-r--r--   0        0        0     6793 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/main.py
--rw-r--r--   0        0        0     2418 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/models.py
--rw-r--r--   0        0        0       74 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/parsers/__init__.py
--rw-r--r--   0        0        0     8744 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/parsers/terachem.py
--rw-r--r--   0        0        0     2701 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/parsers/utils.py
--rw-r--r--   0        0        0     3995 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/registry.py
--rw-r--r--   0        0        0     1193 2023-06-28 18:22:01.752831 qcparse-0.3.0/qcparse/utils.py
--rw-r--r--   0        0        0     4615 1970-01-01 00:00:00.000000 qcparse-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3993 2023-06-30 02:33:33.881337 qcparse-0.3.1/README.md
+-rw-r--r--   0        0        0     1181 2023-06-30 02:33:33.881337 qcparse-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      312 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/__init__.py
+-rw-r--r--   0        0        0      879 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/cli.py
+-rw-r--r--   0        0        0      475 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/exceptions.py
+-rw-r--r--   0        0        0     6793 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/main.py
+-rw-r--r--   0        0        0     2418 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/models.py
+-rw-r--r--   0        0        0       74 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/parsers/__init__.py
+-rw-r--r--   0        0        0     9189 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/parsers/terachem.py
+-rw-r--r--   0        0        0     2701 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/parsers/utils.py
+-rw-r--r--   0        0        0     3995 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/registry.py
+-rw-r--r--   0        0        0     1193 2023-06-30 02:33:33.881337 qcparse-0.3.1/qcparse/utils.py
+-rw-r--r--   0        0        0     4615 1970-01-01 00:00:00.000000 qcparse-0.3.1/PKG-INFO
```

### Comparing `qcparse-0.3.0/README.md` & `qcparse-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.0/pyproject.toml` & `qcparse-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "qcparse"
-version = "0.3.0"
+version = "0.3.1"
 description = "A package for parsing TeraChem file outputs into structured MolSSI data objects."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pydantic = ">=1.7.4,!=1.8,!=1.8.1,<2.0.0"
-qcio = ">=0.1.0"
+qcio = ">=0.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
 isort = "^5.12.0"
 pytest = "^7.2.2"
 pre-commit = "^3.2.0"
```

### Comparing `qcparse-0.3.0/qcparse/cli.py` & `qcparse-0.3.1/qcparse/cli.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.0/qcparse/main.py` & `qcparse-0.3.1/qcparse/main.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.0/qcparse/models.py` & `qcparse-0.3.1/qcparse/models.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.0/qcparse/parsers/terachem.py` & `qcparse-0.3.1/qcparse/parsers/terachem.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,20 +102,34 @@
     """Parse the basis from TeraChem stdout."""
     regex = r"Using basis set: (\S+)"
     data_collector.input_data.program_args.model.basis = regex_search(
         regex, string
     ).group(1)
 
 
-def parse_version_string(string: str) -> str:
+def parse_git_commit(string: str) -> str:
+    """Parse TeraChem git commit from TeraChem stdout."""
+    regex = r"Git Version: (\S*)"
+    return regex_search(regex, string).group(1)
+
+
+def parse_terachem_version(string: str) -> str:
     """Parse TeraChem version from TeraChem stdout."""
     regex = r"TeraChem (v\S*)"
     return regex_search(regex, string).group(1)
 
 
+def parse_version_string(string: str) -> str:
+    """Parse version string plus git commit from TeraChem stdout.
+
+    Matches format of 'terachem --version' on command line.
+    """
+    return f"{parse_terachem_version(string)} [{parse_git_commit(string)}]"
+
+
 @parser(filetype=FileType.stdout)
 def parse_version(string: str, data_collector: ParsedDataCollector):
     """Parse TeraChem version from TeraChem stdout."""
     data_collector.provenance.program_version = parse_version_string(string)
 
 
 # Factored out for use in calculation_succeeded and parse_failure_text
```

### Comparing `qcparse-0.3.0/qcparse/parsers/utils.py` & `qcparse-0.3.1/qcparse/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.0/qcparse/registry.py` & `qcparse-0.3.1/qcparse/registry.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.0/qcparse/utils.py` & `qcparse-0.3.1/qcparse/utils.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.3.0/PKG-INFO` & `qcparse-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: qcparse
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for parsing TeraChem file outputs into structured MolSSI data objects.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.7.4,!=1.8,!=1.8.1,<2.0.0)
-Requires-Dist: qcio (>=0.1.0)
+Requires-Dist: qcio (>=0.2.0)
 Description-Content-Type: text/markdown
 
 # qcparse
 
 A library for parsing Quantum Chemistry output files into structured data objects. Uses data structures from [qcio](https://github.com/coltonbh/qcio).
 
 [![image](https://img.shields.io/pypi/v/qcparse.svg)](https://pypi.python.org/pypi/qcparse)
```

