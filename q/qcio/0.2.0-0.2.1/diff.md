# Comparing `tmp/qcio-0.2.0.tar.gz` & `tmp/qcio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.2.0.tar", max compression
+gzip compressed data, was "qcio-0.2.1.tar", max compression
```

## Comparing `qcio-0.2.0.tar` & `qcio-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1079 2023-06-30 02:24:48.614779 qcio-0.2.0/LICENSE
--rw-r--r--   0        0        0      898 2023-06-30 02:24:48.614779 qcio-0.2.0/README.md
--rw-r--r--   0        0        0     1246 2023-06-30 02:24:48.618779 qcio-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      560 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/__init__.py
--rw-r--r--   0        0        0       89 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/constants.py
--rw-r--r--   0        0        0      346 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/helper_types.py
--rw-r--r--   0        0        0     3671 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/mixins.py
--rw-r--r--   0        0        0      151 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/models/__init__.py
--rw-r--r--   0        0        0     8112 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/models/base_io.py
--rw-r--r--   0        0        0     4486 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/models/base_model.py
--rw-r--r--   0        0        0     3350 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/models/file.py
--rw-r--r--   0        0        0     7534 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/models/molecule.py
--rw-r--r--   0        0        0    12500 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/models/single_point.py
--rw-r--r--   0        0        0      190 2023-06-30 02:24:48.618779 qcio-0.2.0/qcio/utils.py
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 qcio-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-30 03:01:39.044386 qcio-0.2.1/LICENSE
+-rw-r--r--   0        0        0      898 2023-06-30 03:01:39.044386 qcio-0.2.1/README.md
+-rw-r--r--   0        0        0     1246 2023-06-30 03:01:39.044386 qcio-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/__init__.py
+-rw-r--r--   0        0        0       89 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/constants.py
+-rw-r--r--   0        0        0      346 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/helper_types.py
+-rw-r--r--   0        0        0     3671 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/mixins.py
+-rw-r--r--   0        0        0      151 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/__init__.py
+-rw-r--r--   0        0        0     8112 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/base_io.py
+-rw-r--r--   0        0        0     4447 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/base_model.py
+-rw-r--r--   0        0        0     3350 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/file.py
+-rw-r--r--   0        0        0     7534 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/molecule.py
+-rw-r--r--   0        0        0    12500 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/single_point.py
+-rw-r--r--   0        0        0      190 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/utils.py
+-rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 qcio-0.2.1/PKG-INFO
```

### Comparing `qcio-0.2.0/LICENSE` & `qcio-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.2.0/README.md` & `qcio-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.2.0/pyproject.toml` & `qcio-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.2.0"
+version = "0.2.1"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `qcio-0.2.0/qcio/__init__.py` & `qcio-0.2.1/qcio/__init__.py`

 * *Files identical despite different names*

### Comparing `qcio-0.2.0/qcio/mixins.py` & `qcio-0.2.1/qcio/mixins.py`

 * *Files identical despite different names*

### Comparing `qcio-0.2.0/qcio/models/base_io.py` & `qcio-0.2.1/qcio/models/base_io.py`

 * *Files identical despite different names*

### Comparing `qcio-0.2.0/qcio/models/base_model.py` & `qcio-0.2.1/qcio/models/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
         Properly serialize numpy arrays. Serialization is performed in .dict() so that
         multiple string serializers can used it without duplicating logic
         (e.g. json, yaml, toml).
         """
         model_dict = super().dict(**kwargs)
         to_pop = []
-        print(self.__class__.__name__)
         for key, value in model_dict.items():
             # Custom serialization for numpy arrays, enums, and pathlib Paths
             if isinstance(value, np.ndarray):
                 model_dict[key] = value.tolist()
             elif issubclass(type(value), Enum):
                 model_dict[key] = value.value
             elif isinstance(value, Path):
```

### Comparing `qcio-0.2.0/qcio/models/file.py` & `qcio-0.2.1/qcio/models/file.py`

 * *Files identical despite different names*

### Comparing `qcio-0.2.0/qcio/models/molecule.py` & `qcio-0.2.1/qcio/models/molecule.py`

 * *Files identical despite different names*

### Comparing `qcio-0.2.0/qcio/models/single_point.py` & `qcio-0.2.1/qcio/models/single_point.py`

 * *Files identical despite different names*

### Comparing `qcio-0.2.0/PKG-INFO` & `qcio-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.2.0
+Version: 0.2.1
 Summary: Beautiful and user friendly data structures for quantum chemistry.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

