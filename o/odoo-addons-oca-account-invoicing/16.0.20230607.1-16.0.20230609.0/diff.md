# Comparing `tmp/odoo_addons_oca_account_invoicing-16.0.20230607.1-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_invoicing-16.0.20230609.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1652 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2013 b- defN 23-Jun-08 02:48 odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 02:48 odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-08 02:48 odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      441 b- defN 23-Jun-08 02:48 odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/RECORD
-4 files, 2547 bytes uncompressed, 782 bytes compressed:  69.3%
+Zip file size: 1662 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2091 b- defN 23-Jun-10 02:45 odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:45 odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 02:45 odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      441 b- defN 23-Jun-10 02:45 odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/RECORD
+4 files, 2625 bytes uncompressed, 792 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/METADATA
+Filename: odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/WHEEL
+Filename: odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/RECORD
+Filename: odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_invoicing-16.0.20230607.1.dist-info/METADATA` & `odoo_addons_oca_account_invoicing-16.0.20230609.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-invoicing
-Version: 16.0.20230607.1
+Version: 16.0.20230609.0
 Summary: Meta package for oca-account-invoicing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-account-invoice-blocking (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-change-currency (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-check-total (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-currency-taxes (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-fiscal-position-update (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-merge (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-pricelist (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-account-invoice-pricelist-sale (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-refund-line-selection (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-refund-link (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-tax-required (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-transmit-method (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-triple-discount (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-menu-invoice-refund (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-receipt-journal (<16.1dev,>=16.0dev)
```

