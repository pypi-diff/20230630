# Comparing `tmp/pycommons_base-0.0.5.tar.gz` & `tmp/pycommons_base-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycommons_base-0.0.5.tar", max compression
+gzip compressed data, was "pycommons_base-0.0.6.tar", max compression
```

## Comparing `pycommons_base-0.0.5.tar` & `pycommons_base-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0    11346 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/LICENSE
--rw-r--r--   0        0        0     1082 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/README.md
--rw-r--r--   0        0        0      431 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/__init__.py
--rw-r--r--   0        0        0      153 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/atomic/__init__.py
--rw-r--r--   0        0        0      759 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/atomic/atomic.py
--rw-r--r--   0        0        0      768 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/atomic/boolean.py
--rw-r--r--   0        0        0     1791 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/atomic/integer.py
--rw-r--r--   0        0        0     5648 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/char.py
--rw-r--r--   0        0        0      235 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/container/__init__.py
--rw-r--r--   0        0        0      813 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/container/boolean.py
--rw-r--r--   0        0        0      849 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/container/container.py
--rw-r--r--   0        0        0     1469 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/container/integer.py
--rw-r--r--   0        0        0     4457 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/container/optional.py
--rw-r--r--   0        0        0       88 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/exception/__init__.py
--rw-r--r--   0        0        0      367 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/exception/no_such_element_error.py
--rw-r--r--   0        0        0      320 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/function/__init__.py
--rw-r--r--   0        0        0     1266 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/function/comparator.py
--rw-r--r--   0        0        0     1454 2023-06-11 14:19:08.206050 pycommons_base-0.0.5/pycommons/base/function/consumer.py
--rw-r--r--   0        0        0      594 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/function/function.py
--rw-r--r--   0        0        0     2249 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/function/predicate.py
--rw-r--r--   0        0        0      496 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/function/runnable.py
--rw-r--r--   0        0        0      532 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/function/supplier.py
--rw-r--r--   0        0        0      144 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/streams/__init__.py
--rw-r--r--   0        0        0     6823 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/streams/iterator.py
--rw-r--r--   0        0        0     2264 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/streams/stream.py
--rw-r--r--   0        0        0      725 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/streams/streams.py
--rw-r--r--   0        0        0      987 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/synchronized.py
--rw-r--r--   0        0        0       64 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/utils/__init__.py
--rw-r--r--   0        0        0      587 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/utils/objectutils.py
--rw-r--r--   0        0        0      119 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/base/utils/utils.py
--rw-r--r--   0        0        0        0 2023-06-11 14:19:08.210050 pycommons_base-0.0.5/pycommons/py.typed
--rw-r--r--   0        0        0     1828 2023-06-11 14:19:22.621852 pycommons_base-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 pycommons_base-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-30 10:20:07.019579 pycommons_base-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1082 2023-06-30 10:20:07.019579 pycommons_base-0.0.6/README.md
+-rw-r--r--   0        0        0      431 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/atomic/__init__.py
+-rw-r--r--   0        0        0     1348 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/atomic/atomic.py
+-rw-r--r--   0        0        0     1136 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/atomic/boolean.py
+-rw-r--r--   0        0        0     1791 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/atomic/integer.py
+-rw-r--r--   0        0        0     5648 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/char.py
+-rw-r--r--   0        0        0      235 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/__init__.py
+-rw-r--r--   0        0        0     3191 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/boolean.py
+-rw-r--r--   0        0        0     3100 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/container.py
+-rw-r--r--   0        0        0     4334 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/integer.py
+-rw-r--r--   0        0        0     4733 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/optional.py
+-rw-r--r--   0        0        0      427 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/exception/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/__init__.py
+-rw-r--r--   0        0        0     1266 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/comparator.py
+-rw-r--r--   0        0        0     2451 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/consumer.py
+-rw-r--r--   0        0        0     1089 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/function.py
+-rw-r--r--   0        0        0      215 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/interface.py
+-rw-r--r--   0        0        0     4570 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/predicate.py
+-rw-r--r--   0        0        0     1752 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/runnable.py
+-rw-r--r--   0        0        0     2051 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/supplier.py
+-rw-r--r--   0        0        0       41 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/maps/__init__.py
+-rw-r--r--   0        0        0     6975 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/maps/maps.py
+-rw-r--r--   0        0        0      144 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/streams/__init__.py
+-rw-r--r--   0        0        0     6823 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/streams/iterator.py
+-rw-r--r--   0        0        0     2264 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/streams/stream.py
+-rw-r--r--   0        0        0      725 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/streams/streams.py
+-rw-r--r--   0        0        0      987 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/synchronized.py
+-rw-r--r--   0        0        0      112 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/utils/__init__.py
+-rw-r--r--   0        0        0     1458 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/utils/objectutils.py
+-rw-r--r--   0        0        0      119 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/py.typed
+-rw-r--r--   0        0        0     1821 2023-06-30 10:20:21.443592 pycommons_base-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 pycommons_base-0.0.6/PKG-INFO
```

### Comparing `pycommons_base-0.0.5/LICENSE` & `pycommons_base-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/README.md` & `pycommons_base-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/pycommons/base/atomic/integer.py` & `pycommons_base-0.0.6/pycommons/base/atomic/integer.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/pycommons/base/char.py` & `pycommons_base-0.0.6/pycommons/base/char.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/pycommons/base/container/optional.py` & `pycommons_base-0.0.6/pycommons/base/container/optional.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 
 from typing import Generic, TypeVar, Any, Optional
 
 from pycommons.base.exception import NoSuchElementError
 from pycommons.base.function.consumer import Consumer
 from pycommons.base.function.function import Function
 from pycommons.base.function.predicate import Predicate
-from pycommons.base.function.runnable import Runnable
-from pycommons.base.function.supplier import Supplier
+from pycommons.base.function.runnable import RunnableType, Runnable
+from pycommons.base.function.supplier import Supplier, SupplierType
 from pycommons.base.utils.objectutils import ObjectUtils
 
 _T = TypeVar("_T", Any, None)
 _U = TypeVar("_U", Any, None)
 _E = TypeVar("_E", RuntimeError, Exception)
 
 
 class OptionalContainer(Generic[_T]):
     """
     Identical implementation of Java's Optional.
-    A container object which may or may not contain a non-null value
+    A container object which may or may not contain a non-null value.
 
-    See Also
+    References:
         https://docs.oracle.com/javase/8/docs/api/java/util/Optional.html
     """
 
     _value: _T
 
     def __init__(self, value: Optional[_T]):
+        """
+        Initialize the container with a value if present, None if not.
+        Args:
+            value: The initializing value. Can be None or not-None
+        """
         self._value = value
 
     def get(self) -> _T:
         """
         Gets the value in the container
 
         Returns:
@@ -72,29 +77,29 @@
         Returns:
             None
         """
         ObjectUtils.require_not_none(consumer)
         if self.is_present():
             consumer.accept(self._value)
 
-    def if_present_or_else(self, consumer: Consumer[_T], runnable: Runnable) -> None:
+    def if_present_or_else(self, consumer: Consumer[_T], runnable: RunnableType) -> None:
         """
         Runs a consumer if the value is present, else runs the runnable
         Args:
             consumer: Consumer function that runs when value is present
             runnable: Runnable function that runs when value is None
 
         Returns:
             None
         """
         ObjectUtils.require_not_none(consumer)
         if self.is_present():
             consumer.accept(self._value)
         else:
-            runnable.run()
+            Runnable.of(runnable).run()
 
     def filter(self, predicate: Predicate[_T]) -> OptionalContainer[_T]:
         ObjectUtils.require_not_none(predicate)
         if self.is_empty():
             return self
 
         return self if predicate.test(self._value) else OptionalContainer.empty()
@@ -109,30 +114,30 @@
     def flat_map(self, mapper: Function[_T, OptionalContainer[_U]]) -> OptionalContainer[_U]:
         ObjectUtils.require_not_none(mapper)
         if self.is_empty():
             return OptionalContainer.empty()
 
         return ObjectUtils.get_not_none(mapper.apply(self._value))
 
-    def in_turn(self, supplier: Supplier[OptionalContainer[_T]]) -> OptionalContainer[_T]:
+    def in_turn(self, supplier: SupplierType[OptionalContainer[_T]]) -> OptionalContainer[_T]:
         if self.is_present():
             return self
 
-        return ObjectUtils.get_not_none(supplier.get())
+        return ObjectUtils.get_not_none(Supplier.of(supplier).get())
 
     def or_else(self, other: _T) -> _T:
         return self._value if self.is_present() else other
 
-    def or_else_get(self, supplier: Supplier[_T]) -> _T:
-        return self._value if self.is_present() else supplier.get()
+    def or_else_get(self, supplier: SupplierType[_T]) -> _T:
+        return self._value if self.is_present() else Supplier.of(supplier).get()
 
-    def or_else_throw(self, supplier: Optional[Supplier[_E]] = None) -> _T:
+    def or_else_throw(self, supplier: Optional[SupplierType[_E]] = None) -> _T:
         if self.is_empty():
             if supplier:
-                raise supplier.get()
+                raise Supplier.of(supplier).get()
             raise NoSuchElementError("No value present")
         return self._value
 
     @classmethod
     def of(cls, value: _T) -> OptionalContainer[_T]:
         if value is None:
             raise TypeError("Value cannot be None")
```

### Comparing `pycommons_base-0.0.5/pycommons/base/function/comparator.py` & `pycommons_base-0.0.6/pycommons/base/function/comparator.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/pycommons/base/streams/iterator.py` & `pycommons_base-0.0.6/pycommons/base/streams/iterator.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/pycommons/base/streams/stream.py` & `pycommons_base-0.0.6/pycommons/base/streams/stream.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/pycommons/base/streams/streams.py` & `pycommons_base-0.0.6/pycommons/base/streams/streams.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/pycommons/base/synchronized.py` & `pycommons_base-0.0.6/pycommons/base/synchronized.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.5/pyproject.toml` & `pycommons_base-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool]
 
 [tool.poetry]
 name = "pycommons.base"
-version = "0.0.5"
+version = "0.0.6"
 homepage = "https://github.com/shashankrnr32/pycommons-base"
 description = "Python Commons Base"
 authors = ["Shashank Sharma <shashankrnr32@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -24,16 +24,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 importlib_metadata = "*"
 typing_extensions = "4.6.3"
 
 [tool.poetry.dev-dependencies]
-mkdocs-material = ">7.0.0"
-mkdocstrings = { version = ">0.18", extras = ["python-legacy"] }
+mkdocs-material = ">7.1.0"
+mkdocstrings = { version = ">0.18", extras = ["python"] }
 mkdocs-awesome-pages-plugin = "*"
 markdown-include = "*"
 livereload = "*"
 poethepoet = "^0.20.0"
 
 pytest = ">=7.2.0"
 pytest-cov = "^2.10.1"
```

### Comparing `pycommons_base-0.0.5/PKG-INFO` & `pycommons_base-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycommons-base
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Commons Base
 Home-page: https://github.com/shashankrnr32/pycommons-base
 License: Apache-2.0
 Author: Shashank Sharma
 Author-email: shashankrnr32@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

