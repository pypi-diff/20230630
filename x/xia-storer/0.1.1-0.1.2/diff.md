# Comparing `tmp/xia_storer-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_storer-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 113353 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-26 14:11 xia_storer/__init__.py
--rw-r--r--  2.0 unx   278016 b- defN 23-Jun-26 14:14 xia_storer/storer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 14:14 xia_storer-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      623 b- defN 23-Jun-26 14:14 xia_storer-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 14:14 xia_storer-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-26 14:14 xia_storer-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      576 b- defN 23-Jun-26 14:14 xia_storer-0.1.1.dist-info/RECORD
-7 files, 279592 bytes uncompressed, 112327 bytes compressed:  59.8%
+Zip file size: 2581 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-29 21:00 xia_storer/__init__.py
+-rw-r--r--  2.0 unx     1994 b- defN 23-Jun-29 21:00 xia_storer/storer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:02 xia_storer-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      623 b- defN 23-Jun-29 21:02 xia_storer-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:02 xia_storer-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 21:02 xia_storer-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      558 b- defN 23-Jun-29 21:02 xia_storer-0.1.2.dist-info/RECORD
+7 files, 3551 bytes uncompressed, 1587 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_storer/__init__.py
 Comment: 
 
-Filename: xia_storer/storer.cp39-win_amd64.pyd
+Filename: xia_storer/storer.py
 Comment: 
 
-Filename: xia_storer-0.1.1.dist-info/LICENSE.txt
+Filename: xia_storer-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_storer-0.1.1.dist-info/METADATA
+Filename: xia_storer-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_storer-0.1.1.dist-info/WHEEL
+Filename: xia_storer-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_storer-0.1.1.dist-info/top_level.txt
+Filename: xia_storer-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_storer-0.1.1.dist-info/RECORD
+Filename: xia_storer-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_storer/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 
 __all__ = [
     'Storer', "FileStorer"
 ]
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_storer-0.1.1.dist-info/METADATA` & `xia_storer-0.1.2.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-storer
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-storer/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-storer/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_storer-0.1.1.dist-info/RECORD` & `xia_storer-0.1.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_storer/__init__.py,sha256=EsyUszh6SweGlOapHhOeOpG401n_ZkKijXFH0GPjxzI,116
-xia_storer/storer.cp39-win_amd64.pyd,sha256=4iZWn5-Fhh_K6NJYezuNcAwOE-ASVI6x9MtR4l8jZd0,278016
-xia_storer-0.1.1.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_storer-0.1.1.dist-info/METADATA,sha256=nANK7R7UZEyi4MrJD0y0Pw3XOOUJEPtgjXSrZQCu4wE,623
-xia_storer-0.1.1.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_storer-0.1.1.dist-info/top_level.txt,sha256=qVGcZtbSEokZNMgGUQhw9e9FoXdlHNNCf412j7p_i1c,11
-xia_storer-0.1.1.dist-info/RECORD,,
+xia_storer/__init__.py,sha256=NxJ__nZXSkPQCn1VkgaHCT5L-zRjr3lEudMuhZAWj_Y,115
+xia_storer/storer.py,sha256=c02AUqMwvqeqSWyFQbZ8m4SDP1IaIu-aLerVWT304B4,1994
+xia_storer-0.1.2.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_storer-0.1.2.dist-info/METADATA,sha256=BqbU-tnbBwAnaBLbbup2zRwacAVbjrKSHh1uNH9t-Fw,623
+xia_storer-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_storer-0.1.2.dist-info/top_level.txt,sha256=qVGcZtbSEokZNMgGUQhw9e9FoXdlHNNCf412j7p_i1c,11
+xia_storer-0.1.2.dist-info/RECORD,,
```

