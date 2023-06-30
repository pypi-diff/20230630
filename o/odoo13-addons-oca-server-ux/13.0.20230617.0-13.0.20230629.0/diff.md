# Comparing `tmp/odoo13_addons_oca_server_ux-13.0.20230617.0-py3-none-any.whl.zip` & `tmp/odoo13_addons_oca_server_ux-13.0.20230629.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1687 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1997 b- defN 23-Jun-18 05:11 odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 05:11 odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-18 05:11 odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      417 b- defN 23-Jun-18 05:11 odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/RECORD
-4 files, 2507 bytes uncompressed, 865 bytes compressed:  65.5%
+Zip file size: 1699 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2088 b- defN 23-Jun-30 06:33 odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 06:33 odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-30 06:33 odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      417 b- defN 23-Jun-30 06:33 odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/RECORD
+4 files, 2598 bytes uncompressed, 877 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/METADATA
+Filename: odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/WHEEL
+Filename: odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/top_level.txt
+Filename: odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/RECORD
+Filename: odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addons_oca_server_ux-13.0.20230617.0.dist-info/METADATA` & `odoo13_addons_oca_server_ux-13.0.20230629.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: odoo13-addons-oca-server-ux
-Version: 13.0.20230617.0
+Version: 13.0.20230629.0
 Summary: Meta package for oca-server-ux Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
 Requires-Dist: odoo13-addon-announcement
 Requires-Dist: odoo13-addon-barcode-action
 Requires-Dist: odoo13-addon-base-action-visibility-restriction
+Requires-Dist: odoo13-addon-base-archive-date
 Requires-Dist: odoo13-addon-base-binary-url-import
 Requires-Dist: odoo13-addon-base-custom-filter
 Requires-Dist: odoo13-addon-base-duplicate-security-group
 Requires-Dist: odoo13-addon-base-export-manager
 Requires-Dist: odoo13-addon-base-field-deprecated
 Requires-Dist: odoo13-addon-base-import-security-group
 Requires-Dist: odoo13-addon-base-ir-actions-sequence
@@ -37,10 +38,11 @@
 Requires-Dist: odoo13-addon-filter-multi-user
 Requires-Dist: odoo13-addon-mass-editing
 Requires-Dist: odoo13-addon-mass-operation-abstract
 Requires-Dist: odoo13-addon-multi-step-wizard
 Requires-Dist: odoo13-addon-sequence-check-digit
 Requires-Dist: odoo13-addon-sequence-reset-period
 Requires-Dist: odoo13-addon-test-base-binary-url-import
+Requires-Dist: odoo13-addon-web-archive-date
 
 UNKNOWN
```

