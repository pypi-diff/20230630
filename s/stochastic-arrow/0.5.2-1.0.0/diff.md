# Comparing `tmp/stochastic-arrow-0.5.2.tar.gz` & `tmp/stochastic-arrow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stochastic-arrow-0.5.2.tar", last modified: Sun Apr  9 23:12:42 2023, max compression
+gzip compressed data, was "stochastic-arrow-1.0.0.tar", last modified: Fri Jun 30 21:50:43 2023, max compression
```

## Comparing `stochastic-arrow-0.5.2.tar` & `stochastic-arrow-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2023-04-09 23:12:42.130754 stochastic-arrow-0.5.2/
--rw-r--r--   0 jerry      (501) staff       (20)     1050 2019-02-01 03:30:40.000000 stochastic-arrow-0.5.2/LICENSE
--rw-r--r--   0 jerry      (501) staff       (20)       49 2019-02-01 03:30:40.000000 stochastic-arrow-0.5.2/MANIFEST.in
--rw-r--r--   0 jerry      (501) staff       (20)     5127 2023-04-09 23:12:42.130521 stochastic-arrow-0.5.2/PKG-INFO
--rw-r--r--   0 jerry      (501) staff       (20)     4505 2023-04-09 23:11:36.000000 stochastic-arrow-0.5.2/README.md
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2023-04-09 23:12:42.128295 stochastic-arrow-0.5.2/arrow/
--rw-r--r--   0 jerry      (501) staff       (20)      210 2019-10-15 05:15:11.000000 stochastic-arrow-0.5.2/arrow/__init__.py
--rw-r--r--   0 jerry      (501) staff       (20)     7505 2021-10-29 22:16:30.000000 stochastic-arrow-0.5.2/arrow/arrow.py
--rw-r--r--   0 jerry      (501) staff       (20)   954204 2023-04-09 23:12:29.000000 stochastic-arrow-0.5.2/arrow/arrowhead.c
--rw-r--r--   0 jerry      (501) staff       (20)      850 2019-10-15 02:13:11.000000 stochastic-arrow-0.5.2/arrow/math.py
--rw-r--r--   0 jerry      (501) staff       (20)     4796 2019-02-03 01:44:00.000000 stochastic-arrow-0.5.2/arrow/mersenne.c
--rw-r--r--   0 jerry      (501) staff       (20)     1276 2019-02-02 00:02:03.000000 stochastic-arrow-0.5.2/arrow/mersenne.h
--rw-r--r--   0 jerry      (501) staff       (20)    13173 2021-12-21 22:47:26.000000 stochastic-arrow-0.5.2/arrow/obsidian.c
--rw-r--r--   0 jerry      (501) staff       (20)     1366 2021-10-29 22:16:30.000000 stochastic-arrow-0.5.2/arrow/obsidian.h
--rw-r--r--   0 jerry      (501) staff       (20)     6093 2020-03-05 05:31:48.000000 stochastic-arrow-0.5.2/arrow/reference.py
--rw-r--r--   0 jerry      (501) staff       (20)       38 2023-04-09 23:12:42.130829 stochastic-arrow-0.5.2/setup.cfg
--rw-r--r--   0 jerry      (501) staff       (20)     2365 2023-04-09 23:11:36.000000 stochastic-arrow-0.5.2/setup.py
-drwxr-xr-x   0 jerry      (501) staff       (20)        0 2023-04-09 23:12:42.130000 stochastic-arrow-0.5.2/stochastic_arrow.egg-info/
--rw-r--r--   0 jerry      (501) staff       (20)     5127 2023-04-09 23:12:42.000000 stochastic-arrow-0.5.2/stochastic_arrow.egg-info/PKG-INFO
--rw-r--r--   0 jerry      (501) staff       (20)      350 2023-04-09 23:12:42.000000 stochastic-arrow-0.5.2/stochastic_arrow.egg-info/SOURCES.txt
--rw-r--r--   0 jerry      (501) staff       (20)        1 2023-04-09 23:12:42.000000 stochastic-arrow-0.5.2/stochastic_arrow.egg-info/dependency_links.txt
--rw-r--r--   0 jerry      (501) staff       (20)        6 2023-04-09 23:12:42.000000 stochastic-arrow-0.5.2/stochastic_arrow.egg-info/top_level.txt
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2023-06-30 21:50:43.259472 stochastic-arrow-1.0.0/
+-rw-r--r--   0 jerry      (501) staff       (20)     1050 2019-02-01 03:30:40.000000 stochastic-arrow-1.0.0/LICENSE
+-rw-r--r--   0 jerry      (501) staff       (20)       71 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/MANIFEST.in
+-rw-r--r--   0 jerry      (501) staff       (20)     5797 2023-06-30 21:50:43.259144 stochastic-arrow-1.0.0/PKG-INFO
+-rw-r--r--   0 jerry      (501) staff       (20)     5163 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/README.md
+-rw-r--r--   0 jerry      (501) staff       (20)       38 2023-06-30 21:50:43.259580 stochastic-arrow-1.0.0/setup.cfg
+-rw-r--r--   0 jerry      (501) staff       (20)     2538 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/setup.py
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2023-06-30 21:50:43.256928 stochastic-arrow-1.0.0/stochastic_arrow/
+-rw-r--r--   0 jerry      (501) staff       (20)      210 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/stochastic_arrow/__init__.py
+-rw-r--r--   0 jerry      (501) staff       (20)     7554 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/stochastic_arrow/arrow.py
+-rw-r--r--   0 jerry      (501) staff       (20)   959117 2023-06-30 21:47:14.000000 stochastic-arrow-1.0.0/stochastic_arrow/arrowhead.c
+-rw-r--r--   0 jerry      (501) staff       (20)      850 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/stochastic_arrow/math.py
+-rw-r--r--   0 jerry      (501) staff       (20)     4796 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/stochastic_arrow/mersenne.c
+-rw-r--r--   0 jerry      (501) staff       (20)     1276 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/stochastic_arrow/mersenne.h
+-rw-r--r--   0 jerry      (501) staff       (20)    13230 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/stochastic_arrow/obsidian.c
+-rw-r--r--   0 jerry      (501) staff       (20)     1366 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/stochastic_arrow/obsidian.h
+-rw-r--r--   0 jerry      (501) staff       (20)     6104 2023-06-30 21:40:29.000000 stochastic-arrow-1.0.0/stochastic_arrow/reference.py
+drwxr-xr-x   0 jerry      (501) staff       (20)        0 2023-06-30 21:50:43.258494 stochastic-arrow-1.0.0/stochastic_arrow.egg-info/
+-rw-r--r--   0 jerry      (501) staff       (20)     5797 2023-06-30 21:50:43.000000 stochastic-arrow-1.0.0/stochastic_arrow.egg-info/PKG-INFO
+-rw-r--r--   0 jerry      (501) staff       (20)      449 2023-06-30 21:50:43.000000 stochastic-arrow-1.0.0/stochastic_arrow.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry      (501) staff       (20)        1 2023-06-30 21:50:43.000000 stochastic-arrow-1.0.0/stochastic_arrow.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry      (501) staff       (20)       17 2023-06-30 21:50:43.000000 stochastic-arrow-1.0.0/stochastic_arrow.egg-info/top_level.txt
```

### Comparing `stochastic-arrow-0.5.2/LICENSE` & `stochastic-arrow-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stochastic-arrow-0.5.2/PKG-INFO` & `stochastic-arrow-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: stochastic-arrow
-Version: 0.5.2
+Version: 1.0.0
 Home-page: https://github.com/CovertLab/arrow
-Author: Ryan Spangler, John Mason, Jerry Morrison, Chris Skalnik, Travis Ahn-Horst
+Author: Ryan Spangler, John Mason, Jerry Morrison, Chris Skalnik, Travis Ahn-Horst, Sean Cheah
 Author-email: ryan.spangler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -35,22 +35,29 @@
 ## Installation
 
 Add the following to your `requirements.txt`, or run
 `pip install stochastic-arrow` to install it [from PyPI](https://pypi.org/project/stochastic-arrow/):
 
     stochastic-arrow
 
+**NOTE:** If upgrading from a version older than 1.0.0, check if the [`arrow`](https://github.com/arrow-py/arrow) datetime package is installed. If so, uninstall `arrow` before upgrading `stochastic-arrow`, then reinstall `arrow`.
+
+    > pip show arrow
+    > pip uninstall arrow
+    > pip install stochastic-arrow
+    > pip install arrow
+
 ## Usage
 
-The `arrow` library presents a single class as an interface,
+The `stochastic_arrow` library presents a single class as an interface,
 `StochasticSystem`, which operates on a set of reactions (encoded as a `numpy`
 matrix of stoichiometrix coefficients) and associated reaction rates:
 
 ```python
-from arrow import StochasticSystem
+from stochastic_arrow import StochasticSystem
 import numpy as np
 
 # Each row is a reaction and each column is a molecular species (or other
 # entity). The first reaction here means that the first and second elements
 # combine to create the third, while the fourth is unaffected.
 stoichiometric_matrix = np.array([
     [1, 1, -1, 0],
@@ -93,50 +100,54 @@
 ```
 
 If you are interested in the history of states for plotting or otherwise, these can be
 derived from the list of events and the stoichiometric matrix, along with the inital
 state. `reenact_events` will do this for you:
 
 ```python
-from arrow import reenact_events
+from stochastic_arrow import reenact_events
 
-history = reenact_events(stoichiometry, result['events'], state)
+history = reenact_events(stoichiometric_matrix, result['events'], state)
 ```
 
 ## Testing
 
-`arrow` uses [pytest](https://docs.pytest.org/en/latest/). To test it:
+`stochastic_arrow` uses [pytest](https://docs.pytest.org/en/latest/). To test it:
 
     > make clean compile
     > pytest
 
 **NOTE:** `make compile` without an explicit `clean` might not fully build the extension.
 
 There are more command line features in test_arrow:
 
-    > python -m arrow.test.test_arrow --complexation
+    > python -m stochastic_arrow.test.test_arrow --complexation
 
-    > python -m arrow.test.test_arrow --plot
+    > python -m stochastic_arrow.test.test_arrow --plot
 
-    > python -m arrow.test.test_arrow --obsidian
+    > python -m stochastic_arrow.test.test_arrow --obsidian
 
-    > python -m arrow.test.test_arrow --memory
+    > python -m stochastic_arrow.test.test_arrow --memory
 
-    > python -m arrow.test.test_arrow --time
+    > python -m stochastic_arrow.test.test_arrow --time
 
 More examples:
 
-    > python -m arrow.test.test_hang
+    > python -m stochastic_arrow.test.test_hang
 
-    > pytest -m arrow/test/test_arrow.py
+    > pytest -m stochastic_arrow/test/test_arrow.py
 
     > pytest -k flagella
 
 ## Changelog
 
+### Version 1.0.0
+
+* Rename module to `stochastic_arrow` to avoid name conflict (Issue #51). **All users must update their import statements to use `stochastic_arrow` instead of `arrow`.**
+
 ### Version 0.5.2
 
 * Update to Cython 0.29.34. (Cython 3.0.0 is now in beta.)
 
 ### Version 0.5.1
 
 * Update to Cython 3.0.0a11 for compatibility with Python 3.11.
```

### Comparing `stochastic-arrow-0.5.2/README.md` & `stochastic-arrow-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -17,22 +17,29 @@
 ## Installation
 
 Add the following to your `requirements.txt`, or run
 `pip install stochastic-arrow` to install it [from PyPI](https://pypi.org/project/stochastic-arrow/):
 
     stochastic-arrow
 
+**NOTE:** If upgrading from a version older than 1.0.0, check if the [`arrow`](https://github.com/arrow-py/arrow) datetime package is installed. If so, uninstall `arrow` before upgrading `stochastic-arrow`, then reinstall `arrow`.
+
+    > pip show arrow
+    > pip uninstall arrow
+    > pip install stochastic-arrow
+    > pip install arrow
+
 ## Usage
 
-The `arrow` library presents a single class as an interface,
+The `stochastic_arrow` library presents a single class as an interface,
 `StochasticSystem`, which operates on a set of reactions (encoded as a `numpy`
 matrix of stoichiometrix coefficients) and associated reaction rates:
 
 ```python
-from arrow import StochasticSystem
+from stochastic_arrow import StochasticSystem
 import numpy as np
 
 # Each row is a reaction and each column is a molecular species (or other
 # entity). The first reaction here means that the first and second elements
 # combine to create the third, while the fourth is unaffected.
 stoichiometric_matrix = np.array([
     [1, 1, -1, 0],
@@ -75,50 +82,54 @@
 ```
 
 If you are interested in the history of states for plotting or otherwise, these can be
 derived from the list of events and the stoichiometric matrix, along with the inital
 state. `reenact_events` will do this for you:
 
 ```python
-from arrow import reenact_events
+from stochastic_arrow import reenact_events
 
-history = reenact_events(stoichiometry, result['events'], state)
+history = reenact_events(stoichiometric_matrix, result['events'], state)
 ```
 
 ## Testing
 
-`arrow` uses [pytest](https://docs.pytest.org/en/latest/). To test it:
+`stochastic_arrow` uses [pytest](https://docs.pytest.org/en/latest/). To test it:
 
     > make clean compile
     > pytest
 
 **NOTE:** `make compile` without an explicit `clean` might not fully build the extension.
 
 There are more command line features in test_arrow:
 
-    > python -m arrow.test.test_arrow --complexation
+    > python -m stochastic_arrow.test.test_arrow --complexation
 
-    > python -m arrow.test.test_arrow --plot
+    > python -m stochastic_arrow.test.test_arrow --plot
 
-    > python -m arrow.test.test_arrow --obsidian
+    > python -m stochastic_arrow.test.test_arrow --obsidian
 
-    > python -m arrow.test.test_arrow --memory
+    > python -m stochastic_arrow.test.test_arrow --memory
 
-    > python -m arrow.test.test_arrow --time
+    > python -m stochastic_arrow.test.test_arrow --time
 
 More examples:
 
-    > python -m arrow.test.test_hang
+    > python -m stochastic_arrow.test.test_hang
 
-    > pytest -m arrow/test/test_arrow.py
+    > pytest -m stochastic_arrow/test/test_arrow.py
 
     > pytest -k flagella
 
 ## Changelog
 
+### Version 1.0.0
+
+* Rename module to `stochastic_arrow` to avoid name conflict (Issue #51). **All users must update their import statements to use `stochastic_arrow` instead of `arrow`.**
+
 ### Version 0.5.2
 
 * Update to Cython 0.29.34. (Cython 3.0.0 is now in beta.)
 
 ### Version 0.5.1
 
 * Update to Cython 3.0.0a11 for compatibility with Python 3.11.
```

### Comparing `stochastic-arrow-0.5.2/arrow/arrow.py` & `stochastic-arrow-1.0.0/stochastic_arrow/arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         flat: The flattened data.
         lengths: The lengths of all the given sublists.
         indexes: The indexes where the sublists begin in the flat array.
     '''
 
     lengths = np.array([
         len(l)
-        for l in assorted_lists])
-    indexes = np.insert(lengths, 0, 0).cumsum()[:-1]
-    flat = np.array(flatten(assorted_lists))
+        for l in assorted_lists], dtype=np.int64)
+    indexes = np.insert(lengths, 0, 0).cumsum()[:-1].astype(np.int64)
+    flat = np.array(flatten(assorted_lists), dtype=np.int64)
     return flat, lengths, indexes
 
 def reenact_events(stoichiometry, events, state):
     '''
     Reproduce the history of states given an initial state, the history of events and
     the stoichiometry of those events.
```

### Comparing `stochastic-arrow-0.5.2/arrow/arrowhead.c` & `stochastic-arrow-1.0.0/stochastic_arrow/arrowhead.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -13,39 +13,39 @@
             "/usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
             "/usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
             "/usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
             "/usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
             "/usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "arrow",
+            "stochastic_arrow",
             "/usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/core/include"
         ],
-        "name": "arrow.arrowhead",
+        "name": "stochastic_arrow.arrowhead",
         "sources": [
-            "arrow/arrowhead.pyx",
-            "arrow/mersenne.c",
-            "arrow/obsidian.c"
+            "stochastic_arrow/arrowhead.pyx",
+            "stochastic_arrow/mersenne.c",
+            "stochastic_arrow/obsidian.c"
         ]
     },
-    "module_name": "arrow.arrowhead"
+    "module_name": "stochastic_arrow.arrowhead"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -105,16 +105,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -765,16 +769,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__arrow__arrowhead
-#define __PYX_HAVE_API__arrow__arrowhead
+#define __PYX_HAVE__stochastic_arrow__arrowhead
+#define __PYX_HAVE_API__stochastic_arrow__arrowhead
 /* Early includes */
 #include <stdint.h>
 #include <string.h>
 #include <stdlib.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
@@ -1015,15 +1019,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "arrow/arrowhead.pyx",
+  "stochastic_arrow/arrowhead.pyx",
   "stringsource",
   "__init__.pxd",
   "type.pxd",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
@@ -1125,195 +1129,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":718
- * 
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":716
  * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1339,64 +1325,64 @@
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
-struct __pyx_obj_5arrow_9arrowhead_Arrowhead;
+struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "arrow/arrowhead.pyx":21
+/* "stochastic_arrow/arrowhead.pyx":21
  * 
  * 
  * cdef class Arrowhead:             # <<<<<<<<<<<<<<
  *     """Cython interface to the C-coded Gillespie algorithm "obsidian", leaving
  *     obsidian.c free of Python dependencies.
  */
-struct __pyx_obj_5arrow_9arrowhead_Arrowhead {
+struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead {
   PyObject_HEAD
   int random_seed;
   Info info;
   PyObject *refs;
 };
 
 
@@ -1688,14 +1674,19 @@
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -2033,30 +2024,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -2348,36 +2339,36 @@
 static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void); /*proto*/
 
-/* Module declarations from 'arrow' */
+/* Module declarations from 'stochastic_arrow' */
 
-/* Module declarations from 'arrow.mersenne' */
+/* Module declarations from 'stochastic_arrow.mersenne' */
 
 /* Module declarations from 'mersenne' */
 
-/* Module declarations from 'arrow.obsidian' */
+/* Module declarations from 'stochastic_arrow.obsidian' */
 
-/* Module declarations from 'arrow.arrowhead' */
-static PyTypeObject *__pyx_ptype_5arrow_9arrowhead_Arrowhead = 0;
+/* Module declarations from 'stochastic_arrow.arrowhead' */
+static PyTypeObject *__pyx_ptype_16stochastic_arrow_9arrowhead_Arrowhead = 0;
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
 static PyTypeObject *__pyx_memoryview_type = 0;
 static PyTypeObject *__pyx_memoryviewslice_type = 0;
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
-static PyArrayObject *__pyx_f_5arrow_9arrowhead_copy_c_array(void *, npy_intp, size_t, int); /*proto*/
+static PyArrayObject *__pyx_f_16stochastic_arrow_9arrowhead_copy_c_array(void *, npy_intp, size_t, int); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static void *__pyx_align_pointer(void *, size_t); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static PyObject *assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
 static struct __pyx_memoryview_obj *__pyx_memview_slice(struct __pyx_memoryview_obj *, PyObject *); /*proto*/
@@ -2406,19 +2397,19 @@
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn_int64_t = { "int64_t", NULL, sizeof(int64_t), { 0 }, 0, IS_UNSIGNED(int64_t) ? 'U' : 'I', IS_UNSIGNED(int64_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn_uint32_t = { "uint32_t", NULL, sizeof(uint32_t), { 0 }, 0, IS_UNSIGNED(uint32_t) ? 'U' : 'I', IS_UNSIGNED(uint32_t), 0 };
-#define __Pyx_MODULE_NAME "arrow.arrowhead"
-extern int __pyx_module_is_main_arrow__arrowhead;
-int __pyx_module_is_main_arrow__arrowhead = 0;
+#define __Pyx_MODULE_NAME "stochastic_arrow.arrowhead"
+extern int __pyx_module_is_main_stochastic_arrow__arrowhead;
+int __pyx_module_is_main_stochastic_arrow__arrowhead = 0;
 
-/* Implementation of 'arrow.arrowhead' */
+/* Implementation of 'stochastic_arrow.arrowhead' */
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_Ellipsis;
@@ -2638,24 +2629,24 @@
 static PyObject *__pyx_n_s_substrates_indexes;
 static PyObject *__pyx_n_s_substrates_lengths;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
-static int __pyx_pf_5arrow_9arrowhead_9Arrowhead___cinit__(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_args); /* proto */
-static int __pyx_pf_5arrow_9arrowhead_9Arrowhead_2__init__(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, int __pyx_v_random_seed, __Pyx_memviewslice __pyx_v_stoichiometry, __Pyx_memviewslice __pyx_v_reactants_lengths, __Pyx_memviewslice __pyx_v_reactants_indexes, __Pyx_memviewslice __pyx_v_reactants, __Pyx_memviewslice __pyx_v_reactions, __Pyx_memviewslice __pyx_v_dependencies_lengths, __Pyx_memviewslice __pyx_v_dependencies_indexes, __Pyx_memviewslice __pyx_v_dependencies, __Pyx_memviewslice __pyx_v_substrates_lengths, __Pyx_memviewslice __pyx_v_substrates_indexes, __Pyx_memviewslice __pyx_v_substrates, CYTHON_UNUSED PyObject *__pyx_v_args); /* proto */
-static void __pyx_pf_5arrow_9arrowhead_9Arrowhead_4__dealloc__(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_6evolve(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, double __pyx_v_duration, __Pyx_memviewslice __pyx_v_state, __Pyx_memviewslice __pyx_v_rates); /* proto */
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_8reactions_count(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_10substrates_count(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_12get_random_state(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_14set_random_state(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, __Pyx_memviewslice __pyx_v_mt, __Pyx_memviewslice __pyx_v_mt_tempered, size_t __pyx_v_index); /* proto */
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead___cinit__(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_args); /* proto */
+static int __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_2__init__(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, int __pyx_v_random_seed, __Pyx_memviewslice __pyx_v_stoichiometry, __Pyx_memviewslice __pyx_v_reactants_lengths, __Pyx_memviewslice __pyx_v_reactants_indexes, __Pyx_memviewslice __pyx_v_reactants, __Pyx_memviewslice __pyx_v_reactions, __Pyx_memviewslice __pyx_v_dependencies_lengths, __Pyx_memviewslice __pyx_v_dependencies_indexes, __Pyx_memviewslice __pyx_v_dependencies, __Pyx_memviewslice __pyx_v_substrates_lengths, __Pyx_memviewslice __pyx_v_substrates_indexes, __Pyx_memviewslice __pyx_v_substrates, CYTHON_UNUSED PyObject *__pyx_v_args); /* proto */
+static void __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_4__dealloc__(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_6evolve(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, double __pyx_v_duration, __Pyx_memviewslice __pyx_v_state, __Pyx_memviewslice __pyx_v_rates); /* proto */
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_8reactions_count(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_10substrates_count(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_12get_random_state(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_14set_random_state(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, __Pyx_memviewslice __pyx_v_mt, __Pyx_memviewslice __pyx_v_mt_tempered, size_t __pyx_v_index); /* proto */
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2690,15 +2681,15 @@
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_5arrow_9arrowhead_Arrowhead(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_16stochastic_arrow_9arrowhead_Arrowhead(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_112105877;
@@ -2733,125 +2724,125 @@
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_codeobj__30;
 /* Late includes */
 
-/* "arrow/arrowhead.pyx":36
+/* "stochastic_arrow/arrowhead.pyx":36
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     def __cinit__(self, *args):             # <<<<<<<<<<<<<<
  *         memset(&self.info, 0, sizeof(obsidian.Info))
  *         self.info.random_state = <mersenne.MTState*> PyMem_Malloc(sizeof(mersenne.MTState))
  */
 
 /* Python wrapper */
-static int __pyx_pw_5arrow_9arrowhead_9Arrowhead_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_5arrow_9arrowhead_9Arrowhead_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_args = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
   __Pyx_INCREF(__pyx_args);
   __pyx_v_args = __pyx_args;
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead___cinit__(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self), __pyx_v_args);
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead___cinit__(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self), __pyx_v_args);
 
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_args);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_5arrow_9arrowhead_9Arrowhead___cinit__(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_args) {
+static int __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead___cinit__(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_args) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "arrow/arrowhead.pyx":37
+  /* "stochastic_arrow/arrowhead.pyx":37
  *     @cython.wraparound(False)
  *     def __cinit__(self, *args):
  *         memset(&self.info, 0, sizeof(obsidian.Info))             # <<<<<<<<<<<<<<
  *         self.info.random_state = <mersenne.MTState*> PyMem_Malloc(sizeof(mersenne.MTState))
  *         if not self.info.random_state:
  */
   (void)(memset((&__pyx_v_self->info), 0, (sizeof(Info))));
 
-  /* "arrow/arrowhead.pyx":38
+  /* "stochastic_arrow/arrowhead.pyx":38
  *     def __cinit__(self, *args):
  *         memset(&self.info, 0, sizeof(obsidian.Info))
  *         self.info.random_state = <mersenne.MTState*> PyMem_Malloc(sizeof(mersenne.MTState))             # <<<<<<<<<<<<<<
  *         if not self.info.random_state:
  *             raise MemoryError()
  */
   __pyx_v_self->info.random_state = ((MTState *)PyMem_Malloc((sizeof(MTState))));
 
-  /* "arrow/arrowhead.pyx":39
+  /* "stochastic_arrow/arrowhead.pyx":39
  *         memset(&self.info, 0, sizeof(obsidian.Info))
  *         self.info.random_state = <mersenne.MTState*> PyMem_Malloc(sizeof(mersenne.MTState))
  *         if not self.info.random_state:             # <<<<<<<<<<<<<<
  *             raise MemoryError()
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->info.random_state != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "arrow/arrowhead.pyx":40
+    /* "stochastic_arrow/arrowhead.pyx":40
  *         self.info.random_state = <mersenne.MTState*> PyMem_Malloc(sizeof(mersenne.MTState))
  *         if not self.info.random_state:
  *             raise MemoryError()             # <<<<<<<<<<<<<<
  * 
  *     # This will accept any type of array in C-contiguous layout that support
  */
     PyErr_NoMemory(); __PYX_ERR(0, 40, __pyx_L1_error)
 
-    /* "arrow/arrowhead.pyx":39
+    /* "stochastic_arrow/arrowhead.pyx":39
  *         memset(&self.info, 0, sizeof(obsidian.Info))
  *         self.info.random_state = <mersenne.MTState*> PyMem_Malloc(sizeof(mersenne.MTState))
  *         if not self.info.random_state:             # <<<<<<<<<<<<<<
  *             raise MemoryError()
  * 
  */
   }
 
-  /* "arrow/arrowhead.pyx":36
+  /* "stochastic_arrow/arrowhead.pyx":36
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     def __cinit__(self, *args):             # <<<<<<<<<<<<<<
  *         memset(&self.info, 0, sizeof(obsidian.Info))
  *         self.info.random_state = <mersenne.MTState*> PyMem_Malloc(sizeof(mersenne.MTState))
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "arrow/arrowhead.pyx":47
+/* "stochastic_arrow/arrowhead.pyx":47
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             int random_seed,
  */
 
 /* Python wrapper */
-static int __pyx_pw_5arrow_9arrowhead_9Arrowhead_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_5arrow_9arrowhead_9Arrowhead_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_random_seed;
   __Pyx_memviewslice __pyx_v_stoichiometry = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_reactants_lengths = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_reactants_indexes = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_reactants = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_reactions = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dependencies_lengths = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -3017,15 +3008,15 @@
     __pyx_v_substrates = __Pyx_PyObject_to_MemoryviewSlice_dc_nn_int64_t(values[11], PyBUF_WRITABLE); if (unlikely(!__pyx_v_substrates.memview)) __PYX_ERR(0, 63, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 0, 12, 12, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 47, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_stoichiometry.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "stoichiometry"); __PYX_ERR(0, 50, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_reactants_lengths.memview) == Py_None)) {
@@ -3054,27 +3045,27 @@
   }
   if (unlikely(((PyObject *)__pyx_v_substrates_indexes.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "substrates_indexes"); __PYX_ERR(0, 62, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_substrates.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "substrates"); __PYX_ERR(0, 63, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead_2__init__(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self), __pyx_v_random_seed, __pyx_v_stoichiometry, __pyx_v_reactants_lengths, __pyx_v_reactants_indexes, __pyx_v_reactants, __pyx_v_reactions, __pyx_v_dependencies_lengths, __pyx_v_dependencies_indexes, __pyx_v_dependencies, __pyx_v_substrates_lengths, __pyx_v_substrates_indexes, __pyx_v_substrates, __pyx_v_args);
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_2__init__(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self), __pyx_v_random_seed, __pyx_v_stoichiometry, __pyx_v_reactants_lengths, __pyx_v_reactants_indexes, __pyx_v_reactants, __pyx_v_reactions, __pyx_v_dependencies_lengths, __pyx_v_dependencies_indexes, __pyx_v_dependencies, __pyx_v_substrates_lengths, __pyx_v_substrates_indexes, __pyx_v_substrates, __pyx_v_args);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_args);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_5arrow_9arrowhead_9Arrowhead_2__init__(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, int __pyx_v_random_seed, __Pyx_memviewslice __pyx_v_stoichiometry, __Pyx_memviewslice __pyx_v_reactants_lengths, __Pyx_memviewslice __pyx_v_reactants_indexes, __Pyx_memviewslice __pyx_v_reactants, __Pyx_memviewslice __pyx_v_reactions, __Pyx_memviewslice __pyx_v_dependencies_lengths, __Pyx_memviewslice __pyx_v_dependencies_indexes, __Pyx_memviewslice __pyx_v_dependencies, __Pyx_memviewslice __pyx_v_substrates_lengths, __Pyx_memviewslice __pyx_v_substrates_indexes, __Pyx_memviewslice __pyx_v_substrates, CYTHON_UNUSED PyObject *__pyx_v_args) {
+static int __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_2__init__(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, int __pyx_v_random_seed, __Pyx_memviewslice __pyx_v_stoichiometry, __Pyx_memviewslice __pyx_v_reactants_lengths, __Pyx_memviewslice __pyx_v_reactants_indexes, __Pyx_memviewslice __pyx_v_reactants, __Pyx_memviewslice __pyx_v_reactions, __Pyx_memviewslice __pyx_v_dependencies_lengths, __Pyx_memviewslice __pyx_v_dependencies_indexes, __Pyx_memviewslice __pyx_v_dependencies, __Pyx_memviewslice __pyx_v_substrates_lengths, __Pyx_memviewslice __pyx_v_substrates_indexes, __Pyx_memviewslice __pyx_v_substrates, CYTHON_UNUSED PyObject *__pyx_v_args) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -3088,172 +3079,172 @@
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "arrow/arrowhead.pyx":65
+  /* "stochastic_arrow/arrowhead.pyx":65
  *             int64_t[::1] substrates not None,
  *             *args):
  *         self.random_seed = random_seed             # <<<<<<<<<<<<<<
  *         mersenne.seed(self.info.random_state, random_seed)
  * 
  */
   __pyx_v_self->random_seed = __pyx_v_random_seed;
 
-  /* "arrow/arrowhead.pyx":66
+  /* "stochastic_arrow/arrowhead.pyx":66
  *             *args):
  *         self.random_seed = random_seed
  *         mersenne.seed(self.info.random_state, random_seed)             # <<<<<<<<<<<<<<
  * 
- *         self.info.reactions_count = stoichiometry.shape[0]
+ *         self.info.reactions_count = <int>stoichiometry.shape[0]
  */
   seed(__pyx_v_self->info.random_state, __pyx_v_random_seed);
 
-  /* "arrow/arrowhead.pyx":68
+  /* "stochastic_arrow/arrowhead.pyx":68
  *         mersenne.seed(self.info.random_state, random_seed)
  * 
- *         self.info.reactions_count = stoichiometry.shape[0]             # <<<<<<<<<<<<<<
- *         self.info.substrates_count = stoichiometry.shape[1]
+ *         self.info.reactions_count = <int>stoichiometry.shape[0]             # <<<<<<<<<<<<<<
+ *         self.info.substrates_count = <int>stoichiometry.shape[1]
  *         self.info.stoichiometry = &stoichiometry[0, 0]
  */
-  __pyx_v_self->info.reactions_count = (__pyx_v_stoichiometry.shape[0]);
+  __pyx_v_self->info.reactions_count = ((int)(__pyx_v_stoichiometry.shape[0]));
 
-  /* "arrow/arrowhead.pyx":69
+  /* "stochastic_arrow/arrowhead.pyx":69
  * 
- *         self.info.reactions_count = stoichiometry.shape[0]
- *         self.info.substrates_count = stoichiometry.shape[1]             # <<<<<<<<<<<<<<
+ *         self.info.reactions_count = <int>stoichiometry.shape[0]
+ *         self.info.substrates_count = <int>stoichiometry.shape[1]             # <<<<<<<<<<<<<<
  *         self.info.stoichiometry = &stoichiometry[0, 0]
  * 
  */
-  __pyx_v_self->info.substrates_count = (__pyx_v_stoichiometry.shape[1]);
+  __pyx_v_self->info.substrates_count = ((int)(__pyx_v_stoichiometry.shape[1]));
 
-  /* "arrow/arrowhead.pyx":70
- *         self.info.reactions_count = stoichiometry.shape[0]
- *         self.info.substrates_count = stoichiometry.shape[1]
+  /* "stochastic_arrow/arrowhead.pyx":70
+ *         self.info.reactions_count = <int>stoichiometry.shape[0]
+ *         self.info.substrates_count = <int>stoichiometry.shape[1]
  *         self.info.stoichiometry = &stoichiometry[0, 0]             # <<<<<<<<<<<<<<
  * 
  *         self.info.reactants_lengths = &reactants_lengths[0]
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_self->info.stoichiometry = (&(*((int64_t *) ( /* dim=1 */ ((char *) (((int64_t *) ( /* dim=0 */ (__pyx_v_stoichiometry.data + __pyx_t_1 * __pyx_v_stoichiometry.strides[0]) )) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":72
+  /* "stochastic_arrow/arrowhead.pyx":72
  *         self.info.stoichiometry = &stoichiometry[0, 0]
  * 
  *         self.info.reactants_lengths = &reactants_lengths[0]             # <<<<<<<<<<<<<<
  *         self.info.reactants_indexes = &reactants_indexes[0]
  *         self.info.reactants = &reactants[0]
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.reactants_lengths = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_reactants_lengths.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":73
+  /* "stochastic_arrow/arrowhead.pyx":73
  * 
  *         self.info.reactants_lengths = &reactants_lengths[0]
  *         self.info.reactants_indexes = &reactants_indexes[0]             # <<<<<<<<<<<<<<
  *         self.info.reactants = &reactants[0]
  *         self.info.reactions = &reactions[0]
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.reactants_indexes = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_reactants_indexes.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":74
+  /* "stochastic_arrow/arrowhead.pyx":74
  *         self.info.reactants_lengths = &reactants_lengths[0]
  *         self.info.reactants_indexes = &reactants_indexes[0]
  *         self.info.reactants = &reactants[0]             # <<<<<<<<<<<<<<
  *         self.info.reactions = &reactions[0]
  * 
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.reactants = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_reactants.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":75
+  /* "stochastic_arrow/arrowhead.pyx":75
  *         self.info.reactants_indexes = &reactants_indexes[0]
  *         self.info.reactants = &reactants[0]
  *         self.info.reactions = &reactions[0]             # <<<<<<<<<<<<<<
  * 
  *         self.info.dependencies_lengths = &dependencies_lengths[0]
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.reactions = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_reactions.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":77
+  /* "stochastic_arrow/arrowhead.pyx":77
  *         self.info.reactions = &reactions[0]
  * 
  *         self.info.dependencies_lengths = &dependencies_lengths[0]             # <<<<<<<<<<<<<<
  *         self.info.dependencies_indexes = &dependencies_indexes[0]
  *         self.info.dependencies = &dependencies[0]
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.dependencies_lengths = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_dependencies_lengths.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":78
+  /* "stochastic_arrow/arrowhead.pyx":78
  * 
  *         self.info.dependencies_lengths = &dependencies_lengths[0]
  *         self.info.dependencies_indexes = &dependencies_indexes[0]             # <<<<<<<<<<<<<<
  *         self.info.dependencies = &dependencies[0]
  * 
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.dependencies_indexes = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_dependencies_indexes.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":79
+  /* "stochastic_arrow/arrowhead.pyx":79
  *         self.info.dependencies_lengths = &dependencies_lengths[0]
  *         self.info.dependencies_indexes = &dependencies_indexes[0]
  *         self.info.dependencies = &dependencies[0]             # <<<<<<<<<<<<<<
  * 
  *         self.info.substrates_lengths = &substrates_lengths[0]
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.dependencies = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_dependencies.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":81
+  /* "stochastic_arrow/arrowhead.pyx":81
  *         self.info.dependencies = &dependencies[0]
  * 
  *         self.info.substrates_lengths = &substrates_lengths[0]             # <<<<<<<<<<<<<<
  *         self.info.substrates_indexes = &substrates_indexes[0]
  *         self.info.substrates = &substrates[0]
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.substrates_lengths = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_substrates_lengths.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":82
+  /* "stochastic_arrow/arrowhead.pyx":82
  * 
  *         self.info.substrates_lengths = &substrates_lengths[0]
  *         self.info.substrates_indexes = &substrates_indexes[0]             # <<<<<<<<<<<<<<
  *         self.info.substrates = &substrates[0]
  * 
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.substrates_indexes = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_substrates_indexes.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":83
+  /* "stochastic_arrow/arrowhead.pyx":83
  *         self.info.substrates_lengths = &substrates_lengths[0]
  *         self.info.substrates_indexes = &substrates_indexes[0]
  *         self.info.substrates = &substrates[0]             # <<<<<<<<<<<<<<
  * 
  *         # TODO(jerry): Check array sizes? E.g. rates.shape[0] >= reactions_count
  */
   __pyx_t_2 = 0;
   __pyx_v_self->info.substrates = (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_substrates.data) + __pyx_t_2)) ))));
 
-  /* "arrow/arrowhead.pyx":88
+  /* "stochastic_arrow/arrowhead.pyx":88
  * 
  *         self.refs = (  # hold refs to these memoryviews while we hold their data ptrs
  *             stoichiometry,             # <<<<<<<<<<<<<<
  *             reactants_lengths, reactants_indexes, reactants, reactions,
  *             dependencies_lengths, dependencies_indexes, dependencies,
  */
   __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_stoichiometry, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "arrow/arrowhead.pyx":89
+  /* "stochastic_arrow/arrowhead.pyx":89
  *         self.refs = (  # hold refs to these memoryviews while we hold their data ptrs
  *             stoichiometry,
  *             reactants_lengths, reactants_indexes, reactants, reactions,             # <<<<<<<<<<<<<<
  *             dependencies_lengths, dependencies_indexes, dependencies,
  *             substrates_lengths, substrates_indexes, substrates)
  */
   __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_reactants_lengths, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
@@ -3261,43 +3252,43 @@
   __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_v_reactants_indexes, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_reactants, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = __pyx_memoryview_fromslice(__pyx_v_reactions, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "arrow/arrowhead.pyx":90
+  /* "stochastic_arrow/arrowhead.pyx":90
  *             stoichiometry,
  *             reactants_lengths, reactants_indexes, reactants, reactions,
  *             dependencies_lengths, dependencies_indexes, dependencies,             # <<<<<<<<<<<<<<
  *             substrates_lengths, substrates_indexes, substrates)
  * 
  */
   __pyx_t_8 = __pyx_memoryview_fromslice(__pyx_v_dependencies_lengths, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_dependencies_indexes, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_10 = __pyx_memoryview_fromslice(__pyx_v_dependencies, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
 
-  /* "arrow/arrowhead.pyx":91
+  /* "stochastic_arrow/arrowhead.pyx":91
  *             reactants_lengths, reactants_indexes, reactants, reactions,
  *             dependencies_lengths, dependencies_indexes, dependencies,
  *             substrates_lengths, substrates_indexes, substrates)             # <<<<<<<<<<<<<<
  * 
  *     # `self` might no longer be a valid Python object so *BE CAREFUL* invoking
  */
   __pyx_t_11 = __pyx_memoryview_fromslice(__pyx_v_substrates_lengths, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __pyx_t_12 = __pyx_memoryview_fromslice(__pyx_v_substrates_indexes, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __pyx_t_13 = __pyx_memoryview_fromslice(__pyx_v_substrates, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_int64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn_int64_t, 0);; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
 
-  /* "arrow/arrowhead.pyx":88
+  /* "stochastic_arrow/arrowhead.pyx":88
  * 
  *         self.refs = (  # hold refs to these memoryviews while we hold their data ptrs
  *             stoichiometry,             # <<<<<<<<<<<<<<
  *             reactants_lengths, reactants_indexes, reactants, reactions,
  *             dependencies_lengths, dependencies_indexes, dependencies,
  */
   __pyx_t_14 = PyTuple_New(11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 88, __pyx_L1_error)
@@ -3332,28 +3323,28 @@
   __pyx_t_8 = 0;
   __pyx_t_9 = 0;
   __pyx_t_10 = 0;
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
 
-  /* "arrow/arrowhead.pyx":87
+  /* "stochastic_arrow/arrowhead.pyx":87
  *         # TODO(jerry): Check array sizes? E.g. rates.shape[0] >= reactions_count
  * 
  *         self.refs = (  # hold refs to these memoryviews while we hold their data ptrs             # <<<<<<<<<<<<<<
  *             stoichiometry,
  *             reactants_lengths, reactants_indexes, reactants, reactions,
  */
   __Pyx_GIVEREF(__pyx_t_14);
   __Pyx_GOTREF(__pyx_v_self->refs);
   __Pyx_DECREF(__pyx_v_self->refs);
   __pyx_v_self->refs = ((PyObject*)__pyx_t_14);
   __pyx_t_14 = 0;
 
-  /* "arrow/arrowhead.pyx":47
+  /* "stochastic_arrow/arrowhead.pyx":47
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             int random_seed,
  */
 
@@ -3369,15 +3360,15 @@
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_stoichiometry, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_reactants_lengths, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_reactants_indexes, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_reactants, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_reactions, 1);
@@ -3387,70 +3378,70 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_substrates_lengths, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_substrates_indexes, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_substrates, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "arrow/arrowhead.pyx":95
+/* "stochastic_arrow/arrowhead.pyx":95
  *     # `self` might no longer be a valid Python object so *BE CAREFUL* invoking
  *     # Python operations that might touch it!
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         PyMem_Free(self.info.random_state)
  * 
  */
 
 /* Python wrapper */
-static void __pyx_pw_5arrow_9arrowhead_9Arrowhead_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_5arrow_9arrowhead_9Arrowhead_5__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_5__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_5arrow_9arrowhead_9Arrowhead_4__dealloc__(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self));
+  __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_4__dealloc__(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_5arrow_9arrowhead_9Arrowhead_4__dealloc__(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self) {
+static void __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_4__dealloc__(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "arrow/arrowhead.pyx":96
+  /* "stochastic_arrow/arrowhead.pyx":96
  *     # Python operations that might touch it!
  *     def __dealloc__(self):
  *         PyMem_Free(self.info.random_state)             # <<<<<<<<<<<<<<
  * 
  *     @cython.boundscheck(False)
  */
   PyMem_Free(__pyx_v_self->info.random_state);
 
-  /* "arrow/arrowhead.pyx":95
+  /* "stochastic_arrow/arrowhead.pyx":95
  *     # `self` might no longer be a valid Python object so *BE CAREFUL* invoking
  *     # Python operations that might touch it!
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         PyMem_Free(self.info.random_state)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "arrow/arrowhead.pyx":100
+/* "stochastic_arrow/arrowhead.pyx":100
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     def evolve(self, double duration, int64_t[::1] state, double[::1] rates):             # <<<<<<<<<<<<<<
  *         """Run the Gillespie algorithm with the initialized stoichiometry and
  *         rates over the given duration and state.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_7evolve(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_5arrow_9arrowhead_9Arrowhead_6evolve[] = "Run the Gillespie algorithm with the initialized stoichiometry and\n        rates over the given duration and state.\n        Return None or a tuple (status, steps, time, events, outcome).\n        ";
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_7evolve(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_7evolve(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_16stochastic_arrow_9arrowhead_9Arrowhead_6evolve[] = "Run the Gillespie algorithm with the initialized stoichiometry and\n        rates over the given duration and state.\n        Return None or a tuple (status, steps, time, events, outcome).\n        ";
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_7evolve(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   double __pyx_v_duration;
   __Pyx_memviewslice __pyx_v_state = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_rates = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -3504,26 +3495,26 @@
     __pyx_v_state = __Pyx_PyObject_to_MemoryviewSlice_dc_nn_int64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_state.memview)) __PYX_ERR(0, 100, __pyx_L3_error)
     __pyx_v_rates = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_rates.memview)) __PYX_ERR(0, 100, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("evolve", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 100, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.evolve", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.evolve", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead_6evolve(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self), __pyx_v_duration, __pyx_v_state, __pyx_v_rates);
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_6evolve(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self), __pyx_v_duration, __pyx_v_state, __pyx_v_rates);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_6evolve(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, double __pyx_v_duration, __Pyx_memviewslice __pyx_v_state, __Pyx_memviewslice __pyx_v_rates) {
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_6evolve(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, double __pyx_v_duration, __Pyx_memviewslice __pyx_v_state, __Pyx_memviewslice __pyx_v_rates) {
   evolve_result __pyx_v_evolved;
   int __pyx_v_status;
   int __pyx_v_steps;
   int __pyx_v_count;
   PyArrayObject *__pyx_v_time = NULL;
   PyArrayObject *__pyx_v_events = NULL;
   PyArrayObject *__pyx_v_outcome = NULL;
@@ -3538,122 +3529,122 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("evolve", 0);
 
-  /* "arrow/arrowhead.pyx":107
+  /* "stochastic_arrow/arrowhead.pyx":107
  *         # TODO(jerry): Check the state[] array size?
  * 
  *         evolved = obsidian.evolve(&self.info, duration, &state[0], &rates[0])             # <<<<<<<<<<<<<<
  *         cdef int status = evolved.status
  *         cdef int steps = evolved.steps
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_evolved = evolve((&__pyx_v_self->info), __pyx_v_duration, (&(*((int64_t *) ( /* dim=0 */ ((char *) (((int64_t *) __pyx_v_state.data) + __pyx_t_1)) )))), (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_rates.data) + __pyx_t_2)) )))));
 
-  /* "arrow/arrowhead.pyx":108
+  /* "stochastic_arrow/arrowhead.pyx":108
  * 
  *         evolved = obsidian.evolve(&self.info, duration, &state[0], &rates[0])
  *         cdef int status = evolved.status             # <<<<<<<<<<<<<<
  *         cdef int steps = evolved.steps
  *         cdef int count = self.info.substrates_count
  */
   __pyx_t_3 = __pyx_v_evolved.status;
   __pyx_v_status = __pyx_t_3;
 
-  /* "arrow/arrowhead.pyx":109
+  /* "stochastic_arrow/arrowhead.pyx":109
  *         evolved = obsidian.evolve(&self.info, duration, &state[0], &rates[0])
  *         cdef int status = evolved.status
  *         cdef int steps = evolved.steps             # <<<<<<<<<<<<<<
  *         cdef int count = self.info.substrates_count
  * 
  */
   __pyx_t_3 = __pyx_v_evolved.steps;
   __pyx_v_steps = __pyx_t_3;
 
-  /* "arrow/arrowhead.pyx":110
+  /* "stochastic_arrow/arrowhead.pyx":110
  *         cdef int status = evolved.status
  *         cdef int steps = evolved.steps
  *         cdef int count = self.info.substrates_count             # <<<<<<<<<<<<<<
  * 
  *         if steps == -1:
  */
   __pyx_t_3 = __pyx_v_self->info.substrates_count;
   __pyx_v_count = __pyx_t_3;
 
-  /* "arrow/arrowhead.pyx":112
+  /* "stochastic_arrow/arrowhead.pyx":112
  *         cdef int count = self.info.substrates_count
  * 
  *         if steps == -1:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
   __pyx_t_4 = ((__pyx_v_steps == -1L) != 0);
   if (__pyx_t_4) {
 
-    /* "arrow/arrowhead.pyx":113
+    /* "stochastic_arrow/arrowhead.pyx":113
  * 
  *         if steps == -1:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         time = copy_c_array(evolved.time, steps, sizeof(double), np.NPY_DOUBLE)
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "arrow/arrowhead.pyx":112
+    /* "stochastic_arrow/arrowhead.pyx":112
  *         cdef int count = self.info.substrates_count
  * 
  *         if steps == -1:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
   }
 
-  /* "arrow/arrowhead.pyx":115
+  /* "stochastic_arrow/arrowhead.pyx":115
  *             return None
  * 
  *         time = copy_c_array(evolved.time, steps, sizeof(double), np.NPY_DOUBLE)             # <<<<<<<<<<<<<<
  *         events = copy_c_array(evolved.events, steps, sizeof(int64_t), np.NPY_INT64)
  *         outcome = copy_c_array(evolved.outcome, count, sizeof(int64_t), np.NPY_INT64)
  */
-  __pyx_t_5 = ((PyObject *)__pyx_f_5arrow_9arrowhead_copy_c_array(__pyx_v_evolved.time, __pyx_v_steps, (sizeof(double)), NPY_DOUBLE)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_5 = ((PyObject *)__pyx_f_16stochastic_arrow_9arrowhead_copy_c_array(__pyx_v_evolved.time, __pyx_v_steps, (sizeof(double)), NPY_DOUBLE)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_v_time = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "arrow/arrowhead.pyx":116
+  /* "stochastic_arrow/arrowhead.pyx":116
  * 
  *         time = copy_c_array(evolved.time, steps, sizeof(double), np.NPY_DOUBLE)
  *         events = copy_c_array(evolved.events, steps, sizeof(int64_t), np.NPY_INT64)             # <<<<<<<<<<<<<<
  *         outcome = copy_c_array(evolved.outcome, count, sizeof(int64_t), np.NPY_INT64)
  * 
  */
-  __pyx_t_5 = ((PyObject *)__pyx_f_5arrow_9arrowhead_copy_c_array(__pyx_v_evolved.events, __pyx_v_steps, (sizeof(int64_t)), NPY_INT64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_5 = ((PyObject *)__pyx_f_16stochastic_arrow_9arrowhead_copy_c_array(__pyx_v_evolved.events, __pyx_v_steps, (sizeof(int64_t)), NPY_INT64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_v_events = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "arrow/arrowhead.pyx":117
+  /* "stochastic_arrow/arrowhead.pyx":117
  *         time = copy_c_array(evolved.time, steps, sizeof(double), np.NPY_DOUBLE)
  *         events = copy_c_array(evolved.events, steps, sizeof(int64_t), np.NPY_INT64)
  *         outcome = copy_c_array(evolved.outcome, count, sizeof(int64_t), np.NPY_INT64)             # <<<<<<<<<<<<<<
  * 
  *         result = status, steps, time, events, outcome
  */
-  __pyx_t_5 = ((PyObject *)__pyx_f_5arrow_9arrowhead_copy_c_array(__pyx_v_evolved.outcome, __pyx_v_count, (sizeof(int64_t)), NPY_INT64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_5 = ((PyObject *)__pyx_f_16stochastic_arrow_9arrowhead_copy_c_array(__pyx_v_evolved.outcome, __pyx_v_count, (sizeof(int64_t)), NPY_INT64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_v_outcome = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "arrow/arrowhead.pyx":119
+  /* "stochastic_arrow/arrowhead.pyx":119
  *         outcome = copy_c_array(evolved.outcome, count, sizeof(int64_t), np.NPY_INT64)
  * 
  *         result = status, steps, time, events, outcome             # <<<<<<<<<<<<<<
  * 
  *         free(evolved.time)
  */
   __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
@@ -3676,289 +3667,289 @@
   __Pyx_GIVEREF(((PyObject *)__pyx_v_outcome));
   PyTuple_SET_ITEM(__pyx_t_7, 4, ((PyObject *)__pyx_v_outcome));
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_v_result = ((PyObject*)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "arrow/arrowhead.pyx":121
+  /* "stochastic_arrow/arrowhead.pyx":121
  *         result = status, steps, time, events, outcome
  * 
  *         free(evolved.time)             # <<<<<<<<<<<<<<
  *         free(evolved.events)
  *         free(evolved.outcome)
  */
   free(__pyx_v_evolved.time);
 
-  /* "arrow/arrowhead.pyx":122
+  /* "stochastic_arrow/arrowhead.pyx":122
  * 
  *         free(evolved.time)
  *         free(evolved.events)             # <<<<<<<<<<<<<<
  *         free(evolved.outcome)
  * 
  */
   free(__pyx_v_evolved.events);
 
-  /* "arrow/arrowhead.pyx":123
+  /* "stochastic_arrow/arrowhead.pyx":123
  *         free(evolved.time)
  *         free(evolved.events)
  *         free(evolved.outcome)             # <<<<<<<<<<<<<<
  * 
  *         return result
  */
   free(__pyx_v_evolved.outcome);
 
-  /* "arrow/arrowhead.pyx":125
+  /* "stochastic_arrow/arrowhead.pyx":125
  *         free(evolved.outcome)
  * 
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     def reactions_count(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "arrow/arrowhead.pyx":100
+  /* "stochastic_arrow/arrowhead.pyx":100
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     def evolve(self, double duration, int64_t[::1] state, double[::1] rates):             # <<<<<<<<<<<<<<
  *         """Run the Gillespie algorithm with the initialized stoichiometry and
  *         rates over the given duration and state.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.evolve", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.evolve", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_time);
   __Pyx_XDECREF((PyObject *)__pyx_v_events);
   __Pyx_XDECREF((PyObject *)__pyx_v_outcome);
   __Pyx_XDECREF(__pyx_v_result);
   __PYX_XDEC_MEMVIEW(&__pyx_v_state, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_rates, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "arrow/arrowhead.pyx":127
+/* "stochastic_arrow/arrowhead.pyx":127
  *         return result
  * 
  *     def reactions_count(self):             # <<<<<<<<<<<<<<
  *         """Returns the number of reactions for this system."""
  *         return self.info.reactions_count
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_9reactions_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_5arrow_9arrowhead_9Arrowhead_8reactions_count[] = "Returns the number of reactions for this system.";
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_9reactions_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_9reactions_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_16stochastic_arrow_9arrowhead_9Arrowhead_8reactions_count[] = "Returns the number of reactions for this system.";
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_9reactions_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("reactions_count (wrapper)", 0);
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead_8reactions_count(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self));
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_8reactions_count(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_8reactions_count(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self) {
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_8reactions_count(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reactions_count", 0);
 
-  /* "arrow/arrowhead.pyx":129
+  /* "stochastic_arrow/arrowhead.pyx":129
  *     def reactions_count(self):
  *         """Returns the number of reactions for this system."""
  *         return self.info.reactions_count             # <<<<<<<<<<<<<<
  * 
  *     def substrates_count(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->info.reactions_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "arrow/arrowhead.pyx":127
+  /* "stochastic_arrow/arrowhead.pyx":127
  *         return result
  * 
  *     def reactions_count(self):             # <<<<<<<<<<<<<<
  *         """Returns the number of reactions for this system."""
  *         return self.info.reactions_count
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.reactions_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.reactions_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "arrow/arrowhead.pyx":131
+/* "stochastic_arrow/arrowhead.pyx":131
  *         return self.info.reactions_count
  * 
  *     def substrates_count(self):             # <<<<<<<<<<<<<<
  *         """Returns the number of substrates this system operates on."""
  *         return self.info.substrates_count
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_11substrates_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_5arrow_9arrowhead_9Arrowhead_10substrates_count[] = "Returns the number of substrates this system operates on.";
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_11substrates_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_11substrates_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_16stochastic_arrow_9arrowhead_9Arrowhead_10substrates_count[] = "Returns the number of substrates this system operates on.";
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_11substrates_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("substrates_count (wrapper)", 0);
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead_10substrates_count(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self));
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_10substrates_count(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_10substrates_count(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self) {
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_10substrates_count(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("substrates_count", 0);
 
-  /* "arrow/arrowhead.pyx":133
+  /* "stochastic_arrow/arrowhead.pyx":133
  *     def substrates_count(self):
  *         """Returns the number of substrates this system operates on."""
  *         return self.info.substrates_count             # <<<<<<<<<<<<<<
  * 
  *     def get_random_state(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->info.substrates_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "arrow/arrowhead.pyx":131
+  /* "stochastic_arrow/arrowhead.pyx":131
  *         return self.info.reactions_count
  * 
  *     def substrates_count(self):             # <<<<<<<<<<<<<<
  *         """Returns the number of substrates this system operates on."""
  *         return self.info.substrates_count
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.substrates_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.substrates_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "arrow/arrowhead.pyx":135
+/* "stochastic_arrow/arrowhead.pyx":135
  *         return self.info.substrates_count
  * 
  *     def get_random_state(self):             # <<<<<<<<<<<<<<
  *         """Returns the state of the pseudorandom number generator."""
  *         cdef mersenne.MTState state
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_13get_random_state(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_5arrow_9arrowhead_9Arrowhead_12get_random_state[] = "Returns the state of the pseudorandom number generator.";
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_13get_random_state(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_13get_random_state(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_16stochastic_arrow_9arrowhead_9Arrowhead_12get_random_state[] = "Returns the state of the pseudorandom number generator.";
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_13get_random_state(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_random_state (wrapper)", 0);
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead_12get_random_state(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self));
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_12get_random_state(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_12get_random_state(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self) {
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_12get_random_state(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self) {
   MTState __pyx_v_state;
   PyArrayObject *__pyx_v_mt = NULL;
   PyArrayObject *__pyx_v_mt_tempered = NULL;
   size_t __pyx_v_index;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   size_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_random_state", 0);
 
-  /* "arrow/arrowhead.pyx":138
+  /* "stochastic_arrow/arrowhead.pyx":138
  *         """Returns the state of the pseudorandom number generator."""
  *         cdef mersenne.MTState state
  *         obsidian.get_random_state(&self.info, &state)             # <<<<<<<<<<<<<<
  * 
  *         mt = copy_c_array(
  */
   get_random_state((&__pyx_v_self->info), (&__pyx_v_state));
 
-  /* "arrow/arrowhead.pyx":140
+  /* "stochastic_arrow/arrowhead.pyx":140
  *         obsidian.get_random_state(&self.info, &state)
  * 
  *         mt = copy_c_array(             # <<<<<<<<<<<<<<
  *             &state.MT[0], mersenne.TWISTER_SIZE, sizeof(uint32_t),
  *             np.NPY_UINT32)
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_5arrow_9arrowhead_copy_c_array((&(__pyx_v_state.MT[0])), TWISTER_SIZE, (sizeof(uint32_t)), NPY_UINT32)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_16stochastic_arrow_9arrowhead_copy_c_array((&(__pyx_v_state.MT[0])), TWISTER_SIZE, (sizeof(uint32_t)), NPY_UINT32)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_mt = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "arrow/arrowhead.pyx":143
+  /* "stochastic_arrow/arrowhead.pyx":143
  *             &state.MT[0], mersenne.TWISTER_SIZE, sizeof(uint32_t),
  *             np.NPY_UINT32)
  *         mt_tempered = copy_c_array(             # <<<<<<<<<<<<<<
  *             &state.MT_TEMPERED[0], mersenne.TWISTER_SIZE, sizeof(uint32_t),
  *             np.NPY_UINT32)
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_5arrow_9arrowhead_copy_c_array((&(__pyx_v_state.MT_TEMPERED[0])), TWISTER_SIZE, (sizeof(uint32_t)), NPY_UINT32)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_16stochastic_arrow_9arrowhead_copy_c_array((&(__pyx_v_state.MT_TEMPERED[0])), TWISTER_SIZE, (sizeof(uint32_t)), NPY_UINT32)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_mt_tempered = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "arrow/arrowhead.pyx":146
+  /* "stochastic_arrow/arrowhead.pyx":146
  *             &state.MT_TEMPERED[0], mersenne.TWISTER_SIZE, sizeof(uint32_t),
  *             np.NPY_UINT32)
  *         index = state.index             # <<<<<<<<<<<<<<
  * 
  *         return mt, mt_tempered, index
  */
   __pyx_t_2 = __pyx_v_state.index;
   __pyx_v_index = __pyx_t_2;
 
-  /* "arrow/arrowhead.pyx":148
+  /* "stochastic_arrow/arrowhead.pyx":148
  *         index = state.index
  * 
  *         return mt, mt_tempered, index             # <<<<<<<<<<<<<<
  * 
  *     def set_random_state(
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3975,47 +3966,47 @@
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "arrow/arrowhead.pyx":135
+  /* "stochastic_arrow/arrowhead.pyx":135
  *         return self.info.substrates_count
  * 
  *     def get_random_state(self):             # <<<<<<<<<<<<<<
  *         """Returns the state of the pseudorandom number generator."""
  *         cdef mersenne.MTState state
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.get_random_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.get_random_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_mt);
   __Pyx_XDECREF((PyObject *)__pyx_v_mt_tempered);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "arrow/arrowhead.pyx":150
+/* "stochastic_arrow/arrowhead.pyx":150
  *         return mt, mt_tempered, index
  * 
  *     def set_random_state(             # <<<<<<<<<<<<<<
  *             self, uint32_t[::1] mt, uint32_t[::1] mt_tempered,
  *             size_t index):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_15set_random_state(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_15set_random_state(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_15set_random_state(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_15set_random_state(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_mt = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_mt_tempered = { 0, 0, { 0 }, { 0 }, { 0 } };
   size_t __pyx_v_index;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -4069,37 +4060,37 @@
     __pyx_v_mt_tempered = __Pyx_PyObject_to_MemoryviewSlice_dc_nn_uint32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_mt_tempered.memview)) __PYX_ERR(0, 151, __pyx_L3_error)
     __pyx_v_index = __Pyx_PyInt_As_size_t(values[2]); if (unlikely((__pyx_v_index == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 152, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("set_random_state", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 150, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.set_random_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.set_random_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead_14set_random_state(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self), __pyx_v_mt, __pyx_v_mt_tempered, __pyx_v_index);
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_14set_random_state(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self), __pyx_v_mt, __pyx_v_mt_tempered, __pyx_v_index);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_14set_random_state(struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, __Pyx_memviewslice __pyx_v_mt, __Pyx_memviewslice __pyx_v_mt_tempered, size_t __pyx_v_index) {
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_14set_random_state(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, __Pyx_memviewslice __pyx_v_mt, __Pyx_memviewslice __pyx_v_mt_tempered, size_t __pyx_v_index) {
   MTState __pyx_v_state;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_random_state", 0);
 
-  /* "arrow/arrowhead.pyx":154
+  /* "stochastic_arrow/arrowhead.pyx":154
  *             size_t index):
  *         cdef mersenne.MTState state
  *         memcpy(&state.MT[0], &mt[0], sizeof(state.MT))             # <<<<<<<<<<<<<<
  *         memcpy(
  *             &state.MT_TEMPERED[0], &mt_tempered[0],
  */
   __pyx_t_1 = 0;
@@ -4110,15 +4101,15 @@
   } else if (unlikely(__pyx_t_1 >= __pyx_v_mt.shape[0])) __pyx_t_2 = 0;
   if (unlikely(__pyx_t_2 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_2);
     __PYX_ERR(0, 154, __pyx_L1_error)
   }
   (void)(memcpy((&(__pyx_v_state.MT[0])), (&(*((uint32_t *) ( /* dim=0 */ ((char *) (((uint32_t *) __pyx_v_mt.data) + __pyx_t_1)) )))), (sizeof(__pyx_v_state.MT))));
 
-  /* "arrow/arrowhead.pyx":156
+  /* "stochastic_arrow/arrowhead.pyx":156
  *         memcpy(&state.MT[0], &mt[0], sizeof(state.MT))
  *         memcpy(
  *             &state.MT_TEMPERED[0], &mt_tempered[0],             # <<<<<<<<<<<<<<
  *             sizeof(state.MT_TEMPERED))
  *         state.index = index
  */
   __pyx_t_1 = 0;
@@ -4128,54 +4119,54 @@
     if (unlikely(__pyx_t_1 < 0)) __pyx_t_2 = 0;
   } else if (unlikely(__pyx_t_1 >= __pyx_v_mt_tempered.shape[0])) __pyx_t_2 = 0;
   if (unlikely(__pyx_t_2 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_2);
     __PYX_ERR(0, 156, __pyx_L1_error)
   }
 
-  /* "arrow/arrowhead.pyx":155
+  /* "stochastic_arrow/arrowhead.pyx":155
  *         cdef mersenne.MTState state
  *         memcpy(&state.MT[0], &mt[0], sizeof(state.MT))
  *         memcpy(             # <<<<<<<<<<<<<<
  *             &state.MT_TEMPERED[0], &mt_tempered[0],
  *             sizeof(state.MT_TEMPERED))
  */
   (void)(memcpy((&(__pyx_v_state.MT_TEMPERED[0])), (&(*((uint32_t *) ( /* dim=0 */ ((char *) (((uint32_t *) __pyx_v_mt_tempered.data) + __pyx_t_1)) )))), (sizeof(__pyx_v_state.MT_TEMPERED))));
 
-  /* "arrow/arrowhead.pyx":158
+  /* "stochastic_arrow/arrowhead.pyx":158
  *             &state.MT_TEMPERED[0], &mt_tempered[0],
  *             sizeof(state.MT_TEMPERED))
  *         state.index = index             # <<<<<<<<<<<<<<
  *         obsidian.set_random_state(&self.info, &state)
  * 
  */
   __pyx_v_state.index = __pyx_v_index;
 
-  /* "arrow/arrowhead.pyx":159
+  /* "stochastic_arrow/arrowhead.pyx":159
  *             sizeof(state.MT_TEMPERED))
  *         state.index = index
  *         obsidian.set_random_state(&self.info, &state)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   set_random_state((&__pyx_v_self->info), (&__pyx_v_state));
 
-  /* "arrow/arrowhead.pyx":150
+  /* "stochastic_arrow/arrowhead.pyx":150
  *         return mt, mt_tempered, index
  * 
  *     def set_random_state(             # <<<<<<<<<<<<<<
  *             self, uint32_t[::1] mt, uint32_t[::1] mt_tempered,
  *             size_t index):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.set_random_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.set_random_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_mt, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_mt_tempered, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -4184,27 +4175,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead_16__reduce_cython__(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self));
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_16__reduce_cython__(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self) {
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -4226,42 +4217,42 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_5arrow_9arrowhead_9Arrowhead_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5arrow_9arrowhead_9Arrowhead_18__setstate_cython__(((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_18__setstate_cython__(((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5arrow_9arrowhead_9Arrowhead_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5arrow_9arrowhead_Arrowhead *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_16stochastic_arrow_9arrowhead_9Arrowhead_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -4283,91 +4274,91 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("arrow.arrowhead.Arrowhead.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.Arrowhead.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "arrow/arrowhead.pyx":162
+/* "stochastic_arrow/arrowhead.pyx":162
  * 
  * 
  * cdef np.ndarray copy_c_array(             # <<<<<<<<<<<<<<
  *         void *source, np.npy_intp element_count, size_t element_size, int np_typenum):
  *     """Copy the source 1-D C array into a numpy array so it's independent of the
  */
 
-static PyArrayObject *__pyx_f_5arrow_9arrowhead_copy_c_array(void *__pyx_v_source, npy_intp __pyx_v_element_count, size_t __pyx_v_element_size, int __pyx_v_np_typenum) {
+static PyArrayObject *__pyx_f_16stochastic_arrow_9arrowhead_copy_c_array(void *__pyx_v_source, npy_intp __pyx_v_element_count, size_t __pyx_v_element_size, int __pyx_v_np_typenum) {
   PyArrayObject *__pyx_v_result = 0;
   PyArrayObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy_c_array", 0);
 
-  /* "arrow/arrowhead.pyx":167
+  /* "stochastic_arrow/arrowhead.pyx":167
  *     source buffer.
  *     """
  *     cdef np.ndarray result = np.PyArray_SimpleNew(1, &element_count, np_typenum)             # <<<<<<<<<<<<<<
  *     memcpy(np.PyArray_DATA(result), source, element_size * element_count)
  *     return result
  */
   __pyx_t_1 = PyArray_SimpleNew(1, (&__pyx_v_element_count), __pyx_v_np_typenum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 167, __pyx_L1_error)
   __pyx_v_result = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "arrow/arrowhead.pyx":168
+  /* "stochastic_arrow/arrowhead.pyx":168
  *     """
  *     cdef np.ndarray result = np.PyArray_SimpleNew(1, &element_count, np_typenum)
  *     memcpy(np.PyArray_DATA(result), source, element_size * element_count)             # <<<<<<<<<<<<<<
  *     return result
  */
   (void)(memcpy(PyArray_DATA(__pyx_v_result), __pyx_v_source, (__pyx_v_element_size * __pyx_v_element_count)));
 
-  /* "arrow/arrowhead.pyx":169
+  /* "stochastic_arrow/arrowhead.pyx":169
  *     cdef np.ndarray result = np.PyArray_SimpleNew(1, &element_count, np_typenum)
  *     memcpy(np.PyArray_DATA(result), source, element_size * element_count)
  *     return result             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "arrow/arrowhead.pyx":162
+  /* "stochastic_arrow/arrowhead.pyx":162
  * 
  * 
  * cdef np.ndarray copy_c_array(             # <<<<<<<<<<<<<<
  *         void *source, np.npy_intp element_count, size_t element_size, int np_typenum):
  *     """Copy the source 1-D C array into a numpy array so it's independent of the
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("arrow.arrowhead.copy_c_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("stochastic_arrow.arrowhead.copy_c_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4376,29 +4367,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4409,15 +4400,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4426,29 +4417,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4459,15 +4450,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4476,29 +4467,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4509,15 +4500,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4526,29 +4517,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4559,15 +4550,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4576,29 +4567,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4609,212 +4600,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4830,15 +4829,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4846,84 +4845,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4938,15 +4937,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4962,15 +4961,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4978,84 +4977,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5070,15 +5069,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5094,15 +5093,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5110,84 +5109,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5202,176 +5201,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -18417,87 +18416,87 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_tp_new_5arrow_9arrowhead_Arrowhead(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_5arrow_9arrowhead_Arrowhead *p;
+static PyObject *__pyx_tp_new_16stochastic_arrow_9arrowhead_Arrowhead(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)o);
+  p = ((struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)o);
   p->refs = ((PyObject*)Py_None); Py_INCREF(Py_None);
-  if (unlikely(__pyx_pw_5arrow_9arrowhead_9Arrowhead_1__cinit__(o, a, k) < 0)) goto bad;
+  if (unlikely(__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_5arrow_9arrowhead_Arrowhead(PyObject *o) {
-  struct __pyx_obj_5arrow_9arrowhead_Arrowhead *p = (struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)o;
+static void __pyx_tp_dealloc_16stochastic_arrow_9arrowhead_Arrowhead(PyObject *o) {
+  struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *p = (struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_5arrow_9arrowhead_9Arrowhead_5__dealloc__(o);
+    __pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_5__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->refs);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static int __pyx_tp_traverse_5arrow_9arrowhead_Arrowhead(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_16stochastic_arrow_9arrowhead_Arrowhead(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_5arrow_9arrowhead_Arrowhead *p = (struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)o;
+  struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *p = (struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)o;
   if (p->refs) {
     e = (*v)(p->refs, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_5arrow_9arrowhead_Arrowhead(PyObject *o) {
+static int __pyx_tp_clear_16stochastic_arrow_9arrowhead_Arrowhead(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_5arrow_9arrowhead_Arrowhead *p = (struct __pyx_obj_5arrow_9arrowhead_Arrowhead *)o;
+  struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *p = (struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead *)o;
   tmp = ((PyObject*)p->refs);
   p->refs = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyMethodDef __pyx_methods_5arrow_9arrowhead_Arrowhead[] = {
-  {"evolve", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5arrow_9arrowhead_9Arrowhead_7evolve, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5arrow_9arrowhead_9Arrowhead_6evolve},
-  {"reactions_count", (PyCFunction)__pyx_pw_5arrow_9arrowhead_9Arrowhead_9reactions_count, METH_NOARGS, __pyx_doc_5arrow_9arrowhead_9Arrowhead_8reactions_count},
-  {"substrates_count", (PyCFunction)__pyx_pw_5arrow_9arrowhead_9Arrowhead_11substrates_count, METH_NOARGS, __pyx_doc_5arrow_9arrowhead_9Arrowhead_10substrates_count},
-  {"get_random_state", (PyCFunction)__pyx_pw_5arrow_9arrowhead_9Arrowhead_13get_random_state, METH_NOARGS, __pyx_doc_5arrow_9arrowhead_9Arrowhead_12get_random_state},
-  {"set_random_state", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5arrow_9arrowhead_9Arrowhead_15set_random_state, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_5arrow_9arrowhead_9Arrowhead_17__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_5arrow_9arrowhead_9Arrowhead_19__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_16stochastic_arrow_9arrowhead_Arrowhead[] = {
+  {"evolve", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_7evolve, METH_VARARGS|METH_KEYWORDS, __pyx_doc_16stochastic_arrow_9arrowhead_9Arrowhead_6evolve},
+  {"reactions_count", (PyCFunction)__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_9reactions_count, METH_NOARGS, __pyx_doc_16stochastic_arrow_9arrowhead_9Arrowhead_8reactions_count},
+  {"substrates_count", (PyCFunction)__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_11substrates_count, METH_NOARGS, __pyx_doc_16stochastic_arrow_9arrowhead_9Arrowhead_10substrates_count},
+  {"get_random_state", (PyCFunction)__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_13get_random_state, METH_NOARGS, __pyx_doc_16stochastic_arrow_9arrowhead_9Arrowhead_12get_random_state},
+  {"set_random_state", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_15set_random_state, METH_VARARGS|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_17__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_19__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_5arrow_9arrowhead_Arrowhead = {
+static PyTypeObject __pyx_type_16stochastic_arrow_9arrowhead_Arrowhead = {
   PyVarObject_HEAD_INIT(0, 0)
-  "arrow.arrowhead.Arrowhead", /*tp_name*/
-  sizeof(struct __pyx_obj_5arrow_9arrowhead_Arrowhead), /*tp_basicsize*/
+  "stochastic_arrow.arrowhead.Arrowhead", /*tp_name*/
+  sizeof(struct __pyx_obj_16stochastic_arrow_9arrowhead_Arrowhead), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_5arrow_9arrowhead_Arrowhead, /*tp_dealloc*/
+  __pyx_tp_dealloc_16stochastic_arrow_9arrowhead_Arrowhead, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -18516,31 +18515,31 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   "Cython interface to the C-coded Gillespie algorithm \"obsidian\", leaving\n    obsidian.c free of Python dependencies.\n    ", /*tp_doc*/
-  __pyx_tp_traverse_5arrow_9arrowhead_Arrowhead, /*tp_traverse*/
-  __pyx_tp_clear_5arrow_9arrowhead_Arrowhead, /*tp_clear*/
+  __pyx_tp_traverse_16stochastic_arrow_9arrowhead_Arrowhead, /*tp_traverse*/
+  __pyx_tp_clear_16stochastic_arrow_9arrowhead_Arrowhead, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_5arrow_9arrowhead_Arrowhead, /*tp_methods*/
+  __pyx_methods_16stochastic_arrow_9arrowhead_Arrowhead, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
-  __pyx_pw_5arrow_9arrowhead_9Arrowhead_3__init__, /*tp_init*/
+  __pyx_pw_16stochastic_arrow_9arrowhead_9Arrowhead_3__init__, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_5arrow_9arrowhead_Arrowhead, /*tp_new*/
+  __pyx_tp_new_16stochastic_arrow_9arrowhead_Arrowhead, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -18551,15 +18550,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -18678,15 +18677,15 @@
   #endif
   __pyx_array_getbuffer, /*bf_getbuffer*/
   0, /*bf_releasebuffer*/
 };
 
 static PyTypeObject __pyx_type___pyx_array = {
   PyVarObject_HEAD_INIT(0, 0)
-  "arrow.arrowhead.array", /*tp_name*/
+  "stochastic_arrow.arrowhead.array", /*tp_name*/
   sizeof(struct __pyx_array_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_array, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -18743,15 +18742,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -18800,15 +18799,15 @@
   {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_1__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_3__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_MemviewEnum = {
   PyVarObject_HEAD_INIT(0, 0)
-  "arrow.arrowhead.Enum", /*tp_name*/
+  "stochastic_arrow.arrowhead.Enum", /*tp_name*/
   sizeof(struct __pyx_MemviewEnum_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_Enum, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -18865,15 +18864,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -19064,15 +19063,15 @@
   #endif
   __pyx_memoryview_getbuffer, /*bf_getbuffer*/
   0, /*bf_releasebuffer*/
 };
 
 static PyTypeObject __pyx_type___pyx_memoryview = {
   PyVarObject_HEAD_INIT(0, 0)
-  "arrow.arrowhead.memoryview", /*tp_name*/
+  "stochastic_arrow.arrowhead.memoryview", /*tp_name*/
   sizeof(struct __pyx_memoryview_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_memoryview, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19129,15 +19128,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -19205,15 +19204,15 @@
 static struct PyGetSetDef __pyx_getsets__memoryviewslice[] = {
   {(char *)"base", __pyx_getprop___pyx_memoryviewslice_base, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_memoryviewslice = {
   PyVarObject_HEAD_INIT(0, 0)
-  "arrow.arrowhead._memoryviewslice", /*tp_name*/
+  "stochastic_arrow.arrowhead._memoryviewslice", /*tp_name*/
   sizeof(struct __pyx_memoryviewslice_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc__memoryviewslice, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19278,15 +19277,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -19444,15 +19443,15 @@
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 40, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 941, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 134, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 181, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
   return 0;
@@ -19479,33 +19478,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 944, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../usr/local/var/pyenv/versions/arrow-3.11.3/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 950, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -19824,24 +19823,24 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_5arrow_9arrowhead_Arrowhead) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_16stochastic_arrow_9arrowhead_Arrowhead) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_5arrow_9arrowhead_Arrowhead.tp_print = 0;
+  __pyx_type_16stochastic_arrow_9arrowhead_Arrowhead.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5arrow_9arrowhead_Arrowhead.tp_dictoffset && __pyx_type_5arrow_9arrowhead_Arrowhead.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_5arrow_9arrowhead_Arrowhead.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_16stochastic_arrow_9arrowhead_Arrowhead.tp_dictoffset && __pyx_type_16stochastic_arrow_9arrowhead_Arrowhead.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_16stochastic_arrow_9arrowhead_Arrowhead.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Arrowhead, (PyObject *)&__pyx_type_5arrow_9arrowhead_Arrowhead) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5arrow_9arrowhead_Arrowhead) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
-  __pyx_ptype_5arrow_9arrowhead_Arrowhead = &__pyx_type_5arrow_9arrowhead_Arrowhead;
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Arrowhead, (PyObject *)&__pyx_type_16stochastic_arrow_9arrowhead_Arrowhead) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_16stochastic_arrow_9arrowhead_Arrowhead) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_ptype_16stochastic_arrow_9arrowhead_Arrowhead = &__pyx_type_16stochastic_arrow_9arrowhead_Arrowhead;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
   if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
@@ -19902,70 +19901,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -20157,22 +20125,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_arrow__arrowhead) {
+  if (__pyx_module_is_main_stochastic_arrow__arrowhead) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "arrow.arrowhead")) {
-      if (unlikely(PyDict_SetItemString(modules, "arrow.arrowhead", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "stochastic_arrow.arrowhead")) {
+      if (unlikely(PyDict_SetItemString(modules, "stochastic_arrow.arrowhead", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -20185,36 +20153,36 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "arrow/arrowhead.pyx":11
+  /* "stochastic_arrow/arrowhead.pyx":11
  * from libc.stdlib cimport free
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * 
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "arrow/arrowhead.pyx":18
+  /* "stochastic_arrow/arrowhead.pyx":18
  * 
  * 
  * np.import_array()  # Initialize numpy's C API so it won't segfault             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 18, __pyx_L1_error)
 
-  /* "arrow/arrowhead.pyx":1
+  /* "stochastic_arrow/arrowhead.pyx":1
  * # cython: language_level=3str             # <<<<<<<<<<<<<<
  * 
  * from __future__ import absolute_import, division, print_function
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -20376,19 +20344,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init arrow.arrowhead", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init stochastic_arrow.arrowhead", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init arrow.arrowhead");
+    PyErr_SetString(PyExc_ImportError, "init stochastic_arrow.arrowhead");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -20975,14 +20943,54 @@
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
     PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
                  Py_TYPE(obj)->tp_name, type->tp_name);
     return 0;
 }
 
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -22359,18 +22367,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -22416,22 +22424,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -24055,15 +24063,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24251,15 +24259,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24485,15 +24493,15 @@
                         } else if (8 * sizeof(int64_t) >= 4 * PyLong_SHIFT) {
                             return (int64_t) (((((((((int64_t)digits[3]) << PyLong_SHIFT) | (int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24719,15 +24727,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24953,15 +24961,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `stochastic-arrow-0.5.2/arrow/math.py` & `stochastic-arrow-1.0.0/stochastic_arrow/math.py`

 * *Files identical despite different names*

### Comparing `stochastic-arrow-0.5.2/arrow/mersenne.c` & `stochastic-arrow-1.0.0/stochastic_arrow/mersenne.c`

 * *Files identical despite different names*

### Comparing `stochastic-arrow-0.5.2/arrow/mersenne.h` & `stochastic-arrow-1.0.0/stochastic_arrow/mersenne.h`

 * *Files identical despite different names*

### Comparing `stochastic-arrow-0.5.2/arrow/obsidian.c` & `stochastic-arrow-1.0.0/stochastic_arrow/obsidian.c`

 * *Files 1% similar despite different names*

```diff
@@ -111,22 +111,22 @@
   // function
   double *propensities = malloc((sizeof (double)) * reactions_count);
   int64_t *update = malloc((sizeof (int64_t)) * reactions_count);
   int64_t update_length = reactions_count;
 
   // if something goes wrong (like an overflow in propensities), the status will be
   // set to some meaningful number
-  int64_t status = 0;
+  int status = 0;
 
   if (time == NULL ||
       events == NULL ||
       outcome == NULL ||
       propensities == NULL ||
       update == NULL) {
-    printf("arrow.obsidian.evolve - failed to allocate memory: %d", errno);
+    printf("stochastic_arrow.obsidian.evolve - failed to allocate memory: %d", errno);
 
     free(time);
     free(events);
     free(outcome);
     free(propensities);
     free(update);
 
@@ -183,22 +183,22 @@
 
     if (status > 0) {
       break;
     }
 
     if (isnan(total)) {
       printf("failed simulation: total propensity is NaN\n");
-      int max_reaction = 0;
+      int64_t max_reaction = 0;
       for (reaction = 0; reaction < reactions_count; reaction++) {
-        printf("reaction %lld is %f\n", reaction, propensities[reaction]);
+        printf("reaction %lld is %f\n", (long long)reaction, propensities[reaction]);
         if (isnan(propensities[reaction]) || propensities[reaction] > propensities[max_reaction]) {
           max_reaction = reaction;
         }
       }
-      printf("largest reaction is %d at %f\n", max_reaction, propensities[max_reaction]);
+      printf("largest reaction is %lld at %f\n", (long long)max_reaction, propensities[max_reaction]);
       interval = 0.0;
       choice = -1;
       status = 1; // overflow
       break;
     }
 
     // If the total is zero, then we have no more reactions to perform and can exit
@@ -274,15 +274,15 @@
       step += 1;
 
       // If our step has advanced beyond the current `event_bounds`, double the
       // `event_bounds` and reallocate these arrays with the new size
       if (step >= event_bounds) {
         double *new_time = malloc((sizeof (double)) * event_bounds * 2);
         if (new_time == NULL) {
-          printf("arrow.obsidian.evolve - failed to allocate memory: %d", errno);
+          printf("stochastic_arrow.obsidian.evolve - failed to allocate memory: %d", errno);
 
           free(time);
           free(events);
           free(outcome);
           free(propensities);
           free(update);
 
@@ -291,15 +291,15 @@
 
         memcpy(new_time, time, (sizeof (double)) * event_bounds);
         free(time);
         time = new_time;
 
         int64_t *new_events = malloc((sizeof (int64_t)) * event_bounds * 2);
         if (new_events == NULL) {
-          printf("arrow.obsidian.evolve - failed to allocate memory: %d", errno);
+          printf("stochastic_arrow.obsidian.evolve - failed to allocate memory: %d", errno);
 
           free(time);
           free(events);
           free(outcome);
           free(propensities);
           free(update);
```

### Comparing `stochastic-arrow-0.5.2/arrow/obsidian.h` & `stochastic-arrow-1.0.0/stochastic_arrow/obsidian.h`

 * *Files identical despite different names*

### Comparing `stochastic-arrow-0.5.2/arrow/reference.py` & `stochastic-arrow-1.0.0/stochastic_arrow/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import absolute_import, division, print_function
 
 import numpy as np
 from six import moves
 
-from arrow.math import multichoose
+from stochastic_arrow.math import multichoose
 
 
 def derive_reactants(stoichiometric_matrix):
     '''
     Calculate the various derived values this Gillespie implementation uses extensively
     to avoid recalculating these values every step or call to `evolve`.
```

### Comparing `stochastic-arrow-0.5.2/setup.py` & `stochastic-arrow-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,50 +9,53 @@
 from distutils.core import setup
 from distutils.extension import Extension
 import numpy as np
 
 _ = setuptools
 
 
-with open("README.md", 'r') as readme:
+with open("README.md", 'r', encoding="utf-8") as readme:
     long_description = readme.read()
 
 current_dir = os.getcwd()
-arrow_dir = os.path.join(current_dir, 'arrow')
+arrow_dir = os.path.join(current_dir, 'stochastic_arrow')
 
 # Compile the Cython code to C for development builds:
 #    USE_CYTHON=1 python setup.py build_ext --inplace
 # and for building source distribution packages:
 #    USE_CYTHON=1 python setup.py sdist
 # and *not* when installing a distribution package.
 # See http://docs.cython.org/en/latest/src/userguide/source_files_and_compilation.html#distributing-cython-modules
 USE_CYTHON = 'USE_CYTHON' in os.environ
 
 ext = '.pyx' if USE_CYTHON else '.c'
 
 cython_extensions = [
-    Extension('arrow.arrowhead',
-              sources=['arrow/mersenne.c', 'arrow/obsidian.c', 'arrow/arrowhead'+ext,],
-              include_dirs=['arrow', np.get_include()],
+    Extension('stochastic_arrow.arrowhead',
+              sources=[
+                  'stochastic_arrow/mersenne.c',
+                  'stochastic_arrow/obsidian.c',
+                  'stochastic_arrow/arrowhead'+ext,],
+              include_dirs=['stochastic_arrow', np.get_include()],
               define_macros=[('NPY_NO_DEPRECATED_API', 'NPY_1_7_API_VERSION')],
               )]
 
 if USE_CYTHON:
     from Cython.Build import cythonize
     cython_extensions = cythonize(
         cython_extensions,
-        include_path=['arrow'],
+        include_path=['stochastic_arrow'],
         annotate=True,  # to get an HTML code listing
     )
 
 setup(
     name='stochastic-arrow',
-    version='0.5.2',
-    packages=['arrow'],
-    author='Ryan Spangler, John Mason, Jerry Morrison, Chris Skalnik, Travis Ahn-Horst',
+    version='1.0.0',
+    packages=['stochastic_arrow'],
+    author='Ryan Spangler, John Mason, Jerry Morrison, Chris Skalnik, Travis Ahn-Horst, Sean Cheah',
     author_email='ryan.spangler@gmail.com',
     url='https://github.com/CovertLab/arrow',
     license='MIT',
     include_dirs=[arrow_dir, np.get_include()],
     ext_modules=cython_extensions,
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `stochastic-arrow-0.5.2/stochastic_arrow.egg-info/PKG-INFO` & `stochastic-arrow-1.0.0/stochastic_arrow.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: stochastic-arrow
-Version: 0.5.2
+Version: 1.0.0
 Home-page: https://github.com/CovertLab/arrow
-Author: Ryan Spangler, John Mason, Jerry Morrison, Chris Skalnik, Travis Ahn-Horst
+Author: Ryan Spangler, John Mason, Jerry Morrison, Chris Skalnik, Travis Ahn-Horst, Sean Cheah
 Author-email: ryan.spangler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -35,22 +35,29 @@
 ## Installation
 
 Add the following to your `requirements.txt`, or run
 `pip install stochastic-arrow` to install it [from PyPI](https://pypi.org/project/stochastic-arrow/):
 
     stochastic-arrow
 
+**NOTE:** If upgrading from a version older than 1.0.0, check if the [`arrow`](https://github.com/arrow-py/arrow) datetime package is installed. If so, uninstall `arrow` before upgrading `stochastic-arrow`, then reinstall `arrow`.
+
+    > pip show arrow
+    > pip uninstall arrow
+    > pip install stochastic-arrow
+    > pip install arrow
+
 ## Usage
 
-The `arrow` library presents a single class as an interface,
+The `stochastic_arrow` library presents a single class as an interface,
 `StochasticSystem`, which operates on a set of reactions (encoded as a `numpy`
 matrix of stoichiometrix coefficients) and associated reaction rates:
 
 ```python
-from arrow import StochasticSystem
+from stochastic_arrow import StochasticSystem
 import numpy as np
 
 # Each row is a reaction and each column is a molecular species (or other
 # entity). The first reaction here means that the first and second elements
 # combine to create the third, while the fourth is unaffected.
 stoichiometric_matrix = np.array([
     [1, 1, -1, 0],
@@ -93,50 +100,54 @@
 ```
 
 If you are interested in the history of states for plotting or otherwise, these can be
 derived from the list of events and the stoichiometric matrix, along with the inital
 state. `reenact_events` will do this for you:
 
 ```python
-from arrow import reenact_events
+from stochastic_arrow import reenact_events
 
-history = reenact_events(stoichiometry, result['events'], state)
+history = reenact_events(stoichiometric_matrix, result['events'], state)
 ```
 
 ## Testing
 
-`arrow` uses [pytest](https://docs.pytest.org/en/latest/). To test it:
+`stochastic_arrow` uses [pytest](https://docs.pytest.org/en/latest/). To test it:
 
     > make clean compile
     > pytest
 
 **NOTE:** `make compile` without an explicit `clean` might not fully build the extension.
 
 There are more command line features in test_arrow:
 
-    > python -m arrow.test.test_arrow --complexation
+    > python -m stochastic_arrow.test.test_arrow --complexation
 
-    > python -m arrow.test.test_arrow --plot
+    > python -m stochastic_arrow.test.test_arrow --plot
 
-    > python -m arrow.test.test_arrow --obsidian
+    > python -m stochastic_arrow.test.test_arrow --obsidian
 
-    > python -m arrow.test.test_arrow --memory
+    > python -m stochastic_arrow.test.test_arrow --memory
 
-    > python -m arrow.test.test_arrow --time
+    > python -m stochastic_arrow.test.test_arrow --time
 
 More examples:
 
-    > python -m arrow.test.test_hang
+    > python -m stochastic_arrow.test.test_hang
 
-    > pytest -m arrow/test/test_arrow.py
+    > pytest -m stochastic_arrow/test/test_arrow.py
 
     > pytest -k flagella
 
 ## Changelog
 
+### Version 1.0.0
+
+* Rename module to `stochastic_arrow` to avoid name conflict (Issue #51). **All users must update their import statements to use `stochastic_arrow` instead of `arrow`.**
+
 ### Version 0.5.2
 
 * Update to Cython 0.29.34. (Cython 3.0.0 is now in beta.)
 
 ### Version 0.5.1
 
 * Update to Cython 3.0.0a11 for compatibility with Python 3.11.
```

