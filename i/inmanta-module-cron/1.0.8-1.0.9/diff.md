# Comparing `tmp/inmanta_module_cron-1.0.8-py3-none-any.whl.zip` & `tmp/inmanta_module_cron-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3249 bytes, number of entries: 8
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-02 07:16 inmanta_plugins/cron/__init__.py
--rw-rw-r--  2.0 unx      692 b- defN 23-Feb-02 07:16 inmanta_plugins/cron/setup.cfg
--rw-rw-r--  2.0 unx     1622 b- defN 23-Feb-02 07:15 inmanta_plugins/cron/model/_init.cf
--rw-rw-r--  2.0 unx      197 b- defN 23-Feb-02 07:15 inmanta_plugins/cron/templates/cronjob.j2
--rw-rw-r--  2.0 unx      118 b- defN 23-Feb-02 07:16 inmanta_module_cron-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-02 07:16 inmanta_module_cron-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Feb-02 07:16 inmanta_module_cron-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      706 b- defN 23-Feb-02 07:16 inmanta_module_cron-1.0.8.dist-info/RECORD
-8 files, 3443 bytes uncompressed, 1991 bytes compressed:  42.2%
+Zip file size: 3251 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-04 12:30 inmanta_plugins/cron/__init__.py
+-rw-rw-r--  2.0 unx      692 b- defN 23-Apr-04 12:30 inmanta_plugins/cron/setup.cfg
+-rw-rw-r--  2.0 unx     1622 b- defN 23-Apr-04 12:30 inmanta_plugins/cron/model/_init.cf
+-rw-rw-r--  2.0 unx      197 b- defN 23-Apr-04 12:30 inmanta_plugins/cron/templates/cronjob.j2
+-rw-rw-r--  2.0 unx      118 b- defN 23-Apr-04 12:30 inmanta_module_cron-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 12:30 inmanta_module_cron-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Apr-04 12:30 inmanta_module_cron-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      706 b- defN 23-Apr-04 12:30 inmanta_module_cron-1.0.9.dist-info/RECORD
+8 files, 3443 bytes uncompressed, 1993 bytes compressed:  42.1%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: inmanta_plugins/cron/model/_init.cf
 Comment: 
 
 Filename: inmanta_plugins/cron/templates/cronjob.j2
 Comment: 
 
-Filename: inmanta_module_cron-1.0.8.dist-info/METADATA
+Filename: inmanta_module_cron-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_cron-1.0.8.dist-info/WHEEL
+Filename: inmanta_module_cron-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_cron-1.0.8.dist-info/top_level.txt
+Filename: inmanta_module_cron-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_cron-1.0.8.dist-info/RECORD
+Filename: inmanta_module_cron-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/cron/setup.cfg

```diff
@@ -17,15 +17,15 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-cron
 freeze_recursive = False
 freeze_operator = ~=
-version = 1.0.8
+version = 1.0.9
 license = Apache 2.0
 version_tag = 
 
 [options]
 install_requires = inmanta-module-std
 zip_safe = False
 include_package_data = True
```

