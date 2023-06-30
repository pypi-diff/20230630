# Comparing `tmp/xia_service_cloudflare-0.0.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_service_cloudflare-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 234088 bytes, number of entries: 8
--rw-r--r--  2.0 unx      294 b- defN 23-Jun-26 09:24 xia_service_cloudflare/__init__.py
--rw-r--r--  2.0 unx   336896 b- defN 23-Jun-26 09:25 xia_service_cloudflare/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   248832 b- defN 23-Jun-26 09:26 xia_service_cloudflare/service.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 09:26 xia_service_cloudflare-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      711 b- defN 23-Jun-26 09:26 xia_service_cloudflare-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 09:26 xia_service_cloudflare-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-26 09:26 xia_service_cloudflare-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      768 b- defN 23-Jun-26 09:26 xia_service_cloudflare-0.0.3.dist-info/RECORD
-8 files, 587774 bytes uncompressed, 232720 bytes compressed:  60.4%
+Zip file size: 3877 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      293 b- defN 23-Jun-29 20:58 xia_service_cloudflare/__init__.py
+-rw-r--r--  2.0 unx     5892 b- defN 23-Jun-29 20:14 xia_service_cloudflare/engine.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-29 20:14 xia_service_cloudflare/service.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:01 xia_service_cloudflare-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      711 b- defN 23-Jun-29 21:01 xia_service_cloudflare-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:01 xia_service_cloudflare-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-29 21:01 xia_service_cloudflare-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      731 b- defN 23-Jun-29 21:01 xia_service_cloudflare-0.0.4.dist-info/RECORD
+8 files, 8031 bytes uncompressed, 2573 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: xia_service_cloudflare/__init__.py
 Comment: 
 
-Filename: xia_service_cloudflare/engine.cp39-win_amd64.pyd
+Filename: xia_service_cloudflare/engine.py
 Comment: 
 
-Filename: xia_service_cloudflare/service.cp39-win_amd64.pyd
+Filename: xia_service_cloudflare/service.py
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.3.dist-info/LICENSE.txt
+Filename: xia_service_cloudflare-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.3.dist-info/METADATA
+Filename: xia_service_cloudflare-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.3.dist-info/WHEEL
+Filename: xia_service_cloudflare-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.3.dist-info/top_level.txt
+Filename: xia_service_cloudflare-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.3.dist-info/RECORD
+Filename: xia_service_cloudflare-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_service_cloudflare/__init__.py

```diff
@@ -4,8 +4,8 @@
 
 __all__ = [
     "CfServiceAdmEngine", "CfServiceAdmParam", "CfServiceAdmClient",
     "CloudflareService"
 ]
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `xia_service_cloudflare-0.0.3.dist-info/METADATA` & `xia_service_cloudflare-0.0.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-service-cloudflare
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-service-cloudflare/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-service-cloudflare/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

