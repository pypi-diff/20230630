# Comparing `tmp/peaklets-0.1.0.tar.gz` & `tmp/peaklets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peaklets-0.1.0.tar", last modified: Wed Mar 29 02:05:29 2023, max compression
+gzip compressed data, was "peaklets-0.1.1.tar", last modified: Wed Mar 29 02:26:27 2023, max compression
```

## Comparing `peaklets-0.1.0.tar` & `peaklets-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.065774 peaklets-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.061774 peaklets-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.061774 peaklets-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-29 02:05:19.000000 peaklets-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-29 02:05:19.000000 peaklets-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-29 02:05:19.000000 peaklets-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-29 02:05:19.000000 peaklets-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-29 02:05:29.065774 peaklets-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-29 02:05:19.000000 peaklets-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.065774 peaklets-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-29 02:05:19.000000 peaklets-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.065774 peaklets-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:19.000000 peaklets-0.1.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.065774 peaklets-0.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-29 02:05:19.000000 peaklets-0.1.0/docs/_templates/class_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-29 02:05:19.000000 peaklets-0.1.0/docs/_templates/function_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-29 02:05:19.000000 peaklets-0.1.0/docs/_templates/module_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-29 02:05:19.000000 peaklets-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-29 02:05:19.000000 peaklets-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-29 02:05:19.000000 peaklets-0.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.065774 peaklets-0.1.0/peaklets/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-29 02:05:19.000000 peaklets-0.1.0/peaklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-03-29 02:05:19.000000 peaklets-0.1.0/peaklets/peaklets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.065774 peaklets-0.1.0/peaklets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-29 02:05:19.000000 peaklets-0.1.0/peaklets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-29 02:05:19.000000 peaklets-0.1.0/peaklets/tests/test_peaklets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:05:29.065774 peaklets-0.1.0/peaklets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-29 02:05:29.000000 peaklets-0.1.0/peaklets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-29 02:05:29.000000 peaklets-0.1.0/peaklets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 02:05:29.000000 peaklets-0.1.0/peaklets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-29 02:05:29.000000 peaklets-0.1.0/peaklets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 02:05:29.000000 peaklets-0.1.0/peaklets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-29 02:05:19.000000 peaklets-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 02:05:29.065774 peaklets-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.870278 peaklets-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.858279 peaklets-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.862279 peaklets-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-29 02:26:16.000000 peaklets-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-29 02:26:16.000000 peaklets-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-29 02:26:16.000000 peaklets-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-29 02:26:16.000000 peaklets-0.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-29 02:26:27.866279 peaklets-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-29 02:26:16.000000 peaklets-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.862279 peaklets-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-29 02:26:16.000000 peaklets-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.862279 peaklets-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:16.000000 peaklets-0.1.1/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.866279 peaklets-0.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-29 02:26:16.000000 peaklets-0.1.1/docs/_templates/class_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-29 02:26:16.000000 peaklets-0.1.1/docs/_templates/function_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-29 02:26:16.000000 peaklets-0.1.1/docs/_templates/module_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-29 02:26:16.000000 peaklets-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-29 02:26:16.000000 peaklets-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-29 02:26:16.000000 peaklets-0.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.866279 peaklets-0.1.1/peaklets/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-29 02:26:16.000000 peaklets-0.1.1/peaklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-03-29 02:26:16.000000 peaklets-0.1.1/peaklets/peaklets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.866279 peaklets-0.1.1/peaklets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-29 02:26:16.000000 peaklets-0.1.1/peaklets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-29 02:26:16.000000 peaklets-0.1.1/peaklets/tests/test_peaklets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:26:27.866279 peaklets-0.1.1/peaklets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-29 02:26:27.000000 peaklets-0.1.1/peaklets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-29 02:26:27.000000 peaklets-0.1.1/peaklets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 02:26:27.000000 peaklets-0.1.1/peaklets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-29 02:26:27.000000 peaklets-0.1.1/peaklets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 02:26:27.000000 peaklets-0.1.1/peaklets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-29 02:26:16.000000 peaklets-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 02:26:27.870278 peaklets-0.1.1/setup.cfg
```

### Comparing `peaklets-0.1.0/.github/workflows/publish.yml` & `peaklets-0.1.1/.github/workflows/publish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 name: Publish to PyPI
 
-on: release
+on:
+  release:
+    types: [published]
 
 jobs:
   publish:
     name: Build and publish to PyPI and TestPyPI
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@master
```

### Comparing `peaklets-0.1.0/.github/workflows/tests.yml` & `peaklets-0.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/PKG-INFO` & `peaklets-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peaklets
-Version: 0.1.0
+Version: 0.1.1
 Summary: Decompose a 1D positive signal using only positive basis functions
 Author-email: "Charles C. Kankelborg" <kankel@montana.edu>, "Roy T. Smart" <roytsmart@gmail.com>
 Project-URL: Homepage, https://github.com/Kankelborg-Group/peaklets
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `peaklets-0.1.0/README.md` & `peaklets-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/docs/Makefile` & `peaklets-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/docs/_templates/class_custom.rst` & `peaklets-0.1.1/docs/_templates/class_custom.rst`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/docs/_templates/module_custom.rst` & `peaklets-0.1.1/docs/_templates/module_custom.rst`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/docs/conf.py` & `peaklets-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/docs/make.bat` & `peaklets-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/peaklets/peaklets.py` & `peaklets-0.1.1/peaklets/peaklets.py`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/peaklets/tests/test_peaklets.py` & `peaklets-0.1.1/peaklets/tests/test_peaklets.py`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/peaklets.egg-info/PKG-INFO` & `peaklets-0.1.1/peaklets.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peaklets
-Version: 0.1.0
+Version: 0.1.1
 Summary: Decompose a 1D positive signal using only positive basis functions
 Author-email: "Charles C. Kankelborg" <kankel@montana.edu>, "Roy T. Smart" <roytsmart@gmail.com>
 Project-URL: Homepage, https://github.com/Kankelborg-Group/peaklets
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `peaklets-0.1.0/peaklets.egg-info/SOURCES.txt` & `peaklets-0.1.1/peaklets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peaklets-0.1.0/pyproject.toml` & `peaklets-0.1.1/pyproject.toml`

 * *Files identical despite different names*

