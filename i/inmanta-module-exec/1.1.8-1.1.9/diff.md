# Comparing `tmp/inmanta_module_exec-1.1.8-py3-none-any.whl.zip` & `tmp/inmanta_module_exec-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 6601 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     5765 b- defN 22-Apr-05 14:27 inmanta_plugins/exec/__init__.py
--rw-rw-r--  2.0 unx      243 b- defN 22-Apr-05 14:28 inmanta_plugins/exec/setup.cfg
--rw-rw-r--  2.0 unx     3665 b- defN 22-Apr-05 14:27 inmanta_plugins/exec/model/_init.cf
--rw-rw-r--  2.0 unx     8055 b- defN 22-Apr-05 14:27 tests/test_exec.py
--rw-rw-r--  2.0 unx      162 b- defN 22-Apr-05 14:28 inmanta_module_exec-1.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-05 14:28 inmanta_module_exec-1.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       26 b- defN 22-Apr-05 14:28 inmanta_module_exec-1.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      687 b- defN 22-Apr-05 14:28 inmanta_module_exec-1.1.8.dist-info/RECORD
-8 files, 18695 bytes uncompressed, 5389 bytes compressed:  71.2%
+Zip file size: 5146 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     5765 b- defN 22-Apr-21 09:58 inmanta_plugins/exec/__init__.py
+-rw-rw-r--  2.0 unx      295 b- defN 22-Apr-21 09:59 inmanta_plugins/exec/setup.cfg
+-rw-rw-r--  2.0 unx     3665 b- defN 22-Apr-21 09:58 inmanta_plugins/exec/model/_init.cf
+-rw-rw-r--  2.0 unx      162 b- defN 22-Apr-21 09:59 inmanta_module_exec-1.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Apr-21 09:59 inmanta_module_exec-1.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 22-Apr-21 09:59 inmanta_module_exec-1.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      612 b- defN 22-Apr-21 09:59 inmanta_module_exec-1.1.9.dist-info/RECORD
+7 files, 10607 bytes uncompressed, 4046 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -3,23 +3,20 @@
 
 Filename: inmanta_plugins/exec/setup.cfg
 Comment: 
 
 Filename: inmanta_plugins/exec/model/_init.cf
 Comment: 
 
-Filename: tests/test_exec.py
+Filename: inmanta_module_exec-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_exec-1.1.8.dist-info/METADATA
+Filename: inmanta_module_exec-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_exec-1.1.8.dist-info/WHEEL
+Filename: inmanta_module_exec-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_exec-1.1.8.dist-info/top_level.txt
-Comment: 
-
-Filename: inmanta_module_exec-1.1.8.dist-info/RECORD
+Filename: inmanta_module_exec-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/exec/setup.cfg

```diff
@@ -1,13 +1,16 @@
 [metadata]
 name = inmanta-module-exec
 freeze_recursive = False
 freeze_operator = ~=
-version = 1.1.8
+version = 1.1.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-std
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
 
+[options.packages.find]
+include = inmanta_plugins*
+
```

## Comparing `inmanta_module_exec-1.1.8.dist-info/RECORD` & `inmanta_module_exec-1.1.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
 inmanta_plugins/exec/__init__.py,sha256=64QnZJHlxUvsLLosvKutk-WM_wt7xLynWriU8M9POWE,5765
-inmanta_plugins/exec/setup.cfg,sha256=-gFobaj1oS-mIuvXAfwLkCUzgAZ4tJZRIEPMHYIt1F0,243
+inmanta_plugins/exec/setup.cfg,sha256=NHZ81Nq5rYtYwNkwC4eH67lNu-LlyoHEUM8-fhBS1fc,295
 inmanta_plugins/exec/model/_init.cf,sha256=-DhWt2uS_qOeEZNq4bgtMqeSdGsEHOAxse1K2_OuGUY,3665
-tests/test_exec.py,sha256=fMyXL0bWde9qqnoPav-Majr8x4mxgvNKgr-Wa6GiN14,8055
-inmanta_module_exec-1.1.8.dist-info/METADATA,sha256=sJN7ptqQW2gUbnuOXV11-Bdyid0cpxEvyiJA3GI2wGA,162
-inmanta_module_exec-1.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inmanta_module_exec-1.1.8.dist-info/top_level.txt,sha256=kiEAGU2wZ924x342O-45FNMcBEnnI0dzdFENs_pZ7V0,26
-inmanta_module_exec-1.1.8.dist-info/RECORD,,
+inmanta_module_exec-1.1.9.dist-info/METADATA,sha256=cfP3N0oAZORYOSuVdg5mBaGVIfGgkpBJzhml9vMUCb4,162
+inmanta_module_exec-1.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+inmanta_module_exec-1.1.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_exec-1.1.9.dist-info/RECORD,,
```

