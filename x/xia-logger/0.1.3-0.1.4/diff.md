# Comparing `tmp/xia_logger-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger-0.1.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4879 bytes, number of entries: 7
--rw-r--r--  2.0 unx      159 b- defN 23-Jun-29 20:49 xia_logger/__init__.py
--rw-r--r--  2.0 unx    11135 b- defN 23-Jun-29 17:32 xia_logger/logger.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      559 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/RECORD
-7 files, 12840 bytes uncompressed, 3885 bytes compressed:  69.7%
+Zip file size: 4794 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-30 11:29 xia_logger/__init__.py
+-rw-r--r--  2.0 unx    11135 b- defN 23-Jun-30 11:29 xia_logger/logger.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      489 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      559 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/RECORD
+7 files, 12603 bytes uncompressed, 3800 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger/__init__.py
 Comment: 
 
 Filename: xia_logger/logger.py
 Comment: 
 
-Filename: xia_logger-0.1.3.dist-info/LICENSE.txt
+Filename: xia_logger-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger-0.1.3.dist-info/METADATA
+Filename: xia_logger-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger-0.1.3.dist-info/WHEEL
+Filename: xia_logger-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger-0.1.3.dist-info/top_level.txt
+Filename: xia_logger-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger-0.1.3.dist-info/RECORD
+Filename: xia_logger-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger.logger import Logger, HttpLogger, JsonLogger, DataLog
 
 __all__ = [
     "Logger", "HttpLogger", "JsonLogger", "DataLog"
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## Comparing `xia_logger-0.1.3.dist-info/RECORD` & `xia_logger-0.1.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_logger/__init__.py,sha256=GNBEtjM59V2eWJ898SBsqJbxinPkRfVDkIxI52UODIw,159
+xia_logger/__init__.py,sha256=P2arKYNGZUN2hsBLoOpY9YDigxx3OnCZGvoTYOJulNA,159
 xia_logger/logger.py,sha256=jtJ-oToP89LMf2VcjJ_cfWYz0yEzCFbalRb9-u9bgmA,11135
-xia_logger-0.1.3.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_logger-0.1.3.dist-info/METADATA,sha256=Jm5PxxJQzNH8qMHh4TDHb0VIKxxKYkPUehO42yLV3Cw,726
-xia_logger-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_logger-0.1.3.dist-info/top_level.txt,sha256=NeX2Q2B7eQe_oQ6Z-8ZdvET5e12RusIwUImAi4LxTV8,11
-xia_logger-0.1.3.dist-info/RECORD,,
+xia_logger-0.1.4.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_logger-0.1.4.dist-info/METADATA,sha256=BvCdWg-oG_mme3k65VUsNeQ_xAnsuKgPQZRdBcG-xvg,489
+xia_logger-0.1.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_logger-0.1.4.dist-info/top_level.txt,sha256=NeX2Q2B7eQe_oQ6Z-8ZdvET5e12RusIwUImAi4LxTV8,11
+xia_logger-0.1.4.dist-info/RECORD,,
```

