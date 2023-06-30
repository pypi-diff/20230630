# Comparing `tmp/xia_sso_flask-0.1.20-cp39-none-win_amd64.whl.zip` & `tmp/xia_sso_flask-0.1.21-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 133979 bytes, number of entries: 7
--rw-r--r--  2.0 unx      100 b- defN 23-Jun-26 08:09 xia_sso_flask/__init__.py
--rw-r--r--  2.0 unx   336896 b- defN 23-Jun-26 08:11 xia_sso_flask/sso.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 08:11 xia_sso_flask-0.1.20.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      733 b- defN 23-Jun-26 08:11 xia_sso_flask-0.1.20.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 08:11 xia_sso_flask-0.1.20.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-26 08:11 xia_sso_flask-0.1.20.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      599 b- defN 23-Jun-26 08:11 xia_sso_flask-0.1.20.dist-info/RECORD
-7 files, 338592 bytes uncompressed, 132907 bytes compressed:  60.7%
+Zip file size: 4205 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:58 xia_sso_flask/__init__.py
+-rw-r--r--  2.0 unx     7568 b- defN 23-Jun-29 20:58 xia_sso_flask/sso.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:02 xia_sso_flask-0.1.21.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      733 b- defN 23-Jun-29 21:02 xia_sso_flask-0.1.21.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:02 xia_sso_flask-0.1.21.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-29 21:02 xia_sso_flask-0.1.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      580 b- defN 23-Jun-29 21:02 xia_sso_flask-0.1.21.dist-info/RECORD
+7 files, 9244 bytes uncompressed, 3165 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_sso_flask/__init__.py
 Comment: 
 
-Filename: xia_sso_flask/sso.cp39-win_amd64.pyd
+Filename: xia_sso_flask/sso.py
 Comment: 
 
-Filename: xia_sso_flask-0.1.20.dist-info/LICENSE.txt
+Filename: xia_sso_flask-0.1.21.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_sso_flask-0.1.20.dist-info/METADATA
+Filename: xia_sso_flask-0.1.21.dist-info/METADATA
 Comment: 
 
-Filename: xia_sso_flask-0.1.20.dist-info/WHEEL
+Filename: xia_sso_flask-0.1.21.dist-info/WHEEL
 Comment: 
 
-Filename: xia_sso_flask-0.1.20.dist-info/top_level.txt
+Filename: xia_sso_flask-0.1.21.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_sso_flask-0.1.20.dist-info/RECORD
+Filename: xia_sso_flask-0.1.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_sso_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_sso_flask.sso import XiaSsoFlask
 
 __all__ = [
     "XiaSsoFlask",
 ]
 
-__version__ = "0.1.20"
+__version__ = "0.1.21"
```

## Comparing `xia_sso_flask-0.1.20.dist-info/METADATA` & `xia_sso_flask-0.1.21.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-sso-flask
-Version: 0.1.20
+Version: 0.1.21
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-sso-flask/0.1.20/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-sso-flask/0.1.21/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

