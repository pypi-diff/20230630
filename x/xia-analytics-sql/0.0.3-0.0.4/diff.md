# Comparing `tmp/xia_analytics_sql-0.0.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_analytics_sql-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2606 bytes, number of entries: 7
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-29 20:32 xia_analytics_sql/__init__.py
--rw-r--r--  2.0 unx     1186 b- defN 23-Jun-29 20:32 xia_analytics_sql/analyzer.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      609 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/RECORD
-7 files, 2859 bytes uncompressed, 1510 bytes compressed:  47.2%
+Zip file size: 2524 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-30 11:14 xia_analytics_sql/__init__.py
+-rw-r--r--  2.0 unx     1186 b- defN 23-Jun-30 10:22 xia_analytics_sql/analyzer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:17 xia_analytics_sql-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      452 b- defN 23-Jun-30 11:17 xia_analytics_sql-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:17 xia_analytics_sql-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-30 11:17 xia_analytics_sql-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      609 b- defN 23-Jun-30 11:17 xia_analytics_sql-0.0.4.dist-info/RECORD
+7 files, 2620 bytes uncompressed, 1428 bytes compressed:  45.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_analytics_sql/__init__.py
 Comment: 
 
 Filename: xia_analytics_sql/analyzer.py
 Comment: 
 
-Filename: xia_analytics_sql-0.0.3.dist-info/LICENSE.txt
+Filename: xia_analytics_sql-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_analytics_sql-0.0.3.dist-info/METADATA
+Filename: xia_analytics_sql-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_analytics_sql-0.0.3.dist-info/WHEEL
+Filename: xia_analytics_sql-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_analytics_sql-0.0.3.dist-info/top_level.txt
+Filename: xia_analytics_sql-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_analytics_sql-0.0.3.dist-info/RECORD
+Filename: xia_analytics_sql-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_analytics_sql/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_analytics_sql.analyzer import SqlAnalyzer
 
 __all__ = [
    "SqlAnalyzer"
 ]
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `xia_analytics_sql-0.0.3.dist-info/RECORD` & `xia_analytics_sql-0.0.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_analytics_sql/__init__.py,sha256=5cDXOmPpQYudRBFwFsfEyL0rARKbwPjgNkZPUNV-Jeg,105
+xia_analytics_sql/__init__.py,sha256=CRM9BguxgSA2Wb4qj4utCSwnPy8kL8Ip9kTuIQvGYDc,105
 xia_analytics_sql/analyzer.py,sha256=s4PHmL_pTleAht4y_9X2mFMqB8MW10iBeMs4oB5F_jc,1186
-xia_analytics_sql-0.0.3.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_analytics_sql-0.0.3.dist-info/METADATA,sha256=28Wt8A7J0ArnSkgUfakJTDTgI-Wb25Ni10wl6T4aO9Q,691
-xia_analytics_sql-0.0.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_analytics_sql-0.0.3.dist-info/top_level.txt,sha256=mrVMNrm-BLTdC4PUEQWdzBiSd47TAqlb99m7t0MdLok,18
-xia_analytics_sql-0.0.3.dist-info/RECORD,,
+xia_analytics_sql-0.0.4.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_analytics_sql-0.0.4.dist-info/METADATA,sha256=3jYTE7gt_1K-Lx1HvbmjWp-8RRerF249yJa2UrOEpcs,452
+xia_analytics_sql-0.0.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_analytics_sql-0.0.4.dist-info/top_level.txt,sha256=mrVMNrm-BLTdC4PUEQWdzBiSd47TAqlb99m7t0MdLok,18
+xia_analytics_sql-0.0.4.dist-info/RECORD,,
```

