# Comparing `tmp/inmanta_module_std-4.1.7-py3-none-any.whl.zip` & `tmp/inmanta_module_std-4.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 21066 bytes, number of entries: 9
--rw-rw-r--  2.0 unx    31585 b- defN 23-Apr-18 10:12 inmanta_plugins/std/__init__.py
--rw-rw-r--  2.0 unx    21719 b- defN 23-Apr-18 10:12 inmanta_plugins/std/resources.py
--rw-rw-r--  2.0 unx      851 b- defN 23-Apr-18 10:12 inmanta_plugins/std/setup.cfg
--rw-rw-r--  2.0 unx    18184 b- defN 23-Apr-18 10:12 inmanta_plugins/std/model/_init.cf
--rw-rw-r--  2.0 unx     1173 b- defN 23-Apr-18 10:12 inmanta_plugins/std/model/testing.cf
--rw-rw-r--  2.0 unx      194 b- defN 23-Apr-18 10:12 inmanta_module_std-4.1.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 10:12 inmanta_module_std-4.1.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-18 10:12 inmanta_module_std-4.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      790 b- defN 23-Apr-18 10:12 inmanta_module_std-4.1.7.dist-info/RECORD
-9 files, 74604 bytes uncompressed, 19692 bytes compressed:  73.6%
+Zip file size: 21063 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx    31585 b- defN 23-Jun-30 09:08 inmanta_plugins/std/__init__.py
+-rw-rw-r--  2.0 unx    21719 b- defN 23-Jun-30 09:08 inmanta_plugins/std/resources.py
+-rw-rw-r--  2.0 unx      851 b- defN 23-Jun-30 09:08 inmanta_plugins/std/setup.cfg
+-rw-rw-r--  2.0 unx    18184 b- defN 23-Jun-30 09:08 inmanta_plugins/std/model/_init.cf
+-rw-rw-r--  2.0 unx     1173 b- defN 23-Jun-30 09:08 inmanta_plugins/std/model/testing.cf
+-rw-rw-r--  2.0 unx      194 b- defN 23-Jun-30 09:08 inmanta_module_std-4.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-30 09:08 inmanta_module_std-4.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jun-30 09:08 inmanta_module_std-4.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-30 09:08 inmanta_module_std-4.1.8.dist-info/RECORD
+9 files, 74604 bytes uncompressed, 19689 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: inmanta_plugins/std/model/_init.cf
 Comment: 
 
 Filename: inmanta_plugins/std/model/testing.cf
 Comment: 
 
-Filename: inmanta_module_std-4.1.7.dist-info/METADATA
+Filename: inmanta_module_std-4.1.8.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_std-4.1.7.dist-info/WHEEL
+Filename: inmanta_module_std-4.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_std-4.1.7.dist-info/top_level.txt
+Filename: inmanta_module_std-4.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_std-4.1.7.dist-info/RECORD
+Filename: inmanta_module_std-4.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/std/setup.cfg

```diff
@@ -23,15 +23,15 @@
 [irt]
 skip_tests = False
 
 [metadata]
 name = inmanta-module-std
 freeze_recursive = False
 freeze_operator = ~=
-version = 4.1.7
+version = 4.1.8
 license = Apache 2.0
 version_tag = 
 
 [options]
 install_requires = Jinja2>=3.1,<4
 	email_validator>=1.3,<3
 	pydantic>=1.10,<2
```

## Comparing `inmanta_module_std-4.1.7.dist-info/RECORD` & `inmanta_module_std-4.1.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 inmanta_plugins/std/__init__.py,sha256=byslmwchNeYKAokblRu2opRdEdJV6_a-5F8SWhh9128,31585
 inmanta_plugins/std/resources.py,sha256=kZJiQcYMgYPJF5S3x8HkOhHCqUjuGQr8pCM4WXBZgR0,21719
-inmanta_plugins/std/setup.cfg,sha256=4UMajwh-mgiea67u92kwamRD8ENlVkfe6Q6CwHEU2TQ,851
+inmanta_plugins/std/setup.cfg,sha256=x-QFcF7Ewg42cxDc1z1FAxB63uRbcniSskcCtMJMknw,851
 inmanta_plugins/std/model/_init.cf,sha256=I1TJT8L5kZC6VB0pOH1OJWLJ0jgk5qg1or202X2jw2Q,18184
 inmanta_plugins/std/model/testing.cf,sha256=hLBbIMQkBVaCycT0sLjCuImKDvIgn_CeV8O-75mRz7g,1173
-inmanta_module_std-4.1.7.dist-info/METADATA,sha256=nG-Aj7Q1D9-kI7aLAQQK_UFIlqURMIzokFGDRipchIw,194
-inmanta_module_std-4.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-inmanta_module_std-4.1.7.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_std-4.1.7.dist-info/RECORD,,
+inmanta_module_std-4.1.8.dist-info/METADATA,sha256=SRB5lnh7O9CgD2V_yo7M_WHWtAso5ZfvLqJcDhXyUtc,194
+inmanta_module_std-4.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+inmanta_module_std-4.1.8.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_std-4.1.8.dist-info/RECORD,,
```

