# Comparing `tmp/xia_engine_firestore-0.3.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_firestore-0.3.6-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4302 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-29 20:44 xia_engine_firestore/__init__.py
--rw-r--r--  2.0 unx     9905 b- defN 23-Jun-29 20:44 xia_engine_firestore/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:46 xia_engine_firestore-0.3.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      817 b- defN 23-Jun-29 20:46 xia_engine_firestore-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:46 xia_engine_firestore-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-29 20:46 xia_engine_firestore-0.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      628 b- defN 23-Jun-29 20:46 xia_engine_firestore-0.3.5.dist-info/RECORD
-7 files, 11737 bytes uncompressed, 3168 bytes compressed:  73.0%
+Zip file size: 4197 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-30 11:25 xia_engine_firestore/__init__.py
+-rw-r--r--  2.0 unx     9905 b- defN 23-Jun-29 14:06 xia_engine_firestore/engine.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:25 xia_engine_firestore-0.3.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      470 b- defN 23-Jun-30 11:25 xia_engine_firestore-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:25 xia_engine_firestore-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-30 11:25 xia_engine_firestore-0.3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      629 b- defN 23-Jun-30 11:25 xia_engine_firestore-0.3.6.dist-info/RECORD
+7 files, 11400 bytes uncompressed, 3063 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_firestore/__init__.py
 Comment: 
 
 Filename: xia_engine_firestore/engine.py
 Comment: 
 
-Filename: xia_engine_firestore-0.3.5.dist-info/LICENSE.txt
+Filename: xia_engine_firestore-0.3.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.3.5.dist-info/METADATA
+Filename: xia_engine_firestore-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_firestore-0.3.5.dist-info/WHEEL
+Filename: xia_engine_firestore-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_firestore-0.3.5.dist-info/top_level.txt
+Filename: xia_engine_firestore-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.3.5.dist-info/RECORD
+Filename: xia_engine_firestore-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_firestore/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_firestore.engine import FirestoreEngine
 
 
 __all__ = [
     "FirestoreEngine"
 ]
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
```

