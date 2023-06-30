# Comparing `tmp/inmanta_module_user-0.1.8-py3-none-any.whl.zip` & `tmp/inmanta_module_user-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3487 bytes, number of entries: 10
--rw-rw-r--  2.0 unx        0 b- defN 22-Mar-15 16:24 inmanta_plugins/user/__init__.py
--rw-rw-r--  2.0 unx      259 b- defN 22-Mar-15 16:24 inmanta_plugins/user/setup.cfg
--rw-rw-r--  2.0 unx     1715 b- defN 22-Mar-15 16:23 inmanta_plugins/user/model/_init.cf
--rw-rw-r--  2.0 unx       59 b- defN 22-Mar-15 16:23 inmanta_plugins/user/templates/groupadd.j2
--rw-rw-r--  2.0 unx      170 b- defN 22-Mar-15 16:23 inmanta_plugins/user/templates/useradd.j2
--rw-rw-r--  2.0 unx      122 b- defN 22-Mar-15 16:23 tests/test_module.py
--rw-rw-r--  2.0 unx      192 b- defN 22-Mar-15 16:24 inmanta_module_user-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Mar-15 16:24 inmanta_module_user-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       26 b- defN 22-Mar-15 16:24 inmanta_module_user-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      879 b- defN 22-Mar-15 16:24 inmanta_module_user-0.1.8.dist-info/RECORD
-10 files, 3514 bytes uncompressed, 1953 bytes compressed:  44.4%
+Zip file size: 3486 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx        0 b- defN 22-Mar-16 12:38 inmanta_plugins/user/__init__.py
+-rw-rw-r--  2.0 unx      259 b- defN 22-Mar-16 12:38 inmanta_plugins/user/setup.cfg
+-rw-rw-r--  2.0 unx     1715 b- defN 22-Mar-16 12:38 inmanta_plugins/user/model/_init.cf
+-rw-rw-r--  2.0 unx       59 b- defN 22-Mar-16 12:38 inmanta_plugins/user/templates/groupadd.j2
+-rw-rw-r--  2.0 unx      170 b- defN 22-Mar-16 12:38 inmanta_plugins/user/templates/useradd.j2
+-rw-rw-r--  2.0 unx      122 b- defN 22-Mar-16 12:38 tests/test_module.py
+-rw-rw-r--  2.0 unx      192 b- defN 22-Mar-16 12:38 inmanta_module_user-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Mar-16 12:38 inmanta_module_user-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       26 b- defN 22-Mar-16 12:38 inmanta_module_user-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      879 b- defN 22-Mar-16 12:38 inmanta_module_user-0.1.9.dist-info/RECORD
+10 files, 3514 bytes uncompressed, 1952 bytes compressed:  44.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: inmanta_plugins/user/templates/useradd.j2
 Comment: 
 
 Filename: tests/test_module.py
 Comment: 
 
-Filename: inmanta_module_user-0.1.8.dist-info/METADATA
+Filename: inmanta_module_user-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_user-0.1.8.dist-info/WHEEL
+Filename: inmanta_module_user-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_user-0.1.8.dist-info/top_level.txt
+Filename: inmanta_module_user-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_user-0.1.8.dist-info/RECORD
+Filename: inmanta_module_user-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/user/setup.cfg

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = inmanta-module-user
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.1.8
+version = 0.1.9
 license = ASL 2
 
 [options]
 install_requires = inmanta-module-exec
 	inmanta-module-std
 zip_safe = False
 include_package_data = True
```

