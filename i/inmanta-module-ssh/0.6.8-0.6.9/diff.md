# Comparing `tmp/inmanta_module_ssh-0.6.8-py3-none-any.whl.zip` & `tmp/inmanta_module_ssh-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4668 bytes, number of entries: 9
--rw-rw-r--  2.0 unx     1554 b- defN 22-Apr-21 10:17 inmanta_plugins/ssh/__init__.py
--rw-rw-r--  2.0 unx      313 b- defN 22-Apr-21 10:17 inmanta_plugins/ssh/setup.cfg
--rw-rw-r--  2.0 unx     2322 b- defN 22-Apr-21 10:17 inmanta_plugins/ssh/model/_init.cf
--rw-rw-r--  2.0 unx      246 b- defN 22-Apr-21 10:17 inmanta_plugins/ssh/templates/authorized_keys
--rw-rw-r--  2.0 unx     1186 b- defN 22-Apr-21 10:17 inmanta_plugins/ssh/templates/sshd_config.tmpl
--rw-rw-r--  2.0 unx      194 b- defN 22-Apr-21 10:17 inmanta_module_ssh-0.6.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-21 10:17 inmanta_module_ssh-0.6.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 22-Apr-21 10:17 inmanta_module_ssh-0.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      809 b- defN 22-Apr-21 10:17 inmanta_module_ssh-0.6.8.dist-info/RECORD
-9 files, 6732 bytes uncompressed, 3248 bytes compressed:  51.8%
+Zip file size: 4669 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx     1554 b- defN 22-Apr-25 06:59 inmanta_plugins/ssh/__init__.py
+-rw-rw-r--  2.0 unx      313 b- defN 22-Apr-25 06:59 inmanta_plugins/ssh/setup.cfg
+-rw-rw-r--  2.0 unx     2322 b- defN 22-Apr-25 06:59 inmanta_plugins/ssh/model/_init.cf
+-rw-rw-r--  2.0 unx      246 b- defN 22-Apr-25 06:59 inmanta_plugins/ssh/templates/authorized_keys
+-rw-rw-r--  2.0 unx     1186 b- defN 22-Apr-25 06:59 inmanta_plugins/ssh/templates/sshd_config.tmpl
+-rw-rw-r--  2.0 unx      194 b- defN 22-Apr-25 06:59 inmanta_module_ssh-0.6.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Apr-25 06:59 inmanta_module_ssh-0.6.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 22-Apr-25 06:59 inmanta_module_ssh-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      809 b- defN 22-Apr-25 06:59 inmanta_module_ssh-0.6.9.dist-info/RECORD
+9 files, 6732 bytes uncompressed, 3249 bytes compressed:  51.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: inmanta_plugins/ssh/templates/authorized_keys
 Comment: 
 
 Filename: inmanta_plugins/ssh/templates/sshd_config.tmpl
 Comment: 
 
-Filename: inmanta_module_ssh-0.6.8.dist-info/METADATA
+Filename: inmanta_module_ssh-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_ssh-0.6.8.dist-info/WHEEL
+Filename: inmanta_module_ssh-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_ssh-0.6.8.dist-info/top_level.txt
+Filename: inmanta_module_ssh-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_ssh-0.6.8.dist-info/RECORD
+Filename: inmanta_module_ssh-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/ssh/setup.cfg

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = inmanta-module-ssh
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.6.8
+version = 0.6.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-ip
 	inmanta-module-std
 zip_safe = False
 include_package_data = True
```

