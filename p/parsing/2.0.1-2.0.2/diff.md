# Comparing `tmp/parsing-2.0.1.tar.gz` & `tmp/parsing-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsing-2.0.1.tar", last modified: Wed Jun 21 16:11:26 2023, max compression
+gzip compressed data, was "parsing-2.0.2.tar", last modified: Thu Jun 29 16:27:33 2023, max compression
```

## Comparing `parsing-2.0.1.tar` & `parsing-2.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.210492 parsing-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-21 16:11:22.000000 parsing-2.0.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-21 16:11:22.000000 parsing-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 16:11:22.000000 parsing-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-21 16:11:26.210492 parsing-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-21 16:11:22.000000 parsing-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.206492 parsing-2.0.1/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    68232 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/automaton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/glrparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/lrparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/module_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.210492 parsing-2.0.1/parsing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.210492 parsing-2.0.1/parsing/tests/specs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/a.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/b.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/h.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/specs/i.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-21 16:11:22.000000 parsing-2.0.1/parsing/tests/test_codestyle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:11:26.210492 parsing-2.0.1/parsing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 16:11:26.000000 parsing-2.0.1/parsing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-21 16:11:22.000000 parsing-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:11:26.210492 parsing-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-21 16:11:22.000000 parsing-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:33.542313 parsing-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 16:27:29.000000 parsing-2.0.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-29 16:27:29.000000 parsing-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 16:27:29.000000 parsing-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-29 16:27:33.542313 parsing-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-29 16:27:29.000000 parsing-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:33.538313 parsing-2.0.2/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68405 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/automaton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/glrparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/lrparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/module_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:33.542313 parsing-2.0.2/parsing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:33.542313 parsing-2.0.2/parsing/tests/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/specs/a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/specs/b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/specs/d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/specs/h.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/specs/i.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-29 16:27:29.000000 parsing-2.0.2/parsing/tests/test_codestyle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:33.538313 parsing-2.0.2/parsing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-29 16:27:33.000000 parsing-2.0.2/parsing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-29 16:27:33.000000 parsing-2.0.2/parsing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:27:33.000000 parsing-2.0.2/parsing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 16:27:33.000000 parsing-2.0.2/parsing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 16:27:33.000000 parsing-2.0.2/parsing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-29 16:27:29.000000 parsing-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:27:33.542313 parsing-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-29 16:27:29.000000 parsing-2.0.2/setup.py
```

### Comparing `parsing-2.0.1/LICENSE` & `parsing-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/PKG-INFO` & `parsing-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsing
-Version: 2.0.1
+Version: 2.0.2
 Summary: LR(1) parser generator for Python
 Home-page: http://www.canonware.com/Parsing/
 Author: Jason Evans
 Author-email: jasone@canonware.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `parsing-2.0.1/README.rst` & `parsing-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/__init__.py` & `parsing-2.0.2/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/_version.py` & `parsing-2.0.2/parsing/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 # The commit message MUST contain a properly formatted release
 # log, and the commit must be signed.
 #
 # The release automation will: build and test the packages for the
 # supported platforms, publish the packages on PyPI, merge the PR
 # to the target branch, create a Git tag pointing to the commit.
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
```

### Comparing `parsing-2.0.1/parsing/ast.py` & `parsing-2.0.2/parsing/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 with docstrings indicating the intended grammar, and will then be
 used in the parsing as part of the abstract syntax tree that is
 constructed in the process.
 """
 
 from __future__ import annotations
 
+from mypy_extensions import mypyc_attr
 
+
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class Symbol:
     pass
 
 
 class Nonterm(Symbol):
     """
     Non-terminal symbols have sets of productions associated with them.  The
```

### Comparing `parsing-2.0.1/parsing/automaton.py` & `parsing-2.0.2/parsing/automaton.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Iterable,
     Iterator,
     List,
     Optional,
     Tuple,
     Type,
 )
+from mypy_extensions import mypyc_attr
 
 import collections
 import inspect
 import time
 import types
 import pickle
 import sys
@@ -93,14 +94,15 @@
 
         # Cache the result.
         _firstSetCache[s] = firstSet = frozenset(result)
 
     return firstSet
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class ItemSet:
     def __init__(self, items: Iterable[Tuple[Item, set[SymbolSpec]]]) -> None:
         self._kernel: Dict[Item, set[SymbolSpec]] = {}
         self._added: Dict[Item, set[SymbolSpec]] = {}
         self._symMap: dict[SymbolSpec, set[Item]] = {}
         self._all: collections.ChainMap[
             Item, set[SymbolSpec]
@@ -212,17 +214,17 @@
     def closure(self) -> None:
         self._closeItems(self._kernel.items())
 
     # Calculate the kernel of the goto set, given a particular symbol.
     def goto(self, sym: SymbolSpec) -> ItemSet | None:
         items = self._symMap.get(sym)
         if items:
-            return ItemSet(
+            return ItemSet([
                 (i.production.item(i.dotPos + 1), self._all[i]) for i in items
-            )
+            ])
         else:
             return None
 
     # Merge the kernel of other into this ItemSet, then update the closure.
     # It is not sufficient to copy other's added items, since other has not
     # computed its closure.
     def merge(self, other: ItemSet) -> bool:
@@ -270,14 +272,15 @@
                     and isLookahead.isdisjoint(jsLookahead)
                     and ioLookahead.isdisjoint(joLookahead)
                 ):
                     return False
         return True
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class Spec(interfaces.Spec):
     """
     The Spec class contains the read-only data structures that the Parser
     class needs in order to parse input.  Parser generation results in a
     Spec instance, which can then be shared by multiple Parser instances."""
 
     __deletable__ = [
```

### Comparing `parsing-2.0.1/parsing/errors.py` & `parsing-2.0.2/parsing/errors.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/glrparser.py` & `parsing-2.0.2/parsing/glrparser.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/grammar.py` & `parsing-2.0.2/parsing/grammar.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,24 +34,27 @@
     List,
     Mapping,
     Optional,
     Tuple,
     Type,
 )
 
+from mypy_extensions import mypyc_attr
+
 import re
 import sys
 from parsing.ast import Token, Nonterm
 from parsing.errors import SpecError
 from parsing import introspection
 
 if TYPE_CHECKING:
     import types
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class PrecedenceSpec:
     assoc_tok_re: ClassVar[re.Pattern[str]] = re.compile(
         r"([<>=])([A-Za-z]\w*)"
     )
 
     def __init__(
         self,
@@ -79,19 +82,21 @@
             self.assoc,
             self.name,
             ",".join(equiv),
             ",".join(domin),
         )
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class PrecedenceRef(PrecedenceSpec):
     def __init__(self, name: str) -> None:
         super().__init__(name, "fail", {})
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class SymbolSpec:
     name: str
     prec: PrecedenceSpec
     firstSet: set[SymbolSpec]
     followSet: set[SymbolSpec]
 
     def __init__(self, name: str, prec: PrecedenceSpec) -> None:
@@ -118,14 +123,15 @@
         for sym in set:
             if sym != epsilon and sym not in self.followSet:
                 self.followSet.add(sym)
                 ret = False
         return ret
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class NontermSpec(SymbolSpec):
     token_re: ClassVar[re.Pattern[str]] = re.compile(r"([A-Za-z]\w*)")
     precedence_tok_re: ClassVar[re.Pattern[str]] = re.compile(
         r"\[([A-Za-z]\w*)\]"
     )
 
     def __init__(
@@ -189,25 +195,27 @@
         nonterm = NontermSpec(
             nt_subclass, symbol_name, f"{module_name}.{name}", prec
         )
         return nonterm, is_start
 
 
 # AKA terminal symbol.
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class TokenSpec(SymbolSpec):
     def __init__(
         self,
         tokenType: Type[Token],
         name: str,
         prec: PrecedenceSpec,
     ) -> None:
         super().__init__(name, prec)
         self.tokenType = tokenType
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class Item:
     production: Production
     dotPos: int
     symbol: Optional[SymbolSpec]
 
     def __init__(
         self,
@@ -256,14 +264,15 @@
 
         return "".join(strs)
 
 
 _item_cache: dict[tuple[Production, int], Item] = {}
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class Production:
     def __init__(
         self,
         method: Callable[..., Nonterm | None],
         qualified: str,
         prec: PrecedenceSpec,
         lhs: NontermSpec,
@@ -343,14 +352,15 @@
 
 
 class NontermStart(Nonterm):
     def reduce(self, userStartSym: SymbolSpec, eoi: EndOfInputSpec) -> None:
         pass
 
 
+@mypyc_attr(serializable=True, allow_interpreted_subclasses=True)
 class Action:
     """
     Abstract base class, subclassed by {Shift,Reduce}Action."""
 
     def __init__(self) -> None:
         pass
```

### Comparing `parsing-2.0.1/parsing/interfaces.py` & `parsing-2.0.2/parsing/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/lrparser.py` & `parsing-2.0.2/parsing/lrparser.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/module_spec.py` & `parsing-2.0.2/parsing/module_spec.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/tests/specs/a.py` & `parsing-2.0.2/parsing/tests/specs/a.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/tests/specs/b.py` & `parsing-2.0.2/parsing/tests/specs/b.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/tests/specs/d.py` & `parsing-2.0.2/parsing/tests/specs/d.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/tests/specs/h.py` & `parsing-2.0.2/parsing/tests/specs/h.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/tests/specs/i.py` & `parsing-2.0.2/parsing/tests/specs/i.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/tests/test_basic.py` & `parsing-2.0.2/parsing/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing/tests/test_codestyle.py` & `parsing-2.0.2/parsing/tests/test_codestyle.py`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/parsing.egg-info/PKG-INFO` & `parsing-2.0.2/parsing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsing
-Version: 2.0.1
+Version: 2.0.2
 Summary: LR(1) parser generator for Python
 Home-page: http://www.canonware.com/Parsing/
 Author: Jason Evans
 Author-email: jasone@canonware.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `parsing-2.0.1/parsing.egg-info/SOURCES.txt` & `parsing-2.0.2/parsing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/pyproject.toml` & `parsing-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsing-2.0.1/setup.py` & `parsing-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     else:
         raise RuntimeError(
             "unable to read the version from parsing/_version.py"
         )
 
 
 USE_MYPYC = False
-MYPY_DEPENDENCY = "mypy>=0.910"
+MYPY_DEPENDENCY = "mypy>=1.4.1"
 setup_requires = []
 ext_modules = []
 
 if (
     os.environ.get("PARSING_USE_MYPYC", None) in {"true", "1", "on"}
     or "--use-mypyc" in sys.argv
 ):
```

