# Comparing `tmp/xia_broadcast_listener-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_broadcast_listener-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 126642 bytes, number of entries: 7
--rw-r--r--  2.0 unx      125 b- defN 23-Jun-26 17:33 xia_broadcast_listener/__init__.py
--rw-r--r--  2.0 unx   312320 b- defN 23-Jun-26 17:36 xia_broadcast_listener/listener.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 17:36 xia_broadcast_listener-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      712 b- defN 23-Jun-26 17:36 xia_broadcast_listener-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 17:36 xia_broadcast_listener-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-26 17:36 xia_broadcast_listener-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      662 b- defN 23-Jun-26 17:36 xia_broadcast_listener-0.1.1.dist-info/RECORD
-7 files, 314092 bytes uncompressed, 125444 bytes compressed:  60.1%
+Zip file size: 3378 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-29 20:34 xia_broadcast_listener/__init__.py
+-rw-r--r--  2.0 unx     3831 b- defN 23-Jun-29 20:34 xia_broadcast_listener/listener.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:39 xia_broadcast_listener-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      712 b- defN 23-Jun-29 20:39 xia_broadcast_listener-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:39 xia_broadcast_listener-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-29 20:39 xia_broadcast_listener-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      644 b- defN 23-Jun-29 20:39 xia_broadcast_listener-0.1.2.dist-info/RECORD
+7 files, 5584 bytes uncompressed, 2212 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_broadcast_listener/__init__.py
 Comment: 
 
-Filename: xia_broadcast_listener/listener.cp39-win_amd64.pyd
+Filename: xia_broadcast_listener/listener.py
 Comment: 
 
-Filename: xia_broadcast_listener-0.1.1.dist-info/LICENSE.txt
+Filename: xia_broadcast_listener-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_broadcast_listener-0.1.1.dist-info/METADATA
+Filename: xia_broadcast_listener-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_broadcast_listener-0.1.1.dist-info/WHEEL
+Filename: xia_broadcast_listener-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_broadcast_listener-0.1.1.dist-info/top_level.txt
+Filename: xia_broadcast_listener-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_broadcast_listener-0.1.1.dist-info/RECORD
+Filename: xia_broadcast_listener-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_broadcast_listener/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_broadcast_listener.listener import BroadcastListener
 
 
 __all__ = [
     "BroadcastListener"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_broadcast_listener-0.1.1.dist-info/METADATA` & `xia_broadcast_listener-0.1.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-broadcast-listener
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-broadcast-listener/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-broadcast-listener/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

