# Comparing `tmp/xia_engine-0.8.26-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine-0.8.27-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 36952 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1513 b- defN 23-Jun-29 20:44 xia_engine/__init__.py
+Zip file size: 36827 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jun-30 11:24 xia_engine/__init__.py
 -rw-r--r--  2.0 unx    14239 b- defN 23-Jun-29 20:44 xia_engine/acl.py
 -rw-r--r--  2.0 unx    35369 b- defN 23-Jun-29 20:44 xia_engine/base.py
 -rw-r--r--  2.0 unx    52305 b- defN 23-Jun-29 20:44 xia_engine/document.py
 -rw-r--r--  2.0 unx    43611 b- defN 23-Jun-29 20:44 xia_engine/engine.py
 -rw-r--r--  2.0 unx      961 b- defN 23-Jun-29 20:44 xia_engine/exception.py
 -rw-r--r--  2.0 unx    15335 b- defN 23-Jun-29 20:44 xia_engine/fields.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:46 xia_engine-0.8.26.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      747 b- defN 23-Jun-29 20:46 xia_engine-0.8.26.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:46 xia_engine-0.8.26.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:46 xia_engine-0.8.26.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      953 b- defN 23-Jun-29 20:46 xia_engine-0.8.26.dist-info/RECORD
-12 files, 165294 bytes uncompressed, 35368 bytes compressed:  78.6%
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:24 xia_engine-0.8.27.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      414 b- defN 23-Jun-30 11:24 xia_engine-0.8.27.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:24 xia_engine-0.8.27.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:24 xia_engine-0.8.27.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      954 b- defN 23-Jun-30 11:24 xia_engine-0.8.27.dist-info/RECORD
+12 files, 164971 bytes uncompressed, 35243 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_engine/exception.py
 Comment: 
 
 Filename: xia_engine/fields.py
 Comment: 
 
-Filename: xia_engine-0.8.26.dist-info/LICENSE.txt
+Filename: xia_engine-0.8.27.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine-0.8.26.dist-info/METADATA
+Filename: xia_engine-0.8.27.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine-0.8.26.dist-info/WHEEL
+Filename: xia_engine-0.8.27.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine-0.8.26.dist-info/top_level.txt
+Filename: xia_engine-0.8.27.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine-0.8.26.dist-info/RECORD
+Filename: xia_engine-0.8.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine/__init__.py

```diff
@@ -20,8 +20,8 @@
     "MetaEngine", "MetaRamEngine", "MetaCache", "MirrorClient", "MirrorEngine",
     "Acl", "AclItem",
     "XiaError", 'AuthorizationError', 'AuthenticationError', "OutOfQuotaError", "OutOfScopeError",
     'NotFoundError', 'ConflictError', 'BadRequestError', "UnprocessableError",
     "ServerError"
 ]
 
-__version__ = "0.8.26"
+__version__ = "0.8.27"
```

## Comparing `xia_engine-0.8.26.dist-info/RECORD` & `xia_engine-0.8.27.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_engine/__init__.py,sha256=zNzNMNFLjmd1TDTPRSMSLvUgSAkiPosDacnoEzmj9_8,1513
+xia_engine/__init__.py,sha256=MklMTPvul1s06NRqVSNO_6G_J8x1OglPB3TiIdBaW0o,1513
 xia_engine/acl.py,sha256=Ro7FDlS7bxTriLP3dz4laYvl7t8nnqN1dN7FTAuRXGM,14239
 xia_engine/base.py,sha256=5YT455WiN8UjNTzcH1ulYBdPfodkFdEWsedZ5irBlPc,35369
 xia_engine/document.py,sha256=0HRwF65iqt0ePCwiQ2BF6Rk1pMKocQhygAT5MiV6YaA,52305
 xia_engine/engine.py,sha256=o4AkyE0d-TqctNXk4TjPFswUQMNA9iLc8veWfNAu9GI,43611
 xia_engine/exception.py,sha256=3OpfXYqwsnVxTU2Jz2vyFNvKdTfA-_nWMOnBbz_PRTk,961
 xia_engine/fields.py,sha256=h8veDRJLZHX2jmgUvms0iacxMlMAMVvjNvXkP3DBwUY,15335
-xia_engine-0.8.26.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_engine-0.8.26.dist-info/METADATA,sha256=kFkCnB2me4ZRN8fAgJsNsbZ0qmcCMGNcFmgUQYh_ZQU,747
-xia_engine-0.8.26.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine-0.8.26.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
-xia_engine-0.8.26.dist-info/RECORD,,
+xia_engine-0.8.27.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_engine-0.8.27.dist-info/METADATA,sha256=2V3VAjH0JMm8n9wCSo_PunHxc2C-fQZqK5vj0cSVoWg,414
+xia_engine-0.8.27.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_engine-0.8.27.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
+xia_engine-0.8.27.dist-info/RECORD,,
```

