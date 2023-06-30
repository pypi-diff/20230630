# Comparing `tmp/xia_compiler_python-0.1.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_python-0.1.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5202 bytes, number of entries: 7
--rw-r--r--  2.0 unx      115 b- defN 23-Jun-29 20:40 xia_compiler_python/__init__.py
--rw-r--r--  2.0 unx    14558 b- defN 23-Jun-29 14:55 xia_compiler_python/compiler.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      674 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      624 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/RECORD
-7 files, 16241 bytes uncompressed, 4078 bytes compressed:  74.9%
+Zip file size: 5120 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-30 11:20 xia_compiler_python/__init__.py
+-rw-r--r--  2.0 unx    14558 b- defN 23-Jun-30 11:20 xia_compiler_python/compiler.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      624 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/RECORD
+7 files, 15997 bytes uncompressed, 3996 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_python/__init__.py
 Comment: 
 
 Filename: xia_compiler_python/compiler.py
 Comment: 
 
-Filename: xia_compiler_python-0.1.5.dist-info/LICENSE.txt
+Filename: xia_compiler_python-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.5.dist-info/METADATA
+Filename: xia_compiler_python-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_python-0.1.5.dist-info/WHEEL
+Filename: xia_compiler_python-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_python-0.1.5.dist-info/top_level.txt
+Filename: xia_compiler_python-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.5.dist-info/RECORD
+Filename: xia_compiler_python-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_python/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_python.compiler import PythonCompiler
 
 
 __all__ = [
     "PythonCompiler"
 ]
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

