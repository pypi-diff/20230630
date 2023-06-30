# Comparing `tmp/fuzzy-hash-0.0.1.tar.gz` & `tmp/fuzzy-hash-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuzzy-hash-0.0.1.tar", last modified: Sun Jun 25 03:25:40 2023, max compression
+gzip compressed data, was "dist/fuzzy-hash-0.0.2.tar", last modified: Fri Jun 30 11:05:42 2023, max compression
```

## Comparing `fuzzy-hash-0.0.1.tar` & `fuzzy-hash-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-25 03:25:40.911349 fuzzy-hash-0.0.1/
--rw-r--r--   0 guofei     (501) staff       (20)       77 2023-06-25 03:25:40.911068 fuzzy-hash-0.0.1/PKG-INFO
--rw-r--r--   0 guofei     (501) staff       (20)     1893 2023-06-25 03:22:31.000000 fuzzy-hash-0.0.1/README.md
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-25 03:25:40.908540 fuzzy-hash-0.0.1/fuzzy_hash/
--rw-r--r--   0 guofei     (501) staff       (20)      711 2023-06-25 03:17:27.000000 fuzzy-hash-0.0.1/fuzzy_hash/__init__.py
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-25 03:25:40.910731 fuzzy-hash-0.0.1/fuzzy_hash/lib/
--rw-r--r--   0 guofei     (501) staff       (20)      270 2023-06-29 02:01:03.000000 fuzzy-hash-0.0.1/fuzzy_hash/lib/__init__.py
--rw-r--r--   0 guofei     (501) staff       (20)     2792 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.1/fuzzy_hash/lib/edit_dist.c
--rw-r--r--   0 guofei     (501) staff       (20)    29209 2023-06-27 09:54:55.000000 fuzzy-hash-0.0.1/fuzzy_hash/lib/fuzzy.c
--rw-r--r--   0 guofei     (501) staff       (20)      220 2023-06-29 01:42:31.000000 fuzzy-hash-0.0.1/fuzzy_hash/lib/setup.py
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-25 03:25:40.909376 fuzzy-hash-0.0.1/fuzzy_hash.egg-info/
--rw-r--r--   0 guofei     (501) staff       (20)       77 2023-06-25 03:25:40.000000 fuzzy-hash-0.0.1/fuzzy_hash.egg-info/PKG-INFO
--rw-r--r--   0 guofei     (501) staff       (20)      278 2023-06-25 03:25:40.000000 fuzzy-hash-0.0.1/fuzzy_hash.egg-info/SOURCES.txt
--rw-r--r--   0 guofei     (501) staff       (20)        1 2023-06-25 03:25:40.000000 fuzzy-hash-0.0.1/fuzzy_hash.egg-info/dependency_links.txt
--rw-r--r--   0 guofei     (501) staff       (20)       11 2023-06-25 03:25:40.000000 fuzzy-hash-0.0.1/fuzzy_hash.egg-info/top_level.txt
--rw-r--r--   0 guofei     (501) staff       (20)       38 2023-06-25 03:25:40.911433 fuzzy-hash-0.0.1/setup.cfg
--rw-r--r--   0 guofei     (501) staff       (20)      418 2023-06-25 03:25:37.000000 fuzzy-hash-0.0.1/setup.py
+drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-30 11:05:42.695262 fuzzy-hash-0.0.2/
+-rw-r--r--   0 guofei     (501) staff       (20)       26 2023-06-30 10:56:15.000000 fuzzy-hash-0.0.2/MANIFEST.in
+-rw-r--r--   0 guofei     (501) staff       (20)      107 2023-06-30 11:05:42.695016 fuzzy-hash-0.0.2/PKG-INFO
+-rw-r--r--   0 guofei     (501) staff       (20)     1898 2023-06-30 03:28:20.000000 fuzzy-hash-0.0.2/README.md
+drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-30 11:05:42.692405 fuzzy-hash-0.0.2/fuzzy_hash/
+-rw-r--r--   0 guofei     (501) staff       (20)      711 2023-06-30 10:56:52.000000 fuzzy-hash-0.0.2/fuzzy_hash/__init__.py
+drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-30 11:05:42.694735 fuzzy-hash-0.0.2/fuzzy_hash/lib/
+-rw-r--r--   0 guofei     (501) staff       (20)      270 2023-06-29 02:01:03.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/__init__.py
+-rw-r--r--   0 guofei     (501) staff       (20)     2792 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/edit_dist.c
+-rw-r--r--   0 guofei     (501) staff       (20)      497 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/edit_dist.h
+-rw-r--r--   0 guofei     (501) staff       (20)    29209 2023-06-27 09:54:55.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/fuzzy.c
+-rw-r--r--   0 guofei     (501) staff       (20)     8004 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/fuzzy.h
+-rw-r--r--   0 guofei     (501) staff       (20)      220 2023-06-29 01:42:31.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/setup.py
+-rw-r--r--   0 guofei     (501) staff       (20)    26778 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/sum_table.h
+drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-30 11:05:42.693257 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/
+-rw-r--r--   0 guofei     (501) staff       (20)      107 2023-06-30 11:05:42.000000 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/PKG-INFO
+-rw-r--r--   0 guofei     (501) staff       (20)      367 2023-06-30 11:05:42.000000 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 guofei     (501) staff       (20)        1 2023-06-30 11:05:42.000000 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 guofei     (501) staff       (20)       11 2023-06-30 11:05:42.000000 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/top_level.txt
+-rw-r--r--   0 guofei     (501) staff       (20)       38 2023-06-30 11:05:42.695340 fuzzy-hash-0.0.2/setup.cfg
+-rw-r--r--   0 guofei     (501) staff       (20)      775 2023-06-30 11:05:26.000000 fuzzy-hash-0.0.2/setup.py
```

### Comparing `fuzzy-hash-0.0.1/README.md` & `fuzzy-hash-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # fuzzy-hash
 
-This project computes fuzzy hash
+This project computes fuzzy hash.  
+
+
 
 
 ```python
 from fuzzy_hash import fuzzy_hash, fuzzy_compare
 
 sentence = '''
 近期，有一部热播硬核电视剧引发全网关注。与其他硬核电视剧不同的是，这部电视剧真的硬“核”，含“核”量高达100%。这就是《许你万家灯火》——首部全景反映我国核电工业发展历程的电视剧。
```

### Comparing `fuzzy-hash-0.0.1/fuzzy_hash/__init__.py` & `fuzzy-hash-0.0.2/fuzzy_hash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ctypes
 import os
 from .lib import core
 from ctypes import c_char_p, c_uint32, create_string_buffer
 
 module_path = os.path.dirname(__file__)
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 fuzzy_hash_buff = core.fuzzy_hash_buf
 fuzzy_hash_buff.argtypes = [c_char_p, c_uint32, c_char_p]
 fuzzy_hash_buff.restype = c_uint32
 
 
 def fuzzy_hash(buf):
```

### Comparing `fuzzy-hash-0.0.1/fuzzy_hash/lib/edit_dist.c` & `fuzzy-hash-0.0.2/fuzzy_hash/lib/edit_dist.c`

 * *Files identical despite different names*

### Comparing `fuzzy-hash-0.0.1/fuzzy_hash/lib/fuzzy.c` & `fuzzy-hash-0.0.2/fuzzy_hash/lib/fuzzy.c`

 * *Files identical despite different names*

