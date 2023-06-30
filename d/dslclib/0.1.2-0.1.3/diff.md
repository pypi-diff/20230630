# Comparing `tmp/dslclib-0.1.2.tar.gz` & `tmp/dslclib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslclib-0.1.2.tar", max compression
+gzip compressed data, was "dslclib-0.1.3.tar", max compression
```

## Comparing `dslclib-0.1.2.tar` & `dslclib-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      327 2023-06-30 13:55:21.701167 dslclib-0.1.2/README.md
--rw-r--r--   0        0        0      333 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/__init__.py
--rw-r--r--   0        0        0      381 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/__init__.py
--rw-r--r--   0        0        0     3206 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/base.py
--rw-r--r--   0        0        0    11535 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/body_controller.py
--rw-r--r--   0        0        0     5694 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/expression_controller.py
--rw-r--r--   0        0        0     9042 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/face_recognition.py
--rw-r--r--   0        0        0     3643 2023-06-30 13:55:21.701167 dslclib-0.1.2/dslclib/src/speech_recognition.py
--rw-r--r--   0        0        0     4486 2023-06-30 13:55:21.705167 dslclib-0.1.2/dslclib/src/tts.py
--rw-r--r--   0        0        0      635 2023-06-30 13:55:53.917415 dslclib-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 dslclib-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      702 2023-06-30 14:41:31.326866 dslclib-0.1.3/README.md
+-rw-r--r--   0        0        0      334 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/__init__.py
+-rw-r--r--   0        0        0      382 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/__init__.py
+-rw-r--r--   0        0        0     3206 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/base.py
+-rw-r--r--   0        0        0    11535 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/body_controller.py
+-rw-r--r--   0        0        0     5700 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/expression_controller.py
+-rw-r--r--   0        0        0     9049 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/face_recognition.py
+-rw-r--r--   0        0        0     3652 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/speech_recognition.py
+-rw-r--r--   0        0        0     4489 2023-06-30 14:41:31.330865 dslclib-0.1.3/dslclib/src/tts.py
+-rw-r--r--   0        0        0      635 2023-06-30 14:42:02.515082 dslclib-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 dslclib-0.1.3/PKG-INFO
```

### Comparing `dslclib-0.1.2/dslclib/src/base.py` & `dslclib-0.1.3/dslclib/src/base.py`

 * *Files identical despite different names*

### Comparing `dslclib-0.1.2/dslclib/src/body_controller.py` & `dslclib-0.1.3/dslclib/src/body_controller.py`

 * *Files identical despite different names*

### Comparing `dslclib-0.1.2/dslclib/src/expression_controller.py` & `dslclib-0.1.3/dslclib/src/expression_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             ソケット通信を行うポート．
 
         Returns
         -------
 
         Examples
         --------
-        >>> client = BodyController()
+        >>> client = ExpressionController()
         ipがNoneだったため、127.0.0.1をipアドレスとして設定します。
         >>> client
         Socket(
             ip   = 127.0.0.1
             port = 20000
         )
         >>>
```

### Comparing `dslclib-0.1.2/dslclib/src/face_recognition.py` & `dslclib-0.1.3/dslclib/src/face_recognition.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             ソケット通信を行うポート．
 
         Returns
         -------
 
         Examples
         --------
-        >>> client = BodyController()
+        >>> client = FaceRecognitionClient()
         ipがNoneだったため、127.0.0.1をipアドレスとして設定します。
         >>> client
         Socket(
             ip   = 127.0.0.1
             port = 4500
         )
         >>>
```

### Comparing `dslclib-0.1.2/dslclib/src/speech_recognition.py` & `dslclib-0.1.3/dslclib/src/speech_recognition.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             ソケット通信を行うポート．
 
         Returns
         -------
 
         Examples
         --------
-        >>> client = BodyController()
+        >>> client = SpeechRecognitionClient()
         ipがNoneだったため、127.0.0.1をipアドレスとして設定します。
         >>> client
         Socket(
             ip   = 127.0.0.1
             port = 8888
         )
         >>>
```

### Comparing `dslclib-0.1.2/dslclib/src/tts.py` & `dslclib-0.1.3/dslclib/src/tts.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             ソケット通信を行うポート．
 
         Returns
         -------
 
         Examples
         --------
-        >>> client = BodyController()
+        >>> client = Text2SpeechClient()
         ipがNoneだったため、127.0.0.1をipアドレスとして設定します。
         >>> client
         Socket(
             ip   = 127.0.0.1
             port = 3456
         )
         >>>
```

### Comparing `dslclib-0.1.2/pyproject.toml` & `dslclib-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dslclib"
-version = "0.1.2"
+version = "0.1.3"
 description = "対話システムライブコンペティションに使用できるPythonライブラリ"
 authors = ["Yuta SASAKI <yubo1336@lr.pi.titech.ac.jp>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 sphinx = "^7.0.1"
```

