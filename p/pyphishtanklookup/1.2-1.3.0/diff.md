# Comparing `tmp/pyphishtanklookup-1.2.tar.gz` & `tmp/pyphishtanklookup-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphishtanklookup-1.2.tar", max compression
+gzip compressed data, was "pyphishtanklookup-1.3.0.tar", max compression
```

## Comparing `pyphishtanklookup-1.2.tar` & `pyphishtanklookup-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1516 2021-09-14 11:44:38.348381 pyphishtanklookup-1.2/LICENSE
--rw-r--r--   0        0        0      932 2021-09-15 11:51:12.145916 pyphishtanklookup-1.2/README.md
--rw-r--r--   0        0        0     1535 2021-09-15 10:15:33.732488 pyphishtanklookup-1.2/pyphishtanklookup/__init__.py
--rw-r--r--   0        0        0     3944 2021-12-21 15:29:58.537951 pyphishtanklookup-1.2/pyphishtanklookup/api.py
--rw-r--r--   0        0        0        0 2021-09-14 11:44:38.612384 pyphishtanklookup-1.2/pyphishtanklookup/py.typed
--rw-r--r--   0        0        0     1300 2023-01-03 12:57:29.781171 pyphishtanklookup-1.2/pyproject.toml
--rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 pyphishtanklookup-1.2/setup.py
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 pyphishtanklookup-1.2/PKG-INFO
+-rw-r--r--   0        0        0     1516 2021-09-14 11:44:38.348381 pyphishtanklookup-1.3.0/LICENSE
+-rw-r--r--   0        0        0      932 2021-09-15 11:51:12.145916 pyphishtanklookup-1.3.0/README.md
+-rw-r--r--   0        0        0     1535 2021-09-15 10:15:33.732488 pyphishtanklookup-1.3.0/pyphishtanklookup/__init__.py
+-rw-r--r--   0        0        0     3944 2021-12-21 15:29:58.537951 pyphishtanklookup-1.3.0/pyphishtanklookup/api.py
+-rw-r--r--   0        0        0        0 2021-09-14 11:44:38.612384 pyphishtanklookup-1.3.0/pyphishtanklookup/py.typed
+-rw-r--r--   0        0        0     1476 2023-06-30 12:12:03.747210 pyphishtanklookup-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 pyphishtanklookup-1.3.0/PKG-INFO
```

### Comparing `pyphishtanklookup-1.2/LICENSE` & `pyphishtanklookup-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphishtanklookup-1.2/README.md` & `pyphishtanklookup-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyphishtanklookup-1.2/pyphishtanklookup/__init__.py` & `pyphishtanklookup-1.3.0/pyphishtanklookup/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphishtanklookup-1.2/pyphishtanklookup/api.py` & `pyphishtanklookup-1.3.0/pyphishtanklookup/api.py`

 * *Files identical despite different names*

### Comparing `pyphishtanklookup-1.2/pyproject.toml` & `pyphishtanklookup-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyphishtanklookup"
-version = "1.2"
+version = "1.3.0"
 description = "Python CLI and module for PhishtankLookup"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/lookyloo/PyPhishtankLookup"
 
 readme = "README.md"
 
@@ -15,34 +15,39 @@
     'Operating System :: POSIX :: Linux',
     'Intended Audience :: Science/Research',
     'Intended Audience :: Telecommunications Industry',
     'Intended Audience :: Information Technology',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Security',
     'Topic :: Internet',
 ]
 
 include = ['README.md']
 
 [tool.poetry.scripts]
 phishtank-lookup = 'pyphishtanklookup:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.28.1"
-Sphinx = { version = "^6.0.0", optional = true }
+requests = "^2.31.0"
+Sphinx = { version = "^6.2.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.991"
-types-requests = "^2.28.11.7"
-ipython = "^8.7.0"
-pytest-cov = "^4.0.0"
-types-setuptools = "^65.6.0.2"
+types-requests = "^2.31.0.1"
+ipython = [
+    {version = "<8.13.0", python = "<3.9"},
+    {version = "^8.13.0", python = ">=3.9"}
+]
+pytest-cov = "^4.1.0"
+types-setuptools = "^65.7.0.4"
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [build-system]
 requires = ["poetry_core>=1.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyphishtanklookup-1.2/PKG-INFO` & `pyphishtanklookup-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphishtanklookup
-Version: 1.2
+Version: 1.3.0
 Summary: Python CLI and module for PhishtankLookup
 Home-page: https://github.com/lookyloo/PyPhishtankLookup
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,22 +15,19 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=6.0.0,<7.0.0) ; extra == "docs"
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: Sphinx (>=6.2.1,<7.0.0) ; extra == "docs"
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/lookyloo/PyPhishtankLookup
 Description-Content-Type: text/markdown
 
 # PyPhishtank Lookup
 
 This is the client API for [Phishtank Lookup](https://github.com/Lookyloo/phishtank-lookup),
 not the official phishtank API.
```

