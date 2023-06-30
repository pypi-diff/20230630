# Comparing `tmp/xia_compiler_jsoneditor-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_jsoneditor-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6527 bytes, number of entries: 7
--rw-r--r--  2.0 unx      134 b- defN 23-Jun-29 20:38 xia_compiler_jsoneditor/__init__.py
--rw-r--r--  2.0 unx    20330 b- defN 23-Jun-29 20:04 xia_compiler_jsoneditor/compiler.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      687 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      652 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/RECORD
-7 files, 22077 bytes uncompressed, 5347 bytes compressed:  75.8%
+Zip file size: 6450 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-30 11:19 xia_compiler_jsoneditor/__init__.py
+-rw-r--r--  2.0 unx    20330 b- defN 23-Jun-30 11:19 xia_compiler_jsoneditor/compiler.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:23 xia_compiler_jsoneditor-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      435 b- defN 23-Jun-30 11:23 xia_compiler_jsoneditor-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:23 xia_compiler_jsoneditor-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-30 11:23 xia_compiler_jsoneditor-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      652 b- defN 23-Jun-30 11:23 xia_compiler_jsoneditor-0.1.5.dist-info/RECORD
+7 files, 21825 bytes uncompressed, 5270 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_jsoneditor/__init__.py
 Comment: 
 
 Filename: xia_compiler_jsoneditor/compiler.py
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.4.dist-info/LICENSE.txt
+Filename: xia_compiler_jsoneditor-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.4.dist-info/METADATA
+Filename: xia_compiler_jsoneditor-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.4.dist-info/WHEEL
+Filename: xia_compiler_jsoneditor-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.4.dist-info/top_level.txt
+Filename: xia_compiler_jsoneditor-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.4.dist-info/RECORD
+Filename: xia_compiler_jsoneditor-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_jsoneditor/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_jsoneditor.compiler import XiaCompilerJsoneditor
 
 
 __all__ = [
     "XiaCompilerJsoneditor",
 ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

