# Comparing `tmp/xia_engine_test-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_test-0.1.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4264 bytes, number of entries: 9
--rw-r--r--  2.0 unx      307 b- defN 23-Jun-29 20:47 xia_engine_test/__init__.py
--rw-r--r--  2.0 unx     2338 b- defN 23-Jun-29 20:09 xia_engine_test/document_example.py
--rw-r--r--  2.0 unx     6563 b- defN 23-Jun-29 20:09 xia_engine_test/field_test.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-29 20:09 xia_engine_test/models.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      853 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      770 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/RECORD
-9 files, 11724 bytes uncompressed, 2920 bytes compressed:  75.1%
+Zip file size: 4125 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      307 b- defN 23-Jun-30 11:25 xia_engine_test/__init__.py
+-rw-r--r--  2.0 unx     2338 b- defN 23-Jun-30 11:25 xia_engine_test/document_example.py
+-rw-r--r--  2.0 unx     6563 b- defN 23-Jun-30 11:25 xia_engine_test/field_test.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-30 11:25 xia_engine_test/models.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:29 xia_engine_test-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      448 b- defN 23-Jun-30 11:29 xia_engine_test-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:29 xia_engine_test-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:29 xia_engine_test-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      770 b- defN 23-Jun-30 11:29 xia_engine_test-0.1.4.dist-info/RECORD
+9 files, 11319 bytes uncompressed, 2781 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_engine_test/field_test.py
 Comment: 
 
 Filename: xia_engine_test/models.py
 Comment: 
 
-Filename: xia_engine_test-0.1.3.dist-info/LICENSE.txt
+Filename: xia_engine_test-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_test-0.1.3.dist-info/METADATA
+Filename: xia_engine_test-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_test-0.1.3.dist-info/WHEEL
+Filename: xia_engine_test-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_test-0.1.3.dist-info/top_level.txt
+Filename: xia_engine_test-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_test-0.1.3.dist-info/RECORD
+Filename: xia_engine_test-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_test/__init__.py

```diff
@@ -5,8 +5,8 @@
 __all__ = [
     "FieldTest",
     "MessageHello", "DocumentSimple", "External",
     "DocumentBasic"
 ]
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

