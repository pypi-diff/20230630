# Comparing `tmp/caen_felib-1.0.4.tar.gz` & `tmp/caen_felib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/software/frontend/py-caen-felib/dist/.tmp-lvvs9jlu/caen_felib-1.0.4.tar", last modified: Tue Jan  3 11:26:59 2023, max compression
+gzip compressed data, was "/builds/software/frontend/py-caen-felib/dist/.tmp-nh3vwksz/caen_felib-1.0.5.tar", last modified: Fri Jun 30 11:07:41 2023, max compression
```

## Comparing `caen_felib-1.0.4.tar` & `caen_felib-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 11:26:59.000000 caen_felib-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     3441 2023-01-03 11:26:59.000000 caen_felib-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2404 2023-01-03 11:26:50.000000 caen_felib-1.0.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-01-03 11:26:50.000000 caen_felib-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-03 11:26:59.000000 caen_felib-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-01-02 14:25:54.000000 caen_felib-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 11:26:59.000000 caen_felib-1.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 11:26:59.000000 caen_felib-1.0.4/src/caen_felib/
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-01-03 11:26:50.000000 caen_felib-1.0.4/src/caen_felib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-01-02 14:25:54.000000 caen_felib-1.0.4/src/caen_felib/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    18422 2023-01-02 14:25:54.000000 caen_felib-1.0.4/src/caen_felib/device.py
--rw-rw-rw-   0 root         (0) root         (0)     1060 2023-01-02 14:25:54.000000 caen_felib-1.0.4/src/caen_felib/error.py
--rw-rw-rw-   0 root         (0) root         (0)     9901 2023-01-02 14:25:54.000000 caen_felib-1.0.4/src/caen_felib/lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 11:26:59.000000 caen_felib-1.0.4/src/caen_felib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3441 2023-01-03 11:26:59.000000 caen_felib-1.0.4/src/caen_felib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      345 2023-01-03 11:26:59.000000 caen_felib-1.0.4/src/caen_felib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 11:26:59.000000 caen_felib-1.0.4/src/caen_felib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-01-03 11:26:59.000000 caen_felib-1.0.4/src/caen_felib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-03 11:26:59.000000 caen_felib-1.0.4/src/caen_felib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 11:07:41.000000 caen_felib-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-06-30 11:07:41.000000 caen_felib-1.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2404 2023-06-30 11:03:39.000000 caen_felib-1.0.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-30 11:03:39.000000 caen_felib-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 11:07:41.000000 caen_felib-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-30 11:03:39.000000 caen_felib-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 11:07:41.000000 caen_felib-1.0.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 11:07:41.000000 caen_felib-1.0.5/src/caen_felib/
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-06-30 11:03:39.000000 caen_felib-1.0.5/src/caen_felib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-06-30 11:03:39.000000 caen_felib-1.0.5/src/caen_felib/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18340 2023-06-30 11:03:39.000000 caen_felib-1.0.5/src/caen_felib/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-06-30 11:03:39.000000 caen_felib-1.0.5/src/caen_felib/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2023-06-30 11:03:39.000000 caen_felib-1.0.5/src/caen_felib/lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 11:07:41.000000 caen_felib-1.0.5/src/caen_felib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-06-30 11:07:41.000000 caen_felib-1.0.5/src/caen_felib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-30 11:07:41.000000 caen_felib-1.0.5/src/caen_felib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 11:07:41.000000 caen_felib-1.0.5/src/caen_felib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-30 11:07:41.000000 caen_felib-1.0.5/src/caen_felib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-30 11:07:41.000000 caen_felib-1.0.5/src/caen_felib.egg-info/top_level.txt
```

### Comparing `caen_felib-1.0.4/PKG-INFO` & `caen_felib-1.0.5/src/caen_felib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: caen_felib
-Version: 1.0.4
+Name: caen-felib
+Version: 1.0.5
 Summary: Official Python wrapper for the CAEN FELib.
 Author-email: Giovanni Cerretani <g.cerretani@caen.it>, Daniele Ninci <d.ninci@caen.it>
 Project-URL: homepage, https://www.caen.it
 Project-URL: documentation, https://www.caen.it/products/caen-felib-library/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `caen_felib-1.0.4/README.md` & `caen_felib-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `caen_felib-1.0.4/pyproject.toml` & `caen_felib-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `caen_felib-1.0.4/src/caen_felib/_utils.py` & `caen_felib-1.0.5/src/caen_felib/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 @ingroup Python
 """
 
 __author__ = 'Giovanni Cerretani'
-__copyright__ = 'Copyright (C) 2020-2022 CAEN SpA'
+__copyright__ = 'Copyright (C) 2020-2023 CAEN SpA'
 __license__ = 'LGPL-3.0-or-later'  # SPDX-License-Identifier
 
 from functools import lru_cache, wraps, _lru_cache_wrapper
 from typing import Callable, List, Optional, TypeVar, overload
 from weakref import ref, ReferenceType
 
 from typing_extensions import Concatenate, ParamSpec
@@ -46,15 +46,15 @@
     """
     LRU cache decorator that keeps a weak reference to self.
 
     To be used as decorator on methods that are known to return always
     the same value. This can improve the performances of some methods
     by a factor > 1000.
     This wrapper using weak references is required: functools.lru_cache
-    holds a reference to all arguments: using directly on the methos it
+    holds a reference to all arguments: using directly on the methods it
     would hold a reference to self, introducing subdle memory leaks.
 
     @sa https://stackoverflow.com/a/68052994/3287591
     """
 
     def wrapper(method: Callable[Concatenate[_S, _P], _T]) -> Callable[Concatenate[_S, _P], _T]:
```

### Comparing `caen_felib-1.0.4/src/caen_felib/device.py` & `caen_felib-1.0.5/src/caen_felib/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """
 @ingroup Python
 """
 
-from __future__ import annotations  # MyPy 0.991 not supporting Self :(
-
 __author__ = 'Giovanni Cerretani'
-__copyright__ = 'Copyright (C) 2020-2022 CAEN SpA'
+__copyright__ = 'Copyright (C) 2020-2023 CAEN SpA'
 __license__ = 'LGPL-3.0-or-later'  # SPDX-License-Identifier
 
 import ctypes as ct
 from enum import Enum
 from functools import wraps
 from json import dumps, loads
 from typing import Any, Dict, Generator, List, Optional, Tuple, Type
 
 import numpy as np
-from typing_extensions import TypedDict
+from typing_extensions import TypedDict, Self
 
 from caen_felib import lib, _utils
 
 # Comments on imports:
 # - TypedDict moved to typing on Python 3.8
+# - Self moved to typing on Python 3.11
 # - numpy.typing.typing.DTypeLike could be useful but requires numpy >= 1.20
-# - typing_extensions.Self not supported by MyPy 0.991, using annotations
 
 
 _type_map: Dict[str, Type[ct._SimpleCData]] = {
     # Type[ct._SimpleCData] could be replaced by numpy.typing.DTypeLike
     'U8': ct.c_uint8,
     'U16': ct.c_uint16,
     'U32': ct.c_uint32,
@@ -142,36 +140,36 @@
 class Node:
     """
     Class representing a node.
     """
 
     # Public members
     handle: int
-    root_node: Optional[Node]
+    root_node: Optional[Self]
     opened: bool
 
     # Static private members
     __node_cache_manager: _utils.CacheManager = _utils.CacheManager()
 
-    def __init__(self, handle: int, root_node: Optional[Node]) -> None:
+    def __init__(self, handle: int, root_node: Optional[Self]) -> None:
         ## Handle representing the node on the C library
         self.handle = handle
         ## Root node, set to None on root node (stored to prevent garbage collection)
         self.root_node = root_node
         ## Set on instances that requires close() to be called
         self.opened = root_node is None
 
     def __del__(self) -> None:
         if self.opened:
             self.close()
 
     # C API wrappers
 
     @classmethod
-    def open(cls: Type[Node], url: str) -> Node:
+    def open(cls: Type[Self], url: str) -> Self:
         """
         Wrapper to CAEN_FELib_Open()
 
         Example:
         ```
         with device.connect("dig2://<host>") as dig:
             # Do stuff here...
@@ -197,15 +195,15 @@
         @exception					error.Error in case of error
         """
         lib.close(self.handle)
         self.opened = False
         Node.__clear_cache()
 
     @_utils.lru_cache_method(cache_manager=__node_cache_manager)
-    def get_child_nodes(self, path: Optional[str] = None, initial_size: int = 2**6) -> Tuple[Node, ...]:
+    def get_child_nodes(self, path: Optional[str] = None, initial_size: int = 2**6) -> Tuple[Self, ...]:
         """
         Wrapper to CAEN_FELib_GetChildHandles()
 
         @sa child_nodes
         @param[in] path				relative path of a node (either a string or `None` that is interpreted as an empty string)
         @param[in] initial_size		inizial size to allocate for the first iteration
         @return						child nodes (a list)
@@ -213,43 +211,43 @@
         """
         b_path = _utils.to_bytes_opt(path)
         while True:
             child_handles = np.empty([initial_size], dtype=ct.c_uint64)
             child_handles_arg = child_handles.ctypes.data_as(ct.POINTER(ct.c_uint64))
             res = lib.get_child_handles(self.handle, b_path, child_handles_arg, initial_size)
             if res <= initial_size:
-                return tuple(Node(handle.item(), self.__root_node()) for handle in child_handles[:res])
+                return tuple(type(self)(handle.item(), self.__root_node()) for handle in child_handles[:res])
             initial_size = res
 
     @_utils.lru_cache_method(cache_manager=__node_cache_manager)
-    def get_parent_node(self, path: Optional[str] = None) -> Node:
+    def get_parent_node(self, path: Optional[str] = None) -> Self:
         """
         Wrapper to CAEN_FELib_GetParentHandle()
 
         @sa parent_node
         @param[in] path				relative path of a node (either a string or `None` that is interpreted as an empty string)
         @return						parent node
         @exception					error.Error in case of error
         """
         value = ct.c_uint64()
         lib.get_parent_handle(self.handle, _utils.to_bytes_opt(path), value)
-        return Node(value.value, self.__root_node())
+        return type(self)(value.value, self.__root_node())
 
     @_utils.lru_cache_method(cache_manager=__node_cache_manager)
-    def get_node(self, path: Optional[str] = None) -> Node:
+    def get_node(self, path: Optional[str] = None) -> Self:
         """
         Wrapper to CAEN_FELib_GetHandle()
 
         @param[in] path				relative path of a node (either a string or `None` that is interpreted as an empty string)
         @return						node at the provided path
         @exception					error.Error in case of error
         """
         value = ct.c_uint64()
         lib.get_handle(self.handle, _utils.to_bytes_opt(path), value)
-        return Node(value.value, self.__root_node())
+        return type(self)(value.value, self.__root_node())
 
     @_utils.lru_cache_method(cache_manager=__node_cache_manager)
     def get_path(self) -> str:
         """
         Wrapper to CAEN_FELib_GetPath()
 
         @sa path
@@ -447,15 +445,15 @@
         @param[in] timeout			timeout of the function in milliseconds; if this value is -1 the function is blocking with infinite timeout
         @exception					error.Error in case of error
         """
         lib.has_data(self.handle, timeout)
 
     # Private utilities
 
-    def __root_node(self) -> Node:
+    def __root_node(self) -> Self:
         return self if self.root_node is None else self.root_node
 
     @staticmethod
     def __clear_cache() -> None:
         Node.__node_cache_manager.clear_all()
 
     # Python utilities
@@ -472,20 +470,20 @@
 
     @property
     def path(self) -> str:
         """Node absolute path"""
         return self.get_path()
 
     @property
-    def parent_node(self) -> Node:
+    def parent_node(self) -> Self:
         """Parent node"""
         return self.get_parent_node(None)
 
     @property
-    def child_nodes(self) -> Tuple[Node, ...]:
+    def child_nodes(self) -> Tuple[Self, ...]:
         """List of child nodes"""
         return self.get_child_nodes(None)
 
     @property
     def value(self) -> str:
         """Current value"""
         return self.get_value(None)
@@ -494,30 +492,30 @@
     def value(self, value: str) -> None:
         self.set_value(None, value)
 
     def __call__(self) -> None:
         """Execute node"""
         self.send_command(None)
 
-    def __enter__(self) -> Node:
+    def __enter__(self) -> Self:
         """Used by `with`"""
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         """Called when exiting from `with` block"""
         self.close()
 
-    def __iter__(self) -> Generator[Node, None, None]:
-        """Utility to simlify node browsing"""
+    def __iter__(self) -> Generator[Self, None, None]:
+        """Utility to simplify node browsing"""
         yield from self.child_nodes
 
-    def __getitem__(self, index: Any) -> Node:
+    def __getitem__(self, index: Any) -> Self:
         return self.get_node(f'/{index}')
 
-    def __getattr__(self, name: str) -> Node:
+    def __getattr__(self, name: str) -> Self:
         if name.startswith('__') and name.endswith('__'):
             raise AttributeError(name)
         return self.__getitem__(name)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Node):
             return NotImplemented
```

### Comparing `caen_felib-1.0.4/src/caen_felib/error.py` & `caen_felib-1.0.5/src/caen_felib/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 @ingroup Python
 """
 
 __author__ = 'Giovanni Cerretani'
-__copyright__ = 'Copyright (C) 2020-2022 CAEN SpA'
+__copyright__ = 'Copyright (C) 2020-2023 CAEN SpA'
 __license__ = 'LGPL-3.0-or-later'  # SPDX-License-Identifier
 
 from enum import Enum
 
 
 class ErrorCode(Enum):
     """
```

### Comparing `caen_felib-1.0.4/src/caen_felib/lib.py` & `caen_felib-1.0.5/src/caen_felib/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 @ingroup Python
 """
 
 __author__ = 'Giovanni Cerretani'
-__copyright__ = 'Copyright (C) 2020-2022 CAEN SpA'
+__copyright__ = 'Copyright (C) 2020-2023 CAEN SpA'
 __license__ = 'LGPL-3.0-or-later'  # SPDX-License-Identifier
 
 import ctypes as ct
 import ctypes.util as ctutil
 from json import loads
 from sys import platform
 from typing import Any, Callable, Dict, List, Tuple, Type
```

### Comparing `caen_felib-1.0.4/src/caen_felib.egg-info/PKG-INFO` & `caen_felib-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: caen-felib
-Version: 1.0.4
+Name: caen_felib
+Version: 1.0.5
 Summary: Official Python wrapper for the CAEN FELib.
 Author-email: Giovanni Cerretani <g.cerretani@caen.it>, Daniele Ninci <d.ninci@caen.it>
 Project-URL: homepage, https://www.caen.it
 Project-URL: documentation, https://www.caen.it/products/caen-felib-library/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

