# Comparing `tmp/markyp-0.2306.1.tar.gz` & `tmp/markyp-0.2307.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markyp-0.2306.1.tar", last modified: Tue Jun 20 12:35:21 2023, max compression
+gzip compressed data, was "markyp-0.2307.0.tar", last modified: Fri Jun 30 15:07:02 2023, max compression
```

## Comparing `markyp-0.2306.1.tar` & `markyp-0.2307.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:35:21.088674 markyp-0.2306.1/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2023-06-19 14:11:00.000000 markyp-0.2306.1/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)     7790 2023-06-20 12:35:21.088674 markyp-0.2306.1/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     6710 2023-06-19 14:11:00.000000 markyp-0.2306.1/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:35:21.084674 markyp-0.2306.1/markyp/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1503 2023-06-20 12:35:10.000000 markyp-0.2306.1/markyp/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    11810 2023-06-19 14:11:00.000000 markyp-0.2306.1/markyp/elements.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2722 2023-06-19 14:11:00.000000 markyp-0.2306.1/markyp/formatters.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8304 2023-06-19 14:11:00.000000 markyp-0.2306.1/markyp/parser.py
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-06-19 14:11:21.000000 markyp-0.2306.1/markyp/py.typed
--rw-rw-r--   0 peter     (1000) peter     (1000)     1321 2023-06-19 14:11:00.000000 markyp-0.2306.1/markyp/utils.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:35:21.088674 markyp-0.2306.1/markyp.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     7790 2023-06-20 12:35:21.000000 markyp-0.2306.1/markyp.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      357 2023-06-20 12:35:21.000000 markyp-0.2306.1/markyp.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-20 12:35:21.000000 markyp-0.2306.1/markyp.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        7 2023-06-20 12:35:21.000000 markyp-0.2306.1/markyp.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-20 12:35:21.088674 markyp-0.2306.1/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2588 2023-06-20 12:35:02.000000 markyp-0.2306.1/setup.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:35:21.088674 markyp-0.2306.1/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)    17898 2023-06-19 14:11:00.000000 markyp-0.2306.1/test/test_elements.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2857 2023-06-19 14:11:00.000000 markyp-0.2306.1/test/test_formatters.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      521 2023-06-19 14:11:00.000000 markyp-0.2306.1/test/test_init.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4691 2023-06-19 14:11:00.000000 markyp-0.2306.1/test/test_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1359 2023-06-19 14:11:00.000000 markyp-0.2306.1/test/test_utils.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-30 15:07:02.003298 markyp-0.2307.0/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2023-06-19 14:11:00.000000 markyp-0.2307.0/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7893 2023-06-30 15:07:02.003298 markyp-0.2307.0/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6710 2023-06-19 14:11:00.000000 markyp-0.2307.0/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-30 15:07:01.999298 markyp-0.2307.0/markyp/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1503 2023-06-30 15:03:41.000000 markyp-0.2307.0/markyp/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11983 2023-06-30 14:51:32.000000 markyp-0.2307.0/markyp/elements.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2729 2023-06-30 14:21:01.000000 markyp-0.2307.0/markyp/formatters.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8303 2023-06-30 14:48:38.000000 markyp-0.2307.0/markyp/parser.py
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-06-19 14:11:21.000000 markyp-0.2307.0/markyp/py.typed
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1321 2023-06-19 14:11:00.000000 markyp-0.2307.0/markyp/utils.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-30 15:07:01.999298 markyp-0.2307.0/markyp.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7893 2023-06-30 15:07:01.000000 markyp-0.2307.0/markyp.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      357 2023-06-30 15:07:01.000000 markyp-0.2307.0/markyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-30 15:07:01.000000 markyp-0.2307.0/markyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        7 2023-06-30 15:07:01.000000 markyp-0.2307.0/markyp.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-30 15:07:02.003298 markyp-0.2307.0/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2689 2023-06-30 15:02:58.000000 markyp-0.2307.0/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-30 15:07:02.003298 markyp-0.2307.0/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    17898 2023-06-19 14:11:00.000000 markyp-0.2307.0/test/test_elements.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2857 2023-06-19 14:11:00.000000 markyp-0.2307.0/test/test_formatters.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      521 2023-06-19 14:11:00.000000 markyp-0.2307.0/test/test_init.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4691 2023-06-19 14:11:00.000000 markyp-0.2307.0/test/test_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1359 2023-06-19 14:11:00.000000 markyp-0.2307.0/test/test_utils.py
```

### Comparing `markyp-0.2306.1/LICENSE` & `markyp-0.2307.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markyp-0.2306.1/PKG-INFO` & `markyp-0.2307.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: markyp
-Version: 0.2306.1
+Version: 0.2307.0
 Summary: Python 3 tools for creating markup documents.
 Home-page: https://github.com/volfpeter/markyp
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 License: MIT
 Keywords: markup generator utility xml html rss
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://travis-ci.org/volfpeter/markyp.svg?branch=master)](https://travis-ci.org/volfpeter/markyp)
 [![Downloads](https://pepy.tech/badge/markyp)](https://pepy.tech/project/markyp)
 [![Downloads](https://pepy.tech/badge/markyp/month)](https://pepy.tech/project/markyp/month)
 [![Downloads](https://pepy.tech/badge/markyp/week)](https://pepy.tech/project/markyp/week)
```

### Comparing `markyp-0.2306.1/README.md` & `markyp-0.2307.0/README.md`

 * *Files identical despite different names*

### Comparing `markyp-0.2306.1/markyp/__init__.py` & `markyp-0.2307.0/markyp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Dict, Union
 
 __author__ = "Peter Volf"
 __copyright__ = "Copyright 2019, Peter Volf"
 __email__ = "do.volfp@gmail.com"
 __license__ = "MIT"
 __url__ = "https://github.com/volfpeter/markyp"
-__version__ = "0.2306.1"
+__version__ = "0.2307.0"
 
 
 __all__ = ("IElement", "ElementType", "PropertyValue", "PropertyDict", "is_element")
 
 
 class IElement(object):
     """
```

### Comparing `markyp-0.2306.1/markyp/elements.py` & `markyp-0.2307.0/markyp/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Base `markyp` element implementations.
 """
 
-from typing import List, Sequence, Optional
+from typing import Sequence, Optional
 
-from markyp import ElementType, IElement, PropertyDict, PropertyValue, is_element
+from markyp import ElementType, IElement, PropertyDict, PropertyValue
 from markyp.formatters import (
     format_element_sequence,
     format_properties,
     xml_format_element,
     xml_escape,
 )
 
@@ -65,15 +65,15 @@
         """
         Whether the children of the element should be placed on the same line as the element.
 
         The default value is `False`.
         """
         return False
 
-    def get_element_children(self) -> Optional[Sequence[ElementType]]:
+    def get_element_children(self) -> Optional[Sequence[ElementType | None]]:
         """
         Returns the children elements of the element if it has children.
         """
         return None
 
     def get_element_properties(self) -> Optional[PropertyDict]:
         """
@@ -87,22 +87,22 @@
     Base class for elements that have no properties, only children.
 
     Define `__slots__` in derived classes to enjoy the performance benefits the feature provides.
     """
 
     __slots__ = ("children",)
 
-    def __init__(self, *args: ElementType) -> None:
+    def __init__(self, *args: ElementType | None) -> None:
         """
         Initialization.
 
         An arbitrary number of positional arguments are accepted that must be either `IElement`
         instances or strings. Each positional argument will become a child of the element.
         """
-        self.children: Sequence[ElementType] = args
+        self.children: Sequence[ElementType | None] = args
         """The child elements."""
 
     def __str__(self) -> str:
         name: str = self.element_name
         return f"<{name}>{format_element_sequence(self.children, element_formatter=xml_format_element, inline=self.inline_children)}</{name}>"
 
     @property
@@ -135,26 +135,29 @@
 
     Define `__slots__` in derived classes to enjoy the performance benefits the feature provides.
     """
 
     __slots__ = ("children", "properties")
 
     def __init__(
-        self, *args: ElementType, class_: Optional[str] = None, **kwargs: PropertyValue
+        self,
+        *args: ElementType | None,
+        class_: Optional[str] = None,
+        **kwargs: PropertyValue,
     ) -> None:
         """
         Initialization.
 
         An arbitrary number of positional arguments are accepted that must be either `IElement`
         instances or strings. Each positional argument will become a child of the element.
 
         The `class_` keyword argument is converted into the `class` element property,
         other keyword arguments are converted to element properties as they were defined.
         """
-        self.children: Sequence[ElementType] = args
+        self.children: Sequence[ElementType | None] = args
         """The child elements."""
 
         self.properties: PropertyDict = kwargs
         """The properties to set on the element."""
 
         if class_ is not None:
             self.properties["class"] = class_
@@ -209,15 +212,21 @@
 
     __slots__ = ()
 
     def __str__(self) -> str:
         return (
             ""
             if len(self.children) == 0
-            else "\n".join((xml_format_element(element) for element in self.children))
+            else "\n".join(
+                (
+                    xml_format_element(element)
+                    for element in self.children
+                    if element is not None
+                )
+            )
         )
 
 
 class EmptyElement(IElement):
     """
     Base class for elements that have no children, only properties.
```

### Comparing `markyp-0.2306.1/markyp/formatters.py` & `markyp-0.2307.0/markyp/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Generic `markyp` element formatters.
 """
 
-from typing import Any, Callable, Dict, Sequence, Union
+from typing import Callable, Sequence, Union
 
 from xml.sax.saxutils import escape as xml_escape
 
 from markyp import ElementType, PropertyDict, PropertyValue
 
 
 __all__ = (
     "format_property",
     "format_properties",
     "xml_format_element",
+    "xml_escape",
     "format_element_sequence",
 )
 
 
 def format_property(name: str, value: PropertyValue) -> str:
     """
     Formatter function for element properties.
```

### Comparing `markyp-0.2306.1/markyp/parser.py` & `markyp-0.2307.0/markyp/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 class IgnoreElement(IElement):
     """
     Element to use in `ParserRule`s for tags that should not be parsed.
     """
 
     __slots__ = ()
 
-    def __new__(cls, *args, **kwargs) -> None:
+    def __new__(cls, *args, **kwargs) -> None:  # type: ignore
         return None
 
 
 class Parser:
     """
     `markyp` element parser.
 
@@ -182,15 +182,15 @@
 
         if factory == AnyElement:
             props["element_tag"] = tag
 
         if self._converter is not None:
             factory, children, props = self._converter(factory, children, props)
 
-        return factory(*children, **props)  # type: ignore
+        return factory(*children, **props)
 
     def fromstring(self, data: str) -> ElementType:
         """
         Parses the given XML string.
 
         Arguments:
             data: The string to parse.
@@ -274,8 +274,7 @@
         """
         Returns whether the given value is an empty string or `None`.
 
         Arguments:
             value: The value to check.
         """
         return value is None or value.strip() == ""
-
```

### Comparing `markyp-0.2306.1/markyp/utils.py` & `markyp-0.2307.0/markyp/utils.py`

 * *Files identical despite different names*

### Comparing `markyp-0.2306.1/markyp.egg-info/PKG-INFO` & `markyp-0.2307.0/markyp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: markyp
-Version: 0.2306.1
+Version: 0.2307.0
 Summary: Python 3 tools for creating markup documents.
 Home-page: https://github.com/volfpeter/markyp
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 License: MIT
 Keywords: markup generator utility xml html rss
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://travis-ci.org/volfpeter/markyp.svg?branch=master)](https://travis-ci.org/volfpeter/markyp)
 [![Downloads](https://pepy.tech/badge/markyp)](https://pepy.tech/project/markyp)
 [![Downloads](https://pepy.tech/badge/markyp/month)](https://pepy.tech/project/markyp/month)
 [![Downloads](https://pepy.tech/badge/markyp/week)](https://pepy.tech/project/markyp/week)
```

### Comparing `markyp-0.2306.1/setup.py` & `markyp-0.2307.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,23 +50,25 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development",
         "Topic :: Software Development :: Code Generators",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Text Processing :: Markup",
         "Topic :: Utilities",
         "Typing :: Typed",
     ],
     keywords="markup generator utility xml html rss",
     packages=find_packages(exclude=["test"]),
     package_data={"markyp": ["py.typed"]},
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=requirements,
 )
```

### Comparing `markyp-0.2306.1/test/test_elements.py` & `markyp-0.2307.0/test/test_elements.py`

 * *Files identical despite different names*

### Comparing `markyp-0.2306.1/test/test_formatters.py` & `markyp-0.2307.0/test/test_formatters.py`

 * *Files identical despite different names*

### Comparing `markyp-0.2306.1/test/test_init.py` & `markyp-0.2307.0/test/test_init.py`

 * *Files identical despite different names*

### Comparing `markyp-0.2306.1/test/test_parser.py` & `markyp-0.2307.0/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `markyp-0.2306.1/test/test_utils.py` & `markyp-0.2307.0/test/test_utils.py`

 * *Files identical despite different names*

