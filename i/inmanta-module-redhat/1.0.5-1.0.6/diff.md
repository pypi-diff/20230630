# Comparing `tmp/inmanta_module_redhat-1.0.5-py3-none-any.whl.zip` & `tmp/inmanta_module_redhat-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2870 bytes, number of entries: 7
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-04 12:46 inmanta_plugins/redhat/__init__.py
--rw-rw-r--  2.0 unx      694 b- defN 23-Apr-04 12:46 inmanta_plugins/redhat/setup.cfg
--rw-rw-r--  2.0 unx     2778 b- defN 23-Apr-04 12:46 inmanta_plugins/redhat/model/_init.cf
--rw-rw-r--  2.0 unx      120 b- defN 23-Apr-04 12:46 inmanta_module_redhat-1.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 12:46 inmanta_module_redhat-1.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-04 12:46 inmanta_module_redhat-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      623 b- defN 23-Apr-04 12:46 inmanta_module_redhat-1.0.5.dist-info/RECORD
-7 files, 4323 bytes uncompressed, 1742 bytes compressed:  59.7%
+Zip file size: 2871 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-30 09:05 inmanta_plugins/redhat/__init__.py
+-rw-rw-r--  2.0 unx      694 b- defN 23-Jun-30 09:05 inmanta_plugins/redhat/setup.cfg
+-rw-rw-r--  2.0 unx     2778 b- defN 23-Jun-30 09:05 inmanta_plugins/redhat/model/_init.cf
+-rw-rw-r--  2.0 unx      120 b- defN 23-Jun-30 09:05 inmanta_module_redhat-1.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-30 09:05 inmanta_module_redhat-1.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jun-30 09:05 inmanta_module_redhat-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      623 b- defN 23-Jun-30 09:05 inmanta_module_redhat-1.0.6.dist-info/RECORD
+7 files, 4323 bytes uncompressed, 1743 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: inmanta_plugins/redhat/setup.cfg
 Comment: 
 
 Filename: inmanta_plugins/redhat/model/_init.cf
 Comment: 
 
-Filename: inmanta_module_redhat-1.0.5.dist-info/METADATA
+Filename: inmanta_module_redhat-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_redhat-1.0.5.dist-info/WHEEL
+Filename: inmanta_module_redhat-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_redhat-1.0.5.dist-info/top_level.txt
+Filename: inmanta_module_redhat-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_redhat-1.0.5.dist-info/RECORD
+Filename: inmanta_module_redhat-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/redhat/setup.cfg

```diff
@@ -17,15 +17,15 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-redhat
 freeze_recursive = False
 freeze_operator = ~=
-version = 1.0.5
+version = 1.0.6
 license = Apache 2.0
 version_tag = 
 
 [options]
 install_requires = inmanta-module-std
 zip_safe = False
 include_package_data = True
```

