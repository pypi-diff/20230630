# Comparing `tmp/xia_engine_bigquery-0.1.11-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_bigquery-0.1.12-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 459641 bytes, number of entries: 9
--rw-r--r--  2.0 unx      362 b- defN 23-Jun-26 09:46 xia_engine_bigquery/__init__.py
--rw-r--r--  2.0 unx   631808 b- defN 23-Jun-26 09:50 xia_engine_bigquery/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   304128 b- defN 23-Jun-26 09:51 xia_engine_bigquery/proto.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   299520 b- defN 23-Jun-26 09:48 xia_engine_bigquery/schema.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 09:51 xia_engine_bigquery-0.1.11.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      888 b- defN 23-Jun-26 09:51 xia_engine_bigquery-0.1.11.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 09:51 xia_engine_bigquery-0.1.11.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-26 09:51 xia_engine_bigquery-0.1.11.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      851 b- defN 23-Jun-26 09:51 xia_engine_bigquery-0.1.11.dist-info/RECORD
-9 files, 1237827 bytes uncompressed, 458149 bytes compressed:  63.0%
+Zip file size: 12162 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      361 b- defN 23-Jun-29 20:47 xia_engine_bigquery/__init__.py
+-rw-r--r--  2.0 unx    30111 b- defN 23-Jun-29 20:47 xia_engine_bigquery/engine.py
+-rw-r--r--  2.0 unx     5338 b- defN 23-Jun-29 20:47 xia_engine_bigquery/proto.py
+-rw-r--r--  2.0 unx     5526 b- defN 23-Jun-29 20:47 xia_engine_bigquery/schema.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:48 xia_engine_bigquery-0.1.12.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      888 b- defN 23-Jun-29 20:48 xia_engine_bigquery-0.1.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:48 xia_engine_bigquery-0.1.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-29 20:48 xia_engine_bigquery-0.1.12.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      798 b- defN 23-Jun-29 20:48 xia_engine_bigquery-0.1.12.dist-info/RECORD
+9 files, 43292 bytes uncompressed, 10766 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: xia_engine_bigquery/__init__.py
 Comment: 
 
-Filename: xia_engine_bigquery/engine.cp39-win_amd64.pyd
+Filename: xia_engine_bigquery/engine.py
 Comment: 
 
-Filename: xia_engine_bigquery/proto.cp39-win_amd64.pyd
+Filename: xia_engine_bigquery/proto.py
 Comment: 
 
-Filename: xia_engine_bigquery/schema.cp39-win_amd64.pyd
+Filename: xia_engine_bigquery/schema.py
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.11.dist-info/LICENSE.txt
+Filename: xia_engine_bigquery-0.1.12.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.11.dist-info/METADATA
+Filename: xia_engine_bigquery-0.1.12.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.11.dist-info/WHEEL
+Filename: xia_engine_bigquery-0.1.12.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.11.dist-info/top_level.txt
+Filename: xia_engine_bigquery-0.1.12.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.11.dist-info/RECORD
+Filename: xia_engine_bigquery-0.1.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_bigquery/__init__.py

```diff
@@ -5,8 +5,8 @@
 
 __all__ = [
     "DocToProto",
     "DocToSchema",
     "BigqueryWriteEngine", "BigqueryStreamEngine", "BigqueryAppendOnlyEngine"
 ]
 
-__version__ = "0.1.11"
+__version__ = "0.1.12"
```

## Comparing `xia_engine_bigquery-0.1.11.dist-info/METADATA` & `xia_engine_bigquery-0.1.12.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-bigquery
-Version: 0.1.11
+Version: 0.1.12
 Summary: X-I-A Document Engine on Bigquery
-Home-page: https://develop.x-i-a.com/docs/xia-engine-bigquery/0.1.11/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-bigquery/0.1.12/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_bigquery-0.1.11.dist-info/RECORD` & `xia_engine_bigquery-0.1.12.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_engine_bigquery/__init__.py,sha256=aczqGcva56rn9zb4lJcHE4VNaPqvts8TnzPXbSyus8I,362
-xia_engine_bigquery/engine.cp39-win_amd64.pyd,sha256=31wJitOylSliU_plPpsZM63PLh6ovmplsx_4cNfue8o,631808
-xia_engine_bigquery/proto.cp39-win_amd64.pyd,sha256=aaPRKuw2padlPKBG_zmf-sxp6XW37f8MGfkTZa1ciao,304128
-xia_engine_bigquery/schema.cp39-win_amd64.pyd,sha256=wDQpuomagbJZF1u9mL0NxR6g-Z2SgvuAu0wNz87cru8,299520
-xia_engine_bigquery-0.1.11.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_engine_bigquery-0.1.11.dist-info/METADATA,sha256=od_sAW5uF7_QRos4abC2W2U2ju_5qDAxIDKnE-lDV84,888
-xia_engine_bigquery-0.1.11.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_bigquery-0.1.11.dist-info/top_level.txt,sha256=_yEmJhHpPT-DWURs_JBDhoK6nResg3ySwAYjmia8-Cg,20
-xia_engine_bigquery-0.1.11.dist-info/RECORD,,
+xia_engine_bigquery/__init__.py,sha256=5Zdg_CykZaUK-f_27m8z4jBYB37l-hoIPB7GOIY1aoQ,361
+xia_engine_bigquery/engine.py,sha256=zgL4pwfmvWHpyaztPKCpa-WTY72yNJ7MjamC7Hspt1g,30111
+xia_engine_bigquery/proto.py,sha256=I6ANlJqLw6hSbRMjpgknpia0JS_YHFtw-ws707IFbrc,5338
+xia_engine_bigquery/schema.py,sha256=0y_oIn3y5God-u0x3xtyPQ8haA3YZrolDxqVfwYiqZk,5526
+xia_engine_bigquery-0.1.12.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_engine_bigquery-0.1.12.dist-info/METADATA,sha256=S0w14TBBfy1lJxWi-gwQy_-2yVv6agud77ctUfHCRJc,888
+xia_engine_bigquery-0.1.12.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_bigquery-0.1.12.dist-info/top_level.txt,sha256=_yEmJhHpPT-DWURs_JBDhoK6nResg3ySwAYjmia8-Cg,20
+xia_engine_bigquery-0.1.12.dist-info/RECORD,,
```

