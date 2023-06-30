# Comparing `tmp/xia_sendinblue-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_sendinblue-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 110605 bytes, number of entries: 7
--rw-r--r--  2.0 unx      100 b- defN 23-Jun-26 14:22 xia_sendinblue/__init__.py
--rw-r--r--  2.0 unx   269312 b- defN 23-Jun-26 14:23 xia_sendinblue/sender.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 14:23 xia_sendinblue-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      698 b- defN 23-Jun-26 14:23 xia_sendinblue-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 14:23 xia_sendinblue-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-26 14:23 xia_sendinblue-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      604 b- defN 23-Jun-26 14:23 xia_sendinblue-0.0.8.dist-info/RECORD
-7 files, 270979 bytes uncompressed, 109523 bytes compressed:  59.6%
+Zip file size: 2517 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:56 xia_sendinblue/__init__.py
+-rw-r--r--  2.0 unx      997 b- defN 23-Jun-29 20:56 xia_sendinblue/sender.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:59 xia_sendinblue-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      698 b- defN 23-Jun-29 20:59 xia_sendinblue-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:59 xia_sendinblue-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 20:59 xia_sendinblue-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      584 b- defN 23-Jun-29 20:59 xia_sendinblue-0.0.9.dist-info/RECORD
+7 files, 2643 bytes uncompressed, 1467 bytes compressed:  44.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_sendinblue/__init__.py
 Comment: 
 
-Filename: xia_sendinblue/sender.cp39-win_amd64.pyd
+Filename: xia_sendinblue/sender.py
 Comment: 
 
-Filename: xia_sendinblue-0.0.8.dist-info/LICENSE.txt
+Filename: xia_sendinblue-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_sendinblue-0.0.8.dist-info/METADATA
+Filename: xia_sendinblue-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_sendinblue-0.0.8.dist-info/WHEEL
+Filename: xia_sendinblue-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_sendinblue-0.0.8.dist-info/top_level.txt
+Filename: xia_sendinblue-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_sendinblue-0.0.8.dist-info/RECORD
+Filename: xia_sendinblue-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_sendinblue/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_sendinblue.sender import SendInBlue
 
 __all__ = [
     "SendInBlue"
 ]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## Comparing `xia_sendinblue-0.0.8.dist-info/METADATA` & `xia_sendinblue-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-sendinblue
-Version: 0.0.8
+Version: 0.0.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-sendinblue/0.0.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-sendinblue/0.0.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

