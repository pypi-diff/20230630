# Comparing `tmp/func_ai-0.0.3.tar.gz` & `tmp/func_ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_ai-0.0.3.tar", max compression
+gzip compressed data, was "func_ai-0.0.4.tar", max compression
```

## Comparing `func_ai-0.0.3.tar` & `func_ai-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.3/LICENSE
--rw-r--r--   0        0        0     1036 2023-06-29 18:08:36.509794 func_ai-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.3/func_ai/__init__.py
--rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.3/func_ai/function_indexer.py
--rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.3/func_ai/utils/__init__.py
--rw-r--r--   0        0        0    10240 2023-06-29 18:00:21.930012 func_ai-0.0.3/func_ai/utils/llm_tools.py
--rw-r--r--   0        0        0     2242 2023-06-29 09:45:30.583696 func_ai-0.0.3/func_ai/utils/openapi_function_parser.py
--rw-r--r--   0        0        0     3392 2023-06-29 09:04:33.935006 func_ai-0.0.3/func_ai/utils/py_function_parser.py
--rw-r--r--   0        0        0     5337 2023-06-29 15:06:55.283947 func_ai-0.0.3/func_ai/workflow_creator.py
--rw-r--r--   0        0        0      889 2023-06-29 18:06:04.015344 func_ai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 func_ai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2907 2023-06-30 05:05:30.775581 func_ai-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.4/func_ai/__init__.py
+-rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.4/func_ai/function_indexer.py
+-rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.4/func_ai/utils/__init__.py
+-rw-r--r--   0        0        0    10240 2023-06-29 18:00:21.930012 func_ai-0.0.4/func_ai/utils/llm_tools.py
+-rw-r--r--   0        0        0     5701 2023-06-30 05:04:37.316662 func_ai-0.0.4/func_ai/utils/openapi_function_parser.py
+-rw-r--r--   0        0        0     3392 2023-06-29 09:04:33.935006 func_ai-0.0.4/func_ai/utils/py_function_parser.py
+-rw-r--r--   0        0        0     5337 2023-06-29 15:06:55.283947 func_ai-0.0.4/func_ai/workflow_creator.py
+-rw-r--r--   0        0        0      889 2023-06-30 03:07:29.394998 func_ai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3940 1970-01-01 00:00:00.000000 func_ai-0.0.4/PKG-INFO
```

### Comparing `func_ai-0.0.3/LICENSE` & `func_ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.3/func_ai/function_indexer.py` & `func_ai-0.0.4/func_ai/function_indexer.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.3/func_ai/utils/llm_tools.py` & `func_ai-0.0.4/func_ai/utils/llm_tools.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.3/func_ai/utils/py_function_parser.py` & `func_ai-0.0.4/func_ai/utils/py_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.3/func_ai/workflow_creator.py` & `func_ai-0.0.4/func_ai/workflow_creator.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.3/pyproject.toml` & `func_ai-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "func-ai"
-version = "0.0.3"
+version = "0.0.4"
 description = "AI Functional Catalog - OpenAI functions on steriods"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "func_ai" }]
 
 [tool.poetry.urls]
```

