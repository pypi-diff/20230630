# Comparing `tmp/lazy_loader-0.2rc0.tar.gz` & `tmp/lazy_loader-0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_loader-0.2rc0.tar", last modified: Fri Mar 17 15:21:07 2023, max compression
+gzip compressed data, was "lazy_loader-0.3rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lazy_loader-0.2rc0.tar` & `lazy_loader-0.3rc0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      424 2022-08-29 12:38:20.243086 lazy_loader-0.2rc0/.flake8
--rw-r--r--   0        0        0      998 2023-03-12 06:38:52.685654 lazy_loader-0.2rc0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      830 2022-08-29 12:38:20.243086 lazy_loader-0.2rc0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      873 2023-03-11 00:04:48.471309 lazy_loader-0.2rc0/.github/workflows/test.yml
--rw-r--r--   0        0        0      318 2022-08-29 12:32:40.949990 lazy_loader-0.2rc0/.gitignore
--rw-r--r--   0        0        0     1030 2023-03-10 23:56:36.092310 lazy_loader-0.2rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6653 2023-03-17 15:13:19.083813 lazy_loader-0.2rc0/CHANGELOG.md
--rw-r--r--   0        0        0     1539 2023-03-12 04:16:06.935401 lazy_loader-0.2rc0/LICENSE.md
--rw-r--r--   0        0        0     3178 2023-03-16 23:49:10.428869 lazy_loader-0.2rc0/README.md
--rw-r--r--   0        0        0     1419 2023-03-11 00:41:09.081166 lazy_loader-0.2rc0/RELEASE.md
--rw-r--r--   0        0        0     7825 2023-03-10 23:41:47.566938 lazy_loader-0.2rc0/lazy_loader/__init__.py
--rw-r--r--   0        0        0        0 2022-08-29 12:38:20.244086 lazy_loader-0.2rc0/lazy_loader/tests/__init__.py
--rw-r--r--   0        0        0      136 2022-08-29 12:38:20.244086 lazy_loader-0.2rc0/lazy_loader/tests/fake_pkg/__init__.py
--rw-r--r--   0        0        0       33 2022-08-29 12:38:20.244086 lazy_loader-0.2rc0/lazy_loader/tests/fake_pkg/__init__.pyi
--rw-r--r--   0        0        0       74 2022-08-29 12:38:20.244086 lazy_loader-0.2rc0/lazy_loader/tests/fake_pkg/some_func.py
--rw-r--r--   0        0        0     4082 2023-03-12 06:38:52.685654 lazy_loader-0.2rc0/lazy_loader/tests/test_lazy_loader.py
--rw-r--r--   0        0        0      932 2023-03-17 15:12:59.552754 lazy_loader-0.2rc0/pyproject.toml
--rw-r--r--   0        0        0     4078 1970-01-01 00:00:00.000000 lazy_loader-0.2rc0/PKG-INFO
+-rw-r--r--   0        0        0      207 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/.github/dependabot.yml
+-rw-r--r--   0        0        0      998 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      830 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      994 2023-06-27 19:28:19.549616 lazy_loader-0.3rc0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      318 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/.gitignore
+-rw-r--r--   0        0        0     1025 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6916 2023-06-30 20:16:43.694958 lazy_loader-0.3rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     1539 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/LICENSE.md
+-rw-r--r--   0        0        0     3361 2023-06-28 01:54:21.971546 lazy_loader-0.3rc0/README.md
+-rw-r--r--   0        0        0     1419 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/RELEASE.md
+-rw-r--r--   0        0        0     8555 2023-06-28 01:54:21.972546 lazy_loader-0.3rc0/lazy_loader/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:17:17.686092 lazy_loader-0.3rc0/lazy_loader/tests/__init__.py
+-rw-r--r--   0        0        0      136 2023-06-08 18:17:17.687091 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-27 20:26:36.582245 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/__init__.pyi
+-rw-r--r--   0        0        0       74 2023-06-08 18:17:17.687091 lazy_loader-0.3rc0/lazy_loader/tests/fake_pkg/some_func.py
+-rw-r--r--   0        0        0     4468 2023-06-28 01:54:21.972546 lazy_loader-0.3rc0/lazy_loader/tests/test_lazy_loader.py
+-rw-r--r--   0        0        0     1192 2023-06-30 20:17:15.640112 lazy_loader-0.3rc0/pyproject.toml
+-rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 lazy_loader-0.3rc0/PKG-INFO
```

### Comparing `lazy_loader-0.2rc0/.github/workflows/coverage.yml` & `lazy_loader-0.3rc0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.2rc0/.github/workflows/lint.yml` & `lazy_loader-0.3rc0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.2rc0/.github/workflows/test.yml` & `lazy_loader-0.3rc0/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 jobs:
   default:
     runs-on: ${{ matrix.os }}-latest
     strategy:
       matrix:
         os: [ubuntu, macos, windows]
         python-version:
-          ["3.7", "3.8", "3.9", "3.10", "3.11", "pypy-3.8", "pypy-3.9"]
+          [
+            "3.7",
+            "3.8",
+            "3.9",
+            "3.10",
+            "3.11",
+            "3.12-dev",
+            "pypy-3.8",
+            "pypy-3.9",
+          ]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `lazy_loader-0.2rc0/CHANGELOG.md` & `lazy_loader-0.3rc0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [v0.2](https://github.com/scientific-python/lazy_loader/tree/v0.2)
+
+[Full Changelog](https://github.com/scientific-python/lazy_loader/compare/v0.1...v0.2)
+
+There were no changes since the release candidate, so
+see release notes for v0.2rc0 below for details.
+
 ## [v0.2rc0](https://github.com/scientific-python/lazy_loader/tree/v0.2rc0)
 
 [Full Changelog](https://github.com/scientific-python/lazy_loader/compare/v0.1...v0.2rc0)
 
 **Closed issues:**
 
 - Allow to not fail on stub attach in frozen apps [\#38](https://github.com/scientific-python/lazy_loader/issues/38)
```

### Comparing `lazy_loader-0.2rc0/LICENSE.md` & `lazy_loader-0.3rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.2rc0/README.md` & `lazy_loader-0.3rc0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,21 @@
 
 The `lazy.attach` function discussed above is used to set up package
 internal imports.
 
 Use `lazy.load` to lazily import external libraries:
 
 ```python
-linalg = lazy.load('scipy.linalg')  # `linalg` will only be loaded when accessed
+sp = lazy.load('scipy')  # `sp` will only be loaded when accessed
+sp.linalg.norm(...)
 ```
 
-You can also ask `lazy.load` to raise import errors as soon as it is called:
+_Note that lazily importing *sub*packages,
+i.e. `load('scipy.linalg')` will cause the package containing the
+subpackage to be imported immediately; thus, this usage is
+discouraged._
+
+You can ask `lazy.load` to raise import errors as soon as it is called:
 
 ```
 linalg = lazy.load('scipy.linalg', error_on_import=True)
 ```
```

### Comparing `lazy_loader-0.2rc0/RELEASE.md` & `lazy_loader-0.3rc0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `lazy_loader-0.2rc0/lazy_loader/__init__.py` & `lazy_loader-0.3rc0/lazy_loader/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import ast
 import importlib
 import importlib.util
 import inspect
 import os
 import sys
 import types
+import warnings
 
 __all__ = ["attach", "load", "attach_stub"]
 
 
 def attach(package_name, submodules=None, submod_attrs=None):
     """Attach lazily loaded submodules, functions, or other attributes.
 
@@ -62,15 +63,15 @@
     else:
         submodules = set(submodules)
 
     attr_to_modules = {
         attr: mod for mod, attrs in submod_attrs.items() for attr in attrs
     }
 
-    __all__ = list(sorted(submodules | attr_to_modules.keys()))
+    __all__ = sorted(submodules | attr_to_modules.keys())
 
     def __getattr__(name):
         if name in submodules:
             return importlib.import_module(f"{package_name}.{name}")
         elif name in attr_to_modules:
             submod_path = f"{package_name}.{attr_to_modules[name]}"
             submod = importlib.import_module(submod_path)
@@ -117,42 +118,52 @@
 
 def load(fullname, error_on_import=False):
     """Return a lazily imported proxy for a module.
 
     We often see the following pattern::
 
       def myfunc():
-          from numpy import linalg as la
-          la.norm(...)
+          import numpy as np
+          np.norm(...)
           ....
 
-    This is to prevent a module, in this case `numpy`, from being
-    imported at function definition time, since that can be slow.
+    Putting the import inside the function prevents, in this case,
+    `numpy`, from being imported at function definition time.
+    That saves time if `myfunc` ends up not being called.
 
-    This function provides a proxy module that, upon access, imports
+    This `load` function returns a proxy module that, upon access, imports
     the actual module.  So the idiom equivalent to the above example is::
 
-      la = lazy.load("numpy.linalg")
+      np = lazy.load("numpy")
 
       def myfunc():
-          la.norm(...)
+          np.norm(...)
           ....
 
     The initial import time is fast because the actual import is delayed
     until the first attribute is requested. The overall import time may
     decrease as well for users that don't make use of large portions
-    of the library.
+    of your library.
+
+    Warning
+    -------
+    While lazily loading *sub*packages technically works, it causes the
+    package (that contains the subpackage) to be eagerly loaded even
+    if the package is already lazily loaded.
+    So, you probably shouldn't use subpackages with this `load` feature.
+    Instead you should encourage the package maintainers to use the
+    `lazy_loader.attach` to make their subpackages load lazily.
 
     Parameters
     ----------
     fullname : str
         The full name of the module or submodule to import.  For example::
 
           sp = lazy.load('scipy')  # import scipy as sp
-          spla = lazy.load('scipy.linalg')  # import scipy.linalg as spla
+
     error_on_import : bool
         Whether to postpone raising import errors until the module is accessed.
         If set to `True`, import errors are raised as soon as `load` is called.
 
     Returns
     -------
     pm : importlib.util._LazyModule
@@ -161,14 +172,22 @@
 
     """
     try:
         return sys.modules[fullname]
     except KeyError:
         pass
 
+    if "." in fullname:
+        msg = (
+            "subpackages can technically be lazily loaded, but it causes the "
+            "package to be eagerly loaded even if it is already lazily loaded."
+            "So, you probably shouldn't use subpackages with this lazy feature."
+        )
+        warnings.warn(msg, RuntimeWarning)
+
     spec = importlib.util.find_spec(fullname)
     if spec is None:
         if error_on_import:
             raise ModuleNotFoundError(f"No module named '{fullname}'")
         else:
             try:
                 parent = inspect.stack()[1]
```

### Comparing `lazy_loader-0.2rc0/lazy_loader/tests/test_lazy_loader.py` & `lazy_loader-0.3rc0/lazy_loader/tests/test_lazy_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import importlib
 import sys
 import types
 
 import pytest
 
 import lazy_loader as lazy
 
@@ -11,26 +12,36 @@
     anything_not_real = lazy.load("anything_not_real")
 
     # Now test that accessing attributes does what it should
     assert math.sin(math.pi) == pytest.approx(0, 1e-6)
     # poor-mans pytest.raises for testing errors on attribute access
     try:
         anything_not_real.pi
-        assert False  # Should not get here
+        raise AssertionError()  # Should not get here
     except ModuleNotFoundError:
         pass
     assert isinstance(anything_not_real, lazy.DelayedImportErrorModule)
     # see if it changes for second access
     try:
         anything_not_real.pi
-        assert False  # Should not get here
+        raise AssertionError()  # Should not get here
     except ModuleNotFoundError:
         pass
 
 
+def test_lazy_import_subpackages():
+    with pytest.warns(RuntimeWarning):
+        hp = lazy.load("html.parser")
+    assert "html" in sys.modules
+    assert type(sys.modules["html"]) == type(pytest)
+    assert isinstance(hp, importlib.util._LazyModule)
+    assert "html.parser" in sys.modules
+    assert sys.modules["html.parser"] == hp
+
+
 def test_lazy_import_impact_on_sys_modules():
     math = lazy.load("math")
     anything_not_real = lazy.load("anything_not_real")
 
     assert isinstance(math, types.ModuleType)
     assert "math" in sys.modules
     assert isinstance(anything_not_real, lazy.DelayedImportErrorModule)
@@ -52,15 +63,15 @@
     np = lazy.load("numpy")
     sp = lazy.load("scipy")
     if not isinstance(np, lazy.DelayedImportErrorModule):
         assert np.sin(np.pi) == pytest.approx(0, 1e-6)
     if isinstance(sp, lazy.DelayedImportErrorModule):
         try:
             sp.pi
-            assert False
+            raise AssertionError()
         except ModuleNotFoundError:
             pass
 
 
 def test_lazy_attach():
     name = "mymod"
     submods = ["mysubmodule", "anothersubmodule"]
```

### Comparing `lazy_loader-0.2rc0/pyproject.toml` & `lazy_loader-0.3rc0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,52 @@
 [build-system]
 requires = ["flit_core >=3.8,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lazy_loader"
-version = "0.2rc0"
+version = "0.3rc0"
 requires-python = ">=3.7"
 authors = [{name = "Scientific Python Developers"}]
 readme = "README.md"
 license = {file = "LICENSE.md"}
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 dynamic = ["description"]
 
 
 [project.optional-dependencies]
-test = ["pytest >= 7.2", "pytest-cov >= 4.0"]
-lint = ["pre-commit >= 3.1"]
+test = ["pytest >= 7.4", "pytest-cov >= 4.1"]
+lint = ["pre-commit >= 3.3"]
 
 [project.urls]
 Home = "https://scientific-python.org/specs/spec-0001/"
 Source = "https://github.com/scientific-python/lazy_loader"
 
 [tool.flit.sdist]
 exclude = ["tests/*"]
+
+[tool.ruff]
+line-length = 88
+target-version = "py37"
+select = [
+    "C",
+    "E",
+    "F",
+    "W",
+    "B",
+    "I",
+    "UP",
+]
+ignore = ["B018", "B028"]
+exclude = [
+  "lazy_loader/tests/fake_pkg/__init__.pyi",
+]
```

### Comparing `lazy_loader-0.2rc0/PKG-INFO` & `lazy_loader-0.3rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: lazy_loader
-Version: 0.2rc0
+Version: 0.3rc0
 Summary: lazy_loader
 Author: Scientific Python Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pre-commit >= 3.1 ; extra == "lint"
-Requires-Dist: pytest >= 7.2 ; extra == "test"
-Requires-Dist: pytest-cov >= 4.0 ; extra == "test"
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pre-commit >= 3.3 ; extra == "lint"
+Requires-Dist: pytest >= 7.4 ; extra == "test"
+Requires-Dist: pytest-cov >= 4.1 ; extra == "test"
 Project-URL: Home, https://scientific-python.org/specs/spec-0001/
 Project-URL: Source, https://github.com/scientific-python/lazy_loader
 Provides-Extra: lint
 Provides-Extra: test
 
 [![PyPI](https://img.shields.io/pypi/v/lazy_loader)](https://pypi.org/project/lazy_loader/)
 [![Test status](https://github.com/scientific-python/lazy_loader/workflows/test/badge.svg?branch=main)](https://github.com/scientific-python/lazy_loader/actions?query=workflow%3A%22test%22)
@@ -123,16 +124,22 @@
 
 The `lazy.attach` function discussed above is used to set up package
 internal imports.
 
 Use `lazy.load` to lazily import external libraries:
 
 ```python
-linalg = lazy.load('scipy.linalg')  # `linalg` will only be loaded when accessed
+sp = lazy.load('scipy')  # `sp` will only be loaded when accessed
+sp.linalg.norm(...)
 ```
 
-You can also ask `lazy.load` to raise import errors as soon as it is called:
+_Note that lazily importing *sub*packages,
+i.e. `load('scipy.linalg')` will cause the package containing the
+subpackage to be imported immediately; thus, this usage is
+discouraged._
+
+You can ask `lazy.load` to raise import errors as soon as it is called:
 
 ```
 linalg = lazy.load('scipy.linalg', error_on_import=True)
 ```
```

