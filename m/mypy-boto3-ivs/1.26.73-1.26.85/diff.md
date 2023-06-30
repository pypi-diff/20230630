# Comparing `tmp/mypy-boto3-ivs-1.26.73.tar.gz` & `tmp/mypy-boto3-ivs-1.26.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-1.26.73.tar", last modified: Thu Feb 16 20:47:25 2023, max compression
+gzip compressed data, was "mypy-boto3-ivs-1.26.85.tar", last modified: Mon Mar  6 20:27:45 2023, max compression
```

## Comparing `mypy-boto3-ivs-1.26.73.tar` & `mypy-boto3-ivs-1.26.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.451044 mypy-boto3-ivs-1.26.73/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-16 20:47:07.000000 mypy-boto3-ivs-1.26.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-02-16 20:47:25.451044 mypy-boto3-ivs-1.26.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-02-16 20:47:07.000000 mypy-boto3-ivs-1.26.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.447043 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-02-16 20:47:07.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21260 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23265 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23244 2023-02-16 20:47:08.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-16 20:47:07.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.451044 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-02-16 20:47:25.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-16 20:47:25.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-16 20:47:25.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-16 20:47:25.000000 mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 20:47:25.451044 mypy-boto3-ivs-1.26.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-16 20:47:07.000000 mypy-boto3-ivs-1.26.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.512846 mypy-boto3-ivs-1.26.85/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-03-06 20:27:45.512846 mypy-boto3-ivs-1.26.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.508846 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21260 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23265 2023-03-06 20:27:35.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23244 2023-03-06 20:27:35.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.508846 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-06 20:27:45.000000 mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 20:27:45.512846 mypy-boto3-ivs-1.26.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-06 20:27:34.000000 mypy-boto3-ivs-1.26.85/setup.py
```

### Comparing `mypy-boto3-ivs-1.26.73/LICENSE` & `mypy-boto3-ivs-1.26.85/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/PKG-INFO` & `mypy-boto3-ivs-1.26.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.26.73
-Summary: Type annotations for boto3.IVS 1.26.73 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.85
+Summary: Type annotations for boto3.IVS 1.26.85 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.26.73/README.md` & `mypy-boto3-ivs-1.26.85/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/__init__.py` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/__init__.pyi` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/__main__.py` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IVS 1.26.73\nVersion:         1.26.73\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.IVS 1.26.85\nVersion:         1.26.85\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.73")
+    print("1.26.85")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/client.py` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/client.pyi` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/literals.py` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -371,14 +372,15 @@
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
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/literals.pyi` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -369,14 +370,15 @@
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
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/paginator.py` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/paginator.pyi` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/type_defs.py` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs/type_defs.pyi` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/PKG-INFO` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.26.73
-Summary: Type annotations for boto3.IVS 1.26.73 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.85
+Summary: Type annotations for boto3.IVS 1.26.85 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.26.73/mypy_boto3_ivs.egg-info/SOURCES.txt` & `mypy-boto3-ivs-1.26.85/mypy_boto3_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.26.73/setup.py` & `mypy-boto3-ivs-1.26.85/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-ivs",
-    version="1.26.73",
+    version="1.26.85",
     packages=["mypy_boto3_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IVS 1.26.73 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.IVS 1.26.85 service generated with mypy-boto3-builder 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

