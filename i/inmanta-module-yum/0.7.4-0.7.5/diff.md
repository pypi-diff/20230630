# Comparing `tmp/inmanta_module_yum-0.7.4-py3-none-any.whl.zip` & `tmp/inmanta_module_yum-0.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3956 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     1387 b- defN 23-Apr-04 12:38 inmanta_plugins/yum/__init__.py
--rw-rw-r--  2.0 unx      691 b- defN 23-Apr-04 12:38 inmanta_plugins/yum/setup.cfg
--rw-rw-r--  2.0 unx     1719 b- defN 23-Apr-04 12:38 inmanta_plugins/yum/model/_init.cf
--rw-rw-r--  2.0 unx      475 b- defN 23-Apr-04 12:38 inmanta_plugins/yum/templates/repo.tmpl
--rw-rw-r--  2.0 unx      117 b- defN 23-Apr-04 12:38 inmanta_module_yum-0.7.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 12:38 inmanta_module_yum-0.7.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-04 12:38 inmanta_module_yum-0.7.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      700 b- defN 23-Apr-04 12:38 inmanta_module_yum-0.7.4.dist-info/RECORD
-8 files, 5197 bytes uncompressed, 2716 bytes compressed:  47.7%
+Zip file size: 3954 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     1387 b- defN 23-Jun-30 09:08 inmanta_plugins/yum/__init__.py
+-rw-rw-r--  2.0 unx      691 b- defN 23-Jun-30 09:08 inmanta_plugins/yum/setup.cfg
+-rw-rw-r--  2.0 unx     1719 b- defN 23-Jun-30 09:08 inmanta_plugins/yum/model/_init.cf
+-rw-rw-r--  2.0 unx      475 b- defN 23-Jun-30 09:08 inmanta_plugins/yum/templates/repo.tmpl
+-rw-rw-r--  2.0 unx      117 b- defN 23-Jun-30 09:08 inmanta_module_yum-0.7.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-30 09:08 inmanta_module_yum-0.7.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jun-30 09:08 inmanta_module_yum-0.7.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      700 b- defN 23-Jun-30 09:08 inmanta_module_yum-0.7.5.dist-info/RECORD
+8 files, 5197 bytes uncompressed, 2714 bytes compressed:  47.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: inmanta_plugins/yum/model/_init.cf
 Comment: 
 
 Filename: inmanta_plugins/yum/templates/repo.tmpl
 Comment: 
 
-Filename: inmanta_module_yum-0.7.4.dist-info/METADATA
+Filename: inmanta_module_yum-0.7.5.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_yum-0.7.4.dist-info/WHEEL
+Filename: inmanta_module_yum-0.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_yum-0.7.4.dist-info/top_level.txt
+Filename: inmanta_module_yum-0.7.5.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_yum-0.7.4.dist-info/RECORD
+Filename: inmanta_module_yum-0.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/yum/setup.cfg

```diff
@@ -17,15 +17,15 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-yum
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.7.4
+version = 0.7.5
 license = Apache 2.0
 version_tag = 
 
 [options]
 install_requires = inmanta-module-std
 zip_safe = False
 include_package_data = True
```

## Comparing `inmanta_module_yum-0.7.4.dist-info/RECORD` & `inmanta_module_yum-0.7.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 inmanta_plugins/yum/__init__.py,sha256=YS3YJ6FoXGk-cGnGcbrDxGXoOcJkCD-Z0aveQwvW-pA,1387
-inmanta_plugins/yum/setup.cfg,sha256=QC-YSFalvAMmpkVEONDLRdiP9Dr4BxDkYurzCQ9Dvr0,691
+inmanta_plugins/yum/setup.cfg,sha256=M8jM9edS2KSB6NSxVBCvV52dXQGJhElo9OXmRc6RVP4,691
 inmanta_plugins/yum/model/_init.cf,sha256=BNmzD1zA3TaXbHjtxmkHDAfFnfu0WPyk_I2-VZA70cM,1719
 inmanta_plugins/yum/templates/repo.tmpl,sha256=TLvt43CGKp_VPDvWrBWsjIsioI7Y6ik-_yhQLhKevH0,475
-inmanta_module_yum-0.7.4.dist-info/METADATA,sha256=xNVR8WhEZhc7MPZuorDqpwIIDP3GHhfcDMrcLUOVmCU,117
-inmanta_module_yum-0.7.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-inmanta_module_yum-0.7.4.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_yum-0.7.4.dist-info/RECORD,,
+inmanta_module_yum-0.7.5.dist-info/METADATA,sha256=Zcw80q0WqoQCi_NqluNHsvfP9snDguOqSebFvTj0ySI,117
+inmanta_module_yum-0.7.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+inmanta_module_yum-0.7.5.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_yum-0.7.5.dist-info/RECORD,,
```

