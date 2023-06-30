# Comparing `tmp/xia_models-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_models-0.1.9-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9857 bytes, number of entries: 8
--rw-r--r--  2.0 unx      238 b- defN 23-Jun-29 20:56 xia_models/__init__.py
+Zip file size: 9782 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      238 b- defN 23-Jun-30 11:35 xia_models/__init__.py
 -rw-r--r--  2.0 unx    18354 b- defN 23-Jun-29 20:56 xia_models/address.py
 -rw-r--r--  2.0 unx    16070 b- defN 23-Jun-29 20:56 xia_models/model.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      638 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      637 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/RECORD
-8 files, 36198 bytes uncompressed, 8747 bytes compressed:  75.8%
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:35 xia_models-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      412 b- defN 23-Jun-30 11:35 xia_models-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:35 xia_models-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:35 xia_models-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      638 b- defN 23-Jun-30 11:35 xia_models-0.1.9.dist-info/RECORD
+8 files, 35982 bytes uncompressed, 8672 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: xia_models/address.py
 Comment: 
 
 Filename: xia_models/model.py
 Comment: 
 
-Filename: xia_models-0.1.8.dist-info/LICENSE.txt
+Filename: xia_models-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_models-0.1.8.dist-info/METADATA
+Filename: xia_models-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_models-0.1.8.dist-info/WHEEL
+Filename: xia_models-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_models-0.1.8.dist-info/top_level.txt
+Filename: xia_models-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_models-0.1.8.dist-info/RECORD
+Filename: xia_models-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_models/__init__.py

```diff
@@ -2,8 +2,8 @@
 from xia_models.address import DataAddress, TableAddress, TableCatalog
 
 __all__ = [
     "DataModel", "DataField",
     "DataAddress", "TableAddress", "TableCatalog"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

