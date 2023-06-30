# Comparing `tmp/pynabi-0.1.0.tar.gz` & `tmp/pynabi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\feder\Documents\Scuola\Univerit\340\prova finale 3\nasello\dist\.tmp-80jw1a2k\pynabi-0.1.0.tar", last modified: Fri Jun 30 17:24:02 2023, max compression
+gzip compressed data, was "C:\Users\feder\Documents\Scuola\Univerit\340\prova finale 3\nasello\dist\.tmp-x8rox8y2\pynabi-0.1.1.tar", last modified: Fri Jun 30 18:52:21 2023, max compression
```

## Comparing `pynabi-0.1.0.tar` & `pynabi-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 17:24:02.782640 pynabi-0.1.0/
--rw-rw-rw-   0        0        0     1094 2023-06-14 17:22:45.000000 pynabi-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     8279 2023-06-30 17:24:02.781646 pynabi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5996 2023-06-30 17:07:24.000000 pynabi-0.1.0/README.md
--rw-rw-rw-   0        0        0     1084 2023-06-30 17:08:50.000000 pynabi-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 17:24:02.782640 pynabi-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 17:24:02.734703 pynabi-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 17:24:02.773633 pynabi-0.1.0/src/pynabi/
--rw-rw-rw-   0        0        0       47 2023-06-30 16:56:26.000000 pynabi-0.1.0/src/pynabi/__init__.py
--rw-rw-rw-   0        0        0     6041 2023-06-30 17:18:11.000000 pynabi-0.1.0/src/pynabi/_common.py
--rw-rw-rw-   0        0        0     8903 2023-06-25 12:06:13.000000 pynabi-0.1.0/src/pynabi/_dataset.py
--rw-rw-rw-   0        0        0     4204 2023-06-17 21:06:56.000000 pynabi-0.1.0/src/pynabi/calculation.py
--rw-rw-rw-   0        0        0     9529 2023-06-17 21:28:04.000000 pynabi-0.1.0/src/pynabi/crystal.py
--rw-rw-rw-   0        0        0    11672 2023-06-30 17:18:06.000000 pynabi-0.1.0/src/pynabi/kspace.py
--rw-rw-rw-   0        0        0     7844 2023-06-21 21:36:17.000000 pynabi-0.1.0/src/pynabi/occupation.py
--rw-rw-rw-   0        0        0    14540 2023-06-17 19:55:26.000000 pynabi-0.1.0/src/pynabi/relaxation.py
--rw-rw-rw-   0        0        0     3727 2023-06-17 21:24:10.000000 pynabi-0.1.0/src/pynabi/units.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:24:02.779621 pynabi-0.1.0/src/pynabi.egg-info/
--rw-rw-rw-   0        0        0     8279 2023-06-30 17:24:02.000000 pynabi-0.1.0/src/pynabi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-30 17:24:02.000000 pynabi-0.1.0/src/pynabi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 17:24:02.000000 pynabi-0.1.0/src/pynabi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 17:24:02.000000 pynabi-0.1.0/src/pynabi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 18:52:21.183422 pynabi-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-06-14 17:22:45.000000 pynabi-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     8272 2023-06-30 18:52:21.183422 pynabi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5989 2023-06-30 17:30:56.000000 pynabi-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1084 2023-06-30 18:51:30.000000 pynabi-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 18:52:21.183422 pynabi-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 18:52:21.154502 pynabi-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 18:52:21.176444 pynabi-0.1.1/src/pynabi/
+-rw-rw-rw-   0        0        0       47 2023-06-30 16:56:26.000000 pynabi-0.1.1/src/pynabi/__init__.py
+-rw-rw-rw-   0        0        0     6042 2023-06-30 18:35:33.000000 pynabi-0.1.1/src/pynabi/_common.py
+-rw-rw-rw-   0        0        0     9151 2023-06-30 18:45:35.000000 pynabi-0.1.1/src/pynabi/_dataset.py
+-rw-rw-rw-   0        0        0     4204 2023-06-17 21:06:56.000000 pynabi-0.1.1/src/pynabi/calculation.py
+-rw-rw-rw-   0        0        0     9529 2023-06-17 21:28:04.000000 pynabi-0.1.1/src/pynabi/crystal.py
+-rw-rw-rw-   0        0        0    11672 2023-06-30 17:18:06.000000 pynabi-0.1.1/src/pynabi/kspace.py
+-rw-rw-rw-   0        0        0     7844 2023-06-21 21:36:17.000000 pynabi-0.1.1/src/pynabi/occupation.py
+-rw-rw-rw-   0        0        0    14540 2023-06-17 19:55:26.000000 pynabi-0.1.1/src/pynabi/relaxation.py
+-rw-rw-rw-   0        0        0     3727 2023-06-17 21:24:10.000000 pynabi-0.1.1/src/pynabi/units.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:52:21.181456 pynabi-0.1.1/src/pynabi.egg-info/
+-rw-rw-rw-   0        0        0     8272 2023-06-30 18:52:21.000000 pynabi-0.1.1/src/pynabi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-30 18:52:21.000000 pynabi-0.1.1/src/pynabi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 18:52:21.000000 pynabi-0.1.1/src/pynabi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 18:52:21.000000 pynabi-0.1.1/src/pynabi.egg-info/top_level.txt
```

### Comparing `pynabi-0.1.0/LICENSE` & `pynabi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynabi-0.1.0/PKG-INFO` & `pynabi-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynabi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to easily create Abinit input files
 Author: Federico Guglielmi
 License: MIT License
         
         Copyright (c) 2023 Federico Guglielmi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 License-File: LICENSE
 
 # PynAbi
 
 Python package to easily create [Abinit](https://www.abinit.org/) input files.
 
 ```cmd
-pip install pynabi==0.0.3
+pip install pynabi
 ```
 
 ## Example
 
 ```python
 from pynabi import createAbi, DataSet, AbIn, AbOut
 from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
```

### Comparing `pynabi-0.1.0/README.md` & `pynabi-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PynAbi
 
 Python package to easily create [Abinit](https://www.abinit.org/) input files.
 
 ```cmd
-pip install pynabi==0.0.3
+pip install pynabi
 ```
 
 ## Example
 
 ```python
 from pynabi import createAbi, DataSet, AbIn, AbOut
 from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
```

### Comparing `pynabi-0.1.0/pyproject.toml` & `pynabi-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pynabi"
-version = "0.1.0"
+version = "0.1.1"
 description = "A package to easily create Abinit input files"
 keywords = [ "abinit" ]
 license = { file = "LICENSE" }
 readme = "README.md"
 authors = [
   { name="Federico Guglielmi" }
 ]
```

### Comparing `pynabi-0.1.0/src/pynabi/_common.py` & `pynabi-0.1.1/src/pynabi/_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,17 +129,17 @@
         self.i = index
         self.d = cls._delayables[index]
         self.v = self.d.sanitize(value)
     
     def compatible(self, coll: StampCollection):
         v = coll.get(self.c)
         if v is None:
-            raise TypeError(f"{self.d.name} definition requires {self.c.__name__} definition before")
-        if not v._doesDelay(self.i) and coll.nextto(self.c):
-            raise ValueError(f"{self.c.__name__} already defines {self.d.name} in the same dataset")
+            raise TypeError(f"{self.d.name} definition requires also a {self.c.__name__} definition in the base or current dataset")
+        if coll.nextto(self.c):
+            assert v._doesDelay(self.i), f"Adjacent {self.c.__name__} does not delay {self.d.name}"
     
     def stamp(self, index: int):
         return self.d.stamp(index or '', self.v)
 
 
 def delayer(index: int, T: Type, use: Type[Delayed] = Delayed):
     @classmethod
```

### Comparing `pynabi-0.1.0/src/pynabi/_dataset.py` & `pynabi-0.1.1/src/pynabi/_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Union, List, Iterable, Literal, Callable, Optional, Type
+from typing import Union, List, Iterable, Literal, Callable, Optional, Type, TypeVar
 from ._common import Stampable, Singleton, Delayed, StampCollection
 from .crystal import AtomBasis, Atom
 from inspect import stack
 
 from .occupation import _exclusives as _ex1
 from .calculation import _exclusives as _ex2
 from .kspace import _exclusives as _ex3
 
 _excl = [_ex1, _ex2, _ex3]
 
 
-__all__ = ["DataSet", "PreviousRun", "AbIn", "AbOut", "createAbi"]
+__all__ = ["DataSet", "PreviousRun", "AbIn", "AbOut", "createAbi", "append"]
 
 
 _RS = Union[Stampable,Iterable['_RS']]
 
 
 def splat(i: Iterable[_RS]) -> Iterable[Stampable]:
     for v in i:
@@ -29,47 +29,55 @@
 
 class DataSet:
     def __init__(self, *stampables: _RS) -> None:
         self.index = 0
         self.atoms: Union[AtomBasis,None] = None
         self.stamps: list[Stampable] = []
         self.map: dict[Type[Stampable], Stampable] = {}
-        delayed_props = set()
+        self.delayeds = set()
+        self._append(stampables)
+            
+    def _append(self, *stampables: _RS):
         for s in splat(stampables):
             if not isinstance(s, Stampable):
                 raise TypeError(f"{s.__class__.__name__} is not a valid type for a dataset")
             if isinstance(s, Delayed):
                 p = s.d.prop
-                if p in delayed_props:
+                if p in self.delayeds:
                     raise ValueError(f"Multiple {s.d.name} definition are present")
-                delayed_props.add(p)
+                self.delayeds.add(p)
                 self.stamps.append(s)
             else:
                 t = type(s)
                 if t in self.map:
                     raise ValueError(f"Multiple {s.__class__.__name__} given")
                 self.map[t] = s
                 if t is AtomBasis:
                     self.atoms = s # type: ignore
                 else:
                     self.stamps.append(s) # type: ignore
         s = set(self.map.keys())
         for excl in _excl:
             inters = s.intersection(excl)
             if len(inters) > 1:
-                raise ValueError(', '.join(c.__name__ for c in inters) + " are mutually incompatible: please specify only one of them")   
-
+                raise ValueError(', '.join(c.__name__ for c in inters) + " are mutually incompatible: please specify only one of them") 
     
     def stamp(self, atompool: List[Atom]):
         res: list[str] = []
         if self.atoms is not None:
             res.append(self.atoms.stamp(self.index, atompool))
         for s in self.stamps:
             res.append(s.stamp(self.index))
         return '\n'.join(res)
+    
+T = TypeVar("T", bound=Iterable[DataSet])
+def append(what: _RS, to: T) -> T:
+    for d in to:
+        d._append(what)
+    return to
 
 
 class PreviousRun(Singleton):
     pass
 
 
 def _AbInMethod(prop: str, sel: Literal[0,1,2] = 0):
```

### Comparing `pynabi-0.1.0/src/pynabi/calculation.py` & `pynabi-0.1.1/src/pynabi/calculation.py`

 * *Files identical despite different names*

### Comparing `pynabi-0.1.0/src/pynabi/crystal.py` & `pynabi-0.1.1/src/pynabi/crystal.py`

 * *Files identical despite different names*

### Comparing `pynabi-0.1.0/src/pynabi/kspace.py` & `pynabi-0.1.1/src/pynabi/kspace.py`

 * *Files identical despite different names*

### Comparing `pynabi-0.1.0/src/pynabi/occupation.py` & `pynabi-0.1.1/src/pynabi/occupation.py`

 * *Files identical despite different names*

### Comparing `pynabi-0.1.0/src/pynabi/relaxation.py` & `pynabi-0.1.1/src/pynabi/relaxation.py`

 * *Files identical despite different names*

### Comparing `pynabi-0.1.0/src/pynabi/units.py` & `pynabi-0.1.1/src/pynabi/units.py`

 * *Files identical despite different names*

### Comparing `pynabi-0.1.0/src/pynabi.egg-info/PKG-INFO` & `pynabi-0.1.1/src/pynabi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynabi
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to easily create Abinit input files
 Author: Federico Guglielmi
 License: MIT License
         
         Copyright (c) 2023 Federico Guglielmi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 License-File: LICENSE
 
 # PynAbi
 
 Python package to easily create [Abinit](https://www.abinit.org/) input files.
 
 ```cmd
-pip install pynabi==0.0.3
+pip install pynabi
 ```
 
 ## Example
 
 ```python
 from pynabi import createAbi, DataSet, AbIn, AbOut
 from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
```

