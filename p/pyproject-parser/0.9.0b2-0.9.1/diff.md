# Comparing `tmp/pyproject-parser-0.9.0b2.tar.gz` & `tmp/pyproject-parser-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-parser-0.9.0b2.tar", last modified: Tue Apr 25 21:22:24 2023, max compression
+gzip compressed data, was "pyproject-parser-0.9.1.tar", last modified: Fri Jun 30 10:52:47 2023, max compression
```

## Comparing `pyproject-parser-0.9.0b2.tar` & `pyproject-parser-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8395 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5474 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.223481 pyproject-parser-0.9.0b2/pyproject_parser/
--rw-r--r--   0 runner    (1001) docker     (122)    10945 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/pyproject_parser/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/cli/_json_encoders.py
--rw-r--r--   0 runner    (1001) docker     (122)    36419 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/type_hints.py
--rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/pyproject_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.223481 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8395 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-25 21:22:24.000000 pyproject-parser-0.9.0b2/pyproject_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 21:22:24.227481 pyproject-parser-0.9.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    10428 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    15102 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_cli_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    16879 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_dumping.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_pyproject_class.py
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-04-25 21:21:48.000000 pyproject-parser-0.9.0b2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 10:52:47.413567 pyproject-parser-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8391 2023-06-30 10:52:47.413567 pyproject-parser-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 10:52:47.409567 pyproject-parser-0.9.1/pyproject_parser/
+-rw-r--r--   0 runner    (1001) docker     (122)    10943 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 10:52:47.409567 pyproject-parser-0.9.1/pyproject_parser/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/cli/_json_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36419 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/pyproject_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 10:52:47.409567 pyproject-parser-0.9.1/pyproject_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8391 2023-06-30 10:52:47.000000 pyproject-parser-0.9.1/pyproject_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-30 10:52:47.000000 pyproject-parser-0.9.1/pyproject_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 10:52:47.000000 pyproject-parser-0.9.1/pyproject_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-06-30 10:52:47.000000 pyproject-parser-0.9.1/pyproject_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 10:52:47.000000 pyproject-parser-0.9.1/pyproject_parser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-06-30 10:52:47.000000 pyproject-parser-0.9.1/pyproject_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-30 10:52:47.000000 pyproject-parser-0.9.1/pyproject_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-06-30 10:52:47.417567 pyproject-parser-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 10:52:47.413567 pyproject-parser-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    10428 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15102 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/tests/test_cli_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16879 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/tests/test_dumping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/tests/test_pyproject_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-06-30 10:52:09.000000 pyproject-parser-0.9.1/tests/test_utils.py
```

### Comparing `pyproject-parser-0.9.0b2/LICENSE` & `pyproject-parser-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/PKG-INFO` & `pyproject-parser-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-parser
-Version: 0.9.0b2
+Version: 0.9.1
 Summary: Parser for 'pyproject.toml'
 Home-page: https://github.com/repo-helper/pyproject-parser
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -156,15 +156,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.1
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.9.0b2/README.rst` & `pyproject-parser-0.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.1
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.9.0b2/pyproject.toml` & `pyproject-parser-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyproject-parser"
-version = "0.9.0b2"
+version = "0.9.1"
 description = "Parser for 'pyproject.toml'"
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "metadata", "packaging", "pep518", "pep621", "pyproject", "toml",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser/__init__.py` & `pyproject-parser-0.9.1/pyproject_parser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 		_PyProjectAsTomlDict
 		)
 from pyproject_parser.utils import _load_toml
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.9.0b2"
+__version__: str = "0.9.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["PyProject", "PyProjectTomlEncoder", "_PP"]
 
 _PP = TypeVar("_PP", bound="PyProject")
```

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser/__main__.py` & `pyproject-parser-0.9.1/pyproject_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser/classes.py` & `pyproject-parser-0.9.1/pyproject_parser/classes.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser/cli/__init__.py` & `pyproject-parser-0.9.1/pyproject_parser/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser/cli/_json_encoders.py` & `pyproject-parser-0.9.1/pyproject_parser/cli/_json_encoders.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser/parsers.py` & `pyproject-parser-0.9.1/pyproject_parser/parsers.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser/type_hints.py` & `pyproject-parser-0.9.1/pyproject_parser/type_hints.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser/utils.py` & `pyproject-parser-0.9.1/pyproject_parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser.egg-info/PKG-INFO` & `pyproject-parser-0.9.1/pyproject_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-parser
-Version: 0.9.0b2
+Version: 0.9.1
 Summary: Parser for 'pyproject.toml'
 Home-page: https://github.com/repo-helper/pyproject-parser
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -156,15 +156,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.1
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.9.0b2/pyproject_parser.egg-info/SOURCES.txt` & `pyproject-parser-0.9.1/pyproject_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/setup.cfg` & `pyproject-parser-0.9.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyproject-parser
-version = 0.9.0b2
+version = 0.9.1
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = pep518, pep621, pyproject, toml, metadata, packaging
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
```

### Comparing `pyproject-parser-0.9.0b2/setup.py` & `pyproject-parser-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/tests/test_classes.py` & `pyproject-parser-0.9.1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/tests/test_cli.py` & `pyproject-parser-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/tests/test_cli_module.py` & `pyproject-parser-0.9.1/tests/test_cli_module.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/tests/test_config.py` & `pyproject-parser-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/tests/test_dumping.py` & `pyproject-parser-0.9.1/tests/test_dumping.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/tests/test_pyproject_class.py` & `pyproject-parser-0.9.1/tests/test_pyproject_class.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.9.0b2/tests/test_utils.py` & `pyproject-parser-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

