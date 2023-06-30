# Comparing `tmp/func_ai-0.0.5.tar.gz` & `tmp/func_ai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_ai-0.0.5.tar", max compression
+gzip compressed data, was "func_ai-0.0.6.tar", max compression
```

## Comparing `func_ai-0.0.5.tar` & `func_ai-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.5/LICENSE
--rw-r--r--   0        0        0     3375 2023-06-30 11:34:34.818711 func_ai-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.5/func_ai/__init__.py
--rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.5/func_ai/function_indexer.py
--rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.5/func_ai/utils/__init__.py
--rw-r--r--   0        0        0     4515 2023-06-30 11:28:00.351251 func_ai-0.0.5/func_ai/utils/jinja_template_functions.py
--rw-r--r--   0        0        0    10241 2023-06-30 09:42:46.148402 func_ai-0.0.5/func_ai/utils/llm_tools.py
--rw-r--r--   0        0        0     5701 2023-06-30 06:36:30.640188 func_ai-0.0.5/func_ai/utils/openapi_function_parser.py
--rw-r--r--   0        0        0     3392 2023-06-30 06:36:30.641465 func_ai-0.0.5/func_ai/utils/py_function_parser.py
--rw-r--r--   0        0        0     5337 2023-06-30 06:36:30.641834 func_ai-0.0.5/func_ai/workflow_creator.py
--rw-r--r--   0        0        0      907 2023-06-30 11:32:21.641350 func_ai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 func_ai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3375 2023-06-30 11:34:34.818711 func_ai-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.6/func_ai/__init__.py
+-rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.6/func_ai/function_indexer.py
+-rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.6/func_ai/utils/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-30 11:52:33.930306 func_ai-0.0.6/func_ai/utils/jinja_template_functions.py
+-rw-r--r--   0        0        0    10241 2023-06-30 09:42:46.148402 func_ai-0.0.6/func_ai/utils/llm_tools.py
+-rw-r--r--   0        0        0     5701 2023-06-30 06:36:30.640188 func_ai-0.0.6/func_ai/utils/openapi_function_parser.py
+-rw-r--r--   0        0        0     3392 2023-06-30 06:36:30.641465 func_ai-0.0.6/func_ai/utils/py_function_parser.py
+-rw-r--r--   0        0        0     5337 2023-06-30 06:36:30.641834 func_ai-0.0.6/func_ai/workflow_creator.py
+-rw-r--r--   0        0        0      907 2023-06-30 12:10:48.672915 func_ai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 func_ai-0.0.6/PKG-INFO
```

### Comparing `func_ai-0.0.5/LICENSE` & `func_ai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.5/README.md` & `func_ai-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.5/func_ai/function_indexer.py` & `func_ai-0.0.6/func_ai/function_indexer.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.5/func_ai/utils/jinja_template_functions.py` & `func_ai-0.0.6/func_ai/utils/jinja_template_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 
 class JinjaOpenAITemplateFunction:
 
     def __init__(self, environment: Environment, llm_interface: LLMInterface, **kwargs):
         self._lm_interface = llm_interface
         self._environment = environment
+        if "filters" in kwargs and isinstance(kwargs["filters"], dict):
+            self._environment.filters = kwargs["filters"]
         # self._lm_interface.conversation_store.add_system_message("""You are a code helper. Your goal is to help the user to convert a jinja template into a list of parameters.
         #
         # User will provide a jinja template as input.
         #
         # Your task is to extract the jinja parameters and return them in a bullet list.
         #
         # Do not return anything other than the bullet list.
```

### Comparing `func_ai-0.0.5/func_ai/utils/llm_tools.py` & `func_ai-0.0.6/func_ai/utils/llm_tools.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.5/func_ai/utils/openapi_function_parser.py` & `func_ai-0.0.6/func_ai/utils/openapi_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.5/func_ai/utils/py_function_parser.py` & `func_ai-0.0.6/func_ai/utils/py_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.5/func_ai/workflow_creator.py` & `func_ai-0.0.6/func_ai/workflow_creator.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.5/pyproject.toml` & `func_ai-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "func-ai"
-version = "0.0.5"
+version = "0.0.6"
 description = "AI Functional Catalog - OpenAI functions on steriods"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "func_ai" }]
 
 [tool.poetry.urls]
```

### Comparing `func_ai-0.0.5/PKG-INFO` & `func_ai-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func-ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: AI Functional Catalog - OpenAI functions on steriods
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

