# Comparing `tmp/xia_engine_mysql-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_mysql-0.1.9-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4148 bytes, number of entries: 7
--rw-r--r--  2.0 unx      143 b- defN 23-Jun-29 20:44 xia_engine_mysql/__init__.py
--rw-r--r--  2.0 unx     6756 b- defN 23-Jun-29 20:07 xia_engine_mysql/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      715 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      600 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/RECORD
-7 files, 8481 bytes uncompressed, 3070 bytes compressed:  63.8%
+Zip file size: 4076 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-30 11:24 xia_engine_mysql/__init__.py
+-rw-r--r--  2.0 unx     6756 b- defN 23-Jun-30 11:24 xia_engine_mysql/engine.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:24 xia_engine_mysql-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      477 b- defN 23-Jun-30 11:24 xia_engine_mysql-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:24 xia_engine_mysql-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-30 11:24 xia_engine_mysql-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      601 b- defN 23-Jun-30 11:24 xia_engine_mysql-0.1.9.dist-info/RECORD
+7 files, 8253 bytes uncompressed, 2998 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_mysql/__init__.py
 Comment: 
 
 Filename: xia_engine_mysql/engine.py
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/LICENSE.txt
+Filename: xia_engine_mysql-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/METADATA
+Filename: xia_engine_mysql-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/WHEEL
+Filename: xia_engine_mysql-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/top_level.txt
+Filename: xia_engine_mysql-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/RECORD
+Filename: xia_engine_mysql-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_mysql/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_engine_mysql.engine import MysqlEngine, MysqlConnectParam
 
 __all__ = [
     "MysqlEngine", "MysqlConnectParam"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

