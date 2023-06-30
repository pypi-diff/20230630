# Comparing `tmp/xia_easy_proto-1.0.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_easy_proto-1.0.7-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5894 bytes, number of entries: 7
--rw-r--r--  2.0 unx       96 b- defN 23-Jun-29 20:39 xia_easy_proto/__init__.py
--rw-r--r--  2.0 unx     6009 b- defN 23-Jun-29 20:39 xia_easy_proto/proto.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:43 xia_easy_proto-1.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     7084 b- defN 23-Jun-29 20:43 xia_easy_proto-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:43 xia_easy_proto-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 20:43 xia_easy_proto-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      585 b- defN 23-Jun-29 20:43 xia_easy_proto-1.0.6.dist-info/RECORD
-7 files, 14039 bytes uncompressed, 4846 bytes compressed:  65.5%
+Zip file size: 3500 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-30 11:22 xia_easy_proto/__init__.py
+-rw-r--r--  2.0 unx     6009 b- defN 23-Jun-30 09:52 xia_easy_proto/proto.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      418 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      584 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/RECORD
+7 files, 7372 bytes uncompressed, 2452 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_easy_proto/__init__.py
 Comment: 
 
 Filename: xia_easy_proto/proto.py
 Comment: 
 
-Filename: xia_easy_proto-1.0.6.dist-info/LICENSE.txt
+Filename: xia_easy_proto-1.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_easy_proto-1.0.6.dist-info/METADATA
+Filename: xia_easy_proto-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_easy_proto-1.0.6.dist-info/WHEEL
+Filename: xia_easy_proto-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_easy_proto-1.0.6.dist-info/top_level.txt
+Filename: xia_easy_proto-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_easy_proto-1.0.6.dist-info/RECORD
+Filename: xia_easy_proto-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_easy_proto/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_easy_proto.proto import EasyProto
 
 __all__ = [
     "EasyProto"
 ]
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
```

## Comparing `xia_easy_proto-1.0.6.dist-info/RECORD` & `xia_easy_proto-1.0.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_easy_proto/__init__.py,sha256=u4u507cNY--ObFgBUGABHJ2ndzboE6_LYML6AookPEI,96
+xia_easy_proto/__init__.py,sha256=bMUnBIxTwbSq8AI6IyMakov3awrUyMQZUcjbPCTJ0ow,96
 xia_easy_proto/proto.py,sha256=r9ca8pyRsSMvFQgIrcMJdeGVNchGNPgAEfLrj05Y3Qs,6009
-xia_easy_proto-1.0.6.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_easy_proto-1.0.6.dist-info/METADATA,sha256=xnHpJupDggotW1fEwSxYYLWmSIgDd1TIN0h9IJoK9R4,7084
-xia_easy_proto-1.0.6.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_easy_proto-1.0.6.dist-info/top_level.txt,sha256=KPFU7QdTuBBTOvgTGU291M0vL3KHeNgMRHO3mvz1jAc,15
-xia_easy_proto-1.0.6.dist-info/RECORD,,
+xia_easy_proto-1.0.7.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_easy_proto-1.0.7.dist-info/METADATA,sha256=bNP7jCffNByipJJLTgEWTnd4IJ0_K2hmt-jd453j7dI,418
+xia_easy_proto-1.0.7.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_easy_proto-1.0.7.dist-info/top_level.txt,sha256=KPFU7QdTuBBTOvgTGU291M0vL3KHeNgMRHO3mvz1jAc,15
+xia_easy_proto-1.0.7.dist-info/RECORD,,
```

