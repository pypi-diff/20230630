# Comparing `tmp/inmanta_module_web-0.3.8-py3-none-any.whl.zip` & `tmp/inmanta_module_web-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 2998 bytes, number of entries: 8
--rw-rw-r--  2.0 unx        0 b- defN 22-Apr-05 15:27 inmanta_plugins/web/__init__.py
--rw-rw-r--  2.0 unx      261 b- defN 22-Apr-05 15:27 inmanta_plugins/web/setup.cfg
--rw-rw-r--  2.0 unx     2348 b- defN 22-Apr-05 15:26 inmanta_plugins/web/model/_init.cf
--rw-rw-r--  2.0 unx      121 b- defN 22-Apr-05 15:26 tests/test_module.py
--rw-rw-r--  2.0 unx      194 b- defN 22-Apr-05 15:27 inmanta_module_web-0.3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-05 15:27 inmanta_module_web-0.3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       26 b- defN 22-Apr-05 15:27 inmanta_module_web-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      678 b- defN 22-Apr-05 15:27 inmanta_module_web-0.3.8.dist-info/RECORD
-8 files, 3720 bytes uncompressed, 1796 bytes compressed:  51.7%
+Zip file size: 2741 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx        0 b- defN 22-Apr-21 10:16 inmanta_plugins/web/__init__.py
+-rw-rw-r--  2.0 unx      313 b- defN 22-Apr-21 10:16 inmanta_plugins/web/setup.cfg
+-rw-rw-r--  2.0 unx     2348 b- defN 22-Apr-21 10:15 inmanta_plugins/web/model/_init.cf
+-rw-rw-r--  2.0 unx      194 b- defN 22-Apr-21 10:16 inmanta_module_web-0.3.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Apr-21 10:16 inmanta_module_web-0.3.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 22-Apr-21 10:16 inmanta_module_web-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      602 b- defN 22-Apr-21 10:16 inmanta_module_web-0.3.9.dist-info/RECORD
+7 files, 3565 bytes uncompressed, 1655 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -3,23 +3,20 @@
 
 Filename: inmanta_plugins/web/setup.cfg
 Comment: 
 
 Filename: inmanta_plugins/web/model/_init.cf
 Comment: 
 
-Filename: tests/test_module.py
+Filename: inmanta_module_web-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_web-0.3.8.dist-info/METADATA
+Filename: inmanta_module_web-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_web-0.3.8.dist-info/WHEEL
+Filename: inmanta_module_web-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_web-0.3.8.dist-info/top_level.txt
-Comment: 
-
-Filename: inmanta_module_web-0.3.8.dist-info/RECORD
+Filename: inmanta_module_web-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/web/setup.cfg

```diff
@@ -1,14 +1,17 @@
 [metadata]
 name = inmanta-module-web
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.3.8
+version = 0.3.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-ip
 	inmanta-module-std
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
 
+[options.packages.find]
+include = inmanta_plugins*
+
```

## Comparing `inmanta_module_web-0.3.8.dist-info/RECORD` & `inmanta_module_web-0.3.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
 inmanta_plugins/web/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inmanta_plugins/web/setup.cfg,sha256=sMZbocyjE1I25cKhUY2lOFcybN14aimnEOS-vGRWW50,261
+inmanta_plugins/web/setup.cfg,sha256=XjB5DysB9bjaMTlXm5Jgf1b-9dXrF-JPdyy7W3Rv8rg,313
 inmanta_plugins/web/model/_init.cf,sha256=XDE2GK04YN6kmPaIVPotTZhQWj2mgTP6jxD3z_y9HTc,2348
-tests/test_module.py,sha256=t4LTuygnwnQkxNWiNp8MbE8tCEH_iMMduZzhWNqESMY,121
-inmanta_module_web-0.3.8.dist-info/METADATA,sha256=_Z-keyJyyJClA2_G_Cv9NCbpvBgJfszWeAhx3QNRAIM,194
-inmanta_module_web-0.3.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inmanta_module_web-0.3.8.dist-info/top_level.txt,sha256=kiEAGU2wZ924x342O-45FNMcBEnnI0dzdFENs_pZ7V0,26
-inmanta_module_web-0.3.8.dist-info/RECORD,,
+inmanta_module_web-0.3.9.dist-info/METADATA,sha256=GfK2JPGV5_iPW6pX5Wrd_AVxI2GeqBHZs0pw5aLVQbE,194
+inmanta_module_web-0.3.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+inmanta_module_web-0.3.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_web-0.3.9.dist-info/RECORD,,
```

