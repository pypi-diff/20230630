# Comparing `tmp/mypy-boto3-mediaconvert-1.26.84.tar.gz` & `tmp/mypy-boto3-mediaconvert-1.26.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconvert-1.26.84.tar", last modified: Fri Mar  3 20:27:52 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconvert-1.26.98.tar", last modified: Thu Mar 23 19:33:06 2023, max compression
```

## Comparing `mypy-boto3-mediaconvert-1.26.84.tar` & `mypy-boto3-mediaconvert-1.26.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.690264 mypy-boto3-mediaconvert-1.26.84/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-03 20:27:29.000000 mypy-boto3-mediaconvert-1.26.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32977 2023-03-03 20:27:52.686264 mypy-boto3-mediaconvert-1.26.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31470 2023-03-03 20:27:29.000000 mypy-boto3-mediaconvert-1.26.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.678264 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-03 20:27:29.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-03 20:27:29.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-03 20:27:29.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-03-03 20:27:30.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-03-03 20:27:30.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54737 2023-03-03 20:27:31.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    54735 2023-03-03 20:27:30.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-03-03 20:27:30.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-03-03 20:27:30.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:29.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   102152 2023-03-03 20:27:33.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102127 2023-03-03 20:27:32.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-03 20:27:29.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.686264 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32977 2023-03-03 20:27:52.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-03 20:27:52.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:27:52.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:27:52.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-03 20:27:52.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-03 20:27:52.000000 mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 20:27:52.690264 mypy-boto3-mediaconvert-1.26.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-03 20:27:29.000000 mypy-boto3-mediaconvert-1.26.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.811666 mypy-boto3-mediaconvert-1.26.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32943 2023-03-23 19:33:06.803666 mypy-boto3-mediaconvert-1.26.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31436 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.795666 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54757 2023-03-23 19:32:21.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54755 2023-03-23 19:32:21.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   102152 2023-03-23 19:32:24.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102127 2023-03-23 19:32:23.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.803666 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32943 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:06.811666 mypy-boto3-mediaconvert-1.26.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/setup.py
```

### Comparing `mypy-boto3-mediaconvert-1.26.84/LICENSE` & `mypy-boto3-mediaconvert-1.26.98/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-mediaconvert-1.26.84/PKG-INFO` & `mypy-boto3-mediaconvert-1.26.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.26.84
-Summary: Type annotations for boto3.MediaConvert 1.26.84 service generated with mypy-boto3-builder 7.12.5
+Version: 1.26.98
+Summary: Type annotations for boto3.MediaConvert 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -977,42 +977,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-mediaconvert-1.26.84/README.md` & `mypy-boto3-mediaconvert-1.26.98/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -945,42 +945,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/__init__.py` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/__init__.pyi` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/__main__.py` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConvert 1.26.84\nVersion:         1.26.84\nBuilder"
-        " version: 7.12.5\nDocs:           "
+        "Type annotations for boto3.MediaConvert 1.26.98\nVersion:         1.26.98\nBuilder"
+        " version: 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.84")
+    print("1.26.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/client.py` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/client.pyi` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/literals.py` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1448,14 +1448,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/literals.pyi` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1446,14 +1446,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/paginator.py` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/paginator.pyi` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/type_defs.py` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert/type_defs.pyi` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/PKG-INFO` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.26.84
-Summary: Type annotations for boto3.MediaConvert 1.26.84 service generated with mypy-boto3-builder 7.12.5
+Version: 1.26.98
+Summary: Type annotations for boto3.MediaConvert 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -977,42 +977,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-mediaconvert-1.26.84/mypy_boto3_mediaconvert.egg-info/SOURCES.txt` & `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.84/setup.py` & `mypy-boto3-mediaconvert-1.26.98/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-mediaconvert.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconvert",
-    version="1.26.84",
+    version="1.26.98",
     packages=["mypy_boto3_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConvert 1.26.84 service generated with mypy-boto3-builder"
-        " 7.12.5"
+        "Type annotations for boto3.MediaConvert 1.26.98 service generated with mypy-boto3-builder"
+        " 7.14.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

