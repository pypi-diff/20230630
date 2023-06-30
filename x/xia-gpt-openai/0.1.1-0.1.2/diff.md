# Comparing `tmp/xia_gpt_openai-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_gpt_openai-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2758 bytes, number of entries: 7
--rw-r--r--  2.0 unx       94 b- defN 23-Jun-29 20:48 xia_gpt_openai/__init__.py
--rw-r--r--  2.0 unx     1724 b- defN 23-Jun-29 20:10 xia_gpt_openai/gpt.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:53 xia_gpt_openai-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      673 b- defN 23-Jun-29 20:53 xia_gpt_openai-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:53 xia_gpt_openai-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 20:53 xia_gpt_openai-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      582 b- defN 23-Jun-29 20:53 xia_gpt_openai-0.1.1.dist-info/RECORD
-7 files, 3338 bytes uncompressed, 1714 bytes compressed:  48.7%
+Zip file size: 2674 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-30 11:30 xia_gpt_openai/__init__.py
+-rw-r--r--  2.0 unx     1724 b- defN 23-Jun-30 11:30 xia_gpt_openai/gpt.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      439 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      582 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/RECORD
+7 files, 3104 bytes uncompressed, 1630 bytes compressed:  47.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_gpt_openai/__init__.py
 Comment: 
 
 Filename: xia_gpt_openai/gpt.py
 Comment: 
 
-Filename: xia_gpt_openai-0.1.1.dist-info/LICENSE.txt
+Filename: xia_gpt_openai-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.1.1.dist-info/METADATA
+Filename: xia_gpt_openai-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_gpt_openai-0.1.1.dist-info/WHEEL
+Filename: xia_gpt_openai-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_gpt_openai-0.1.1.dist-info/top_level.txt
+Filename: xia_gpt_openai-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.1.1.dist-info/RECORD
+Filename: xia_gpt_openai-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_gpt_openai/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_gpt_openai.gpt import OpenaiGpt
 
 __all__ = [
     "OpenaiGpt"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_gpt_openai-0.1.1.dist-info/RECORD` & `xia_gpt_openai-0.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_gpt_openai/__init__.py,sha256=oqHUBTWIK_HXsZ35qA8OkcE5XvdvJ8Vm76ueg-8dNqg,94
+xia_gpt_openai/__init__.py,sha256=9neW5S0hipNxn3zFbZxTAPJCQo19JeGbSXZMmkH5qE8,94
 xia_gpt_openai/gpt.py,sha256=CkS_FLsUXn_c7HG1tr81Sv9Ci43eNmWDDlRI5g36Cso,1724
-xia_gpt_openai-0.1.1.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_gpt_openai-0.1.1.dist-info/METADATA,sha256=rcIqToF_2kQsYfg4A7cG6zOpnGCAoo1sMrzhui3559U,673
-xia_gpt_openai-0.1.1.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_gpt_openai-0.1.1.dist-info/top_level.txt,sha256=jfjlRNwHE1wgDClmy0nje2mJka0SPlg7iN9E3IKxRGM,15
-xia_gpt_openai-0.1.1.dist-info/RECORD,,
+xia_gpt_openai-0.1.2.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_gpt_openai-0.1.2.dist-info/METADATA,sha256=lHcsw515Ly2Fw9zm8AyzsLmPkDwGBDu9cpK6ZucTshg,439
+xia_gpt_openai-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_gpt_openai-0.1.2.dist-info/top_level.txt,sha256=jfjlRNwHE1wgDClmy0nje2mJka0SPlg7iN9E3IKxRGM,15
+xia_gpt_openai-0.1.2.dist-info/RECORD,,
```

