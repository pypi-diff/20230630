# Comparing `tmp/xia_broadcast_fastapi-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_broadcast_fastapi-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3840 bytes, number of entries: 7
--rw-r--r--  2.0 unx      129 b- defN 23-Jun-29 20:33 xia_broadcast_fastapi/__init__.py
+Zip file size: 3698 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-30 11:15 xia_broadcast_fastapi/__init__.py
 -rw-r--r--  2.0 unx     4771 b- defN 23-Jun-29 20:33 xia_broadcast_fastapi/broadcaster.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      900 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      640 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/RECORD
-7 files, 6712 bytes uncompressed, 2682 bytes compressed:  60.0%
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      640 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/RECORD
+7 files, 6298 bytes uncompressed, 2540 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_broadcast_fastapi/__init__.py
 Comment: 
 
 Filename: xia_broadcast_fastapi/broadcaster.py
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.1.dist-info/LICENSE.txt
+Filename: xia_broadcast_fastapi-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.1.dist-info/METADATA
+Filename: xia_broadcast_fastapi-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.1.dist-info/WHEEL
+Filename: xia_broadcast_fastapi-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.1.dist-info/top_level.txt
+Filename: xia_broadcast_fastapi-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.1.dist-info/RECORD
+Filename: xia_broadcast_fastapi-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_broadcast_fastapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_broadcast_fastapi.broadcaster import BroadcasterFastapi
 
 
 __all__ = [
     "BroadcasterFastapi",
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_broadcast_fastapi-0.1.1.dist-info/RECORD` & `xia_broadcast_fastapi-0.1.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_broadcast_fastapi/__init__.py,sha256=ywMWnVZ5GvlYc8VZNp-A8muh_tz1-Khasx-ReGL9WWk,129
+xia_broadcast_fastapi/__init__.py,sha256=EPZasv_pqpaN2qad7GC3JivvoNA-Z0nUMjlMTJaOmUw,129
 xia_broadcast_fastapi/broadcaster.py,sha256=eGRCKnE6Elx2QArLCgLadsOvjeyeGQ6EUK9xbV6W4hk,4771
-xia_broadcast_fastapi-0.1.1.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_broadcast_fastapi-0.1.1.dist-info/METADATA,sha256=pjJmYF6D3fvCfUFec_9WmhgKNJZ9EkNexVqai5perg8,900
-xia_broadcast_fastapi-0.1.1.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_broadcast_fastapi-0.1.1.dist-info/top_level.txt,sha256=t1WhzbP6ZYMQR5rAS86UFjQkSu3TvquMHCAklcm7YlA,22
-xia_broadcast_fastapi-0.1.1.dist-info/RECORD,,
+xia_broadcast_fastapi-0.1.2.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_broadcast_fastapi-0.1.2.dist-info/METADATA,sha256=zHxysQYBPHOujVyBN9i-FqgfSoE6VBDE7kjI3ZibT04,486
+xia_broadcast_fastapi-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_broadcast_fastapi-0.1.2.dist-info/top_level.txt,sha256=t1WhzbP6ZYMQR5rAS86UFjQkSu3TvquMHCAklcm7YlA,22
+xia_broadcast_fastapi-0.1.2.dist-info/RECORD,,
```

