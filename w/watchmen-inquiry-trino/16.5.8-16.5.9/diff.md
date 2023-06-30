# Comparing `tmp/watchmen_inquiry_trino-16.5.8.tar.gz` & `tmp/watchmen_inquiry_trino-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_trino-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_inquiry_trino-16.5.9.tar", max compression
```

## Comparing `watchmen_inquiry_trino-16.5.8.tar` & `watchmen_inquiry_trino-16.5.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.199630 watchmen_inquiry_trino-16.5.8/LICENSE
--rw-r--r--   0        0        0      482 2023-06-08 03:33:39.199630 watchmen_inquiry_trino-16.5.8/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-08 03:33:39.199630 watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/__init__.py
--rw-r--r--   0        0        0       46 2023-06-08 03:33:39.199630 watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/exception.py
--rw-r--r--   0        0        0     1169 2023-06-08 03:33:39.199630 watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/settings.py
--rw-r--r--   0        0        0    37618 2023-06-08 03:33:39.199630 watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/trino_storage.py
--rw-r--r--   0        0        0      257 2023-06-08 03:33:39.199630 watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/trino_storage_helper.py
--rw-r--r--   0        0        0     7247 2023-06-08 03:33:39.199630 watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/trino_storage_spi.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 watchmen_inquiry_trino-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.879968 watchmen_inquiry_trino-16.5.9/LICENSE
+-rw-r--r--   0        0        0      482 2023-06-10 16:48:37.879968 watchmen_inquiry_trino-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-10 16:48:37.879968 watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/__init__.py
+-rw-r--r--   0        0        0       46 2023-06-10 16:48:37.879968 watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/exception.py
+-rw-r--r--   0        0        0     1171 2023-06-10 16:48:37.879968 watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/settings.py
+-rw-r--r--   0        0        0    37618 2023-06-10 16:48:37.879968 watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/trino_storage.py
+-rw-r--r--   0        0        0      257 2023-06-10 16:48:37.879968 watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/trino_storage_helper.py
+-rw-r--r--   0        0        0     7446 2023-06-10 16:48:37.879968 watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/trino_storage_spi.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 watchmen_inquiry_trino-16.5.9/PKG-INFO
```

### Comparing `watchmen_inquiry_trino-16.5.8/LICENSE` & `watchmen_inquiry_trino-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/settings.py` & `watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 		# secrets_dir = '/var/run'
 		env_file = '.env'
 		env_file_encoding = 'utf-8'
 		case_sensitive = True
 
 
 settings = KernelSettings()
-logger.info(f'Inquiry trino settings[{settings.dict()}].')
+# logger.info(f'Inquiry trino settings[{settings.dict()}].')
 
 
 def ask_trino_host() -> Tuple[str, int]:
 	return settings.TRINO_HOST, settings.TRINO_PORT
 
 
 def ask_trino_user() -> str:
```

### Comparing `watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/trino_storage.py` & `watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/trino_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.8/src/watchmen_inquiry_trino/trino_storage_spi.py` & `watchmen_inquiry_trino-16.5.9/src/watchmen_inquiry_trino/trino_storage_spi.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 
 	def ask_synonym_factors(self, table_name: str) -> List[Factor]:
 		"""
 		not supported by trino
 		"""
 		raise InquiryTrinoException('Method[ask_synonym_factors] does not support by trino storage.')
 
+	def ask_reflect_factors(self, table_name: str) -> List[Factor]:
+		"""
+		not supported by trino
+		"""
+		raise InquiryTrinoException('Method[ask_reflect_factors] does not support by trino storage.')
+
 	def begin(self) -> None:
 		"""
 		not supported by trino
 		"""
 		raise InquiryTrinoException('Method[begin] does not support by trino storage.')
 
 	def commit_and_close(self) -> None:
```

### Comparing `watchmen_inquiry_trino-16.5.8/PKG-INFO` & `watchmen_inquiry_trino-16.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-trino
-Version: 16.5.8
+Version: 16.5.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: trino (>=0.312.0,<0.313.0)
-Requires-Dist: watchmen-data-kernel (==16.5.8)
+Requires-Dist: watchmen-data-kernel (==16.5.9)
```

