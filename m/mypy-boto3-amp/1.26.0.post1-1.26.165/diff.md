# Comparing `tmp/mypy-boto3-amp-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-amp-1.26.165.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amp-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:01 2022, max compression
+gzip compressed data, was "mypy-boto3-amp-1.26.165.tar", last modified: Fri Jun 30 19:48:24 2023, max compression
```

## Comparing `mypy-boto3-amp-1.26.0.post1.tar` & `mypy-boto3-amp-1.26.165.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:01.388824 mypy-boto3-amp-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15931 2022-11-01 21:43:01.384824 mypy-boto3-amp-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14492 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:01.380824 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17087 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    17055 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8309 2022-11-01 21:30:08.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8307 2022-11-01 21:30:08.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3020 2022-11-01 21:30:08.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    22713 2022-11-01 21:30:08.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22668 2022-11-01 21:30:08.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-11-01 21:30:08.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-11-01 21:30:08.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:01.384824 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15931 2022-11-01 21:43:01.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-01 21:43:01.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:01.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:01.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:01.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:43:01.000000 mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:01.388824 mypy-boto3-amp-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-11-01 21:30:07.000000 mypy-boto3-amp-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:48:24.133283 mypy-boto3-amp-1.26.165/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-06-30 19:48:24.125282 mypy-boto3-amp-1.26.165/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:48:24.125282 mypy-boto3-amp-1.26.165/mypy_boto3_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-30 19:47:18.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22713 2023-06-30 19:47:18.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-06-30 19:47:18.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:48:24.125282 mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-06-30 19:48:23.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-30 19:48:23.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:48:23.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:48:23.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 19:48:23.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 19:48:23.000000 mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:48:24.133283 mypy-boto3-amp-1.26.165/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-30 19:47:17.000000 mypy-boto3-amp-1.26.165/setup.py
```

### Comparing `mypy-boto3-amp-1.26.0.post1/LICENSE` & `mypy-boto3-amp-1.26.165/LICENSE`

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

### Comparing `mypy-boto3-amp-1.26.0.post1/PKG-INFO` & `mypy-boto3-amp-1.26.165/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amp
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.PrometheusService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.165
+Summary: Type annotations for boto3.PrometheusService 1.26.165 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-amp"></a>
 
 # mypy-boto3-amp
 
 [![PyPI - mypy-boto3-amp](https://img.shields.io/pypi/v/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amp?color=blue)](https://pypistats.org/packages/mypy-boto3-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PrometheusService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[boto3.PrometheusService 1.26.165](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-amp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,42 +416,42 @@
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

### Comparing `mypy-boto3-amp-1.26.0.post1/README.md` & `mypy-boto3-amp-1.26.165/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-amp"></a>
 
 # mypy-boto3-amp
 
 [![PyPI - mypy-boto3-amp](https://img.shields.io/pypi/v/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amp?color=blue)](https://pypistats.org/packages/mypy-boto3-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PrometheusService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[boto3.PrometheusService 1.26.165](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-amp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -384,42 +384,42 @@
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

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/__init__.py` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/__init__.pyi` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/__main__.py` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PrometheusService 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.PrometheusService 1.26.165\nVersion:         1.26.165\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.165")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/client.py` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,41 +99,41 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#close)
         """
 
     def create_alert_manager_definition(
         self,
         *,
-        data: Union[str, bytes, IO[Any], StreamingBody],
         workspaceId: str,
+        data: Union[str, bytes, IO[Any], StreamingBody],
         clientToken: str = ...
     ) -> CreateAlertManagerDefinitionResponseTypeDef:
         """
         Create an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_alert_manager_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#create_alert_manager_definition)
         """
 
     def create_logging_configuration(
-        self, *, logGroupArn: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, logGroupArn: str, clientToken: str = ...
     ) -> CreateLoggingConfigurationResponseTypeDef:
         """
         Create logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#create_logging_configuration)
         """
 
     def create_rule_groups_namespace(
         self,
         *,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        name: str,
         workspaceId: str,
+        name: str,
+        data: Union[str, bytes, IO[Any], StreamingBody],
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleGroupsNamespaceResponseTypeDef:
         """
         Create a rule group namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)
@@ -167,15 +167,15 @@
         Delete logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#delete_logging_configuration)
         """
 
     def delete_rule_groups_namespace(
-        self, *, name: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, name: str, clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_rule_groups_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#delete_rule_groups_namespace)
         """
@@ -207,15 +207,15 @@
         Describes logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#describe_logging_configuration)
         """
 
     def describe_rule_groups_namespace(
-        self, *, name: str, workspaceId: str
+        self, *, workspaceId: str, name: str
     ) -> DescribeRuleGroupsNamespaceResponseTypeDef:
         """
         Describe a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_rule_groups_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#describe_rule_groups_namespace)
         """
@@ -239,15 +239,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#generate_presigned_url)
         """
 
     def list_rule_groups_namespaces(
-        self, *, workspaceId: str, maxResults: int = ..., name: str = ..., nextToken: str = ...
+        self, *, workspaceId: str, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListRuleGroupsNamespacesResponseTypeDef:
         """
         Lists rule groups namespaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_rule_groups_namespaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#list_rule_groups_namespaces)
         """
@@ -257,43 +257,43 @@
         Lists the tags you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#list_tags_for_resource)
         """
 
     def list_workspaces(
-        self, *, alias: str = ..., maxResults: int = ..., nextToken: str = ...
+        self, *, nextToken: str = ..., alias: str = ..., maxResults: int = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Lists all AMP workspaces, including workspaces being created or deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#list_workspaces)
         """
 
     def put_alert_manager_definition(
         self,
         *,
-        data: Union[str, bytes, IO[Any], StreamingBody],
         workspaceId: str,
+        data: Union[str, bytes, IO[Any], StreamingBody],
         clientToken: str = ...
     ) -> PutAlertManagerDefinitionResponseTypeDef:
         """
         Update an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_alert_manager_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#put_alert_manager_definition)
         """
 
     def put_rule_groups_namespace(
         self,
         *,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        name: str,
         workspaceId: str,
+        name: str,
+        data: Union[str, bytes, IO[Any], StreamingBody],
         clientToken: str = ...
     ) -> PutRuleGroupsNamespaceResponseTypeDef:
         """
         Update a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_rule_groups_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#put_rule_groups_namespace)
@@ -312,15 +312,15 @@
         Deletes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#untag_resource)
         """
 
     def update_logging_configuration(
-        self, *, logGroupArn: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, logGroupArn: str, clientToken: str = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Update logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#update_logging_configuration)
         """
```

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/client.pyi` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -92,39 +92,39 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#close)
         """
     def create_alert_manager_definition(
         self,
         *,
-        data: Union[str, bytes, IO[Any], StreamingBody],
         workspaceId: str,
+        data: Union[str, bytes, IO[Any], StreamingBody],
         clientToken: str = ...
     ) -> CreateAlertManagerDefinitionResponseTypeDef:
         """
         Create an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_alert_manager_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#create_alert_manager_definition)
         """
     def create_logging_configuration(
-        self, *, logGroupArn: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, logGroupArn: str, clientToken: str = ...
     ) -> CreateLoggingConfigurationResponseTypeDef:
         """
         Create logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#create_logging_configuration)
         """
     def create_rule_groups_namespace(
         self,
         *,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        name: str,
         workspaceId: str,
+        name: str,
+        data: Union[str, bytes, IO[Any], StreamingBody],
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleGroupsNamespaceResponseTypeDef:
         """
         Create a rule group namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)
@@ -154,15 +154,15 @@
         """
         Delete logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#delete_logging_configuration)
         """
     def delete_rule_groups_namespace(
-        self, *, name: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, name: str, clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_rule_groups_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#delete_rule_groups_namespace)
         """
@@ -190,15 +190,15 @@
         """
         Describes logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#describe_logging_configuration)
         """
     def describe_rule_groups_namespace(
-        self, *, name: str, workspaceId: str
+        self, *, workspaceId: str, name: str
     ) -> DescribeRuleGroupsNamespaceResponseTypeDef:
         """
         Describe a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_rule_groups_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#describe_rule_groups_namespace)
         """
@@ -219,15 +219,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#generate_presigned_url)
         """
     def list_rule_groups_namespaces(
-        self, *, workspaceId: str, maxResults: int = ..., name: str = ..., nextToken: str = ...
+        self, *, workspaceId: str, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListRuleGroupsNamespacesResponseTypeDef:
         """
         Lists rule groups namespaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_rule_groups_namespaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#list_rule_groups_namespaces)
         """
@@ -235,41 +235,41 @@
         """
         Lists the tags you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#list_tags_for_resource)
         """
     def list_workspaces(
-        self, *, alias: str = ..., maxResults: int = ..., nextToken: str = ...
+        self, *, nextToken: str = ..., alias: str = ..., maxResults: int = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Lists all AMP workspaces, including workspaces being created or deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#list_workspaces)
         """
     def put_alert_manager_definition(
         self,
         *,
-        data: Union[str, bytes, IO[Any], StreamingBody],
         workspaceId: str,
+        data: Union[str, bytes, IO[Any], StreamingBody],
         clientToken: str = ...
     ) -> PutAlertManagerDefinitionResponseTypeDef:
         """
         Update an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_alert_manager_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#put_alert_manager_definition)
         """
     def put_rule_groups_namespace(
         self,
         *,
-        data: Union[str, bytes, IO[Any], StreamingBody],
-        name: str,
         workspaceId: str,
+        name: str,
+        data: Union[str, bytes, IO[Any], StreamingBody],
         clientToken: str = ...
     ) -> PutRuleGroupsNamespaceResponseTypeDef:
         """
         Update a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_rule_groups_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#put_rule_groups_namespace)
@@ -285,15 +285,15 @@
         """
         Deletes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#untag_resource)
         """
     def update_logging_configuration(
-        self, *, logGroupArn: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, logGroupArn: str, clientToken: str = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Update logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/client/#update_logging_configuration)
         """
```

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/literals.py` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlertManagerDefinitionStatusCodeType",
     "ListRuleGroupsNamespacesPaginatorName",
     "ListWorkspacesPaginatorName",
     "LoggingConfigurationStatusCodeType",
     "RuleGroupsNamespaceStatusCodeType",
     "WorkspaceActiveWaiterName",
@@ -32,15 +31,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AlertManagerDefinitionStatusCodeType = Literal[
     "ACTIVE", "CREATING", "CREATION_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
 ListRuleGroupsNamespacesPaginatorName = Literal["list_rule_groups_namespaces"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 LoggingConfigurationStatusCodeType = Literal[
     "ACTIVE", "CREATING", "CREATION_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
@@ -63,23 +61,25 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -89,30 +89,35 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -138,14 +143,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -190,51 +196,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
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
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -247,14 +259,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -266,28 +279,35 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -296,14 +316,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -314,55 +335,64 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -384,17 +414,21 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_rule_groups_namespaces", "list_workspaces"]
 WaiterName = Literal["workspace_active", "workspace_deleted"]
 RegionName = Literal[
     "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
+    "eu-west-3",
+    "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/literals.pyi` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AlertManagerDefinitionStatusCodeType",
     "ListRuleGroupsNamespacesPaginatorName",
     "ListWorkspacesPaginatorName",
     "LoggingConfigurationStatusCodeType",
     "RuleGroupsNamespaceStatusCodeType",
     "WorkspaceActiveWaiterName",
@@ -31,14 +32,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AlertManagerDefinitionStatusCodeType = Literal[
     "ACTIVE", "CREATING", "CREATION_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
 ListRuleGroupsNamespacesPaginatorName = Literal["list_rule_groups_namespaces"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 LoggingConfigurationStatusCodeType = Literal[
     "ACTIVE", "CREATING", "CREATION_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
@@ -61,23 +63,25 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -87,30 +91,35 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -136,14 +145,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -188,51 +198,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
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
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -245,14 +261,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -264,28 +281,35 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -294,14 +318,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -312,55 +337,64 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -382,17 +416,21 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_rule_groups_namespaces", "list_workspaces"]
 WaiterName = Literal["workspace_active", "workspace_deleted"]
 RegionName = Literal[
     "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
+    "eu-west-3",
+    "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/paginator.py` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/paginator.pyi` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/type_defs.py` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/type_defs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -106,16 +106,16 @@
 ):
     pass
 
 
 _RequiredCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef",
     {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
         "workspaceId": str,
+        "data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -140,16 +140,16 @@
         "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
     {
-        "logGroupArn": str,
         "workspaceId": str,
+        "logGroupArn": str,
     },
 )
 _OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -184,17 +184,17 @@
 ):
     pass
 
 
 _RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-        "name": str,
         "workspaceId": str,
+        "name": str,
+        "data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
         "tags": Mapping[str, str],
@@ -291,16 +291,16 @@
 ):
     pass
 
 
 _RequiredDeleteRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "name": str,
         "workspaceId": str,
+        "name": str,
     },
 )
 _OptionalDeleteRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -349,16 +349,16 @@
         "workspaceId": str,
     },
 )
 
 DescribeRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "name": str,
         "workspaceId": str,
+        "name": str,
     },
 )
 
 DescribeWorkspaceRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -389,17 +389,17 @@
     {
         "workspaceId": str,
     },
 )
 _OptionalListRuleGroupsNamespacesRequestRequestTypeDef = TypedDict(
     "_OptionalListRuleGroupsNamespacesRequestRequestTypeDef",
     {
-        "maxResults": int,
         "name": str,
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
 class ListRuleGroupsNamespacesRequestRequestTypeDef(
     _RequiredListRuleGroupsNamespacesRequestRequestTypeDef,
@@ -414,26 +414,26 @@
         "resourceArn": str,
     },
 )
 
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
+        "nextToken": str,
         "alias": str,
         "maxResults": int,
-        "nextToken": str,
     },
     total=False,
 )
 
 _RequiredPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredPutAlertManagerDefinitionRequestRequestTypeDef",
     {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
         "workspaceId": str,
+        "data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalPutAlertManagerDefinitionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -447,17 +447,17 @@
 ):
     pass
 
 
 _RequiredPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-        "name": str,
         "workspaceId": str,
+        "name": str,
+        "data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -487,16 +487,16 @@
         "tagKeys": Sequence[str],
     },
 )
 
 _RequiredUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggingConfigurationRequestRequestTypeDef",
     {
-        "logGroupArn": str,
         "workspaceId": str,
+        "logGroupArn": str,
     },
 )
 _OptionalUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -533,18 +533,18 @@
 ):
     pass
 
 
 AlertManagerDefinitionDescriptionTypeDef = TypedDict(
     "AlertManagerDefinitionDescriptionTypeDef",
     {
-        "createdAt": datetime,
+        "status": AlertManagerDefinitionStatusTypeDef,
         "data": bytes,
+        "createdAt": datetime,
         "modifiedAt": datetime,
-        "status": AlertManagerDefinitionStatusTypeDef,
     },
 )
 
 CreateAlertManagerDefinitionResponseTypeDef = TypedDict(
     "CreateAlertManagerDefinitionResponseTypeDef",
     {
         "status": AlertManagerDefinitionStatusTypeDef,
@@ -582,61 +582,61 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingConfigurationMetadataTypeDef = TypedDict(
     "LoggingConfigurationMetadataTypeDef",
     {
-        "createdAt": datetime,
-        "logGroupArn": str,
-        "modifiedAt": datetime,
         "status": LoggingConfigurationStatusTypeDef,
         "workspace": str,
+        "logGroupArn": str,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 
 UpdateLoggingConfigurationResponseTypeDef = TypedDict(
     "UpdateLoggingConfigurationResponseTypeDef",
     {
         "status": LoggingConfigurationStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupsNamespaceResponseTypeDef = TypedDict(
     "CreateRuleGroupsNamespaceResponseTypeDef",
     {
-        "arn": str,
         "name": str,
+        "arn": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRuleGroupsNamespaceResponseTypeDef = TypedDict(
     "PutRuleGroupsNamespaceResponseTypeDef",
     {
-        "arn": str,
         "name": str,
+        "arn": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRuleGroupsNamespaceDescriptionTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceDescriptionTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "data": bytes,
-        "modifiedAt": datetime,
         "name": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
+        "data": bytes,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 _OptionalRuleGroupsNamespaceDescriptionTypeDef = TypedDict(
     "_OptionalRuleGroupsNamespaceDescriptionTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -650,18 +650,18 @@
     pass
 
 
 _RequiredRuleGroupsNamespaceSummaryTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceSummaryTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "modifiedAt": datetime,
         "name": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 _OptionalRuleGroupsNamespaceSummaryTypeDef = TypedDict(
     "_OptionalRuleGroupsNamespaceSummaryTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -674,29 +674,29 @@
 ):
     pass
 
 
 CreateWorkspaceResponseTypeDef = TypedDict(
     "CreateWorkspaceResponseTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
         "status": WorkspaceStatusTypeDef,
         "tags": Dict[str, str],
-        "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
-        "createdAt": datetime,
         "status": WorkspaceStatusTypeDef,
-        "workspaceId": str,
+        "createdAt": datetime,
     },
 )
 _OptionalWorkspaceDescriptionTypeDef = TypedDict(
     "_OptionalWorkspaceDescriptionTypeDef",
     {
         "alias": str,
         "prometheusEndpoint": str,
@@ -711,18 +711,18 @@
 ):
     pass
 
 
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
-        "createdAt": datetime,
         "status": WorkspaceStatusTypeDef,
-        "workspaceId": str,
+        "createdAt": datetime,
     },
 )
 _OptionalWorkspaceSummaryTypeDef = TypedDict(
     "_OptionalWorkspaceSummaryTypeDef",
     {
         "alias": str,
         "tags": Dict[str, str],
@@ -834,16 +834,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRuleGroupsNamespacesResponseTypeDef = TypedDict(
     "ListRuleGroupsNamespacesResponseTypeDef",
     {
-        "nextToken": str,
         "ruleGroupsNamespaces": List[RuleGroupsNamespaceSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceResponseTypeDef = TypedDict(
     "DescribeWorkspaceResponseTypeDef",
     {
@@ -851,12 +851,12 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
-        "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/type_defs.pyi` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/type_defs.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -103,16 +103,16 @@
     _RequiredAlertManagerDefinitionStatusTypeDef, _OptionalAlertManagerDefinitionStatusTypeDef
 ):
     pass
 
 _RequiredCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef",
     {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
         "workspaceId": str,
+        "data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -135,16 +135,16 @@
         "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
     {
-        "logGroupArn": str,
         "workspaceId": str,
+        "logGroupArn": str,
     },
 )
 _OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -175,17 +175,17 @@
     _RequiredLoggingConfigurationStatusTypeDef, _OptionalLoggingConfigurationStatusTypeDef
 ):
     pass
 
 _RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-        "name": str,
         "workspaceId": str,
+        "name": str,
+        "data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
         "tags": Mapping[str, str],
@@ -274,16 +274,16 @@
     _OptionalDeleteLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 _RequiredDeleteRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "name": str,
         "workspaceId": str,
+        "name": str,
     },
 )
 _OptionalDeleteRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -328,16 +328,16 @@
         "workspaceId": str,
     },
 )
 
 DescribeRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "name": str,
         "workspaceId": str,
+        "name": str,
     },
 )
 
 DescribeWorkspaceRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -368,17 +368,17 @@
     {
         "workspaceId": str,
     },
 )
 _OptionalListRuleGroupsNamespacesRequestRequestTypeDef = TypedDict(
     "_OptionalListRuleGroupsNamespacesRequestRequestTypeDef",
     {
-        "maxResults": int,
         "name": str,
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 class ListRuleGroupsNamespacesRequestRequestTypeDef(
     _RequiredListRuleGroupsNamespacesRequestRequestTypeDef,
     _OptionalListRuleGroupsNamespacesRequestRequestTypeDef,
@@ -391,26 +391,26 @@
         "resourceArn": str,
     },
 )
 
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
+        "nextToken": str,
         "alias": str,
         "maxResults": int,
-        "nextToken": str,
     },
     total=False,
 )
 
 _RequiredPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredPutAlertManagerDefinitionRequestRequestTypeDef",
     {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
         "workspaceId": str,
+        "data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalPutAlertManagerDefinitionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -422,17 +422,17 @@
     _OptionalPutAlertManagerDefinitionRequestRequestTypeDef,
 ):
     pass
 
 _RequiredPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "data": Union[str, bytes, IO[Any], StreamingBody],
-        "name": str,
         "workspaceId": str,
+        "name": str,
+        "data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 _OptionalPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -460,16 +460,16 @@
         "tagKeys": Sequence[str],
     },
 )
 
 _RequiredUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggingConfigurationRequestRequestTypeDef",
     {
-        "logGroupArn": str,
         "workspaceId": str,
+        "logGroupArn": str,
     },
 )
 _OptionalUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -502,18 +502,18 @@
     _OptionalUpdateWorkspaceAliasRequestRequestTypeDef,
 ):
     pass
 
 AlertManagerDefinitionDescriptionTypeDef = TypedDict(
     "AlertManagerDefinitionDescriptionTypeDef",
     {
-        "createdAt": datetime,
+        "status": AlertManagerDefinitionStatusTypeDef,
         "data": bytes,
+        "createdAt": datetime,
         "modifiedAt": datetime,
-        "status": AlertManagerDefinitionStatusTypeDef,
     },
 )
 
 CreateAlertManagerDefinitionResponseTypeDef = TypedDict(
     "CreateAlertManagerDefinitionResponseTypeDef",
     {
         "status": AlertManagerDefinitionStatusTypeDef,
@@ -551,61 +551,61 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingConfigurationMetadataTypeDef = TypedDict(
     "LoggingConfigurationMetadataTypeDef",
     {
-        "createdAt": datetime,
-        "logGroupArn": str,
-        "modifiedAt": datetime,
         "status": LoggingConfigurationStatusTypeDef,
         "workspace": str,
+        "logGroupArn": str,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 
 UpdateLoggingConfigurationResponseTypeDef = TypedDict(
     "UpdateLoggingConfigurationResponseTypeDef",
     {
         "status": LoggingConfigurationStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupsNamespaceResponseTypeDef = TypedDict(
     "CreateRuleGroupsNamespaceResponseTypeDef",
     {
-        "arn": str,
         "name": str,
+        "arn": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRuleGroupsNamespaceResponseTypeDef = TypedDict(
     "PutRuleGroupsNamespaceResponseTypeDef",
     {
-        "arn": str,
         "name": str,
+        "arn": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRuleGroupsNamespaceDescriptionTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceDescriptionTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "data": bytes,
-        "modifiedAt": datetime,
         "name": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
+        "data": bytes,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 _OptionalRuleGroupsNamespaceDescriptionTypeDef = TypedDict(
     "_OptionalRuleGroupsNamespaceDescriptionTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -617,18 +617,18 @@
 ):
     pass
 
 _RequiredRuleGroupsNamespaceSummaryTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceSummaryTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "modifiedAt": datetime,
         "name": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 _OptionalRuleGroupsNamespaceSummaryTypeDef = TypedDict(
     "_OptionalRuleGroupsNamespaceSummaryTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -639,29 +639,29 @@
     _RequiredRuleGroupsNamespaceSummaryTypeDef, _OptionalRuleGroupsNamespaceSummaryTypeDef
 ):
     pass
 
 CreateWorkspaceResponseTypeDef = TypedDict(
     "CreateWorkspaceResponseTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
         "status": WorkspaceStatusTypeDef,
         "tags": Dict[str, str],
-        "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
-        "createdAt": datetime,
         "status": WorkspaceStatusTypeDef,
-        "workspaceId": str,
+        "createdAt": datetime,
     },
 )
 _OptionalWorkspaceDescriptionTypeDef = TypedDict(
     "_OptionalWorkspaceDescriptionTypeDef",
     {
         "alias": str,
         "prometheusEndpoint": str,
@@ -674,18 +674,18 @@
     _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
 ):
     pass
 
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
-        "createdAt": datetime,
         "status": WorkspaceStatusTypeDef,
-        "workspaceId": str,
+        "createdAt": datetime,
     },
 )
 _OptionalWorkspaceSummaryTypeDef = TypedDict(
     "_OptionalWorkspaceSummaryTypeDef",
     {
         "alias": str,
         "tags": Dict[str, str],
@@ -789,16 +789,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRuleGroupsNamespacesResponseTypeDef = TypedDict(
     "ListRuleGroupsNamespacesResponseTypeDef",
     {
-        "nextToken": str,
         "ruleGroupsNamespaces": List[RuleGroupsNamespaceSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceResponseTypeDef = TypedDict(
     "DescribeWorkspaceResponseTypeDef",
     {
@@ -806,12 +806,12 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
-        "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/waiter.py` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp/waiter.pyi` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/PKG-INFO` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amp
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.PrometheusService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.165
+Summary: Type annotations for boto3.PrometheusService 1.26.165 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-amp"></a>
 
 # mypy-boto3-amp
 
 [![PyPI - mypy-boto3-amp](https://img.shields.io/pypi/v/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amp.svg?color=blue)](https://pypi.org/project/mypy-boto3-amp)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amp?color=blue)](https://pypistats.org/packages/mypy-boto3-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PrometheusService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[boto3.PrometheusService 1.26.165](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-amp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,42 +416,42 @@
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

### Comparing `mypy-boto3-amp-1.26.0.post1/mypy_boto3_amp.egg-info/SOURCES.txt` & `mypy-boto3-amp-1.26.165/mypy_boto3_amp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amp-1.26.0.post1/setup.py` & `mypy-boto3-amp-1.26.165/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-amp.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amp",
-    version="1.26.0.post1",
+    version="1.26.165",
     packages=["mypy_boto3_amp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PrometheusService 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.PrometheusService 1.26.165 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 amp type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_amp": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_amp": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amp/",
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

