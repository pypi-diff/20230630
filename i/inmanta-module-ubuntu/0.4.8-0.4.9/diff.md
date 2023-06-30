# Comparing `tmp/inmanta_module_ubuntu-0.4.8-py3-none-any.whl.zip` & `tmp/inmanta_module_ubuntu-0.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3793 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     4463 b- defN 22-Apr-21 10:28 inmanta_plugins/ubuntu/__init__.py
--rw-rw-r--  2.0 unx      317 b- defN 22-Apr-21 10:28 inmanta_plugins/ubuntu/setup.cfg
--rw-rw-r--  2.0 unx     1021 b- defN 22-Apr-21 10:28 inmanta_plugins/ubuntu/model/_init.cf
--rw-rw-r--  2.0 unx      198 b- defN 22-Apr-21 10:29 inmanta_module_ubuntu-0.4.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-21 10:29 inmanta_module_ubuntu-0.4.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 22-Apr-21 10:29 inmanta_module_ubuntu-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      626 b- defN 22-Apr-21 10:29 inmanta_module_ubuntu-0.4.8.dist-info/RECORD
-7 files, 6733 bytes uncompressed, 2665 bytes compressed:  60.4%
+Zip file size: 3795 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     4463 b- defN 22-Apr-25 07:09 inmanta_plugins/ubuntu/__init__.py
+-rw-rw-r--  2.0 unx      317 b- defN 22-Apr-25 07:09 inmanta_plugins/ubuntu/setup.cfg
+-rw-rw-r--  2.0 unx     1021 b- defN 22-Apr-25 07:09 inmanta_plugins/ubuntu/model/_init.cf
+-rw-rw-r--  2.0 unx      198 b- defN 22-Apr-25 07:09 inmanta_module_ubuntu-0.4.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Apr-25 07:09 inmanta_module_ubuntu-0.4.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 22-Apr-25 07:09 inmanta_module_ubuntu-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      626 b- defN 22-Apr-25 07:09 inmanta_module_ubuntu-0.4.9.dist-info/RECORD
+7 files, 6733 bytes uncompressed, 2667 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: inmanta_plugins/ubuntu/setup.cfg
 Comment: 
 
 Filename: inmanta_plugins/ubuntu/model/_init.cf
 Comment: 
 
-Filename: inmanta_module_ubuntu-0.4.8.dist-info/METADATA
+Filename: inmanta_module_ubuntu-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_ubuntu-0.4.8.dist-info/WHEEL
+Filename: inmanta_module_ubuntu-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_ubuntu-0.4.8.dist-info/top_level.txt
+Filename: inmanta_module_ubuntu-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_ubuntu-0.4.8.dist-info/RECORD
+Filename: inmanta_module_ubuntu-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/ubuntu/setup.cfg

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = inmanta-module-ubuntu
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.4.8
+version = 0.4.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-apt
 	inmanta-module-std
 zip_safe = False
 include_package_data = True
```

