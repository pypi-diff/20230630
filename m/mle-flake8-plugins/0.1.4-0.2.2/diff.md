# Comparing `tmp/mle_flake8_plugins-0.1.4.tar.gz` & `tmp/mle_flake8_plugins-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mle_flake8_plugins-0.1.4.tar", max compression
+gzip compressed data, was "mle_flake8_plugins-0.2.2.tar", max compression
```

## Comparing `mle_flake8_plugins-0.1.4.tar` & `mle_flake8_plugins-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/mle_flake8_plugins/__init__.py
--rw-r--r--   0        0        0      680 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_convention/__init__.py
--rw-r--r--   0        0        0      143 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_convention/errors.py
--rw-r--r--   0        0        0     1303 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py
--rw-r--r--   0        0        0     1607 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py
--rw-r--r--   0        0        0     2178 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_docstring/__init__.py
--rw-r--r--   0        0        0     1910 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py
--rw-r--r--   0        0        0      105 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_docstring/errors.py
--rw-r--r--   0        0        0      576 2023-04-24 14:25:12.349911 mle_flake8_plugins-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mle_flake8_plugins-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/__init__.py
+-rw-r--r--   0        0        0      811 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/__init__.py
+-rw-r--r--   0        0        0     1197 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/disallow_final_w_pydantic.py
+-rw-r--r--   0        0        0      226 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/errors.py
+-rw-r--r--   0        0        0     1327 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py
+-rw-r--r--   0        0        0     1764 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py
+-rw-r--r--   0        0        0     2178 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/__init__.py
+-rw-r--r--   0        0        0     2170 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py
+-rw-r--r--   0        0        0      111 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/errors.py
+-rw-r--r--   0        0        0      596 2023-06-30 12:06:40.600240 mle_flake8_plugins-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mle_flake8_plugins-0.2.2/PKG-INFO
```

### Comparing `mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_convention/__init__.py` & `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import ast
 
+from .disallow_final_w_pydantic import PydanticFinalChecker
 from .legacy_type_hint_checker import LegacyTypeHintChecker
 from .no_operation_checker import NoOperationsChecker
 
 __version__ = "0.1.0"
 
 
 class MleConventionChecker:
     name = "flake8-mle-convention"
 
     def __init__(self, tree: ast.AST):
         self.tree = tree
 
     def run(self):
-        checkers = [LegacyTypeHintChecker(), NoOperationsChecker()]
+        checkers = [
+            LegacyTypeHintChecker(),
+            NoOperationsChecker(),
+            PydanticFinalChecker(),
+        ]
         errors = []
         for checker in checkers:
             checker.visit(self.tree)
             errors.extend(checker.errors)
 
         errors_seen = set()
         for error in errors:
```

### Comparing `mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py` & `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     def check_type_hint(self, hint: ast.AST, lineno: int, col_offset: int) -> None:
         if isinstance(hint, ast.Subscript) and isinstance(hint.value, ast.Name):
             if hint.value.id in {"List", "Dict", "Tuple"}:
                 self.errors.append(
                     (
                         lineno,
                         col_offset,
-                        error_codes["legacy_type_hint"] % (hint.value.id.lower(), hint.value.id),
+                        error_codes["legacy_type_hint"]
+                        % (hint.value.id.lower(), hint.value.id),
                         type(self),
                     )
                 )
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
         if node.returns is not None:
             self.check_type_hint(node.returns, node.lineno, node.col_offset)
```

### Comparing `mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py` & `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,12 +47,19 @@
     def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
         has_only_pass = len(node.body) == 1 and isinstance(node.body[0], ast.Pass)
         has_decorator = bool(node.decorator_list)
 
         if not has_only_pass and not has_decorator:
             operations_count = self._count_operations(node)
             if operations_count < 1:
-                self.errors.append((node.lineno, node.col_offset, error_codes["no_operation"], type(self)))
+                self.errors.append(
+                    (
+                        node.lineno,
+                        node.col_offset,
+                        error_codes["no_operation"],
+                        type(self),
+                    )
+                )
         self.generic_visit(node)
 
     def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:
         self.visit_FunctionDef(node)
```

### Comparing `mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_docstring/__init__.py` & `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.4/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py` & `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,22 +32,32 @@
             # dataclass, class member
             if (
                 isinstance(child, ast.AnnAssign)
                 and isinstance(child.target, ast.Name)
                 and self.is_public(child.target.id)
                 and child.target.id not in doc_attrs
             ):
-                self.errors.append((node.lineno, node.col_offset, error_codes["attribute"] % child.target.id))
+                self.errors.append(
+                    (
+                        node.lineno,
+                        node.col_offset,
+                        error_codes["attribute"] % child.target.id,
+                    )
+                )
 
             # assign value in functions
             if isinstance(child, ast.FunctionDef):
                 for gc in child.body:
                     if (
                         isinstance(gc, ast.Assign)
                         and gc.targets
                         and isinstance(gc.targets[0], ast.Attribute)
                         and self.is_public(gc.targets[0].attr)
                         and gc.targets[0].attr not in doc_attrs
                     ):
                         self.errors.append(
-                            (node.lineno, node.col_offset, error_codes["attribute"] % gc.targets[0].attr)
+                            (
+                                node.lineno,
+                                node.col_offset,
+                                error_codes["attribute"] % gc.targets[0].attr,
+                            )
                         )
```

### Comparing `mle_flake8_plugins-0.1.4/pyproject.toml` & `mle_flake8_plugins-0.2.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "mle-flake8-plugins"
-version = "0.1.4"
+version = "0.2.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docstring-parser = "^0.15"
 flake8 = "^5.0.4"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^22.8.0"
 pytest = "^7.1.3"
+autoflake = ">=1.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."flake8.extension"]
 MLE00 = "mle_flake8_plugins.flake8_mle_docstring:MleDocstringChecker"
```

