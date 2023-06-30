# Comparing `tmp/odoo_addons_oca_maintenance-16.0.20230608.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_maintenance-16.0.20230629.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1396 bytes, number of entries: 4
--rw-r--r--  2.0 unx      520 b- defN 23-Jun-09 04:12 odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 04:12 odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-09 04:12 odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      416 b- defN 23-Jun-09 04:12 odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/RECORD
-4 files, 1029 bytes uncompressed, 574 bytes compressed:  44.2%
+Zip file size: 1412 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      671 b- defN 23-Jun-30 04:47 odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 04:47 odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-30 04:47 odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      416 b- defN 23-Jun-30 04:47 odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/RECORD
+4 files, 1180 bytes uncompressed, 590 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/METADATA
+Filename: odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/WHEEL
+Filename: odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/RECORD
+Filename: odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_maintenance-16.0.20230608.0.dist-info/METADATA` & `odoo_addons_oca_maintenance-16.0.20230629.1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-maintenance
-Version: 16.0.20230608.0
+Version: 16.0.20230629.1
 Summary: Meta package for oca-maintenance Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-base-maintenance (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-maintenance-equipment-hierarchy (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-maintenance-equipment-image (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-maintenance-project (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-maintenance-request-sequence (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

