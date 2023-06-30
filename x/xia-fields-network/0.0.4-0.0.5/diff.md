# Comparing `tmp/xia_fields_network-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_fields_network-0.0.5-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2714 bytes, number of entries: 7
--rw-r--r--  2.0 unx      171 b- defN 23-Jun-29 20:47 xia_fields_network/__init__.py
--rw-r--r--  2.0 unx     2344 b- defN 23-Jun-29 20:47 xia_fields_network/fields.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      670 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      614 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/RECORD
-7 files, 4068 bytes uncompressed, 1608 bytes compressed:  60.5%
+Zip file size: 2642 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-30 11:29 xia_fields_network/__init__.py
+-rw-r--r--  2.0 unx     2344 b- defN 23-Jun-30 11:29 xia_fields_network/fields.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:29 xia_fields_network-0.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      428 b- defN 23-Jun-30 11:29 xia_fields_network-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:29 xia_fields_network-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-30 11:29 xia_fields_network-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      615 b- defN 23-Jun-30 11:29 xia_fields_network-0.0.5.dist-info/RECORD
+7 files, 3836 bytes uncompressed, 1536 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_fields_network/__init__.py
 Comment: 
 
 Filename: xia_fields_network/fields.py
 Comment: 
 
-Filename: xia_fields_network-0.0.4.dist-info/LICENSE.txt
+Filename: xia_fields_network-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_fields_network-0.0.4.dist-info/METADATA
+Filename: xia_fields_network-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_fields_network-0.0.4.dist-info/WHEEL
+Filename: xia_fields_network-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_fields_network-0.0.4.dist-info/top_level.txt
+Filename: xia_fields_network-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_fields_network-0.0.4.dist-info/RECORD
+Filename: xia_fields_network-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_fields_network/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_fields_network.fields import EmailField, IpField, IpV6Field, MacField
 
 
 __all__ = [
     "EmailField", "IpField", "IpV6Field", "MacField",
 ]
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

