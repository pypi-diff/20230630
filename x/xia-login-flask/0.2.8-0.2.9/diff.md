# Comparing `tmp/xia_login_flask-0.2.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_login_flask-0.2.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7403 bytes, number of entries: 7
--rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:52 xia_login_flask/__init__.py
--rw-r--r--  2.0 unx    25032 b- defN 23-Jun-29 20:52 xia_login_flask/account.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      739 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      595 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/RECORD
-7 files, 26740 bytes uncompressed, 6337 bytes compressed:  76.3%
+Zip file size: 7320 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:33 xia_login_flask/__init__.py
+-rw-r--r--  2.0 unx    25032 b- defN 23-Jun-30 11:33 xia_login_flask/account.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:35 xia_login_flask-0.2.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      503 b- defN 23-Jun-30 11:35 xia_login_flask-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:35 xia_login_flask-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:35 xia_login_flask-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      595 b- defN 23-Jun-30 11:35 xia_login_flask-0.2.9.dist-info/RECORD
+7 files, 26504 bytes uncompressed, 6254 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_login_flask/__init__.py
 Comment: 
 
 Filename: xia_login_flask/account.py
 Comment: 
 
-Filename: xia_login_flask-0.2.8.dist-info/LICENSE.txt
+Filename: xia_login_flask-0.2.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_login_flask-0.2.8.dist-info/METADATA
+Filename: xia_login_flask-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_login_flask-0.2.8.dist-info/WHEEL
+Filename: xia_login_flask-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_login_flask-0.2.8.dist-info/top_level.txt
+Filename: xia_login_flask-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_login_flask-0.2.8.dist-info/RECORD
+Filename: xia_login_flask-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_login_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_login_flask.account import XiaLoginFlask
 
 __all__ = [
     "XiaLoginFlask",
 ]
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
```

