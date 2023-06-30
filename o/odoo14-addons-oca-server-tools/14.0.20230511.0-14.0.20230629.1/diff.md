# Comparing `tmp/odoo14_addons_oca_server_tools-14.0.20230511.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_server_tools-14.0.20230629.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2038 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3667 b- defN 23-May-12 07:36 odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 07:36 odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-12 07:36 odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      429 b- defN 23-May-12 07:36 odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/RECORD
-4 files, 4189 bytes uncompressed, 1192 bytes compressed:  71.5%
+Zip file size: 2056 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3761 b- defN 23-Jun-30 06:31 odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 06:31 odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-30 06:31 odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      429 b- defN 23-Jun-30 06:31 odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/RECORD
+4 files, 4283 bytes uncompressed, 1210 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/METADATA
+Filename: odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/RECORD
+Filename: odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_server_tools-14.0.20230511.0.dist-info/METADATA` & `odoo14_addons_oca_server_tools-14.0.20230629.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-server-tools
-Version: 14.0.20230511.0
+Version: 14.0.20230629.1
 Summary: Meta package for oca-server-tools Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -13,19 +13,21 @@
 Requires-Dist: odoo14-addon-attachment-synchronize
 Requires-Dist: odoo14-addon-attachment-unindex-content
 Requires-Dist: odoo14-addon-auditlog
 Requires-Dist: odoo14-addon-auto-backup
 Requires-Dist: odoo14-addon-autovacuum-message-attachment
 Requires-Dist: odoo14-addon-base-changeset
 Requires-Dist: odoo14-addon-base-conditional-image
+Requires-Dist: odoo14-addon-base-contextvars
 Requires-Dist: odoo14-addon-base-cron-exclusion
 Requires-Dist: odoo14-addon-base-custom-info
 Requires-Dist: odoo14-addon-base-deterministic-session-gc
 Requires-Dist: odoo14-addon-base-exception
 Requires-Dist: odoo14-addon-base-fontawesome
+Requires-Dist: odoo14-addon-base-future-response
 Requires-Dist: odoo14-addon-base-generate-code
 Requires-Dist: odoo14-addon-base-jsonify
 Requires-Dist: odoo14-addon-base-kanban-stage
 Requires-Dist: odoo14-addon-base-kanban-stage-state
 Requires-Dist: odoo14-addon-base-m2m-custom-field
 Requires-Dist: odoo14-addon-base-model-restrict-update
 Requires-Dist: odoo14-addon-base-multi-image
```

