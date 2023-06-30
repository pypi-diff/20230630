# Comparing `tmp/pylookyloomonitoring-1.0.5.tar.gz` & `tmp/pylookyloomonitoring-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylookyloomonitoring-1.0.5.tar", max compression
+gzip compressed data, was "pylookyloomonitoring-1.1.0.tar", max compression
```

## Comparing `pylookyloomonitoring-1.0.5.tar` & `pylookyloomonitoring-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1516 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.5/LICENSE
--rw-r--r--   0        0        0      822 2023-02-28 15:25:48.760683 pylookyloomonitoring-1.0.5/README.md
--rw-r--r--   0        0        0      953 2023-02-28 11:41:23.346353 pylookyloomonitoring-1.0.5/pylookyloomonitoring/__init__.py
--rw-r--r--   0        0        0     6746 2023-05-10 14:23:50.249459 pylookyloomonitoring-1.0.5/pylookyloomonitoring/api.py
--rw-r--r--   0        0        0        0 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.5/pylookyloomonitoring/py.typed
--rw-r--r--   0        0        0     1541 2023-05-23 13:12:59.377411 pylookyloomonitoring-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 pylookyloomonitoring-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.1.0/LICENSE
+-rw-r--r--   0        0        0      822 2023-02-28 15:25:48.760683 pylookyloomonitoring-1.1.0/README.md
+-rw-r--r--   0        0        0      953 2023-02-28 11:41:23.346353 pylookyloomonitoring-1.1.0/pylookyloomonitoring/__init__.py
+-rw-r--r--   0        0        0     6746 2023-05-10 14:23:50.249459 pylookyloomonitoring-1.1.0/pylookyloomonitoring/api.py
+-rw-r--r--   0        0        0        0 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.1.0/pylookyloomonitoring/py.typed
+-rw-r--r--   0        0        0     1541 2023-06-30 09:55:13.178164 pylookyloomonitoring-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pylookyloomonitoring-1.1.0/PKG-INFO
```

### Comparing `pylookyloomonitoring-1.0.5/LICENSE` & `pylookyloomonitoring-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.5/README.md` & `pylookyloomonitoring-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.5/pylookyloomonitoring/__init__.py` & `pylookyloomonitoring-1.1.0/pylookyloomonitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.5/pylookyloomonitoring/api.py` & `pylookyloomonitoring-1.1.0/pylookyloomonitoring/api.py`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.5/pyproject.toml` & `pylookyloomonitoring-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylookyloomonitoring"
-version = "1.0.5"
+version = "1.1.0"
 description = "Python API to connect to lookyloo monitoring"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PyLookylooMonitoring"
 documentation = "https://pylookyloomonitoring.readthedocs.io/en/latest/index.html"
 
 readme = "README.md"
@@ -37,18 +37,18 @@
 Sphinx = { version = "^7.0.1", optional = true }
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
-mypy = "^1.3.0"
-types-requests = "^2.31.0.0"
+mypy = "^1.4.1"
+types-requests = "^2.31.0.1"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.13.0", python = ">=3.9"}
 ]
-pytest = "^7.3.1"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pylookyloomonitoring-1.0.5/PKG-INFO` & `pylookyloomonitoring-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookyloomonitoring
-Version: 1.0.5
+Version: 1.1.0
 Summary: Python API to connect to lookyloo monitoring
 Home-page: https://github.com/Lookyloo/PyLookylooMonitoring
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,14 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://pylookyloomonitoring.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/Lookyloo/PyLookylooMonitoring
```

