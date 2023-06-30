# Comparing `tmp/pymultithreading-0.2.3.tar.gz` & `tmp/pymultithreading-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultithreading-0.2.3.tar", last modified: Tue Jun 20 16:17:38 2023, max compression
+gzip compressed data, was "pymultithreading-0.2.4.tar", last modified: Fri Jun 30 19:54:18 2023, max compression
```

## Comparing `pymultithreading-0.2.3.tar` & `pymultithreading-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 16:17:38.619904 pymultithreading-0.2.3/
--rw-rw-rw-   0        0        0       98 2023-06-20 16:17:38.000000 pymultithreading-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2045 2023-06-20 16:17:38.619904 pymultithreading-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.2.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.3/build.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:17:38.609904 pymultithreading-0.2.3/multithreading/
--rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.3/multithreading/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.2.3/multithreading/base.py
--rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.2.3/multithreading/document.py
--rw-rw-rw-   0        0        0    12687 2023-06-20 16:17:10.000000 pymultithreading-0.2.3/multithreading/process.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:17:38.618933 pymultithreading-0.2.3/pymultithreading.egg-info/
--rw-rw-rw-   0        0        0     2045 2023-06-20 16:17:38.000000 pymultithreading-0.2.3/pymultithreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-06-20 16:17:38.000000 pymultithreading-0.2.3/pymultithreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 16:17:38.000000 pymultithreading-0.2.3/pymultithreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-20 16:17:38.000000 pymultithreading-0.2.3/pymultithreading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-20 16:17:38.000000 pymultithreading-0.2.3/pymultithreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-06-20 16:17:38.000000 pymultithreading-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 16:17:38.619904 pymultithreading-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1561 2023-06-20 16:17:30.000000 pymultithreading-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:54:18.176730 pymultithreading-0.2.4/
+-rw-rw-rw-   0        0        0       98 2023-06-30 19:54:17.000000 pymultithreading-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2045 2023-06-30 19:54:18.175728 pymultithreading-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.2.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.4/build.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:54:18.160728 pymultithreading-0.2.4/multithreading/
+-rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.4/multithreading/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.2.4/multithreading/base.py
+-rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.2.4/multithreading/document.py
+-rw-rw-rw-   0        0        0    11624 2023-06-30 18:20:08.000000 pymultithreading-0.2.4/multithreading/process.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:54:18.174727 pymultithreading-0.2.4/pymultithreading.egg-info/
+-rw-rw-rw-   0        0        0     2045 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-06-30 19:54:17.000000 pymultithreading-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 19:54:18.176730 pymultithreading-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-06-30 19:54:06.000000 pymultithreading-0.2.4/setup.py
```

### Comparing `pymultithreading-0.2.3/PKG-INFO` & `pymultithreading-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.2.3/README.md` & `pymultithreading-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.3/build.py` & `pymultithreading-0.2.4/build.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.3/multithreading/base.py` & `pymultithreading-0.2.4/multithreading/base.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.3/multithreading/process.py` & `pymultithreading-0.2.4/multithreading/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # process.py
 
 import datetime as dt
+from dataclasses import dataclass
 import threading
 import time
 from abc import ABCMeta
 from typing import (
-    Any, Optional, Dict, Callable,
+    Any, Optional, Dict, Callable, ClassVar,
     Iterable, Union, TypeVar, Generic
 )
 
 from represent import BaseModel, Modifiers
 
 __all__ = [
     "Caller",
@@ -20,36 +21,22 @@
     "wait_call_completion",
     "ProcessTime",
     "ProcessInfo",
     "find_caller",
     "CallResults"
 ]
 
+@dataclass(repr=False, slots=True)
 class ProcessInfo(BaseModel, metaclass=ABCMeta):
     """A class to contain the info of a call to the callers."""
 
-    modifiers = Modifiers(properties=True)
+    start: dt.datetime
+    end: dt.datetime
 
-    __slots__ = 'start', 'end'
-
-    def __init__(
-            self,
-            start: dt.datetime,
-            end: dt.datetime,
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param start: The starting time for the call.
-        :param end: The ending time for the call.
-        """
-
-        self.start = start
-        self.end = end
-    # end __init__
+    modifiers: ClassVar[Modifiers] = Modifiers(properties=['time'])
 
     @property
     def time(self) -> dt.timedelta:
         """
         Returns the time duration of the call.
 
         :return: The call time.
@@ -61,41 +48,26 @@
 
 class ProcessTime(ProcessInfo):
     """A class to contain the info of a call to the callers."""
 # end ProcessTime
 
 _ReturnType = TypeVar("_ReturnType")
 
+@dataclass(repr=False, slots=True)
 class CallResults(BaseModel, Generic[_ReturnType]):
     """A class to represent a container for the call results."""
 
-    modifiers = Modifiers(excluded=["thread"], force=True)
-
-    __slots__ = "returns", "thread", "start", "end"
-
-    def __init__(
-            self,
-            returns: Optional[_ReturnType] = None,
-            thread: Optional[threading.Thread] = None,
-            start: Optional[dt.datetime] = None,
-            end: Optional[dt.datetime] = None,
+    returns: Optional[_ReturnType] = None
+    thread: Optional[threading.Thread] = None
+    start: Optional[dt.datetime] = None
+    end: Optional[dt.datetime] = None
 
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param returns: The returned response.
-        """
-
-        self.start = start
-        self.end = end
-
-        self.returns = returns
-        self.thread = thread
-    # end __init__
+    modifiers: ClassVar[Modifiers] = Modifiers(
+        excluded=["thread"], force=True
+    )
 # end CallResults
 
 class Caller(BaseModel, Generic[_ReturnType]):
     """A class to represent a function caller object."""
 
     modifiers = Modifiers(excluded=["thread", "results"])
 
@@ -265,39 +237,22 @@
         self.wait = wait
         self.reset_before = reset_before
         self.reset_after = reset_after
         self.sleep = sleep
     # end __init__
 # end CallDefinition
 
+@dataclass(repr=False, slots=True)
 class CallsResults(BaseModel):
     """A class to contain the info of a call to the callers."""
 
-    __slots__ = "waiting", "callers", "definition", "total"
-
-    def __init__(
-            self,
-            callers: Dict[Caller, CallResults],
-            total: ProcessTime,
-            waiting: ProcessTime,
-            definition: CallDefinition
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param callers: The callers object.
-        :param total: The time object for the call.
-        :param definition: The call definition object.
-        """
-
-        self.callers = callers
-        self.definition = definition
-        self.total = total
-        self.waiting = waiting
-    # end __init__
+    callers: Dict[Caller, CallResults]
+    total: ProcessTime
+    waiting: ProcessTime
+    definition: CallDefinition
 
     def caller(self, identifier: Any) -> Caller:
         """
         Finds the caller object by its identifier
 
         :param identifier: The identifier of the caller to return.
```

### Comparing `pymultithreading-0.2.3/pymultithreading.egg-info/PKG-INFO` & `pymultithreading-0.2.4/pymultithreading.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.2.3/pyproject.toml` & `pymultithreading-0.2.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pymultithreading'
-version = '0.2.3'
+version = '0.2.4'
 description = 'A python module for creating multithreading processes easily, in a more Pythonic way.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pymultithreading-0.2.3/setup.py` & `pymultithreading-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pymultithreading',
-        version='0.2.3',
+        version='0.2.4',
         description=(
             "A python module for creating multithreading "
             "processes easily, in a more Pythonic way."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

