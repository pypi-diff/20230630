# Comparing `tmp/xia_gpt-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_gpt-0.1.3-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2391 bytes, number of entries: 7
--rw-r--r--  2.0 unx       75 b- defN 23-Jun-29 20:48 xia_gpt/__init__.py
--rw-r--r--  2.0 unx     1049 b- defN 23-Jun-29 20:48 xia_gpt/gpt.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:52 xia_gpt-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      600 b- defN 23-Jun-29 20:52 xia_gpt-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:52 xia_gpt-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 20:52 xia_gpt-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      532 b- defN 23-Jun-29 20:52 xia_gpt-0.1.2.dist-info/RECORD
-7 files, 2514 bytes uncompressed, 1445 bytes compressed:  42.5%
+Zip file size: 2319 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-30 11:30 xia_gpt/__init__.py
+-rw-r--r--  2.0 unx     1049 b- defN 23-Jun-29 20:50 xia_gpt/gpt.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:30 xia_gpt-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      380 b- defN 23-Jun-30 11:30 xia_gpt-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:30 xia_gpt-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 11:30 xia_gpt-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      533 b- defN 23-Jun-30 11:30 xia_gpt-0.1.3.dist-info/RECORD
+7 files, 2304 bytes uncompressed, 1373 bytes compressed:  40.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_gpt/__init__.py
 Comment: 
 
 Filename: xia_gpt/gpt.py
 Comment: 
 
-Filename: xia_gpt-0.1.2.dist-info/LICENSE.txt
+Filename: xia_gpt-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_gpt-0.1.2.dist-info/METADATA
+Filename: xia_gpt-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_gpt-0.1.2.dist-info/WHEEL
+Filename: xia_gpt-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_gpt-0.1.2.dist-info/top_level.txt
+Filename: xia_gpt-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_gpt-0.1.2.dist-info/RECORD
+Filename: xia_gpt-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_gpt/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_gpt.gpt import Gpt
 
 __all__ = [
     "Gpt"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

