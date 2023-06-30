# Comparing `tmp/xia_pusher_flask-0.0.10-cp39-none-win_amd64.whl.zip` & `tmp/xia_pusher_flask-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2602 bytes, number of entries: 7
--rw-r--r--  2.0 unx       97 b- defN 23-Jun-29 20:56 xia_pusher_flask/__init__.py
--rw-r--r--  2.0 unx     1212 b- defN 23-Jun-29 20:17 xia_pusher_flask/api.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:00 xia_pusher_flask-0.0.10.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      716 b- defN 23-Jun-29 21:00 xia_pusher_flask-0.0.10.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:00 xia_pusher_flask-0.0.10.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-29 21:00 xia_pusher_flask-0.0.10.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      601 b- defN 23-Jun-29 21:00 xia_pusher_flask-0.0.10.dist-info/RECORD
-7 files, 2893 bytes uncompressed, 1520 bytes compressed:  47.5%
+Zip file size: 112126 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-26 13:15 xia_pusher_flask/__init__.py
+-rw-r--r--  2.0 unx   272384 b- defN 23-Jun-26 13:17 xia_pusher_flask/api.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      714 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      614 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/RECORD
+7 files, 274076 bytes uncompressed, 111022 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_pusher_flask/__init__.py
 Comment: 
 
-Filename: xia_pusher_flask/api.py
+Filename: xia_pusher_flask/api.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_pusher_flask-0.0.10.dist-info/LICENSE.txt
+Filename: xia_pusher_flask-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_pusher_flask-0.0.10.dist-info/METADATA
+Filename: xia_pusher_flask-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_pusher_flask-0.0.10.dist-info/WHEEL
+Filename: xia_pusher_flask-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_pusher_flask-0.0.10.dist-info/top_level.txt
+Filename: xia_pusher_flask-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_pusher_flask-0.0.10.dist-info/RECORD
+Filename: xia_pusher_flask-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_pusher_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_pusher_flask.api import PusherApi
 
 __all__ = [
     "PusherApi"
 ]
 
-__version__ = "0.0.10"
+__version__ = "0.0.9"
```

## Comparing `xia_pusher_flask-0.0.10.dist-info/METADATA` & `xia_pusher_flask-0.0.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-pusher-flask
-Version: 0.0.10
+Version: 0.0.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-pusher-flask/0.0.10/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-pusher-flask/0.0.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_pusher_flask-0.0.10.dist-info/RECORD` & `xia_pusher_flask-0.0.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_pusher_flask/__init__.py,sha256=3TfcqfBgraTgQ7_gM6k1I9jtd9-xgSThRoZufCf4a2g,97
-xia_pusher_flask/api.py,sha256=J5HaE08QDBYgNg0B-V1VMdF6kHLiQiGmrAnwHaDts6g,1212
-xia_pusher_flask-0.0.10.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_pusher_flask-0.0.10.dist-info/METADATA,sha256=0bdcHwYdc5_SqGfVXEjOsMK_H8MBkT42ivi8MPH2G3s,716
-xia_pusher_flask-0.0.10.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_pusher_flask-0.0.10.dist-info/top_level.txt,sha256=bwG9aPiKiGDYuKjuxyCH1xRmPzxRHfspYZ0_OOvaz90,17
-xia_pusher_flask-0.0.10.dist-info/RECORD,,
+xia_pusher_flask/__init__.py,sha256=GpgyjTSZqyOByUW9YfLvQFySswYkS5HZAt2Jo5DZAVQ,97
+xia_pusher_flask/api.cp39-win_amd64.pyd,sha256=rQ_-DM919F5ccHxPAmexn00FAJIVkWsZiaB-hwV0fk4,272384
+xia_pusher_flask-0.0.9.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
+xia_pusher_flask-0.0.9.dist-info/METADATA,sha256=WP5IxDRqkH9sadzO-eyWxk5k3RAODkjiMtSKh1CuHLw,714
+xia_pusher_flask-0.0.9.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_pusher_flask-0.0.9.dist-info/top_level.txt,sha256=bwG9aPiKiGDYuKjuxyCH1xRmPzxRHfspYZ0_OOvaz90,17
+xia_pusher_flask-0.0.9.dist-info/RECORD,,
```

