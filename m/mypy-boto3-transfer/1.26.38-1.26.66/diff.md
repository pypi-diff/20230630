# Comparing `tmp/mypy-boto3-transfer-1.26.38.tar.gz` & `tmp/mypy-boto3-transfer-1.26.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.26.38.tar", last modified: Tue Dec 27 20:32:14 2022, max compression
+gzip compressed data, was "mypy-boto3-transfer-1.26.66.tar", last modified: Tue Feb  7 20:25:40 2023, max compression
```

## Comparing `mypy-boto3-transfer-1.26.38.tar` & `mypy-boto3-transfer-1.26.66.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.269875 mypy-boto3-transfer-1.26.38/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21631 2022-12-27 20:32:14.269875 mypy-boto3-transfer-1.26.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20140 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.265875 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46025 2022-12-27 20:32:05.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45947 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2022-12-27 20:32:05.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2022-12-27 20:32:05.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2022-12-27 20:32:05.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2022-12-27 20:32:05.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58819 2022-12-27 20:32:06.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58730 2022-12-27 20:32:05.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-27 20:32:05.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2022-12-27 20:32:05.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.265875 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21631 2022-12-27 20:32:14.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2022-12-27 20:32:14.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 20:32:14.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 20:32:14.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-27 20:32:14.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-27 20:32:14.000000 mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 20:32:14.269875 mypy-boto3-transfer-1.26.38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2022-12-27 20:32:04.000000 mypy-boto3-transfer-1.26.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:25:40.553150 mypy-boto3-transfer-1.26.66/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-02-07 20:25:40.553150 mypy-boto3-transfer-1.26.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20140 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:25:40.553150 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46025 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45947 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58819 2023-02-07 20:25:33.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58730 2023-02-07 20:25:32.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:25:40.553150 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-02-07 20:25:40.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-07 20:25:40.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 20:25:40.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 20:25:40.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-07 20:25:40.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-07 20:25:40.000000 mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 20:25:40.553150 mypy-boto3-transfer-1.26.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-07 20:25:31.000000 mypy-boto3-transfer-1.26.66/setup.py
```

### Comparing `mypy-boto3-transfer-1.26.38/LICENSE` & `mypy-boto3-transfer-1.26.66/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/PKG-INFO` & `mypy-boto3-transfer-1.26.66/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.26.38
-Summary: Type annotations for boto3.Transfer 1.26.38 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.66
+Summary: Type annotations for boto3.Transfer 1.26.66 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.26.38](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.26.66](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.26.38/README.md` & `mypy-boto3-transfer-1.26.66/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.26.38](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.26.66](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/__init__.py` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/__init__.pyi` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/__main__.py` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.26.38\nVersion:         1.26.38\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.Transfer 1.26.66\nVersion:         1.26.66\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.38")
+    print("1.26.66")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/client.py` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/client.pyi` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/literals.py` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,24 +156,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -281,14 +283,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/literals.pyi` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -154,24 +154,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -279,14 +281,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/paginator.py` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/paginator.pyi` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/type_defs.py` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/type_defs.pyi` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/waiter.py` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer/waiter.pyi` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.26.38
-Summary: Type annotations for boto3.Transfer 1.26.38 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.66
+Summary: Type annotations for boto3.Transfer 1.26.66 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.26.38](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.26.66](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.26.38/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy-boto3-transfer-1.26.66/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.26.38/setup.py` & `mypy-boto3-transfer-1.26.66/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.26.38",
+    version="1.26.66",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Transfer 1.26.38 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.Transfer 1.26.66 service generated with mypy-boto3-builder"
+        " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

