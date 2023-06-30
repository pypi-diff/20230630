# Comparing `tmp/cellxgene_census-1.2.1.tar.gz` & `tmp/cellxgene_census-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.2.1.tar", last modified: Sat Jun 17 00:54:46 2023, max compression
+gzip compressed data, was "cellxgene_census-1.3.0.tar", last modified: Fri Jun 30 18:31:12 2023, max compression
```

## Comparing `cellxgene_census-1.2.1.tar` & `cellxgene_census-1.3.0.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.233991 cellxgene_census-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/src/cellxgene_census/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/src/cellxgene_census/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/ml/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_eager_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_online.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25438 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/tests/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/ml/test_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/tests/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/pp/test_hvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/pp/test_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.485628 cellxgene_census-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-30 18:31:12.485628 cellxgene_census-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.477628 cellxgene_census-1.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:31:12.485628 cellxgene_census-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.477628 cellxgene_census-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.481628 cellxgene_census-1.3.0/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.481628 cellxgene_census-1.3.0/src/cellxgene_census/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.481628 cellxgene_census-1.3.0/src/cellxgene_census/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/ml/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.481628 cellxgene_census-1.3.0/src/cellxgene_census/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/pp/_online.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.481628 cellxgene_census-1.3.0/src/cellxgene_census/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/util/_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/src/cellxgene_census/experimental/util/_eager_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.481628 cellxgene_census-1.3.0/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-30 18:31:12.000000 cellxgene_census-1.3.0/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-30 18:31:12.000000 cellxgene_census-1.3.0/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:31:12.000000 cellxgene_census-1.3.0/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-30 18:31:12.000000 cellxgene_census-1.3.0/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 18:31:12.000000 cellxgene_census-1.3.0/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.481628 cellxgene_census-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25438 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.481628 cellxgene_census-1.3.0/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.485628 cellxgene_census-1.3.0/tests/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/experimental/ml/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.485628 cellxgene_census-1.3.0/tests/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/experimental/pp/test_hvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/experimental/pp/test_online.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:31:12.485628 cellxgene_census-1.3.0/tests/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/experimental/util/test_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-30 18:30:58.000000 cellxgene_census-1.3.0/tests/test_util.py
```

### Comparing `cellxgene_census-1.2.1/LICENSE` & `cellxgene_census-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/PKG-INFO` & `cellxgene_census-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.2.1
+Version: 1.3.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: experimental
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/).
```

### Comparing `cellxgene_census-1.2.1/README.md` & `cellxgene_census-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/pyproject.toml` & `cellxgene_census-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,42 +7,41 @@
 dynamic = ["version"]
 description = "API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/"
 authors = [
     { name = "Chan Zuckerberg Initiative", email = "soma@chanzuckerberg.com" }
 ]
 license = { text = "MIT" }
 readme = "README.md"
-requires-python = ">= 3.7, < 3.12"
+requires-python = ">= 3.8, < 3.12"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies= [
     # NOTE: the tiledbsoma version must be >= to the version used in the Census builder, to
     # ensure that the assets are readable (tiledbsoma supports backward compatible reading).
     # Make sure this version does not fall behind the builder's tiledbsoma version.
-    "tiledbsoma==1.2.5",
+    "tiledbsoma==1.2.7",
     "anndata",
     "numpy>=1.21,<1.25",  # numpy is constrained by numba and the old pip solver
     "requests",
     "typing_extensions",
-    "s3fs",
-    "scipy",
+    "s3fs>=2021.06.1",
+    "scipy<1.11",  # work around incompatibility between scipy and pyarrow
     # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
     "certifi",
 ]
 
 [project.optional-dependencies]
 experimental = [
     "torch==2.0.1",
```

### Comparing `cellxgene_census-1.2.1/release_process.md` & `cellxgene_census-1.3.0/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/__init__.py` & `cellxgene_census-1.3.0/src/cellxgene_census/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,19 +16,15 @@
 .. _cellxgene_census repo:
     https://github.com/chanzuckerberg/cellxgene-census/
 
 .. _tiledbsoma repo:
     https://github.com/single-cell-data/TileDB-SOMA
 """
 
-try:
-    from importlib import metadata
-except ImportError:
-    # for python <=3.7
-    import importlib_metadata as metadata  # type: ignore[no-redef]
+from importlib import metadata
 
 from ._get_anndata import get_anndata
 from ._open import download_source_h5ad, get_source_h5ad_uri, open_soma
 from ._presence_matrix import get_presence_matrix
 from ._release_directory import get_census_version_description, get_census_version_directory
 
 try:
```

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.3.0/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.3.0/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/_open.py` & `cellxgene_census-1.3.0/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.3.0/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.3.0/src/cellxgene_census/_release_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/experimental/ml/pytorch.py` & `cellxgene_census-1.3.0/src/cellxgene_census/experimental/ml/pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 import logging
 import os
 import sys
+from contextlib import contextmanager
 from datetime import timedelta
 from time import time
-from typing import Any, Dict, Iterator, List, Optional, Sequence, Tuple
+from typing import Any, Dict, Iterator, Optional, Sequence, Tuple
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import pyarrow as pa
 import scipy
 import somacore
 import tiledbsoma as soma
 import torch
 import torchdata.datapipes.iter as pipes
-from attr import attrs
+from attr import define
 from scipy import sparse
 from sklearn.preprocessing import LabelEncoder
 from somacore.query import _fast_csr
 from torch import Tensor
 from torch.utils.data import DataLoader
 from torch.utils.data.dataset import Dataset
 
 import cellxgene_census
-from cellxgene_census._open import _build_soma_tiledb_context
 
-ObsDatum = Tuple[Tensor, Tensor]
+from ..._open import _build_soma_tiledb_context
+from ..util import EagerIterator
+
+ObsAndXDatum = Tuple[Tensor, Tensor]
+
+
+@define
+class ObsAndXSOMABatch:
+    obs: pd.DataFrame
+    X: scipy.matrix
+    stats: "Stats"
+
+    def __len__(self) -> int:
+        return len(self.obs)
+
 
 Encoders = Dict[str, LabelEncoder]
 
 pytorch_logger = logging.getLogger("cellxgene_census.experimental.pytorch")
-pytorch_logger.setLevel(logging.INFO)
 
 
-@attrs
+@define
 class Stats:
     """
     Statistics about the data retrieved by ``ExperimentDataPipe`` via SOMA API.
 
     Lifecycle:
         experimental
     """
@@ -56,212 +69,237 @@
 
     def __str__(self) -> str:
         return (
             f"n_soma_batches={self.n_soma_batches}, n_obs={self.n_obs}, nnz={self.nnz}, "
             f"elapsed={timedelta(seconds=self.elapsed)}"
         )
 
+    def __add__(self, other: "Stats") -> "Stats":
+        self.n_obs += other.n_obs
+        self.nnz += other.nnz
+        self.elapsed += other.elapsed
+        self.n_soma_batches += other.n_soma_batches
+        return self
+
 
+@contextmanager
 def _open_experiment(
     uri: str, aws_region: Optional[str] = None, soma_buffer_bytes: Optional[int] = None
 ) -> soma.Experiment:
     context = _build_soma_tiledb_context(aws_region)
 
     if soma_buffer_bytes is not None:
         context = context.replace(
             tiledb_config={
                 "py.init_buffer_bytes": soma_buffer_bytes,
                 "soma.init_buffer_bytes": soma_buffer_bytes,
             }
         )
 
-    return soma.Experiment.open(uri, context=context)
+    with soma.Experiment.open(uri, context=context) as exp:
+        yield exp
+
+
+class _ObsAndXSOMAIterator(Iterator[ObsAndXSOMABatch]):
+    obs_tables_iter: somacore.ReadIter[pa.Table]
+    """Iterates the SOMA batches (tables) of obs data"""
+
+    X: soma.SparseNDArray
+    """All X data"""
+
+    var_joinids: pa.Array
+
+    def __init__(self, X: soma.SparseNDArray, obs_tables_iter: somacore.ReadIter[pa.Table], var_joinids: pa.Array):
+        self.obs_tables_iter = obs_tables_iter
+        self.X = X
+        self.var_joinids = var_joinids
+
+    def __next__(self) -> ObsAndXSOMABatch:
+        pytorch_logger.debug("Retrieving next SOMA batch...")
+        start_time = time()
+
+        # If no more batches to iterate through, raise StopIteration, as all iterators do when at end
+        obs_table = next(self.obs_tables_iter)
+        obs_batch = obs_table.to_pandas()
+
+        # handle case of empty result (first batch has 0 rows)
+        if len(obs_batch) == 0:
+            raise StopIteration
+
+        X_batch = _fast_csr.read_scipy_csr(self.X, obs_table["soma_joinid"].combine_chunks(), self.var_joinids)
+        assert obs_batch.shape[0] == X_batch.shape[0]
+
+        stats = Stats()
+        stats.n_obs += X_batch.shape[0]
+        stats.nnz += X_batch.nnz
+        stats.elapsed += int(time() - start_time)
+        stats.n_soma_batches += 1
+
+        pytorch_logger.debug(f"Retrieved SOMA batch: {stats}")
+        return ObsAndXSOMABatch(obs=obs_batch, X=X_batch, stats=stats)
 
 
-class _ObsAndXIterator(Iterator[ObsDatum]):
+class _ObsAndXIterator(Iterator[ObsAndXDatum]):
     """
     Iterates through a set of obs and related X rows, specified as ``soma_joinid``s. Encapsulates the batch-based data
     fetching from SOMA objects, providing row-based iteration.
     """
 
-    obs_tables_iter: somacore.ReadIter[pa.Table]
-    """Iterates the SOMA batches (tables) of obs data"""
-
-    obs_batch_: pd.DataFrame = pd.DataFrame()
-    """The current SOMA batch of obs data"""
+    soma_batch_iter: Iterator[ObsAndXSOMABatch]
+    """The iterator for SOMA batches of paired obs and X data"""
 
-    X_batch: scipy.matrix = None
-    """All X data for the ``soma_joinid``s of the current obs - batch"""
+    soma_batch: Optional[ObsAndXSOMABatch]
+    """The current SOMA batch of obs and X data"""
 
     i: int = -1
     """Index into current obs ``SOMA`` batch"""
 
     def __init__(
         self,
-        obs_joinids: List[int],
-        var_joinids: pa.Array,
-        exp_uri: str,
-        aws_region: Optional[str],
-        measurement_name: str,
-        X_layer_name: str,
+        X: soma.SparseNDArray,
+        obs_tables_iter: somacore.ReadIter[pa.Table],
+        var_joinids: npt.NDArray[np.int64],
         batch_size: int,
         encoders: Dict[str, LabelEncoder],
         stats: Stats,
-        obs_column_names: Sequence[str],
         sparse_X: bool,
-        soma_buffer_bytes: Optional[int] = None,
+        use_eager_fetch: bool,
     ) -> None:
+        self.soma_batch_iter = _ObsAndXSOMAIterator(X, obs_tables_iter, pa.array(var_joinids))
+        if use_eager_fetch:
+            self.soma_batch_iter = EagerIterator(self.soma_batch_iter)
+        self.soma_batch = None
         self.var_joinids = var_joinids
         self.batch_size = batch_size
         self.sparse_X = sparse_X
-
-        # holding reference to SOMA object prevents it from being closed
-        self.exp = _open_experiment(exp_uri, aws_region, soma_buffer_bytes=soma_buffer_bytes)
-        self.X: soma.SparseNDArray = self.exp.ms[measurement_name].X[X_layer_name]
-        self.obs_tables_iter = self.exp.obs.read(
-            coords=(obs_joinids,), batch_size=somacore.BatchSize(), column_names=obs_column_names
-        )
         self.encoders = encoders
         self.stats = stats
 
-    def __next__(self) -> ObsDatum:
-        # read the next torch batch, possibly across multiple soma batches
+    def __next__(self) -> ObsAndXDatum:
+        """Read the next torch batch, possibly across multiple soma batches"""
+
         obs: pd.DataFrame = pd.DataFrame()
         X: sparse.csr_matrix = sparse.csr_matrix((0, len(self.var_joinids)))
 
         while len(obs) < self.batch_size:
             try:
-                obs_partial, X_partial = self._read_partial_torch_batch(self.batch_size)
-                if X is None:
-                    obs = obs_partial
-                    X = X_partial
-                else:
-                    obs = pd.concat([obs, obs_partial], axis=0)
-                    X = sparse.vstack([X, X_partial])
-
+                obs_partial, X_partial = self._read_partial_torch_batch(self.batch_size - len(obs))
+                obs = pd.concat([obs, obs_partial], axis=0)
+                X = sparse.vstack([X, X_partial])
             except StopIteration:
                 break
 
         if len(obs) == 0:
             raise StopIteration
 
         obs_encoded = pd.DataFrame(
-            data={"soma_joinid": obs.soma_joinid}, columns=obs.columns, dtype=np.int32, index=obs.index
+            data={"soma_joinid": obs.soma_joinid}, columns=obs.columns, dtype=np.int64, index=obs.index
         )
+        # TODO: Encode the entire SOMA batch at once in _read_partial_torch_batch()
         for col, enc in self.encoders.items():
             obs_encoded[col] = enc.transform(obs[col])
 
-        obs_tensor = torch.Tensor(obs_encoded.to_numpy()).int()
+        # `to_numpy()` avoids copying the numpy array data
+        obs_tensor = torch.from_numpy(obs_encoded.to_numpy())
+
         if not self.sparse_X:
-            X_tensor = torch.Tensor(X.todense())
+            X_tensor = torch.from_numpy(X.todense())
         else:
             coo = X.tocoo()
 
             X_tensor = torch.sparse_coo_tensor(
                 # Note: The `np.array` seems unnecessary, but PyTorch warns bare array is "extremely slow"
-                indices=torch.Tensor(np.array([coo.row, coo.col])),
+                indices=torch.from_numpy(np.array([coo.row, coo.col])),
                 values=coo.data,
                 size=coo.shape,
             )
 
         if self.batch_size == 1:
             X_tensor = X_tensor[0]
             obs_tensor = obs_tensor[0]
 
         return X_tensor, obs_tensor
 
-    def _read_partial_torch_batch(self, batch_size: int) -> Tuple[pd.DataFrame, sparse.csr_matrix]:
-        safe_batch_size = min(batch_size, len(self.obs_batch) - self.i)
+    def _read_partial_torch_batch(self, batch_size: int) -> ObsAndXDatum:
+        if self.soma_batch is None or not (0 <= self.i < len(self.soma_batch)):
+            self.soma_batch: ObsAndXSOMABatch = next(self.soma_batch_iter)
+            self.stats += self.soma_batch.stats
+            self.i = 0
+
+            pytorch_logger.debug(f"Retrieved SOMA batch totals: {self.stats}")
+
+        obs_batch = self.soma_batch.obs
+        X_batch = self.soma_batch.X
+
+        safe_batch_size = min(batch_size, len(obs_batch) - self.i)
         slice_ = slice(self.i, self.i + safe_batch_size)
-        obs_rows = self.obs_batch.iloc[slice_]
-        X_csr_scipy = self.X_batch[slice_]
-        self.i += safe_batch_size
-        return obs_rows, X_csr_scipy
+        assert slice_.stop <= obs_batch.shape[0]
 
-    @property
-    # TODO: Retrieve next batch asynchronously, so it's available before the current batch's iteration ends
-    def obs_batch(self) -> pd.DataFrame:
-        """
-        Returns the current SOMA batch of obs rows.
-        If the current SOMA batch has been fully iterated, loads the next SOMA batch of both obs and X data and returns
-        the new obs batch (only).
-        Raises ``StopIteration`` if there are no more SOMA batches to retrieve.
-        """
-        if 0 <= self.i < len(self.obs_batch_):
-            return self.obs_batch_
+        obs_rows = obs_batch.iloc[slice_]
+        assert obs_rows["soma_joinid"].is_unique
+        X_csr_scipy = X_batch[slice_]
+        assert safe_batch_size == obs_rows.shape[0]
+        assert obs_rows.shape[0] == X_csr_scipy.shape[0]
 
-        pytorch_logger.debug("Retrieving next TileDB-SOMA batch...")
-        start_time = time()
-        # If no more batch to iterate through, raise StopIteration, as all iterators do when at end
-        obs_table = next(self.obs_tables_iter)
-        self.obs_batch_ = obs_table.to_pandas()
-        # handle case of empty result (first batch has 0 rows)
-        if len(self.obs_batch_) == 0:
-            raise StopIteration
-        self.X_batch = _fast_csr.read_scipy_csr(self.X, obs_table["soma_joinid"].combine_chunks(), self.var_joinids)
-        self.i = 0
-        self.stats.n_obs += self.X_batch.shape[0]
-        self.stats.nnz += self.X_batch.nnz
-        self.stats.elapsed += int(time() - start_time)
-        self.stats.n_soma_batches += 1
-        # TODO: also show per-batch stats (non-cumulative)
-        pytorch_logger.debug(f"Retrieved batch: shape={self.X_batch.shape}, cum_stats: {self.stats}")
-        return self.obs_batch_
+        self.i += safe_batch_size
 
+        return obs_rows, X_csr_scipy
 
-class ExperimentDataPipe(pipes.IterDataPipe[Dataset[ObsDatum]]):  # type: ignore
+
+class ExperimentDataPipe(pipes.IterDataPipe[Dataset[ObsAndXDatum]]):  # type: ignore
     """
     An iterable-style PyTorch ``DataPipe`` that reads obs and X data from a SOMA Experiment, and returns an iterator of
     tuples of PyTorch ``Tensor`` objects.
 
     >>> (tensor([0., 0., 0., 0., 0., 1., 0., 0., 0.]),  # X data
-        tensor([2415,    0,    0], dtype=torch.int32)) # obs data, encoded
+        tensor([2415,    0,    0], dtype=torch.int64)) # obs data, encoded
 
     Supports batching via `batch_size` param:
 
     >>> DataLoader(..., batch_size=3, ...):
         (tensor([[0., 0., 0., 0., 0., 1., 0., 0., 0.],     # X batch
                  [0., 0., 0., 0., 0., 0., 0., 0., 0.],
                  [0., 0., 0., 0., 0., 0., 0., 0., 0.]]),
          tensor([[2415,    0,    0],                       # obs batch
                  [2416,    0,    4],
-                 [2417,    0,    3]], dtype=torch.int32))
+                 [2417,    0,    3]], dtype=torch.int64))
 
     Obs attribute values are encoded as categoricals. Values can be decoded by obtaining the encoder for a given
     attribute:
 
     >>> exp_data_pipe.obs_encoders()["<obs_attr_name>"].inverse_transform(encoded_values)
 
     Lifecycle:
         experimental
     """
 
-    _query: Optional[soma.ExperimentAxisQuery]
-    """In multi-processing mode (i.e. num_workers > 0), this ``ExperimentAxisQuery`` object will *not* be pickled; 
-    each worker will instantiate a new query"""
+    _initialized: bool
+
+    _obs_joinids: Optional[npt.NDArray[np.int64]]
 
-    _obs_joinids_partitioned: Optional[npt.NDArray[np.int64]] = None
+    _var_joinids: Optional[npt.NDArray[np.int64]]
 
     _encoders: Optional[Encoders]
 
     _stats: Stats
 
     # TODO: Consider adding another convenience method wrapper to construct this object whose signature is more closely
     #  aligned with get_anndata() params (i.e. "exploded" AxisQuery params).
     def __init__(
         self,
         experiment: soma.Experiment,
-        measurement_name: str,
-        X_name: str,
+        measurement_name: str = "raw",
+        X_name: str = "X",
         obs_query: Optional[soma.AxisQuery] = None,
         var_query: Optional[soma.AxisQuery] = None,
         obs_column_names: Sequence[str] = (),
         batch_size: int = 1,
         sparse_X: bool = False,
         soma_buffer_bytes: Optional[int] = None,
+        use_eager_fetch: bool = True,
     ) -> None:
         """
         Construct a new ``ExperimentDataPipe``.
 
         Returns:
             ``ExperimentDataPipe``.
 
@@ -277,146 +315,141 @@
         self.var_query = var_query
         self.obs_column_names = obs_column_names
         self.batch_size = batch_size
         self.sparse_X = sparse_X
         # TODO: This will control the SOMA batch sizes, and could be replaced with a row count once TileDB-SOMA
         #  supports `batch_size` param. It affects both the obs and X read operations.
         self.soma_buffer_bytes = soma_buffer_bytes
-        self._query = None
+        self.use_eager_fetch = use_eager_fetch
         self._stats = Stats()
         self._encoders = None
+        self._obs_joinids = None
+        self._var_joinids = None
+        self._initialized = False
 
         if "soma_joinid" not in self.obs_column_names:
             self.obs_column_names = ["soma_joinid", *self.obs_column_names]
 
     def _init(self) -> None:
-        if self._query is not None:
+        if self._initialized:
             return
 
-        # TODO: support multiple layers, per somacore.query.query.ExperimentAxisQuery.to_anndata()
-        # TODO: handle closing of `_query` (and transitively, `exp`) when iterator is no longer in use; may need be used as a ContextManager,
-        #  but not clear how we can do that when used by DataLoader
-        exp = _open_experiment(self.exp_uri, self.aws_region, soma_buffer_bytes=self.soma_buffer_bytes)
-
-        self._query = exp.axis_query(
-            measurement_name=self.measurement_name,
-            obs_query=self.obs_query,
-            var_query=self.var_query,
-        )
+        pytorch_logger.debug("Initializing ExperimentDataPipe")
+
+        with _open_experiment(self.exp_uri, self.aws_region, soma_buffer_bytes=self.soma_buffer_bytes) as exp:
+            query = exp.axis_query(
+                measurement_name=self.measurement_name,
+                obs_query=self.obs_query,
+                var_query=self.var_query,
+            )
+
+            # The to_numpy() call is a workaround for a possible bug in TileDB-SOMA:
+            # https://github.com/single-cell-data/TileDB-SOMA/issues/1456
+            self._obs_joinids = query.obs_joinids().to_numpy()
+            self._var_joinids = query.var_joinids().to_numpy()
+
+            self._encoders = self._build_obs_encoders(query)
 
-        obs_joinids = self._query.obs_joinids()
+        self._initialized = True
 
+    @staticmethod
+    def _partition_obs_joinids(ids: npt.NDArray[np.int64]) -> npt.NDArray[np.int64]:
+        # NOTE: Can alternately use a `worker_init_fn` to split among workers split workload
         worker_info = torch.utils.data.get_worker_info()
-        if worker_info:
-            # multi-processing mode
 
-            if worker_info.num_workers > 0 and self.sparse_X:
-                raise NotImplementedError(
-                    "torch does not work with sparse tensors in multi-processing mode "
-                    "(see https://github.com/pytorch/pytorch/issues/20248)"
-                )
+        if worker_info is None or worker_info.num_workers < 2:
+            return ids
 
-            partition, num_partitions = worker_info.id, worker_info.num_workers
+        partition, num_partitions = worker_info.id, worker_info.num_workers
 
-        else:
-            partition, num_partitions = 0, 1
+        partitions = np.array_split(ids, num_partitions)
+        ids = partitions[partition]
 
-        if num_partitions is not None:
-            # partitioned data loading
-            # NOTE: Can alternately use a `worker_init_fn` to split among workers split workload
-            partition_size = len(obs_joinids) // num_partitions
-            partition_start = partition_size * partition
-            partition_end_excl = min(len(obs_joinids), partition_start + partition_size)
-            # The to_numpy() call is a workaround for a possible bug in TileDB-SOMA:
-            # https://github.com/single-cell-data/TileDB-SOMA/issues/1456
-            self._obs_joinids_partitioned = obs_joinids[partition_start:partition_end_excl].to_numpy()
+        if pytorch_logger.isEnabledFor(logging.DEBUG) and len(ids) > 0:
+            joinids_start = ids[0]
+            joinids_end = ids[-1]
+            lens = [len(p) for p in partitions]
+            partition_start = sum(lens[:partition])
+            partition_end_excl = partition_start + lens[partition]
+
+            pytorch_logger.debug(
+                f"Process {os.getpid()} handling partition {partition + 1} of {num_partitions}, "
+                f"index range=[{partition_start}:{partition_end_excl}), "
+                f"soma_joinid range=[{joinids_start}:{joinids_end}], "
+                f"partition_size={len(ids)}"
+            )
 
-            if pytorch_logger.isEnabledFor(logging.DEBUG):
-                if self._obs_joinids_partitioned is not None and len(self._obs_joinids_partitioned) > 0:
-                    joinids_start = self._obs_joinids_partitioned[0]
-                    joinids_end = self._obs_joinids_partitioned[-1]
-                else:
-                    joinids_start = joinids_end = 0
-
-                pytorch_logger.debug(
-                    f"Process {os.getpid()} handling partition {partition + 1} of {num_partitions}, "
-                    f"index range={partition_start}:{partition_end_excl}, "
-                    f"soma_joinid range={joinids_start}:{joinids_end}, "
-                    f"{partition_size:}"
-                )
+        return ids
 
-    def __iter__(self) -> Iterator[ObsDatum]:
-        # TODO: avoid re-initializing query if in multi-processing mode, when _obs_joinids_partitioned is set. will need to cache var_joinids for serialization
+    def __iter__(self) -> Iterator[ObsAndXDatum]:
         self._init()
-        assert self._query is not None
+        assert self._obs_joinids is not None
+        assert self._var_joinids is not None
 
-        obs_joinids = (
-            self._obs_joinids_partitioned if self._obs_joinids_partitioned is not None else self._query.obs_joinids()
-        )
+        if self.sparse_X and torch.utils.data.get_worker_info() and torch.utils.data.get_worker_info().num_workers > 0:
+            raise NotImplementedError(
+                "torch does not work with sparse tensors in multi-processing mode "
+                "(see https://github.com/pytorch/pytorch/issues/20248)"
+            )
 
-        return _ObsAndXIterator(
-            obs_joinids=obs_joinids,
-            var_joinids=self._query.var_joinids(),
-            exp_uri=self.exp_uri,
-            aws_region=self.aws_region,
-            measurement_name=self.measurement_name,
-            X_layer_name=self.layer_name,
-            batch_size=self.batch_size,
-            encoders=self.obs_encoders(),
-            stats=self._stats,
-            obs_column_names=self.obs_column_names,
-            sparse_X=self.sparse_X,
-            soma_buffer_bytes=self.soma_buffer_bytes,
-        )
+        with _open_experiment(self.exp_uri, self.aws_region, soma_buffer_bytes=self.soma_buffer_bytes) as exp:
+            X: soma.SparseNDArray = exp.ms[self.measurement_name].X[self.layer_name]
+
+            obs_tables_iter = exp.obs.read(
+                coords=(self._partition_obs_joinids(self._obs_joinids),),
+                batch_size=somacore.BatchSize(),
+                column_names=self.obs_column_names,
+            )
+
+            obs_and_x_iter = _ObsAndXIterator(
+                X,
+                obs_tables_iter,
+                var_joinids=self._var_joinids,
+                batch_size=self.batch_size,
+                encoders=self.obs_encoders,
+                stats=self._stats,
+                sparse_X=self.sparse_X,
+                use_eager_fetch=self.use_eager_fetch,
+            )
+
+            for datum_ in obs_and_x_iter:
+                yield datum_
 
     def __len__(self) -> int:
         self._init()
-        assert self._query is not None
+        assert self._obs_joinids is not None
 
-        return int(self._query.n_obs)
+        return len(self._obs_joinids)
 
-    def __getitem__(self, index: int) -> ObsDatum:
+    def __getitem__(self, index: int) -> ObsAndXDatum:
         raise NotImplementedError("IterDataPipe can only be iterated")
 
-    def __getstate__(self) -> Dict[str, Any]:
-        state = self.__dict__.copy()
-        # Don't pickle `_query`
-        del state["_query"]
-        return state
-
-    def __setstate__(self, state: Dict[str, Any]) -> None:
-        self.__dict__.update(state)
-        self._query = None
-
-    def obs_encoders(self) -> Encoders:
+    def _build_obs_encoders(self, query: soma.ExperimentAxisQuery) -> Encoders:
         """
         Returns the encoders that were used to encode obs column values and that are needed to decode them.
 
         Returns:
             ``Dict[str, LabelEncoder]`` mapping column names to ``LabelEncoder``s.
 
         Lifecycle:
             experimental
         """
-        if self._encoders is not None:
-            return self._encoders
-
-        self._init()
-        assert self._query is not None
+        pytorch_logger.debug("Initializing encoders")
 
-        obs = self._query.obs(column_names=self.obs_column_names).concat()
-        self._encoders = {}
+        obs = query.obs(column_names=self.obs_column_names).concat()
+        encoders = {}
         for col in self.obs_column_names:
             if obs[col].type in (pa.string(), pa.large_string()):
                 enc = LabelEncoder()
                 enc.fit(obs[col].combine_chunks().unique())
-                self._encoders[col] = enc
+                encoders[col] = enc
 
-        return self._encoders
+        return encoders
 
+    # TODO: This does not work in multiprocessing mode, as child process's stats are not collected
     def stats(self) -> Stats:
         """
         Get data loading stats for this ``ExperimentDataPipe``.
 
         Args: None.
 
         Returns:
@@ -438,17 +471,25 @@
         Returns:
             2-tuple of ``int``s, for obs and var counts, respectively.
 
         Lifecycle:
             experimental
         """
         self._init()
-        assert self._query is not None
+        assert self._obs_joinids is not None
+        assert self._var_joinids is not None
+
+        return len(self._obs_joinids), len(self._var_joinids)
+
+    @property
+    def obs_encoders(self) -> Encoders:
+        self._init()
+        assert self._encoders is not None
 
-        return self._query.n_obs, self._query.n_vars
+        return self._encoders
 
 
 # Note: must be a top-level function (and not a lambda), to play nice with multiprocessing pickling
 def _collate_noop(x: Any) -> Any:
     return x
```

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_eager_iter.py` & `cellxgene_census-1.3.0/src/cellxgene_census/experimental/util/_eager_iter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,48 @@
+import logging
 import threading
 from collections import deque
 from concurrent import futures
+from concurrent.futures import Future
 from typing import Deque, Iterator, Optional, TypeVar
 
+util_logger = logging.getLogger("cellxgene_census.experimental.util")
+
 _T = TypeVar("_T")
 
 
 class EagerIterator(Iterator[_T]):
     def __init__(
         self,
         iterator: Iterator[_T],
         pool: Optional[futures.Executor] = None,
     ):
         super().__init__()
         self.iterator = iterator
         self._pool = pool or futures.ThreadPoolExecutor()
         self._own_pool = pool is None
+        self._future: Optional[Future[_T]] = None
+        self.fetch_next()
+
+    def fetch_next(self) -> None:
         self._future = self._pool.submit(self.iterator.__next__)
+        util_logger.debug("Fetching next iterator element, eagerly")
 
     def __next__(self) -> _T:
         try:
+            assert self._future
             res = self._future.result()
-            self._future = self._pool.submit(self.iterator.__next__)
+            self.fetch_next()
             return res
         except StopIteration:
             self._cleanup()
             raise
 
     def _cleanup(self) -> None:
+        util_logger.debug("Cleaning up eager iterator")
         if self._own_pool:
             self._pool.shutdown()
 
     def __del__(self) -> None:
         # Ensure the threadpool is cleaned up in the case where the
         # iterator is not exhausted. For more information on __del__:
         # https://docs.python.org/3/reference/datamodel.html#object.__del__
@@ -64,26 +75,29 @@
             return res
         except StopIteration:
             self._cleanup()
             raise
 
     def _begin_next(self) -> None:
         def _fut_done(fut: futures.Future[_T]) -> None:
+            util_logger.debug("Finished fetching next iterator element, eagerly")
             if fut.exception() is None:
                 self._begin_next()
 
         with self._lock:
             not_running = len(self._pending_results) == 0 or self._pending_results[-1].done()
             if len(self._pending_results) < self.max_pending and not_running:
                 _future = self._pool.submit(self.iterator.__next__)
+                util_logger.debug("Fetching next iterator element, eagerly")
                 _future.add_done_callback(_fut_done)
                 self._pending_results.append(_future)
             assert len(self._pending_results) <= self.max_pending
 
     def _cleanup(self) -> None:
+        util_logger.debug("Cleaning up eager iterator")
         if self._own_pool:
             self._pool.shutdown()
 
     def __del__(self) -> None:
         # Ensure the threadpool is cleaned up in the case where the
         # iterator is not exhausted. For more information on __del__:
         # https://docs.python.org/3/reference/datamodel.html#object.__del__
```

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py` & `cellxgene_census-1.3.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import pandas as pd
 import tiledbsoma as soma
 from somacore.options import SparseDFCoord
 from typing_extensions import Literal
 
 from ..._experiment import _get_experiment
-from ._eager_iter import EagerIterator
+from ..util import EagerIterator
 from ._online import CountsAccumulator, MeanVarianceAccumulator
 
 """
 Acknowledgements: ScanPy highly variable genes implementation (scanpy.pp.highly_variable_genes), in turn
 based upon the original implementation in Seurat V3.
 
 Ref:
```

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_online.py` & `cellxgene_census-1.3.0/src/cellxgene_census/experimental/pp/_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.3.0/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.2.1
+Version: 1.3.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: experimental
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/).
```

### Comparing `cellxgene_census-1.2.1/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.3.0/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,27 @@
 src/cellxgene_census.egg-info/dependency_links.txt
 src/cellxgene_census.egg-info/requires.txt
 src/cellxgene_census.egg-info/top_level.txt
 src/cellxgene_census/experimental/__init__.py
 src/cellxgene_census/experimental/ml/__init__.py
 src/cellxgene_census/experimental/ml/pytorch.py
 src/cellxgene_census/experimental/pp/__init__.py
-src/cellxgene_census/experimental/pp/_eager_iter.py
 src/cellxgene_census/experimental/pp/_highly_variable_genes.py
 src/cellxgene_census/experimental/pp/_online.py
+src/cellxgene_census/experimental/util/__init__.py
+src/cellxgene_census/experimental/util/_csr_iter.py
+src/cellxgene_census/experimental/util/_eager_iter.py
 tests/README.md
 tests/__init__.py
 tests/conftest.py
 tests/test_acceptance.py
 tests/test_directory.py
 tests/test_get_anndata.py
 tests/test_get_helpers.py
 tests/test_open.py
 tests/test_util.py
 tests/experimental/__init__.py
 tests/experimental/ml/__init__.py
 tests/experimental/ml/test_pytorch.py
 tests/experimental/pp/test_hvg.py
-tests/experimental/pp/test_online.py
+tests/experimental/pp/test_online.py
+tests/experimental/util/test_csr_iter.py
```

### Comparing `cellxgene_census-1.2.1/tests/README.md` & `cellxgene_census-1.3.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/tests/conftest.py` & `cellxgene_census-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/tests/experimental/ml/test_pytorch.py` & `cellxgene_census-1.3.0/tests/experimental/ml/test_pytorch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import pathlib
 import sys
-from typing import Callable, List, Optional, Sequence, Tuple
+from typing import Callable, List, Optional, Sequence, Union
+from unittest.mock import patch
 
 import numpy as np
+import pandas as pd
 import pyarrow as pa
 import pytest
 import tiledbsoma as soma
 from scipy import sparse
 from scipy.sparse import coo_matrix, spmatrix
 from somacore import AxisQuery
 from tiledbsoma import Experiment, _factory
 from tiledbsoma._collection import CollectionBase
 
 # conditionally import torch, as it will not be available in all test environments
 try:
     from torch import Tensor
 
-    from cellxgene_census.experimental.ml.pytorch import ExperimentDataPipe, experiment_dataloader
+    from cellxgene_census.experimental.ml.pytorch import (
+        ExperimentDataPipe,
+        ObsAndXSOMABatch,
+        Stats,
+        experiment_dataloader,
+    )
 except ImportError:
     # this should only occur when not running `experimental`-marked tests
     pass
 
 
-def pytorch_x_value_gen(shape: Tuple[int, int]) -> spmatrix:
-    checkerboard_of_ones = coo_matrix(np.indices(shape).sum(axis=0) % 2)
+def pytorch_x_value_gen(obs_range: range, var_range: range) -> spmatrix:
+    occupied_shape = (obs_range.stop - obs_range.start, var_range.stop - var_range.start)
+    checkerboard_of_ones = coo_matrix(np.indices(occupied_shape).sum(axis=0) % 2)
+    checkerboard_of_ones.row += obs_range.start
+    checkerboard_of_ones.col += var_range.start
     return checkerboard_of_ones
 
 
 @pytest.fixture
 def X_layer_names() -> List[str]:
     return ["raw"]
 
@@ -38,106 +48,98 @@
 
 
 @pytest.fixture
 def varp_layer_names() -> Optional[List[str]]:
     return None
 
 
-@pytest.fixture
-def X_value_gen() -> Callable[[Tuple[int, int]], sparse.spmatrix]:
-    def _x_value_gen(shape: Tuple[int, int]) -> sparse.coo_matrix:
-        return sparse.random(
-            shape[0],
-            shape[1],
-            density=0.1,
-            format="coo",
-            dtype=np.float32,
-            random_state=np.random.default_rng(),
-        )
-
-    return _x_value_gen
-
-
-def add_dataframe(coll: CollectionBase, key: str, sz: int) -> None:
+def add_dataframe(coll: CollectionBase, key: str, value_range: range) -> None:
     df = coll.add_new_dataframe(
         key,
         schema=pa.schema(
             [
                 ("soma_joinid", pa.int64()),
                 ("label", pa.large_string()),
             ]
         ),
         index_column_names=["soma_joinid"],
     )
     df.write(
         pa.Table.from_pydict(
             {
-                "soma_joinid": [i for i in range(sz)],
-                "label": [str(i) for i in range(sz)],
+                "soma_joinid": list(value_range),
+                "label": [str(i) for i in value_range],
             }
         )
     )
 
 
 def add_sparse_array(
-    coll: CollectionBase, key: str, shape: Tuple[int, int], value_gen: Callable[[Tuple[int, int]], sparse.spmatrix]
+    coll: CollectionBase,
+    key: str,
+    obs_range: range,
+    var_range: range,
+    value_gen: Callable[[range, range], spmatrix],
 ) -> None:
-    a = coll.add_new_sparse_ndarray(key, type=pa.float32(), shape=shape)
-    tensor = pa.SparseCOOTensor.from_scipy(value_gen(shape))
+    a = coll.add_new_sparse_ndarray(key, type=pa.float32(), shape=(obs_range.stop, var_range.stop))
+    tensor = pa.SparseCOOTensor.from_scipy(value_gen(obs_range, var_range))
     a.write(tensor)
 
 
 @pytest.fixture(scope="function")
 def soma_experiment(
     tmp_path: pathlib.Path,
-    n_obs: int,
-    n_vars: int,
-    X_layer_names: Sequence[str],
-    X_value_gen: Callable[[Tuple[int, int]], sparse.spmatrix],
+    obs_range: Union[int, range],
+    var_range: Union[int, range],
+    X_value_gen: Callable[[range, range], sparse.spmatrix],
     obsp_layer_names: Sequence[str],
     varp_layer_names: Sequence[str],
 ) -> soma.Experiment:
     with soma.Experiment.create((tmp_path / "exp").as_posix()) as exp:
-        add_dataframe(exp, "obs", n_obs)
+        if isinstance(obs_range, int):
+            obs_range = range(obs_range)
+        if isinstance(var_range, int):
+            var_range = range(var_range)
+
+        add_dataframe(exp, "obs", obs_range)
         ms = exp.add_new_collection("ms")
         rna = ms.add_new_collection("RNA", soma.Measurement)
-        add_dataframe(rna, "var", n_vars)
+        add_dataframe(rna, "var", var_range)
         rna_x = rna.add_new_collection("X", soma.Collection)
-        for X_layer_name in X_layer_names:
-            add_sparse_array(rna_x, X_layer_name, (n_obs, n_vars), X_value_gen)
+        add_sparse_array(rna_x, "raw", obs_range, var_range, X_value_gen)
 
         if obsp_layer_names:
             obsp = rna.add_new_collection("obsp")
             for obsp_layer_name in obsp_layer_names:
-                add_sparse_array(obsp, obsp_layer_name, (n_obs, n_obs), X_value_gen)
+                add_sparse_array(obsp, obsp_layer_name, obs_range, var_range, X_value_gen)
 
         if varp_layer_names:
             varp = rna.add_new_collection("varp")
             for varp_layer_name in varp_layer_names:
-                add_sparse_array(varp, varp_layer_name, (n_vars, n_vars), X_value_gen)
+                add_sparse_array(varp, varp_layer_name, obs_range, var_range, X_value_gen)
     return _factory.open((tmp_path / "exp").as_posix())
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(6, 3, pytorch_x_value_gen)])
 def test_non_batched(soma_experiment: Experiment) -> None:
     exp_data_pipe = ExperimentDataPipe(
         soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"]
     )
     row_iter = iter(exp_data_pipe)
 
     row = next(row_iter)
     assert row[0].int().tolist() == [0, 1, 0]
     assert row[1].tolist() == [0, 0]
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized,DuplicatedCode
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(6, 3, pytorch_x_value_gen)])
 def test_batching__all_batches_full_size(soma_experiment: Experiment) -> None:
     exp_data_pipe = ExperimentDataPipe(
         soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"], batch_size=3
     )
     batch_iter = iter(exp_data_pipe)
 
     batch = next(batch_iter)
@@ -149,16 +151,29 @@
     assert batch[1].tolist() == [[3, 3], [4, 4], [5, 5]]
 
     with pytest.raises(StopIteration):
         next(batch_iter)
 
 
 @pytest.mark.experimental
+# noinspection PyTestParametrized,DuplicatedCode
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(range(100_000_000, 100_000_003), 3, pytorch_x_value_gen)])
+def test_unique_soma_joinids(soma_experiment: Experiment) -> None:
+    exp_data_pipe = ExperimentDataPipe(
+        soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"], batch_size=3
+    )
+
+    soma_joinids = np.concatenate([batch[1][:, 0].numpy() for batch in exp_data_pipe])
+
+    assert len(np.unique(soma_joinids)) == len(soma_joinids)
+
+
+@pytest.mark.experimental
 # noinspection PyTestParametrized
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(5, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(5, 3, pytorch_x_value_gen)])
 def test_batching__partial_final_batch_size(soma_experiment: Experiment) -> None:
     exp_data_pipe = ExperimentDataPipe(
         soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"], batch_size=3
     )
     batch_iter = iter(exp_data_pipe)
 
     next(batch_iter)
@@ -167,15 +182,15 @@
 
     with pytest.raises(StopIteration):
         next(batch_iter)
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized,DuplicatedCode
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(3, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(3, 3, pytorch_x_value_gen)])
 def test_batching__exactly_one_batch(soma_experiment: Experiment) -> None:
     exp_data_pipe = ExperimentDataPipe(
         soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"], batch_size=3
     )
     batch_iter = iter(exp_data_pipe)
 
     batch = next(batch_iter)
@@ -184,15 +199,15 @@
 
     with pytest.raises(StopIteration):
         next(batch_iter)
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(6, 3, pytorch_x_value_gen)])
 def test_batching__empty_query_result(soma_experiment: Experiment) -> None:
     exp_data_pipe = ExperimentDataPipe(
         soma_experiment,
         measurement_name="RNA",
         X_name="raw",
         obs_query=AxisQuery(coords=([],)),
         obs_column_names=["label"],
@@ -202,15 +217,15 @@
 
     with pytest.raises(StopIteration):
         next(batch_iter)
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(6, 3, pytorch_x_value_gen)])
 def test_sparse_output__non_batched(soma_experiment: Experiment) -> None:
     exp_data_pipe = ExperimentDataPipe(
         soma_experiment,
         measurement_name="RNA",
         X_name="raw",
         obs_column_names=["label"],
         sparse_X=True,
@@ -220,15 +235,15 @@
     batch = next(batch_iter)
     assert isinstance(batch[1], Tensor)
     assert batch[0].to_dense().tolist() == [0, 1, 0]
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(6, 3, pytorch_x_value_gen)])
 def test_sparse_output__batched(soma_experiment: Experiment) -> None:
     exp_data_pipe = ExperimentDataPipe(
         soma_experiment,
         measurement_name="RNA",
         X_name="raw",
         obs_column_names=["label"],
         batch_size=3,
@@ -238,40 +253,65 @@
 
     batch = next(batch_iter)
     assert isinstance(batch[1], Tensor)
     assert batch[0].to_dense().tolist() == [[0, 1, 0], [1, 0, 1], [0, 1, 0]]
 
 
 @pytest.mark.experimental
+# noinspection PyTestParametrized,DuplicatedCode
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(10, 1, pytorch_x_value_gen)])
+def test_batching__partial_soma_batches_are_concatenated(soma_experiment: Experiment) -> None:
+    with patch("cellxgene_census.experimental.ml.pytorch._ObsAndXSOMAIterator.__next__") as mock_soma_iterator_next:
+        # Mock the SOMA batch sizes such that PyTorch batches will span the tail and head of two SOMA batches
+        mock_soma_iterator_next.side_effect = [
+            ObsAndXSOMABatch(pd.DataFrame({"soma_joinid": list(range(0, 4))}), sparse.csr_matrix([[1]] * 4), Stats()),
+            ObsAndXSOMABatch(pd.DataFrame({"soma_joinid": list(range(4, 8))}), sparse.csr_matrix([[1]] * 4), Stats()),
+            ObsAndXSOMABatch(pd.DataFrame({"soma_joinid": list(range(8, 10))}), sparse.csr_matrix([[1]] * 2), Stats()),
+        ]
+
+        exp_data_pipe = ExperimentDataPipe(
+            soma_experiment,
+            measurement_name="RNA",
+            X_name="raw",
+            obs_column_names=[],
+            batch_size=3,
+        )
+
+        full_result = list(exp_data_pipe)
+
+        assert [len(batch[1]) for batch in full_result] == [3, 3, 3, 1]
+
+
+@pytest.mark.experimental
 # noinspection PyTestParametrized
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(3, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(3, 3, pytorch_x_value_gen)])
 def test_encoders(soma_experiment: Experiment) -> None:
     exp_data_pipe = ExperimentDataPipe(
         soma_experiment,
         measurement_name="RNA",
         X_name="raw",
         obs_column_names=["label"],
         batch_size=3,
     )
     batch_iter = iter(exp_data_pipe)
 
     batch = next(batch_iter)
     assert isinstance(batch[1], Tensor)
 
     labels_encoded = batch[1][:, 1]
-    labels_decoded = exp_data_pipe.obs_encoders()["label"].inverse_transform(labels_encoded)
+    labels_decoded = exp_data_pipe.obs_encoders["label"].inverse_transform(labels_encoded)
     assert labels_decoded.tolist() == ["0", "1", "2"]
 
 
 @pytest.mark.experimental
 @pytest.mark.skipif(
     (sys.version_info.major, sys.version_info.minor) == (3, 9), reason="fails intermittently with OOM error for 3.9"
 )
 # noinspection PyTestParametrized
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(6, 3, pytorch_x_value_gen)])
 def test_multiprocessing__returns_full_result(soma_experiment: Experiment) -> None:
     dp = ExperimentDataPipe(
         soma_experiment,
         measurement_name="RNA",
         X_name="raw",
         obs_column_names=["label"],
     )
@@ -281,28 +321,28 @@
 
     soma_joinids = [t[1][0].item() for t in full_result]
     assert sorted(soma_joinids) == list(range(6))
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized,DuplicatedCode
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(3, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(3, 3, pytorch_x_value_gen)])
 def test_experiment_dataloader__non_batched(soma_experiment: Experiment) -> None:
     dp = ExperimentDataPipe(soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"])
     dl = experiment_dataloader(dp)
     torch_data = [row for row in dl]
 
     row = torch_data[0]
     assert row[0].to_dense().tolist() == [0, 1, 0]
     assert row[1].tolist() == [0, 0]
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized,DuplicatedCode
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(6, 3, pytorch_x_value_gen)])
 def test_experiment_dataloader__batched(soma_experiment: Experiment) -> None:
     dp = ExperimentDataPipe(
         soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"], batch_size=3
     )
     dl = experiment_dataloader(dp)
     torch_data = [row for row in dl]
 
@@ -321,60 +361,37 @@
 @pytest.mark.skip(reason="Not implemented")
 def test_experiment_dataloader__multiprocess_dense_matrix__ok() -> None:
     pass
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized,DuplicatedCode
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(10, 1, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(10, 1, pytorch_x_value_gen)])
 def test_experiment_dataloader__splitting(soma_experiment: Experiment) -> None:
     dp = ExperimentDataPipe(soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"])
     dp_train, dp_test = dp.random_split(weights={"train": 0.7, "test": 0.3}, seed=1234)
     dl = experiment_dataloader(dp_train)
 
     all_rows = list(iter(dl))
     assert len(all_rows) == 7
 
 
 @pytest.mark.experimental
 # noinspection PyTestParametrized,DuplicatedCode
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(10, 1, ("raw",), pytorch_x_value_gen)])
+@pytest.mark.parametrize("obs_range,var_range,X_value_gen", [(10, 1, pytorch_x_value_gen)])
 def test_experiment_dataloader__shuffling(soma_experiment: Experiment) -> None:
     dp = ExperimentDataPipe(soma_experiment, measurement_name="RNA", X_name="raw", obs_column_names=["label"])
     dp = dp.shuffle()
     dl = experiment_dataloader(dp)
 
     data1 = list(iter(dl))
     data2 = list(iter(dl))
 
     data1_soma_joinids = [row[1][0].item() for row in data1]
     data2_soma_joinids = [row[1][0].item() for row in data2]
     assert data1_soma_joinids != data2_soma_joinids
 
 
 @pytest.mark.experimental
-# noinspection PyTestParametrized,DuplicatedCode
-@pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(3, 3, ("raw",), pytorch_x_value_gen)])
-def test_experiment_dataloader__multiprocess_pickling(soma_experiment: Experiment) -> None:
-    """
-    If the DataPipe is accessed prior to multiprocessing (num_workers > 0), its internal _query will be
-    initialized. But since it cannot be pickled, we must ensure it is ignored during pickling in multiprocessing mode.
-    This test verifies the correct pickling behavior is in place.
-    """
-
-    dp = ExperimentDataPipe(
-        soma_experiment,
-        measurement_name="RNA",
-        X_name="raw",
-        obs_column_names=["label"],
-    )
-    dl = experiment_dataloader(dp, num_workers=1)  # multiprocessing used when num_workers > 0
-    dp.obs_encoders()  # trigger query building
-    row = next(iter(dl))  # trigger multiprocessing
-
-    assert row is not None
-
-
-@pytest.mark.experimental
 @pytest.mark.skip(reason="TODO")
 def test_experiment_data_loader__unsupported_params__fails() -> None:
     pass
```

### Comparing `cellxgene_census-1.2.1/tests/experimental/pp/test_hvg.py` & `cellxgene_census-1.3.0/tests/experimental/pp/test_hvg.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 @pytest.fixture
 def small_mem_context() -> soma.SOMATileDBContext:
     """used to keep memory usage smaller for GHA runners."""
     cfg = {
         "tiledb_config": {
-            "soma.init_buffer_bytes": 64 * 1024**2,
+            "soma.init_buffer_bytes": 32 * 1024**2,
             "vfs.s3.no_sign_request": True,
         },
     }
     return soma.SOMATileDBContext().replace(**cfg)
 
 
 @pytest.mark.experimental
@@ -133,26 +133,26 @@
 
     assert isinstance(hvg, pd.DataFrame)
     assert len(hvg) == n_vars
     assert len(hvg[hvg.highly_variable]) == 1000
 
 
 @pytest.mark.experimental
-def test_hvg_error_cases() -> None:
-    with cellxgene_census.open_soma(census_version="stable") as census:
+def test_hvg_error_cases(small_mem_context: soma.SOMATileDBContext) -> None:
+    with cellxgene_census.open_soma(census_version="stable", context=small_mem_context) as census:
         with census["census_data"]["mus_musculus"].axis_query(measurement_name="RNA") as query:
             # Only flavor="seurat_v3" is supported
             with pytest.raises(ValueError):
                 highly_variable_genes(query, flavor="oopsie")  # type: ignore[arg-type]
 
 
 @pytest.mark.experimental
 @pytest.mark.live_corpus
-def test_max_loess_jitter_error() -> None:
-    with cellxgene_census.open_soma(census_version="stable") as census:
+def test_max_loess_jitter_error(small_mem_context: soma.SOMATileDBContext) -> None:
+    with cellxgene_census.open_soma(census_version="stable", context=small_mem_context) as census:
         with pytest.raises(ValueError):
             get_highly_variable_genes(
                 census,
                 organism="mus_musculus",
                 obs_value_filter='is_primary_data == True and tissue_general == "heart"',
                 batch_key="cell_type",
                 max_loess_jitter=0.0,
```

### Comparing `cellxgene_census-1.2.1/tests/experimental/pp/test_online.py` & `cellxgene_census-1.3.0/tests/experimental/pp/test_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/tests/test_acceptance.py` & `cellxgene_census-1.3.0/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/tests/test_directory.py` & `cellxgene_census-1.3.0/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/tests/test_get_anndata.py` & `cellxgene_census-1.3.0/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/tests/test_get_helpers.py` & `cellxgene_census-1.3.0/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/tests/test_open.py` & `cellxgene_census-1.3.0/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.1/tests/test_util.py` & `cellxgene_census-1.3.0/tests/test_util.py`

 * *Files identical despite different names*

