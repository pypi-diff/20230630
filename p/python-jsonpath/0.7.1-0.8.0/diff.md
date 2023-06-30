# Comparing `tmp/python_jsonpath-0.7.1.tar.gz` & `tmp/python_jsonpath-0.8.0.tar.gz`

## Comparing `python_jsonpath-0.7.1.tar` & `python_jsonpath-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/__about__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/__init__.py
--rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/env.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/exceptions.py
--rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/filter.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/lex.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/match.py
--rw-r--r--   0        0        0    20477 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/parse.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/py.typed
--rw-r--r--   0        0        0    23699 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/selectors.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/stream.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/token.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/arguments.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/count.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/is_instance.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/keys.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/length.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/match.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/search.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/typeof.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/value.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/README.md
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/__about__.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/__init__.py
+-rw-r--r--   0        0        0    16812 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/env.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/exceptions.py
+-rw-r--r--   0        0        0    19524 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/filter.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/lex.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/match.py
+-rw-r--r--   0        0        0    20477 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/parse.py
+-rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/patch.py
+-rw-r--r--   0        0        0    13672 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/path.py
+-rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/pointer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/py.typed
+-rw-r--r--   0        0        0    24303 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/selectors.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/stream.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/token.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/arguments.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/count.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/is_instance.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/keys.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/length.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/match.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/search.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/typeof.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/jsonpath/function_extensions/value.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/README.md
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 python_jsonpath-0.8.0/PKG-INFO
```

### Comparing `python_jsonpath-0.7.1/jsonpath/env.py` & `python_jsonpath-0.8.0/jsonpath/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,37 +10,38 @@
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
-from typing import TextIO
 from typing import Type
 from typing import Union
 
 from . import function_extensions
 from .exceptions import JSONPathNameError
 from .exceptions import JSONPathSyntaxError
 from .filter import UNDEFINED
 from .function_extensions import validate
 from .lex import Lexer
+from .match import JSONPathMatch
 from .match import NodeList
 from .parse import Parser
 from .path import CompoundJSONPath
 from .path import JSONPath
 from .stream import TokenStream
 from .token import TOKEN_EOF
 from .token import TOKEN_INTERSECTION
 from .token import TOKEN_UNION
 from .token import Token
 
 if TYPE_CHECKING:
+    from io import IOBase
+
     from .match import FilterContextVars
-    from .match import JSONPathMatch
 
 
 class JSONPathEnvironment:
     """JSONPath configuration.
 
     This class contains settings for path tokenization, parsing and resolution
     behavior, plus convenience methods for matching an unparsed path to some
@@ -64,14 +65,18 @@
     - Setup built-in function extensions by overriding
       `setup_function_extensions()`
     - Hook in to mapping and sequence item getting by overriding `getitem()`.
     - Change filter comparison operator behavior by overriding `compare()`.
 
     ## Class attributes
 
+    Arguments:
+        filter_caching (bool): If `True`, filter expressions will be cached where
+            possible.
+
     Attributes:
         filter_context_token (str): The pattern used to select extra filter context
             data. Defaults to `"_"`.
         intersection_token (str): The pattern used as the intersection operator.
             Defaults to `"&"`.
         key_token (str): The pattern used to identify the current key or index when
             filtering a, mapping or sequence. Defaults to `"#"`.
@@ -102,16 +107,19 @@
 
     max_int_index = (2**53) - 1
     min_int_index = -(2**53) + 1
 
     # Override these to customize path tokenization and parsing.
     lexer_class: Type[Lexer] = Lexer
     parser_class: Type[Parser] = Parser
+    match_class: Type[JSONPathMatch] = JSONPathMatch
+
+    def __init__(self, *, filter_caching: bool = True) -> None:
+        self.filter_caching = filter_caching
 
-    def __init__(self) -> None:  # noqa: D107
         self.lexer: Lexer = self.lexer_class(env=self)
         """The lexer bound to this environment."""
 
         self.parser: Parser = self.parser_class(env=self)
         """The parser bound to this environment."""
 
         self.function_extensions: Dict[str, Callable[..., Any]] = {}
@@ -170,15 +178,15 @@
                     )
 
         return _path
 
     def findall(
         self,
         path: str,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """Find all objects in `data` matching the given JSONPath `path`.
 
         If `data` is a string or a file-like objects, it will be loaded
         using `json.loads()` and the default `JSONDecoder`.
@@ -192,21 +200,23 @@
 
         Returns:
             A list of matched objects. If there are no matches, the list will
                 be empty.
 
         Raises:
             JSONPathSyntaxError: If the path is invalid.
+            JSONPathTypeError: If a filter expression attempts to use types in
+                an incompatible way.
         """
         return self.compile(path).findall(data, filter_context=filter_context)
 
     def finditer(
         self,
         path: str,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> Iterable[JSONPathMatch]:
         """Generate `JSONPathMatch` objects for each match.
 
         If `data` is a string or a file-like objects, it will be loaded
         using `json.loads()` and the default `JSONDecoder`.
@@ -217,34 +227,66 @@
                 or `Mapping` interfaces.
             filter_context: Arbitrary data made available to filters using
                 the _filter context_ selector.
 
         Returns:
             An iterator yielding `JSONPathMatch` objects for each match.
 
-        Raises a `JSONPathSyntaxError` if the path is invalid.
+        Raises:
+            JSONPathSyntaxError: If the path is invalid.
+            JSONPathTypeError: If a filter expression attempts to use types in
+                an incompatible way.
         """
         return self.compile(path).finditer(data, filter_context=filter_context)
 
+    def match(
+        self,
+        path: str,
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
+        *,
+        filter_context: Optional[FilterContextVars] = None,
+    ) -> Union[JSONPathMatch, None]:
+        """Return a `JSONPathMatch` instance for the first object found in _data_.
+
+        `None` is returned if there are no matches.
+
+        Arguments:
+            path: The JSONPath as a string.
+            data: A JSON document or Python object implementing the `Sequence`
+                or `Mapping` interfaces.
+            filter_context: Arbitrary data made available to filters using
+                the _filter context_ selector.
+
+        Returns:
+            A `JSONPathMatch` object for the first match, or `None` if there were
+                no matches.
+
+        Raises:
+            JSONPathSyntaxError: If the path is invalid.
+            JSONPathTypeError: If a filter expression attempts to use types in
+                an incompatible way.
+        """
+        return self.compile(path).match(data, filter_context=filter_context)
+
     async def findall_async(
         self,
         path: str,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """An async version of `findall()`."""
         return await self.compile(path).findall_async(
             data, filter_context=filter_context
         )
 
     async def finditer_async(
         self,
         path: str,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> AsyncIterable[JSONPathMatch]:
         """An async version of `finditer()`."""
         return await self.compile(path).finditer_async(
             data, filter_context=filter_context
         )
```

### Comparing `python_jsonpath-0.7.1/jsonpath/exceptions.py` & `python_jsonpath-0.8.0/jsonpath/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -72,14 +72,46 @@
     """
 
     def __init__(self, *args: object, token: Token) -> None:
         super().__init__(*args)
         self.token = token
 
 
+class JSONPointerError(Exception):
+    """Base class for all JSON Pointer errors."""
+
+
+class JSONPointerEncodeError(JSONPointerError):
+    """An exception raised when a JSONPathMatch can't be encoded to a JSON Pointer."""
+
+
+class JSONPointerResolutionError(JSONPointerError):
+    """Base exception for those that can be raised during pointer resolution."""
+
+
+class JSONPointerIndexError(JSONPointerResolutionError, IndexError):
+    """An exception raised when an array index is out of range."""
+
+
+class JSONPointerKeyError(JSONPointerResolutionError, KeyError):
+    """An exception raised when a pointer references a mapping with a missing key."""
+
+
+class JSONPointerTypeError(JSONPointerResolutionError, TypeError):
+    """An exception raised when a pointer resolves a string against a sequence."""
+
+
+class JSONPatchError(Exception):
+    """Base class for all JSON Patch errors."""
+
+
+class JSONPatchTestFailure(JSONPatchError):  # noqa: N818
+    """An exception raised when a JSON Patch _test_ op fails."""
+
+
 def _truncate_message(value: str, num: int, end: str = "...") -> str:
     if len(value) < num:
         return value
     return f"{value[:num-len(end)]}{end}"
 
 
 def _truncate_words(val: str, num: int, end: str = "...") -> str:
```

### Comparing `python_jsonpath-0.7.1/jsonpath/lex.py` & `python_jsonpath-0.8.0/jsonpath/lex.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/match.py` & `python_jsonpath-0.8.0/jsonpath/match.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
+from .pointer import JSONPointer
+
 FilterContextVars = Mapping[str, Any]
-PathPart = Union[int, slice, str]
+PathPart = Union[int, str]
 
 
 class JSONPathMatch:
     """A matched object with a concrete path.
 
     Attributes:
         children: Matched child nodes. This will only be populated after
@@ -35,14 +37,16 @@
         "obj",
         "parent",
         "parts",
         "path",
         "root",
     )
 
+    pointer_class = JSONPointer
+
     def __init__(
         self,
         *,
         filter_context: FilterContextVars,
         obj: object,
         parent: Optional[JSONPathMatch],
         path: str,
@@ -64,14 +68,18 @@
         """Append one or more children to this match."""
         self.children.extend(children)
 
     def filter_context(self) -> FilterContextVars:
         """Return filter context data for this match."""
         return self._filter_context
 
+    def pointer(self) -> JSONPointer:
+        """Return a `JSONPointer` pointing to this match's path."""
+        return JSONPointer.from_match(self)
+
 
 def _truncate(val: str, num: int, end: str = "...") -> str:
     # Replaces consecutive whitespace with a single newline.
     # Treats quoted whitespace the same as unquoted whitespace.
     words = val.split()
     if len(words) < num:
         return " ".join(words)
```

### Comparing `python_jsonpath-0.7.1/jsonpath/parse.py` & `python_jsonpath-0.8.0/jsonpath/parse.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/path.py` & `python_jsonpath-0.8.0/jsonpath/path.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # noqa: D100
 from __future__ import annotations
 
 import itertools
 import json
+from io import IOBase
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import AsyncIterable
 from typing import Iterable
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
-from typing import TextIO
 from typing import Tuple
 from typing import TypeVar
 from typing import Union
 
 from .match import FilterContextVars
 from .match import JSONPathMatch
 
@@ -27,35 +27,39 @@
 class JSONPath:
     """A compiled JSONPath ready to be applied to a JSON string or Python object.
 
     Arguments:
         env: The `JSONPathEnvironment` this path is bound to.
         selectors: An iterable of `JSONPathSelector` objects, as generated by
             a `Parser`.
+
+    Attributes:
+        env: The `JSONPathEnvironment` this path is bound to.
+        selectors: The `JSONPathSelector` instances that make up this path.
     """
 
-    __slots__ = ("env", "_selectors")
+    __slots__ = ("env", "selectors")
 
     def __init__(
         self,
         *,
         env: JSONPathEnvironment,
         selectors: Iterable[JSONPathSelector],
     ) -> None:
         self.env = env
-        self._selectors = tuple(selectors)
+        self.selectors = tuple(selectors)
 
     def __str__(self) -> str:
         return self.env.root_token + "".join(
-            str(selector) for selector in self._selectors
+            str(selector) for selector in self.selectors
         )
 
     def findall(
         self,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """Find all objects in `data` matching the given JSONPath `path`.
 
         If `data` is a string or a file-like objects, it will be loaded
         using `json.loads()` and the default `JSONDecoder`.
@@ -73,25 +77,25 @@
         Raises:
             JSONPathSyntaxError: If the path is invalid.
             JSONPathTypeError: If a filter expression attempts to use types in
                 an incompatible way.
         """
         if isinstance(data, str):
             _data = json.loads(data)
-        elif isinstance(data, TextIO):
+        elif isinstance(data, IOBase):
             _data = json.loads(data.read())
         else:
             _data = data
         return [
             match.obj for match in self.finditer(_data, filter_context=filter_context)
         ]
 
     def finditer(
         self,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> Iterable[JSONPathMatch]:
         """Generate `JSONPathMatch` objects for each match.
 
         If `data` is a string or a file-like objects, it will be loaded
         using `json.loads()` and the default `JSONDecoder`.
@@ -101,21 +105,22 @@
                 or `Mapping` interfaces.
             filter_context: Arbitrary data made available to filters using
                 the _filter context_ selector.
 
         Returns:
             An iterator yielding `JSONPathMatch` objects for each match.
 
-        JSONPathSyntaxError: If the path is invalid.
+        Raises:
+            JSONPathSyntaxError: If the path is invalid.
             JSONPathTypeError: If a filter expression attempts to use types in
                 an incompatible way.
         """
         if isinstance(data, str):
             _data = json.loads(data)
-        elif isinstance(data, TextIO):
+        elif isinstance(data, IOBase):
             _data = json.loads(data.read())
         else:
             _data = data
 
         matches: Iterable[JSONPathMatch] = [
             JSONPathMatch(
                 filter_context=filter_context or {},
@@ -123,73 +128,103 @@
                 parent=None,
                 path=self.env.root_token,
                 parts=(),
                 root=_data,
             )
         ]
 
-        for selector in self._selectors:
+        for selector in self.selectors:
             matches = selector.resolve(matches)
 
         return matches
 
     async def findall_async(
         self,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """An async version of `findall()`."""
         if isinstance(data, str):
             _data = json.loads(data)
-        elif isinstance(data, TextIO):
+        elif isinstance(data, IOBase):
             _data = json.loads(data.read())
         else:
             _data = data
         return [
             match.obj
             async for match in await self.finditer_async(
                 _data, filter_context=filter_context
             )
         ]
 
     async def finditer_async(
         self,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> AsyncIterable[JSONPathMatch]:
         """An async version of `finditer()`."""
         if isinstance(data, str):
             _data = json.loads(data)
-        elif isinstance(data, TextIO):
+        elif isinstance(data, IOBase):
             _data = json.loads(data.read())
         else:
             _data = data
 
         async def root_iter() -> AsyncIterable[JSONPathMatch]:
-            yield JSONPathMatch(
+            yield self.env.match_class(
                 filter_context=filter_context or {},
                 obj=_data,
                 parent=None,
                 path=self.env.root_token,
                 parts=(),
                 root=_data,
             )
 
         matches: AsyncIterable[JSONPathMatch] = root_iter()
 
-        for selector in self._selectors:
+        for selector in self.selectors:
             matches = selector.resolve_async(matches)
 
         return matches
 
+    def match(
+        self,
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
+        *,
+        filter_context: Optional[FilterContextVars] = None,
+    ) -> Union[JSONPathMatch, None]:
+        """Return a `JSONPathMatch` instance for the first object found in _data_.
+
+        `None` is returned if there are no matches.
+
+        Arguments:
+            data: A JSON document or Python object implementing the `Sequence`
+                or `Mapping` interfaces.
+            filter_context: Arbitrary data made available to filters using
+                the _filter context_ selector.
+
+        Returns:
+            A `JSONPathMatch` object for the first match, or `None` if there were
+                no matches.
+
+        Raises:
+            JSONPathSyntaxError: If the path is invalid.
+            JSONPathTypeError: If a filter expression attempts to use types in
+                an incompatible way.
+        """
+        try:
+            return next(iter(self.finditer(data, filter_context=filter_context)))
+        except StopIteration:
+            return None
+
     def empty(self) -> bool:
         """Return `True` if this path has no selectors."""
-        return not bool(self._selectors)
+        return not bool(self.selectors)
 
 
 class CompoundJSONPath:
     """Multiple `JSONPath`s combined."""
 
     __slots__ = ("env", "path", "paths")
 
@@ -208,15 +243,16 @@
         for op, path in self.paths:
             buf.append(f" {op} ")
             buf.append(str(path))
         return "".join(buf)
 
     def findall(
         self,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
+        *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """Find all objects in `data` matching the given JSONPath `path`.
 
         If `data` is a string or a file-like objects, it will be loaded
         using `json.loads()` and the default `JSONDecoder`.
 
@@ -245,15 +281,16 @@
                 assert op == self.env.intersection_token, op
                 objs = [obj for obj in objs if obj in _objs]
 
         return objs
 
     def finditer(
         self,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
+        *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> Iterable[JSONPathMatch]:
         """Generate `JSONPathMatch` objects for each match.
 
         If `data` is a string or a file-like objects, it will be loaded
         using `json.loads()` and the default `JSONDecoder`.
 
@@ -280,17 +317,48 @@
             else:
                 assert op == self.env.intersection_token
                 _objs = [match.obj for match in _matches]
                 matches = (match for match in matches if match.obj in _objs)
 
         return matches
 
+    def match(
+        self,
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
+        *,
+        filter_context: Optional[FilterContextVars] = None,
+    ) -> Union[JSONPathMatch, None]:
+        """Return a `JSONPathMatch` instance for the first object found in _data_.
+
+        `None` is returned if there are no matches.
+
+        Arguments:
+            data: A JSON document or Python object implementing the `Sequence`
+                or `Mapping` interfaces.
+            filter_context: Arbitrary data made available to filters using
+                the _filter context_ selector.
+
+        Returns:
+            A `JSONPathMatch` object for the first match, or `None` if there were
+                no matches.
+
+        Raises:
+            JSONPathSyntaxError: If the path is invalid.
+            JSONPathTypeError: If a filter expression attempts to use types in
+                an incompatible way.
+        """
+        try:
+            return next(iter(self.finditer(data, filter_context=filter_context)))
+        except StopIteration:
+            return None
+
     async def findall_async(
         self,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
+        *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """An async version of `findall()`."""
         objs = await self.path.findall_async(data, filter_context=filter_context)
 
         for op, path in self.paths:
             _objs = await path.findall_async(data, filter_context=filter_context)
@@ -300,15 +368,16 @@
                 assert op == self.env.intersection_token
                 objs = [obj for obj in objs if obj in _objs]
 
         return objs
 
     async def finditer_async(
         self,
-        data: Union[str, TextIO, Sequence[Any], Mapping[str, Any]],
+        data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
+        *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> AsyncIterable[JSONPathMatch]:
         """An async version of `finditer()`."""
         matches = await self.path.finditer_async(data, filter_context=filter_context)
 
         for op, path in self.paths:
             _matches = await path.finditer_async(data, filter_context=filter_context)
```

### Comparing `python_jsonpath-0.7.1/jsonpath/selectors.py` & `python_jsonpath-0.8.0/jsonpath/selectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from typing import List
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 
 from .exceptions import JSONPathIndexError
 from .exceptions import JSONPathTypeError
-from .match import JSONPathMatch
 
 if TYPE_CHECKING:
     from .env import JSONPathEnvironment
     from .filter import BooleanExpression
+    from .match import JSONPathMatch
     from .token import Token
 
 # ruff: noqa: D102
 
 
 class JSONPathSelector(ABC):
     """Base class for all JSONPath selectors."""
@@ -40,15 +40,15 @@
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         """Expand matches from previous JSONPath selectors in to new matches."""
 
     @abstractmethod
     def resolve_async(
         self, matches: AsyncIterable[JSONPathMatch]
     ) -> AsyncIterable[JSONPathMatch]:
-        """An async version of `expand`."""
+        """An async version of `resolve`."""
 
 
 class PropertySelector(JSONPathSelector):
     """A JSONPath property."""
 
     __slots__ = ("name",)
 
@@ -67,15 +67,15 @@
 
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         for match in matches:
             if not isinstance(match.obj, Mapping):
                 continue
 
             with suppress(KeyError):
-                _match = JSONPathMatch(
+                _match = self.env.match_class(
                     filter_context=match.filter_context(),
                     obj=self.env.getitem(match.obj, self.name),
                     parent=match,
                     parts=match.parts + (self.name,),
                     path=match.path + f"['{self.name}']",
                     root=match.root,
                 )
@@ -86,15 +86,15 @@
         self, matches: AsyncIterable[JSONPathMatch]
     ) -> AsyncIterable[JSONPathMatch]:
         async for match in matches:
             if not isinstance(match.obj, Mapping):
                 continue
 
             with suppress(KeyError):
-                _match = JSONPathMatch(
+                _match = self.env.match_class(
                     filter_context=match.filter_context(),
                     obj=await self.env.getitem_async(match.obj, self.name),
                     parent=match,
                     parts=match.parts + (self.name,),
                     path=match.path + f"['{self.name}']",
                     root=match.root,
                 )
@@ -130,28 +130,28 @@
         return self.index
 
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         for match in matches:
             if isinstance(match.obj, Mapping):
                 # Try the string representation of the index as a key.
                 with suppress(KeyError):
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=self.env.getitem(match.obj, self._as_key),
                         parent=match,
-                        parts=match.parts + (self.index,),
+                        parts=match.parts + (self._as_key,),
                         path=f"{match.path}['{self.index}']",
                         root=match.root,
                     )
                     match.add_child(_match)
                     yield _match
             elif isinstance(match.obj, Sequence):
                 norm_index = self._normalized_index(match.obj)
                 with suppress(IndexError):
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=self.env.getitem(match.obj, self.index),
                         parent=match,
                         parts=match.parts + (norm_index,),
                         path=match.path + f"[{norm_index}]",
                         root=match.root,
                     )
@@ -161,28 +161,28 @@
     async def resolve_async(
         self, matches: AsyncIterable[JSONPathMatch]
     ) -> AsyncIterable[JSONPathMatch]:
         async for match in matches:
             if isinstance(match.obj, Mapping):
                 # Try the string representation of the index as a key.
                 with suppress(KeyError):
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=await self.env.getitem_async(match.obj, self._as_key),
                         parent=match,
-                        parts=match.parts + (self.index,),
+                        parts=match.parts + (self._as_key,),
                         path=f"{match.path}['{self.index}']",
                         root=match.root,
                     )
                     match.add_child(_match)
                     yield _match
             elif isinstance(match.obj, Sequence):
                 norm_index = self._normalized_index(match.obj)
                 with suppress(IndexError):
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=await self.env.getitem_async(match.obj, self.index),
                         parent=match,
                         parts=match.parts + (norm_index,),
                         path=match.path + f"[{norm_index}]",
                         root=match.root,
                     )
@@ -197,19 +197,19 @@
 
     def __str__(self) -> str:
         return f"[{self.env.keys_selector_token}]"
 
     def _keys(self, match: JSONPathMatch) -> Iterable[JSONPathMatch]:
         if isinstance(match.obj, Mapping):
             for i, key in enumerate(match.obj.keys()):
-                _match = JSONPathMatch(
+                _match = self.env.match_class(
                     filter_context=match.filter_context(),
                     obj=key,
                     parent=match,
-                    parts=match.parts + (self.env.keys_selector_token, i),
+                    parts=match.parts + (f"{self.env.keys_selector_token}{key}",),
                     path=f"{match.path}[{self.env.keys_selector_token}][{i}]",
                     root=match.root,
                 )
                 match.add_child(_match)
                 yield _match
 
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
@@ -265,15 +265,15 @@
             if not isinstance(match.obj, Sequence) or self.slice.step == 0:
                 continue
 
             idx = self.slice.start or 0
             step = self.slice.step or 1
             for obj in self.env.getitem(match.obj, self.slice):
                 norm_index = self._normalized_index(match.obj, idx)
-                _match = JSONPathMatch(
+                _match = self.env.match_class(
                     filter_context=match.filter_context(),
                     obj=obj,
                     parent=match,
                     parts=match.parts + (norm_index,),
                     path=f"{match.path}[{norm_index}]",
                     root=match.root,
                 )
@@ -288,15 +288,15 @@
             if not isinstance(match.obj, Sequence) or self.slice.step == 0:
                 continue
 
             idx = self.slice.start or 0
             step = self.slice.step or 1
             for obj in await self.env.getitem_async(match.obj, self.slice):
                 norm_index = self._normalized_index(match.obj, idx)
-                _match = JSONPathMatch(
+                _match = self.env.match_class(
                     filter_context=match.filter_context(),
                     obj=obj,
                     parent=match,
                     parts=match.parts + (norm_index,),
                     path=f"{match.path}[{norm_index}]",
                     root=match.root,
                 )
@@ -313,27 +313,27 @@
 
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         for match in matches:
             if isinstance(match.obj, str):
                 continue
             if isinstance(match.obj, Mapping):
                 for key, val in match.obj.items():
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=val,
                         parent=match,
                         parts=match.parts + (key,),
                         path=match.path + f"['{key}']",
                         root=match.root,
                     )
                     match.add_child(_match)
                     yield _match
             elif isinstance(match.obj, Sequence):
                 for i, val in enumerate(match.obj):
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=val,
                         parent=match,
                         parts=match.parts + (i,),
                         path=f"{match.path}[{i}]",
                         root=match.root,
                     )
@@ -342,27 +342,27 @@
 
     async def resolve_async(
         self, matches: AsyncIterable[JSONPathMatch]
     ) -> AsyncIterable[JSONPathMatch]:
         async for match in matches:
             if isinstance(match.obj, Mapping):
                 for key, val in match.obj.items():
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=val,
                         parent=match,
                         parts=match.parts + (key,),
                         path=match.path + f"['{key}']",
                         root=match.root,
                     )
                     match.add_child(_match)
                     yield _match
             elif isinstance(match.obj, Sequence):
                 for i, val in enumerate(match.obj):
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=val,
                         parent=match,
                         parts=match.parts + (i,),
                         path=f"{match.path}[{i}]",
                         root=match.root,
                     )
@@ -378,15 +378,15 @@
 
     def _expand(self, match: JSONPathMatch) -> Iterable[JSONPathMatch]:
         if isinstance(match.obj, Mapping):
             for key, val in match.obj.items():
                 if isinstance(val, str):
                     pass
                 elif isinstance(val, (Mapping, Sequence)):
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=val,
                         parent=match,
                         parts=match.parts + (key,),
                         path=match.path + f"['{key}']",
                         root=match.root,
                     )
@@ -394,15 +394,15 @@
                     yield _match
                     yield from self._expand(_match)
         elif isinstance(match.obj, Sequence) and not isinstance(match.obj, str):
             for i, val in enumerate(match.obj):
                 if isinstance(val, str):
                     pass
                 elif isinstance(val, (Mapping, Sequence)):
-                    _match = JSONPathMatch(
+                    _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=val,
                         parent=match,
                         parts=match.parts + (i,),
                         path=f"{match.path}[{i}]",
                         root=match.root,
                     )
@@ -486,45 +486,52 @@
             async for match in item.resolve_async(_alist(_matches)):
                 yield match
 
 
 class Filter(JSONPathSelector):
     """A filter selector."""
 
-    __slots__ = ("expression",)
+    __slots__ = ("expression", "cacheable_nodes")
 
     def __init__(
         self,
         *,
         env: JSONPathEnvironment,
         token: Token,
         expression: BooleanExpression,
     ) -> None:
         super().__init__(env=env, token=token)
         self.expression = expression
+        # Compile-time check for cacheable nodes.
+        self.cacheable_nodes = self.expression.cacheable_nodes()
 
     def __str__(self) -> str:
         return f"[?({self.expression})]"
 
     def resolve(  # noqa: PLR0912
         self, matches: Iterable[JSONPathMatch]
     ) -> Iterable[JSONPathMatch]:
+        if self.cacheable_nodes and self.env.filter_caching:
+            expr = self.expression.cache_tree()
+        else:
+            expr = self.expression
+
         for match in matches:
             if isinstance(match.obj, Mapping):
                 for key, val in match.obj.items():
                     context = FilterContext(
                         env=self.env,
                         current=val,
                         root=match.root,
                         extra_context=match.filter_context(),
                         current_key=key,
                     )
                     try:
-                        if self.expression.evaluate(context):
-                            _match = JSONPathMatch(
+                        if expr.evaluate(context):
+                            _match = self.env.match_class(
                                 filter_context=match.filter_context(),
                                 obj=val,
                                 parent=match,
                                 parts=match.parts + (key,),
                                 path=match.path + f"['{key}']",
                                 root=match.root,
                             )
@@ -541,16 +548,16 @@
                         env=self.env,
                         current=obj,
                         root=match.root,
                         extra_context=match.filter_context(),
                         current_key=i,
                     )
                     try:
-                        if self.expression.evaluate(context):
-                            _match = JSONPathMatch(
+                        if expr.evaluate(context):
+                            _match = self.env.match_class(
                                 filter_context=match.filter_context(),
                                 obj=obj,
                                 parent=match,
                                 parts=match.parts + (i,),
                                 path=f"{match.path}[{i}]",
                                 root=match.root,
                             )
@@ -560,34 +567,39 @@
                         if not err.token:
                             err.token = self.token
                         raise
 
     async def resolve_async(  # noqa: PLR0912
         self, matches: AsyncIterable[JSONPathMatch]
     ) -> AsyncIterable[JSONPathMatch]:
+        if self.cacheable_nodes and self.env.filter_caching:
+            expr = self.expression.cache_tree()
+        else:
+            expr = self.expression
+
         async for match in matches:
             if isinstance(match.obj, Mapping):
                 for key, val in match.obj.items():
                     context = FilterContext(
                         env=self.env,
                         current=val,
                         root=match.root,
                         extra_context=match.filter_context(),
                         current_key=key,
                     )
 
                     try:
-                        result = await self.expression.evaluate_async(context)
+                        result = await expr.evaluate_async(context)
                     except JSONPathTypeError as err:
                         if not err.token:
                             err.token = self.token
                         raise
 
                     if result:
-                        _match = JSONPathMatch(
+                        _match = self.env.match_class(
                             filter_context=match.filter_context(),
                             obj=val,
                             parent=match,
                             parts=match.parts + (key,),
                             path=match.path + f"['{key}']",
                             root=match.root,
                         )
@@ -601,36 +613,42 @@
                         current=obj,
                         root=match.root,
                         extra_context=match.filter_context(),
                         current_key=i,
                     )
 
                     try:
-                        result = await self.expression.evaluate_async(context)
+                        result = await expr.evaluate_async(context)
                     except JSONPathTypeError as err:
                         if not err.token:
                             err.token = self.token
                         raise
                     if result:
-                        _match = JSONPathMatch(
+                        _match = self.env.match_class(
                             filter_context=match.filter_context(),
                             obj=obj,
                             parent=match,
                             parts=match.parts + (i,),
                             path=f"{match.path}[{i}]",
                             root=match.root,
                         )
                         match.add_child(_match)
                         yield _match
 
 
 class FilterContext:
     """A filter expression context."""
 
-    __slots__ = ("current", "current_key", "env", "root", "extra_context")
+    __slots__ = (
+        "current_key",
+        "current",
+        "env",
+        "extra_context",
+        "root",
+    )
 
     def __init__(
         self,
         *,
         env: JSONPathEnvironment,
         current: object,
         root: Union[Sequence[Any], Mapping[str, Any]],
```

### Comparing `python_jsonpath-0.7.1/jsonpath/stream.py` & `python_jsonpath-0.8.0/jsonpath/stream.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/token.py` & `python_jsonpath-0.8.0/jsonpath/token.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/function_extensions/arguments.py` & `python_jsonpath-0.8.0/jsonpath/function_extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/function_extensions/count.py` & `python_jsonpath-0.8.0/jsonpath/function_extensions/count.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/function_extensions/is_instance.py` & `python_jsonpath-0.8.0/jsonpath/function_extensions/is_instance.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/function_extensions/match.py` & `python_jsonpath-0.8.0/jsonpath/function_extensions/match.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/function_extensions/search.py` & `python_jsonpath-0.8.0/jsonpath/function_extensions/search.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/jsonpath/function_extensions/typeof.py` & `python_jsonpath-0.8.0/jsonpath/function_extensions/typeof.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/.gitignore` & `python_jsonpath-0.8.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -76,11 +76,13 @@
 .ropeproject
 
 # IDE
 .vscode/
 
 # Dev utils
 dev.py
+benchmark.py
+profile_.py
 
 # Test fixtures
 comparison_regression_suite.yaml
 cts.json
```

### Comparing `python_jsonpath-0.7.1/LICENSE.txt` & `python_jsonpath-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/README.md` & `python_jsonpath-0.8.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ---
 
 **Table of Contents**
 
 - [Install](#install)
 - [Links](#links)
-- [Example](#example)
+- [Examples](#examples)
 - [License](#license)
 
 ## Install
 
 Install Python JSONPath using [pip](https://pip.pypa.io/en/stable/getting-started/):
 
 ```console
@@ -39,24 +39,32 @@
 
 Or [Pipenv](https://pipenv.pypa.io/en/latest/):
 
 ```console
 pipenv install -u python-jsonpath
 ```
 
+Or from [conda-forge](https://anaconda.org/conda-forge/python-jsonpath):
+
+```console
+conda install -c conda-forge python-jsonpath
+```
+
 ## Links
 
 - Documentation: https://jg-rp.github.io/python-jsonpath/.
 - JSONPath Syntax: https://jg-rp.github.io/python-jsonpath/syntax/
 - Change log: https://github.com/jg-rp/python-jsonpath/blob/main/CHANGELOG.md
 - PyPi: https://pypi.org/project/python-jsonpath
 - Source code: https://github.com/jg-rp/python-jsonpath
 - Issue tracker: https://github.com/jg-rp/python-jsonpath/issues
 
-## Example
+## Examples
+
+### JSONPath
 
 ```python
 import jsonpath
 
 data = {
     "users": [
         {
@@ -78,10 +86,45 @@
     ]
 }
 
 user_names = jsonpath.findall("$.users[?@.score < 100].name", data)
 print(user_names) # ['John', 'Sally', 'Jane']
 ```
 
+### JSON Pointer
+
+Since version 0.8.0, we also include an [RFC 6901](https://datatracker.ietf.org/doc/html/rfc6901) compliant implementation of JSON Pointer.
+
+```python
+from jsonpath import pointer
+
+data = {
+    "users": [
+        {
+            "name": "Sue",
+            "score": 100,
+        },
+        {
+            "name": "John",
+            "score": 86,
+        },
+        {
+            "name": "Sally",
+            "score": 84,
+        },
+        {
+            "name": "Jane",
+            "score": 55,
+        },
+    ]
+}
+
+sue_score = pointer.resolve("/users/0/score", data)
+print(sue_score)  # 100
+
+jane_score = pointer.resolve(["users", 3, "score"], data)
+print(jane_score)  # 55
+```
+
 ## License
 
 `python-jsonpath` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### html2text {}

```diff
@@ -1,20 +1,28 @@
                          ****** Python JSONPath ******
                     A flexible JSONPath engine for Python.
                               [License] [Tests]
                       [PyPi_-_Version] [Python_versions]
---- **Table of Contents** - [Install](#install) - [Links](#links) - [Example]
-(#example) - [License](#license) ## Install Install Python JSONPath using [pip]
-(https://pip.pypa.io/en/stable/getting-started/): ```console pip install
+--- **Table of Contents** - [Install](#install) - [Links](#links) - [Examples]
+(#examples) - [License](#license) ## Install Install Python JSONPath using
+[pip](https://pip.pypa.io/en/stable/getting-started/): ```console pip install
 python-jsonpath ``` Or [Pipenv](https://pipenv.pypa.io/en/latest/): ```console
-pipenv install -u python-jsonpath ``` ## Links - Documentation: https://jg-
-rp.github.io/python-jsonpath/. - JSONPath Syntax: https://jg-rp.github.io/
-python-jsonpath/syntax/ - Change log: https://github.com/jg-rp/python-jsonpath/
-blob/main/CHANGELOG.md - PyPi: https://pypi.org/project/python-jsonpath -
-Source code: https://github.com/jg-rp/python-jsonpath - Issue tracker: https://
-github.com/jg-rp/python-jsonpath/issues ## Example ```python import jsonpath
+pipenv install -u python-jsonpath ``` Or from [conda-forge](https://
+anaconda.org/conda-forge/python-jsonpath): ```console conda install -c conda-
+forge python-jsonpath ``` ## Links - Documentation: https://jg-rp.github.io/
+python-jsonpath/. - JSONPath Syntax: https://jg-rp.github.io/python-jsonpath/
+syntax/ - Change log: https://github.com/jg-rp/python-jsonpath/blob/main/
+CHANGELOG.md - PyPi: https://pypi.org/project/python-jsonpath - Source code:
+https://github.com/jg-rp/python-jsonpath - Issue tracker: https://github.com/
+jg-rp/python-jsonpath/issues ## Examples ### JSONPath ```python import jsonpath
 data = { "users": [ { "name": "Sue", "score": 100, }, { "name": "John",
 "score": 86, }, { "name": "Sally", "score": 84, }, { "name": "Jane", "score":
 55, }, ] } user_names = jsonpath.findall("$.users[?@.score < 100].name", data)
-print(user_names) # ['John', 'Sally', 'Jane'] ``` ## License `python-jsonpath`
-is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html)
-license.
+print(user_names) # ['John', 'Sally', 'Jane'] ``` ### JSON Pointer Since
+version 0.8.0, we also include an [RFC 6901](https://datatracker.ietf.org/doc/
+html/rfc6901) compliant implementation of JSON Pointer. ```python from jsonpath
+import pointer data = { "users": [ { "name": "Sue", "score": 100, }, { "name":
+"John", "score": 86, }, { "name": "Sally", "score": 84, }, { "name": "Jane",
+"score": 55, }, ] } sue_score = pointer.resolve("/users/0/score", data) print
+(sue_score) # 100 jane_score = pointer.resolve(["users", 3, "score"], data)
+print(jane_score) # 55 ``` ## License `python-jsonpath` is distributed under
+the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `python_jsonpath-0.7.1/pyproject.toml` & `python_jsonpath-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.1/PKG-INFO` & `python_jsonpath-0.8.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-jsonpath
-Version: 0.7.1
+Version: 0.8.0
 Summary: Another JSONPath implementation for Python.
 Project-URL: Documentation, https://jg-rp.github.io/python-jsonpath/
 Project-URL: Issues, https://github.com/jg-rp/python-jsonpath/issues
 Project-URL: Source, https://github.com/jg-rp/python-jsonpath
 Author-email: James Prior <jamesgr.prior@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -46,15 +46,15 @@
 
 ---
 
 **Table of Contents**
 
 - [Install](#install)
 - [Links](#links)
-- [Example](#example)
+- [Examples](#examples)
 - [License](#license)
 
 ## Install
 
 Install Python JSONPath using [pip](https://pip.pypa.io/en/stable/getting-started/):
 
 ```console
@@ -63,24 +63,32 @@
 
 Or [Pipenv](https://pipenv.pypa.io/en/latest/):
 
 ```console
 pipenv install -u python-jsonpath
 ```
 
+Or from [conda-forge](https://anaconda.org/conda-forge/python-jsonpath):
+
+```console
+conda install -c conda-forge python-jsonpath
+```
+
 ## Links
 
 - Documentation: https://jg-rp.github.io/python-jsonpath/.
 - JSONPath Syntax: https://jg-rp.github.io/python-jsonpath/syntax/
 - Change log: https://github.com/jg-rp/python-jsonpath/blob/main/CHANGELOG.md
 - PyPi: https://pypi.org/project/python-jsonpath
 - Source code: https://github.com/jg-rp/python-jsonpath
 - Issue tracker: https://github.com/jg-rp/python-jsonpath/issues
 
-## Example
+## Examples
+
+### JSONPath
 
 ```python
 import jsonpath
 
 data = {
     "users": [
         {
@@ -102,10 +110,45 @@
     ]
 }
 
 user_names = jsonpath.findall("$.users[?@.score < 100].name", data)
 print(user_names) # ['John', 'Sally', 'Jane']
 ```
 
+### JSON Pointer
+
+Since version 0.8.0, we also include an [RFC 6901](https://datatracker.ietf.org/doc/html/rfc6901) compliant implementation of JSON Pointer.
+
+```python
+from jsonpath import pointer
+
+data = {
+    "users": [
+        {
+            "name": "Sue",
+            "score": 100,
+        },
+        {
+            "name": "John",
+            "score": 86,
+        },
+        {
+            "name": "Sally",
+            "score": 84,
+        },
+        {
+            "name": "Jane",
+            "score": 55,
+        },
+    ]
+}
+
+sue_score = pointer.resolve("/users/0/score", data)
+print(sue_score)  # 100
+
+jane_score = pointer.resolve(["users", 3, "score"], data)
+print(jane_score)  # 55
+```
+
 ## License
 
 `python-jsonpath` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-jsonpath Version: 0.7.1 Summary: Another
+Metadata-Version: 2.1 Name: python-jsonpath Version: 0.8.0 Summary: Another
 JSONPath implementation for Python. Project-URL: Documentation, https://jg-
 rp.github.io/python-jsonpath/ Project-URL: Issues, https://github.com/jg-rp/
 python-jsonpath/issues Project-URL: Source, https://github.com/jg-rp/python-
 jsonpath Author-email: James Prior
 prior@gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
@@ -13,23 +13,31 @@
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown
                          ****** Python JSONPath ******
                     A flexible JSONPath engine for Python.
                               [License] [Tests]
                       [PyPi_-_Version] [Python_versions]
---- **Table of Contents** - [Install](#install) - [Links](#links) - [Example]
-(#example) - [License](#license) ## Install Install Python JSONPath using [pip]
-(https://pip.pypa.io/en/stable/getting-started/): ```console pip install
+--- **Table of Contents** - [Install](#install) - [Links](#links) - [Examples]
+(#examples) - [License](#license) ## Install Install Python JSONPath using
+[pip](https://pip.pypa.io/en/stable/getting-started/): ```console pip install
 python-jsonpath ``` Or [Pipenv](https://pipenv.pypa.io/en/latest/): ```console
-pipenv install -u python-jsonpath ``` ## Links - Documentation: https://jg-
-rp.github.io/python-jsonpath/. - JSONPath Syntax: https://jg-rp.github.io/
-python-jsonpath/syntax/ - Change log: https://github.com/jg-rp/python-jsonpath/
-blob/main/CHANGELOG.md - PyPi: https://pypi.org/project/python-jsonpath -
-Source code: https://github.com/jg-rp/python-jsonpath - Issue tracker: https://
-github.com/jg-rp/python-jsonpath/issues ## Example ```python import jsonpath
+pipenv install -u python-jsonpath ``` Or from [conda-forge](https://
+anaconda.org/conda-forge/python-jsonpath): ```console conda install -c conda-
+forge python-jsonpath ``` ## Links - Documentation: https://jg-rp.github.io/
+python-jsonpath/. - JSONPath Syntax: https://jg-rp.github.io/python-jsonpath/
+syntax/ - Change log: https://github.com/jg-rp/python-jsonpath/blob/main/
+CHANGELOG.md - PyPi: https://pypi.org/project/python-jsonpath - Source code:
+https://github.com/jg-rp/python-jsonpath - Issue tracker: https://github.com/
+jg-rp/python-jsonpath/issues ## Examples ### JSONPath ```python import jsonpath
 data = { "users": [ { "name": "Sue", "score": 100, }, { "name": "John",
 "score": 86, }, { "name": "Sally", "score": 84, }, { "name": "Jane", "score":
 55, }, ] } user_names = jsonpath.findall("$.users[?@.score < 100].name", data)
-print(user_names) # ['John', 'Sally', 'Jane'] ``` ## License `python-jsonpath`
-is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html)
-license.
+print(user_names) # ['John', 'Sally', 'Jane'] ``` ### JSON Pointer Since
+version 0.8.0, we also include an [RFC 6901](https://datatracker.ietf.org/doc/
+html/rfc6901) compliant implementation of JSON Pointer. ```python from jsonpath
+import pointer data = { "users": [ { "name": "Sue", "score": 100, }, { "name":
+"John", "score": 86, }, { "name": "Sally", "score": 84, }, { "name": "Jane",
+"score": 55, }, ] } sue_score = pointer.resolve("/users/0/score", data) print
+(sue_score) # 100 jane_score = pointer.resolve(["users", 3, "score"], data)
+print(jane_score) # 55 ``` ## License `python-jsonpath` is distributed under
+the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

