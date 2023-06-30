# Comparing `tmp/bridgestan-2.1.0.tar.gz` & `tmp/bridgestan-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgestan-2.1.0.tar", last modified: Thu Jun 29 16:08:39 2023, max compression
+gzip compressed data, was "bridgestan-2.1.1.tar", last modified: Fri Jun 30 18:36:30 2023, max compression
```

## Comparing `bridgestan-2.1.0.tar` & `bridgestan-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:38.996098 bridgestan-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-29 16:08:38.996098 bridgestan-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-29 16:06:07.000000 bridgestan-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:38.992098 bridgestan-2.1.0/bridgestan/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 16:08:01.000000 bridgestan-2.1.0/bridgestan/__version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:38.996098 bridgestan-2.1.0/bridgestan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 16:06:07.000000 bridgestan-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 16:08:38.996098 bridgestan-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 16:06:07.000000 bridgestan-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:38.996098 bridgestan-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-29 16:06:07.000000 bridgestan-2.1.0/test/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-29 16:06:07.000000 bridgestan-2.1.0/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    25485 2023-06-29 16:06:07.000000 bridgestan-2.1.0/test/test_stanmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:30.481672 bridgestan-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-30 18:36:30.485672 bridgestan-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 18:33:56.000000 bridgestan-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:30.481672 bridgestan-2.1.1/bridgestan/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 18:35:45.000000 bridgestan-2.1.1/bridgestan/__version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25859 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-30 18:33:56.000000 bridgestan-2.1.1/bridgestan/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:30.481672 bridgestan-2.1.1/bridgestan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 18:36:30.000000 bridgestan-2.1.1/bridgestan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 18:33:56.000000 bridgestan-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-30 18:36:30.485672 bridgestan-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 18:33:56.000000 bridgestan-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:36:30.481672 bridgestan-2.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 18:33:56.000000 bridgestan-2.1.1/test/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 18:33:56.000000 bridgestan-2.1.1/test/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25485 2023-06-30 18:33:56.000000 bridgestan-2.1.1/test/test_stanmodel.py
```

### Comparing `bridgestan-2.1.0/PKG-INFO` & `bridgestan-2.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 2.1.0
+Version: 2.1.1
 Home-page: https://github.com/roualdes/bridgestan
 Author: Brian Ward, Edward Roualdes, Bob Carpenter
 License: BSD 3-Clause License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bridgestan.py - The Python interface to BridgeStan
```

### Comparing `bridgestan-2.1.0/bridgestan/download.py` & `bridgestan-2.1.1/bridgestan/download.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.1.0/bridgestan/model.py` & `bridgestan-2.1.1/bridgestan/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Optional, Tuple
 
 import numpy as np
 import numpy.typing as npt
 from numpy.ctypeslib import ndpointer
 
 from .__version import __version_info__
-from .compile import compile_model
+from .compile import windows_dll_path_setup, compile_model
 from .util import validate_readable
 
 FloatArray = npt.NDArray[np.float64]
 double_array = ndpointer(dtype=ctypes.c_double, flags=("C_CONTIGUOUS"))
 star_star_char = ctypes.POINTER(ctypes.c_char_p)
 c_print_callback = ctypes.CFUNCTYPE(None, ctypes.POINTER(ctypes.c_char), ctypes.c_int)
 
@@ -63,14 +63,15 @@
         """
         validate_readable(model_lib)
         if model_data is not None and model_data.endswith(".json"):
             validate_readable(model_data)
             with open(model_data, "r") as f:
                 model_data = f.read()
 
+        windows_dll_path_setup()
         self.lib_path = model_lib
         self.stanlib = ctypes.CDLL(self.lib_path)
 
         self.data = model_data or ""
         self.seed = seed
 
         self._construct = self.stanlib.bs_model_construct
```

### Comparing `bridgestan-2.1.0/bridgestan.egg-info/PKG-INFO` & `bridgestan-2.1.1/bridgestan.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 2.1.0
+Version: 2.1.1
 Home-page: https://github.com/roualdes/bridgestan
 Author: Brian Ward, Edward Roualdes, Bob Carpenter
 License: BSD 3-Clause License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bridgestan.py - The Python interface to BridgeStan
```

### Comparing `bridgestan-2.1.0/test/test_compile.py` & `bridgestan-2.1.1/test/test_compile.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.1.0/test/test_stanmodel.py` & `bridgestan-2.1.1/test/test_stanmodel.py`

 * *Files identical despite different names*

