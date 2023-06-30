# Comparing `tmp/xia_mail_sender-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_mail_sender-0.1.2-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2609 bytes, number of entries: 7
--rw-r--r--  2.0 unx      100 b- defN 23-Jun-29 20:53 xia_mail_sender/__init__.py
--rw-r--r--  2.0 unx     1333 b- defN 23-Jun-29 20:53 xia_mail_sender/sender.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      714 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      593 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/RECORD
-7 files, 3006 bytes uncompressed, 1545 bytes compressed:  48.6%
+Zip file size: 2518 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-30 11:34 xia_mail_sender/__init__.py
+-rw-r--r--  2.0 unx     1333 b- defN 23-Jun-29 20:54 xia_mail_sender/sender.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-30 11:35 xia_mail_sender-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      420 b- defN 23-Jun-30 11:35 xia_mail_sender-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-30 11:35 xia_mail_sender-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:35 xia_mail_sender-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      594 b- defN 23-Jun-30 11:35 xia_mail_sender-0.1.2.dist-info/RECORD
+7 files, 2722 bytes uncompressed, 1454 bytes compressed:  46.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_mail_sender/__init__.py
 Comment: 
 
 Filename: xia_mail_sender/sender.py
 Comment: 
 
-Filename: xia_mail_sender-0.1.1.dist-info/LICENSE.txt
+Filename: xia_mail_sender-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_mail_sender-0.1.1.dist-info/METADATA
+Filename: xia_mail_sender-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_mail_sender-0.1.1.dist-info/WHEEL
+Filename: xia_mail_sender-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_mail_sender-0.1.1.dist-info/top_level.txt
+Filename: xia_mail_sender-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_mail_sender-0.1.1.dist-info/RECORD
+Filename: xia_mail_sender-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_mail_sender/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_mail_sender.sender import MailSender
 
 __all__ = [
     "MailSender"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_mail_sender-0.1.1.dist-info/RECORD` & `xia_mail_sender-0.1.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_mail_sender/__init__.py,sha256=OhdqK1ahEOZ_YCyArlON0_YcTs-nv21PogepQ_KPO0k,100
+xia_mail_sender/__init__.py,sha256=vatMK36gLfSem__FDNOuFtvgrswJ0ZVK_1cN-I4i7S0,100
 xia_mail_sender/sender.py,sha256=ioaMLRFCuW_gevrOgE_nl4-C3aoGkH3INdPsb6Ffpvc,1333
-xia_mail_sender-0.1.1.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_mail_sender-0.1.1.dist-info/METADATA,sha256=HwjRQzlYSt2d_wQDjlhix4tpIYlm7gkCclyOQ5ymXhg,714
-xia_mail_sender-0.1.1.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_mail_sender-0.1.1.dist-info/top_level.txt,sha256=EW8EA08ajOwMMeu9pkLqim3lN2Lezfwz4nTYUZHeihE,16
-xia_mail_sender-0.1.1.dist-info/RECORD,,
+xia_mail_sender-0.1.2.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_mail_sender-0.1.2.dist-info/METADATA,sha256=WfBMn2S3DgezXBekH_dqSfLVRZJ9HE-2rd6l5SvA9rE,420
+xia_mail_sender-0.1.2.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_mail_sender-0.1.2.dist-info/top_level.txt,sha256=EW8EA08ajOwMMeu9pkLqim3lN2Lezfwz4nTYUZHeihE,16
+xia_mail_sender-0.1.2.dist-info/RECORD,,
```

