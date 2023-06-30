# Comparing `tmp/openai_function_calling-1.0.0.tar.gz` & `tmp/openai_function_calling-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_calling-1.0.0.tar", max compression
+gzip compressed data, was "openai_function_calling-1.0.1.tar", max compression
```

## Comparing `openai_function_calling-1.0.0.tar` & `openai_function_calling-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2210 2023-06-28 04:20:47.915657 openai_function_calling-1.0.0/README.md
--rw-r--r--   0        0        0      407 2023-06-28 04:20:47.916273 openai_function_calling-1.0.0/openai_function_calling/__init__.py
--rw-r--r--   0        0        0     2901 2023-06-28 04:20:47.916495 openai_function_calling-1.0.0/openai_function_calling/function.py
--rw-r--r--   0        0        0      330 2023-06-28 04:20:47.916650 openai_function_calling-1.0.0/openai_function_calling/json_schema_type.py
--rw-r--r--   0        0        0     3147 2023-06-28 04:20:47.916870 openai_function_calling-1.0.0/openai_function_calling/parameter.py
--rw-r--r--   0        0        0        0 2023-06-28 04:20:47.916908 openai_function_calling-1.0.0/openai_function_calling/py.typed
--rw-r--r--   0        0        0      625 2023-06-28 04:21:05.954270 openai_function_calling-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 openai_function_calling-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2210 2023-06-28 04:20:47.915657 openai_function_calling-1.0.1/README.md
+-rw-r--r--   0        0        0      407 2023-06-28 04:20:47.916273 openai_function_calling-1.0.1/openai_function_calling/__init__.py
+-rw-r--r--   0        0        0     3410 2023-06-30 18:14:11.747488 openai_function_calling-1.0.1/openai_function_calling/function.py
+-rw-r--r--   0        0        0      330 2023-06-28 04:20:47.916650 openai_function_calling-1.0.1/openai_function_calling/json_schema_type.py
+-rw-r--r--   0        0        0     3147 2023-06-28 04:20:47.916870 openai_function_calling-1.0.1/openai_function_calling/parameter.py
+-rw-r--r--   0        0        0        0 2023-06-28 04:20:47.916908 openai_function_calling-1.0.1/openai_function_calling/py.typed
+-rw-r--r--   0        0        0      625 2023-06-30 18:17:45.444765 openai_function_calling-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 openai_function_calling-1.0.1/PKG-INFO
```

### Comparing `openai_function_calling-1.0.0/README.md` & `openai_function_calling-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_function_calling-1.0.0/openai_function_calling/function.py` & `openai_function_calling-1.0.1/openai_function_calling/function.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Define the Function class and related objects."""
 
 from typing import TypedDict
 
-from typing_extensions import NotRequired
+from typing_extensions import NotRequired, deprecated
 
 from openai_function_calling.json_schema_type import JsonSchemaType
 from openai_function_calling.parameter import Parameter, ParameterDict
 
 
 class ParametersDict(TypedDict):
     """A JSON schema representation of a parameter object."""
@@ -60,14 +60,29 @@
         for required_parameter in self.required_parameters:
             if required_parameter not in parameter_names:
                 raise ValueError(
                     f"Cannot require a parameter, '{required_parameter}', that is not "
                     "defined.",
                 )
 
+    @deprecated(
+        "The to_dict method has been deprecated in favor of the "
+        "to_json_schema method. Please use the to_json_schema method instead.",
+    )
+    def to_dict(self) -> FunctionDict:
+        """Convert the function instance to a JSON schema dict.
+
+        Raises:
+            ValueError: If a parameter is marked as required, but it not defined.
+
+        Returns:
+            A JSON schema representation of the function.
+        """
+        return self.to_json_schema()
+
     def to_json_schema(self) -> FunctionDict:
         """Convert the function instance to a JSON schema dict.
 
         Raises:
             ValueError: If a parameter is marked as required, but it not defined.
 
         Returns:
```

### Comparing `openai_function_calling-1.0.0/openai_function_calling/parameter.py` & `openai_function_calling-1.0.1/openai_function_calling/parameter.py`

 * *Files identical despite different names*

### Comparing `openai_function_calling-1.0.0/pyproject.toml` & `openai_function_calling-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-function-calling"
-version = "1.0.0"
+version = "1.0.1"
 description = "Helper functions to generate OpenAI GPT function calling requests."
 authors = ["Jake Cyr <cyrjake@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_function_calling"}]
 include = ["openai_function_calling/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `openai_function_calling-1.0.0/PKG-INFO` & `openai_function_calling-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function-calling
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helper functions to generate OpenAI GPT function calling requests.
 Author: Jake Cyr
 Author-email: cyrjake@gmail.com
 Requires-Python: >=3.10,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

