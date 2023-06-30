# Comparing `tmp/xia_synchronizer-0.0.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_synchronizer-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 108247 bytes, number of entries: 7
--rw-r--r--  2.0 unx      112 b- defN 23-Jun-26 18:52 xia_synchronizer/__init__.py
--rw-r--r--  2.0 unx   264704 b- defN 23-Jun-26 18:54 xia_synchronizer/synchronizer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:54 xia_synchronizer-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      713 b- defN 23-Jun-26 18:54 xia_synchronizer-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:54 xia_synchronizer-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-26 18:54 xia_synchronizer-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      624 b- defN 23-Jun-26 18:54 xia_synchronizer-0.0.3.dist-info/RECORD
-7 files, 266420 bytes uncompressed, 107125 bytes compressed:  59.8%
+Zip file size: 2700 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-29 20:58 xia_synchronizer/__init__.py
+-rw-r--r--  2.0 unx     1924 b- defN 23-Jun-29 20:58 xia_synchronizer/synchronizer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:03 xia_synchronizer-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      713 b- defN 23-Jun-29 21:03 xia_synchronizer-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:03 xia_synchronizer-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-29 21:03 xia_synchronizer-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      606 b- defN 23-Jun-29 21:03 xia_synchronizer-0.0.4.dist-info/RECORD
+7 files, 3621 bytes uncompressed, 1610 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_synchronizer/__init__.py
 Comment: 
 
-Filename: xia_synchronizer/synchronizer.cp39-win_amd64.pyd
+Filename: xia_synchronizer/synchronizer.py
 Comment: 
 
-Filename: xia_synchronizer-0.0.3.dist-info/LICENSE.txt
+Filename: xia_synchronizer-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_synchronizer-0.0.3.dist-info/METADATA
+Filename: xia_synchronizer-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_synchronizer-0.0.3.dist-info/WHEEL
+Filename: xia_synchronizer-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_synchronizer-0.0.3.dist-info/top_level.txt
+Filename: xia_synchronizer-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_synchronizer-0.0.3.dist-info/RECORD
+Filename: xia_synchronizer-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_synchronizer/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_synchronizer.synchronizer import Synchronizer
 
 __all__ = [
     "Synchronizer"
 ]
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `xia_synchronizer-0.0.3.dist-info/METADATA` & `xia_synchronizer-0.0.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-synchronizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-synchronizer/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-synchronizer/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_synchronizer-0.0.3.dist-info/RECORD` & `xia_synchronizer-0.0.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_synchronizer/__init__.py,sha256=dWc9otR1KLx3xTv-eViRRSD7mVSUDEukQPAJOli0Pnc,112
-xia_synchronizer/synchronizer.cp39-win_amd64.pyd,sha256=IMBLb36TtVWuL0ijc6M-DNabH3DOkudvY_9GrapLK20,264704
-xia_synchronizer-0.0.3.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_synchronizer-0.0.3.dist-info/METADATA,sha256=ORYNsBCx5dI6UsgMPEB050e6MwiCn9CTNA4a5n0UGxA,713
-xia_synchronizer-0.0.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_synchronizer-0.0.3.dist-info/top_level.txt,sha256=EahQyqx1d2L_ftYTJKK2xMeqqBeLdlPQrJTCzXNxp9M,17
-xia_synchronizer-0.0.3.dist-info/RECORD,,
+xia_synchronizer/__init__.py,sha256=k8pJ9eq0epIZxyWQj3X4T-hM9WyvUyL56EZqHjf3rXU,111
+xia_synchronizer/synchronizer.py,sha256=q45rkKyE8JxESGPTy4iVbwqY9G8WPo36Uv-3tSgND4g,1924
+xia_synchronizer-0.0.4.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_synchronizer-0.0.4.dist-info/METADATA,sha256=gphnGIPWKfOCF55udv3s3ntEnqDxC0T4RoKlOMheNDQ,713
+xia_synchronizer-0.0.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_synchronizer-0.0.4.dist-info/top_level.txt,sha256=EahQyqx1d2L_ftYTJKK2xMeqqBeLdlPQrJTCzXNxp9M,17
+xia_synchronizer-0.0.4.dist-info/RECORD,,
```

