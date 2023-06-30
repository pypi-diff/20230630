# Comparing `tmp/dslclib-0.1.1.tar.gz` & `tmp/dslclib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslclib-0.1.1.tar", max compression
+gzip compressed data, was "dslclib-0.1.2.tar", max compression
```

## Comparing `dslclib-0.1.1.tar` & `dslclib-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       99 2023-06-24 23:40:05.059152 dslclib-0.1.1/README.md
--rw-r--r--   0        0        0      315 2023-06-24 23:40:28.955105 dslclib-0.1.1/dslclib/__init__.py
--rw-r--r--   0        0        0      381 2023-06-24 23:40:05.059152 dslclib-0.1.1/dslclib/src/__init__.py
--rw-r--r--   0        0        0     1274 2023-06-24 23:40:05.059152 dslclib-0.1.1/dslclib/src/base.py
--rw-r--r--   0        0        0     5063 2023-06-24 23:40:05.059152 dslclib-0.1.1/dslclib/src/body_controller.py
--rw-r--r--   0        0        0     3994 2023-06-24 23:40:05.059152 dslclib-0.1.1/dslclib/src/expression_controller.py
--rw-r--r--   0        0        0     6278 2023-06-24 23:40:05.059152 dslclib-0.1.1/dslclib/src/face_recognition.py
--rw-r--r--   0        0        0     2630 2023-06-24 23:40:05.059152 dslclib-0.1.1/dslclib/src/speech_recognition.py
--rw-r--r--   0        0        0     3588 2023-06-24 23:40:05.059152 dslclib-0.1.1/dslclib/src/tts.py
--rw-r--r--   0        0        0      597 2023-06-24 23:40:28.951105 dslclib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 dslclib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      327 2023-06-30 13:55:21.701167 dslclib-0.1.2/README.md
+-rw-r--r--   0        0        0      333 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/__init__.py
+-rw-r--r--   0        0        0     3206 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/base.py
+-rw-r--r--   0        0        0    11535 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/body_controller.py
+-rw-r--r--   0        0        0     5694 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/expression_controller.py
+-rw-r--r--   0        0        0     9042 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/face_recognition.py
+-rw-r--r--   0        0        0     3643 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/speech_recognition.py
+-rw-r--r--   0        0        0     4486 2023-06-30 13:55:21.705167 dslclib-0.1.2/dslclib/src/tts.py
+-rw-r--r--   0        0        0      635 2023-06-30 13:55:53.917415 dslclib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 dslclib-0.1.2/PKG-INFO
```

### Comparing `dslclib-0.1.1/pyproject.toml` & `dslclib-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "dslclib"
-version = "0.1.1"
+version = "0.1.2"
 description = "対話システムライブコンペティションに使用できるPythonライブラリ"
 authors = ["Yuta SASAKI <yubo1336@lr.pi.titech.ac.jp>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
+sphinx = "^7.0.1"
+furo = "^2023.5.20"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 mypy = "^1.4.0"
 isort = "^5.12.0"
 black = "^23.3.0"
```

### Comparing `dslclib-0.1.1/PKG-INFO` & `dslclib-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: dslclib
-Version: 0.1.1
+Version: 0.1.2
 Summary: 対話システムライブコンペティションに使用できるPythonライブラリ
 Author: Yuta SASAKI
 Author-email: yubo1336@lr.pi.titech.ac.jp
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: furo (>=2023.5.20,<2024.0.0)
+Requires-Dist: sphinx (>=7.0.1,<8.0.0)
 Description-Content-Type: text/markdown
 
 # dslc6
 対話システムライブコンペティションに使用できるPythonライブラリ
 
+リファレンスは[https://yuta0306.github.io/dslclib/](https://yuta0306.github.io/dslclib/)にあります．
+
+このライブラリに関する要望や質問は，yubo1336[at]lr.pi.titech.ac.jpまでお願いします．
+
```

