# Comparing `tmp/xia_cache-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_cache-0.1.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 135481 bytes, number of entries: 7
--rw-r--r--  2.0 unx      114 b- defN 23-Jun-26 17:34 xia_cache/__init__.py
--rw-r--r--  2.0 unx   349184 b- defN 23-Jun-26 17:37 xia_cache/cache.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 17:37 xia_cache-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      748 b- defN 23-Jun-26 17:37 xia_cache-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 17:37 xia_cache-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-26 17:37 xia_cache-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      568 b- defN 23-Jun-26 17:37 xia_cache-0.1.3.dist-info/RECORD
-7 files, 350874 bytes uncompressed, 134471 bytes compressed:  61.7%
+Zip file size: 2828 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-29 20:35 xia_cache/__init__.py
+-rw-r--r--  2.0 unx     3965 b- defN 23-Jun-29 20:04 xia_cache/cache.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:40 xia_cache-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      748 b- defN 23-Jun-29 20:40 xia_cache-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:40 xia_cache-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-29 20:40 xia_cache-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      550 b- defN 23-Jun-29 20:40 xia_cache-0.1.4.dist-info/RECORD
+7 files, 5636 bytes uncompressed, 1850 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_cache/__init__.py
 Comment: 
 
-Filename: xia_cache/cache.cp39-win_amd64.pyd
+Filename: xia_cache/cache.py
 Comment: 
 
-Filename: xia_cache-0.1.3.dist-info/LICENSE.txt
+Filename: xia_cache-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_cache-0.1.3.dist-info/METADATA
+Filename: xia_cache-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_cache-0.1.3.dist-info/WHEEL
+Filename: xia_cache-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_cache-0.1.3.dist-info/top_level.txt
+Filename: xia_cache-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_cache-0.1.3.dist-info/RECORD
+Filename: xia_cache-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_cache/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_cache.cache import Cache, LruRamCache
 
 
 __all__ = [
     "Cache", "LruRamCache",
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## Comparing `xia_cache-0.1.3.dist-info/METADATA` & `xia_cache-0.1.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-cache
-Version: 0.1.3
+Version: 0.1.4
 Summary: X-I-A Cache
-Home-page: https://develop.x-i-a.com/docs/xia-cache/0.1.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-cache/0.1.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

