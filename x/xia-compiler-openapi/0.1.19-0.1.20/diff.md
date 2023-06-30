# Comparing `tmp/xia_compiler_openapi-0.1.19-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_openapi-0.1.20-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9021 bytes, number of entries: 7
--rw-r--r--  2.0 unx      126 b- defN 23-Jun-29 20:40 xia_compiler_openapi/__init__.py
--rw-r--r--  2.0 unx    38580 b- defN 23-Jun-29 20:40 xia_compiler_openapi/compiler.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      697 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      636 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/RECORD
-7 files, 40310 bytes uncompressed, 7873 bytes compressed:  80.5%
+Zip file size: 8935 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-30 11:20 xia_compiler_openapi/__init__.py
+-rw-r--r--  2.0 unx    38580 b- defN 23-Jun-30 11:20 xia_compiler_openapi/compiler.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:23 xia_compiler_openapi-0.1.20.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      431 b- defN 23-Jun-30 11:23 xia_compiler_openapi-0.1.20.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:23 xia_compiler_openapi-0.1.20.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-30 11:23 xia_compiler_openapi-0.1.20.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      636 b- defN 23-Jun-30 11:23 xia_compiler_openapi-0.1.20.dist-info/RECORD
+7 files, 40044 bytes uncompressed, 7787 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_openapi/__init__.py
 Comment: 
 
 Filename: xia_compiler_openapi/compiler.py
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.19.dist-info/LICENSE.txt
+Filename: xia_compiler_openapi-0.1.20.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.19.dist-info/METADATA
+Filename: xia_compiler_openapi-0.1.20.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.19.dist-info/WHEEL
+Filename: xia_compiler_openapi-0.1.20.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.19.dist-info/top_level.txt
+Filename: xia_compiler_openapi-0.1.20.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.19.dist-info/RECORD
+Filename: xia_compiler_openapi-0.1.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_openapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_openapi.compiler import XiaCompilerOpenapi
 
 
 __all__ = [
     "XiaCompilerOpenapi",
 ]
 
-__version__ = "0.1.19"
+__version__ = "0.1.20"
```

