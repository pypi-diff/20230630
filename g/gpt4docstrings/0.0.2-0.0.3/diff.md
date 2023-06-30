# Comparing `tmp/gpt4docstrings-0.0.2.tar.gz` & `tmp/gpt4docstrings-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4docstrings-0.0.2.tar", max compression
+gzip compressed data, was "gpt4docstrings-0.0.3.tar", max compression
```

## Comparing `gpt4docstrings-0.0.2.tar` & `gpt4docstrings-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-06-29 00:44:10.891511 gpt4docstrings-0.0.2/LICENSE
--rw-r--r--   0        0        0     2830 2023-06-29 00:44:10.891511 gpt4docstrings-0.0.2/README.md
--rw-r--r--   0        0        0     1987 2023-06-29 00:44:34.371432 gpt4docstrings-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       83 2023-06-29 00:44:10.899511 gpt4docstrings-0.0.2/src/gpt4docstrings/__init__.py
--rw-r--r--   0        0        0       75 2023-06-29 00:44:10.899511 gpt4docstrings-0.0.2/src/gpt4docstrings/__main__.py
--rw-r--r--   0        0        0     1558 2023-06-29 00:44:10.899511 gpt4docstrings-0.0.2/src/gpt4docstrings/cli.py
--rw-r--r--   0        0        0       67 2023-06-29 00:44:10.899511 gpt4docstrings-0.0.2/src/gpt4docstrings/docstrings_generators/__init__.py
--rw-r--r--   0        0        0     2868 2023-06-29 00:44:10.899511 gpt4docstrings-0.0.2/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py
--rw-r--r--   0        0        0     4183 2023-06-29 00:44:10.899511 gpt4docstrings-0.0.2/src/gpt4docstrings/generate_docstrings.py
--rw-r--r--   0        0        0     1591 2023-06-29 00:44:10.899511 gpt4docstrings-0.0.2/src/gpt4docstrings/utils.py
--rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 gpt4docstrings-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-30 08:34:23.906921 gpt4docstrings-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2830 2023-06-30 08:34:23.906921 gpt4docstrings-0.0.3/README.md
+-rw-r--r--   0        0        0     1987 2023-06-30 08:34:38.246877 gpt4docstrings-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/__init__.py
+-rw-r--r--   0        0        0       75 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/__main__.py
+-rw-r--r--   0        0        0     1558 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/cli.py
+-rw-r--r--   0        0        0       67 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/docstrings_generators/__init__.py
+-rw-r--r--   0        0        0     4877 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py
+-rw-r--r--   0        0        0     4084 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/generate_docstrings.py
+-rw-r--r--   0        0        0     1591 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/utils.py
+-rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 gpt4docstrings-0.0.3/PKG-INFO
```

### Comparing `gpt4docstrings-0.0.2/LICENSE` & `gpt4docstrings-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.2/README.md` & `gpt4docstrings-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.2/pyproject.toml` & `gpt4docstrings-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt4docstrings"
-version = "0.0.2"
+version = "0.0.3"
 description = "gpt4docstrings"
 authors = ["Miguel Otero Pedrido <miguel.otero.pedrido.1993@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MichaelisTrofficus/gpt4docstrings"
 repository = "https://github.com/MichaelisTrofficus/gpt4docstrings"
 documentation = "https://gpt4docstrings.readthedocs.io"
```

### Comparing `gpt4docstrings-0.0.2/src/gpt4docstrings/cli.py` & `gpt4docstrings-0.0.3/src/gpt4docstrings/cli.py`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.2/src/gpt4docstrings/generate_docstrings.py` & `gpt4docstrings-0.0.3/src/gpt4docstrings/generate_docstrings.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,32 +88,30 @@
         for node in source.find_all("def"):
             if not node.value[
                 0
             ].type == "string" and not utils.check_def_node_is_class_method(node):
                 docstring_dict = self.docstring_generator.generate_function_docstring(
                     node.dumps()
                 )
-                node.value.insert(0, f'"""\n{docstring_dict["docstring"]}\n"""')
+                node.value.insert(0, docstring_dict["docstring"])
 
         for node in source.find_all("class"):
             if not node.value[0].type == "string":
                 docstring_dict = self.docstring_generator.generate_class_docstring(
                     node.dumps()
                 )
-                node.value.insert(0, f'"""\n{docstring_dict["docstring"]}\n"""')
+                node.value.insert(0, docstring_dict["docstring"])
 
                 for method_node in node.value:
                     if (
                         method_node.type == "def"
                         and not utils.check_is_private_method(method_node)
                         and not method_node.value[0].type == "string"
                     ):
-                        method_node.value.insert(
-                            0, f'"""\n{docstring_dict[method_node.name]}\n"""'
-                        )
+                        method_node.value.insert(0, docstring_dict[method_node.name])
 
         utils.write_updated_source_to_file(source, filename)
 
     def _generate_docstrings(self, filenames: List[str]):
         """
         Traverses the filenames and generate docstrings for undocumented classes / functions
         inside each file.
```

### Comparing `gpt4docstrings-0.0.2/src/gpt4docstrings/utils.py` & `gpt4docstrings-0.0.3/src/gpt4docstrings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.2/PKG-INFO` & `gpt4docstrings-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4docstrings
-Version: 0.0.2
+Version: 0.0.3
 Summary: gpt4docstrings
 Home-page: https://github.com/MichaelisTrofficus/gpt4docstrings
 License: MIT
 Author: Miguel Otero Pedrido
 Author-email: miguel.otero.pedrido.1993@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 1 - Planning
```

