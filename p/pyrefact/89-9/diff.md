# Comparing `tmp/pyrefact-89.tar.gz` & `tmp/pyrefact-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefact-89.tar", last modified: Fri Jun 30 07:09:26 2023, max compression
+gzip compressed data, was "pyrefact-9.tar", last modified: Wed Nov  2 20:30:27 2022, max compression
```

## Comparing `pyrefact-89.tar` & `pyrefact-9.tar`

### file list

```diff
@@ -1,34 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:09:26.604974 pyrefact-89/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 07:09:07.000000 pyrefact-89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-30 07:09:26.604974 pyrefact-89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-30 07:09:07.000000 pyrefact-89/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-30 07:09:07.000000 pyrefact-89/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:09:26.604974 pyrefact-89/pyrefact/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26513 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    34184 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   130397 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/logs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13175 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/object_oriented.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/performance_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/performance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    23318 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    33478 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/symbolic_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-06-30 07:09:07.000000 pyrefact-89/pyrefact/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:09:26.604974 pyrefact-89/pyrefact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-30 07:09:26.000000 pyrefact-89/pyrefact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-30 07:09:26.000000 pyrefact-89/pyrefact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:09:26.000000 pyrefact-89/pyrefact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 07:09:26.000000 pyrefact-89/pyrefact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 07:09:26.000000 pyrefact-89/pyrefact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 07:09:26.000000 pyrefact-89/pyrefact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 07:09:26.604974 pyrefact-89/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:09:26.604974 pyrefact-89/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-30 07:09:07.000000 pyrefact-89/tests/testing_infra.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405663 pyrefact-9/
+-rw-r--r--   0 olle       (501) staff       (20)     1069 2022-10-20 08:55:02.000000 pyrefact-9/LICENSE
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.405542 pyrefact-9/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)     1262 2022-11-02 18:36:20.000000 pyrefact-9/README.md
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.404795 pyrefact-9/pyrefact/
+-rw-r--r--   0 olle       (501) staff       (20)        0 2022-10-23 21:51:04.000000 pyrefact-9/pyrefact/__init__.py
+-rwxr-xr-x   0 olle       (501) staff       (20)      120 2022-10-20 18:11:25.000000 pyrefact-9/pyrefact/__main__.py
+-rw-r--r--   0 olle       (501) staff       (20)     2148 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/completion.py
+-rw-r--r--   0 olle       (501) staff       (20)     1065 2022-10-30 20:04:01.000000 pyrefact-9/pyrefact/constants.py
+-rw-r--r--   0 olle       (501) staff       (20)    31081 2022-11-02 20:24:19.000000 pyrefact-9/pyrefact/fixes.py
+-rwxr-xr-x   0 olle       (501) staff       (20)     3867 2022-11-02 12:50:20.000000 pyrefact-9/pyrefact/main.py
+-rw-r--r--   0 olle       (501) staff       (20)    12892 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/parsing.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405383 pyrefact-9/pyrefact.egg-info/
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)      327 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/SOURCES.txt
+-rw-r--r--   0 olle       (501) staff       (20)        1 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/dependency_links.txt
+-rw-r--r--   0 olle       (501) staff       (20)       40 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/requires.txt
+-rw-r--r--   0 olle       (501) staff       (20)        9 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/top_level.txt
+-rw-r--r--   0 olle       (501) staff       (20)       38 2022-11-02 20:30:27.405698 pyrefact-9/setup.cfg
+-rw-r--r--   0 olle       (501) staff       (20)      468 2022-11-02 20:30:04.000000 pyrefact-9/setup.py
```

### Comparing `pyrefact-89/LICENSE` & `pyrefact-9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrefact-89/pyrefact/abstractions.py` & `pyrefact-9/pyrefact/fixes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,711 +1,875 @@
 import ast
+import builtins
 import collections
+import heapq
+import io
 import itertools
+import queue
 import re
-from typing import Collection, Iterable, Sequence, Tuple
+import sys
+import tempfile
+from pathlib import Path
+from typing import Collection, Iterable, List, Mapping, Tuple, Union
+
+import black
+import isort
+import rmspace
+from pylint.lint import Run
+
+from pyrefact import parsing
+from pyrefact.constants import ASSUMED_PACKAGES, ASSUMED_SOURCES, PACKAGE_ALIASES
+
+_REDUNDANT_UNDERSCORED_ASSIGN_RE_PATTERN = r"(?<![^\n]) *(\*?_ *,? *)+[\*\+\/\-\|\&:]?= *(?![=])"
+
+
+def _deconstruct_pylint_warning(error_line: str) -> Tuple[Path, int, int, str, str]:
+    filename, lineno, charno, error_code, error_msg = error_line.split(":")
+
+    return filename, lineno, charno, error_code.strip(), error_msg.strip()
+
+
+def _find_pylint_errors(content: str, error_code: str) -> Iterable[str]:
+    original_sys_stdout = sys.stdout
+    with tempfile.NamedTemporaryFile(suffix=".py") as temp:
+        temp.write(content.encode("utf-8"))
+        temp.seek(0)
+        stdout = io.StringIO()
+        args = [
+            "--disable",
+            "all",
+            "--enable",
+            f"{error_code}",
+            temp.name,
+        ]
+        try:
+            sys.stdout = stdout
+            Run(args, exit=False)
+        finally:
+            sys.stdout = original_sys_stdout
+
+    re_pattern = re.compile(r".*\.py:\d+:\d+: \w\d+: .* \(" + error_code + r"\)")
+    output = stdout.getvalue()
+    for line in output.splitlines():
+        if re_pattern.match(line):
+            yield line
 
-from pyrefact import constants, core, parsing, processing, style, tracing
 
+def _get_undefined_variables(content: str) -> Collection[str]:
+    variables = set()
+    for line in _find_pylint_errors(content, "undefined-variable"):
+        try:
+            _, *_, error_msg = _deconstruct_pylint_warning(line)
+            _, variable_name, _ = error_msg.split("'")
+            variables.add(variable_name)
+        except ValueError:
+            pass
 
-class _EverythingContainer:
-    """Object that contains everything."""
+    return variables
 
-    @staticmethod
-    def __contains__(_) -> bool:
-        return True
 
+def _is_private(variable: str) -> bool:
+    return variable.startswith("_")
 
-def _scoped_dependencies(node: ast.AST):
-    return {name.id for name in parsing.iter_assignments(node)}
 
+def _rename_variable(variable: str, *, static: bool, private: bool) -> str:
+    if variable == "_":
+        return variable
 
-def hash_node(
-    node: ast.AST, preserved_callable_names: Collection[str] = _EverythingContainer()
-) -> int:
-    """Compute a hash for a node, such that equivalent nodes should get the same hash.
+    renamed_variable = variable.upper() if static else variable.lower()
+    renamed_variable = re.sub("_{1,}", "_", renamed_variable)
 
-    For example, the expressions (lambda x: x) and (lambda y: y) should get the same hash.
+    if renamed_variable.endswith("_"):
+        renamed_variable = renamed_variable[:-1]
 
-    Args:
-        node (ast.AST): AST to hash.
-        preserved_callable_names (Collection[str], optional): Names to preserve. By default all names.
+    if private and not _is_private(renamed_variable):
+        renamed_variable = f"_{renamed_variable}"
+    if not private and _is_private(renamed_variable):
+        renamed_variable = renamed_variable.lstrip("_")
 
-    Returns:
-        int: Hash of node.
-    """
-    name_increment = 0
-    name_hashes = {}
+    if renamed_variable:
+        return renamed_variable
 
-    things_to_hash = []
-    for child in ast.walk(node):
-        things_to_hash.append(type(child))
-        names = []
-        if isinstance(child, ast.Name):
-            names = [child.id]
-        elif isinstance(child, ast.arg):
-            names = [child.arg]
-        elif isinstance(child, (ast.FunctionDef, ast.AsyncFunctionDef)):
-            names = [child.name]
-        else:
-            things_to_hash.extend(
-                (key, value)
-                for key, value in child.__dict__.items()
-                if isinstance(value, (str, int))
-                if key not in {"lineno", "end_lineno", "col_offset", "end_col_offset"}
+    raise RuntimeError(f"Unable to find a replacement name for {variable}")
+
+
+def _rename_class(name: str, *, private: bool) -> str:
+    name = re.sub("_{1,}", "_", name)
+    if len(name) == 0:
+        raise ValueError("Cannot rename empty name")
+    if len(name) == 1:
+        name = name.upper()
+    else:
+        accum = (last := name[0].upper())
+        for char in name[1:]:
+            if last == "_":
+                accum += (last := char.upper())
+            else:
+                accum += char
+            last = char
+
+        name = accum
+
+    if private and not _is_private(name):
+        return f"_{name}"
+    if not private and _is_private(name):
+        return name[1:]
+
+    return name
+
+
+def _get_uses_of(node: ast.AST, scope: ast.AST, content: str) -> Iterable[ast.Name]:
+    name = node.id if isinstance(node, ast.Name) else node.name
+    reference_nodes = {
+        refnode
+        for refnode in ast.walk(scope)
+        if isinstance(refnode, ast.Name)
+        and isinstance(refnode.ctx, ast.Load)
+        and refnode.id == name
+    }
+    if isinstance(node, ast.Name):
+        start = (node.lineno, node.col_offset)
+        end = (node.end_lineno, node.end_col_offset)
+    elif isinstance(node, (ast.ClassDef, ast.AsyncFunctionDef, ast.FunctionDef)):
+        start_charno, end_charno = _get_func_name_start_end(node, content)
+        start = (node.lineno, start_charno)
+        end = (node.lineno, end_charno)
+    else:
+        raise NotImplementedError(f"Unknown type: {type(node)}")
+    for refnode in reference_nodes:
+        n_start = (refnode.lineno, refnode.col_offset)
+        n_end = (refnode.end_lineno, refnode.end_col_offset)
+        if end < n_start:
+            yield refnode
+        elif isinstance(node, (ast.Module, ast.ClassDef)) and n_end < start:
+            yield refnode
+
+
+def _get_variable_name_substitutions(ast_tree: ast.AST, content: str) -> Mapping[ast.AST, str]:
+    renamings = collections.defaultdict(set)
+    classdefs: List[parsing.Statement] = []
+    funcdefs: List[parsing.Statement] = []
+    for node in parsing.iter_classdefs(ast_tree):
+        name = node.name
+        substitute = _rename_class(name, private=_is_private(name))
+        classdefs.append(node)
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, content):
+            renamings[refnode].add(substitute)
+
+    for node in parsing.iter_funcdefs(ast_tree):
+        name = node.name
+        substitute = _rename_variable(name, private=_is_private(name), static=False)
+        funcdefs.append(node)
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, content):
+            renamings[refnode].add(substitute)
+
+    for node in parsing.iter_assignments(ast_tree):
+        substitute = _rename_variable(node.id, private=_is_private(node.id), static=True)
+        renamings[node].add(substitute)
+        for refnode in _get_uses_of(node, ast_tree, content):
+            renamings[refnode].add(substitute)
+
+    while funcdefs or classdefs:
+        for partial_tree in classdefs.copy():
+            classdefs.remove(partial_tree)
+            for node in parsing.iter_classdefs(partial_tree):
+                name = node.name
+                classdefs.append(node)
+                substitute = _rename_class(name, private=_is_private(name))
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_funcdefs(partial_tree):
+                name = node.name
+                if name.startswith("__") and name.endswith("__"):
+                    continue
+                funcdefs.append(node)
+                substitute = _rename_variable(name, private=_is_private(name), static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_assignments(partial_tree):
+                name = node.id
+                substitute = _rename_variable(name, private=_is_private(name), static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+        for partial_tree in funcdefs.copy():
+            funcdefs.remove(partial_tree)
+            for node in parsing.iter_classdefs(partial_tree):
+                name = node.name
+                classdefs.append(node)
+                substitute = _rename_class(name, private=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_funcdefs(partial_tree):
+                name = node.name
+                funcdefs.append(node)
+                substitute = _rename_variable(name, private=False, static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+            for node in parsing.iter_assignments(partial_tree):
+                name = node.id
+                substitute = _rename_variable(name, private=False, static=False)
+                renamings[node].add(substitute)
+                for refnode in _get_uses_of(node, partial_tree, content):
+                    renamings[refnode].add(substitute)
+
+    return renamings
+
+
+def _get_variable_re_pattern(variable) -> str:
+    return r"(?<![A-Za-z_\.])" + variable + r"(?![A-Za-z_])"
+
+
+def _get_func_name_start_end(
+    node: Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef], content: str
+) -> Tuple[int, int]:
+    start, end = parsing.get_charnos(node, content)
+    codeblock = content[start:end]
+    for match in re.finditer(_get_variable_re_pattern(node.name), codeblock):
+        if match.group() == node.name:
+            end = start + match.end()
+            start += match.start()
+            return start, end
+
+    raise RuntimeError(f"Cannot find {node.name} in code block:\n{codeblock}")
+
+
+def _fix_variable_names(
+    content: str,
+    renamings: Mapping[ast.AST, str],
+    preserve: Collection[str] = frozenset(),
+) -> str:
+    replacements = []
+    for node, substitutes in renamings.items():
+        if len(substitutes) != 1:
+            raise RuntimeError(
+                f"Expected 1 substitute, got {len(substitutes)}: {substitutes}\nCode:\n{ast.dump(node, indent=2)}"
             )
-        for name in names:
-            if name in preserved_callable_names:
-                things_to_hash.append(name)
+        substitute = substitutes.pop()
+        if isinstance(node, ast.Name):
+            if node.id != substitute and node.id not in preserve:
+                start, end = parsing.get_charnos(node, content)
+                replacements.append((start, end, substitute))
+            continue
 
-                continue
+        if node.name == substitute or node.name in preserve:
+            continue
 
-            if name in name_hashes:
-                things_to_hash.append(name_hashes[name])
+        if not isinstance(node, (ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef)):
+            raise TypeError(f"Unknown type: {type(node)}")
 
-                continue
+        start, end = _get_func_name_start_end(node, content)
 
-            name_increment += 1
-            name_hashes[name] = name_increment
-            things_to_hash.append(name_increment)
+        replacements.append((start, end, substitute))
 
-    return hash(tuple(things_to_hash))
+    for start, end, substitute in sorted(set(replacements), reverse=True):
+        print(f"Replacing {content[start:end]} with {substitute}")
+        content = content[:start] + substitute + content[end:]
 
+    return content
 
-def _possible_external_effects(node: ast.AST, safe_callables: Collection[str]) -> Iterable[ast.AST]:
-    """Things that could possibly happen when going into a node
 
-    Args:
-        node (ast.AST): Ast node to enter
-        safe_callables (Collection[str]): Function names that are safe to call
+def _fix_undefined_variables(content: str, variables: Collection[str]) -> str:
+    variables = set(variables)
 
-    Yields:
-        ast.AST: Node that could potentially be encountered, and that may have some effect.
-    """
-    comprehension_local_vars = {comp.target for comp in core.walk(node, ast.comprehension)}
-    for child in core.walk(
-        node, (ast.Name(ctx=ast.Store), ast.Subscript(ctx=ast.Store, value=ast.Name))
-    ):
-        if child not in comprehension_local_vars:
-            yield child
-    halting_types = (ast.Yield, ast.YieldFrom, ast.Continue, ast.Break, ast.Return)
-    for child in core.walk(node, halting_types):
-        yield child
-    for child in core.walk(node, ast.Call):
-        if not (isinstance(child.func, ast.Name) and child.func.id in safe_callables):
-            yield child
-
-
-def _definite_external_effects(
-    node: ast.AST, safe_callables: Collection[str]
-) -> Iterable[Sequence[ast.AST]]:
-    """Things that will surely happen when going into a node
-
-    Args:
-        node (ast.AST): Ast node to enter
-        safe_callables (Collection[str]): Function names that are safe to call
-
-    Yields:
-        ast.AST: Node that will be encountered, and that may have some effect.
-    """
-    if isinstance(node, (ast.Break, ast.Continue)):
-        yield node
-        return
-    if not isinstance(node, (ast.If, ast.IfExp)):
-        yield from _possible_external_effects(node, safe_callables)
-        return
-
-    body_effects = {}
-    for child in node.body:
-        body_effects.update({
-            hash_node(n, safe_callables): n
-            for n in _definite_external_effects(child, safe_callables)
-        })
-        if core.is_blocking(node):
-            break
-    orelse_effects = {}
-    for child in node.body:
-        orelse_effects.update({
-            hash_node(n, safe_callables): n
-            for n in _definite_external_effects(child, safe_callables)
-        })
-        if core.is_blocking(node):
-            break
-    for key in body_effects.keys() & orelse_effects:
-        yield body_effects[key]
-
-
-def _definite_stored_names(node: ast.AST) -> Iterable[str]:
-    for child in _definite_external_effects(node, _EverythingContainer()):
-        if core.match_template(child, ast.Name(ctx=ast.Store)):
-            yield child.id
-        elif core.match_template(child, ast.Subscript(ctx=ast.Store, value=ast.Name)):
-            yield child.value.id
-
-
-def _hashable_node_purpose_type(node: ast.AST) -> Tuple[str]:
-    if isinstance(node, (ast.Continue, ast.Break)):
-        return (type(node),)
-    if isinstance(node, (ast.Assign, ast.AnnAssign, ast.AugAssign, ast.NamedExpr, ast.If)):
-        side_effects = [
-            child.value if isinstance(child, ast.Subscript) else child
-            for child in _possible_external_effects(node, _EverythingContainer())
-        ]
-        if all(isinstance(child, ast.Name) for child in side_effects):
-            stored_names = set(_definite_stored_names(node))
-            if all(effect.id in stored_names for effect in side_effects):
-                return tuple([ast.Assign] + sorted(stored_names))
-        elif all(isinstance(node, ast.Break) for node in side_effects):
-            return (ast.Break,)
-        elif all(isinstance(node, ast.Continue) for node in side_effects):
-            return (ast.Continue,)
+    lines = content.splitlines()
+    change_count = -len(lines)
+    lineno = next(
+        i
+        for i, line in enumerate(lines)
+        if not line.startswith("#")
+        and not line.startswith("'''")
+        and not line.startswith('"""')
+        and not line.startswith("from __future__ import")
+    )
+    for package, package_variables in ASSUMED_SOURCES.items():
+        overlap = variables.intersection(package_variables)
+        if overlap:
+            fix = f"from {package} import " + ", ".join(sorted(overlap))
+            print(f"Inserting '{fix}' at line {lineno}")
+            lines.insert(lineno, fix)
 
-        raise ValueError(f"Node {node} of type {type(node)} has no singular purpose")
+    for package in ASSUMED_PACKAGES & variables:
+        fix = f"import {package}"
+        print(f"Inserting '{fix}' at line {lineno}")
+        lines.insert(lineno, fix)
 
-    raise NotImplementedError(f"Cannot determine hashable node type of node of type {type(node)}")
+    for alias in PACKAGE_ALIASES.keys() & variables:
+        package = PACKAGE_ALIASES[alias]
+        fix = f"import {package} as {alias}"
+        print(f"Inserting '{fix}' at line {lineno}")
+        lines.insert(lineno, fix)
 
+    change_count += len(lines)
 
-def _group_nodes_by_purpose(body: Sequence[ast.AST]) -> Iterable[Sequence[ast.AST]]:
-    """Group nodes by common purpose
+    assert change_count >= 0
 
-    Args:
-        body (Sequence[ast.AST]): Sequence of ast nodes to group ifs in.
-        preserved_callable_names (Collection[str]): Callable names that should be preserved.
+    if change_count == 0:
+        return content
 
-    Yields:
-        Sequence[ast.AST]: A number of ifs that occur in sequence, and that have the same body.
-    """
-    if len(body) <= 1:
-        return
+    return "\n".join(lines) + "\n"
 
-    hashes = []
-    for child in body:
-        try:
-            hashes.append(_hashable_node_purpose_type(child))
-        except (NotImplementedError, ValueError):
-            hashes.append(None)
 
-    nodes = []
-    iterator = iter(range(len(body)))
-    i = next(iterator)
-    if hashes[i] is not None:
-        nodes.append(body[i])
+def define_undefined_variables(content: str) -> str:
+    """Attempt to find imports matching all undefined variables.
 
-    for i in iterator:
-        use = hashes[i] is not None
-        append = hashes[i] == hashes[i - 1]
+    Args:
+        content (str): Python source code
 
-        if use and append:
-            nodes.append(body[i])
-        elif use:
-            if nodes:
-                yield nodes
-            nodes = [body[i]]
+    Returns:
+        str: Source code with added imports
+    """
+    undefined_variables = _get_undefined_variables(content)
+    if undefined_variables:
+        return _fix_undefined_variables(content, undefined_variables)
 
-    if nodes:
-        yield nodes
+    return content
 
 
-def _build_function_body(
-    nodes: Sequence[ast.AST], return_injection_type: ast.AST
-) -> ast.FunctionDef:
-    """Build function from nodes.
+def _recursive_attribute_name(attribute: ast.Attribute) -> str:
+    if isinstance(attribute.value, ast.Attribute):
+        return f"{_recursive_attribute_name(attribute.value)}.{attribute.attr}"
+    return f"{attribute.value.id}.{attribute.attr}"
 
-    All effects should assign the same variable, or call the same function.
 
-    Args:
-        node_effects (Sequence[Tuple[ast.AST, ast.AST]]): Tuples of (test, effect)
+def _get_unused_imports(ast_tree: ast.Module) -> str:
 
-    Raises:
-        NotImplementedError: If all effects are not of type (Assign, Break, Continue, Call)
+    names = set()
+    attributes = set()
+    imports = set()
+    for node in ast.walk(ast_tree):
+        if isinstance(node, ast.Name) and isinstance(node.ctx, ast.Load):
+            names.add(node)
+        elif isinstance(node, ast.Attribute):
+            attributes.add(node)
+        elif isinstance(node, (ast.Import, ast.ImportFrom)):
+            if isinstance(node, ast.ImportFrom) and node.module == "__future__":
+                continue
+            for alias in node.names:
+                imports.add(alias.name if alias.asname is None else alias.asname)
 
-    Returns:
-        FunctionDef: Function created from effects
-    """
-    body = []
-    for node in nodes:
-        if return_injection_type is not None and isinstance(node, return_injection_type):
-            if return_injection_type == ast.Continue:
-                body.append(ast.Return(value=ast.Constant(value=False, kind=None)))
-            elif return_injection_type == ast.Break:
-                body.append(ast.Return(value=ast.Constant(value=True, kind=None)))
-            elif return_injection_type == ast.Assign:
-                # The purpose of the function is just to assign some variable, so we return
-                # whatever it would have been assigned to.
-                body.append(ast.Return(value=node.value))
-            else:
-                raise NotImplementedError(f"Unknown injection type: {return_injection_type}")
-        elif isinstance(node, ast.If):
-            body.append(
-                ast.If(
-                    test=node.test,
-                    body=_build_function_body(node.body, return_injection_type),
-                    orelse=_build_function_body(node.orelse, return_injection_type),
-            ))
-        elif isinstance(node, ast.With):
-            body.append(
-                ast.With(
-                    items=node.items, body=_build_function_body(node.body, return_injection_type)
-            ))
-        elif isinstance(node, ast.For):
-            body.append(
-                ast.For(
-                    target=node.target,
-                    iter=node.iter,
-                    body=node.body,
-                    orelse=_build_function_body(node.orelse, return_injection_type),
-            ))
-        elif isinstance(node, ast.While):
-            body.append(
-                ast.While(
-                    test=node.test,
-                    body=node.body,
-                    orelse=_build_function_body(node.orelse, return_injection_type),
-            ))
+    used_names = {name.id for name in names}
+    for attribute in attributes:
+        try:
+            full_name = _recursive_attribute_name(attribute)
+        except AttributeError:
+            continue
+
+        used_names.add(full_name)
+        while "." in full_name:
+            full_name = re.sub(r"\.[^\.]*$", "", full_name)
+            used_names.add(full_name)
+
+    return imports - used_names
+
+
+def _get_unused_imports_split(
+    ast_tree: ast.Module, unused_imports: Collection[str]
+) -> Tuple[
+    Collection[Union[ast.Import, ast.ImportFrom]],
+    Collection[Union[ast.Import, ast.ImportFrom]],
+]:
+    import_unused_aliases = collections.defaultdict(set)
+    for node in ast.walk(ast_tree):
+        if isinstance(node, (ast.Import, ast.ImportFrom)):
+            for alias in node.names:
+                used_name = alias.name if alias.asname is None else alias.asname
+                if used_name in unused_imports:
+                    import_unused_aliases[node].add(alias)
+
+    partially_unused_imports = set()
+    completely_unused_imports = set()
+
+    for node, unused_aliases in import_unused_aliases.items():
+        if set(node.names) - unused_aliases:
+            partially_unused_imports.add(node)
         else:
-            body.append(node)
+            completely_unused_imports.add(node)
 
-    return body
+    return completely_unused_imports, partially_unused_imports
 
 
-def _get_function_insertion_lineno(
-    containing_node: ast.AST, function_def_linenos: Collection[int], import_linenos: Collection[int]
-) -> int:
-    """Get line number to insert new function at.
+def _construct_import_statement(
+    node: Union[ast.Import, ast.ImportFrom], unused_imports: Collection[str]
+) -> str:
+    statement = "import " + ", ".join(
+        sorted(
+            alias.name if alias.asname is None else f"{alias.name} as {alias.asname}"
+            for alias in node.names
+            if (alias.name if alias.asname is None else alias.asname) not in unused_imports
+        )
+    )
+    if isinstance(node, ast.Import):
+        return statement
 
-    Args:
-        containing_node (ast.AST): Node that originally contained the logic in the function.
-        function_def_linenos (Collection[int]): Line numbers of function defs.
-        import_linenos (Collection[int]): Line numbers of imports.
+    return f"from {node.module} {statement}"
 
-    Returns:
-        int: Line number to insert function definition at
-    """
-    if isinstance(containing_node, ast.Module):
-        if function_def_linenos:
-            return min(function_def_linenos) - 1
-        if import_linenos:
-            return max(import_linenos) + 1
 
-        return 1
+def _remove_unused_imports(
+    ast_tree: ast.Module, content: str, unused_imports: Collection[str]
+) -> str:
+    completely_unused_imports, partially_unused_imports = _get_unused_imports_split(
+        ast_tree, unused_imports
+    )
+    if completely_unused_imports:
+        content = remove_nodes(content, completely_unused_imports, ast_tree)
+        if not partially_unused_imports:
+            return content
+        ast_tree = ast.parse(content)
+        completely_unused_imports, partially_unused_imports = _get_unused_imports_split(
+            ast_tree, unused_imports
+        )
 
-    if containing_node.lineno in function_def_linenos:
-        return containing_node.lineno - 1
+    if completely_unused_imports:
+        raise RuntimeError("Failed to remove unused imports")
 
-    if function_def_linenos:
-        if all((lineno > containing_node.lineno for lineno in function_def_linenos)):
-            return max(import_linenos) if import_linenos else containing_node.lineno - 1
+    # For every import, construct what we would like it to look like with redundant stuff removed, find the old
+    # version of it, and replace it.
 
-        return (
-            max((lineno for lineno in function_def_linenos if lineno <= containing_node.lineno)) - 1
-        )
+    # Iterate from bottom to top of file, so we don't have to re-calculate the linenos etc.
+    for node in sorted(
+        partially_unused_imports,
+        key=lambda n: (n.lineno, n.col_offset, n.end_lineno, n.end_col_offset),
+        reverse=True,
+    ):
+        start, end = parsing.get_charnos(node, content)
+        code = content[start:end]
+        replacement = _construct_import_statement(node, unused_imports)
+        print(f"Replacing:\n{code}\nWith:\n{replacement}")
+        content = content[:start] + replacement + content[end:]
 
-    if import_linenos:
-        return max(import_linenos) + 1
+    return content
 
-    return containing_node.lineno - 1
 
+def remove_unused_imports(content: str) -> str:
+    """Remove unused imports from source code.
 
-def _get_constant_insertion_lineno(scope: ast.AST) -> int:
-    import_types = (ast.Import, ast.ImportFrom)
-    imports = [node for node in scope.body if not isinstance(node, import_types)]
-    return min((node.lineno for node in imports)) - 1
+    Args:
+        content (str): Python source code
 
+    Returns:
+        str: Source code, with added imports removed
+    """
+    ast_tree = ast.parse(content)
+    unused_imports = _get_unused_imports(ast_tree)
+    if unused_imports:
+        content = _remove_unused_imports(ast_tree, content, unused_imports)
 
-def create_abstractions(source: str) -> str:
-    root = core.parse(source)
-    global_names = (
-        _scoped_dependencies(root) | tracing.get_imported_names(root) | constants.BUILTIN_FUNCTIONS
-    )
-    for node in parsing.iter_funcdefs(root):
-        global_names.add(node.name)
-    for node in parsing.iter_classdefs(root):
-        global_names.add(node.name)
-    replacements = {}
-    additions = []
-    removals = []
-    abstraction_count = 0
-
-    function_def_linenos = []
-    import_linenos = []
-
-    for node in core.walk(root, (ast.AsyncFunctionDef, ast.FunctionDef)):
-        candidates = [node.lineno] + [x.lineno for x in node.decorator_list]
-        function_def_linenos.append(min(candidates))
-    for node in core.walk(root, (ast.Import, ast.ImportFrom)):
-        import_linenos.append(node.lineno)
-
-    for node in itertools.chain([root], parsing.iter_bodies_recursive(root)):
-        for nodes in _group_nodes_by_purpose(node.body):
-            if len(nodes) > len(node.body) - 2:
-                continue
-            if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)) and all(
-                core.match_template(child, (ast.Return, ast.Expr(value=ast.Constant)))
-                or child in nodes
-                for child in node.body
-            ):
-                continue
+    return content
 
-            purposes = {_hashable_node_purpose_type(child) for child in nodes}
-            assert len(purposes) == 1
-            purpose = purposes.pop()
 
-            if core.match_template(nodes, [(ast.Assign, ast.AnnAssign)]):
-                continue
+def fix_rmspace(content: str) -> str:
+    """Remove trailing whitespace from source code.
 
-            children_with_purpose = sum(
-                isinstance(grandchild, purpose[0])
-                for child in nodes
-                for grandchild in ast.walk(child)
-            )
-            if children_with_purpose <= 2:
-                continue
+    Args:
+        content (str): Python source code
 
-            created_names, _, required_names = tracing.code_dependencies_outputs(nodes)
-            if len(created_names) > 1:
-                continue
+    Returns:
+        str: Source code, without trailing whitespace
+    """
+    return rmspace.format_str(content)
 
-            abstraction_count += 1
-            function_name = f"_pyrefact_abstraction_{abstraction_count}"
-            while function_name in global_names:
-                abstraction_count += 1
-                function_name = f"_pyrefact_abstraction_{abstraction_count}"
-
-            args = sorted(
-                required_names
-                - (global_names - _scoped_dependencies(root) if node is root else global_names)
-            )
-            # Abstractions with too many arguments are bad
-            if len(args) > 4:
-                continue
 
-            call_args = [ast.Name(id=arg, ctx=ast.Load()) for arg in args]
-            signature_args = ast.arguments(
-                posonlyargs=[],
-                args=[ast.arg(arg=arg, annotation=None) for arg in args],
-                vararg=None,
-                kwonlyargs=[],
-                kw_defaults=None,
-                kwarg=None,
-                defaults=[],
-            )
-            return_args = sorted(set(created_names))
+def fix_black(content: str) -> str:
+    """Format source code with black.
 
-            if set(args) & {"self", "cls"}:  # Not implemented
-                continue
+    Args:
+        content (str): Python source code
 
-            call = ast.Call(
-                func=ast.Name(id=function_name, ctx=ast.Load()),
-                args=call_args,
-                keywords=[],
-                starargs=[],
-                kwargs=[],
-            )
+    Returns:
+        str: Source code, formatted with black
+    """
+    return black.format_str(content, mode=black.Mode(line_length=100))
 
-            if purpose[0] in (ast.Continue, ast.Break):
-                if purpose[0] == ast.Continue:
-                    call = ast.UnaryOp(op=ast.Not(), operand=call)
-                function_call = ast.If(
-                    test=call, body=[purpose[0](col_offset=nodes[0].col_offset + 4)], orelse=[]
-                )
-                return_value = purpose[0] == ast.Continue
-                function_body = _build_function_body(nodes, purpose[0]) + [
-                    ast.Return(value=ast.Constant(value=return_value, kind=None))
-                ]
-                returns = ast.Name(id="bool", ctx=ast.Load())
-
-            elif purpose[0] == ast.Assign:
-                assign_targets = [ast.Name(id=arg, ctx=ast.Store()) for arg in return_args]
-                return_targets = [ast.Name(id=arg, ctx=ast.Load()) for arg in return_args]
-                if len(assign_targets) > 1:
-                    assign_targets = [ast.Tuple(elts=assign_targets)]
-                    return_targets = [ast.Tuple(elts=return_targets)]
-                function_call = ast.Assign(
-                    targets=assign_targets, value=call, lineno=nodes[0].lineno
-                )
-                ifs = [c for n in nodes for c in core.walk(n, ast.If)]
 
-                pure_nested_if = len(nodes) == 1 and all(
-                    len(n.body) == len(n.orelse) == 1 for n in ifs
-                )
-                function_body = _build_function_body(nodes, purpose[0] if pure_nested_if else None)
-                if not pure_nested_if:
-                    if not isinstance(nodes[0], (ast.Assign, ast.AnnAssign)) and not all(
-                        len(n.body) == len(n.orelse) == 1 for n in core.walk(nodes[0], ast.If)
-                    ):
-                        continue
-                    function_body.append(ast.Return(value=return_targets))
-                returns = None
+def fix_isort(content: str, *, line_length: int = 100) -> str:
+    """Format source code with isort
 
-            else:
-                continue
+    Args:
+        content (str): Python source code
+        line_length (int, optional): Line length. Defaults to 100.
 
-            insertion_lineno = _get_function_insertion_lineno(
-                node, function_def_linenos, import_linenos
-            )
+    Returns:
+        str: Source code, formatted with isort
+    """
+    return isort.code(content, config=isort.Config(profile="black", line_length=line_length))
 
-            function_def = ast.FunctionDef(
-                name=function_name,
-                args=signature_args,
-                body=function_body,
-                decorator_list=[],
-                type_params=[],
-                returns=returns,
-                lineno=insertion_lineno,
-                end_lineno=insertion_lineno + len(function_body),  # This isn't necessarily accurate
-                col_offset=0,  # May be inaccurate
-                end_col_offset=0,  # Definitely inaccurate
-            )
 
-            if isinstance(function_call, ast.Assign) and not return_args:
-                continue  # Probably a property of an input arg being modified, I don't particularly like these anyways
+def align_variable_names_with_convention(
+    content: str, preserve: Collection[str] = frozenset()
+) -> str:
+    """Align variable names with normal convention
 
-            if isinstance(function_call, (ast.Continue, ast.Break)) and len(return_args) != 1:
-                raise RuntimeError("Found bool abstraction without return")
+    Class names should have CamelCase names
+    Non-static variables and functions should have snake_case names
+    Static variables should have UPPERCASE_UNDERSCORED names
 
-            after_nodes = False
-            nodes_after_abstraction = []
-            for child in node.body:
-                if after_nodes:
-                    nodes_after_abstraction.append(child)
-                elif child is nodes[-1]:
-                    after_nodes = True
-
-            is_singular_return_reassignment = (
-                isinstance(function_call, ast.Assign)
-                and len(return_args) == 1
-                and core.match_template(
-                    nodes_after_abstraction,
-                    [(
-                        ast.Return(value=ast.Name),
-                        ast.Expr(
-                            value=(ast.Yield(value=ast.Name), ast.YieldFrom(value=ast.Name))
-            ),)],))
+    All names defined in global scope may be private and start with a single underscore
+    Names outside global scope are never allowed to be private
+    __magic__ names may only be defined in global scope
 
-            if is_singular_return_reassignment and isinstance(
-                nodes_after_abstraction[0], ast.Return
-            ):
-                col_offset = nodes[0].col_offset
-                lineno = nodes[0].lineno
-                for i, child in enumerate(function_body):
-                    child.lineno = lineno + i
-                    child.col_offset = col_offset
-                removals.extend(nodes)
-                additions.extend(function_body)
-                continue
+    Args:
+        content (str): Python source code
 
-            if not is_singular_return_reassignment:
-                replacements[nodes[0]] = function_call
-                removals.extend(nodes[1:])
-                additions.append(function_def)
-                continue
+    Returns:
+        str: Source code, where all variable names comply with normal convention
+    """
+    ast_tree = ast.parse(content)
+    renamings = _get_variable_name_substitutions(ast_tree, content)
 
-            if isinstance(nodes_after_abstraction[0], ast.Return):
-                inlined_return_call = ast.Return(
-                    value=function_call.value, lineno=function_call.lineno
-                )
-            else:
-                inlined_return_call = ast.Expr(
-                    type(nodes_after_abstraction[0].value)(value=function_call.value),
-                    lineno=function_call.lineno,
-                )
-            replacements[nodes_after_abstraction[0]] = inlined_return_call
-            removals.extend(nodes)
-            additions.append(function_def)
+    if renamings:
+        content = _fix_variable_names(content, renamings, preserve)
 
-    return processing.alter_code(
-        source, root, additions=additions, removals=removals, replacements=replacements
-    )
+    return content
+
+
+def _iter_bodies_recursive(
+    ast_root: ast.Module,
+) -> Iterable[Union[ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef]]:
+    left = list(ast_root.body)
+    while left:
+        for node in left.copy():
+            left.remove(node)
+            if isinstance(
+                node,
+                (ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef, ast.For, ast.While, ast.With),
+            ):
+                left.extend(node.body)
+                yield node
+            if isinstance(node, ast.If):
+                left.extend(node.body)
+                left.extend(node.orelse)
+                yield node
+
+
+def _unique_assignment_targets(
+    node: Union[ast.Assign, ast.AnnAssign, ast.AugAssign, ast.For]
+) -> Collection[ast.Name]:
+    targets = set()
+    if isinstance(node, (ast.AugAssign, ast.AnnAssign, ast.For)):
+        for subtarget in ast.walk(node.target):
+            if isinstance(subtarget, ast.Name) and isinstance(subtarget.ctx, ast.Store):
+                targets.add(subtarget)
+        return targets
+    if isinstance(node, ast.Assign):
+        for target in node.targets:
+            for subtarget in ast.walk(target):
+                if isinstance(subtarget, ast.Name) and isinstance(subtarget.ctx, ast.Store):
+                    targets.add(subtarget)
+        return targets
+    raise TypeError(f"Expected Assignment type, got {type(node)}")
 
 
-def overused_constant(source: str, *, root_is_static: bool) -> str:
-    """Create variables for overused constants
+def undefine_unused_variables(content: str, preserve: Collection[str] = frozenset()) -> str:
+    """Remove definitions of unused variables
 
     Args:
-        source (str): Python source code
-        root_is_static (bool): True if the outermost scope is module-level
+        content (str): Python source code
+        preserve (Collection[str], optional): Variable names to preserve
 
     Returns:
-        str: Modified source code
+        str: Python source code, with no definitions of unused variables
     """
-    root = core.parse(source)
+    ast_tree = ast.parse(content)
+    renamings = collections.defaultdict(set)
+    imports = set()
+    for node in ast.walk(ast_tree):
+        if isinstance(node, (ast.Import, ast.ImportFrom)):
+            imports.update(alias.name for alias in node.names)
+
+    for def_node in itertools.chain(
+        [ast_tree],
+        parsing.iter_funcdefs(ast_tree),
+    ):
+        reference_nodes = {
+            node
+            for node in ast.walk(def_node)
+            if isinstance(node, ast.Name) and isinstance(node.ctx, ast.Load)
+        }
+        body = queue.PriorityQueue()
+        for node in def_node.body:
+            body.put((node.lineno, node, None))
+        while not body.empty():
+            _, node, containing_loop_node = body.get()
+            if isinstance(node, (ast.For, ast.While)):
+                for subnode in reversed(node.body):
+                    body.put((subnode.lineno, subnode, containing_loop_node or node))
+            elif isinstance(node, ast.If):
+                for subnode in node.body:
+                    body.put((subnode.lineno, subnode, containing_loop_node))
+                for subnode in node.orelse:
+                    body.put((subnode.lineno, subnode, containing_loop_node))
+            if isinstance(node, (ast.Assign, ast.AnnAssign, ast.AugAssign, ast.For)):
+                target_nodes = _unique_assignment_targets(node)
+                if not target_nodes:
+                    continue
+                target_names = {x.id for x in target_nodes}
+                referenced_names = set()
+                starts = []
+                ends = []
+                if containing_loop_node is not None:
+                    loop_start, loop_end = parsing.get_charnos(containing_loop_node, content)
+                else:
+                    loop_start = loop_end = -1
+                for target_node in target_nodes:
+                    s, e = parsing.get_charnos(target_node, content)
+                    starts.append(s)
+                    ends.append(e)
+                start = min(starts)
+                end = max(ends)
+                for refnode in reference_nodes:
+                    n_start, n_end = parsing.get_charnos(refnode, content)
+                    if (
+                        end < n_start
+                        or (isinstance(def_node, (ast.ClassDef, ast.Module)) and n_end < start)
+                        or isinstance(def_node, ast.For)
+                        or loop_start <= n_start <= n_end <= loop_end
+                    ):
+                        referenced_names.add(refnode.id)
+                redundant_targets = target_names - referenced_names - imports
+                if def_node is ast_tree:
+                    redundant_targets = redundant_targets - preserve
+                for target_node in target_nodes:
+                    if isinstance(target_node, ast.Attribute):
+                        target_node = target_node.value
+                    if target_node.id in redundant_targets:
+                        renamings[target_node].add("_")
+
+    if renamings:
+        content = _fix_variable_names(content, renamings, preserve)
+        ast_tree = ast.parse(content)
+
+    for node in ast.walk(ast_tree):
+        if isinstance(node, (ast.Assign, ast.AnnAssign, ast.AugAssign)):
+            target_nodes = _unique_assignment_targets(node)
+            target_names = {x.id for x in target_nodes}
+            if target_names == {"_"}:
+                code = parsing.get_code(node, content)
+                changed_code = re.sub(_REDUNDANT_UNDERSCORED_ASSIGN_RE_PATTERN, "", code)
+                if code != changed_code:
+                    print(f"Removing redundant assignments in {code}")
+                    content = content.replace(code, changed_code)
 
-    template = (
-        ast.Constant,
-        ast.Dict(keys={ast.Constant}, values={ast.Constant}),
-        ast.Set(elts={ast.Constant}),
-        ast.Tuple(elts={ast.Constant}),
-        ast.List(elts={ast.Constant}),
-    )
+    return content
 
-    candidates = set(core.walk(root, template))
 
-    for fstring in core.walk(root, ast.JoinedStr):
-        for node in core.walk(fstring, ast.AST):
-            candidates.discard(node)
-
-    # For every node, all scopes it can be found in
-    scope_node_definitions = collections.defaultdict(set)
-    for scope in itertools.chain([root], core.walk(root, (ast.FunctionDef, ast.AsyncFunctionDef))):
-        for node in core.walk(scope, ast.AST):
-            scope_node_definitions[node].add(scope)
-
-    for scope in itertools.chain([root], core.walk(root, ast.AST(body=list))):
-        if scope.body and core.match_template(scope.body[0], ast.Expr(value=ast.Constant)):
-            candidates.discard(scope.body[0].value)
-
-    code_node_mapping = collections.defaultdict(set)
-    for node in candidates:
-        code_node_mapping[core.unparse(node)].add(node)
-
-    replacements = {}
-    additions = set()
-
-    i = 0
-    names = {name.id.lower().strip("_") for name in core.walk(root, ast.Name)}
-    while f"pyrefact_overused_constant_{i}" in names and i < 10:
-        i += 1
+def remove_nodes(content: str, nodes: Iterable[ast.AST], root: ast.Module) -> str:
+    """Remove ast nodes from code
 
-    if f"pyrefact_overused_constant_{i}" in names:
-        return source
+    Args:
+        content (str): Python source code
+        nodes (Iterable[ast.AST]): Nodes to delete from code
+        root (ast.Module): Complete corresponding module
 
-    for code, nodes in sorted(code_node_mapping.items(), key=lambda t: t[0]):
-        if len(nodes) < 5:
-            continue
-        if len(re.sub(r"\s", "", code)) < 20:
+    Returns:
+        str: Code after deleting nodes
+    """
+    keep_mask = [True] * len(content)
+    nodes = list(nodes)
+    for node in nodes:
+        start, end = parsing.get_charnos(node, content)
+        print(f"Removing:\n{content[start:end]}")
+        keep_mask[start:end] = [False] * (end - start)
+        for decorator_node in getattr(node, "decorator_list", []):
+            start, end = parsing.get_charnos(decorator_node, content)
+            start -= 1  # The @ is missed otherwise
+            print(f"Removing:\n{content[start:end]}")
+            keep_mask[start:end] = [False] * (end - start)
+
+    passes = [len(content) + 1]
+
+    for node in ast.walk(root):
+        for bodytype in "body", "finalbody", "orelse":
+            if body := getattr(node, bodytype, []):
+                if isinstance(body, list) and all(child in nodes for child in body):
+                    print(f"Found empty {bodytype}")
+                    start_charno, _ = parsing.get_charnos(body[0], content)
+                    passes.append(start_charno)
+
+    heapq.heapify(passes)
+
+    next_pass = heapq.heappop(passes)
+    chars = []
+    for i, char, keep in zip(range(len(content)), content, keep_mask):
+        if i == next_pass:
+            chars.extend("pass")
+        elif next_pass < i < next_pass + 3:
             continue
+        else:
+            if i > next_pass:
+                next_pass = heapq.heappop(passes)
+            if keep:
+                chars.append(char)
 
-        common_scopes = set.intersection(*(scope_node_definitions[node] for node in nodes))
+    return "".join(chars)
 
-        # root is a Module and has no lineno
-        best_common_scope = max(
-            common_scopes, key=lambda node: getattr(node, "lineno", 1), default=root
-        )
-        variable_name = f"pyrefact_overused_constant_{i}"
-        variable_name = style.rename_variable(
-            variable_name, static=best_common_scope is root and root_is_static, private=False
-        )
 
-        name = ast.Name(id=variable_name)
-        assign = core.parse(f"{variable_name} = {code}").body[0]
-        assign.lineno = _get_constant_insertion_lineno(best_common_scope)
-        assign.col_offset = best_common_scope.body[0].col_offset
-        additions.add(assign)
-        replacements.update({node: name for node in nodes})
+def _compute_safe_funcdef_calls(root: ast.Module) -> Collection[str]:
+    """Compute what functions can safely be called without having a side effect.
 
-        i += 1
+    This is also to compute the inverse, i.e. what function calls may be removed
+    without breaking something.
 
-    return processing.alter_code(source, root, additions=additions, replacements=replacements)
+    Args:
+        root (ast.Module): Module to find function definitions in
 
+    Returns:
+        Collection[str]: Names of all functions that have no side effect when called.
+    """
+    defined_names = {
+        node.id
+        for node in ast.walk(root)
+        if isinstance(node, ast.Name) and isinstance(node.ctx, ast.Store)
+    }
+    function_defs = {
+        node for node in ast.walk(root) if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef))
+    }
+    builtin_names = set(dir(builtins))
+    safe_callables = builtin_names - {"print", "exit"}
+    safe_callable_nodes = set()
+    changes = True
+    while changes:
+        changes = False
+        for node in function_defs:
+            if node.name in defined_names:
+                continue
+            nonreturn_children = [
+                child
+                for child in node.body
+                if not isinstance(
+                    child,
+                    (ast.Return, ast.Yield, ast.YieldFrom, ast.Continue, ast.Break),
+                )
+            ]
+            if not any(
+                parsing.has_side_effect(child, safe_callables) for child in nonreturn_children
+            ):
+                safe_callable_nodes.add(node)
+                safe_callables.add(node.name)
+                changes = True
+        function_defs = {node for node in function_defs if node.name not in safe_callables}
+
+    for node in ast.walk(root):
+        if isinstance(node, ast.ClassDef):
+            constructors = {
+                child
+                for child in node.body
+                if isinstance(child, ast.FunctionDef)
+                and child.name in ("__init__", "__post_init__", "__new__")
+            }
+            if not constructors - safe_callable_nodes:
+                safe_callables.add(node.name)
 
-def simplify_if_control_flow(source: str) -> str:
-    root = core.parse(source)
+    return safe_callables
 
-    # This should run after the first run of breakout_common_code_in_ifs(), so that code that
-    # can be broken out without this having run first can be broken out first. That way, this
-    # doesn't trigger unless it enables breakout_common_code_in_ifs() to do work it wouldn't
-    # otherwise have done.
 
-    for node in core.walk(root, ast.If):
-        if not node.orelse:
-            continue
+def delete_pointless_statements(content: str) -> str:
+    """Delete pointless statements with no side effects from code
 
-        # Assignments make things more complicated. For example, the variables fed into the
-        # if body/orelse blocks may be mutated and then used later on, or they may be changed
-        # inside the node, etc. I won't deal with these cases for now.
-        if any(core.walk(node, (ast.Assign, ast.AnnAssign, ast.AugAssign, ast.NamedExpr))):
-            continue
+    Args:
+        content (str): Python source code.
 
-        node_body_names = sorted(
-            (name for n in node.body for name in core.walk(n, ast.Name)),
-            key=lambda n: (n.lineno, n.col_offset),
-        )
-        node_orelse_names = sorted(
-            (name for n in node.orelse for name in core.walk(n, ast.Name)),
-            key=lambda n: (n.lineno, n.col_offset),
-        )
-        if len(node_body_names) != len(node_orelse_names):
-            continue
+    Returns:
+        str: Modified code
+    """
+    ast_tree = ast.parse(content)
+    delete = []
+    safe_callables = _compute_safe_funcdef_calls(ast_tree)
+    for node in itertools.chain([ast_tree], _iter_bodies_recursive(ast_tree)):
+        for i, child in enumerate(node.body):
+            if not parsing.has_side_effect(child, safe_callables):
+                if i > 0 or not (
+                    isinstance(child, ast.Expr)
+                    and isinstance(child.value, ast.Constant)
+                    and isinstance(child.value.value, str)
+                ):
+                    delete.append(child)
+
+    content = remove_nodes(content, delete, ast_tree)
+
+    return content
+
+
+def _get_unused_functions_classes(root: ast.AST, preserve: Collection[str]) -> Iterable[ast.AST]:
+    funcdefs = []
+    classdefs = []
+    names = []
+
+    for node in ast.walk(root):
+        if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
+            funcdefs.append(node)
+        elif isinstance(node, ast.ClassDef):
+            classdefs.append(node)
+        elif isinstance(node, ast.Name) and isinstance(node.ctx, ast.Load):
+            names.append(node)
+
+    class_magics = collections.defaultdict(set)
+    for node in classdefs:
+        for child in node.body:
+            if (
+                isinstance(child, ast.FunctionDef)
+                and child.name.startswith("__")
+                and child.name.endswith("__")
+            ):
+                class_magics[node].add(child)
+
+    magic_source_classes = {}
+    for classdef, magics in class_magics.items():
+        for magic in magics:
+            magic_source_classes[magic] = classdef
 
-        differing_names_index_name_mapping = {
-            i: names
-            for i, names in enumerate(zip(node_body_names, node_orelse_names))
-            if len({n.id for n in names}) > 1
+    for def_node in funcdefs:
+        if def_node.name in preserve:
+            continue
+        usages = {node for node in names if node.id == def_node.name}
+        if parent_class := magic_source_classes.get(def_node):
+            usages.update(node for node in names if node.id == parent_class.name)
+        recursive_usages = {
+            node
+            for node in ast.walk(def_node)
+            if isinstance(node, ast.Name) and node.id == def_node.name
         }
-        something = collections.defaultdict(list)
-        for i, names in differing_names_index_name_mapping.items():
-            something[tuple(name.id for name in names)].append(i)
-
-        # Add definitions of new variables at start of if statements
-        # Replace all references to differing variables with new ones
-        # Then, breakout_common_code_in_ifs() should trigger on the
-        # identical code at the end of both branches and move it after
-        # the branches.
-
-        bodies = [node.body, node.orelse]
-
-        body_equivalent_function_srcs = [[
-            core.unparse(
-                ast.FunctionDef(
-                    name="func",
-                    args=ast.arguments(
-                        posonlyargs=[],
-                        args=[],
-                        vararg=None,
-                        kwonlyargs=[],
-                        kw_defaults=[],
-                        kwarg=None,
-                        defaults=[],
-                    ),
-                    body=body,
-                    decorator_list=[],
-                    type_params=[],
-                    returns=None,
-                    lineno=0,
-                    end_lineno=0 + len(body),
-                    col_offset=0,
-                    end_col_offset=0,
-            ))]  # Put as single element in list to emulate mutable string
-            for body in bodies
-        ]
+        if not usages - recursive_usages:
+            print(f"{def_node.name} is never used")
+            yield def_node
 
-        additions = set()
-        replacements = {}
-        for new_variable_number, (names, indexes) in enumerate(something.items()):
-            new_variable = ast.Name(id=f"var_{new_variable_number + 1}")
-            for src_list, body, name in zip(body_equivalent_function_srcs, bodies, names):
-                assign = ast.Assign(targets=[new_variable], value=ast.Name(id=name))
-                ast.copy_location(assign, body[0])
-                assign.lineno -= 1
-                additions.add(assign)
-
-                src_list[0] = src_list[0].replace(name, new_variable.id)
-
-            for index in indexes:
-                for name in differing_names_index_name_mapping[index]:
-                    replacements[name] = new_variable
-
-        # Check if replacing all names really made the code equivalent.
-        # This will be prone to false-negatives, in all kinds of ways, which is better
-        # than the opposite.
-        unique_srcs = {src_list[0] for src_list in body_equivalent_function_srcs}
-        if len(unique_srcs) != 1:
+    for def_node in classdefs:
+        if def_node.name in preserve:
             continue
+        usages = {node for node in names if node.id == def_node.name}
+        internal_usages = {
+            node
+            for node in ast.walk(def_node)
+            if isinstance(node, ast.Name)
+            and isinstance(node.ctx, ast.Load)
+            and node.id in (def_node.name, "self", "cls")
+        }
+        if not usages - internal_usages:
+            print(f"{def_node.name} is never used")
+            yield def_node
 
-        added_code_chars = sum(len(core.unparse(addition)) for addition in additions)
-        removed_code_chars = len(unique_srcs.pop())
 
-        if added_code_chars > removed_code_chars / 2:
-            continue
+def delete_unused_functions_and_classes(
+    content: str, preserve: Collection[str] = frozenset()
+) -> str:
+    """Delete unused functions and classes from code.
 
-        if additions and replacements:
-            source = processing.alter_code(
-                source,
-                root,
-                replacements=replacements,
-                additions=additions,
-                priority=("additions", "replacements"),
-            )
+    Args:
+        content (str): Python source code
+        preserve (Collection[str], optional): Names to preserve
+
+    Returns:
+        str: Python source code, where unused functions and classes have been deleted.
+    """
+    root = ast.parse(content)
+
+    delete = set(_get_unused_functions_classes(root, preserve))
 
-            return simplify_if_control_flow(source)
+    content = remove_nodes(content, delete, root)
 
-    return source
+    return content
```

