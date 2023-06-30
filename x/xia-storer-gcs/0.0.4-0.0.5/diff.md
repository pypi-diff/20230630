# Comparing `tmp/xia_storer_gcs-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_storer_gcs-0.0.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2961 bytes, number of entries: 7
--rw-r--r--  2.0 unx       83 b- defN 23-Jun-29 20:59 xia_storer_gcs/__init__.py
--rw-r--r--  2.0 unx     2653 b- defN 23-Jun-29 20:59 xia_storer_gcs/storer.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      585 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/RECORD
-7 files, 4312 bytes uncompressed, 1911 bytes compressed:  55.7%
+Zip file size: 2873 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-30 11:41 xia_storer_gcs/__init__.py
+-rw-r--r--  2.0 unx     2653 b- defN 23-Jun-30 11:41 xia_storer_gcs/storer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      477 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      585 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/RECORD
+7 files, 4063 bytes uncompressed, 1823 bytes compressed:  55.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_storer_gcs/__init__.py
 Comment: 
 
 Filename: xia_storer_gcs/storer.py
 Comment: 
 
-Filename: xia_storer_gcs-0.0.4.dist-info/LICENSE.txt
+Filename: xia_storer_gcs-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_storer_gcs-0.0.4.dist-info/METADATA
+Filename: xia_storer_gcs-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_storer_gcs-0.0.4.dist-info/WHEEL
+Filename: xia_storer_gcs-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_storer_gcs-0.0.4.dist-info/top_level.txt
+Filename: xia_storer_gcs-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_storer_gcs-0.0.4.dist-info/RECORD
+Filename: xia_storer_gcs-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_storer_gcs/__init__.py

```diff
@@ -1,8 +1,8 @@
 from storer import GcsStorer
 
 __all__ = [
     "GcsStorer"
 ]
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `xia_storer_gcs-0.0.4.dist-info/RECORD` & `xia_storer_gcs-0.0.5.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_storer_gcs/__init__.py,sha256=lJsPJwAgj63gz1rnF8cGga19mHp8bs7qCYoExRyAQj4,83
+xia_storer_gcs/__init__.py,sha256=t7QXeethblAoOBnJib9xI3R6EKOpi25FcZo6yb5K-uo,83
 xia_storer_gcs/storer.py,sha256=bz429qULWZqmQhXUxC7MnUX6EaXQulFKx8FhVC6YOdQ,2653
-xia_storer_gcs-0.0.4.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_storer_gcs-0.0.4.dist-info/METADATA,sha256=HgGXLwJZDTTayKQBMuFLLRPWkE9onZSXBitKXNqGQKs,726
-xia_storer_gcs-0.0.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_storer_gcs-0.0.4.dist-info/top_level.txt,sha256=aDNj14oeR6Vdo7cGaXCT3vqDp846HIU9Za_nxatqEiI,15
-xia_storer_gcs-0.0.4.dist-info/RECORD,,
+xia_storer_gcs-0.0.5.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_storer_gcs-0.0.5.dist-info/METADATA,sha256=-1Tn_4WlM830SYUGk45jfsSoe2dhYCGVVhPaSNQU8Dk,477
+xia_storer_gcs-0.0.5.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_storer_gcs-0.0.5.dist-info/top_level.txt,sha256=aDNj14oeR6Vdo7cGaXCT3vqDp846HIU9Za_nxatqEiI,15
+xia_storer_gcs-0.0.5.dist-info/RECORD,,
```

