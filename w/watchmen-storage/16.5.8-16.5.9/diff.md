# Comparing `tmp/watchmen_storage-16.5.8.tar.gz` & `tmp/watchmen_storage-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_storage-16.5.9.tar", max compression
```

## Comparing `watchmen_storage-16.5.8.tar` & `watchmen_storage-16.5.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/LICENSE
--rw-r--r--   0        0        0      442 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/pyproject.toml
--rw-r--r--   0        0        0     2261 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/__init__.py
--rw-r--r--   0        0        0     4917 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/competitive_worker_id_generator.py
--rw-r--r--   0        0        0     5549 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/data_source_helper.py
--rw-r--r--   0        0        0     1853 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/free_storage_types.py
--rw-r--r--   0        0        0      211 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/secrets_manager.py
--rw-r--r--   0        0        0      730 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/secrets_manager_aws.py
--rw-r--r--   0        0        0     1096 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/settings.py
--rw-r--r--   0        0        0     2750 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/snowflake.py
--rw-r--r--   0        0        0      232 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/snowflake_worker_id_generator.py
--rw-r--r--   0        0        0       43 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/sql_analysis/__init__.py
--rw-r--r--   0        0        0    10961 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/sql_analysis/ast_visitor.py
--rw-r--r--   0        0        0     2833 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/sql_analysis/parse_sql.py
--rw-r--r--   0        0        0     1441 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/sql_analysis/topic_generator.py
--rw-r--r--   0        0        0     7259 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/storage_based_worker_id_generator.py
--rw-r--r--   0        0        0      721 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/storage_exception.py
--rw-r--r--   0        0        0     5998 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/storage_spi.py
--rw-r--r--   0        0        0     4717 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/storage_types.py
--rw-r--r--   0        0        0      630 2023-06-08 03:33:39.235631 watchmen_storage-16.5.8/src/watchmen_storage/topic_utils.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 watchmen_storage-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/LICENSE
+-rw-r--r--   0        0        0      442 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2261 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/__init__.py
+-rw-r--r--   0        0        0     4917 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/competitive_worker_id_generator.py
+-rw-r--r--   0        0        0     5549 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/data_source_helper.py
+-rw-r--r--   0        0        0     1853 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/free_storage_types.py
+-rw-r--r--   0        0        0      211 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/secrets_manager.py
+-rw-r--r--   0        0        0      730 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/secrets_manager_aws.py
+-rw-r--r--   0        0        0     1098 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/settings.py
+-rw-r--r--   0        0        0     2750 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/snowflake.py
+-rw-r--r--   0        0        0      232 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/snowflake_worker_id_generator.py
+-rw-r--r--   0        0        0       43 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/sql_analysis/__init__.py
+-rw-r--r--   0        0        0    10961 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/sql_analysis/ast_visitor.py
+-rw-r--r--   0        0        0     2833 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/sql_analysis/parse_sql.py
+-rw-r--r--   0        0        0     1441 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/sql_analysis/topic_generator.py
+-rw-r--r--   0        0        0     7259 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/storage_based_worker_id_generator.py
+-rw-r--r--   0        0        0      721 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/storage_exception.py
+-rw-r--r--   0        0        0     6088 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/storage_spi.py
+-rw-r--r--   0        0        0     4717 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/storage_types.py
+-rw-r--r--   0        0        0      630 2023-06-10 16:48:37.915968 watchmen_storage-16.5.9/src/watchmen_storage/topic_utils.py
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 watchmen_storage-16.5.9/PKG-INFO
```

### Comparing `watchmen_storage-16.5.8/LICENSE` & `watchmen_storage-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/__init__.py` & `watchmen_storage-16.5.9/src/watchmen_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/competitive_worker_id_generator.py` & `watchmen_storage-16.5.9/src/watchmen_storage/competitive_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/data_source_helper.py` & `watchmen_storage-16.5.9/src/watchmen_storage/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/free_storage_types.py` & `watchmen_storage-16.5.9/src/watchmen_storage/free_storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/secrets_manager_aws.py` & `watchmen_storage-16.5.9/src/watchmen_storage/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/settings.py` & `watchmen_storage-16.5.9/src/watchmen_storage/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 		# secrets_dir = '/var/run'
 		env_file = '.env'
 		env_file_encoding = 'utf-8'
 		case_sensitive = True
 
 
 storage_settings = StorageSettings()
-logger.info(f'Storage settings[{storage_settings.dict()}].')
+# logger.info(f'Storage settings[{storage_settings.dict()}].')
 
 
 def ask_sql_analyzer_on() -> bool:
 	return storage_settings.SQL_ANALYZER_ON
 
 def ask_decimal_integral_digits() -> int:
 	return storage_settings.DECIMAL_INTEGRAL_DIGITS
```

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/snowflake.py` & `watchmen_storage-16.5.9/src/watchmen_storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/sql_analysis/ast_visitor.py` & `watchmen_storage-16.5.9/src/watchmen_storage/sql_analysis/ast_visitor.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/sql_analysis/parse_sql.py` & `watchmen_storage-16.5.9/src/watchmen_storage/sql_analysis/parse_sql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/sql_analysis/topic_generator.py` & `watchmen_storage-16.5.9/src/watchmen_storage/sql_analysis/topic_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/storage_based_worker_id_generator.py` & `watchmen_storage-16.5.9/src/watchmen_storage/storage_based_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/storage_exception.py` & `watchmen_storage-16.5.9/src/watchmen_storage/storage_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/storage_spi.py` & `watchmen_storage-16.5.9/src/watchmen_storage/storage_spi.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,18 @@
 	def truncate(self, helper: EntityHelper) -> None:
 		pass
 
 	@abstractmethod
 	def ask_synonym_factors(self, table_name: str) -> List[Factor]:
 		pass
 
+	@abstractmethod
+	def ask_reflect_factors(self, table_name: str) -> List[Factor]:
+		pass
+
 	# noinspection PyMethodMayBeStatic
 	def is_free_find_supported(self) -> bool:
 		return True
 
 	def append_topic_to_trino(self, topic: Topic) -> None:
 		pass
```

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/storage_types.py` & `watchmen_storage-16.5.9/src/watchmen_storage/storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/src/watchmen_storage/topic_utils.py` & `watchmen_storage-16.5.9/src/watchmen_storage/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.8/PKG-INFO` & `watchmen_storage-16.5.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage
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
 Requires-Dist: boto3 (==1.24.45)
-Requires-Dist: watchmen-model (==16.5.8)
+Requires-Dist: watchmen-model (==16.5.9)
```

