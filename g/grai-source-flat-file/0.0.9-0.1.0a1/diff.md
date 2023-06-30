# Comparing `tmp/grai_source_flat_file-0.0.9.tar.gz` & `tmp/grai_source_flat_file-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_flat_file-0.0.9.tar", max compression
+gzip compressed data, was "grai_source_flat_file-0.1.0a1.tar", max compression
```

## Comparing `grai_source_flat_file-0.0.9.tar` & `grai_source_flat_file-0.1.0a1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      165 2023-04-29 00:58:02.883973 grai_source_flat_file-0.0.9/README.md
--rw-r--r--   0        0        0      908 2023-04-30 17:37:11.522290 grai_source_flat_file-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      147 2023-02-13 20:16:22.718033 grai_source_flat_file-0.0.9/src/grai_source_flat_file/__init__.py
--rw-r--r--   0        0        0     4437 2023-04-29 00:19:10.366840 grai_source_flat_file-0.0.9/src/grai_source_flat_file/adapters.py
--rw-r--r--   0        0        0      834 2023-02-13 20:16:22.718432 grai_source_flat_file-0.0.9/src/grai_source_flat_file/base.py
--rw-r--r--   0        0        0     2029 2023-04-17 19:49:39.123184 grai_source_flat_file-0.0.9/src/grai_source_flat_file/loader.py
--rw-r--r--   0        0        0      978 2023-02-13 20:16:22.718610 grai_source_flat_file-0.0.9/src/grai_source_flat_file/models.py
--rw-r--r--   0        0        0      188 2023-02-13 20:16:22.718657 grai_source_flat_file-0.0.9/src/grai_source_flat_file/package_definitions.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.9/setup.py
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-05-19 11:07:12.932554 grai_source_flat_file-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1066 2023-06-30 03:30:27.619158 grai_source_flat_file-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-06-30 03:30:27.624589 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/__init__.py
+-rw-r--r--   0        0        0     6885 2023-06-29 15:34:52.425608 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/adapters.py
+-rw-r--r--   0        0        0      997 2023-06-29 15:34:52.425750 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/base.py
+-rw-r--r--   0        0        0     2843 2023-06-14 21:02:53.377068 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/loader.py
+-rw-r--r--   0        0        0     1094 2023-06-29 15:34:52.426279 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/models.py
+-rw-r--r--   0        0        0      201 2023-06-01 16:01:43.263838 grai_source_flat_file-0.1.0a1/src/grai_source_flat_file/package_definitions.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 grai_source_flat_file-0.1.0a1/PKG-INFO
```

### Comparing `grai_source_flat_file-0.0.9/PKG-INFO` & `grai_source_flat_file-0.1.0a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-source-flat-file
-Version: 0.0.9
+Version: 0.1.0a1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: grai-client (>=0.2.0,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.10,<0.2.0)
+Requires-Dist: grai-client (>=0.3.0a3,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-flat-file
 Description-Content-Type: text/markdown
```

