# Comparing `tmp/xia_engine_terraform-0.1.17-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.1.18-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7652 bytes, number of entries: 7
--rw-r--r--  2.0 unx      645 b- defN 23-Jun-29 20:43 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx    28900 b- defN 23-Jun-29 20:43 xia_engine_terraform/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      634 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/RECORD
-7 files, 31176 bytes uncompressed, 6508 bytes compressed:  79.1%
+Zip file size: 7570 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      645 b- defN 23-Jun-30 11:24 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx    28900 b- defN 23-Jun-30 11:24 xia_engine_terraform/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      480 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      634 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/RECORD
+7 files, 30930 bytes uncompressed, 6426 bytes compressed:  79.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform/engine.py
 Comment: 
 
-Filename: xia_engine_terraform-0.1.17.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.1.18.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.17.dist-info/METADATA
+Filename: xia_engine_terraform-0.1.18.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.1.17.dist-info/WHEEL
+Filename: xia_engine_terraform-0.1.18.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.1.17.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.1.18.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.17.dist-info/RECORD
+Filename: xia_engine_terraform-0.1.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform/__init__.py

```diff
@@ -6,8 +6,8 @@
 __all__ = [
     "TerraformEngine", "TerraformConnectParam", "TerraformClient",
     "TerraformLocalEngine", "TerraformLocalConnectParam", "TerraformLocalClient",
     "ScwTerraformLocalEngine", "ScwTerraformLocalConnectParam",
     "TerraformConfigFactory"
 ]
 
-__version__ = "0.1.17"
+__version__ = "0.1.18"
```

