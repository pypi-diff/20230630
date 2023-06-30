# Comparing `tmp/absl_extra-0.0.2.dev2.tar.gz` & `tmp/absl_extra-0.0.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.2.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.2.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.2.dev2.tar` & `absl_extra-0.0.2.dev3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1588 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/Readme.md
--rw-r--r--   0        0        0      694 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/absl_extra/__init__.py
--rw-r--r--   0        0        0       64 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/absl_extra/py.typed
--rw-r--r--   0        0        0        0 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/absl_extra/src/__init__.py
--rw-r--r--   0        0        0     2061 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/absl_extra/src/logging_utils.py
--rw-r--r--   0        0        0     2487 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/absl_extra/src/notifier.py
--rw-r--r--   0        0        0     4175 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/absl_extra/src/tasks.py
--rw-r--r--   0        0        0     4522 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/absl_extra/src/tf_utils.py
--rw-r--r--   0        0        0      880 2023-06-30 18:05:39.759076 absl_extra-0.0.2.dev2/pyproject.toml
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1588 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/Readme.md
+-rw-r--r--   0        0        0      694 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/absl_extra/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/absl_extra/py.typed
+-rw-r--r--   0        0        0        0 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/absl_extra/src/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/absl_extra/src/logging_utils.py
+-rw-r--r--   0        0        0     2487 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/absl_extra/src/notifier.py
+-rw-r--r--   0        0        0     4179 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/absl_extra/src/tasks.py
+-rw-r--r--   0        0        0     4522 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/absl_extra/src/tf_utils.py
+-rw-r--r--   0        0        0      880 2023-06-30 18:10:12.848501 absl_extra-0.0.2.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev3/PKG-INFO
```

### Comparing `absl_extra-0.0.2.dev2/Readme.md` & `absl_extra-0.0.2.dev3/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev2/absl_extra/__init__.py` & `absl_extra-0.0.2.dev3/absl_extra/__init__.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev2/absl_extra/src/logging_utils.py` & `absl_extra-0.0.2.dev3/absl_extra/src/logging_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev2/absl_extra/src/notifier.py` & `absl_extra-0.0.2.dev3/absl_extra/src/notifier.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev2/absl_extra/src/tasks.py` & `absl_extra-0.0.2.dev3/absl_extra/src/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 from functools import wraps
 from importlib import util
 from typing import Callable, NamedTuple, TypeVar, Mapping, List
 
 from absl import app, flags, logging
 
-from absl_extra.notifier import BaseNotifier
+from absl_extra.src.notifier import BaseNotifier
 
 T = TypeVar("T", bound=Callable, covariant=True)
 FLAGS = flags.FLAGS
 
 if util.find_spec("pymongo"):
     from pymongo import MongoClient
     from pymongo.collection import Collection
```

### Comparing `absl_extra-0.0.2.dev2/absl_extra/src/tf_utils.py` & `absl_extra-0.0.2.dev3/absl_extra/src/tf_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev2/pyproject.toml` & `absl_extra-0.0.2.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.2dev2"
+version = "0.0.2dev3"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.2.dev2/PKG-INFO` & `absl_extra-0.0.2.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.2.dev2
+Version: 0.0.2.dev3
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

