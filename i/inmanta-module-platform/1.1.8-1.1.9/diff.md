# Comparing `tmp/inmanta_module_platform-1.1.8-py3-none-any.whl.zip` & `tmp/inmanta_module_platform-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4656 bytes, number of entries: 8
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-02 07:17 inmanta_plugins/platform/__init__.py
--rw-rw-r--  2.0 unx      701 b- defN 23-Feb-02 07:17 inmanta_plugins/platform/setup.cfg
--rw-rw-r--  2.0 unx     1984 b- defN 23-Feb-02 07:17 inmanta_plugins/platform/model/_init.cf
--rw-rw-r--  2.0 unx     4338 b- defN 23-Feb-02 07:17 inmanta_plugins/platform/templates/user_data.j2
--rw-rw-r--  2.0 unx      130 b- defN 23-Feb-02 07:17 inmanta_module_platform-1.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-02 07:17 inmanta_module_platform-1.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Feb-02 07:17 inmanta_module_platform-1.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      741 b- defN 23-Feb-02 07:17 inmanta_module_platform-1.1.8.dist-info/RECORD
-8 files, 8002 bytes uncompressed, 3330 bytes compressed:  58.4%
+Zip file size: 4655 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx        0 b- defN 23-Feb-02 14:51 inmanta_plugins/platform/__init__.py
+-rw-rw-r--  2.0 unx      701 b- defN 23-Feb-02 14:51 inmanta_plugins/platform/setup.cfg
+-rw-rw-r--  2.0 unx     1984 b- defN 23-Feb-02 14:51 inmanta_plugins/platform/model/_init.cf
+-rw-rw-r--  2.0 unx     4338 b- defN 23-Feb-02 14:51 inmanta_plugins/platform/templates/user_data.j2
+-rw-rw-r--  2.0 unx      130 b- defN 23-Feb-02 14:51 inmanta_module_platform-1.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Feb-02 14:51 inmanta_module_platform-1.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Feb-02 14:51 inmanta_module_platform-1.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      741 b- defN 23-Feb-02 14:51 inmanta_module_platform-1.1.9.dist-info/RECORD
+8 files, 8002 bytes uncompressed, 3329 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: inmanta_plugins/platform/model/_init.cf
 Comment: 
 
 Filename: inmanta_plugins/platform/templates/user_data.j2
 Comment: 
 
-Filename: inmanta_module_platform-1.1.8.dist-info/METADATA
+Filename: inmanta_module_platform-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_platform-1.1.8.dist-info/WHEEL
+Filename: inmanta_module_platform-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_platform-1.1.8.dist-info/top_level.txt
+Filename: inmanta_module_platform-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_platform-1.1.8.dist-info/RECORD
+Filename: inmanta_module_platform-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/platform/setup.cfg

```diff
@@ -17,15 +17,15 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-platform
 freeze_recursive = False
 freeze_operator = ~=
-version = 1.1.8
+version = 1.1.9
 license = ASL 2.0
 version_tag = 
 
 [options]
 install_requires = inmanta-module-std>=0.21.0
 zip_safe = False
 include_package_data = True
```

## Comparing `inmanta_module_platform-1.1.8.dist-info/RECORD` & `inmanta_module_platform-1.1.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 inmanta_plugins/platform/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inmanta_plugins/platform/setup.cfg,sha256=ymIgaW0yIW2FASFSlaXPq9A-6nATpBkjaRFCnmuYrB8,701
+inmanta_plugins/platform/setup.cfg,sha256=SkCYh0fUAHtEtxiJPssHv_uWyCYlNqyOk5q_YK__XrI,701
 inmanta_plugins/platform/model/_init.cf,sha256=3Cx9J2-t-Ku8EEKCMtF6QMlQcptBnC-RYDrd9tCh36c,1984
 inmanta_plugins/platform/templates/user_data.j2,sha256=p5NaZx14VJOlyjAW8VJoBgtpKvRUYj3bE7n_wtquWvQ,4338
-inmanta_module_platform-1.1.8.dist-info/METADATA,sha256=0ys_QmEsEZtv6SAb452iIzesyWdrHKZXkFccDDeJeTM,130
-inmanta_module_platform-1.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-inmanta_module_platform-1.1.8.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_platform-1.1.8.dist-info/RECORD,,
+inmanta_module_platform-1.1.9.dist-info/METADATA,sha256=BGn0ERj0A2c99vbpjjohhkqrhzG5TVmnpGZxdqMNs_E,130
+inmanta_module_platform-1.1.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+inmanta_module_platform-1.1.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_platform-1.1.9.dist-info/RECORD,,
```

