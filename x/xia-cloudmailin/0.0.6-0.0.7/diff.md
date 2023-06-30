# Comparing `tmp/xia_cloudmailin-0.0.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_cloudmailin-0.0.7-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 117491 bytes, number of entries: 7
--rw-r--r--  2.0 unx       98 b- defN 23-Jun-26 18:50 xia_cloudmailin/__init__.py
--rw-r--r--  2.0 unx   287232 b- defN 23-Jun-26 18:53 xia_cloudmailin/mail.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:53 xia_cloudmailin-0.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      774 b- defN 23-Jun-26 18:53 xia_cloudmailin-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:53 xia_cloudmailin-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-26 18:53 xia_cloudmailin-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      608 b- defN 23-Jun-26 18:53 xia_cloudmailin-0.0.6.dist-info/RECORD
-7 files, 288978 bytes uncompressed, 116399 bytes compressed:  59.7%
+Zip file size: 2660 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-29 20:37 xia_cloudmailin/__init__.py
+-rw-r--r--  2.0 unx     1587 b- defN 23-Jun-29 20:37 xia_cloudmailin/mail.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:42 xia_cloudmailin-0.0.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      774 b- defN 23-Jun-29 20:42 xia_cloudmailin-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:42 xia_cloudmailin-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:42 xia_cloudmailin-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      590 b- defN 23-Jun-29 20:42 xia_cloudmailin-0.0.7.dist-info/RECORD
+7 files, 3314 bytes uncompressed, 1600 bytes compressed:  51.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_cloudmailin/__init__.py
 Comment: 
 
-Filename: xia_cloudmailin/mail.cp39-win_amd64.pyd
+Filename: xia_cloudmailin/mail.py
 Comment: 
 
-Filename: xia_cloudmailin-0.0.6.dist-info/LICENSE.txt
+Filename: xia_cloudmailin-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_cloudmailin-0.0.6.dist-info/METADATA
+Filename: xia_cloudmailin-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_cloudmailin-0.0.6.dist-info/WHEEL
+Filename: xia_cloudmailin-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_cloudmailin-0.0.6.dist-info/top_level.txt
+Filename: xia_cloudmailin-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_cloudmailin-0.0.6.dist-info/RECORD
+Filename: xia_cloudmailin-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_cloudmailin/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_cloudmailin.mail import CloudMail
 
 
 __all__ = [
     "CloudMail"
 ]
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

## Comparing `xia_cloudmailin-0.0.6.dist-info/METADATA` & `xia_cloudmailin-0.0.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-cloudmailin
-Version: 0.0.6
+Version: 0.0.7
 Summary: X-I-A Cloud Mail In Tools
-Home-page: https://develop.x-i-a.com/docs/xia-cloudmailin/0.0.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-cloudmailin/0.0.7/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

