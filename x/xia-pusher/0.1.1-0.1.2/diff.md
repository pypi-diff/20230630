# Comparing `tmp/xia_pusher-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_pusher-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 112838 bytes, number of entries: 7
--rw-r--r--  2.0 unx       88 b- defN 23-Jun-26 13:22 xia_pusher/__init__.py
--rw-r--r--  2.0 unx   275456 b- defN 23-Jun-26 13:24 xia_pusher/pusher.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      689 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      575 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/RECORD
-7 files, 277069 bytes uncompressed, 111812 bytes compressed:  59.6%
+Zip file size: 2629 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-29 20:55 xia_pusher/__init__.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-Jun-29 20:55 xia_pusher/pusher.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:59 xia_pusher-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      689 b- defN 23-Jun-29 20:59 xia_pusher-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:59 xia_pusher-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:59 xia_pusher-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      557 b- defN 23-Jun-29 20:59 xia_pusher-0.1.2.dist-info/RECORD
+7 files, 3337 bytes uncompressed, 1635 bytes compressed:  51.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_pusher/__init__.py
 Comment: 
 
-Filename: xia_pusher/pusher.cp39-win_amd64.pyd
+Filename: xia_pusher/pusher.py
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/LICENSE.txt
+Filename: xia_pusher-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/METADATA
+Filename: xia_pusher-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/WHEEL
+Filename: xia_pusher-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/top_level.txt
+Filename: xia_pusher-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/RECORD
+Filename: xia_pusher-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_pusher/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_pusher.pusher import Pusher
 
 __all__ = [
     "Pusher"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_pusher-0.1.1.dist-info/METADATA` & `xia_pusher-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-pusher
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-pusher/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-pusher/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_pusher-0.1.1.dist-info/RECORD` & `xia_pusher-0.1.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_pusher/__init__.py,sha256=gWBbX-JSvKSUbQNuCSZeTHR2dg-Jk_7WnJm-JZ1mCRI,88
-xia_pusher/pusher.cp39-win_amd64.pyd,sha256=GsQPg0XXrYrfBaBJosZPyy9YnU1ECgrAg9Xg9a8ThHI,275456
-xia_pusher-0.1.1.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_pusher-0.1.1.dist-info/METADATA,sha256=T9ZAwihwaBbXQsyxXm7Hkt4wimgWd04wwUWQzUxAtYw,689
-xia_pusher-0.1.1.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_pusher-0.1.1.dist-info/top_level.txt,sha256=uSGJ_X9EmGNhwPpC0AJJ2Ym5zCI-37onXj9SOzAH1Es,11
-xia_pusher-0.1.1.dist-info/RECORD,,
+xia_pusher/__init__.py,sha256=uhoYi3y6NRI3Pw5ZRS66N5WnihHQb8E-XxzizD2TJlo,87
+xia_pusher/pusher.py,sha256=8qxxlERTmePCHqmvJef0PbM59og_41iwLDAu1KAF89c,1743
+xia_pusher-0.1.2.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_pusher-0.1.2.dist-info/METADATA,sha256=ihn7vbue3MnS73Zu4xAJUMR4YH0JVdliBemIsKAURyI,689
+xia_pusher-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_pusher-0.1.2.dist-info/top_level.txt,sha256=uSGJ_X9EmGNhwPpC0AJJ2Ym5zCI-37onXj9SOzAH1Es,11
+xia_pusher-0.1.2.dist-info/RECORD,,
```

