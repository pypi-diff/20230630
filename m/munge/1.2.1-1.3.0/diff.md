# Comparing `tmp/munge-1.2.1.tar.gz` & `tmp/munge-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "munge-1.2.1.tar", max compression
+gzip compressed data, was "munge-1.3.0.tar", max compression
```

## Comparing `munge-1.2.1.tar` & `munge-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0    11358 2021-08-24 15:39:21.275709 munge-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1287 2021-08-24 15:39:21.275709 munge-1.2.1/README.md
--rw-r--r--   0        0        0     1404 2021-08-24 15:40:08.255727 munge-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      334 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/__init__.py
--rw-r--r--   0        0        0     2801 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/base.py
--rw-r--r--   0        0        0     1568 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/cli.py
--rw-r--r--   0        0        0     4865 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/click.py
--rw-r--r--   0        0        0     2261 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/codec/__init__.py
--rw-r--r--   0        0        0      105 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/codec/all.py
--rw-r--r--   0        0        0      620 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/codec/json.py
--rw-r--r--   0        0        0     1513 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/codec/mysql.py
--rw-r--r--   0        0        0      441 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/codec/toml.py
--rw-r--r--   0        0        0      622 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/codec/toml_toml.py
--rw-r--r--   0        0        0      693 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/codec/toml_tomlkit.py
--rw-r--r--   0        0        0      725 2021-08-24 15:39:21.279043 munge-1.2.1/src/munge/codec/yaml.py
--rw-r--r--   0        0        0     7040 2021-08-24 15:39:21.282376 munge-1.2.1/src/munge/config.py
--rw-r--r--   0        0        0     1041 2021-08-24 15:39:21.282376 munge-1.2.1/src/munge/util.py
--rw-r--r--   0        0        0     2291 2021-08-24 15:40:09.397194 munge-1.2.1/setup.py
--rw-r--r--   0        0        0     2260 2021-08-24 15:40:09.397691 munge-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2020-10-31 23:51:46.695682 munge-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1298 2023-06-30 19:14:41.516206 munge-1.3.0/README.md
+-rw-r--r--   0        0        0     1508 2023-06-30 19:23:12.782409 munge-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      334 2021-06-18 04:10:38.154803 munge-1.3.0/src/munge/__init__.py
+-rw-r--r--   0        0        0     2801 2021-06-18 04:10:38.154803 munge-1.3.0/src/munge/base.py
+-rw-r--r--   0        0        0     1568 2021-06-18 04:10:38.154803 munge-1.3.0/src/munge/cli.py
+-rw-r--r--   0        0        0     4865 2021-05-27 17:57:09.974960 munge-1.3.0/src/munge/click.py
+-rw-r--r--   0        0        0     2259 2023-06-30 18:39:14.840038 munge-1.3.0/src/munge/codec/__init__.py
+-rw-r--r--   0        0        0      105 2021-05-27 17:57:09.975960 munge-1.3.0/src/munge/codec/all.py
+-rw-r--r--   0        0        0      620 2021-06-18 04:10:38.155803 munge-1.3.0/src/munge/codec/json.py
+-rw-r--r--   0        0        0     1513 2021-05-29 02:39:50.744137 munge-1.3.0/src/munge/codec/mysql.py
+-rw-r--r--   0        0        0      441 2021-06-18 04:10:38.155803 munge-1.3.0/src/munge/codec/toml.py
+-rw-r--r--   0        0        0      621 2023-06-30 18:39:14.840038 munge-1.3.0/src/munge/codec/toml_toml.py
+-rw-r--r--   0        0        0      692 2023-06-30 18:39:14.840038 munge-1.3.0/src/munge/codec/toml_tomlkit.py
+-rw-r--r--   0        0        0      724 2023-06-30 18:39:14.840038 munge-1.3.0/src/munge/codec/yaml.py
+-rw-r--r--   0        0        0     7040 2021-05-29 02:39:50.744137 munge-1.3.0/src/munge/config.py
+-rw-r--r--   0        0        0     1041 2021-05-27 17:57:09.976960 munge-1.3.0/src/munge/util.py
+-rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 munge-1.3.0/PKG-INFO
```

### Comparing `munge-1.2.1/LICENSE.txt` & `munge-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `munge-1.2.1/README.md` & `munge-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # munge
 
 [![PyPI](https://img.shields.io/pypi/v/munge.svg?maxAge=3600)](https://pypi.python.org/pypi/munge)
 [![PyPI](https://img.shields.io/pypi/pyversions/munge.svg?maxAge=600)](https://pypi.python.org/pypi/munge)
 [![Tests](https://github.com/20c/munge/workflows/tests/badge.svg)](https://github.com/20c/munge)
-[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/20c/munge)](https://lgtm.com/projects/g/20c/munge/alerts/)
-[![Codecov](https://img.shields.io/codecov/c/github/20c/munge/master.svg?maxAge=3600)](https://codecov.io/github/20c/munge?branch=master)
+[![tests](https://github.com/20c/munge/actions/workflows/tests.yaml/badge.svg)](https://github.com/20c/munge/actions/workflows/tests.yaml)
+[![Codecov](https://img.shields.io/codecov/c/github/20c/munge/main.svg?maxAge=3600)](https://codecov.io/github/20c/munge?branch=main)
 
 data manipulation library and client
 
 ## Changes
 
-The current change log is available at <https://github.com/20c/munge/blob/master/CHANGELOG.md>
+The current change log is available at <https://github.com/20c/munge/blob/main/CHANGELOG.md>
 
 
 ## License
 
 Copyright 2015-2021 20C, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `munge-1.2.1/pyproject.toml` & `munge-1.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "munge"
-version = "1.2.1"
+version = "1.3.0"
 description = "data manipulation library and client"
 readme = "README.md"
 repository = "https://github.com/20c/munge/"
 authors = [ "20C <code@20c.com>",]
 license = "Apache-2.0"
-classifiers = [ "Topic :: Software Development", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.6", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9",]
+classifiers = [
+  "Topic :: Software Development",
+  "License :: OSI Approved :: Apache Software License",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+]
+
 [[tool.poetry.packages]]
 include = "munge"
 from = "src"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry.scripts]
 munge = "munge.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-requests = "^2.6"
+python = "^3.8"
+requests = ">=2.6"
 click = ">=5.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "*"
+# testing
+coverage = ">=5"
+pytest = ">=6"
+pytest-django = ">=3.8"
+pytest-filedata = "^0.4.0"
 pytest-cov = "*"
-codecov = "^2"
-coverage = "^5.5"
-tox = "^3.15"
-bandit = "^1"
-black = "^20.8b1"
-isort = "^5.7.0"
-flake8 = "^3"
-pre-commit = "^2"
-mypy = "^0.812"
-pyupgrade = "^2"
-ctl = "^1.0.0"
-jinja2 = "^2.11.2"
-tmpl = "^0.3.0"
-twine = "^3.3.0"
+tox = ">=3.20"
+tox-gh-actions = "^2.9.1"
+
+# linting
+black = ">=20"
+isort = ">=5.7"
+flake8 = ">=3.8"
+mypy = ">=0.950"
+pre-commit = ">=2.13"
+pyupgrade = ">=2.19"
+
+# docs
+markdown = "*"
+markdown-include = ">=0.5,<1"
+mkdocs = ">=1.2.3"
 
 [tool.poetry.extras]
 toml = [ "toml",]
 tomlkit = [ "tomlkit",]
 yaml = [ "PyYAML",]
 
 [tool.poetry.dependencies.PyYAML]
-version = "^5.1"
+version = ">=5.1"
 optional = true
 
 [tool.poetry.dependencies.toml]
-version = "^0.10.2"
+version = ">=0.10.2"
 optional = true
 
 [tool.poetry.dependencies.tomlkit]
-version = "^0.7.2"
+version = ">=0.7.2"
 optional = true
```

### Comparing `munge-1.2.1/src/munge/base.py` & `munge-1.3.0/src/munge/base.py`

 * *Files identical despite different names*

### Comparing `munge-1.2.1/src/munge/cli.py` & `munge-1.3.0/src/munge/cli.py`

 * *Files identical despite different names*

### Comparing `munge-1.2.1/src/munge/click.py` & `munge-1.3.0/src/munge/click.py`

 * *Files identical despite different names*

### Comparing `munge-1.2.1/src/munge/codec/__init__.py` & `munge-1.3.0/src/munge/codec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         raise ValueError(f"duplicate extension {str(dupe_exts)}")
 
     __codecs[exts] = cls
 
 
 # TODO - could take a type argument to get only codecs that can handle that data type
 def get_codecs():
-    """ Get all currently registered codecs. """
+    """Get all currently registered codecs."""
     return __codecs
 
 
 def list_codecs():
     return [ext[0] for ext in list(get_codecs().keys())]
```

### Comparing `munge-1.2.1/src/munge/codec/json.py` & `munge-1.3.0/src/munge/codec/json.py`

 * *Files identical despite different names*

### Comparing `munge-1.2.1/src/munge/codec/mysql.py` & `munge-1.3.0/src/munge/codec/mysql.py`

 * *Files identical despite different names*

### Comparing `munge-1.2.1/src/munge/codec/toml_toml.py` & `munge-1.3.0/src/munge/codec/toml_toml.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,10 +19,9 @@
 
         def dump(self, data, fobj, **kwargs):
             return toml.dump(data, fobj, **kwargs)
 
         def dumps(self, data):
             return toml.dumps(data)
 
-
 except ImportError:
     pass
```

### Comparing `munge-1.2.1/src/munge/codec/toml_tomlkit.py` & `munge-1.3.0/src/munge/codec/toml_tomlkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,10 +20,9 @@
 
         def dump(self, data, fobj, **kwargs):
             return fobj.write(self.dumps(data, **kwargs))
 
         def dumps(self, data, **kwargs):
             return tomlkit.dumps(data)
 
-
 except ImportError:
     pass
```

### Comparing `munge-1.2.1/src/munge/codec/yaml.py` & `munge-1.3.0/src/munge/codec/yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,9 @@
             return fobj.write(
                 yaml.safe_dump(data, default_flow_style=False, sort_keys=False)
             )
 
         def dumps(self, data):
             return yaml.safe_dump(data, default_flow_style=False, sort_keys=False)
 
-
 except ImportError:
     pass
```

### Comparing `munge-1.2.1/src/munge/config.py` & `munge-1.3.0/src/munge/config.py`

 * *Files identical despite different names*

### Comparing `munge-1.2.1/src/munge/util.py` & `munge-1.3.0/src/munge/util.py`

 * *Files identical despite different names*

### Comparing `munge-1.2.1/PKG-INFO` & `munge-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: munge
-Version: 1.2.1
+Version: 1.3.0
 Summary: data manipulation library and client
 Home-page: https://github.com/20c/munge/
 License: Apache-2.0
 Author: 20C
 Author-email: code@20c.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Provides-Extra: toml
 Provides-Extra: tomlkit
 Provides-Extra: yaml
-Requires-Dist: PyYAML (>=5.1,<6.0); extra == "yaml"
+Requires-Dist: PyYAML (>=5.1) ; extra == "yaml"
 Requires-Dist: click (>=5.1)
-Requires-Dist: requests (>=2.6,<3.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0); extra == "toml"
-Requires-Dist: tomlkit (>=0.7.2,<0.8.0); extra == "tomlkit"
+Requires-Dist: requests (>=2.6)
+Requires-Dist: toml (>=0.10.2) ; extra == "toml"
+Requires-Dist: tomlkit (>=0.7.2) ; extra == "tomlkit"
 Project-URL: Repository, https://github.com/20c/munge/
 Description-Content-Type: text/markdown
 
 # munge
 
 [![PyPI](https://img.shields.io/pypi/v/munge.svg?maxAge=3600)](https://pypi.python.org/pypi/munge)
 [![PyPI](https://img.shields.io/pypi/pyversions/munge.svg?maxAge=600)](https://pypi.python.org/pypi/munge)
 [![Tests](https://github.com/20c/munge/workflows/tests/badge.svg)](https://github.com/20c/munge)
-[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/20c/munge)](https://lgtm.com/projects/g/20c/munge/alerts/)
-[![Codecov](https://img.shields.io/codecov/c/github/20c/munge/master.svg?maxAge=3600)](https://codecov.io/github/20c/munge?branch=master)
+[![tests](https://github.com/20c/munge/actions/workflows/tests.yaml/badge.svg)](https://github.com/20c/munge/actions/workflows/tests.yaml)
+[![Codecov](https://img.shields.io/codecov/c/github/20c/munge/main.svg?maxAge=3600)](https://codecov.io/github/20c/munge?branch=main)
 
 data manipulation library and client
 
 ## Changes
 
-The current change log is available at <https://github.com/20c/munge/blob/master/CHANGELOG.md>
+The current change log is available at <https://github.com/20c/munge/blob/main/CHANGELOG.md>
 
 
 ## License
 
 Copyright 2015-2021 20C, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

