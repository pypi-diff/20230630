# Comparing `tmp/inmanta_module_net-1.0.8-py3-none-any.whl.zip` & `tmp/inmanta_module_net-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2896 bytes, number of entries: 8
--rw-rw-r--  2.0 unx        0 b- defN 22-Mar-16 12:19 inmanta_plugins/net/__init__.py
--rw-rw-r--  2.0 unx      242 b- defN 22-Mar-16 12:19 inmanta_plugins/net/setup.cfg
--rw-rw-r--  2.0 unx     1373 b- defN 22-Mar-16 12:18 inmanta_plugins/net/model/_init.cf
--rw-rw-r--  2.0 unx      149 b- defN 22-Mar-16 12:18 tests/test_module.py
--rw-rw-r--  2.0 unx      161 b- defN 22-Mar-16 12:19 inmanta_module_net-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Mar-16 12:19 inmanta_module_net-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       26 b- defN 22-Mar-16 12:19 inmanta_module_net-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      678 b- defN 22-Mar-16 12:19 inmanta_module_net-1.0.8.dist-info/RECORD
-8 files, 2721 bytes uncompressed, 1694 bytes compressed:  37.7%
+Zip file size: 2894 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx        0 b- defN 22-Apr-05 14:33 inmanta_plugins/net/__init__.py
+-rw-rw-r--  2.0 unx      242 b- defN 22-Apr-05 14:33 inmanta_plugins/net/setup.cfg
+-rw-rw-r--  2.0 unx     1373 b- defN 22-Apr-05 14:33 inmanta_plugins/net/model/_init.cf
+-rw-rw-r--  2.0 unx      149 b- defN 22-Apr-05 14:33 tests/test_module.py
+-rw-rw-r--  2.0 unx      161 b- defN 22-Apr-05 14:33 inmanta_module_net-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Apr-05 14:33 inmanta_module_net-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       26 b- defN 22-Apr-05 14:33 inmanta_module_net-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      678 b- defN 22-Apr-05 14:33 inmanta_module_net-1.0.9.dist-info/RECORD
+8 files, 2721 bytes uncompressed, 1692 bytes compressed:  37.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: inmanta_plugins/net/model/_init.cf
 Comment: 
 
 Filename: tests/test_module.py
 Comment: 
 
-Filename: inmanta_module_net-1.0.8.dist-info/METADATA
+Filename: inmanta_module_net-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_net-1.0.8.dist-info/WHEEL
+Filename: inmanta_module_net-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_net-1.0.8.dist-info/top_level.txt
+Filename: inmanta_module_net-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_net-1.0.8.dist-info/RECORD
+Filename: inmanta_module_net-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/net/setup.cfg

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = inmanta-module-net
 freeze_recursive = False
 freeze_operator = ~=
-version = 1.0.8
+version = 1.0.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-std
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
```

