# Comparing `tmp/xia_token_flask-0.1.13-cp39-none-win_amd64.whl.zip` & `tmp/xia_token_flask-0.1.14-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5373 bytes, number of entries: 7
--rw-r--r--  2.0 unx      102 b- defN 23-Jun-29 21:02 xia_token_flask/__init__.py
--rw-r--r--  2.0 unx    17714 b- defN 23-Jun-29 21:00 xia_token_flask/token.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:03 xia_token_flask-0.1.13.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      702 b- defN 23-Jun-29 21:03 xia_token_flask-0.1.13.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:03 xia_token_flask-0.1.13.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 21:03 xia_token_flask-0.1.13.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      598 b- defN 23-Jun-29 21:03 xia_token_flask-0.1.13.dist-info/RECORD
-7 files, 19382 bytes uncompressed, 4301 bytes compressed:  77.8%
+Zip file size: 5374 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-29 21:06 xia_token_flask/__init__.py
+-rw-r--r--  2.0 unx    17714 b- defN 23-Jun-29 21:06 xia_token_flask/token.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:06 xia_token_flask-0.1.14.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      702 b- defN 23-Jun-29 21:06 xia_token_flask-0.1.14.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:06 xia_token_flask-0.1.14.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 21:06 xia_token_flask-0.1.14.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      598 b- defN 23-Jun-29 21:06 xia_token_flask-0.1.14.dist-info/RECORD
+7 files, 19382 bytes uncompressed, 4302 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_token_flask/__init__.py
 Comment: 
 
 Filename: xia_token_flask/token.py
 Comment: 
 
-Filename: xia_token_flask-0.1.13.dist-info/LICENSE.txt
+Filename: xia_token_flask-0.1.14.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_token_flask-0.1.13.dist-info/METADATA
+Filename: xia_token_flask-0.1.14.dist-info/METADATA
 Comment: 
 
-Filename: xia_token_flask-0.1.13.dist-info/WHEEL
+Filename: xia_token_flask-0.1.14.dist-info/WHEEL
 Comment: 
 
-Filename: xia_token_flask-0.1.13.dist-info/top_level.txt
+Filename: xia_token_flask-0.1.14.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_token_flask-0.1.13.dist-info/RECORD
+Filename: xia_token_flask-0.1.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_token_flask/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_token_flask.token import FlaskToken
 
 
 __all__ = [
     "FlaskToken",
 ]
 
-__version__ = "0.1.13"
+__version__ = "0.1.14"
```

## Comparing `xia_token_flask-0.1.13.dist-info/METADATA` & `xia_token_flask-0.1.14.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-token-flask
-Version: 0.1.13
+Version: 0.1.14
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-token-flask/0.1.13/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-token-flask/0.1.14/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_token_flask-0.1.13.dist-info/RECORD` & `xia_token_flask-0.1.14.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_token_flask/__init__.py,sha256=wdrf2uOUUM8LFpdJvjw3OnZBapVlJmqx2z6OiZA0gmI,102
+xia_token_flask/__init__.py,sha256=hnRpFT-CHcRSh-Nf_cAsD0OeJP-zGPzB0KOOM89keSc,102
 xia_token_flask/token.py,sha256=zMcXrlhJf8Yntyv-v5m5rueo8RJ4kiRtRhMBpqPGpL0,17714
-xia_token_flask-0.1.13.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_token_flask-0.1.13.dist-info/METADATA,sha256=bVKCFRAWTYg0YgrFIXb4SenjzYGaNq1vEtSms2Pqcs4,702
-xia_token_flask-0.1.13.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_token_flask-0.1.13.dist-info/top_level.txt,sha256=DjfAUnatm0oQUQYtViP5G4-EtGPX2Qy2If_5IEkj03c,16
-xia_token_flask-0.1.13.dist-info/RECORD,,
+xia_token_flask-0.1.14.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_token_flask-0.1.14.dist-info/METADATA,sha256=0fW6lQ2exUoPNHQ53UzEV5iTPz9guyapdVeiDtCgRKc,702
+xia_token_flask-0.1.14.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_token_flask-0.1.14.dist-info/top_level.txt,sha256=DjfAUnatm0oQUQYtViP5G4-EtGPX2Qy2If_5IEkj03c,16
+xia_token_flask-0.1.14.dist-info/RECORD,,
```

