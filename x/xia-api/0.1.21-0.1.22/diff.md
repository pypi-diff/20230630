# Comparing `tmp/xia_api-0.1.21-cp39-none-win_amd64.whl.zip` & `tmp/xia_api-0.1.22-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7953 bytes, number of entries: 9
--rw-r--r--  2.0 unx      497 b- defN 23-Jun-29 20:33 xia_api/__init__.py
--rw-r--r--  2.0 unx     1577 b- defN 23-Jun-29 20:33 xia_api/auth_client.py
--rw-r--r--  2.0 unx     2329 b- defN 23-Jun-29 20:33 xia_api/message.py
--rw-r--r--  2.0 unx    18688 b- defN 23-Jun-29 20:33 xia_api/rest.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      677 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      694 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/RECORD
-9 files, 24720 bytes uncompressed, 6763 bytes compressed:  72.6%
+Zip file size: 7870 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      497 b- defN 23-Jun-30 11:14 xia_api/__init__.py
+-rw-r--r--  2.0 unx     1577 b- defN 23-Jun-30 11:14 xia_api/auth_client.py
+-rw-r--r--  2.0 unx     2329 b- defN 23-Jun-30 11:14 xia_api/message.py
+-rw-r--r--  2.0 unx    18688 b- defN 23-Jun-30 11:14 xia_api/rest.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:19 xia_api-0.1.22.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      458 b- defN 23-Jun-30 11:19 xia_api-0.1.22.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:19 xia_api-0.1.22.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 11:19 xia_api-0.1.22.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      694 b- defN 23-Jun-30 11:19 xia_api-0.1.22.dist-info/RECORD
+9 files, 24501 bytes uncompressed, 6680 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_api/message.py
 Comment: 
 
 Filename: xia_api/rest.py
 Comment: 
 
-Filename: xia_api-0.1.21.dist-info/LICENSE.txt
+Filename: xia_api-0.1.22.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_api-0.1.21.dist-info/METADATA
+Filename: xia_api-0.1.22.dist-info/METADATA
 Comment: 
 
-Filename: xia_api-0.1.21.dist-info/WHEEL
+Filename: xia_api-0.1.22.dist-info/WHEEL
 Comment: 
 
-Filename: xia_api-0.1.21.dist-info/top_level.txt
+Filename: xia_api-0.1.22.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_api-0.1.21.dist-info/RECORD
+Filename: xia_api-0.1.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_api/__init__.py

```diff
@@ -7,8 +7,8 @@
 __all__ = [
     "AuthClient",
     "RestApi", "error_handle",
     "XiaCollectionDeleteMsg", "XiaDocumentDeleteMsg", "XiaFileMsg", "XiaRecordBook", "XiaRecordItem",
     "XiaErrorMessage", "XiaActionResult"
 ]
 
-__version__ = "0.1.21"
+__version__ = "0.1.22"
```

## Comparing `xia_api-0.1.21.dist-info/RECORD` & `xia_api-0.1.22.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_api/__init__.py,sha256=Z4j_d7U2ljA9nrGZ-tX94KeCQ498q3TaJ2ppfM_rGjc,497
+xia_api/__init__.py,sha256=09EcBfQ-HI4uok1dCIh2_fOer284LFzlL4jcOXdtuDc,497
 xia_api/auth_client.py,sha256=3gil1nZcpCJWofPlqLBHBVx9or06u5vBseoTyCPca1w,1577
 xia_api/message.py,sha256=9sAiVt2D-4_K3-_K36vfG2GooIBAAiKIBRoLIKKKkQs,2329
 xia_api/rest.py,sha256=95F4grhmdjxVJuIPGBowsgSNN0Ch0C-DBW-TKeM5_9Q,18688
-xia_api-0.1.21.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_api-0.1.21.dist-info/METADATA,sha256=BDEJ78rFx-ywdWXi9pKX4m5Vk4vKUdsb-XN_VuC2IIs,677
-xia_api-0.1.21.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_api-0.1.21.dist-info/top_level.txt,sha256=krL7__RbzvbaNfgnuF-oCqAnr2y3Yy6whD8CBZyVXyw,8
-xia_api-0.1.21.dist-info/RECORD,,
+xia_api-0.1.22.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_api-0.1.22.dist-info/METADATA,sha256=4OxvREe2rIdaZyBOlo00Ni9Lem_f8iMcqpDqSxucjUk,458
+xia_api-0.1.22.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_api-0.1.22.dist-info/top_level.txt,sha256=krL7__RbzvbaNfgnuF-oCqAnr2y3Yy6whD8CBZyVXyw,8
+xia_api-0.1.22.dist-info/RECORD,,
```

