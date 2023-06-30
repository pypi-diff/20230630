# Comparing `tmp/xia_git-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_git-0.1.4-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3424 bytes, number of entries: 7
--rw-r--r--  2.0 unx       75 b- defN 23-Jun-29 20:50 xia_git/__init__.py
--rw-r--r--  2.0 unx     5437 b- defN 23-Jun-29 20:50 xia_git/git.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:52 xia_git-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      625 b- defN 23-Jun-29 20:52 xia_git-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:52 xia_git-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 20:52 xia_git-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      532 b- defN 23-Jun-29 20:52 xia_git-0.1.3.dist-info/RECORD
-7 files, 6927 bytes uncompressed, 2478 bytes compressed:  64.2%
+Zip file size: 3350 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-30 11:29 xia_git/__init__.py
+-rw-r--r--  2.0 unx     5437 b- defN 23-Jun-30 11:29 xia_git/git.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:29 xia_git-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      405 b- defN 23-Jun-30 11:29 xia_git-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:29 xia_git-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 11:29 xia_git-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      533 b- defN 23-Jun-30 11:29 xia_git-0.1.4.dist-info/RECORD
+7 files, 6717 bytes uncompressed, 2404 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git/__init__.py
 Comment: 
 
 Filename: xia_git/git.py
 Comment: 
 
-Filename: xia_git-0.1.3.dist-info/LICENSE.txt
+Filename: xia_git-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git-0.1.3.dist-info/METADATA
+Filename: xia_git-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_git-0.1.3.dist-info/WHEEL
+Filename: xia_git-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git-0.1.3.dist-info/top_level.txt
+Filename: xia_git-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git-0.1.3.dist-info/RECORD
+Filename: xia_git-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git.git import Git
 
 __all__ = [
     "Git"
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

