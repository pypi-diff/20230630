# Comparing `tmp/inmanta_module_mysql-0.6.8-py3-none-any.whl.zip` & `tmp/inmanta_module_mysql-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 8295 bytes, number of entries: 15
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/__init__.py
--rw-rw-r--  2.0 unx      718 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/setup.cfg
--rw-rw-r--  2.0 unx      189 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/files/mysql_create_db.service
--rw-rw-r--  2.0 unx       62 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/files/mysqld_sysconfig
--rwxrwxr-x  2.0 unx      518 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/files/redhat_mysql_create_db
--rwxrwxr-x  2.0 unx      492 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/files/ubuntu_mysql_create_db
--rw-rw-r--  2.0 unx     6475 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/model/_init.cf
--rw-rw-r--  2.0 unx      113 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/templates/databases.tmpl
--rw-rw-r--  2.0 unx      369 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/templates/mariadb.cnf.tmpl
--rw-rw-r--  2.0 unx      517 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/templates/my.cnf.tmpl
--rw-rw-r--  2.0 unx     2885 b- defN 22-Sep-28 08:46 inmanta_plugins/mysql/templates/my.cnf.ubuntu.tmpl
--rw-rw-r--  2.0 unx      187 b- defN 22-Sep-28 08:46 inmanta_module_mysql-0.6.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-28 08:46 inmanta_module_mysql-0.6.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 22-Sep-28 08:46 inmanta_module_mysql-0.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1446 b- defN 22-Sep-28 08:46 inmanta_module_mysql-0.6.8.dist-info/RECORD
-15 files, 14079 bytes uncompressed, 5809 bytes compressed:  58.7%
+Zip file size: 8293 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/__init__.py
+-rw-rw-r--  2.0 unx      718 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/setup.cfg
+-rw-rw-r--  2.0 unx      189 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/files/mysql_create_db.service
+-rw-rw-r--  2.0 unx       62 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/files/mysqld_sysconfig
+-rwxrwxr-x  2.0 unx      518 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/files/redhat_mysql_create_db
+-rwxrwxr-x  2.0 unx      492 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/files/ubuntu_mysql_create_db
+-rw-rw-r--  2.0 unx     6475 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/model/_init.cf
+-rw-rw-r--  2.0 unx      113 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/templates/databases.tmpl
+-rw-rw-r--  2.0 unx      369 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/templates/mariadb.cnf.tmpl
+-rw-rw-r--  2.0 unx      517 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/templates/my.cnf.tmpl
+-rw-rw-r--  2.0 unx     2885 b- defN 22-Nov-29 13:42 inmanta_plugins/mysql/templates/my.cnf.ubuntu.tmpl
+-rw-rw-r--  2.0 unx      187 b- defN 22-Nov-29 13:42 inmanta_module_mysql-0.6.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Nov-29 13:42 inmanta_module_mysql-0.6.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 22-Nov-29 13:42 inmanta_module_mysql-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1446 b- defN 22-Nov-29 13:42 inmanta_module_mysql-0.6.9.dist-info/RECORD
+15 files, 14079 bytes uncompressed, 5807 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: inmanta_plugins/mysql/templates/my.cnf.tmpl
 Comment: 
 
 Filename: inmanta_plugins/mysql/templates/my.cnf.ubuntu.tmpl
 Comment: 
 
-Filename: inmanta_module_mysql-0.6.8.dist-info/METADATA
+Filename: inmanta_module_mysql-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_mysql-0.6.8.dist-info/WHEEL
+Filename: inmanta_module_mysql-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_mysql-0.6.8.dist-info/top_level.txt
+Filename: inmanta_module_mysql-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_mysql-0.6.8.dist-info/RECORD
+Filename: inmanta_module_mysql-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/mysql/setup.cfg

```diff
@@ -17,15 +17,15 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-mysql
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.6.8
+version = 0.6.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-exec
 	inmanta-module-ip
 	inmanta-module-std
 zip_safe = False
```

## Comparing `inmanta_module_mysql-0.6.8.dist-info/RECORD` & `inmanta_module_mysql-0.6.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 inmanta_plugins/mysql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inmanta_plugins/mysql/setup.cfg,sha256=mJ8UgQLkwkajUYxi8W_k48w-EYatOCH6ml6NVC38Tt4,718
+inmanta_plugins/mysql/setup.cfg,sha256=IifgCR9xb3j7mrnVIsci9l4w6w85A5zjbMByA1iohcQ,718
 inmanta_plugins/mysql/files/mysql_create_db.service,sha256=QE63EaEJvNF_BfWwNq2KFzyn8idrzIVqoqadlM3jubg,189
 inmanta_plugins/mysql/files/mysqld_sysconfig,sha256=_18iiDuKx7NOx4QYsvMW_4G0TufgJL1VfBTedwWPfMw,62
 inmanta_plugins/mysql/files/redhat_mysql_create_db,sha256=M_YxWZVnivcMLD2k2pkir9ipn2nCCjt9ZWTzo6h-jFg,518
 inmanta_plugins/mysql/files/ubuntu_mysql_create_db,sha256=mUkqCfkNzxmLyBorugyhWVd7G96mex5-jop1HkkQlUA,492
 inmanta_plugins/mysql/model/_init.cf,sha256=ynB-Z4DsRcwkBEXpiqfLdPln7UGCyM06S1bsy6PaxxA,6475
 inmanta_plugins/mysql/templates/databases.tmpl,sha256=ux57XJySj8Yw68t2yw4jb23BmvBnLFpYoTXk6d_nLK4,113
 inmanta_plugins/mysql/templates/mariadb.cnf.tmpl,sha256=UVa5yxtHnx7hyGMnT03JktjA1uHIUMRcQzs_ukKggNA,369
 inmanta_plugins/mysql/templates/my.cnf.tmpl,sha256=zfe2_9qaCBFzcrpJHx_QsfabYTK9YKuTZ1fmjYqufA4,517
 inmanta_plugins/mysql/templates/my.cnf.ubuntu.tmpl,sha256=7vNvxorHjiuCISXm9mdAYdwiKDZTpnpPTwXbuB7gdY4,2885
-inmanta_module_mysql-0.6.8.dist-info/METADATA,sha256=EzYOWfdBJuXIlJQvBsvQCrY67Ucv0z0_ti3F0I9G-Vc,187
-inmanta_module_mysql-0.6.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inmanta_module_mysql-0.6.8.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_mysql-0.6.8.dist-info/RECORD,,
+inmanta_module_mysql-0.6.9.dist-info/METADATA,sha256=J3tvQTVqTBiXXIYhCI4o4CcfrJgCCudLClwLRR5bLDE,187
+inmanta_module_mysql-0.6.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+inmanta_module_mysql-0.6.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_mysql-0.6.9.dist-info/RECORD,,
```

