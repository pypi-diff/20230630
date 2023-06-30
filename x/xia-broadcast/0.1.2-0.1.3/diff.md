# Comparing `tmp/xia_broadcast-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_broadcast-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4292 bytes, number of entries: 7
--rw-r--r--  2.0 unx      131 b- defN 23-Jun-29 20:33 xia_broadcast/__init__.py
--rw-r--r--  2.0 unx     7587 b- defN 23-Jun-29 20:33 xia_broadcast/broadcast.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:38 xia_broadcast-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      840 b- defN 23-Jun-29 20:38 xia_broadcast-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:38 xia_broadcast-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-29 20:38 xia_broadcast-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      582 b- defN 23-Jun-29 20:38 xia_broadcast-0.1.2.dist-info/RECORD
-7 files, 9404 bytes uncompressed, 3250 bytes compressed:  65.4%
+Zip file size: 4157 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-30 11:15 xia_broadcast/__init__.py
+-rw-r--r--  2.0 unx     7587 b- defN 23-Jun-29 17:07 xia_broadcast/broadcast.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      442 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      582 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/RECORD
+7 files, 9006 bytes uncompressed, 3115 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_broadcast/__init__.py
 Comment: 
 
 Filename: xia_broadcast/broadcast.py
 Comment: 
 
-Filename: xia_broadcast-0.1.2.dist-info/LICENSE.txt
+Filename: xia_broadcast-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_broadcast-0.1.2.dist-info/METADATA
+Filename: xia_broadcast-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_broadcast-0.1.2.dist-info/WHEEL
+Filename: xia_broadcast-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_broadcast-0.1.2.dist-info/top_level.txt
+Filename: xia_broadcast-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_broadcast-0.1.2.dist-info/RECORD
+Filename: xia_broadcast-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_broadcast/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_broadcast.broadcast import AuthClient, Broadcaster
 
 
 __all__ = [
     "AuthClient", "Broadcaster",
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_broadcast-0.1.2.dist-info/RECORD` & `xia_broadcast-0.1.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_broadcast/__init__.py,sha256=F3Y1i_Ztz1ri7K73Y3ZzJCv3KZPkQR0ztzRITd24Vyk,131
+xia_broadcast/__init__.py,sha256=gCCh9WJCjR1McgNs_PQK_q2ivlGDYpN8_BkqzaX_j6M,131
 xia_broadcast/broadcast.py,sha256=6f423ThasO3F0ff6KUqXwKgKCKhtOySfLtjLcaO2l4o,7587
-xia_broadcast-0.1.2.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_broadcast-0.1.2.dist-info/METADATA,sha256=P7KGgJ1H3qB_3YCDwkO-o3HeizN8EL7jKGD3FUFz3AM,840
-xia_broadcast-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_broadcast-0.1.2.dist-info/top_level.txt,sha256=BVEHXFDj1kIY7lo8v-H6KOU-bvTC9FQrjB2mSvZppd8,14
-xia_broadcast-0.1.2.dist-info/RECORD,,
+xia_broadcast-0.1.3.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_broadcast-0.1.3.dist-info/METADATA,sha256=0tqGZYmEMX16FhyotgdF2Sdq-JvSyMFUMZgxCoAn42E,442
+xia_broadcast-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_broadcast-0.1.3.dist-info/top_level.txt,sha256=BVEHXFDj1kIY7lo8v-H6KOU-bvTC9FQrjB2mSvZppd8,14
+xia_broadcast-0.1.3.dist-info/RECORD,,
```

