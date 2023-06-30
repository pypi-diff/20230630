# Comparing `tmp/fatfs-0.0.6.tar.gz` & `tmp/fatfs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fatfs-0.0.6.tar", last modified: Tue Feb 21 13:52:26 2023, max compression
+gzip compressed data, was "fatfs-0.0.7.tar", last modified: Fri Jun 30 11:04:07 2023, max compression
```

## Comparing `fatfs-0.0.6.tar` & `fatfs-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 krakonos  (1000) krakonos  (1000)        0 2023-02-21 13:52:26.056473 fatfs-0.0.6/
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)      610 2023-02-21 13:18:44.000000 fatfs-0.0.6/LICENSE.md
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)       33 2023-02-21 13:18:44.000000 fatfs-0.0.6/MANIFEST.in
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)     1035 2023-02-21 13:52:26.056473 fatfs-0.0.6/PKG-INFO
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)      264 2023-02-21 13:18:44.000000 fatfs-0.0.6/README.md
-drwxr-xr-x   0 krakonos  (1000) krakonos  (1000)        0 2023-02-21 13:52:26.049807 fatfs-0.0.6/fatfs/
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)       93 2023-02-21 13:18:44.000000 fatfs-0.0.6/fatfs/__init__.py
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)     1716 2023-02-21 13:18:44.000000 fatfs-0.0.6/fatfs/diskio.py
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)    10237 2023-02-21 13:18:44.000000 fatfs-0.0.6/fatfs/diskiocheck.c
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)   558159 2023-02-21 13:34:28.000000 fatfs-0.0.6/fatfs/wrapper.c
-drwxr-xr-x   0 krakonos  (1000) krakonos  (1000)        0 2023-02-21 13:52:26.049807 fatfs-0.0.6/fatfs.egg-info/
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)     1035 2023-02-21 13:52:24.000000 fatfs-0.0.6/fatfs.egg-info/PKG-INFO
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)      460 2023-02-21 13:52:25.000000 fatfs-0.0.6/fatfs.egg-info/SOURCES.txt
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)        1 2023-02-21 13:52:24.000000 fatfs-0.0.6/fatfs.egg-info/dependency_links.txt
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)        1 2023-02-21 13:34:41.000000 fatfs-0.0.6/fatfs.egg-info/not-zip-safe
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)        7 2023-02-21 13:52:25.000000 fatfs-0.0.6/fatfs.egg-info/requires.txt
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)       14 2023-02-21 13:52:25.000000 fatfs-0.0.6/fatfs.egg-info/top_level.txt
-drwxr-xr-x   0 krakonos  (1000) krakonos  (1000)        0 2023-02-21 13:52:26.046474 fatfs-0.0.6/foreign/
-drwxr-xr-x   0 krakonos  (1000) krakonos  (1000)        0 2023-02-21 13:52:26.046474 fatfs-0.0.6/foreign/fatfs/
-drwxr-xr-x   0 krakonos  (1000) krakonos  (1000)        0 2023-02-21 13:52:26.053140 fatfs-0.0.6/foreign/fatfs/source/
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)     2693 2023-02-21 13:18:44.000000 fatfs-0.0.6/foreign/fatfs/source/diskio.h
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)   247597 2023-02-21 13:18:44.000000 fatfs-0.0.6/foreign/fatfs/source/ff.c
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)    16099 2023-02-21 13:18:44.000000 fatfs-0.0.6/foreign/fatfs/source/ff.h
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)    12202 2023-02-21 13:18:44.000000 fatfs-0.0.6/foreign/fatfs/source/ffconf.h
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)     5118 2023-02-21 13:18:44.000000 fatfs-0.0.6/foreign/fatfs/source/ffsystem.c
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)  1974982 2023-02-21 13:18:44.000000 fatfs-0.0.6/foreign/fatfs/source/ffunicode.c
--rw-r--r--   0 krakonos  (1000) krakonos  (1000)       38 2023-02-21 13:52:26.056473 fatfs-0.0.6/setup.cfg
--rwxr-xr-x   0 krakonos  (1000) krakonos  (1000)     2553 2023-02-21 13:51:13.000000 fatfs-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:04:07.313324 fatfs-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-30 11:03:49.000000 fatfs-0.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 11:03:49.000000 fatfs-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-30 11:04:07.313324 fatfs-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-30 11:03:49.000000 fatfs-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:04:07.305324 fatfs-0.0.7/fatfs/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 11:03:49.000000 fatfs-0.0.7/fatfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 11:03:49.000000 fatfs-0.0.7/fatfs/diskio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-06-30 11:03:49.000000 fatfs-0.0.7/fatfs/diskiocheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)   560653 2023-06-30 11:03:58.000000 fatfs-0.0.7/fatfs/wrapper.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:04:07.309324 fatfs-0.0.7/fatfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-30 11:04:07.000000 fatfs-0.0.7/fatfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-30 11:04:07.000000 fatfs-0.0.7/fatfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:04:07.000000 fatfs-0.0.7/fatfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:04:07.000000 fatfs-0.0.7/fatfs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 11:04:07.000000 fatfs-0.0.7/fatfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:04:07.305324 fatfs-0.0.7/foreign/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:04:07.305324 fatfs-0.0.7/foreign/fatfs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:04:07.309324 fatfs-0.0.7/foreign/fatfs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-30 11:03:49.000000 fatfs-0.0.7/foreign/fatfs/source/diskio.h
+-rw-r--r--   0 runner    (1001) docker     (123)   247597 2023-06-30 11:03:49.000000 fatfs-0.0.7/foreign/fatfs/source/ff.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-06-30 11:03:49.000000 fatfs-0.0.7/foreign/fatfs/source/ff.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-06-30 11:03:49.000000 fatfs-0.0.7/foreign/fatfs/source/ffconf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-30 11:03:49.000000 fatfs-0.0.7/foreign/fatfs/source/ffsystem.c
+-rw-r--r--   0 runner    (1001) docker     (123)  1974982 2023-06-30 11:03:49.000000 fatfs-0.0.7/foreign/fatfs/source/ffunicode.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:04:07.313324 fatfs-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2672 2023-06-30 11:03:49.000000 fatfs-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:04:07.313324 fatfs-0.0.7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1703 2023-06-30 11:03:49.000000 fatfs-0.0.7/tests/test_fatfs.py
```

### Comparing `fatfs-0.0.6/LICENSE.md` & `fatfs-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/PKG-INFO` & `fatfs-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fatfs
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper around ChaN's FatFS library for FAT filesystem manipulation.
 Home-page: https://github.com/krakonos/fatfs-python
 Author: Ladislav Laska
 Author-email: krakonos@krakonos.org
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # FatFS wrapper for Python
 
 This library provides a Python wrapper around [ChaN's FatFS](http://elm-chan.org/fsw/ff/00index_e.html) library.
```

### Comparing `fatfs-0.0.6/fatfs/diskio.py` & `fatfs-0.0.7/fatfs/diskio.py`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/fatfs/diskiocheck.c` & `fatfs-0.0.7/fatfs/diskiocheck.c`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/fatfs/wrapper.c` & `fatfs-0.0.7/fatfs/wrapper.c`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,20 @@
-/* Generated by Cython 0.29.30 */
-
-/* BEGIN: Cython Metadata
-{
-    "distutils": {
-        "depends": [
-            "foreign/fatfs/source/diskio.h",
-            "foreign/fatfs/source/ff.h"
-        ],
-        "include_dirs": [
-            "foreign/fatfs/source"
-        ],
-        "name": "wrapper",
-        "sources": [
-            "fatfs/wrapper.pyx",
-            "fatfs/diskiocheck.c",
-            "foreign/fatfs/source/ff.c",
-            "foreign/fatfs/source/ffsystem.c",
-            "foreign/fatfs/source/ffunicode.c"
-        ]
-    },
-    "module_name": "wrapper"
-}
-END: Cython Metadata */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_30"
-#define CYTHON_HEX_VERSION 0x001D1EF0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -68,14 +45,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -96,29 +74,34 @@
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
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -151,18 +134,64 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -174,15 +203,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -213,15 +242,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -523,35 +552,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -709,16 +738,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__wrapper
-#define __PYX_HAVE_API__wrapper
+#define __PYX_HAVE__fatfs__wrapper
+#define __PYX_HAVE_API__fatfs__wrapper
 /* Early includes */
 #include <stdint.h>
 #include "ff.h"
 #include "diskio.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
@@ -929,16 +958,16 @@
 
 static const char *__pyx_f[] = {
   "fatfs/wrapper.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_obj_7wrapper_FIL_Handle;
-struct __pyx_obj_7wrapper_FATFS_Handle;
+struct __pyx_obj_5fatfs_7wrapper_FIL_Handle;
+struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle;
 
 /* "fatfs/diskio.pxd":5
  * # Defined as macros in diskio.h
  * # We will duplicate them here as enum for further use
  * cdef enum DSTATUS_Values:             # <<<<<<<<<<<<<<
  *     STA_OK = 0
  *     STA_NOINIT = 1
@@ -961,35 +990,35 @@
   __pyx_e_5fatfs_6diskio_CTRL_SYNC = 0,
   __pyx_e_5fatfs_6diskio_GET_SECTOR_COUNT = 1,
   __pyx_e_5fatfs_6diskio_GET_SECTOR_SIZE = 2,
   __pyx_e_5fatfs_6diskio_GET_BLOCK_SIZE = 3,
   __pyx_e_5fatfs_6diskio_CTRL_TRIM = 4
 };
 
-/* "wrapper.pyx":107
+/* "fatfs/wrapper.pyx":107
  * # #endif
  * 
  * cdef class FIL_Handle:             # <<<<<<<<<<<<<<
  *     cdef FIL *fp
  *     def __cinit__(self):
  */
-struct __pyx_obj_7wrapper_FIL_Handle {
+struct __pyx_obj_5fatfs_7wrapper_FIL_Handle {
   PyObject_HEAD
   FIL *fp;
 };
 
 
-/* "wrapper.pyx":115
+/* "fatfs/wrapper.pyx":115
  *         PyMem_Free(self.fp)
  * 
  * cdef class FATFS_Handle:             # <<<<<<<<<<<<<<
  *     cdef FATFS* fp
  *     def __cinit__(self):
  */
-struct __pyx_obj_7wrapper_FATFS_Handle {
+struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle {
   PyObject_HEAD
   FATFS *fp;
 };
 
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
@@ -1089,26 +1118,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1541,23 +1570,23 @@
 
 /* Module declarations from 'fatfs.ff' */
 
 /* Module declarations from 'fatfs.diskio' */
 
 /* Module declarations from 'cpython.mem' */
 
-/* Module declarations from 'wrapper' */
-static PyTypeObject *__pyx_ptype_7wrapper_FIL_Handle = 0;
-static PyTypeObject *__pyx_ptype_7wrapper_FATFS_Handle = 0;
+/* Module declarations from 'fatfs.wrapper' */
+static PyTypeObject *__pyx_ptype_5fatfs_7wrapper_FIL_Handle = 0;
+static PyTypeObject *__pyx_ptype_5fatfs_7wrapper_FATFS_Handle = 0;
 __PYX_EXTERN_C DL_IMPORT(int) diskiocheck(void); /*proto*/
-#define __Pyx_MODULE_NAME "wrapper"
-extern int __pyx_module_is_main_wrapper;
-int __pyx_module_is_main_wrapper = 0;
+#define __Pyx_MODULE_NAME "fatfs.wrapper"
+extern int __pyx_module_is_main_fatfs__wrapper;
+int __pyx_module_is_main_fatfs__wrapper = 0;
 
-/* Implementation of 'wrapper' */
+/* Implementation of 'fatfs.wrapper' */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_print;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_map;
 static const char __pyx_k_d[] = "%d:";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_p[] = "p";
@@ -1614,15 +1643,14 @@
 static const char __pyx_k_au_size[] = "au_size";
 static const char __pyx_k_dataptr[] = "dataptr";
 static const char __pyx_k_dealloc[] = "__dealloc__";
 static const char __pyx_k_fresult[] = "fresult";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_ret_str[] = "ret_str";
 static const char __pyx_k_unmount[] = "unmount";
-static const char __pyx_k_wrapper[] = "wrapper";
 static const char __pyx_k_written[] = "written";
 static const char __pyx_k_args_str[] = "args_str";
 static const char __pyx_k_datetime[] = "datetime";
 static const char __pyx_k_function[] = "function";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pyf_mkfs[] = "pyf_mkfs";
 static const char __pyx_k_pyf_open[] = "pyf_open";
@@ -1641,14 +1669,15 @@
 static const char __pyx_k_UNKNOWN__i[] = "UNKNOWN_%i";
 static const char __pyx_k_ioctl_sync[] = "ioctl_sync";
 static const char __pyx_k_adjust_path[] = "_adjust_path";
 static const char __pyx_k_except_type[] = "except_type";
 static const char __pyx_k_FATFS_Handle[] = "FATFS_Handle";
 static const char __pyx_k_check_diskio[] = "check_diskio";
 static const char __pyx_k_except_value[] = "except_value";
+static const char __pyx_k_fatfs_wrapper[] = "fatfs.wrapper";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_workarea_size[] = "workarea_size";
 static const char __pyx_k_FatFSException[] = "FatFSException";
 static const char __pyx_k_Partition_mkfs[] = "Partition.mkfs";
 static const char __pyx_k_Partition_open[] = "Partition.open";
 static const char __pyx_k_FileHandle_read[] = "FileHandle.read";
 static const char __pyx_k_Partition_mkdir[] = "Partition.mkdir";
@@ -1728,14 +1757,15 @@
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_drive;
 static PyObject *__pyx_n_s_enter;
 static PyObject *__pyx_n_s_except_traceback;
 static PyObject *__pyx_n_s_except_type;
 static PyObject *__pyx_n_s_except_value;
 static PyObject *__pyx_n_s_exit;
+static PyObject *__pyx_n_s_fatfs_wrapper;
 static PyObject *__pyx_kp_s_fatfs_wrapper_pyx;
 static PyObject *__pyx_n_s_fp;
 static PyObject *__pyx_n_s_fph;
 static PyObject *__pyx_n_s_fresult;
 static PyObject *__pyx_n_s_fresult_to_name;
 static PyObject *__pyx_n_s_fs;
 static PyObject *__pyx_n_s_function;
@@ -1794,52 +1824,51 @@
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_unmount;
 static PyObject *__pyx_n_u_unmount;
 static PyObject *__pyx_n_s_workarea_size;
-static PyObject *__pyx_n_s_wrapper;
 static PyObject *__pyx_n_s_write;
 static PyObject *__pyx_n_u_write;
 static PyObject *__pyx_n_s_written;
 static PyObject *__pyx_n_s_year;
-static int __pyx_pf_7wrapper_10FIL_Handle___cinit__(struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_self); /* proto */
-static void __pyx_pf_7wrapper_10FIL_Handle_2__dealloc__(struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FIL_Handle_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FIL_Handle_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_7wrapper_12FATFS_Handle___cinit__(struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_self); /* proto */
-static void __pyx_pf_7wrapper_12FATFS_Handle_2__dealloc__(struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_12FATFS_Handle_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_12FATFS_Handle_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_7wrapper_pyf_open(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_fph, TCHAR const *__pyx_v_path, BYTE __pyx_v_mode); /* proto */
-static PyObject *__pyx_pf_7wrapper_2pyf_close(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_fph); /* proto */
-static PyObject *__pyx_pf_7wrapper_4pyf_write(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_fph, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_7wrapper_6pyf_mkdir(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path); /* proto */
-static PyObject *__pyx_pf_7wrapper_8pyf_mount(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_fph, TCHAR const *__pyx_v_path, BYTE __pyx_v_opt); /* proto */
-static PyObject *__pyx_pf_7wrapper_10pyf_mkfs(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path, PyObject *__pyx_v_n_fat, PyObject *__pyx_v_align, PyObject *__pyx_v_n_root, PyObject *__pyx_v_au_size, PyObject *__pyx_v_workarea_size); /* proto */
-static PyObject *__pyx_pf_7wrapper_12fresult_to_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fresult); /* proto */
-static PyObject *__pyx_pf_7wrapper_14FatFSException___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_function, PyObject *__pyx_v_ret, PyObject *__pyx_v_args); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FileHandle___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FileHandle_2close(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FileHandle_4__enter__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FileHandle_6__exit__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_except_type, CYTHON_UNUSED PyObject *__pyx_v_except_value, CYTHON_UNUSED PyObject *__pyx_v_except_traceback); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FileHandle_8__dealloc__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FileHandle_10write(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_7wrapper_10FileHandle_12read(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_size); /* proto */
-static PyObject *__pyx_pf_7wrapper_9Partition___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_disk); /* proto */
-static PyObject *__pyx_pf_7wrapper_9Partition_2_adjust_path(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path); /* proto */
-static PyObject *__pyx_pf_7wrapper_9Partition_4mount(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_9Partition_6unmount(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_9Partition_8mkfs(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7wrapper_9Partition_10mkdir(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path); /* proto */
-static PyObject *__pyx_pf_7wrapper_9Partition_12open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path, CYTHON_UNUSED PyObject *__pyx_v_mode); /* proto */
-static PyObject *__pyx_pf_7wrapper_14check_diskio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_drive); /* proto */
-static PyObject *__pyx_tp_new_7wrapper_FIL_Handle(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_7wrapper_FATFS_Handle(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static int __pyx_pf_5fatfs_7wrapper_10FIL_Handle___cinit__(struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_self); /* proto */
+static void __pyx_pf_5fatfs_7wrapper_10FIL_Handle_2__dealloc__(struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FIL_Handle_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FIL_Handle_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_5fatfs_7wrapper_12FATFS_Handle___cinit__(struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_self); /* proto */
+static void __pyx_pf_5fatfs_7wrapper_12FATFS_Handle_2__dealloc__(struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_12FATFS_Handle_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_12FATFS_Handle_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_pyf_open(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_fph, TCHAR const *__pyx_v_path, BYTE __pyx_v_mode); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_2pyf_close(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_fph); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_4pyf_write(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_fph, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_6pyf_mkdir(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_8pyf_mount(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_fph, TCHAR const *__pyx_v_path, BYTE __pyx_v_opt); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10pyf_mkfs(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path, PyObject *__pyx_v_n_fat, PyObject *__pyx_v_align, PyObject *__pyx_v_n_root, PyObject *__pyx_v_au_size, PyObject *__pyx_v_workarea_size); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_12fresult_to_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fresult); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_14FatFSException___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_function, PyObject *__pyx_v_ret, PyObject *__pyx_v_args); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_2close(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_4__enter__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_6__exit__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_except_type, CYTHON_UNUSED PyObject *__pyx_v_except_value, CYTHON_UNUSED PyObject *__pyx_v_except_traceback); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_8__dealloc__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_10write(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_12read(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_size); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_disk); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_2_adjust_path(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_4mount(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_6unmount(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_8mkfs(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_10mkdir(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_12open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path, CYTHON_UNUSED PyObject *__pyx_v_mode); /* proto */
+static PyObject *__pyx_pf_5fatfs_7wrapper_14check_diskio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_drive); /* proto */
+static PyObject *__pyx_tp_new_5fatfs_7wrapper_FIL_Handle(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_5fatfs_7wrapper_FATFS_Handle(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_5;
 static PyObject *__pyx_int_16;
 static PyObject *__pyx_int_21;
 static PyObject *__pyx_int_25;
@@ -1896,15 +1925,15 @@
 static PyObject *__pyx_codeobj__45;
 static PyObject *__pyx_codeobj__47;
 static PyObject *__pyx_codeobj__49;
 static PyObject *__pyx_codeobj__51;
 static PyObject *__pyx_codeobj__53;
 /* Late includes */
 
-/* "wrapper.pyx":8
+/* "fatfs/wrapper.pyx":8
  * __diskio_wrapper_disks = {}
  * 
  * cdef DSTATUS disk_initialize (BYTE pdrv):             # <<<<<<<<<<<<<<
  *     if pdrv in __diskio_wrapper_disks:
  *         return DSTATUS_Values.STA_OK
  */
 
@@ -1916,15 +1945,15 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("disk_initialize", 0);
 
-  /* "wrapper.pyx":9
+  /* "fatfs/wrapper.pyx":9
  * 
  * cdef DSTATUS disk_initialize (BYTE pdrv):
  *     if pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DSTATUS_Values.STA_OK
  *     else:
  */
   __pyx_t_1 = __Pyx_PyInt_From_BYTE(__pyx_v_pdrv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
@@ -1933,46 +1962,46 @@
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_2, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "wrapper.pyx":10
+    /* "fatfs/wrapper.pyx":10
  * cdef DSTATUS disk_initialize (BYTE pdrv):
  *     if pdrv in __diskio_wrapper_disks:
  *         return DSTATUS_Values.STA_OK             # <<<<<<<<<<<<<<
  *     else:
  *         return DSTATUS_Values.STA_NODISK
  */
     __pyx_r = __pyx_e_5fatfs_6diskio_STA_OK;
     goto __pyx_L0;
 
-    /* "wrapper.pyx":9
+    /* "fatfs/wrapper.pyx":9
  * 
  * cdef DSTATUS disk_initialize (BYTE pdrv):
  *     if pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DSTATUS_Values.STA_OK
  *     else:
  */
   }
 
-  /* "wrapper.pyx":12
+  /* "fatfs/wrapper.pyx":12
  *         return DSTATUS_Values.STA_OK
  *     else:
  *         return DSTATUS_Values.STA_NODISK             # <<<<<<<<<<<<<<
  * 
  * cdef DSTATUS disk_status (BYTE pdrv):
  */
   /*else*/ {
     __pyx_r = __pyx_e_5fatfs_6diskio_STA_NODISK;
     goto __pyx_L0;
   }
 
-  /* "wrapper.pyx":8
+  /* "fatfs/wrapper.pyx":8
  * __diskio_wrapper_disks = {}
  * 
  * cdef DSTATUS disk_initialize (BYTE pdrv):             # <<<<<<<<<<<<<<
  *     if pdrv in __diskio_wrapper_disks:
  *         return DSTATUS_Values.STA_OK
  */
 
@@ -1983,15 +2012,15 @@
   __Pyx_WriteUnraisable("fatfs.diskio.disk_initialize", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":14
+/* "fatfs/wrapper.pyx":14
  *         return DSTATUS_Values.STA_NODISK
  * 
  * cdef DSTATUS disk_status (BYTE pdrv):             # <<<<<<<<<<<<<<
  *     if pdrv in __diskio_wrapper_disks:
  *         return DSTATUS_Values.STA_OK
  */
 
@@ -2003,15 +2032,15 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("disk_status", 0);
 
-  /* "wrapper.pyx":15
+  /* "fatfs/wrapper.pyx":15
  * 
  * cdef DSTATUS disk_status (BYTE pdrv):
  *     if pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DSTATUS_Values.STA_OK
  *     else:
  */
   __pyx_t_1 = __Pyx_PyInt_From_BYTE(__pyx_v_pdrv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
@@ -2020,46 +2049,46 @@
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_2, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "wrapper.pyx":16
+    /* "fatfs/wrapper.pyx":16
  * cdef DSTATUS disk_status (BYTE pdrv):
  *     if pdrv in __diskio_wrapper_disks:
  *         return DSTATUS_Values.STA_OK             # <<<<<<<<<<<<<<
  *     else:
  *         return DSTATUS_Values.STA_NODISK
  */
     __pyx_r = __pyx_e_5fatfs_6diskio_STA_OK;
     goto __pyx_L0;
 
-    /* "wrapper.pyx":15
+    /* "fatfs/wrapper.pyx":15
  * 
  * cdef DSTATUS disk_status (BYTE pdrv):
  *     if pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DSTATUS_Values.STA_OK
  *     else:
  */
   }
 
-  /* "wrapper.pyx":18
+  /* "fatfs/wrapper.pyx":18
  *         return DSTATUS_Values.STA_OK
  *     else:
  *         return DSTATUS_Values.STA_NODISK             # <<<<<<<<<<<<<<
  * 
  * cdef DRESULT disk_read (BYTE pdrv, BYTE* buff, DWORD sector, UINT count):
  */
   /*else*/ {
     __pyx_r = __pyx_e_5fatfs_6diskio_STA_NODISK;
     goto __pyx_L0;
   }
 
-  /* "wrapper.pyx":14
+  /* "fatfs/wrapper.pyx":14
  *         return DSTATUS_Values.STA_NODISK
  * 
  * cdef DSTATUS disk_status (BYTE pdrv):             # <<<<<<<<<<<<<<
  *     if pdrv in __diskio_wrapper_disks:
  *         return DSTATUS_Values.STA_OK
  */
 
@@ -2070,15 +2099,15 @@
   __Pyx_WriteUnraisable("fatfs.diskio.disk_status", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":20
+/* "fatfs/wrapper.pyx":20
  *         return DSTATUS_Values.STA_NODISK
  * 
  * cdef DRESULT disk_read (BYTE pdrv, BYTE* buff, DWORD sector, UINT count):             # <<<<<<<<<<<<<<
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  */
 
@@ -2102,15 +2131,15 @@
   UINT __pyx_t_12;
   BYTE __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("disk_read", 0);
 
-  /* "wrapper.pyx":21
+  /* "fatfs/wrapper.pyx":21
  * 
  * cdef DRESULT disk_read (BYTE pdrv, BYTE* buff, DWORD sector, UINT count):
  *     if not pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]
  */
   __pyx_t_1 = __Pyx_PyInt_From_BYTE(__pyx_v_pdrv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
@@ -2119,49 +2148,49 @@
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_2, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "wrapper.pyx":22
+    /* "fatfs/wrapper.pyx":22
  * cdef DRESULT disk_read (BYTE pdrv, BYTE* buff, DWORD sector, UINT count):
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY             # <<<<<<<<<<<<<<
  *     drive = __diskio_wrapper_disks[pdrv]
  * 
  */
     __pyx_r = RES_NOTRDY;
     goto __pyx_L0;
 
-    /* "wrapper.pyx":21
+    /* "fatfs/wrapper.pyx":21
  * 
  * cdef DRESULT disk_read (BYTE pdrv, BYTE* buff, DWORD sector, UINT count):
  *     if not pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]
  */
   }
 
-  /* "wrapper.pyx":23
+  /* "fatfs/wrapper.pyx":23
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]             # <<<<<<<<<<<<<<
  * 
  *     # Count is actually in number of sectors. Convert to bytes now.
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_diskio_wrapper_disks); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_2, __pyx_v_pdrv, BYTE, 0, __Pyx_PyInt_From_BYTE, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_drive = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":26
+  /* "fatfs/wrapper.pyx":26
  * 
  *     # Count is actually in number of sectors. Convert to bytes now.
  *     count *= drive.ioctl_get_sector_size()             # <<<<<<<<<<<<<<
  *     data = drive.read(sector, count)
  *     for i in range(count):
  */
   __pyx_t_1 = __Pyx_PyInt_From_UINT(__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
@@ -2187,15 +2216,15 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_7 = __Pyx_PyInt_As_UINT(__pyx_t_5); if (unlikely((__pyx_t_7 == ((UINT)-1)) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_count = __pyx_t_7;
 
-  /* "wrapper.pyx":27
+  /* "fatfs/wrapper.pyx":27
  *     # Count is actually in number of sectors. Convert to bytes now.
  *     count *= drive.ioctl_get_sector_size()
  *     data = drive.read(sector, count)             # <<<<<<<<<<<<<<
  *     for i in range(count):
  *         buff[i] = data[i]
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_drive, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
@@ -2252,51 +2281,51 @@
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "wrapper.pyx":28
+  /* "fatfs/wrapper.pyx":28
  *     count *= drive.ioctl_get_sector_size()
  *     data = drive.read(sector, count)
  *     for i in range(count):             # <<<<<<<<<<<<<<
  *         buff[i] = data[i]
  *     # TODO: This doesn't work: buff[:count] = data
  */
   __pyx_t_7 = __pyx_v_count;
   __pyx_t_11 = __pyx_t_7;
   for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
     __pyx_v_i = __pyx_t_12;
 
-    /* "wrapper.pyx":29
+    /* "fatfs/wrapper.pyx":29
  *     data = drive.read(sector, count)
  *     for i in range(count):
  *         buff[i] = data[i]             # <<<<<<<<<<<<<<
  *     # TODO: This doesn't work: buff[:count] = data
  *     return DRESULT.RES_OK
  */
     __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_data, __pyx_v_i, UINT, 0, __Pyx_PyInt_From_UINT, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_13 = __Pyx_PyInt_As_BYTE(__pyx_t_5); if (unlikely((__pyx_t_13 == ((BYTE)-1)) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     (__pyx_v_buff[__pyx_v_i]) = __pyx_t_13;
   }
 
-  /* "wrapper.pyx":31
+  /* "fatfs/wrapper.pyx":31
  *         buff[i] = data[i]
  *     # TODO: This doesn't work: buff[:count] = data
  *     return DRESULT.RES_OK             # <<<<<<<<<<<<<<
  * 
  * cdef DRESULT disk_write (BYTE pdrv, const BYTE* buff, DWORD sector, UINT count):
  */
   __pyx_r = RES_OK;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":20
+  /* "fatfs/wrapper.pyx":20
  *         return DSTATUS_Values.STA_NODISK
  * 
  * cdef DRESULT disk_read (BYTE pdrv, BYTE* buff, DWORD sector, UINT count):             # <<<<<<<<<<<<<<
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  */
 
@@ -2313,15 +2342,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_drive);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":33
+/* "fatfs/wrapper.pyx":33
  *     return DRESULT.RES_OK
  * 
  * cdef DRESULT disk_write (BYTE pdrv, const BYTE* buff, DWORD sector, UINT count):             # <<<<<<<<<<<<<<
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  */
 
@@ -2341,15 +2370,15 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("disk_write", 0);
 
-  /* "wrapper.pyx":34
+  /* "fatfs/wrapper.pyx":34
  * 
  * cdef DRESULT disk_write (BYTE pdrv, const BYTE* buff, DWORD sector, UINT count):
  *     if not pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]
  */
   __pyx_t_1 = __Pyx_PyInt_From_BYTE(__pyx_v_pdrv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
@@ -2358,49 +2387,49 @@
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_2, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "wrapper.pyx":35
+    /* "fatfs/wrapper.pyx":35
  * cdef DRESULT disk_write (BYTE pdrv, const BYTE* buff, DWORD sector, UINT count):
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY             # <<<<<<<<<<<<<<
  *     drive = __diskio_wrapper_disks[pdrv]
  * 
  */
     __pyx_r = RES_NOTRDY;
     goto __pyx_L0;
 
-    /* "wrapper.pyx":34
+    /* "fatfs/wrapper.pyx":34
  * 
  * cdef DRESULT disk_write (BYTE pdrv, const BYTE* buff, DWORD sector, UINT count):
  *     if not pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]
  */
   }
 
-  /* "wrapper.pyx":36
+  /* "fatfs/wrapper.pyx":36
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]             # <<<<<<<<<<<<<<
  * 
  *     # Count is actually in number of sectors. Convert to bytes now.
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_diskio_wrapper_disks); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_2, __pyx_v_pdrv, BYTE, 0, __Pyx_PyInt_From_BYTE, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_drive = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":39
+  /* "fatfs/wrapper.pyx":39
  * 
  *     # Count is actually in number of sectors. Convert to bytes now.
  *     count *= drive.ioctl_get_sector_size()             # <<<<<<<<<<<<<<
  *     drive.write(sector, count, buff[:count])
  *     return DRESULT.RES_OK
  */
   __pyx_t_1 = __Pyx_PyInt_From_UINT(__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
@@ -2426,15 +2455,15 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_7 = __Pyx_PyInt_As_UINT(__pyx_t_5); if (unlikely((__pyx_t_7 == ((UINT)-1)) && PyErr_Occurred())) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_count = __pyx_t_7;
 
-  /* "wrapper.pyx":40
+  /* "fatfs/wrapper.pyx":40
  *     # Count is actually in number of sectors. Convert to bytes now.
  *     count *= drive.ioctl_get_sector_size()
  *     drive.write(sector, count, buff[:count])             # <<<<<<<<<<<<<<
  *     return DRESULT.RES_OK
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_drive, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
@@ -2497,25 +2526,25 @@
     __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "wrapper.pyx":41
+  /* "fatfs/wrapper.pyx":41
  *     count *= drive.ioctl_get_sector_size()
  *     drive.write(sector, count, buff[:count])
  *     return DRESULT.RES_OK             # <<<<<<<<<<<<<<
  * 
  * cdef DRESULT disk_ioctl (BYTE pdrv, BYTE cmd, void* buff):
  */
   __pyx_r = RES_OK;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":33
+  /* "fatfs/wrapper.pyx":33
  *     return DRESULT.RES_OK
  * 
  * cdef DRESULT disk_write (BYTE pdrv, const BYTE* buff, DWORD sector, UINT count):             # <<<<<<<<<<<<<<
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  */
 
@@ -2532,15 +2561,15 @@
   __pyx_r = (DRESULT) 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_drive);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":43
+/* "fatfs/wrapper.pyx":43
  *     return DRESULT.RES_OK
  * 
  * cdef DRESULT disk_ioctl (BYTE pdrv, BYTE cmd, void* buff):             # <<<<<<<<<<<<<<
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  */
 
@@ -2556,15 +2585,15 @@
   DWORD __pyx_t_6;
   WORD __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("disk_ioctl", 0);
 
-  /* "wrapper.pyx":44
+  /* "fatfs/wrapper.pyx":44
  * 
  * cdef DRESULT disk_ioctl (BYTE pdrv, BYTE cmd, void* buff):
  *     if not pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]
  */
   __pyx_t_1 = __Pyx_PyInt_From_BYTE(__pyx_v_pdrv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
@@ -2573,59 +2602,59 @@
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_2, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "wrapper.pyx":45
+    /* "fatfs/wrapper.pyx":45
  * cdef DRESULT disk_ioctl (BYTE pdrv, BYTE cmd, void* buff):
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY             # <<<<<<<<<<<<<<
  *     drive = __diskio_wrapper_disks[pdrv]
  * 
  */
     __pyx_r = RES_NOTRDY;
     goto __pyx_L0;
 
-    /* "wrapper.pyx":44
+    /* "fatfs/wrapper.pyx":44
  * 
  * cdef DRESULT disk_ioctl (BYTE pdrv, BYTE cmd, void* buff):
  *     if not pdrv in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]
  */
   }
 
-  /* "wrapper.pyx":46
+  /* "fatfs/wrapper.pyx":46
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  *     drive = __diskio_wrapper_disks[pdrv]             # <<<<<<<<<<<<<<
  * 
  *     if cmd == IOCTL_Commands.CTRL_SYNC:
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_diskio_wrapper_disks); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_2, __pyx_v_pdrv, BYTE, 0, __Pyx_PyInt_From_BYTE, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_drive = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":48
+  /* "fatfs/wrapper.pyx":48
  *     drive = __diskio_wrapper_disks[pdrv]
  * 
  *     if cmd == IOCTL_Commands.CTRL_SYNC:             # <<<<<<<<<<<<<<
  *         drive.ioctl_sync()
  *     elif cmd == IOCTL_Commands.GET_SECTOR_COUNT:
  */
   switch (__pyx_v_cmd) {
     case __pyx_e_5fatfs_6diskio_CTRL_SYNC:
 
-    /* "wrapper.pyx":49
+    /* "fatfs/wrapper.pyx":49
  * 
  *     if cmd == IOCTL_Commands.CTRL_SYNC:
  *         drive.ioctl_sync()             # <<<<<<<<<<<<<<
  *     elif cmd == IOCTL_Commands.GET_SECTOR_COUNT:
  *         (<DWORD*> buff)[0] = drive.ioctl_get_sector_count()
  */
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_drive, __pyx_n_s_ioctl_sync); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
@@ -2643,25 +2672,25 @@
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "wrapper.pyx":48
+    /* "fatfs/wrapper.pyx":48
  *     drive = __diskio_wrapper_disks[pdrv]
  * 
  *     if cmd == IOCTL_Commands.CTRL_SYNC:             # <<<<<<<<<<<<<<
  *         drive.ioctl_sync()
  *     elif cmd == IOCTL_Commands.GET_SECTOR_COUNT:
  */
     break;
     case __pyx_e_5fatfs_6diskio_GET_SECTOR_COUNT:
 
-    /* "wrapper.pyx":51
+    /* "fatfs/wrapper.pyx":51
  *         drive.ioctl_sync()
  *     elif cmd == IOCTL_Commands.GET_SECTOR_COUNT:
  *         (<DWORD*> buff)[0] = drive.ioctl_get_sector_count()             # <<<<<<<<<<<<<<
  *     elif cmd == IOCTL_Commands.GET_SECTOR_SIZE:
  *         (<WORD*> buff)[0] = drive.ioctl_get_sector_size()
  */
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_drive, __pyx_n_s_ioctl_get_sector_count); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
@@ -2681,25 +2710,25 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_t_1); if (unlikely((__pyx_t_6 == ((DWORD)-1)) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     (((DWORD *)__pyx_v_buff)[0]) = __pyx_t_6;
 
-    /* "wrapper.pyx":50
+    /* "fatfs/wrapper.pyx":50
  *     if cmd == IOCTL_Commands.CTRL_SYNC:
  *         drive.ioctl_sync()
  *     elif cmd == IOCTL_Commands.GET_SECTOR_COUNT:             # <<<<<<<<<<<<<<
  *         (<DWORD*> buff)[0] = drive.ioctl_get_sector_count()
  *     elif cmd == IOCTL_Commands.GET_SECTOR_SIZE:
  */
     break;
     case __pyx_e_5fatfs_6diskio_GET_SECTOR_SIZE:
 
-    /* "wrapper.pyx":53
+    /* "fatfs/wrapper.pyx":53
  *         (<DWORD*> buff)[0] = drive.ioctl_get_sector_count()
  *     elif cmd == IOCTL_Commands.GET_SECTOR_SIZE:
  *         (<WORD*> buff)[0] = drive.ioctl_get_sector_size()             # <<<<<<<<<<<<<<
  *     elif cmd == IOCTL_Commands.GET_BLOCK_SIZE:
  *         (<DWORD*> buff)[0] = drive.ioctl_get_block_size()
  */
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_drive, __pyx_n_s_ioctl_get_sector_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
@@ -2719,25 +2748,25 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_t_1); if (unlikely((__pyx_t_7 == ((WORD)-1)) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     (((WORD *)__pyx_v_buff)[0]) = __pyx_t_7;
 
-    /* "wrapper.pyx":52
+    /* "fatfs/wrapper.pyx":52
  *     elif cmd == IOCTL_Commands.GET_SECTOR_COUNT:
  *         (<DWORD*> buff)[0] = drive.ioctl_get_sector_count()
  *     elif cmd == IOCTL_Commands.GET_SECTOR_SIZE:             # <<<<<<<<<<<<<<
  *         (<WORD*> buff)[0] = drive.ioctl_get_sector_size()
  *     elif cmd == IOCTL_Commands.GET_BLOCK_SIZE:
  */
     break;
     case __pyx_e_5fatfs_6diskio_GET_BLOCK_SIZE:
 
-    /* "wrapper.pyx":55
+    /* "fatfs/wrapper.pyx":55
  *         (<WORD*> buff)[0] = drive.ioctl_get_sector_size()
  *     elif cmd == IOCTL_Commands.GET_BLOCK_SIZE:
  *         (<DWORD*> buff)[0] = drive.ioctl_get_block_size()             # <<<<<<<<<<<<<<
  *     else:
  *         print("Unknown ioctl command %d." % cmd)
  */
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_drive, __pyx_n_s_ioctl_get_block_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
@@ -2757,25 +2786,25 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_t_1); if (unlikely((__pyx_t_6 == ((DWORD)-1)) && PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     (((DWORD *)__pyx_v_buff)[0]) = __pyx_t_6;
 
-    /* "wrapper.pyx":54
+    /* "fatfs/wrapper.pyx":54
  *     elif cmd == IOCTL_Commands.GET_SECTOR_SIZE:
  *         (<WORD*> buff)[0] = drive.ioctl_get_sector_size()
  *     elif cmd == IOCTL_Commands.GET_BLOCK_SIZE:             # <<<<<<<<<<<<<<
  *         (<DWORD*> buff)[0] = drive.ioctl_get_block_size()
  *     else:
  */
     break;
     default:
 
-    /* "wrapper.pyx":57
+    /* "fatfs/wrapper.pyx":57
  *         (<DWORD*> buff)[0] = drive.ioctl_get_block_size()
  *     else:
  *         print("Unknown ioctl command %d." % cmd)             # <<<<<<<<<<<<<<
  *         return DRESULT.RES_ERROR
  * 
  */
     __pyx_t_1 = __Pyx_PyInt_From_BYTE(__pyx_v_cmd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
@@ -2784,27 +2813,27 @@
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "wrapper.pyx":58
+    /* "fatfs/wrapper.pyx":58
  *     else:
  *         print("Unknown ioctl command %d." % cmd)
  *         return DRESULT.RES_ERROR             # <<<<<<<<<<<<<<
  * 
  * cdef extern int diskiocheck()
  */
     __pyx_r = RES_ERROR;
     goto __pyx_L0;
     break;
   }
 
-  /* "wrapper.pyx":43
+  /* "fatfs/wrapper.pyx":43
  *     return DRESULT.RES_OK
  * 
  * cdef DRESULT disk_ioctl (BYTE pdrv, BYTE cmd, void* buff):             # <<<<<<<<<<<<<<
  *     if not pdrv in __diskio_wrapper_disks:
  *         return DRESULT.RES_NOTRDY
  */
 
@@ -2819,15 +2848,15 @@
   __pyx_r = (DRESULT) 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_drive);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":67
+/* "fatfs/wrapper.pyx":67
  *     DWORD get_fattime()
  * 
  * cdef DWORD get_fattime():             # <<<<<<<<<<<<<<
  *     t = datetime.datetime.now()
  *     return ((t.year - 1980) << 25) | (t.month << 21) | (t.day << 16) | (t.minute << 5) | int(t.second / 2)
  */
 
@@ -2840,15 +2869,15 @@
   PyObject *__pyx_t_3 = NULL;
   DWORD __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_fattime", 0);
 
-  /* "wrapper.pyx":68
+  /* "fatfs/wrapper.pyx":68
  * 
  * cdef DWORD get_fattime():
  *     t = datetime.datetime.now()             # <<<<<<<<<<<<<<
  *     return ((t.year - 1980) << 25) | (t.month << 21) | (t.day << 16) | (t.minute << 5) | int(t.second / 2)
  *     # Return Value
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
@@ -2873,15 +2902,15 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_t = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":69
+  /* "fatfs/wrapper.pyx":69
  * cdef DWORD get_fattime():
  *     t = datetime.datetime.now()
  *     return ((t.year - 1980) << 25) | (t.month << 21) | (t.day << 16) | (t.minute << 5) | int(t.second / 2)             # <<<<<<<<<<<<<<
  *     # Return Value
  *     # Currnet local time shall be returned as bit-fields packed into a DWORD value. The bit fields are as follows:
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_t, __pyx_n_s_year); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
@@ -2932,120 +2961,120 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_4 == ((DWORD)-1)) && PyErr_Occurred())) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":67
+  /* "fatfs/wrapper.pyx":67
  *     DWORD get_fattime()
  * 
  * cdef DWORD get_fattime():             # <<<<<<<<<<<<<<
  *     t = datetime.datetime.now()
  *     return ((t.year - 1980) << 25) | (t.month << 21) | (t.day << 16) | (t.minute << 5) | int(t.second / 2)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_WriteUnraisable("wrapper.get_fattime", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("fatfs.wrapper.get_fattime", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":109
+/* "fatfs/wrapper.pyx":109
  * cdef class FIL_Handle:
  *     cdef FIL *fp
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.fp = <FIL*> PyMem_Malloc(sizeof(FIL))
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_7wrapper_10FIL_Handle_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_7wrapper_10FIL_Handle_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_5fatfs_7wrapper_10FIL_Handle_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_5fatfs_7wrapper_10FIL_Handle_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
     __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return -1;}
   if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
-  __pyx_r = __pyx_pf_7wrapper_10FIL_Handle___cinit__(((struct __pyx_obj_7wrapper_FIL_Handle *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FIL_Handle___cinit__(((struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7wrapper_10FIL_Handle___cinit__(struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_self) {
+static int __pyx_pf_5fatfs_7wrapper_10FIL_Handle___cinit__(struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "wrapper.pyx":110
+  /* "fatfs/wrapper.pyx":110
  *     cdef FIL *fp
  *     def __cinit__(self):
  *         self.fp = <FIL*> PyMem_Malloc(sizeof(FIL))             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __pyx_v_self->fp = ((FIL *)PyMem_Malloc((sizeof(FIL))));
 
-  /* "wrapper.pyx":109
+  /* "fatfs/wrapper.pyx":109
  * cdef class FIL_Handle:
  *     cdef FIL *fp
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.fp = <FIL*> PyMem_Malloc(sizeof(FIL))
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":112
+/* "fatfs/wrapper.pyx":112
  *         self.fp = <FIL*> PyMem_Malloc(sizeof(FIL))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         PyMem_Free(self.fp)
  * 
  */
 
 /* Python wrapper */
-static void __pyx_pw_7wrapper_10FIL_Handle_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_7wrapper_10FIL_Handle_3__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_5fatfs_7wrapper_10FIL_Handle_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_5fatfs_7wrapper_10FIL_Handle_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_7wrapper_10FIL_Handle_2__dealloc__(((struct __pyx_obj_7wrapper_FIL_Handle *)__pyx_v_self));
+  __pyx_pf_5fatfs_7wrapper_10FIL_Handle_2__dealloc__(((struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_7wrapper_10FIL_Handle_2__dealloc__(struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_self) {
+static void __pyx_pf_5fatfs_7wrapper_10FIL_Handle_2__dealloc__(struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "wrapper.pyx":113
+  /* "fatfs/wrapper.pyx":113
  * 
  *     def __dealloc__(self):
  *         PyMem_Free(self.fp)             # <<<<<<<<<<<<<<
  * 
  * cdef class FATFS_Handle:
  */
   PyMem_Free(__pyx_v_self->fp);
 
-  /* "wrapper.pyx":112
+  /* "fatfs/wrapper.pyx":112
  *         self.fp = <FIL*> PyMem_Malloc(sizeof(FIL))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         PyMem_Free(self.fp)
  * 
  */
 
@@ -3056,28 +3085,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_10FIL_Handle_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_7wrapper_10FIL_Handle_4__reduce_cython__[] = "FIL_Handle.__reduce_cython__(self)";
-static PyObject *__pyx_pw_7wrapper_10FIL_Handle_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FIL_Handle_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FIL_Handle_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_10FIL_Handle_4__reduce_cython__(((struct __pyx_obj_7wrapper_FIL_Handle *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FIL_Handle_4__reduce_cython__(((struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FIL_Handle_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FIL_Handle_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -3099,43 +3127,42 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.FIL_Handle.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FIL_Handle.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
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
-static PyObject *__pyx_pw_7wrapper_10FIL_Handle_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_7wrapper_10FIL_Handle_6__setstate_cython__[] = "FIL_Handle.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_7wrapper_10FIL_Handle_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FIL_Handle_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FIL_Handle_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_10FIL_Handle_6__setstate_cython__(((struct __pyx_obj_7wrapper_FIL_Handle *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FIL_Handle_6__setstate_cython__(((struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FIL_Handle_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FIL_Handle_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -3157,106 +3184,106 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.FIL_Handle.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FIL_Handle.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":117
+/* "fatfs/wrapper.pyx":117
  * cdef class FATFS_Handle:
  *     cdef FATFS* fp
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.fp = <FATFS*> PyMem_Malloc(sizeof(FATFS))
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_7wrapper_12FATFS_Handle_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_7wrapper_12FATFS_Handle_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_5fatfs_7wrapper_12FATFS_Handle_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_5fatfs_7wrapper_12FATFS_Handle_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
     __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return -1;}
   if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
-  __pyx_r = __pyx_pf_7wrapper_12FATFS_Handle___cinit__(((struct __pyx_obj_7wrapper_FATFS_Handle *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_12FATFS_Handle___cinit__(((struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7wrapper_12FATFS_Handle___cinit__(struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_self) {
+static int __pyx_pf_5fatfs_7wrapper_12FATFS_Handle___cinit__(struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "wrapper.pyx":118
+  /* "fatfs/wrapper.pyx":118
  *     cdef FATFS* fp
  *     def __cinit__(self):
  *         self.fp = <FATFS*> PyMem_Malloc(sizeof(FATFS))             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __pyx_v_self->fp = ((FATFS *)PyMem_Malloc((sizeof(FATFS))));
 
-  /* "wrapper.pyx":117
+  /* "fatfs/wrapper.pyx":117
  * cdef class FATFS_Handle:
  *     cdef FATFS* fp
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.fp = <FATFS*> PyMem_Malloc(sizeof(FATFS))
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":120
+/* "fatfs/wrapper.pyx":120
  *         self.fp = <FATFS*> PyMem_Malloc(sizeof(FATFS))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         PyMem_Free(self.fp)
  * 
  */
 
 /* Python wrapper */
-static void __pyx_pw_7wrapper_12FATFS_Handle_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_7wrapper_12FATFS_Handle_3__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_5fatfs_7wrapper_12FATFS_Handle_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_5fatfs_7wrapper_12FATFS_Handle_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_7wrapper_12FATFS_Handle_2__dealloc__(((struct __pyx_obj_7wrapper_FATFS_Handle *)__pyx_v_self));
+  __pyx_pf_5fatfs_7wrapper_12FATFS_Handle_2__dealloc__(((struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_7wrapper_12FATFS_Handle_2__dealloc__(struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_self) {
+static void __pyx_pf_5fatfs_7wrapper_12FATFS_Handle_2__dealloc__(struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "wrapper.pyx":121
+  /* "fatfs/wrapper.pyx":121
  * 
  *     def __dealloc__(self):
  *         PyMem_Free(self.fp)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   PyMem_Free(__pyx_v_self->fp);
 
-  /* "wrapper.pyx":120
+  /* "fatfs/wrapper.pyx":120
  *         self.fp = <FATFS*> PyMem_Malloc(sizeof(FATFS))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         PyMem_Free(self.fp)
  * 
  */
 
@@ -3267,28 +3294,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_12FATFS_Handle_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_7wrapper_12FATFS_Handle_4__reduce_cython__[] = "FATFS_Handle.__reduce_cython__(self)";
-static PyObject *__pyx_pw_7wrapper_12FATFS_Handle_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_12FATFS_Handle_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_5fatfs_7wrapper_12FATFS_Handle_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_12FATFS_Handle_4__reduce_cython__(((struct __pyx_obj_7wrapper_FATFS_Handle *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_12FATFS_Handle_4__reduce_cython__(((struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_12FATFS_Handle_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_12FATFS_Handle_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -3310,43 +3336,42 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.FATFS_Handle.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FATFS_Handle.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
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
-static PyObject *__pyx_pw_7wrapper_12FATFS_Handle_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_7wrapper_12FATFS_Handle_6__setstate_cython__[] = "FATFS_Handle.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_7wrapper_12FATFS_Handle_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_12FATFS_Handle_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_5fatfs_7wrapper_12FATFS_Handle_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_12FATFS_Handle_6__setstate_cython__(((struct __pyx_obj_7wrapper_FATFS_Handle *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_12FATFS_Handle_6__setstate_cython__(((struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_12FATFS_Handle_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_12FATFS_Handle_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -3368,35 +3393,34 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.FATFS_Handle.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FATFS_Handle.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":125
+/* "fatfs/wrapper.pyx":125
  * 
  * # Open or create a file
  * def pyf_open (FIL_Handle fph, const TCHAR* path, BYTE mode) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_open(fph.fp, path, mode)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_1pyf_open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_pyf_open[] = "pyf_open(FIL_Handle fph, const TCHAR *path, BYTE mode) -> FRESULT";
-static PyMethodDef __pyx_mdef_7wrapper_1pyf_open = {"pyf_open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_1pyf_open, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_pyf_open};
-static PyObject *__pyx_pw_7wrapper_1pyf_open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_fph = 0;
+static PyObject *__pyx_pw_5fatfs_7wrapper_1pyf_open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_1pyf_open = {"pyf_open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_1pyf_open, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_1pyf_open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_fph = 0;
   TCHAR const *__pyx_v_path;
   BYTE __pyx_v_mode;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3441,167 +3465,165 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_fph = ((struct __pyx_obj_7wrapper_FIL_Handle *)values[0]);
+    __pyx_v_fph = ((struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *)values[0]);
     __pyx_v_path = __Pyx_PyObject_AsString(values[1]); if (unlikely((!__pyx_v_path) && PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L3_error)
     __pyx_v_mode = __Pyx_PyInt_As_BYTE(values[2]); if (unlikely((__pyx_v_mode == ((BYTE)-1)) && PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pyf_open", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.pyf_open", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fph), __pyx_ptype_7wrapper_FIL_Handle, 1, "fph", 0))) __PYX_ERR(0, 125, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7wrapper_pyf_open(__pyx_self, __pyx_v_fph, __pyx_v_path, __pyx_v_mode);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fph), __pyx_ptype_5fatfs_7wrapper_FIL_Handle, 1, "fph", 0))) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_pyf_open(__pyx_self, __pyx_v_fph, __pyx_v_path, __pyx_v_mode);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_pyf_open(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_fph, TCHAR const *__pyx_v_path, BYTE __pyx_v_mode) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_pyf_open(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_fph, TCHAR const *__pyx_v_path, BYTE __pyx_v_mode) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyf_open", 0);
 
-  /* "wrapper.pyx":126
+  /* "fatfs/wrapper.pyx":126
  * # Open or create a file
  * def pyf_open (FIL_Handle fph, const TCHAR* path, BYTE mode) -> FRESULT:
  *     return f_open(fph.fp, path, mode)             # <<<<<<<<<<<<<<
  * 
  * # Close an open file object
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_FRESULT(f_open(__pyx_v_fph->fp, __pyx_v_path, __pyx_v_mode)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":125
+  /* "fatfs/wrapper.pyx":125
  * 
  * # Open or create a file
  * def pyf_open (FIL_Handle fph, const TCHAR* path, BYTE mode) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_open(fph.fp, path, mode)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.pyf_open", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":129
+/* "fatfs/wrapper.pyx":129
  * 
  * # Close an open file object
  * def pyf_close (FIL_Handle fph) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_close(fph.fp)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_3pyf_close(PyObject *__pyx_self, PyObject *__pyx_v_fph); /*proto*/
-static char __pyx_doc_7wrapper_2pyf_close[] = "pyf_close(FIL_Handle fph) -> FRESULT";
-static PyMethodDef __pyx_mdef_7wrapper_3pyf_close = {"pyf_close", (PyCFunction)__pyx_pw_7wrapper_3pyf_close, METH_O, __pyx_doc_7wrapper_2pyf_close};
-static PyObject *__pyx_pw_7wrapper_3pyf_close(PyObject *__pyx_self, PyObject *__pyx_v_fph) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_3pyf_close(PyObject *__pyx_self, PyObject *__pyx_v_fph); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_3pyf_close = {"pyf_close", (PyCFunction)__pyx_pw_5fatfs_7wrapper_3pyf_close, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_3pyf_close(PyObject *__pyx_self, PyObject *__pyx_v_fph) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pyf_close (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fph), __pyx_ptype_7wrapper_FIL_Handle, 1, "fph", 0))) __PYX_ERR(0, 129, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7wrapper_2pyf_close(__pyx_self, ((struct __pyx_obj_7wrapper_FIL_Handle *)__pyx_v_fph));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fph), __pyx_ptype_5fatfs_7wrapper_FIL_Handle, 1, "fph", 0))) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_2pyf_close(__pyx_self, ((struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *)__pyx_v_fph));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_2pyf_close(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_fph) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_2pyf_close(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_fph) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyf_close", 0);
 
-  /* "wrapper.pyx":130
+  /* "fatfs/wrapper.pyx":130
  * # Close an open file object
  * def pyf_close (FIL_Handle fph) -> FRESULT:
  *     return f_close(fph.fp)             # <<<<<<<<<<<<<<
  * 
  * # Read data from the file
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_FRESULT(f_close(__pyx_v_fph->fp)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":129
+  /* "fatfs/wrapper.pyx":129
  * 
  * # Close an open file object
  * def pyf_close (FIL_Handle fph) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_close(fph.fp)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.pyf_close", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":136
+/* "fatfs/wrapper.pyx":136
  * #    raise Exception("Not implemented.")
  * ## Write data to the file
  * def pyf_write (FIL_Handle fph, data) -> FRESULT:             # <<<<<<<<<<<<<<
  *     assert isinstance(data, (bytes, bytearray))
  *     cdef UINT written
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_5pyf_write(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_4pyf_write[] = "pyf_write(FIL_Handle fph, data) -> FRESULT";
-static PyMethodDef __pyx_mdef_7wrapper_5pyf_write = {"pyf_write", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_5pyf_write, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_4pyf_write};
-static PyObject *__pyx_pw_7wrapper_5pyf_write(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_fph = 0;
+static PyObject *__pyx_pw_5fatfs_7wrapper_5pyf_write(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_5pyf_write = {"pyf_write", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_5pyf_write, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_5pyf_write(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_fph = 0;
   PyObject *__pyx_v_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pyf_write (wrapper)", 0);
@@ -3636,38 +3658,38 @@
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_fph = ((struct __pyx_obj_7wrapper_FIL_Handle *)values[0]);
+    __pyx_v_fph = ((struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *)values[0]);
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pyf_write", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 136, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.pyf_write", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fph), __pyx_ptype_7wrapper_FIL_Handle, 1, "fph", 0))) __PYX_ERR(0, 136, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7wrapper_4pyf_write(__pyx_self, __pyx_v_fph, __pyx_v_data);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fph), __pyx_ptype_5fatfs_7wrapper_FIL_Handle, 1, "fph", 0))) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_4pyf_write(__pyx_self, __pyx_v_fph, __pyx_v_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_4pyf_write(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7wrapper_FIL_Handle *__pyx_v_fph, PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_4pyf_write(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5fatfs_7wrapper_FIL_Handle *__pyx_v_fph, PyObject *__pyx_v_data) {
   UINT __pyx_v_written;
   char *__pyx_v_dataptr;
   FRESULT __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
@@ -3681,15 +3703,15 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyf_write", 0);
 
-  /* "wrapper.pyx":137
+  /* "fatfs/wrapper.pyx":137
  * ## Write data to the file
  * def pyf_write (FIL_Handle fph, data) -> FRESULT:
  *     assert isinstance(data, (bytes, bytearray))             # <<<<<<<<<<<<<<
  *     cdef UINT written
  *     cdef char* dataptr = data
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
@@ -3708,45 +3730,45 @@
     if (unlikely(!(__pyx_t_1 != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 137, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "wrapper.pyx":139
+  /* "fatfs/wrapper.pyx":139
  *     assert isinstance(data, (bytes, bytearray))
  *     cdef UINT written
  *     cdef char* dataptr = data             # <<<<<<<<<<<<<<
  *     ret = f_write(fph.fp, <void*>dataptr, len(data), &written)
  *     if ret != FR_OK:
  */
   __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L1_error)
   __pyx_v_dataptr = __pyx_t_4;
 
-  /* "wrapper.pyx":140
+  /* "fatfs/wrapper.pyx":140
  *     cdef UINT written
  *     cdef char* dataptr = data
  *     ret = f_write(fph.fp, <void*>dataptr, len(data), &written)             # <<<<<<<<<<<<<<
  *     if ret != FR_OK:
  *         raise FatFSException("write", ret, fph, data)
  */
   __pyx_t_5 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 140, __pyx_L1_error)
   __pyx_v_ret = f_write(__pyx_v_fph->fp, ((void *)__pyx_v_dataptr), __pyx_t_5, (&__pyx_v_written));
 
-  /* "wrapper.pyx":141
+  /* "fatfs/wrapper.pyx":141
  *     cdef char* dataptr = data
  *     ret = f_write(fph.fp, <void*>dataptr, len(data), &written)
  *     if ret != FR_OK:             # <<<<<<<<<<<<<<
  *         raise FatFSException("write", ret, fph, data)
  *     assert((ret != FR_OK) or (written == len(data)), "FatFS::write succeeded, but written different %i bytes out of %i." % (written, len(data)))
  */
   __pyx_t_1 = ((__pyx_v_ret != FR_OK) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "wrapper.pyx":142
+    /* "fatfs/wrapper.pyx":142
  *     ret = f_write(fph.fp, <void*>dataptr, len(data), &written)
  *     if ret != FR_OK:
  *         raise FatFSException("write", ret, fph, data)             # <<<<<<<<<<<<<<
  *     assert((ret != FR_OK) or (written == len(data)), "FatFS::write succeeded, but written different %i bytes out of %i." % (written, len(data)))
  *     return ret, written
  */
     __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_FatFSException); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 142, __pyx_L1_error)
@@ -3806,24 +3828,24 @@
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     }
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __PYX_ERR(0, 142, __pyx_L1_error)
 
-    /* "wrapper.pyx":141
+    /* "fatfs/wrapper.pyx":141
  *     cdef char* dataptr = data
  *     ret = f_write(fph.fp, <void*>dataptr, len(data), &written)
  *     if ret != FR_OK:             # <<<<<<<<<<<<<<
  *         raise FatFSException("write", ret, fph, data)
  *     assert((ret != FR_OK) or (written == len(data)), "FatFS::write succeeded, but written different %i bytes out of %i." % (written, len(data)))
  */
   }
 
-  /* "wrapper.pyx":143
+  /* "fatfs/wrapper.pyx":143
  *     if ret != FR_OK:
  *         raise FatFSException("write", ret, fph, data)
  *     assert((ret != FR_OK) or (written == len(data)), "FatFS::write succeeded, but written different %i bytes out of %i." % (written, len(data)))             # <<<<<<<<<<<<<<
  *     return ret, written
  * ## Move file pointer of the file object
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
@@ -3873,15 +3895,15 @@
     if (unlikely(!__pyx_t_1)) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 143, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "wrapper.pyx":144
+  /* "fatfs/wrapper.pyx":144
  *         raise FatFSException("write", ret, fph, data)
  *     assert((ret != FR_OK) or (written == len(data)), "FatFS::write succeeded, but written different %i bytes out of %i." % (written, len(data)))
  *     return ret, written             # <<<<<<<<<<<<<<
  * ## Move file pointer of the file object
  * #def pyf_lseek (FIL* fp, FSIZE_t ofs) -> FRESULT:
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3897,118 +3919,116 @@
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_11);
   __pyx_t_8 = 0;
   __pyx_t_11 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":136
+  /* "fatfs/wrapper.pyx":136
  * #    raise Exception("Not implemented.")
  * ## Write data to the file
  * def pyf_write (FIL_Handle fph, data) -> FRESULT:             # <<<<<<<<<<<<<<
  *     assert isinstance(data, (bytes, bytearray))
  *     cdef UINT written
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_AddTraceback("wrapper.pyf_write", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":170
+/* "fatfs/wrapper.pyx":170
  * #    raise Exception("Not implemented.")
  * ## Create a sub directory
  * def pyf_mkdir (path) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_mkdir(path)
  * ## Delete an existing file or directory
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_7pyf_mkdir(PyObject *__pyx_self, PyObject *__pyx_v_path); /*proto*/
-static char __pyx_doc_7wrapper_6pyf_mkdir[] = "pyf_mkdir(path) -> FRESULT";
-static PyMethodDef __pyx_mdef_7wrapper_7pyf_mkdir = {"pyf_mkdir", (PyCFunction)__pyx_pw_7wrapper_7pyf_mkdir, METH_O, __pyx_doc_7wrapper_6pyf_mkdir};
-static PyObject *__pyx_pw_7wrapper_7pyf_mkdir(PyObject *__pyx_self, PyObject *__pyx_v_path) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_7pyf_mkdir(PyObject *__pyx_self, PyObject *__pyx_v_path); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_7pyf_mkdir = {"pyf_mkdir", (PyCFunction)__pyx_pw_5fatfs_7wrapper_7pyf_mkdir, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_7pyf_mkdir(PyObject *__pyx_self, PyObject *__pyx_v_path) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pyf_mkdir (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_6pyf_mkdir(__pyx_self, ((PyObject *)__pyx_v_path));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_6pyf_mkdir(__pyx_self, ((PyObject *)__pyx_v_path));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_6pyf_mkdir(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_6pyf_mkdir(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   TCHAR const *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyf_mkdir", 0);
 
-  /* "wrapper.pyx":171
+  /* "fatfs/wrapper.pyx":171
  * ## Create a sub directory
  * def pyf_mkdir (path) -> FRESULT:
  *     return f_mkdir(path)             # <<<<<<<<<<<<<<
  * ## Delete an existing file or directory
  * #def pyf_unlink (const TCHAR* path) -> FRESULT:
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyObject_AsString(__pyx_v_path); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L1_error)
   __pyx_t_2 = __Pyx_PyInt_From_FRESULT(f_mkdir(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":170
+  /* "fatfs/wrapper.pyx":170
  * #    raise Exception("Not implemented.")
  * ## Create a sub directory
  * def pyf_mkdir (path) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_mkdir(path)
  * ## Delete an existing file or directory
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("wrapper.pyf_mkdir", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_mkdir", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":212
+/* "fatfs/wrapper.pyx":212
  * #    raise Exception("Not implemented.")
  * # Mount/Unmount a logical drive
  * def pyf_mount (FATFS_Handle fph, const TCHAR* path, BYTE opt) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_mount(fph.fp, path, opt)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_9pyf_mount(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_8pyf_mount[] = "pyf_mount(FATFS_Handle fph, const TCHAR *path, BYTE opt) -> FRESULT";
-static PyMethodDef __pyx_mdef_7wrapper_9pyf_mount = {"pyf_mount", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_9pyf_mount, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_8pyf_mount};
-static PyObject *__pyx_pw_7wrapper_9pyf_mount(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_fph = 0;
+static PyObject *__pyx_pw_5fatfs_7wrapper_9pyf_mount(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_9pyf_mount = {"pyf_mount", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_9pyf_mount, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_9pyf_mount(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_fph = 0;
   TCHAR const *__pyx_v_path;
   BYTE __pyx_v_opt;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4053,93 +4073,93 @@
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_fph = ((struct __pyx_obj_7wrapper_FATFS_Handle *)values[0]);
+    __pyx_v_fph = ((struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *)values[0]);
     __pyx_v_path = __Pyx_PyObject_AsString(values[1]); if (unlikely((!__pyx_v_path) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L3_error)
     __pyx_v_opt = __Pyx_PyInt_As_BYTE(values[2]); if (unlikely((__pyx_v_opt == ((BYTE)-1)) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pyf_mount", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 212, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.pyf_mount", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_mount", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fph), __pyx_ptype_7wrapper_FATFS_Handle, 1, "fph", 0))) __PYX_ERR(0, 212, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7wrapper_8pyf_mount(__pyx_self, __pyx_v_fph, __pyx_v_path, __pyx_v_opt);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fph), __pyx_ptype_5fatfs_7wrapper_FATFS_Handle, 1, "fph", 0))) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_8pyf_mount(__pyx_self, __pyx_v_fph, __pyx_v_path, __pyx_v_opt);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_8pyf_mount(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7wrapper_FATFS_Handle *__pyx_v_fph, TCHAR const *__pyx_v_path, BYTE __pyx_v_opt) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_8pyf_mount(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle *__pyx_v_fph, TCHAR const *__pyx_v_path, BYTE __pyx_v_opt) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyf_mount", 0);
 
-  /* "wrapper.pyx":213
+  /* "fatfs/wrapper.pyx":213
  * # Mount/Unmount a logical drive
  * def pyf_mount (FATFS_Handle fph, const TCHAR* path, BYTE opt) -> FRESULT:
  *     return f_mount(fph.fp, path, opt)             # <<<<<<<<<<<<<<
  * 
  * # Create a FAT volume
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_FRESULT(f_mount(__pyx_v_fph->fp, __pyx_v_path, __pyx_v_opt)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":212
+  /* "fatfs/wrapper.pyx":212
  * #    raise Exception("Not implemented.")
  * # Mount/Unmount a logical drive
  * def pyf_mount (FATFS_Handle fph, const TCHAR* path, BYTE opt) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_mount(fph.fp, path, opt)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.pyf_mount", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_mount", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":216
+/* "fatfs/wrapper.pyx":216
  * 
  * # Create a FAT volume
  * def pyf_mkfs (path, n_fat = 1, align = 0, n_root = 0, au_size = 0, workarea_size = 512) -> FRESULT:             # <<<<<<<<<<<<<<
  *     """
  *     Create a new FAT filesystem on volum given in path. The optional parameters
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_11pyf_mkfs(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_10pyf_mkfs[] = "pyf_mkfs(path, n_fat=1, align=0, n_root=0, au_size=0, workarea_size=512) -> FRESULT\n\n    Create a new FAT filesystem on volum given in path. The optional parameters\n    are passed to FATFS as is. Defaults will create filesystem with 1 FAT\n    table, auto alignment probed from backing device, automatically choose\n    number of rot entries and allocation unit size.\n    ";
-static PyMethodDef __pyx_mdef_7wrapper_11pyf_mkfs = {"pyf_mkfs", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_11pyf_mkfs, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_10pyf_mkfs};
-static PyObject *__pyx_pw_7wrapper_11pyf_mkfs(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_11pyf_mkfs(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_5fatfs_7wrapper_10pyf_mkfs[] = "\n    Create a new FAT filesystem on volum given in path. The optional parameters\n    are passed to FATFS as is. Defaults will create filesystem with 1 FAT\n    table, auto alignment probed from backing device, automatically choose\n    number of rot entries and allocation unit size.\n    ";
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_11pyf_mkfs = {"pyf_mkfs", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_11pyf_mkfs, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5fatfs_7wrapper_10pyf_mkfs};
+static PyObject *__pyx_pw_5fatfs_7wrapper_11pyf_mkfs(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_path = 0;
   PyObject *__pyx_v_n_fat = 0;
   PyObject *__pyx_v_align = 0;
   PyObject *__pyx_v_n_root = 0;
   PyObject *__pyx_v_au_size = 0;
   PyObject *__pyx_v_workarea_size = 0;
   int __pyx_lineno = 0;
@@ -4238,26 +4258,26 @@
     __pyx_v_au_size = values[4];
     __pyx_v_workarea_size = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pyf_mkfs", 0, 1, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 216, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.pyf_mkfs", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_mkfs", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_10pyf_mkfs(__pyx_self, __pyx_v_path, __pyx_v_n_fat, __pyx_v_align, __pyx_v_n_root, __pyx_v_au_size, __pyx_v_workarea_size);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10pyf_mkfs(__pyx_self, __pyx_v_path, __pyx_v_n_fat, __pyx_v_align, __pyx_v_n_root, __pyx_v_au_size, __pyx_v_workarea_size);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10pyf_mkfs(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path, PyObject *__pyx_v_n_fat, PyObject *__pyx_v_align, PyObject *__pyx_v_n_root, PyObject *__pyx_v_au_size, PyObject *__pyx_v_workarea_size) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10pyf_mkfs(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_path, PyObject *__pyx_v_n_fat, PyObject *__pyx_v_align, PyObject *__pyx_v_n_root, PyObject *__pyx_v_au_size, PyObject *__pyx_v_workarea_size) {
   char *__pyx_v_buff;
   MKFS_PARM __pyx_v_opt;
   FRESULT __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
   BYTE __pyx_t_2;
@@ -4266,203 +4286,201 @@
   TCHAR const *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyf_mkfs", 0);
 
-  /* "wrapper.pyx":223
+  /* "fatfs/wrapper.pyx":223
  *     number of rot entries and allocation unit size.
  *     """
  *     cdef char* buff = <char*> PyMem_Malloc(workarea_size)             # <<<<<<<<<<<<<<
  *     cdef MKFS_PARM opt
  *     opt.fmt = FM_FAT | FM_SFD
  */
   __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_workarea_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L1_error)
   __pyx_v_buff = ((char *)PyMem_Malloc(__pyx_t_1));
 
-  /* "wrapper.pyx":225
+  /* "fatfs/wrapper.pyx":225
  *     cdef char* buff = <char*> PyMem_Malloc(workarea_size)
  *     cdef MKFS_PARM opt
  *     opt.fmt = FM_FAT | FM_SFD             # <<<<<<<<<<<<<<
  *     opt.n_fat = n_fat # 1 copy of FAT table
  *     opt.align = align # auto align from lower layer
  */
   __pyx_v_opt.fmt = (FM_FAT | FM_SFD);
 
-  /* "wrapper.pyx":226
+  /* "fatfs/wrapper.pyx":226
  *     cdef MKFS_PARM opt
  *     opt.fmt = FM_FAT | FM_SFD
  *     opt.n_fat = n_fat # 1 copy of FAT table             # <<<<<<<<<<<<<<
  *     opt.align = align # auto align from lower layer
  *     opt.n_root = n_root # auto number of root FAT entries
  */
   __pyx_t_2 = __Pyx_PyInt_As_BYTE(__pyx_v_n_fat); if (unlikely((__pyx_t_2 == ((BYTE)-1)) && PyErr_Occurred())) __PYX_ERR(0, 226, __pyx_L1_error)
   __pyx_v_opt.n_fat = __pyx_t_2;
 
-  /* "wrapper.pyx":227
+  /* "fatfs/wrapper.pyx":227
  *     opt.fmt = FM_FAT | FM_SFD
  *     opt.n_fat = n_fat # 1 copy of FAT table
  *     opt.align = align # auto align from lower layer             # <<<<<<<<<<<<<<
  *     opt.n_root = n_root # auto number of root FAT entries
  *     opt.au_size = au_size # auto
  */
   __pyx_t_3 = __Pyx_PyInt_As_UINT(__pyx_v_align); if (unlikely((__pyx_t_3 == ((UINT)-1)) && PyErr_Occurred())) __PYX_ERR(0, 227, __pyx_L1_error)
   __pyx_v_opt.align = __pyx_t_3;
 
-  /* "wrapper.pyx":228
+  /* "fatfs/wrapper.pyx":228
  *     opt.n_fat = n_fat # 1 copy of FAT table
  *     opt.align = align # auto align from lower layer
  *     opt.n_root = n_root # auto number of root FAT entries             # <<<<<<<<<<<<<<
  *     opt.au_size = au_size # auto
  *     cdef FRESULT ret = f_mkfs(path, &opt, buff, 512)
  */
   __pyx_t_3 = __Pyx_PyInt_As_UINT(__pyx_v_n_root); if (unlikely((__pyx_t_3 == ((UINT)-1)) && PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L1_error)
   __pyx_v_opt.n_root = __pyx_t_3;
 
-  /* "wrapper.pyx":229
+  /* "fatfs/wrapper.pyx":229
  *     opt.align = align # auto align from lower layer
  *     opt.n_root = n_root # auto number of root FAT entries
  *     opt.au_size = au_size # auto             # <<<<<<<<<<<<<<
  *     cdef FRESULT ret = f_mkfs(path, &opt, buff, 512)
  *     PyMem_Free(buff)
  */
   __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_au_size); if (unlikely((__pyx_t_4 == ((DWORD)-1)) && PyErr_Occurred())) __PYX_ERR(0, 229, __pyx_L1_error)
   __pyx_v_opt.au_size = __pyx_t_4;
 
-  /* "wrapper.pyx":230
+  /* "fatfs/wrapper.pyx":230
  *     opt.n_root = n_root # auto number of root FAT entries
  *     opt.au_size = au_size # auto
  *     cdef FRESULT ret = f_mkfs(path, &opt, buff, 512)             # <<<<<<<<<<<<<<
  *     PyMem_Free(buff)
  *     return ret
  */
   __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_v_path); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L1_error)
   __pyx_v_ret = f_mkfs(__pyx_t_5, (&__pyx_v_opt), __pyx_v_buff, 0x200);
 
-  /* "wrapper.pyx":231
+  /* "fatfs/wrapper.pyx":231
  *     opt.au_size = au_size # auto
  *     cdef FRESULT ret = f_mkfs(path, &opt, buff, 512)
  *     PyMem_Free(buff)             # <<<<<<<<<<<<<<
  *     return ret
  * ## Divide a physical drive into some partitions
  */
   PyMem_Free(__pyx_v_buff);
 
-  /* "wrapper.pyx":232
+  /* "fatfs/wrapper.pyx":232
  *     cdef FRESULT ret = f_mkfs(path, &opt, buff, 512)
  *     PyMem_Free(buff)
  *     return ret             # <<<<<<<<<<<<<<
  * ## Divide a physical drive into some partitions
  * #def pyf_fdisk (BYTE pdrv, const LBA_t ptbl[], void* work) -> FRESULT:
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_6 = __Pyx_PyInt_From_FRESULT(__pyx_v_ret); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":216
+  /* "fatfs/wrapper.pyx":216
  * 
  * # Create a FAT volume
  * def pyf_mkfs (path, n_fat = 1, align = 0, n_root = 0, au_size = 0, workarea_size = 512) -> FRESULT:             # <<<<<<<<<<<<<<
  *     """
  *     Create a new FAT filesystem on volum given in path. The optional parameters
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("wrapper.pyf_mkfs", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.pyf_mkfs", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":255
+/* "fatfs/wrapper.pyx":255
  * from cpython.mem cimport PyMem_Malloc, PyMem_Realloc, PyMem_Free
  * 
  * def fresult_to_name(fresult):             # <<<<<<<<<<<<<<
  *     # TODO: Implement.
  *     return "UNKNOWN_%i" % fresult
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_13fresult_to_name(PyObject *__pyx_self, PyObject *__pyx_v_fresult); /*proto*/
-static char __pyx_doc_7wrapper_12fresult_to_name[] = "fresult_to_name(fresult)";
-static PyMethodDef __pyx_mdef_7wrapper_13fresult_to_name = {"fresult_to_name", (PyCFunction)__pyx_pw_7wrapper_13fresult_to_name, METH_O, __pyx_doc_7wrapper_12fresult_to_name};
-static PyObject *__pyx_pw_7wrapper_13fresult_to_name(PyObject *__pyx_self, PyObject *__pyx_v_fresult) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_13fresult_to_name(PyObject *__pyx_self, PyObject *__pyx_v_fresult); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_13fresult_to_name = {"fresult_to_name", (PyCFunction)__pyx_pw_5fatfs_7wrapper_13fresult_to_name, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_13fresult_to_name(PyObject *__pyx_self, PyObject *__pyx_v_fresult) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("fresult_to_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_12fresult_to_name(__pyx_self, ((PyObject *)__pyx_v_fresult));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_12fresult_to_name(__pyx_self, ((PyObject *)__pyx_v_fresult));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_12fresult_to_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fresult) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_12fresult_to_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fresult) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fresult_to_name", 0);
 
-  /* "wrapper.pyx":257
+  /* "fatfs/wrapper.pyx":257
  * def fresult_to_name(fresult):
  *     # TODO: Implement.
  *     return "UNKNOWN_%i" % fresult             # <<<<<<<<<<<<<<
  * 
  * class FatFSException(Exception):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_UNKNOWN__i, __pyx_v_fresult); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":255
+  /* "fatfs/wrapper.pyx":255
  * from cpython.mem cimport PyMem_Malloc, PyMem_Realloc, PyMem_Free
  * 
  * def fresult_to_name(fresult):             # <<<<<<<<<<<<<<
  *     # TODO: Implement.
  *     return "UNKNOWN_%i" % fresult
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.fresult_to_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.fresult_to_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":260
+/* "fatfs/wrapper.pyx":260
  * 
  * class FatFSException(Exception):
  *     def __init__(self, function, ret, *args):             # <<<<<<<<<<<<<<
  *         self.code = ret
  *         args_str = ", ".join(map(str, args))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_14FatFSException_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_14FatFSException___init__[] = "FatFSException.__init__(self, function, ret, *args)";
-static PyMethodDef __pyx_mdef_7wrapper_14FatFSException_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_14FatFSException_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_14FatFSException___init__};
-static PyObject *__pyx_pw_7wrapper_14FatFSException_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_14FatFSException_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_14FatFSException_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_14FatFSException_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_14FatFSException_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_function = 0;
   PyObject *__pyx_v_ret = 0;
   PyObject *__pyx_v_args = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -4529,27 +4547,27 @@
     __pyx_v_ret = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 0, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 260, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
-  __Pyx_AddTraceback("wrapper.FatFSException.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FatFSException.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_14FatFSException___init__(__pyx_self, __pyx_v_self, __pyx_v_function, __pyx_v_ret, __pyx_v_args);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_14FatFSException___init__(__pyx_self, __pyx_v_self, __pyx_v_function, __pyx_v_ret, __pyx_v_args);
 
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_args);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_14FatFSException___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_function, PyObject *__pyx_v_ret, PyObject *__pyx_v_args) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_14FatFSException___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_function, PyObject *__pyx_v_ret, PyObject *__pyx_v_args) {
   PyObject *__pyx_v_args_str = NULL;
   PyObject *__pyx_v_ret_str = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -4557,24 +4575,24 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "wrapper.pyx":261
+  /* "fatfs/wrapper.pyx":261
  * class FatFSException(Exception):
  *     def __init__(self, function, ret, *args):
  *         self.code = ret             # <<<<<<<<<<<<<<
  *         args_str = ", ".join(map(str, args))
  *         ret_str = fresult_to_name(ret)
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_code, __pyx_v_ret) < 0) __PYX_ERR(0, 261, __pyx_L1_error)
 
-  /* "wrapper.pyx":262
+  /* "fatfs/wrapper.pyx":262
  *     def __init__(self, function, ret, *args):
  *         self.code = ret
  *         args_str = ", ".join(map(str, args))             # <<<<<<<<<<<<<<
  *         ret_str = fresult_to_name(ret)
  *         Exception.__init__(self, "FatFS::%s(%s) failed with error code %i (%s)" % (function, args_str, ret, ret_str))
  */
   __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
@@ -4590,15 +4608,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_args_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":263
+  /* "fatfs/wrapper.pyx":263
  *         self.code = ret
  *         args_str = ", ".join(map(str, args))
  *         ret_str = fresult_to_name(ret)             # <<<<<<<<<<<<<<
  *         Exception.__init__(self, "FatFS::%s(%s) failed with error code %i (%s)" % (function, args_str, ret, ret_str))
  *     pass
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fresult_to_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
@@ -4617,15 +4635,15 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ret_str = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":264
+  /* "fatfs/wrapper.pyx":264
  *         args_str = ", ".join(map(str, args))
  *         ret_str = fresult_to_name(ret)
  *         Exception.__init__(self, "FatFS::%s(%s) failed with error code %i (%s)" % (function, args_str, ret, ret_str))             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
@@ -4692,15 +4710,15 @@
     __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":260
+  /* "fatfs/wrapper.pyx":260
  * 
  * class FatFSException(Exception):
  *     def __init__(self, function, ret, *args):             # <<<<<<<<<<<<<<
  *         self.code = ret
  *         args_str = ", ".join(map(str, args))
  */
 
@@ -4709,136 +4727,134 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("wrapper.FatFSException.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FatFSException.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_args_str);
   __Pyx_XDECREF(__pyx_v_ret_str);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":268
+/* "fatfs/wrapper.pyx":268
  * 
  * class FileHandle:
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.isopen = False
  *         self.fp = FIL_Handle()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_10FileHandle_1__init__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_7wrapper_10FileHandle___init__[] = "FileHandle.__init__(self)";
-static PyMethodDef __pyx_mdef_7wrapper_10FileHandle_1__init__ = {"__init__", (PyCFunction)__pyx_pw_7wrapper_10FileHandle_1__init__, METH_O, __pyx_doc_7wrapper_10FileHandle___init__};
-static PyObject *__pyx_pw_7wrapper_10FileHandle_1__init__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_1__init__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_10FileHandle_1__init__ = {"__init__", (PyCFunction)__pyx_pw_5fatfs_7wrapper_10FileHandle_1__init__, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_1__init__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_10FileHandle___init__(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FileHandle___init__(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FileHandle___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "wrapper.pyx":269
+  /* "fatfs/wrapper.pyx":269
  * class FileHandle:
  *     def __init__(self):
  *         self.isopen = False             # <<<<<<<<<<<<<<
  *         self.fp = FIL_Handle()
  * 
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_isopen, Py_False) < 0) __PYX_ERR(0, 269, __pyx_L1_error)
 
-  /* "wrapper.pyx":270
+  /* "fatfs/wrapper.pyx":270
  *     def __init__(self):
  *         self.isopen = False
  *         self.fp = FIL_Handle()             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_7wrapper_FIL_Handle)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5fatfs_7wrapper_FIL_Handle)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_fp, __pyx_t_1) < 0) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":268
+  /* "fatfs/wrapper.pyx":268
  * 
  * class FileHandle:
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.isopen = False
  *         self.fp = FIL_Handle()
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("wrapper.FileHandle.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FileHandle.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":272
+/* "fatfs/wrapper.pyx":272
  *         self.fp = FIL_Handle()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         ret = pyf_close(self.fp)
  *         if ret != FR_OK:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_10FileHandle_3close(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_7wrapper_10FileHandle_2close[] = "FileHandle.close(self)";
-static PyMethodDef __pyx_mdef_7wrapper_10FileHandle_3close = {"close", (PyCFunction)__pyx_pw_7wrapper_10FileHandle_3close, METH_O, __pyx_doc_7wrapper_10FileHandle_2close};
-static PyObject *__pyx_pw_7wrapper_10FileHandle_3close(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_3close(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_10FileHandle_3close = {"close", (PyCFunction)__pyx_pw_5fatfs_7wrapper_10FileHandle_3close, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_3close(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_10FileHandle_2close(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FileHandle_2close(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FileHandle_2close(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_2close(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_v_ret = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "wrapper.pyx":273
+  /* "fatfs/wrapper.pyx":273
  * 
  *     def close(self):
  *         ret = pyf_close(self.fp)             # <<<<<<<<<<<<<<
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pyf_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
@@ -4860,30 +4876,30 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ret = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":274
+  /* "fatfs/wrapper.pyx":274
  *     def close(self):
  *         ret = pyf_close(self.fp)
  *         if ret != FR_OK:             # <<<<<<<<<<<<<<
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *     def __enter__(self):
  */
   __pyx_t_1 = __Pyx_PyInt_From_FRESULT(FR_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyObject_RichCompare(__pyx_v_ret, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_5)) {
 
-    /* "wrapper.pyx":275
+    /* "fatfs/wrapper.pyx":275
  *         ret = pyf_close(self.fp)
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)             # <<<<<<<<<<<<<<
  *     def __enter__(self):
  *         return self
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FatFSException); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error)
@@ -4906,24 +4922,24 @@
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 275, __pyx_L1_error)
 
-    /* "wrapper.pyx":274
+    /* "fatfs/wrapper.pyx":274
  *     def close(self):
  *         ret = pyf_close(self.fp)
  *         if ret != FR_OK:             # <<<<<<<<<<<<<<
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *     def __enter__(self):
  */
   }
 
-  /* "wrapper.pyx":272
+  /* "fatfs/wrapper.pyx":272
  *         self.fp = FIL_Handle()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         ret = pyf_close(self.fp)
  *         if ret != FR_OK:
  */
 
@@ -4931,91 +4947,89 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("wrapper.FileHandle.close", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FileHandle.close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":276
+/* "fatfs/wrapper.pyx":276
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_10FileHandle_5__enter__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_7wrapper_10FileHandle_4__enter__[] = "FileHandle.__enter__(self)";
-static PyMethodDef __pyx_mdef_7wrapper_10FileHandle_5__enter__ = {"__enter__", (PyCFunction)__pyx_pw_7wrapper_10FileHandle_5__enter__, METH_O, __pyx_doc_7wrapper_10FileHandle_4__enter__};
-static PyObject *__pyx_pw_7wrapper_10FileHandle_5__enter__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_5__enter__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_10FileHandle_5__enter__ = {"__enter__", (PyCFunction)__pyx_pw_5fatfs_7wrapper_10FileHandle_5__enter__, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_5__enter__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_10FileHandle_4__enter__(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FileHandle_4__enter__(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FileHandle_4__enter__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_4__enter__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "wrapper.pyx":277
+  /* "fatfs/wrapper.pyx":277
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, except_type, except_value, except_traceback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self);
   __pyx_r = __pyx_v_self;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":276
+  /* "fatfs/wrapper.pyx":276
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":279
+/* "fatfs/wrapper.pyx":279
  *         return self
  * 
  *     def __exit__(self, except_type, except_value, except_traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_10FileHandle_7__exit__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_10FileHandle_6__exit__[] = "FileHandle.__exit__(self, except_type, except_value, except_traceback)";
-static PyMethodDef __pyx_mdef_7wrapper_10FileHandle_7__exit__ = {"__exit__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_10FileHandle_7__exit__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_10FileHandle_6__exit__};
-static PyObject *__pyx_pw_7wrapper_10FileHandle_7__exit__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_7__exit__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_10FileHandle_7__exit__ = {"__exit__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_10FileHandle_7__exit__, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_7__exit__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   CYTHON_UNUSED PyObject *__pyx_v_except_type = 0;
   CYTHON_UNUSED PyObject *__pyx_v_except_value = 0;
   CYTHON_UNUSED PyObject *__pyx_v_except_traceback = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -5080,37 +5094,37 @@
     __pyx_v_except_value = values[2];
     __pyx_v_except_traceback = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__exit__", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 279, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.FileHandle.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FileHandle.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_10FileHandle_6__exit__(__pyx_self, __pyx_v_self, __pyx_v_except_type, __pyx_v_except_value, __pyx_v_except_traceback);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FileHandle_6__exit__(__pyx_self, __pyx_v_self, __pyx_v_except_type, __pyx_v_except_value, __pyx_v_except_traceback);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FileHandle_6__exit__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_except_type, CYTHON_UNUSED PyObject *__pyx_v_except_value, CYTHON_UNUSED PyObject *__pyx_v_except_traceback) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_6__exit__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_except_type, CYTHON_UNUSED PyObject *__pyx_v_except_value, CYTHON_UNUSED PyObject *__pyx_v_except_traceback) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "wrapper.pyx":280
+  /* "fatfs/wrapper.pyx":280
  * 
  *     def __exit__(self, except_type, except_value, except_traceback):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
@@ -5128,86 +5142,85 @@
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":279
+  /* "fatfs/wrapper.pyx":279
  *         return self
  * 
  *     def __exit__(self, except_type, except_value, except_traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("wrapper.FileHandle.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FileHandle.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":282
+/* "fatfs/wrapper.pyx":282
  *         self.close()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.isopen:
  *             self.close()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_10FileHandle_9__dealloc__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_7wrapper_10FileHandle_8__dealloc__[] = "FileHandle.__dealloc__(self)";
-static PyMethodDef __pyx_mdef_7wrapper_10FileHandle_9__dealloc__ = {"__dealloc__", (PyCFunction)__pyx_pw_7wrapper_10FileHandle_9__dealloc__, METH_O, __pyx_doc_7wrapper_10FileHandle_8__dealloc__};
-static PyObject *__pyx_pw_7wrapper_10FileHandle_9__dealloc__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_9__dealloc__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_10FileHandle_9__dealloc__ = {"__dealloc__", (PyCFunction)__pyx_pw_5fatfs_7wrapper_10FileHandle_9__dealloc__, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_9__dealloc__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_10FileHandle_8__dealloc__(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FileHandle_8__dealloc__(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FileHandle_8__dealloc__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_8__dealloc__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "wrapper.pyx":283
+  /* "fatfs/wrapper.pyx":283
  * 
  *     def __dealloc__(self):
  *         if self.isopen:             # <<<<<<<<<<<<<<
  *             self.close()
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_isopen); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "wrapper.pyx":284
+    /* "fatfs/wrapper.pyx":284
  *     def __dealloc__(self):
  *         if self.isopen:
  *             self.close()             # <<<<<<<<<<<<<<
  * 
  *     def write(self, data):
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
@@ -5225,59 +5238,58 @@
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "wrapper.pyx":283
+    /* "fatfs/wrapper.pyx":283
  * 
  *     def __dealloc__(self):
  *         if self.isopen:             # <<<<<<<<<<<<<<
  *             self.close()
  * 
  */
   }
 
-  /* "wrapper.pyx":282
+  /* "fatfs/wrapper.pyx":282
  *         self.close()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.isopen:
  *             self.close()
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("wrapper.FileHandle.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FileHandle.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":286
+/* "fatfs/wrapper.pyx":286
  *             self.close()
  * 
  *     def write(self, data):             # <<<<<<<<<<<<<<
  *         if isinstance(data, str):
  *             data = bytes(data, 'ascii')
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_10FileHandle_11write(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_10FileHandle_10write[] = "FileHandle.write(self, data)";
-static PyMethodDef __pyx_mdef_7wrapper_10FileHandle_11write = {"write", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_10FileHandle_11write, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_10FileHandle_10write};
-static PyObject *__pyx_pw_7wrapper_10FileHandle_11write(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_11write(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_10FileHandle_11write = {"write", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_10FileHandle_11write, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_11write(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5320,26 +5332,26 @@
     __pyx_v_self = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("write", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 286, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.FileHandle.write", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FileHandle.write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_10FileHandle_10write(__pyx_self, __pyx_v_self, __pyx_v_data);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FileHandle_10write(__pyx_self, __pyx_v_self, __pyx_v_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FileHandle_10write(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_10write(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data) {
   PyObject *__pyx_v_ret = NULL;
   PyObject *__pyx_v_written = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -5351,26 +5363,26 @@
   PyObject *(*__pyx_t_9)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("write", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "wrapper.pyx":287
+  /* "fatfs/wrapper.pyx":287
  * 
  *     def write(self, data):
  *         if isinstance(data, str):             # <<<<<<<<<<<<<<
  *             data = bytes(data, 'ascii')
  *         ret, written = pyf_write(self.fp, data)
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "wrapper.pyx":288
+    /* "fatfs/wrapper.pyx":288
  *     def write(self, data):
  *         if isinstance(data, str):
  *             data = bytes(data, 'ascii')             # <<<<<<<<<<<<<<
  *         ret, written = pyf_write(self.fp, data)
  *         if ret != FR_OK:
  */
     __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
@@ -5383,24 +5395,24 @@
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_n_u_ascii);
     __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 288, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "wrapper.pyx":287
+    /* "fatfs/wrapper.pyx":287
  * 
  *     def write(self, data):
  *         if isinstance(data, str):             # <<<<<<<<<<<<<<
  *             data = bytes(data, 'ascii')
  *         ret, written = pyf_write(self.fp, data)
  */
   }
 
-  /* "wrapper.pyx":289
+  /* "fatfs/wrapper.pyx":289
  *         if isinstance(data, str):
  *             data = bytes(data, 'ascii')
  *         ret, written = pyf_write(self.fp, data)             # <<<<<<<<<<<<<<
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pyf_write); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 289, __pyx_L1_error)
@@ -5501,30 +5513,30 @@
     __pyx_L5_unpacking_done:;
   }
   __pyx_v_ret = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_written = __pyx_t_8;
   __pyx_t_8 = 0;
 
-  /* "wrapper.pyx":290
+  /* "fatfs/wrapper.pyx":290
  *             data = bytes(data, 'ascii')
  *         ret, written = pyf_write(self.fp, data)
  *         if ret != FR_OK:             # <<<<<<<<<<<<<<
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *         return written
  */
   __pyx_t_4 = __Pyx_PyInt_From_FRESULT(FR_OK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_8 = PyObject_RichCompare(__pyx_v_ret, __pyx_t_4, Py_NE); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "wrapper.pyx":291
+    /* "fatfs/wrapper.pyx":291
  *         ret, written = pyf_write(self.fp, data)
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)             # <<<<<<<<<<<<<<
  *         return written
  * 
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FatFSException); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 291, __pyx_L1_error)
@@ -5547,74 +5559,73 @@
     if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 291, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_8, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __PYX_ERR(0, 291, __pyx_L1_error)
 
-    /* "wrapper.pyx":290
+    /* "fatfs/wrapper.pyx":290
  *             data = bytes(data, 'ascii')
  *         ret, written = pyf_write(self.fp, data)
  *         if ret != FR_OK:             # <<<<<<<<<<<<<<
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *         return written
  */
   }
 
-  /* "wrapper.pyx":292
+  /* "fatfs/wrapper.pyx":292
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *         return written             # <<<<<<<<<<<<<<
  * 
  *     def read(self, size = -1):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_written);
   __pyx_r = __pyx_v_written;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":286
+  /* "fatfs/wrapper.pyx":286
  *             self.close()
  * 
  *     def write(self, data):             # <<<<<<<<<<<<<<
  *         if isinstance(data, str):
  *             data = bytes(data, 'ascii')
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("wrapper.FileHandle.write", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FileHandle.write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_XDECREF(__pyx_v_written);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":294
+/* "fatfs/wrapper.pyx":294
  *         return written
  * 
  *     def read(self, size = -1):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_10FileHandle_13read(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_10FileHandle_12read[] = "FileHandle.read(self, size=-1)";
-static PyMethodDef __pyx_mdef_7wrapper_10FileHandle_13read = {"read", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_10FileHandle_13read, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_10FileHandle_12read};
-static PyObject *__pyx_pw_7wrapper_10FileHandle_13read(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_13read(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_10FileHandle_13read = {"read", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_10FileHandle_13read, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_10FileHandle_13read(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   CYTHON_UNUSED PyObject *__pyx_v_size = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5661,50 +5672,49 @@
     __pyx_v_self = values[0];
     __pyx_v_size = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("read", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 294, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.FileHandle.read", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.FileHandle.read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_10FileHandle_12read(__pyx_self, __pyx_v_self, __pyx_v_size);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_10FileHandle_12read(__pyx_self, __pyx_v_self, __pyx_v_size);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_10FileHandle_12read(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_size) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_10FileHandle_12read(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_size) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read", 0);
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":299
+/* "fatfs/wrapper.pyx":299
  * 
  * class Partition():
  *     def __init__(self, disk):             # <<<<<<<<<<<<<<
  *         self.fs = FATFS_Handle()
  *         self.disk = disk
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_9Partition_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_9Partition___init__[] = "Partition.__init__(self, disk)";
-static PyMethodDef __pyx_mdef_7wrapper_9Partition_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_9Partition_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_9Partition___init__};
-static PyObject *__pyx_pw_7wrapper_9Partition_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_9Partition_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_9Partition_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_disk = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5747,115 +5757,115 @@
     __pyx_v_self = values[0];
     __pyx_v_disk = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 299, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.Partition.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_9Partition___init__(__pyx_self, __pyx_v_self, __pyx_v_disk);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_9Partition___init__(__pyx_self, __pyx_v_self, __pyx_v_disk);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_9Partition___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_disk) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_disk) {
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   long __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "wrapper.pyx":300
+  /* "fatfs/wrapper.pyx":300
  * class Partition():
  *     def __init__(self, disk):
  *         self.fs = FATFS_Handle()             # <<<<<<<<<<<<<<
  *         self.disk = disk
  *         self.pname = None
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_7wrapper_FATFS_Handle)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5fatfs_7wrapper_FATFS_Handle)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_fs, __pyx_t_1) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":301
+  /* "fatfs/wrapper.pyx":301
  *     def __init__(self, disk):
  *         self.fs = FATFS_Handle()
  *         self.disk = disk             # <<<<<<<<<<<<<<
  *         self.pname = None
  *         self.pdev = None
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_disk, __pyx_v_disk) < 0) __PYX_ERR(0, 301, __pyx_L1_error)
 
-  /* "wrapper.pyx":302
+  /* "fatfs/wrapper.pyx":302
  *         self.fs = FATFS_Handle()
  *         self.disk = disk
  *         self.pname = None             # <<<<<<<<<<<<<<
  *         self.pdev = None
  * 
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pname, Py_None) < 0) __PYX_ERR(0, 302, __pyx_L1_error)
 
-  /* "wrapper.pyx":303
+  /* "fatfs/wrapper.pyx":303
  *         self.disk = disk
  *         self.pname = None
  *         self.pdev = None             # <<<<<<<<<<<<<<
  * 
  *         # Find pdev and pname
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pdev, Py_None) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
 
-  /* "wrapper.pyx":307
+  /* "fatfs/wrapper.pyx":307
  *         # Find pdev and pname
  *         # TODO: Can we fetch the constant directly? Or define it here? Does it have to be 10 only?
  *         for i in range(10): # corresponds to FF_VOLUMES in ffconf.h             # <<<<<<<<<<<<<<
  *             if not i in __diskio_wrapper_disks:
  *                 self.pdev = i
  */
   for (__pyx_t_2 = 0; __pyx_t_2 < 10; __pyx_t_2+=1) {
     __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_i = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "wrapper.pyx":308
+    /* "fatfs/wrapper.pyx":308
  *         # TODO: Can we fetch the constant directly? Or define it here? Does it have to be 10 only?
  *         for i in range(10): # corresponds to FF_VOLUMES in ffconf.h
  *             if not i in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *                 self.pdev = i
  *                 self.pname = bytes("%d:" % i, 'ascii')
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_diskio_wrapper_disks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_v_i, __pyx_t_1, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 308, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_4 = (__pyx_t_3 != 0);
     if (__pyx_t_4) {
 
-      /* "wrapper.pyx":309
+      /* "fatfs/wrapper.pyx":309
  *         for i in range(10): # corresponds to FF_VOLUMES in ffconf.h
  *             if not i in __diskio_wrapper_disks:
  *                 self.pdev = i             # <<<<<<<<<<<<<<
  *                 self.pname = bytes("%d:" % i, 'ascii')
  *                 __diskio_wrapper_disks[i] = disk
  */
       if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pdev, __pyx_v_i) < 0) __PYX_ERR(0, 309, __pyx_L1_error)
 
-      /* "wrapper.pyx":310
+      /* "fatfs/wrapper.pyx":310
  *             if not i in __diskio_wrapper_disks:
  *                 self.pdev = i
  *                 self.pname = bytes("%d:" % i, 'ascii')             # <<<<<<<<<<<<<<
  *                 __diskio_wrapper_disks[i] = disk
  *                 break
  */
       __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_d, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
@@ -5870,45 +5880,45 @@
       __pyx_t_1 = 0;
       __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pname, __pyx_t_1) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "wrapper.pyx":311
+      /* "fatfs/wrapper.pyx":311
  *                 self.pdev = i
  *                 self.pname = bytes("%d:" % i, 'ascii')
  *                 __diskio_wrapper_disks[i] = disk             # <<<<<<<<<<<<<<
  *                 break
  *             raise FatFSException("__init__", -1)
  */
       __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_diskio_wrapper_disks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_i, __pyx_v_disk) < 0)) __PYX_ERR(0, 311, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "wrapper.pyx":312
+      /* "fatfs/wrapper.pyx":312
  *                 self.pname = bytes("%d:" % i, 'ascii')
  *                 __diskio_wrapper_disks[i] = disk
  *                 break             # <<<<<<<<<<<<<<
  *             raise FatFSException("__init__", -1)
  *     def _adjust_path(self, path):
  */
       goto __pyx_L4_break;
 
-      /* "wrapper.pyx":308
+      /* "fatfs/wrapper.pyx":308
  *         # TODO: Can we fetch the constant directly? Or define it here? Does it have to be 10 only?
  *         for i in range(10): # corresponds to FF_VOLUMES in ffconf.h
  *             if not i in __diskio_wrapper_disks:             # <<<<<<<<<<<<<<
  *                 self.pdev = i
  *                 self.pname = bytes("%d:" % i, 'ascii')
  */
     }
 
-    /* "wrapper.pyx":313
+    /* "fatfs/wrapper.pyx":313
  *                 __diskio_wrapper_disks[i] = disk
  *                 break
  *             raise FatFSException("__init__", -1)             # <<<<<<<<<<<<<<
  *     def _adjust_path(self, path):
  *         """
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FatFSException); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
@@ -5918,50 +5928,50 @@
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __PYX_ERR(0, 313, __pyx_L1_error)
   }
   __pyx_L4_break:;
 
-  /* "wrapper.pyx":299
+  /* "fatfs/wrapper.pyx":299
  * 
  * class Partition():
  *     def __init__(self, disk):             # <<<<<<<<<<<<<<
  *         self.fs = FATFS_Handle()
  *         self.disk = disk
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("wrapper.Partition.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":314
+/* "fatfs/wrapper.pyx":314
  *                 break
  *             raise FatFSException("__init__", -1)
  *     def _adjust_path(self, path):             # <<<<<<<<<<<<<<
  *         """
  *         Adjusts path for use in pyf_ calls: adds partition prefix and converts to bytes.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_9Partition_3_adjust_path(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_9Partition_2_adjust_path[] = "Partition._adjust_path(self, path)\n\n        Adjusts path for use in pyf_ calls: adds partition prefix and converts to bytes.\n        ";
-static PyMethodDef __pyx_mdef_7wrapper_9Partition_3_adjust_path = {"_adjust_path", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_9Partition_3_adjust_path, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_9Partition_2_adjust_path};
-static PyObject *__pyx_pw_7wrapper_9Partition_3_adjust_path(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_3_adjust_path(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_5fatfs_7wrapper_9Partition_2_adjust_path[] = "\n        Adjusts path for use in pyf_ calls: adds partition prefix and converts to bytes.\n        ";
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_9Partition_3_adjust_path = {"_adjust_path", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_9Partition_3_adjust_path, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5fatfs_7wrapper_9Partition_2_adjust_path};
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_3_adjust_path(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_path = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6004,37 +6014,37 @@
     __pyx_v_self = values[0];
     __pyx_v_path = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_adjust_path", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 314, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.Partition._adjust_path", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition._adjust_path", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_9Partition_2_adjust_path(__pyx_self, __pyx_v_self, __pyx_v_path);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_9Partition_2_adjust_path(__pyx_self, __pyx_v_self, __pyx_v_path);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_9Partition_2_adjust_path(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_2_adjust_path(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_adjust_path", 0);
 
-  /* "wrapper.pyx":318
+  /* "fatfs/wrapper.pyx":318
  *         Adjusts path for use in pyf_ calls: adds partition prefix and converts to bytes.
  *         """
  *         return self.pname + bytes(path, 'ascii')             # <<<<<<<<<<<<<<
  * 
  *     def mount(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -6055,59 +6065,58 @@
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":314
+  /* "fatfs/wrapper.pyx":314
  *                 break
  *             raise FatFSException("__init__", -1)
  *     def _adjust_path(self, path):             # <<<<<<<<<<<<<<
  *         """
  *         Adjusts path for use in pyf_ calls: adds partition prefix and converts to bytes.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("wrapper.Partition._adjust_path", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition._adjust_path", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":320
+/* "fatfs/wrapper.pyx":320
  *         return self.pname + bytes(path, 'ascii')
  * 
  *     def mount(self):             # <<<<<<<<<<<<<<
  *         ret = pyf_mount(self.fs, self.pname, 1)
  *         if ret == FR_OK:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_9Partition_5mount(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_7wrapper_9Partition_4mount[] = "Partition.mount(self)";
-static PyMethodDef __pyx_mdef_7wrapper_9Partition_5mount = {"mount", (PyCFunction)__pyx_pw_7wrapper_9Partition_5mount, METH_O, __pyx_doc_7wrapper_9Partition_4mount};
-static PyObject *__pyx_pw_7wrapper_9Partition_5mount(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_5mount(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_9Partition_5mount = {"mount", (PyCFunction)__pyx_pw_5fatfs_7wrapper_9Partition_5mount, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_5mount(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("mount (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_9Partition_4mount(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_9Partition_4mount(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_9Partition_4mount(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_4mount(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_v_ret = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -6116,15 +6125,15 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mount", 0);
 
-  /* "wrapper.pyx":321
+  /* "fatfs/wrapper.pyx":321
  * 
  *     def mount(self):
  *         ret = pyf_mount(self.fs, self.pname, 1)             # <<<<<<<<<<<<<<
  *         if ret == FR_OK:
  *             return True
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pyf_mount); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 321, __pyx_L1_error)
@@ -6184,51 +6193,51 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ret = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":322
+  /* "fatfs/wrapper.pyx":322
  *     def mount(self):
  *         ret = pyf_mount(self.fs, self.pname, 1)
  *         if ret == FR_OK:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   __pyx_t_1 = __Pyx_PyInt_From_FRESULT(FR_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyObject_RichCompare(__pyx_v_ret, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(__pyx_t_8)) {
 
-    /* "wrapper.pyx":323
+    /* "fatfs/wrapper.pyx":323
  *         ret = pyf_mount(self.fs, self.pname, 1)
  *         if ret == FR_OK:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             raise FatFSException("mount", ret, self.pname)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "wrapper.pyx":322
+    /* "fatfs/wrapper.pyx":322
  *     def mount(self):
  *         ret = pyf_mount(self.fs, self.pname, 1)
  *         if ret == FR_OK:             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
   }
 
-  /* "wrapper.pyx":325
+  /* "fatfs/wrapper.pyx":325
  *             return True
  *         else:
  *             raise FatFSException("mount", ret, self.pname)             # <<<<<<<<<<<<<<
  * 
  *     def unmount(self):
  */
   /*else*/ {
@@ -6287,15 +6296,15 @@
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 325, __pyx_L1_error)
   }
 
-  /* "wrapper.pyx":320
+  /* "fatfs/wrapper.pyx":320
  *         return self.pname + bytes(path, 'ascii')
  * 
  *     def mount(self):             # <<<<<<<<<<<<<<
  *         ret = pyf_mount(self.fs, self.pname, 1)
  *         if ret == FR_OK:
  */
 
@@ -6303,47 +6312,46 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("wrapper.Partition.mount", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.mount", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":327
+/* "fatfs/wrapper.pyx":327
  *             raise FatFSException("mount", ret, self.pname)
  * 
  *     def unmount(self):             # <<<<<<<<<<<<<<
  *         ret = f_mount(NULL, self.pname, 0)
  *         if ret == FR_OK:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_9Partition_7unmount(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_7wrapper_9Partition_6unmount[] = "Partition.unmount(self)";
-static PyMethodDef __pyx_mdef_7wrapper_9Partition_7unmount = {"unmount", (PyCFunction)__pyx_pw_7wrapper_9Partition_7unmount, METH_O, __pyx_doc_7wrapper_9Partition_6unmount};
-static PyObject *__pyx_pw_7wrapper_9Partition_7unmount(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_7unmount(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_9Partition_7unmount = {"unmount", (PyCFunction)__pyx_pw_5fatfs_7wrapper_9Partition_7unmount, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_7unmount(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("unmount (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_9Partition_6unmount(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_9Partition_6unmount(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_9Partition_6unmount(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_6unmount(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   FRESULT __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   TCHAR const *__pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
@@ -6353,74 +6361,74 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unmount", 0);
 
-  /* "wrapper.pyx":328
+  /* "fatfs/wrapper.pyx":328
  * 
  *     def unmount(self):
  *         ret = f_mount(NULL, self.pname, 0)             # <<<<<<<<<<<<<<
  *         if ret == FR_OK:
  *             del __diskio_wrapper_disks[self.pdev]
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pname); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 328, __pyx_L1_error)
   __pyx_v_ret = f_mount(NULL, __pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":329
+  /* "fatfs/wrapper.pyx":329
  *     def unmount(self):
  *         ret = f_mount(NULL, self.pname, 0)
  *         if ret == FR_OK:             # <<<<<<<<<<<<<<
  *             del __diskio_wrapper_disks[self.pdev]
  *             return True
  */
   __pyx_t_3 = ((__pyx_v_ret == FR_OK) != 0);
   if (likely(__pyx_t_3)) {
 
-    /* "wrapper.pyx":330
+    /* "fatfs/wrapper.pyx":330
  *         ret = f_mount(NULL, self.pname, 0)
  *         if ret == FR_OK:
  *             del __diskio_wrapper_disks[self.pdev]             # <<<<<<<<<<<<<<
  *             return True
  *         else:
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_diskio_wrapper_disks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pdev); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (unlikely(PyObject_DelItem(__pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "wrapper.pyx":331
+    /* "fatfs/wrapper.pyx":331
  *         if ret == FR_OK:
  *             del __diskio_wrapper_disks[self.pdev]
  *             return True             # <<<<<<<<<<<<<<
  *         else:
  *             raise FatFSException("unmount", ret, self.pname)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "wrapper.pyx":329
+    /* "fatfs/wrapper.pyx":329
  *     def unmount(self):
  *         ret = f_mount(NULL, self.pname, 0)
  *         if ret == FR_OK:             # <<<<<<<<<<<<<<
  *             del __diskio_wrapper_disks[self.pdev]
  *             return True
  */
   }
 
-  /* "wrapper.pyx":333
+  /* "fatfs/wrapper.pyx":333
  *             return True
  *         else:
  *             raise FatFSException("unmount", ret, self.pname)             # <<<<<<<<<<<<<<
  * 
  *     def mkfs(self):
  */
   /*else*/ {
@@ -6483,15 +6491,15 @@
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(0, 333, __pyx_L1_error)
   }
 
-  /* "wrapper.pyx":327
+  /* "fatfs/wrapper.pyx":327
  *             raise FatFSException("mount", ret, self.pname)
  * 
  *     def unmount(self):             # <<<<<<<<<<<<<<
  *         ret = f_mount(NULL, self.pname, 0)
  *         if ret == FR_OK:
  */
 
@@ -6499,58 +6507,57 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("wrapper.Partition.unmount", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.unmount", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":335
+/* "fatfs/wrapper.pyx":335
  *             raise FatFSException("unmount", ret, self.pname)
  * 
  *     def mkfs(self):             # <<<<<<<<<<<<<<
  *         pyf_mkfs(self.pname)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_9Partition_9mkfs(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_7wrapper_9Partition_8mkfs[] = "Partition.mkfs(self)";
-static PyMethodDef __pyx_mdef_7wrapper_9Partition_9mkfs = {"mkfs", (PyCFunction)__pyx_pw_7wrapper_9Partition_9mkfs, METH_O, __pyx_doc_7wrapper_9Partition_8mkfs};
-static PyObject *__pyx_pw_7wrapper_9Partition_9mkfs(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_9mkfs(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_9Partition_9mkfs = {"mkfs", (PyCFunction)__pyx_pw_5fatfs_7wrapper_9Partition_9mkfs, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_9mkfs(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("mkfs (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_9Partition_8mkfs(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_9Partition_8mkfs(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_9Partition_8mkfs(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_8mkfs(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mkfs", 0);
 
-  /* "wrapper.pyx":336
+  /* "fatfs/wrapper.pyx":336
  * 
  *     def mkfs(self):
  *         pyf_mkfs(self.pname)             # <<<<<<<<<<<<<<
  * 
  *     def mkdir(self, path):
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pyf_mkfs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
@@ -6571,15 +6578,15 @@
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":335
+  /* "fatfs/wrapper.pyx":335
  *             raise FatFSException("unmount", ret, self.pname)
  * 
  *     def mkfs(self):             # <<<<<<<<<<<<<<
  *         pyf_mkfs(self.pname)
  * 
  */
 
@@ -6587,35 +6594,34 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("wrapper.Partition.mkfs", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.mkfs", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":338
+/* "fatfs/wrapper.pyx":338
  *         pyf_mkfs(self.pname)
  * 
  *     def mkdir(self, path):             # <<<<<<<<<<<<<<
  *         p = self._adjust_path(path)
  *         ret = pyf_mkdir(p)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_9Partition_11mkdir(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_9Partition_10mkdir[] = "Partition.mkdir(self, path)";
-static PyMethodDef __pyx_mdef_7wrapper_9Partition_11mkdir = {"mkdir", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_9Partition_11mkdir, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_9Partition_10mkdir};
-static PyObject *__pyx_pw_7wrapper_9Partition_11mkdir(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_11mkdir(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_9Partition_11mkdir = {"mkdir", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_9Partition_11mkdir, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_11mkdir(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_path = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6658,26 +6664,26 @@
     __pyx_v_self = values[0];
     __pyx_v_path = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("mkdir", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 338, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.Partition.mkdir", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.mkdir", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_9Partition_10mkdir(__pyx_self, __pyx_v_self, __pyx_v_path);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_9Partition_10mkdir(__pyx_self, __pyx_v_self, __pyx_v_path);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_9Partition_10mkdir(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_10mkdir(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path) {
   PyObject *__pyx_v_p = NULL;
   PyObject *__pyx_v_ret = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -6685,15 +6691,15 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mkdir", 0);
 
-  /* "wrapper.pyx":339
+  /* "fatfs/wrapper.pyx":339
  * 
  *     def mkdir(self, path):
  *         p = self._adjust_path(path)             # <<<<<<<<<<<<<<
  *         ret = pyf_mkdir(p)
  *         if ret != FR_OK:
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_adjust_path); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
@@ -6712,15 +6718,15 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_p = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":340
+  /* "fatfs/wrapper.pyx":340
  *     def mkdir(self, path):
  *         p = self._adjust_path(path)
  *         ret = pyf_mkdir(p)             # <<<<<<<<<<<<<<
  *         if ret != FR_OK:
  *             #raise FatFSException("FatFS::mkdir(%s) failed with error code %s" % (p, ret))
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pyf_mkdir); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
@@ -6739,30 +6745,30 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ret = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":341
+  /* "fatfs/wrapper.pyx":341
  *         p = self._adjust_path(path)
  *         ret = pyf_mkdir(p)
  *         if ret != FR_OK:             # <<<<<<<<<<<<<<
  *             #raise FatFSException("FatFS::mkdir(%s) failed with error code %s" % (p, ret))
  *             raise FatFSException("mount", ret, p)
  */
   __pyx_t_1 = __Pyx_PyInt_From_FRESULT(FR_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyObject_RichCompare(__pyx_v_ret, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_4)) {
 
-    /* "wrapper.pyx":343
+    /* "fatfs/wrapper.pyx":343
  *         if ret != FR_OK:
  *             #raise FatFSException("FatFS::mkdir(%s) failed with error code %s" % (p, ret))
  *             raise FatFSException("mount", ret, p)             # <<<<<<<<<<<<<<
  * 
  *     def open(self, path, mode):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FatFSException); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
@@ -6815,24 +6821,24 @@
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 343, __pyx_L1_error)
 
-    /* "wrapper.pyx":341
+    /* "fatfs/wrapper.pyx":341
  *         p = self._adjust_path(path)
  *         ret = pyf_mkdir(p)
  *         if ret != FR_OK:             # <<<<<<<<<<<<<<
  *             #raise FatFSException("FatFS::mkdir(%s) failed with error code %s" % (p, ret))
  *             raise FatFSException("mount", ret, p)
  */
   }
 
-  /* "wrapper.pyx":338
+  /* "fatfs/wrapper.pyx":338
  *         pyf_mkfs(self.pname)
  * 
  *     def mkdir(self, path):             # <<<<<<<<<<<<<<
  *         p = self._adjust_path(path)
  *         ret = pyf_mkdir(p)
  */
 
@@ -6840,37 +6846,36 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("wrapper.Partition.mkdir", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.mkdir", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_p);
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":345
+/* "fatfs/wrapper.pyx":345
  *             raise FatFSException("mount", ret, p)
  * 
  *     def open(self, path, mode):             # <<<<<<<<<<<<<<
  *         # TODO: Implement mode.
  *         handle = FileHandle()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_9Partition_13open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7wrapper_9Partition_12open[] = "Partition.open(self, path, mode)";
-static PyMethodDef __pyx_mdef_7wrapper_9Partition_13open = {"open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7wrapper_9Partition_13open, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7wrapper_9Partition_12open};
-static PyObject *__pyx_pw_7wrapper_9Partition_13open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_13open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_9Partition_13open = {"open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5fatfs_7wrapper_9Partition_13open, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_9Partition_13open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_path = 0;
   CYTHON_UNUSED PyObject *__pyx_v_mode = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -6924,26 +6929,26 @@
     __pyx_v_path = values[1];
     __pyx_v_mode = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("open", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 345, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("wrapper.Partition.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_9Partition_12open(__pyx_self, __pyx_v_self, __pyx_v_path, __pyx_v_mode);
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_9Partition_12open(__pyx_self, __pyx_v_self, __pyx_v_path, __pyx_v_mode);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_9Partition_12open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path, CYTHON_UNUSED PyObject *__pyx_v_mode) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_9Partition_12open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path, CYTHON_UNUSED PyObject *__pyx_v_mode) {
   PyObject *__pyx_v_handle = NULL;
   PyObject *__pyx_v_p = NULL;
   PyObject *__pyx_v_ret = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -6954,15 +6959,15 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
 
-  /* "wrapper.pyx":347
+  /* "fatfs/wrapper.pyx":347
  *     def open(self, path, mode):
  *         # TODO: Implement mode.
  *         handle = FileHandle()             # <<<<<<<<<<<<<<
  *         p = self._adjust_path(path)
  *         ret = pyf_open(handle.fp, p, FA_WRITE | FA_CREATE_ALWAYS)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FileHandle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
@@ -6981,15 +6986,15 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_handle = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":348
+  /* "fatfs/wrapper.pyx":348
  *         # TODO: Implement mode.
  *         handle = FileHandle()
  *         p = self._adjust_path(path)             # <<<<<<<<<<<<<<
  *         ret = pyf_open(handle.fp, p, FA_WRITE | FA_CREATE_ALWAYS)
  *         if ret != FR_OK:
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_adjust_path); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
@@ -7008,15 +7013,15 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_p = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":349
+  /* "fatfs/wrapper.pyx":349
  *         handle = FileHandle()
  *         p = self._adjust_path(path)
  *         ret = pyf_open(handle.fp, p, FA_WRITE | FA_CREATE_ALWAYS)             # <<<<<<<<<<<<<<
  *         if ret != FR_OK:
  *             raise FatFSException("open", ret, p)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pyf_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
@@ -7076,30 +7081,30 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ret = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":350
+  /* "fatfs/wrapper.pyx":350
  *         p = self._adjust_path(path)
  *         ret = pyf_open(handle.fp, p, FA_WRITE | FA_CREATE_ALWAYS)
  *         if ret != FR_OK:             # <<<<<<<<<<<<<<
  *             raise FatFSException("open", ret, p)
  *         handle.isopen = True
  */
   __pyx_t_1 = __Pyx_PyInt_From_FRESULT(FR_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyObject_RichCompare(__pyx_v_ret, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_8)) {
 
-    /* "wrapper.pyx":351
+    /* "fatfs/wrapper.pyx":351
  *         ret = pyf_open(handle.fp, p, FA_WRITE | FA_CREATE_ALWAYS)
  *         if ret != FR_OK:
  *             raise FatFSException("open", ret, p)             # <<<<<<<<<<<<<<
  *         handle.isopen = True
  *         return handle
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FatFSException); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 351, __pyx_L1_error)
@@ -7152,45 +7157,45 @@
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 351, __pyx_L1_error)
 
-    /* "wrapper.pyx":350
+    /* "fatfs/wrapper.pyx":350
  *         p = self._adjust_path(path)
  *         ret = pyf_open(handle.fp, p, FA_WRITE | FA_CREATE_ALWAYS)
  *         if ret != FR_OK:             # <<<<<<<<<<<<<<
  *             raise FatFSException("open", ret, p)
  *         handle.isopen = True
  */
   }
 
-  /* "wrapper.pyx":352
+  /* "fatfs/wrapper.pyx":352
  *         if ret != FR_OK:
  *             raise FatFSException("open", ret, p)
  *         handle.isopen = True             # <<<<<<<<<<<<<<
  *         return handle
  * 
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_handle, __pyx_n_s_isopen, Py_True) < 0) __PYX_ERR(0, 352, __pyx_L1_error)
 
-  /* "wrapper.pyx":353
+  /* "fatfs/wrapper.pyx":353
  *             raise FatFSException("open", ret, p)
  *         handle.isopen = True
  *         return handle             # <<<<<<<<<<<<<<
  * 
  * def check_diskio(drive):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_handle);
   __pyx_r = __pyx_v_handle;
   goto __pyx_L0;
 
-  /* "wrapper.pyx":345
+  /* "fatfs/wrapper.pyx":345
  *             raise FatFSException("mount", ret, p)
  * 
  *     def open(self, path, mode):             # <<<<<<<<<<<<<<
  *         # TODO: Implement mode.
  *         handle = FileHandle()
  */
 
@@ -7198,61 +7203,60 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("wrapper.Partition.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.Partition.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_handle);
   __Pyx_XDECREF(__pyx_v_p);
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "wrapper.pyx":355
+/* "fatfs/wrapper.pyx":355
  *         return handle
  * 
  * def check_diskio(drive):             # <<<<<<<<<<<<<<
  *     assert(not 0 in __diskio_wrapper_disks, "Check diskio must be used before mounting any real drives.")
  *     __diskio_wrapper_disks[0] = drive
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7wrapper_15check_diskio(PyObject *__pyx_self, PyObject *__pyx_v_drive); /*proto*/
-static char __pyx_doc_7wrapper_14check_diskio[] = "check_diskio(drive)";
-static PyMethodDef __pyx_mdef_7wrapper_15check_diskio = {"check_diskio", (PyCFunction)__pyx_pw_7wrapper_15check_diskio, METH_O, __pyx_doc_7wrapper_14check_diskio};
-static PyObject *__pyx_pw_7wrapper_15check_diskio(PyObject *__pyx_self, PyObject *__pyx_v_drive) {
+static PyObject *__pyx_pw_5fatfs_7wrapper_15check_diskio(PyObject *__pyx_self, PyObject *__pyx_v_drive); /*proto*/
+static PyMethodDef __pyx_mdef_5fatfs_7wrapper_15check_diskio = {"check_diskio", (PyCFunction)__pyx_pw_5fatfs_7wrapper_15check_diskio, METH_O, 0};
+static PyObject *__pyx_pw_5fatfs_7wrapper_15check_diskio(PyObject *__pyx_self, PyObject *__pyx_v_drive) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("check_diskio (wrapper)", 0);
-  __pyx_r = __pyx_pf_7wrapper_14check_diskio(__pyx_self, ((PyObject *)__pyx_v_drive));
+  __pyx_r = __pyx_pf_5fatfs_7wrapper_14check_diskio(__pyx_self, ((PyObject *)__pyx_v_drive));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_14check_diskio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_drive) {
+static PyObject *__pyx_pf_5fatfs_7wrapper_14check_diskio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_drive) {
   CYTHON_UNUSED int __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("check_diskio", 0);
 
-  /* "wrapper.pyx":356
+  /* "fatfs/wrapper.pyx":356
  * 
  * def check_diskio(drive):
  *     assert(not 0 in __diskio_wrapper_disks, "Check diskio must be used before mounting any real drives.")             # <<<<<<<<<<<<<<
  *     __diskio_wrapper_disks[0] = drive
  *     ret = diskiocheck()
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
@@ -7276,112 +7280,112 @@
     if (unlikely(!__pyx_t_2)) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 356, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "wrapper.pyx":357
+  /* "fatfs/wrapper.pyx":357
  * def check_diskio(drive):
  *     assert(not 0 in __diskio_wrapper_disks, "Check diskio must be used before mounting any real drives.")
  *     __diskio_wrapper_disks[0] = drive             # <<<<<<<<<<<<<<
  *     ret = diskiocheck()
  *     del __diskio_wrapper_disks[0]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_diskio_wrapper_disks); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (unlikely(__Pyx_SetItemInt(__pyx_t_3, 0, __pyx_v_drive, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "wrapper.pyx":358
+  /* "fatfs/wrapper.pyx":358
  *     assert(not 0 in __diskio_wrapper_disks, "Check diskio must be used before mounting any real drives.")
  *     __diskio_wrapper_disks[0] = drive
  *     ret = diskiocheck()             # <<<<<<<<<<<<<<
  *     del __diskio_wrapper_disks[0]
  * 
  */
   __pyx_v_ret = diskiocheck();
 
-  /* "wrapper.pyx":359
+  /* "fatfs/wrapper.pyx":359
  *     __diskio_wrapper_disks[0] = drive
  *     ret = diskiocheck()
  *     del __diskio_wrapper_disks[0]             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_diskio_wrapper_disks); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (unlikely(__Pyx_DelItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "wrapper.pyx":355
+  /* "fatfs/wrapper.pyx":355
  *         return handle
  * 
  * def check_diskio(drive):             # <<<<<<<<<<<<<<
  *     assert(not 0 in __diskio_wrapper_disks, "Check diskio must be used before mounting any real drives.")
  *     __diskio_wrapper_disks[0] = drive
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("wrapper.check_diskio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fatfs.wrapper.check_diskio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_tp_new_7wrapper_FIL_Handle(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_5fatfs_7wrapper_FIL_Handle(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  if (unlikely(__pyx_pw_7wrapper_10FIL_Handle_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
+  if (unlikely(__pyx_pw_5fatfs_7wrapper_10FIL_Handle_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_7wrapper_FIL_Handle(PyObject *o) {
+static void __pyx_tp_dealloc_5fatfs_7wrapper_FIL_Handle(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_7wrapper_10FIL_Handle_3__dealloc__(o);
+    __pyx_pw_5fatfs_7wrapper_10FIL_Handle_3__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static PyMethodDef __pyx_methods_7wrapper_FIL_Handle[] = {
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7wrapper_10FIL_Handle_5__reduce_cython__, METH_NOARGS, __pyx_doc_7wrapper_10FIL_Handle_4__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7wrapper_10FIL_Handle_7__setstate_cython__, METH_O, __pyx_doc_7wrapper_10FIL_Handle_6__setstate_cython__},
+static PyMethodDef __pyx_methods_5fatfs_7wrapper_FIL_Handle[] = {
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_5fatfs_7wrapper_10FIL_Handle_5__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_5fatfs_7wrapper_10FIL_Handle_7__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_7wrapper_FIL_Handle = {
+static PyTypeObject __pyx_type_5fatfs_7wrapper_FIL_Handle = {
   PyVarObject_HEAD_INIT(0, 0)
-  "wrapper.FIL_Handle", /*tp_name*/
-  sizeof(struct __pyx_obj_7wrapper_FIL_Handle), /*tp_basicsize*/
+  "fatfs.wrapper.FIL_Handle", /*tp_name*/
+  sizeof(struct __pyx_obj_5fatfs_7wrapper_FIL_Handle), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_7wrapper_FIL_Handle, /*tp_dealloc*/
+  __pyx_tp_dealloc_5fatfs_7wrapper_FIL_Handle, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -7406,25 +7410,25 @@
   0, /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_7wrapper_FIL_Handle, /*tp_methods*/
+  __pyx_methods_5fatfs_7wrapper_FIL_Handle, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_7wrapper_FIL_Handle, /*tp_new*/
+  __pyx_tp_new_5fatfs_7wrapper_FIL_Handle, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -7435,63 +7439,63 @@
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
 
-static PyObject *__pyx_tp_new_7wrapper_FATFS_Handle(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_5fatfs_7wrapper_FATFS_Handle(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  if (unlikely(__pyx_pw_7wrapper_12FATFS_Handle_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
+  if (unlikely(__pyx_pw_5fatfs_7wrapper_12FATFS_Handle_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_7wrapper_FATFS_Handle(PyObject *o) {
+static void __pyx_tp_dealloc_5fatfs_7wrapper_FATFS_Handle(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_7wrapper_12FATFS_Handle_3__dealloc__(o);
+    __pyx_pw_5fatfs_7wrapper_12FATFS_Handle_3__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static PyMethodDef __pyx_methods_7wrapper_FATFS_Handle[] = {
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7wrapper_12FATFS_Handle_5__reduce_cython__, METH_NOARGS, __pyx_doc_7wrapper_12FATFS_Handle_4__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7wrapper_12FATFS_Handle_7__setstate_cython__, METH_O, __pyx_doc_7wrapper_12FATFS_Handle_6__setstate_cython__},
+static PyMethodDef __pyx_methods_5fatfs_7wrapper_FATFS_Handle[] = {
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_5fatfs_7wrapper_12FATFS_Handle_5__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_5fatfs_7wrapper_12FATFS_Handle_7__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_7wrapper_FATFS_Handle = {
+static PyTypeObject __pyx_type_5fatfs_7wrapper_FATFS_Handle = {
   PyVarObject_HEAD_INIT(0, 0)
-  "wrapper.FATFS_Handle", /*tp_name*/
-  sizeof(struct __pyx_obj_7wrapper_FATFS_Handle), /*tp_basicsize*/
+  "fatfs.wrapper.FATFS_Handle", /*tp_name*/
+  sizeof(struct __pyx_obj_5fatfs_7wrapper_FATFS_Handle), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_7wrapper_FATFS_Handle, /*tp_dealloc*/
+  __pyx_tp_dealloc_5fatfs_7wrapper_FATFS_Handle, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -7516,25 +7520,25 @@
   0, /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_7wrapper_FATFS_Handle, /*tp_methods*/
+  __pyx_methods_5fatfs_7wrapper_FATFS_Handle, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_7wrapper_FATFS_Handle, /*tp_new*/
+  __pyx_tp_new_5fatfs_7wrapper_FATFS_Handle, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -7545,15 +7549,15 @@
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
@@ -7650,14 +7654,15 @@
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_drive, __pyx_k_drive, sizeof(__pyx_k_drive), 0, 0, 1, 1},
   {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
   {&__pyx_n_s_except_traceback, __pyx_k_except_traceback, sizeof(__pyx_k_except_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_except_type, __pyx_k_except_type, sizeof(__pyx_k_except_type), 0, 0, 1, 1},
   {&__pyx_n_s_except_value, __pyx_k_except_value, sizeof(__pyx_k_except_value), 0, 0, 1, 1},
   {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
+  {&__pyx_n_s_fatfs_wrapper, __pyx_k_fatfs_wrapper, sizeof(__pyx_k_fatfs_wrapper), 0, 0, 1, 1},
   {&__pyx_kp_s_fatfs_wrapper_pyx, __pyx_k_fatfs_wrapper_pyx, sizeof(__pyx_k_fatfs_wrapper_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_fp, __pyx_k_fp, sizeof(__pyx_k_fp), 0, 0, 1, 1},
   {&__pyx_n_s_fph, __pyx_k_fph, sizeof(__pyx_k_fph), 0, 0, 1, 1},
   {&__pyx_n_s_fresult, __pyx_k_fresult, sizeof(__pyx_k_fresult), 0, 0, 1, 1},
   {&__pyx_n_s_fresult_to_name, __pyx_k_fresult_to_name, sizeof(__pyx_k_fresult_to_name), 0, 0, 1, 1},
   {&__pyx_n_s_fs, __pyx_k_fs, sizeof(__pyx_k_fs), 0, 0, 1, 1},
   {&__pyx_n_s_function, __pyx_k_function, sizeof(__pyx_k_function), 0, 0, 1, 1},
@@ -7716,15 +7721,14 @@
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_unmount, __pyx_k_unmount, sizeof(__pyx_k_unmount), 0, 0, 1, 1},
   {&__pyx_n_u_unmount, __pyx_k_unmount, sizeof(__pyx_k_unmount), 0, 1, 0, 1},
   {&__pyx_n_s_workarea_size, __pyx_k_workarea_size, sizeof(__pyx_k_workarea_size), 0, 0, 1, 1},
-  {&__pyx_n_s_wrapper, __pyx_k_wrapper, sizeof(__pyx_k_wrapper), 0, 0, 1, 1},
   {&__pyx_n_s_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 0, 1, 1},
   {&__pyx_n_u_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 1, 0, 1},
   {&__pyx_n_s_written, __pyx_k_written, sizeof(__pyx_k_written), 0, 0, 1, 1},
   {&__pyx_n_s_year, __pyx_k_year, sizeof(__pyx_k_year), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
@@ -7775,293 +7779,293 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "wrapper.pyx":313
+  /* "fatfs/wrapper.pyx":313
  *                 __diskio_wrapper_disks[i] = disk
  *                 break
  *             raise FatFSException("__init__", -1)             # <<<<<<<<<<<<<<
  *     def _adjust_path(self, path):
  *         """
  */
   __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_u_init, __pyx_int_neg_1); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "wrapper.pyx":125
+  /* "fatfs/wrapper.pyx":125
  * 
  * # Open or create a file
  * def pyf_open (FIL_Handle fph, const TCHAR* path, BYTE mode) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_open(fph.fp, path, mode)
  * 
  */
   __pyx_tuple__7 = PyTuple_Pack(3, __pyx_n_s_fph, __pyx_n_s_path, __pyx_n_s_mode); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
   __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_pyf_open, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 125, __pyx_L1_error)
 
-  /* "wrapper.pyx":129
+  /* "fatfs/wrapper.pyx":129
  * 
  * # Close an open file object
  * def pyf_close (FIL_Handle fph) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_close(fph.fp)
  * 
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_fph); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
   __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_pyf_close, 129, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 129, __pyx_L1_error)
 
-  /* "wrapper.pyx":136
+  /* "fatfs/wrapper.pyx":136
  * #    raise Exception("Not implemented.")
  * ## Write data to the file
  * def pyf_write (FIL_Handle fph, data) -> FRESULT:             # <<<<<<<<<<<<<<
  *     assert isinstance(data, (bytes, bytearray))
  *     cdef UINT written
  */
   __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_fph, __pyx_n_s_data, __pyx_n_s_written, __pyx_n_s_dataptr, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
   __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_pyf_write, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 136, __pyx_L1_error)
 
-  /* "wrapper.pyx":170
+  /* "fatfs/wrapper.pyx":170
  * #    raise Exception("Not implemented.")
  * ## Create a sub directory
  * def pyf_mkdir (path) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_mkdir(path)
  * ## Delete an existing file or directory
  */
   __pyx_tuple__13 = PyTuple_Pack(1, __pyx_n_s_path); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
   __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_pyf_mkdir, 170, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 170, __pyx_L1_error)
 
-  /* "wrapper.pyx":212
+  /* "fatfs/wrapper.pyx":212
  * #    raise Exception("Not implemented.")
  * # Mount/Unmount a logical drive
  * def pyf_mount (FATFS_Handle fph, const TCHAR* path, BYTE opt) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_mount(fph.fp, path, opt)
  * 
  */
   __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_fph, __pyx_n_s_path, __pyx_n_s_opt); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
   __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_pyf_mount, 212, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 212, __pyx_L1_error)
 
-  /* "wrapper.pyx":216
+  /* "fatfs/wrapper.pyx":216
  * 
  * # Create a FAT volume
  * def pyf_mkfs (path, n_fat = 1, align = 0, n_root = 0, au_size = 0, workarea_size = 512) -> FRESULT:             # <<<<<<<<<<<<<<
  *     """
  *     Create a new FAT filesystem on volum given in path. The optional parameters
  */
   __pyx_tuple__17 = PyTuple_Pack(9, __pyx_n_s_path, __pyx_n_s_n_fat, __pyx_n_s_align, __pyx_n_s_n_root, __pyx_n_s_au_size, __pyx_n_s_workarea_size, __pyx_n_s_buff, __pyx_n_s_opt, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
   __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(6, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_pyf_mkfs, 216, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 216, __pyx_L1_error)
 
-  /* "wrapper.pyx":255
+  /* "fatfs/wrapper.pyx":255
  * from cpython.mem cimport PyMem_Malloc, PyMem_Realloc, PyMem_Free
  * 
  * def fresult_to_name(fresult):             # <<<<<<<<<<<<<<
  *     # TODO: Implement.
  *     return "UNKNOWN_%i" % fresult
  */
   __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_fresult); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
   __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_fresult_to_name, 255, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 255, __pyx_L1_error)
 
-  /* "wrapper.pyx":260
+  /* "fatfs/wrapper.pyx":260
  * 
  * class FatFSException(Exception):
  *     def __init__(self, function, ret, *args):             # <<<<<<<<<<<<<<
  *         self.code = ret
  *         args_str = ", ".join(map(str, args))
  */
   __pyx_tuple__21 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_function, __pyx_n_s_ret, __pyx_n_s_args, __pyx_n_s_args_str, __pyx_n_s_ret_str); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
   __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_init, 260, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 260, __pyx_L1_error)
 
-  /* "wrapper.pyx":268
+  /* "fatfs/wrapper.pyx":268
  * 
  * class FileHandle:
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.isopen = False
  *         self.fp = FIL_Handle()
  */
   __pyx_tuple__23 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
   __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_init, 268, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 268, __pyx_L1_error)
 
-  /* "wrapper.pyx":272
+  /* "fatfs/wrapper.pyx":272
  *         self.fp = FIL_Handle()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         ret = pyf_close(self.fp)
  *         if ret != FR_OK:
  */
   __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
   __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_close, 272, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 272, __pyx_L1_error)
 
-  /* "wrapper.pyx":276
+  /* "fatfs/wrapper.pyx":276
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_tuple__27 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
   __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_enter, 276, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 276, __pyx_L1_error)
 
-  /* "wrapper.pyx":279
+  /* "fatfs/wrapper.pyx":279
  *         return self
  * 
  *     def __exit__(self, except_type, except_value, except_traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
   __pyx_tuple__29 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_except_type, __pyx_n_s_except_value, __pyx_n_s_except_traceback); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
   __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_exit, 279, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 279, __pyx_L1_error)
 
-  /* "wrapper.pyx":282
+  /* "fatfs/wrapper.pyx":282
  *         self.close()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.isopen:
  *             self.close()
  */
   __pyx_tuple__31 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
   __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_dealloc, 282, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 282, __pyx_L1_error)
 
-  /* "wrapper.pyx":286
+  /* "fatfs/wrapper.pyx":286
  *             self.close()
  * 
  *     def write(self, data):             # <<<<<<<<<<<<<<
  *         if isinstance(data, str):
  *             data = bytes(data, 'ascii')
  */
   __pyx_tuple__33 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_ret, __pyx_n_s_written); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
   __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_write, 286, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 286, __pyx_L1_error)
 
-  /* "wrapper.pyx":294
+  /* "fatfs/wrapper.pyx":294
  *         return written
  * 
  *     def read(self, size = -1):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
   __pyx_tuple__35 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_size); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
   __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_read, 294, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 294, __pyx_L1_error)
   __pyx_tuple__37 = PyTuple_Pack(1, ((PyObject *)__pyx_int_neg_1)); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
 
-  /* "wrapper.pyx":299
+  /* "fatfs/wrapper.pyx":299
  * 
  * class Partition():
  *     def __init__(self, disk):             # <<<<<<<<<<<<<<
  *         self.fs = FATFS_Handle()
  *         self.disk = disk
  */
   __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_disk, __pyx_n_s_i); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
   __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_init, 299, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 299, __pyx_L1_error)
 
-  /* "wrapper.pyx":314
+  /* "fatfs/wrapper.pyx":314
  *                 break
  *             raise FatFSException("__init__", -1)
  *     def _adjust_path(self, path):             # <<<<<<<<<<<<<<
  *         """
  *         Adjusts path for use in pyf_ calls: adds partition prefix and converts to bytes.
  */
   __pyx_tuple__40 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_path); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
   __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_adjust_path, 314, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 314, __pyx_L1_error)
 
-  /* "wrapper.pyx":320
+  /* "fatfs/wrapper.pyx":320
  *         return self.pname + bytes(path, 'ascii')
  * 
  *     def mount(self):             # <<<<<<<<<<<<<<
  *         ret = pyf_mount(self.fs, self.pname, 1)
  *         if ret == FR_OK:
  */
   __pyx_tuple__42 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__42);
   __Pyx_GIVEREF(__pyx_tuple__42);
   __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_mount, 320, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 320, __pyx_L1_error)
 
-  /* "wrapper.pyx":327
+  /* "fatfs/wrapper.pyx":327
  *             raise FatFSException("mount", ret, self.pname)
  * 
  *     def unmount(self):             # <<<<<<<<<<<<<<
  *         ret = f_mount(NULL, self.pname, 0)
  *         if ret == FR_OK:
  */
   __pyx_tuple__44 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__44);
   __Pyx_GIVEREF(__pyx_tuple__44);
   __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_unmount, 327, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 327, __pyx_L1_error)
 
-  /* "wrapper.pyx":335
+  /* "fatfs/wrapper.pyx":335
  *             raise FatFSException("unmount", ret, self.pname)
  * 
  *     def mkfs(self):             # <<<<<<<<<<<<<<
  *         pyf_mkfs(self.pname)
  * 
  */
   __pyx_tuple__46 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__46);
   __Pyx_GIVEREF(__pyx_tuple__46);
   __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_mkfs, 335, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 335, __pyx_L1_error)
 
-  /* "wrapper.pyx":338
+  /* "fatfs/wrapper.pyx":338
  *         pyf_mkfs(self.pname)
  * 
  *     def mkdir(self, path):             # <<<<<<<<<<<<<<
  *         p = self._adjust_path(path)
  *         ret = pyf_mkdir(p)
  */
   __pyx_tuple__48 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_p, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__48);
   __Pyx_GIVEREF(__pyx_tuple__48);
   __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_mkdir, 338, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 338, __pyx_L1_error)
 
-  /* "wrapper.pyx":345
+  /* "fatfs/wrapper.pyx":345
  *             raise FatFSException("mount", ret, p)
  * 
  *     def open(self, path, mode):             # <<<<<<<<<<<<<<
  *         # TODO: Implement mode.
  *         handle = FileHandle()
  */
   __pyx_tuple__50 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_mode, __pyx_n_s_handle, __pyx_n_s_p, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__50);
   __Pyx_GIVEREF(__pyx_tuple__50);
   __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(3, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fatfs_wrapper_pyx, __pyx_n_s_open, 345, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 345, __pyx_L1_error)
 
-  /* "wrapper.pyx":355
+  /* "fatfs/wrapper.pyx":355
  *         return handle
  * 
  * def check_diskio(drive):             # <<<<<<<<<<<<<<
  *     assert(not 0 in __diskio_wrapper_disks, "Check diskio must be used before mounting any real drives.")
  *     __diskio_wrapper_disks[0] = drive
  */
   __pyx_tuple__52 = PyTuple_Pack(2, __pyx_n_s_drive, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 355, __pyx_L1_error)
@@ -8072,15 +8076,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_5 = PyInt_FromLong(5); if (unlikely(!__pyx_int_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_21 = PyInt_FromLong(21); if (unlikely(!__pyx_int_21)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_25 = PyInt_FromLong(25); if (unlikely(!__pyx_int_25)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8127,34 +8131,34 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_7wrapper_FIL_Handle) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5fatfs_7wrapper_FIL_Handle) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_7wrapper_FIL_Handle.tp_print = 0;
+  __pyx_type_5fatfs_7wrapper_FIL_Handle.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7wrapper_FIL_Handle.tp_dictoffset && __pyx_type_7wrapper_FIL_Handle.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_7wrapper_FIL_Handle.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5fatfs_7wrapper_FIL_Handle.tp_dictoffset && __pyx_type_5fatfs_7wrapper_FIL_Handle.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_5fatfs_7wrapper_FIL_Handle.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FIL_Handle, (PyObject *)&__pyx_type_7wrapper_FIL_Handle) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7wrapper_FIL_Handle) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
-  __pyx_ptype_7wrapper_FIL_Handle = &__pyx_type_7wrapper_FIL_Handle;
-  if (PyType_Ready(&__pyx_type_7wrapper_FATFS_Handle) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FIL_Handle, (PyObject *)&__pyx_type_5fatfs_7wrapper_FIL_Handle) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5fatfs_7wrapper_FIL_Handle) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_ptype_5fatfs_7wrapper_FIL_Handle = &__pyx_type_5fatfs_7wrapper_FIL_Handle;
+  if (PyType_Ready(&__pyx_type_5fatfs_7wrapper_FATFS_Handle) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_7wrapper_FATFS_Handle.tp_print = 0;
+  __pyx_type_5fatfs_7wrapper_FATFS_Handle.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7wrapper_FATFS_Handle.tp_dictoffset && __pyx_type_7wrapper_FATFS_Handle.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_7wrapper_FATFS_Handle.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5fatfs_7wrapper_FATFS_Handle.tp_dictoffset && __pyx_type_5fatfs_7wrapper_FATFS_Handle.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_5fatfs_7wrapper_FATFS_Handle.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FATFS_Handle, (PyObject *)&__pyx_type_7wrapper_FATFS_Handle) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7wrapper_FATFS_Handle) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
-  __pyx_ptype_7wrapper_FATFS_Handle = &__pyx_type_7wrapper_FATFS_Handle;
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FATFS_Handle, (PyObject *)&__pyx_type_5fatfs_7wrapper_FATFS_Handle) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5fatfs_7wrapper_FATFS_Handle) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_ptype_5fatfs_7wrapper_FATFS_Handle = &__pyx_type_5fatfs_7wrapper_FATFS_Handle;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -8347,28 +8351,28 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_wrapper) {
+  if (__pyx_module_is_main_fatfs__wrapper) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "wrapper")) {
-      if (unlikely(PyDict_SetItemString(modules, "wrapper", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "fatfs.wrapper")) {
+      if (unlikely(PyDict_SetItemString(modules, "fatfs.wrapper", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8381,394 +8385,394 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "wrapper.pyx":6
+  /* "fatfs/wrapper.pyx":6
  * #from pyfatfs.diskio import RamDisk
  * 
  * __diskio_wrapper_disks = {}             # <<<<<<<<<<<<<<
  * 
  * cdef DSTATUS disk_initialize (BYTE pdrv):
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_diskio_wrapper_disks, __pyx_t_1) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":62
+  /* "fatfs/wrapper.pyx":62
  * cdef extern int diskiocheck()
  * 
  * import datetime             # <<<<<<<<<<<<<<
  * 
  * cdef extern from "diskio.h":
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_datetime, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_datetime, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":125
+  /* "fatfs/wrapper.pyx":125
  * 
  * # Open or create a file
  * def pyf_open (FIL_Handle fph, const TCHAR* path, BYTE mode) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_open(fph.fp, path, mode)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7wrapper_1pyf_open, NULL, __pyx_n_s_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5fatfs_7wrapper_1pyf_open, NULL, __pyx_n_s_fatfs_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyf_open, __pyx_t_1) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":129
+  /* "fatfs/wrapper.pyx":129
  * 
  * # Close an open file object
  * def pyf_close (FIL_Handle fph) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_close(fph.fp)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7wrapper_3pyf_close, NULL, __pyx_n_s_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5fatfs_7wrapper_3pyf_close, NULL, __pyx_n_s_fatfs_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyf_close, __pyx_t_1) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":136
+  /* "fatfs/wrapper.pyx":136
  * #    raise Exception("Not implemented.")
  * ## Write data to the file
  * def pyf_write (FIL_Handle fph, data) -> FRESULT:             # <<<<<<<<<<<<<<
  *     assert isinstance(data, (bytes, bytearray))
  *     cdef UINT written
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7wrapper_5pyf_write, NULL, __pyx_n_s_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5fatfs_7wrapper_5pyf_write, NULL, __pyx_n_s_fatfs_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyf_write, __pyx_t_1) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":170
+  /* "fatfs/wrapper.pyx":170
  * #    raise Exception("Not implemented.")
  * ## Create a sub directory
  * def pyf_mkdir (path) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_mkdir(path)
  * ## Delete an existing file or directory
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7wrapper_7pyf_mkdir, NULL, __pyx_n_s_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5fatfs_7wrapper_7pyf_mkdir, NULL, __pyx_n_s_fatfs_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyf_mkdir, __pyx_t_1) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":212
+  /* "fatfs/wrapper.pyx":212
  * #    raise Exception("Not implemented.")
  * # Mount/Unmount a logical drive
  * def pyf_mount (FATFS_Handle fph, const TCHAR* path, BYTE opt) -> FRESULT:             # <<<<<<<<<<<<<<
  *     return f_mount(fph.fp, path, opt)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7wrapper_9pyf_mount, NULL, __pyx_n_s_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5fatfs_7wrapper_9pyf_mount, NULL, __pyx_n_s_fatfs_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyf_mount, __pyx_t_1) < 0) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":216
+  /* "fatfs/wrapper.pyx":216
  * 
  * # Create a FAT volume
  * def pyf_mkfs (path, n_fat = 1, align = 0, n_root = 0, au_size = 0, workarea_size = 512) -> FRESULT:             # <<<<<<<<<<<<<<
  *     """
  *     Create a new FAT filesystem on volum given in path. The optional parameters
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7wrapper_11pyf_mkfs, NULL, __pyx_n_s_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5fatfs_7wrapper_11pyf_mkfs, NULL, __pyx_n_s_fatfs_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyf_mkfs, __pyx_t_1) < 0) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":255
+  /* "fatfs/wrapper.pyx":255
  * from cpython.mem cimport PyMem_Malloc, PyMem_Realloc, PyMem_Free
  * 
  * def fresult_to_name(fresult):             # <<<<<<<<<<<<<<
  *     # TODO: Implement.
  *     return "UNKNOWN_%i" % fresult
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7wrapper_13fresult_to_name, NULL, __pyx_n_s_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5fatfs_7wrapper_13fresult_to_name, NULL, __pyx_n_s_fatfs_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_fresult_to_name, __pyx_t_1) < 0) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":259
+  /* "fatfs/wrapper.pyx":259
  *     return "UNKNOWN_%i" % fresult
  * 
  * class FatFSException(Exception):             # <<<<<<<<<<<<<<
  *     def __init__(self, function, ret, *args):
  *         self.code = ret
  */
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_FatFSException, __pyx_n_s_FatFSException, (PyObject *) NULL, __pyx_n_s_wrapper, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_FatFSException, __pyx_n_s_FatFSException, (PyObject *) NULL, __pyx_n_s_fatfs_wrapper, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "wrapper.pyx":260
+  /* "fatfs/wrapper.pyx":260
  * 
  * class FatFSException(Exception):
  *     def __init__(self, function, ret, *args):             # <<<<<<<<<<<<<<
  *         self.code = ret
  *         args_str = ", ".join(map(str, args))
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_14FatFSException_1__init__, 0, __pyx_n_s_FatFSException___init, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_14FatFSException_1__init__, 0, __pyx_n_s_FatFSException___init, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "wrapper.pyx":259
+  /* "fatfs/wrapper.pyx":259
  *     return "UNKNOWN_%i" % fresult
  * 
  * class FatFSException(Exception):             # <<<<<<<<<<<<<<
  *     def __init__(self, function, ret, *args):
  *         self.code = ret
  */
   __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_FatFSException, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FatFSException, __pyx_t_4) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":267
+  /* "fatfs/wrapper.pyx":267
  *     pass
  * 
  * class FileHandle:             # <<<<<<<<<<<<<<
  *     def __init__(self):
  *         self.isopen = False
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_FileHandle, __pyx_n_s_FileHandle, (PyObject *) NULL, __pyx_n_s_wrapper, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_FileHandle, __pyx_n_s_FileHandle, (PyObject *) NULL, __pyx_n_s_fatfs_wrapper, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "wrapper.pyx":268
+  /* "fatfs/wrapper.pyx":268
  * 
  * class FileHandle:
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.isopen = False
  *         self.fp = FIL_Handle()
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_10FileHandle_1__init__, 0, __pyx_n_s_FileHandle___init, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_10FileHandle_1__init__, 0, __pyx_n_s_FileHandle___init, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":272
+  /* "fatfs/wrapper.pyx":272
  *         self.fp = FIL_Handle()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         ret = pyf_close(self.fp)
  *         if ret != FR_OK:
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_10FileHandle_3close, 0, __pyx_n_s_FileHandle_close, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_10FileHandle_3close, 0, __pyx_n_s_FileHandle_close, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_close, __pyx_t_2) < 0) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":276
+  /* "fatfs/wrapper.pyx":276
  *         if ret != FR_OK:
  *             raise FatFSException("FatFS::close failed with error code %s" % ret)
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_10FileHandle_5__enter__, 0, __pyx_n_s_FileHandle___enter, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_10FileHandle_5__enter__, 0, __pyx_n_s_FileHandle___enter, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_enter, __pyx_t_2) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":279
+  /* "fatfs/wrapper.pyx":279
  *         return self
  * 
  *     def __exit__(self, except_type, except_value, except_traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_10FileHandle_7__exit__, 0, __pyx_n_s_FileHandle___exit, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_10FileHandle_7__exit__, 0, __pyx_n_s_FileHandle___exit, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_exit, __pyx_t_2) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":282
+  /* "fatfs/wrapper.pyx":282
  *         self.close()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.isopen:
  *             self.close()
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_10FileHandle_9__dealloc__, 0, __pyx_n_s_FileHandle___dealloc, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_10FileHandle_9__dealloc__, 0, __pyx_n_s_FileHandle___dealloc, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_dealloc, __pyx_t_2) < 0) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":286
+  /* "fatfs/wrapper.pyx":286
  *             self.close()
  * 
  *     def write(self, data):             # <<<<<<<<<<<<<<
  *         if isinstance(data, str):
  *             data = bytes(data, 'ascii')
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_10FileHandle_11write, 0, __pyx_n_s_FileHandle_write, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_10FileHandle_11write, 0, __pyx_n_s_FileHandle_write, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_write, __pyx_t_2) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":294
+  /* "fatfs/wrapper.pyx":294
  *         return written
  * 
  *     def read(self, size = -1):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_10FileHandle_13read, 0, __pyx_n_s_FileHandle_read, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_10FileHandle_13read, 0, __pyx_n_s_FileHandle_read, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__37);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_read, __pyx_t_2) < 0) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":267
+  /* "fatfs/wrapper.pyx":267
  *     pass
  * 
  * class FileHandle:             # <<<<<<<<<<<<<<
  *     def __init__(self):
  *         self.isopen = False
  */
   __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_FileHandle, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FileHandle, __pyx_t_2) < 0) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":298
+  /* "fatfs/wrapper.pyx":298
  * 
  * 
  * class Partition():             # <<<<<<<<<<<<<<
  *     def __init__(self, disk):
  *         self.fs = FATFS_Handle()
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Partition, __pyx_n_s_Partition, (PyObject *) NULL, __pyx_n_s_wrapper, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Partition, __pyx_n_s_Partition, (PyObject *) NULL, __pyx_n_s_fatfs_wrapper, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "wrapper.pyx":299
+  /* "fatfs/wrapper.pyx":299
  * 
  * class Partition():
  *     def __init__(self, disk):             # <<<<<<<<<<<<<<
  *         self.fs = FATFS_Handle()
  *         self.disk = disk
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_9Partition_1__init__, 0, __pyx_n_s_Partition___init, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_9Partition_1__init__, 0, __pyx_n_s_Partition___init, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":314
+  /* "fatfs/wrapper.pyx":314
  *                 break
  *             raise FatFSException("__init__", -1)
  *     def _adjust_path(self, path):             # <<<<<<<<<<<<<<
  *         """
  *         Adjusts path for use in pyf_ calls: adds partition prefix and converts to bytes.
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_9Partition_3_adjust_path, 0, __pyx_n_s_Partition__adjust_path, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_9Partition_3_adjust_path, 0, __pyx_n_s_Partition__adjust_path, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_adjust_path, __pyx_t_2) < 0) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":320
+  /* "fatfs/wrapper.pyx":320
  *         return self.pname + bytes(path, 'ascii')
  * 
  *     def mount(self):             # <<<<<<<<<<<<<<
  *         ret = pyf_mount(self.fs, self.pname, 1)
  *         if ret == FR_OK:
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_9Partition_5mount, 0, __pyx_n_s_Partition_mount, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_9Partition_5mount, 0, __pyx_n_s_Partition_mount, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_mount, __pyx_t_2) < 0) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":327
+  /* "fatfs/wrapper.pyx":327
  *             raise FatFSException("mount", ret, self.pname)
  * 
  *     def unmount(self):             # <<<<<<<<<<<<<<
  *         ret = f_mount(NULL, self.pname, 0)
  *         if ret == FR_OK:
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_9Partition_7unmount, 0, __pyx_n_s_Partition_unmount, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_9Partition_7unmount, 0, __pyx_n_s_Partition_unmount, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_unmount, __pyx_t_2) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":335
+  /* "fatfs/wrapper.pyx":335
  *             raise FatFSException("unmount", ret, self.pname)
  * 
  *     def mkfs(self):             # <<<<<<<<<<<<<<
  *         pyf_mkfs(self.pname)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_9Partition_9mkfs, 0, __pyx_n_s_Partition_mkfs, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_9Partition_9mkfs, 0, __pyx_n_s_Partition_mkfs, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_mkfs, __pyx_t_2) < 0) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":338
+  /* "fatfs/wrapper.pyx":338
  *         pyf_mkfs(self.pname)
  * 
  *     def mkdir(self, path):             # <<<<<<<<<<<<<<
  *         p = self._adjust_path(path)
  *         ret = pyf_mkdir(p)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_9Partition_11mkdir, 0, __pyx_n_s_Partition_mkdir, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_9Partition_11mkdir, 0, __pyx_n_s_Partition_mkdir, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_mkdir, __pyx_t_2) < 0) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":345
+  /* "fatfs/wrapper.pyx":345
  *             raise FatFSException("mount", ret, p)
  * 
  *     def open(self, path, mode):             # <<<<<<<<<<<<<<
  *         # TODO: Implement mode.
  *         handle = FileHandle()
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_9Partition_13open, 0, __pyx_n_s_Partition_open, NULL, __pyx_n_s_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5fatfs_7wrapper_9Partition_13open, 0, __pyx_n_s_Partition_open, NULL, __pyx_n_s_fatfs_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_open, __pyx_t_2) < 0) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "wrapper.pyx":298
+  /* "fatfs/wrapper.pyx":298
  * 
  * 
  * class Partition():             # <<<<<<<<<<<<<<
  *     def __init__(self, disk):
  *         self.fs = FATFS_Handle()
  */
   __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Partition, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Partition, __pyx_t_2) < 0) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":355
+  /* "fatfs/wrapper.pyx":355
  *         return handle
  * 
  * def check_diskio(drive):             # <<<<<<<<<<<<<<
  *     assert(not 0 in __diskio_wrapper_disks, "Check diskio must be used before mounting any real drives.")
  *     __diskio_wrapper_disks[0] = drive
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7wrapper_15check_diskio, NULL, __pyx_n_s_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5fatfs_7wrapper_15check_diskio, NULL, __pyx_n_s_fatfs_wrapper); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_check_diskio, __pyx_t_1) < 0) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "wrapper.pyx":1
+  /* "fatfs/wrapper.pyx":1
  * from fatfs.ff cimport *             # <<<<<<<<<<<<<<
  * from fatfs.diskio cimport *
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8780,19 +8784,19 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init fatfs.wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init wrapper");
+    PyErr_SetString(PyExc_ImportError, "init fatfs.wrapper");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -8939,17 +8943,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -9224,15 +9226,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -9850,28 +9852,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -10106,18 +10108,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* SetItemInt */
 static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
     int r;
     if (!j) return -1;
     r = PyObject_SetItem(o, j, v);
@@ -11035,17 +11035,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -11112,15 +11117,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -11231,15 +11239,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -11540,15 +11548,15 @@
                         } else if (8 * sizeof(BYTE) >= 4 * PyLong_SHIFT) {
                             return (BYTE) (((((((((BYTE)digits[3]) << PyLong_SHIFT) | (BYTE)digits[2]) << PyLong_SHIFT) | (BYTE)digits[1]) << PyLong_SHIFT) | (BYTE)digits[0]));
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
@@ -11850,15 +11858,15 @@
                         } else if (8 * sizeof(UINT) >= 4 * PyLong_SHIFT) {
                             return (UINT) (((((((((UINT)digits[3]) << PyLong_SHIFT) | (UINT)digits[2]) << PyLong_SHIFT) | (UINT)digits[1]) << PyLong_SHIFT) | (UINT)digits[0]));
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
@@ -12046,15 +12054,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
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
@@ -12242,15 +12250,15 @@
                         } else if (8 * sizeof(uint16_t) >= 4 * PyLong_SHIFT) {
                             return (uint16_t) (((((((((uint16_t)digits[3]) << PyLong_SHIFT) | (uint16_t)digits[2]) << PyLong_SHIFT) | (uint16_t)digits[1]) << PyLong_SHIFT) | (uint16_t)digits[0]));
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
@@ -12476,15 +12484,15 @@
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
@@ -12748,15 +12756,15 @@
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
@@ -12944,15 +12952,15 @@
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
```

### Comparing `fatfs-0.0.6/fatfs.egg-info/PKG-INFO` & `fatfs-0.0.7/fatfs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fatfs
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper around ChaN's FatFS library for FAT filesystem manipulation.
 Home-page: https://github.com/krakonos/fatfs-python
 Author: Ladislav Laska
 Author-email: krakonos@krakonos.org
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # FatFS wrapper for Python
 
 This library provides a Python wrapper around [ChaN's FatFS](http://elm-chan.org/fsw/ff/00index_e.html) library.
```

### Comparing `fatfs-0.0.6/foreign/fatfs/source/diskio.h` & `fatfs-0.0.7/foreign/fatfs/source/diskio.h`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/foreign/fatfs/source/ff.c` & `fatfs-0.0.7/foreign/fatfs/source/ff.c`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/foreign/fatfs/source/ff.h` & `fatfs-0.0.7/foreign/fatfs/source/ff.h`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/foreign/fatfs/source/ffconf.h` & `fatfs-0.0.7/foreign/fatfs/source/ffconf.h`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/foreign/fatfs/source/ffsystem.c` & `fatfs-0.0.7/foreign/fatfs/source/ffsystem.c`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/foreign/fatfs/source/ffunicode.c` & `fatfs-0.0.7/foreign/fatfs/source/ffunicode.c`

 * *Files identical despite different names*

### Comparing `fatfs-0.0.6/setup.py` & `fatfs-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,41 +29,46 @@
     return extensions
 
 
 extensions = [
     Extension("wrapper", ["fatfs/wrapper.pyx", "fatfs/diskiocheck.c", "foreign/fatfs/source/ff.c", "foreign/fatfs/source/ffsystem.c", "foreign/fatfs/source/ffunicode.c"], include_dirs=["foreign/fatfs/source"]),
 ]
 
-CYTHONIZE = bool(int(os.getenv("CYTHONIZE", 0))) and cythonize is not None
+cythonize_env = bool(int(os.getenv("CYTHONIZE", 0)))
+
+if cythonize_env and cythonize_env is None:
+    raise Exception("Cython needs to be installed for CYTHONIZE=1")
+
+CYTHONIZE = cythonize_env and cythonize is not None
 
 if CYTHONIZE:
     compiler_directives = {"language_level": 3, "embedsignature": True}
     extensions = cythonize(extensions, compiler_directives=compiler_directives)
 else:
     extensions = no_cythonize(extensions)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='fatfs',
-    version="0.0.6",
+    version="0.0.7",
     author="Ladislav Laska",
     author_email="krakonos@krakonos.org",
     description="A wrapper around ChaN's FatFS library for FAT filesystem manipulation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_package='fatfs',
     ext_modules=extensions,
     url="https://github.com/krakonos/fatfs-python",
     #packages=['pyfatfs', 'pyfatfs.tests'],
     packages=find_packages(),
-    install_requires=['cython'],
+    setup_requires=['cython'],
     zip_safe=False,
-    python_requires='>=3.6', #TODO: Actual version?
+    python_requires='>=3.8',
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
```

