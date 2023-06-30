# Comparing `tmp/xia_engine_rest-0.1.12-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_rest-0.1.13-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4023 bytes, number of entries: 7
--rw-r--r--  2.0 unx      140 b- defN 23-Jun-29 20:43 xia_engine_rest/__init__.py
--rw-r--r--  2.0 unx     7322 b- defN 23-Jun-29 17:29 xia_engine_rest/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      684 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      598 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/RECORD
-7 files, 9010 bytes uncompressed, 2949 bytes compressed:  67.3%
+Zip file size: 3950 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-30 11:25 xia_engine_rest/__init__.py
+-rw-r--r--  2.0 unx     7322 b- defN 23-Jun-29 20:45 xia_engine_rest/engine.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:25 xia_engine_rest-0.1.13.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      448 b- defN 23-Jun-30 11:25 xia_engine_rest-0.1.13.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:25 xia_engine_rest-0.1.13.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:25 xia_engine_rest-0.1.13.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      599 b- defN 23-Jun-30 11:25 xia_engine_rest-0.1.13.dist-info/RECORD
+7 files, 8784 bytes uncompressed, 2876 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_rest/__init__.py
 Comment: 
 
 Filename: xia_engine_rest/engine.py
 Comment: 
 
-Filename: xia_engine_rest-0.1.12.dist-info/LICENSE.txt
+Filename: xia_engine_rest-0.1.13.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_rest-0.1.12.dist-info/METADATA
+Filename: xia_engine_rest-0.1.13.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_rest-0.1.12.dist-info/WHEEL
+Filename: xia_engine_rest-0.1.13.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_rest-0.1.12.dist-info/top_level.txt
+Filename: xia_engine_rest-0.1.13.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_rest-0.1.12.dist-info/RECORD
+Filename: xia_engine_rest-0.1.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_rest/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_rest.engine import RestEngine, RestConnectParam
 
 
 __all__ = [
     "RestEngine", "RestConnectParam"
 ]
 
-__version__ = "0.1.12"
+__version__ = "0.1.13"
```

## Comparing `xia_engine_rest-0.1.12.dist-info/RECORD` & `xia_engine_rest-0.1.13.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_rest/__init__.py,sha256=UPXJD1nvpX-nlj7UT1ynBn7rRvn1fRAjGlRQyBrf5b4,140
+xia_engine_rest/__init__.py,sha256=qh2yqBl1ZUY5HCO3s7Ry9L58c7NH-h71eiajDXWo6Wo,140
 xia_engine_rest/engine.py,sha256=inDcFQMgT9zTNdkwZrzNjj-6KvSTUI1daD-rjcF4yyY,7322
-xia_engine_rest-0.1.12.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_engine_rest-0.1.12.dist-info/METADATA,sha256=i2ft2BsWRXw7ybprEErRCON6VyFzxisLG-dazCfJZA0,684
-xia_engine_rest-0.1.12.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_rest-0.1.12.dist-info/top_level.txt,sha256=Y6M8ui9-spd32kpo6unwoI0veR6mPHw-V7WRkhbl74g,16
-xia_engine_rest-0.1.12.dist-info/RECORD,,
+xia_engine_rest-0.1.13.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_engine_rest-0.1.13.dist-info/METADATA,sha256=YYVp-OME6wMVHSxPMYIyBWAZEO-K_XRrTKjnj7lDgEM,448
+xia_engine_rest-0.1.13.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_engine_rest-0.1.13.dist-info/top_level.txt,sha256=Y6M8ui9-spd32kpo6unwoI0veR6mPHw-V7WRkhbl74g,16
+xia_engine_rest-0.1.13.dist-info/RECORD,,
```

