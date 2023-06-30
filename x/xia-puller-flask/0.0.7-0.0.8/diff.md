# Comparing `tmp/xia_puller_flask-0.0.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_puller_flask-0.0.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2460 bytes, number of entries: 7
--rw-r--r--  2.0 unx       96 b- defN 23-Jun-30 09:58 xia_puller_flask/__init__.py
--rw-r--r--  2.0 unx     1104 b- defN 23-Jun-29 08:52 xia_puller_flask/api.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 09:58 xia_puller_flask-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      476 b- defN 23-Jun-30 09:58 xia_puller_flask-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 09:58 xia_puller_flask-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-30 09:58 xia_puller_flask-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      596 b- defN 23-Jun-30 09:58 xia_puller_flask-0.0.7.dist-info/RECORD
-7 files, 2539 bytes uncompressed, 1388 bytes compressed:  45.3%
+Zip file size: 2463 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-30 11:35 xia_puller_flask/__init__.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Jun-30 11:35 xia_puller_flask/api.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      476 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/RECORD
+7 files, 2539 bytes uncompressed, 1391 bytes compressed:  45.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_puller_flask/__init__.py
 Comment: 
 
 Filename: xia_puller_flask/api.py
 Comment: 
 
-Filename: xia_puller_flask-0.0.7.dist-info/LICENSE.txt
+Filename: xia_puller_flask-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_puller_flask-0.0.7.dist-info/METADATA
+Filename: xia_puller_flask-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_puller_flask-0.0.7.dist-info/WHEEL
+Filename: xia_puller_flask-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_puller_flask-0.0.7.dist-info/top_level.txt
+Filename: xia_puller_flask-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_puller_flask-0.0.7.dist-info/RECORD
+Filename: xia_puller_flask-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_puller_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_puller_flask.api import PullerApi
 
 __all__ = [
     "PullerApi"
 ]
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

## Comparing `xia_puller_flask-0.0.7.dist-info/RECORD` & `xia_puller_flask-0.0.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_puller_flask/__init__.py,sha256=s0EYE0vtg0jAfdVwjg7VQne0TgG7KkHgxKWQbypt6e0,96
+xia_puller_flask/__init__.py,sha256=sVU06Fd4wVlcD2devOgCYeTm0BD_gBRY7yY-g0d4QaY,96
 xia_puller_flask/api.py,sha256=f8wnWHHisVLGbyzHs1v3EvLdMgS9CfTG9013xtX--4k,1104
-xia_puller_flask-0.0.7.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_puller_flask-0.0.7.dist-info/METADATA,sha256=0t0zqBtFrLssFmLaX_acnWPWdPR2M0AKmfq6-a56z2E,476
-xia_puller_flask-0.0.7.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_puller_flask-0.0.7.dist-info/top_level.txt,sha256=1L3f8B1GOTeCgn915g1myzSBbN-3IeHhv_zU2W0cmrE,17
-xia_puller_flask-0.0.7.dist-info/RECORD,,
+xia_puller_flask-0.0.8.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_puller_flask-0.0.8.dist-info/METADATA,sha256=UzcYqXFnLvy-s9WfqXV_HuDoBUpLzC0zU9ufFSESV10,476
+xia_puller_flask-0.0.8.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_puller_flask-0.0.8.dist-info/top_level.txt,sha256=1L3f8B1GOTeCgn915g1myzSBbN-3IeHhv_zU2W0cmrE,17
+xia_puller_flask-0.0.8.dist-info/RECORD,,
```

