# Comparing `tmp/pyrepresent-0.1.2.tar.gz` & `tmp/pyrepresent-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.1.2.tar", last modified: Mon Jun 19 17:06:22 2023, max compression
+gzip compressed data, was "pyrepresent-0.1.3.tar", last modified: Fri Jun 30 19:49:51 2023, max compression
```

## Comparing `pyrepresent-0.1.2.tar` & `pyrepresent-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 17:06:22.511126 pyrepresent-0.1.2/
--rw-rw-rw-   0        0        0      115 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-06-19 17:06:22.510676 pyrepresent-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.2/README.md
--rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.1.2/build.py
--rw-rw-rw-   0        0        0      715 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-19 17:06:22.503676 pyrepresent-0.1.2/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 17:06:22.000000 pyrepresent-0.1.2/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 17:06:22.509675 pyrepresent-0.1.2/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.2/represent/__init__.py
--rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.1.2/represent/base.py
--rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.1.2/represent/document.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.2/represent/indentation.py
--rw-rw-rw-   0        0        0    19303 2023-06-19 17:04:33.000000 pyrepresent-0.1.2/represent/object.py
--rw-rw-rw-   0        0        0    20795 2023-06-19 17:05:54.000000 pyrepresent-0.1.2/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 17:06:22.511126 pyrepresent-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-19 17:06:11.000000 pyrepresent-0.1.2/setup.py
--rw-rw-rw-   0        0        0      971 2023-06-13 13:18:42.000000 pyrepresent-0.1.2/test.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:49:51.980747 pyrepresent-0.1.3/
+-rw-rw-rw-   0        0        0      115 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5268 2023-06-30 19:49:51.979775 pyrepresent-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.3/README.md
+-rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.1.3/build.py
+-rw-rw-rw-   0        0        0      715 2023-06-30 18:38:22.000000 pyrepresent-0.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-30 19:49:51.973760 pyrepresent-0.1.3/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 19:49:51.978749 pyrepresent-0.1.3/represent/
+-rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.3/represent/__init__.py
+-rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.1.3/represent/base.py
+-rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.1.3/represent/document.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.3/represent/indentation.py
+-rw-rw-rw-   0        0        0    19907 2023-06-30 19:49:10.000000 pyrepresent-0.1.3/represent/object.py
+-rw-rw-rw-   0        0        0    20997 2023-06-30 19:26:36.000000 pyrepresent-0.1.3/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 19:49:51.980747 pyrepresent-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-30 18:38:17.000000 pyrepresent-0.1.3/setup.py
+-rw-rw-rw-   0        0        0     1028 2023-06-30 19:49:35.000000 pyrepresent-0.1.3/test.py
```

### Comparing `pyrepresent-0.1.2/PKG-INFO` & `pyrepresent-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.1.2
+Version: 0.1.3
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.1.2/README.md` & `pyrepresent-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.2/build.py` & `pyrepresent-0.1.3/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.2/pyproject.toml` & `pyrepresent-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.1.2'
+version = '0.1.3'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.1.2/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.1.3/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.1.2
+Version: 0.1.3
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.1.2/represent/base.py` & `pyrepresent-0.1.3/represent/base.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.2/represent/indentation.py` & `pyrepresent-0.1.3/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.2/represent/object.py` & `pyrepresent-0.1.3/represent/object.py`

 * *Files 7% similar despite different names*

```diff
@@ -126,14 +126,16 @@
         return to_string(self)
     # end __str__
 # end BaseModel
 
 class FrozenHashable:
     """A hashable dict structure."""
 
+    _cache = {}
+
     def __hash__(self) -> int:
         """
         Returns the hash of the signature for hashing the object.
 
         :return: The hash of the object.
         """
 
@@ -145,18 +147,20 @@
         Checks if the signatures of the objects are the same.
 
         :param other: The other object to compare.
 
         :return: The equality value.
         """
 
-        return (
-                (type(self) is type(other)) and
-                (self._signature == other.__signature)
-        )
+        if type(self) is not type(other):
+            return NotImplemented
+        # end if
+
+        # noinspection PyProtectedMember
+        return self._signature == other._signature
     # end __eq__
 
     def __str__(self) -> str:
         """
         Returns a string to represent the model commands and structure.
 
         :return: The string representation of the model.
@@ -213,54 +217,59 @@
     def _signature(self) -> Tuple[Tuple[Any, Any], ...]:
         """
         Returns a hashable dict signature.
 
         :return: The signature of the object.
         """
 
-        data = []
+        data = [(f"--id--", id(self))]
 
-        matches = {
-            dict: HashableDict,
-            list: HashableList,
-            set: HashableSet
-        }
+        if id(self) in self._cache:
+            return tuple(self._cache[id(self)])
+        # end if
+
+        self._cache[id(self)] = data
 
         for key in self:
             value = self[key]
 
-            for base, hashable_base in matches.items():
+            for base, hashable_base in hashable_matches.items():
                 if isinstance(key, base) and not isinstance(key, hashable_base):
                     try:
                         hash(key)
 
                     except TypeError:
                         key = hashable_base(key)
                     # end try
                 # end if
             # end for
 
-            for base, hashable_base in matches.items():
+            for base, hashable_base in hashable_matches.items():
                 if isinstance(value, base) and not isinstance(value, hashable_base):
                     try:
                         hash(value)
 
                     except TypeError:
                         value = hashable_base(value)
                     # end try
                 # end if
             # end for
 
             data.append((key, value))
         # end for
 
-        data.sort(key=lambda v: hash(v))
+        try:
+            data.sort(key=lambda v: hash(v))
 
-        return tuple(data)
-    # end __signature
+        except RecursionError:
+            pass
+        # end try
+
+        return tuple(self._cache[id(self)])
+    # end _signature
 
     def __str__(self) -> str:
         """
         Returns a string to represent the object.
 
         :return: A string representation for the commands of the object.
         """
@@ -282,41 +291,46 @@
     def _signature(self) -> Tuple[Any, ...]:
         """
         Returns a hashable dict signature.
 
         :return: The signature of the object.
         """
 
-        data = []
+        data = [("--id--", id(self))]
 
-        matches = {
-            dict: HashableDict,
-            list: HashableList,
-            set: HashableSet
-        }
+        if id(self) in self._cache:
+            return tuple(self._cache[id(self)])
+        # end if
+
+        self._cache[id(self)] = data
 
         for value in self:
-            for base, hashable_base in matches.items():
+            for base, hashable_base in hashable_matches.items():
                 if isinstance(value, base) and not isinstance(value, hashable_base):
                     try:
                         hash(value)
 
                     except TypeError:
                         value = hashable_base(value)
                     # end try
                 # end if
             # end for
 
             data.append(value)
         # end for
 
-        data.sort(key=lambda v: hash(v))
+        try:
+            data.sort(key=lambda v: hash(v))
 
-        return tuple(data)
-    # end __signature
+        except RecursionError:
+            pass
+        # end try
+
+        return tuple(self._cache[id(self)])
+    # end _signature
 
     def __str__(self) -> str:
         """
         Returns a string to represent the object.
 
         :return: A string representation for the commands of the object.
         """
@@ -338,41 +352,46 @@
     def _signature(self) -> Tuple[Any, ...]:
         """
         Returns a hashable dict signature.
 
         :return: The signature of the object.
         """
 
-        data = []
+        data = [("--id--", id(self))]
+
+        if id(self) in self._cache:
+            return tuple(self._cache[id(self)])
+        # end if
 
-        matches = {
-            dict: HashableDict,
-            list: HashableList,
-            set: HashableSet
-        }
+        self._cache[id(self)] = data
 
         for value in self:
-            for base, hashable_base in matches.items():
+            for base, hashable_base in hashable_matches.items():
                 if isinstance(value, base) and not isinstance(value, hashable_base):
                     try:
                         hash(value)
 
                     except TypeError:
                         value = hashable_base(value)
                     # end try
                 # end if
             # end for
 
             data.append(value)
         # end for
 
-        data.sort(key=lambda v: hash(v))
+        try:
+            data.sort(key=lambda v: hash(v))
 
-        return tuple(data)
-    # end __signature
+        except RecursionError:
+            pass
+        # end try
+
+        return tuple(self._cache[id(self)])
+    # end _signature
 
     def __str__(self) -> str:
         """
         Returns a string to represent the object.
 
         :return: A string representation for the commands of the object.
         """
@@ -383,14 +402,20 @@
             return HashableSet.__name__ + "(" + content + ")"
         # end if
 
         return content
     # end __str__
 # end HashableDict
 
+hashable_matches = {
+    dict: HashableDict,
+    list: HashableList,
+    set: HashableSet
+}
+
 def unwrap(
         data: Any, /, *,
         hidden: Optional[Union[Dict[Any, Any], Iterable[Any]]] = None,
         assign: Optional[bool] = False,
         properties: Optional[bool] = False,
         protected: Optional[bool] = False,
         legalize: Optional[bool] = False,
@@ -457,28 +482,27 @@
     else:
         if isinstance(data, types.FunctionType):
             ids[data_id] = repr(data) if legalize else FunctionStructure(data)
 
             return ids[data_id]
         # end if
 
-        # noinspection PyTypeChecker
         ids[data_id] = (
             data if (
                 (type(data).__name__ in dir(builtins) + dir(dt)) or
                 (data is None)
             )
             else (
                 (
                     repr(CircularReferenceStructure(data))
                     if legalize else (
                         StringWrapper(repr(CircularReferenceStructure(data)))
                     )
                 ) if (repr(data) != repr(HiddenStructure()))
-                else (data if legalize else StringWrapper(data))
+                else (data if legalize else StringWrapper(repr(data)))
             )
         )
     # end if
 
     assignment = None
 
     bound = False
```

### Comparing `pyrepresent-0.1.2/represent/structures.py` & `pyrepresent-0.1.3/represent/structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,19 +95,19 @@
         if not color:
             return content
         # end if
 
         name = content
 
         return (
-                name[:name.rfind(".") + 1] +
-                Colors.CYAN +
-                name[name.rfind(".") + 1:len(name) + name.find("(") + 1] +
-                Colors.END +
-                name[len(name) + name.find("(") + 1:]
+            name[:name.rfind(".") + 1] +
+            Colors.CYAN +
+            name[name.rfind(".") + 1:len(name) + name.find("(") + 1] +
+            Colors.END +
+            name[len(name) + name.find("(") + 1:]
         )
     # end color_repr_class
 
     @staticmethod
     def color_repr_class(content: str, color: Optional[bool] = True) -> str:
         """
         Colors the string of the object's repr.
@@ -121,19 +121,19 @@
         if not color:
             return content
         # end if
 
         name = content
 
         return (
-                name[:name.rfind(".") + 1] +
-                Colors.CYAN +
-                name[name.rfind(".") + 1:name.find(" object at")] +
-                Colors.END +
-                name[name.find(" object at"):]
+            name[:name.rfind(".") + 1] +
+            Colors.CYAN +
+            name[name.rfind(".") + 1:name.find(" object at")] +
+            Colors.END +
+            name[name.find(" object at"):]
         )
     # end color_repr_class
 
     @staticmethod
     def color_repr(content: str, value: Any, color: Optional[bool] = True) -> str:
         """
         Colors the string of the object's repr.
@@ -339,15 +339,19 @@
 
         try:
             return (
                 constructor(*args, **kwargs).
                 replace("END$$(", Colors.END + "(").
                 replace("END$$,", Colors.END + ",").
                 replace("END$$[", Colors.END + "[").
-                replace("END$${", Colors.END + "{")
+                replace("END$${", Colors.END + "{").
+                replace(Colors.END + Colors.END, Colors.END).
+                replace(f">{Colors.END}END$$(", ">(").
+                replace(f"$E{Colors.END}ND$", Colors.END).
+                replace(Colors.RED + Colors.RED, Colors.RED)
             )
 
         except RecursionError:
             return repr(CircularReferenceStructure(*args, **kwargs))
         # end try
     # end __str__
```

### Comparing `pyrepresent-0.1.2/setup.py` & `pyrepresent-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.1.2',
+        version='0.1.3',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.1.2/test.py` & `pyrepresent-0.1.3/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # test.py
 
 import pandas as pd
 import numpy as np
 
-from represent import BaseModel
+from represent import BaseModel, to_string
 
 class Model(BaseModel):
 
     def __init__(self) -> None:
 
         self.self = self
         self.type = type(self)
@@ -42,12 +42,13 @@
 # end Data
 
 def main() -> None:
     """Tests the module."""
 
     print(Model())
     print(Data())
+    print(to_string({Data(): 0, Data(): 1}))
 # end main
 
 if __name__ == "__main__":
     main()
 # end if
```

