# Comparing `tmp/xia_logger_gcp-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger_gcp-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2347 bytes, number of entries: 7
--rw-r--r--  2.0 unx       97 b- defN 23-Jun-29 20:52 xia_logger_gcp/__init__.py
--rw-r--r--  2.0 unx      549 b- defN 23-Jun-29 20:52 xia_logger_gcp/logger.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      690 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      584 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/RECORD
-7 files, 2185 bytes uncompressed, 1297 bytes compressed:  40.6%
+Zip file size: 2265 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-30 11:32 xia_logger_gcp/__init__.py
+-rw-r--r--  2.0 unx      549 b- defN 23-Jun-30 11:32 xia_logger_gcp/logger.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      456 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      584 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/RECORD
+7 files, 1951 bytes uncompressed, 1215 bytes compressed:  37.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger_gcp/__init__.py
 Comment: 
 
 Filename: xia_logger_gcp/logger.py
 Comment: 
 
-Filename: xia_logger_gcp-0.1.2.dist-info/LICENSE.txt
+Filename: xia_logger_gcp-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger_gcp-0.1.2.dist-info/METADATA
+Filename: xia_logger_gcp-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger_gcp-0.1.2.dist-info/WHEEL
+Filename: xia_logger_gcp-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger_gcp-0.1.2.dist-info/top_level.txt
+Filename: xia_logger_gcp-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger_gcp-0.1.2.dist-info/RECORD
+Filename: xia_logger_gcp-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger_gcp/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger_gcp.logger import GcpLogger
 
 __all__ = [
     "GcpLogger"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_logger_gcp-0.1.2.dist-info/RECORD` & `xia_logger_gcp-0.1.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_logger_gcp/__init__.py,sha256=lhUKucqLN-vKwbidjiyjtF0ZG1SHtTaSS5af5YhYUrM,97
+xia_logger_gcp/__init__.py,sha256=LNHxjNiRVHtAczcb_YQnueeezcC5Jg_TF_SF7enrBI0,97
 xia_logger_gcp/logger.py,sha256=sz-E3pDHuTURtUfhhGqluuIxIqP3DI1MISpdNIhF4-E,549
-xia_logger_gcp-0.1.2.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_logger_gcp-0.1.2.dist-info/METADATA,sha256=zLAvOKTB5nB-60xrxEqtP7VaksHLMCYxu2O0pcwF-0A,690
-xia_logger_gcp-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_logger_gcp-0.1.2.dist-info/top_level.txt,sha256=c5S6Io75CGyFOYz1y3f4z_covUMj-YmHjiiIOd_Fdm8,15
-xia_logger_gcp-0.1.2.dist-info/RECORD,,
+xia_logger_gcp-0.1.3.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_logger_gcp-0.1.3.dist-info/METADATA,sha256=Xc9OnLbfAqpnDRysMwCMlNN6daTQai0Q-JCYHP3pQEU,456
+xia_logger_gcp-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_logger_gcp-0.1.3.dist-info/top_level.txt,sha256=c5S6Io75CGyFOYz1y3f4z_covUMj-YmHjiiIOd_Fdm8,15
+xia_logger_gcp-0.1.3.dist-info/RECORD,,
```

