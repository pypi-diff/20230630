# Comparing `tmp/xia_logger_pubsub-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger_pubsub-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3989 bytes, number of entries: 7
--rw-r--r--  2.0 unx      106 b- defN 23-Jun-29 20:50 xia_logger_pubsub/__init__.py
--rw-r--r--  2.0 unx     8477 b- defN 23-Jun-29 20:12 xia_logger_pubsub/logger.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      701 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      607 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/RECORD
-7 files, 10159 bytes uncompressed, 2897 bytes compressed:  71.5%
+Zip file size: 3905 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-30 11:32 xia_logger_pubsub/__init__.py
+-rw-r--r--  2.0 unx     8477 b- defN 23-Jun-29 20:55 xia_logger_pubsub/logger.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      461 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/RECORD
+7 files, 9919 bytes uncompressed, 2813 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger_pubsub/__init__.py
 Comment: 
 
 Filename: xia_logger_pubsub/logger.py
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.2.dist-info/LICENSE.txt
+Filename: xia_logger_pubsub-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.2.dist-info/METADATA
+Filename: xia_logger_pubsub-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.2.dist-info/WHEEL
+Filename: xia_logger_pubsub-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.2.dist-info/top_level.txt
+Filename: xia_logger_pubsub-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.2.dist-info/RECORD
+Filename: xia_logger_pubsub-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger_pubsub/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger_pubsub.logger import PubsubLogger
 
 __all__ = [
     "PubsubLogger"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_logger_pubsub-0.1.2.dist-info/RECORD` & `xia_logger_pubsub-0.1.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_logger_pubsub/__init__.py,sha256=b2sGkz7XFMF4wlNa56TrsG7Ck_3v9XycsV-g0Kxjx3c,106
+xia_logger_pubsub/__init__.py,sha256=Sr_8JjIKfgv3wBb_5Y6QxUgsCWNBhK3AxRfS4YH1fGw,106
 xia_logger_pubsub/logger.py,sha256=J4gfKeVPWEmiUx5dcHH4lBYfFbHEM3CcW2crw5bvwhc,8477
-xia_logger_pubsub-0.1.2.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_logger_pubsub-0.1.2.dist-info/METADATA,sha256=-GrKVJCjfVusBUUQdJ-Nbpa0zLgZ6k1vLT4W1rykM5k,701
-xia_logger_pubsub-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_logger_pubsub-0.1.2.dist-info/top_level.txt,sha256=Mqcsr6nvL5Sosyn07D9D1ckGO-vobonIclRaTN-5t3o,18
-xia_logger_pubsub-0.1.2.dist-info/RECORD,,
+xia_logger_pubsub-0.1.3.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_logger_pubsub-0.1.3.dist-info/METADATA,sha256=A0gWcVMLkmwKkQzSKG8pzy3K0w-cpXbyt1ALzBgDEgc,461
+xia_logger_pubsub-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_logger_pubsub-0.1.3.dist-info/top_level.txt,sha256=Mqcsr6nvL5Sosyn07D9D1ckGO-vobonIclRaTN-5t3o,18
+xia_logger_pubsub-0.1.3.dist-info/RECORD,,
```

