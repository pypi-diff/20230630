# Comparing `tmp/yandil-0.2.3.tar.gz` & `tmp/yandil-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.2.3.tar", max compression
+gzip compressed data, was "yandil-0.2.4.tar", max compression
```

## Comparing `yandil-0.2.3.tar` & `yandil-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1498 2023-06-27 22:56:56.391521 yandil-0.2.3/LICENSE
--rw-r--r--   0        0        0    11594 2023-06-27 22:56:56.391521 yandil-0.2.3/README.md
--rw-r--r--   0        0        0      842 2023-06-27 22:57:52.692485 yandil-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0    10681 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/dependency.py
--rw-r--r--   0        0        0     1505 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3192 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      257 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      301 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     3548 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-06-27 22:56:56.391521 yandil-0.2.3/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    11998 1970-01-01 00:00:00.000000 yandil-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-06-30 17:01:10.398100 yandil-0.2.4/LICENSE
+-rw-r--r--   0        0        0    11594 2023-06-30 17:01:10.398100 yandil-0.2.4/README.md
+-rw-r--r--   0        0        0      988 2023-06-30 17:02:06.610940 yandil-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0    10681 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1505 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3664 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      257 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      301 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     4954 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-06-30 17:01:10.398100 yandil-0.2.4/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    12144 1970-01-01 00:00:00.000000 yandil-0.2.4/PKG-INFO
```

### Comparing `yandil-0.2.3/LICENSE` & `yandil-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/README.md` & `yandil-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/pyproject.toml` & `yandil-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "yandil"
-version = "0.2.3"
+version = "0.2.4"
 description = "Yet ANother Dependency Injection Library"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 license = "BSD-3-Clause"
+repository = "https://github.com/DeejayRevok/yandil"
+homepage = "https://github.com/DeejayRevok/yandil"
+keywords = ["dependency injection", "di"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 
 [tool.poetry.dev-dependencies]
 black = "22.1.0"
 coverage = "5.3"
@@ -31,15 +34,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.3"
+version = "0.2.4"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.2.3/src/yandil/configuration/configuration_container.py` & `yandil-0.2.4/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/src/yandil/container.py` & `yandil-0.2.4/src/yandil/container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/src/yandil/declarative/decorators.py` & `yandil-0.2.4/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/src/yandil/dependency.py` & `yandil-0.2.4/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/src/yandil/dependency_filler.py` & `yandil-0.2.4/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/src/yandil/discovery/class_discovery.py` & `yandil-0.2.4/src/yandil/discovery/class_discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ast import Call, ClassDef, FunctionDef, Name, Subscript, parse
 from dataclasses import dataclass
 from importlib import import_module
 from os import path
 from os.path import relpath, splitext
-from typing import Iterable, Set, Type
+from typing import Iterable, Optional, Set, Type
 
 
 @dataclass(frozen=True)
 class ClassData:
     module_file_path: str
     class_name: str
 
@@ -48,28 +48,40 @@
     for class_node in class_nodes:
         yield ClassData(
             module_file_path=module_file_path,
             class_name=class_node.name,
         )
 
 
-def exclude_classes_without_public_methods(class_nodes: Iterable[ClassDef]) -> Iterable[ClassDef]:
+def exclude_classes_without_public_methods(
+    class_nodes: Iterable[ClassDef],
+    classes_without_defined_public_methods: Optional[Set[ClassDef]] = None,
+) -> Iterable[ClassDef]:
     for class_node in class_nodes:
         if class_defines_public_methods(class_node):
             yield class_node
+        elif classes_without_defined_public_methods is not None:
+            classes_without_defined_public_methods.add(class_node)
 
 
 def class_defines_public_methods(class_node: ClassDef) -> bool:
     for node in class_node.body:
-        if not isinstance(node, FunctionDef) or node.name.startswith("_"):
+        if not isinstance(node, FunctionDef) or node.name.startswith("_") or is_class_method(node):
             continue
         return True
     return False
 
 
+def is_class_method(node: FunctionDef) -> bool:
+    for decorator_node in node.decorator_list:
+        if isinstance(decorator_node, Name) and decorator_node.id == "classmethod":
+            return True
+    return False
+
+
 def exclude_dataclasses(class_nodes: Iterable[ClassDef]) -> Iterable[ClassDef]:
     for class_node in class_nodes:
         if class_has_any_decorator(class_node, {"dataclass"}):
             continue
         yield class_node
```

### Comparing `yandil-0.2.3/src/yandil/discovery/module_discovery.py` & `yandil-0.2.4/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.2.4/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/src/yandil/typing_tools.py` & `yandil-0.2.4/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.3/PKG-INFO` & `yandil-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.2.3
+Version: 0.2.4
 Summary: Yet ANother Dependency Injection Library
+Home-page: https://github.com/DeejayRevok/yandil
 License: BSD-3-Clause
+Keywords: dependency injection,di
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Project-URL: Repository, https://github.com/DeejayRevok/yandil
 Description-Content-Type: text/markdown
 
 # YANDIL
 [![YANDIL CI](https://github.com/DeejayRevok/yandil/actions/workflows/pythonapp.yml/badge.svg?branch=main)](https://github.com/DeejayRevok/yandil/actions/workflows/pythonapp.yml)
 [![PyPI version](https://badge.fury.io/py/yandil.svg)](https://pypi.org/project/yandil/)
 
 ## What is YANDIL?
```

