# Comparing `tmp/superagi_tools-1.0.0.tar.gz` & `tmp/superagi_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagi_tools-1.0.0.tar", last modified: Thu Jun 29 10:07:15 2023, max compression
+gzip compressed data, was "superagi_tools-1.0.1.tar", last modified: Fri Jun 30 17:36:08 2023, max compression
```

## Comparing `superagi_tools-1.0.0.tar` & `superagi_tools-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 10:07:15.368196 superagi_tools-1.0.0/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-28 12:07:33.000000 superagi_tools-1.0.0/LICENSE
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-06-29 10:07:15.368196 superagi_tools-1.0.0/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.0/README.md
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-06-29 10:07:15.368196 superagi_tools-1.0.0/setup.cfg
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      306 2023-06-29 10:03:16.000000 superagi_tools-1.0.0/setup.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 10:07:15.364196 superagi_tools-1.0.0/superagi/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.0/superagi/__init__.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 10:07:15.368196 superagi_tools-1.0.0/superagi/tools/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.0/superagi/tools/__init__.py
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6763 2023-06-29 00:49:48.000000 superagi_tools-1.0.0/superagi/tools/base_tool.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 10:07:15.368196 superagi_tools-1.0.0/superagi_tools.egg-info/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-06-29 10:07:15.000000 superagi_tools-1.0.0/superagi_tools.egg-info/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-06-29 10:07:15.000000 superagi_tools-1.0.0/superagi_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-06-29 10:07:15.000000 superagi_tools-1.0.0/superagi_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       16 2023-06-29 10:07:15.000000 superagi_tools-1.0.0/superagi_tools.egg-info/requires.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-06-29 10:07:15.000000 superagi_tools-1.0.0/superagi_tools.egg-info/top_level.txt
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 17:36:08.539578 superagi_tools-1.0.1/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-28 12:07:33.000000 superagi_tools-1.0.1/LICENSE
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-06-30 17:36:08.539578 superagi_tools-1.0.1/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.1/README.md
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-06-30 17:36:08.539578 superagi_tools-1.0.1/setup.cfg
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      306 2023-06-30 17:36:03.000000 superagi_tools-1.0.1/setup.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 17:36:08.483577 superagi_tools-1.0.1/superagi/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.1/superagi/__init__.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 17:36:08.483577 superagi_tools-1.0.1/superagi/tools/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.1/superagi/tools/__init__.py
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6603 2023-06-30 05:10:33.000000 superagi_tools-1.0.1/superagi/tools/base_tool.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 17:36:08.539578 superagi_tools-1.0.1/superagi_tools.egg-info/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-06-30 17:36:07.000000 superagi_tools-1.0.1/superagi_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-06-30 17:36:08.000000 superagi_tools-1.0.1/superagi_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-06-30 17:36:07.000000 superagi_tools-1.0.1/superagi_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       16 2023-06-30 17:36:07.000000 superagi_tools-1.0.1/superagi_tools.egg-info/requires.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-06-30 17:36:07.000000 superagi_tools-1.0.1/superagi_tools.egg-info/top_level.txt
```

### Comparing `superagi_tools-1.0.0/superagi/tools/base_tool.py` & `superagi_tools-1.0.1/superagi/tools/base_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from typing import List
 from typing import Optional, Type, Callable, Any, Union, Dict, Tuple
 
 import yaml
 from pydantic import BaseModel, create_model, validate_arguments, Extra
 
 
-def testing():
-    print("Hello from SuperAGI Package!")
 class SchemaSettings:
     """Configuration for the pydantic model."""
     extra = Extra.forbid
     arbitrary_types_allowed = True
 
 
 def extract_valid_parameters(
@@ -88,17 +86,15 @@
 
     @abstractmethod
     def _execute(self, *args: Any, **kwargs: Any):
         pass
 
     @property
     def max_token_limit(self):
-        token_limit = self.get_tool_config("MAX_TOOL_TOKEN_LIMIT")
-        if token_limit is None:
-            token_limit = 600
+        token_limit = 600
         return token_limit
 
     def _parse_input(
             self,
             tool_input: Union[str, Dict],
     ) -> Union[str, Dict[str, Any]]:
         """Convert tool input to pydantic model."""
```

