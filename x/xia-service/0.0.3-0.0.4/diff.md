# Comparing `tmp/xia_service-0.0.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_service-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 106461 bytes, number of entries: 7
--rw-r--r--  2.0 unx       94 b- defN 23-Jun-26 08:11 xia_service/__init__.py
--rw-r--r--  2.0 unx   259584 b- defN 23-Jun-26 08:12 xia_service/service.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 08:12 xia_service-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      668 b- defN 23-Jun-26 08:12 xia_service-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 08:12 xia_service-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-26 08:12 xia_service-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 23-Jun-26 08:12 xia_service-0.0.3.dist-info/RECORD
-7 files, 261191 bytes uncompressed, 105419 bytes compressed:  59.6%
+Zip file size: 2479 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-29 20:58 xia_service/__init__.py
+-rw-r--r--  2.0 unx     1269 b- defN 23-Jun-29 20:14 xia_service/service.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:00 xia_service-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      668 b- defN 23-Jun-29 21:00 xia_service-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:00 xia_service-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-29 21:00 xia_service-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      565 b- defN 23-Jun-29 21:00 xia_service-0.0.4.dist-info/RECORD
+7 files, 2857 bytes uncompressed, 1469 bytes compressed:  48.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_service/__init__.py
 Comment: 
 
-Filename: xia_service/service.cp39-win_amd64.pyd
+Filename: xia_service/service.py
 Comment: 
 
-Filename: xia_service-0.0.3.dist-info/LICENSE.txt
+Filename: xia_service-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_service-0.0.3.dist-info/METADATA
+Filename: xia_service-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_service-0.0.3.dist-info/WHEEL
+Filename: xia_service-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_service-0.0.3.dist-info/top_level.txt
+Filename: xia_service-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_service-0.0.3.dist-info/RECORD
+Filename: xia_service-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_service/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 
 __all__ = [
     "Service"
 ]
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `xia_service-0.0.3.dist-info/METADATA` & `xia_service-0.0.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-service
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-service/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-service/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_service-0.0.3.dist-info/RECORD` & `xia_service-0.0.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_service/__init__.py,sha256=YsA61iiG0qeucrX3kqWXC1SB0jTjg3GGuHx8JCjZ1h8,94
-xia_service/service.cp39-win_amd64.pyd,sha256=A7pwDEOZifDx2TAW7G26bL6qUFqQr34h6i8nspTk4lM,259584
-xia_service-0.0.3.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_service-0.0.3.dist-info/METADATA,sha256=vKeru4uI3CpvI3f2rl2QTr2rwiAy-_4iqw7P7mA7_Rw,668
-xia_service-0.0.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_service-0.0.3.dist-info/top_level.txt,sha256=EZLz1bDGz3dyp4mGaW5IdTEqXzGwEB3L8B-Krokb0Xk,12
-xia_service-0.0.3.dist-info/RECORD,,
+xia_service/__init__.py,sha256=G9nToxRUC5MAMAodfLh1eux7GFj-zADacvco3Z_iLYA,93
+xia_service/service.py,sha256=OszL43rGOgAkQHo0JmIfQQl_IeubJQ_5nmt75oBBFOc,1269
+xia_service-0.0.4.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_service-0.0.4.dist-info/METADATA,sha256=6N_xH6igFm3OvfhgpyPYEJMAQHyViiLZ3Le0BrDH7EU,668
+xia_service-0.0.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_service-0.0.4.dist-info/top_level.txt,sha256=EZLz1bDGz3dyp4mGaW5IdTEqXzGwEB3L8B-Krokb0Xk,12
+xia_service-0.0.4.dist-info/RECORD,,
```

