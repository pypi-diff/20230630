# Comparing `tmp/watchmen_inquiry_kernel-16.5.8.tar.gz` & `tmp/watchmen_inquiry_kernel-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_kernel-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_inquiry_kernel-16.5.9.tar", max compression
```

## Comparing `watchmen_inquiry_kernel-16.5.8.tar` & `watchmen_inquiry_kernel-16.5.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/LICENSE
--rw-r--r--   0        0        0     1275 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/__init__.py
--rw-r--r--   0        0        0      112 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/__init__.py
--rw-r--r--   0        0        0       47 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/exception.py
--rw-r--r--   0        0        0      620 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/settings.py
--rw-r--r--   0        0        0      289 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/utils.py
--rw-r--r--   0        0        0       86 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/enum_service.py
--rw-r--r--   0        0        0     1404 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/report_service.py
--rw-r--r--   0        0        0     2358 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/subject_service.py
--rw-r--r--   0        0        0       82 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/__init__.py
--rw-r--r--   0        0        0     2178 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/report_schema.py
--rw-r--r--   0        0        0    12544 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/subject_schema.py
--rw-r--r--   0        0        0      104 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1769 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/report_data_service.py
--rw-r--r--   0        0        0     1496 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/subject_data_service.py
--rw-r--r--   0        0        0    55853 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/subject_storage.py
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/LICENSE
+-rw-r--r--   0        0        0     1275 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/common/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/common/exception.py
+-rw-r--r--   0        0        0      622 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/common/settings.py
+-rw-r--r--   0        0        0      289 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/common/utils.py
+-rw-r--r--   0        0        0       86 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/meta/enum_service.py
+-rw-r--r--   0        0        0     1404 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/meta/report_service.py
+-rw-r--r--   0        0        0     2358 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/meta/subject_service.py
+-rw-r--r--   0        0        0       82 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/schema/__init__.py
+-rw-r--r--   0        0        0     2178 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/schema/report_schema.py
+-rw-r--r--   0        0        0    12544 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/schema/subject_schema.py
+-rw-r--r--   0        0        0      104 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1769 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/storage/report_data_service.py
+-rw-r--r--   0        0        0     1496 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/storage/subject_data_service.py
+-rw-r--r--   0        0        0    55853 2023-06-10 16:48:37.879968 watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/storage/subject_storage.py
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.5.9/PKG-INFO
```

### Comparing `watchmen_inquiry_kernel-16.5.8/LICENSE` & `watchmen_inquiry_kernel-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/pyproject.toml` & `watchmen_inquiry_kernel-16.5.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-inquiry-kernel"
-version = "16.5.8"
+version = "16.5.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-kernel = "16.5.8"
-watchmen-inquiry-trino = { version = "16.5.8", optional = true }
-watchmen-storage-mysql = { version = "16.5.8", optional = true }
-watchmen-storage-oracle = { version = "16.5.8", optional = true }
-watchmen-storage-mongodb = { version = "16.5.8", optional = true }
-watchmen-storage-mssql = { version = "16.5.8", optional = true }
-watchmen-storage-postgresql = { version = "16.5.8", optional = true }
-watchmen-storage-oss = { version = "16.5.8", optional = true }
-watchmen-storage-s3 = { version = "16.5.8", optional = true }
+watchmen-data-kernel = "16.5.9"
+watchmen-inquiry-trino = { version = "16.5.9", optional = true }
+watchmen-storage-mysql = { version = "16.5.9", optional = true }
+watchmen-storage-oracle = { version = "16.5.9", optional = true }
+watchmen-storage-mongodb = { version = "16.5.9", optional = true }
+watchmen-storage-mssql = { version = "16.5.9", optional = true }
+watchmen-storage-postgresql = { version = "16.5.9", optional = true }
+watchmen-storage-oss = { version = "16.5.9", optional = true }
+watchmen-storage-s3 = { version = "16.5.9", optional = true }
 
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/settings.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/common/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 		# secrets_dir = '/var/run'
 		env_file = '.env'
 		env_file_encoding = 'utf-8'
 		case_sensitive = True
 
 
 settings = KernelSettings()
-logger.info(f'Inquiry kernel settings[{settings.dict()}].')
+# logger.info(f'Inquiry kernel settings[{settings.dict()}].')
 
 
 def ask_use_storage_directly() -> bool:
 	return settings.USE_STORAGE_DIRECTLY
 
 
 def ask_trino_enabled() -> bool:
```

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/enum_service.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/meta/enum_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/report_service.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/meta/report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/subject_service.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/meta/subject_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/report_schema.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/schema/report_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/subject_schema.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/schema/subject_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/report_data_service.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/storage/report_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/subject_data_service.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/storage/subject_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/subject_storage.py` & `watchmen_inquiry_kernel-16.5.9/src/watchmen_inquiry_kernel/storage/subject_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.8/PKG-INFO` & `watchmen_inquiry_kernel-16.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-kernel
-Version: 16.5.8
+Version: 16.5.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,16 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-data-kernel (==16.5.8)
-Requires-Dist: watchmen-inquiry-trino (==16.5.8) ; extra == "trino"
-Requires-Dist: watchmen-storage-mongodb (==16.5.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.8) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.5.9)
+Requires-Dist: watchmen-inquiry-trino (==16.5.9) ; extra == "trino"
+Requires-Dist: watchmen-storage-mongodb (==16.5.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.9) ; extra == "s3"
```

