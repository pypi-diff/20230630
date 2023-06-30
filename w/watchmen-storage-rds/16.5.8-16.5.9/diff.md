# Comparing `tmp/watchmen_storage_rds-16.5.8.tar.gz` & `tmp/watchmen_storage_rds-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_rds-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_storage_rds-16.5.9.tar", max compression
```

## Comparing `watchmen_storage_rds-16.5.8.tar` & `watchmen_storage_rds-16.5.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      455 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/pyproject.toml
--rw-r--r--   0        0        0      643 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/__init__.py
--rw-r--r--   0        0        0      652 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/dbscript_builder.py
--rw-r--r--   0        0        0      518 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/ext_types.py
--rw-r--r--   0        0        0      672 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/settings.py
--rw-r--r--   0        0        0      941 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/sort_build.py
--rw-r--r--   0        0        0    17832 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/storage_rds.py
--rw-r--r--   0        0        0    22728 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/table_defs.py
--rw-r--r--   0        0        0     2249 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/table_defs_helper.py
--rw-r--r--   0        0        0    24063 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/topic_data_storage_rds.py
--rw-r--r--   0        0        0     8191 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/topic_table_generate.py
--rw-r--r--   0        0        0      916 2023-06-08 03:33:39.235631 watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/types.py
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0      455 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0      643 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/__init__.py
+-rw-r--r--   0        0        0      652 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/dbscript_builder.py
+-rw-r--r--   0        0        0      518 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/ext_types.py
+-rw-r--r--   0        0        0      674 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/settings.py
+-rw-r--r--   0        0        0      941 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/sort_build.py
+-rw-r--r--   0        0        0    17832 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/storage_rds.py
+-rw-r--r--   0        0        0    23736 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/table_defs.py
+-rw-r--r--   0        0        0     2249 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/table_defs_helper.py
+-rw-r--r--   0        0        0      906 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/table_reflector.py
+-rw-r--r--   0        0        0    24367 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/topic_data_storage_rds.py
+-rw-r--r--   0        0        0     8191 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/topic_table_generate.py
+-rw-r--r--   0        0        0      916 2023-06-10 16:48:37.915968 watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/types.py
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.5.9/PKG-INFO
```

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/__init__.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/dbscript_builder.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/dbscript_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/ext_types.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/ext_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/settings.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class StorageRDSSettings(BaseSettings):
 	DETECT_RDS_CONNECTION_LEAK: bool = False
 	PRINT_RDS_CONNECTION_LEAK_INTERVAL: int = 300
 	RDS_CONNECTION_LEAK_TIME_IN_SECONDS: int = 1
 
 
 settings = StorageRDSSettings()
-logger.info(f'Pipeline surface settings[{settings.dict()}].')
+# logger.info(f'Pipeline surface settings[{settings.dict()}].')
 
 
 def ask_detect_connection_leak_enabled() -> bool:
 	return settings.DETECT_RDS_CONNECTION_LEAK
 
 
 def ask_print_connection_leak_interval() -> int:
```

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/sort_build.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/sort_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/storage_rds.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/storage_rds.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/table_defs.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/table_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -319,19 +319,27 @@
 	create_str('topic_code', 50), create_json('content'),
 	create_str('model_name', 20), create_str('object_id', 100),
 	create_json('depend_on'), create_json('parent_task_id'),
 	create_int('is_finished', False), create_json('result'),
 	create_tenant_id(),
 	*create_tuple_audit_columns()
 )
+table_collector_module_config = Table(
+	'collector_module_config', meta_data,
+	create_pk('module_id'), create_str('module_name', 50),
+	create_int('priority', False), create_int('priority', False),
+	create_tenant_id(), *create_tuple_audit_columns(),
+	create_optimistic_lock()
+)
 table_collector_model_config = Table(
 	'collector_model_config', meta_data,
 	create_pk('model_id'), create_str('model_name', 50),
+	create_str('module_id', 50),
 	create_json('depend_on'), create_str('raw_topic_code', 50),
-	create_int('is_paralleled'),
+	create_int('is_paralleled'), create_int('priority', False),
 	create_tenant_id(), *create_tuple_audit_columns(),
 	create_optimistic_lock()
 )
 table_collector_table_config = Table(
 	'collector_table_config', meta_data,
 	create_pk('config_id'), create_str('name', 50),
 	create_str('table_name', 50), create_json('primary_key'), create_str('object_key', 50),
@@ -346,65 +354,79 @@
 table_trigger_event = Table(
 	'trigger_event', meta_data,
 	create_pk('event_trigger_id', Integer),
 	create_date('start_time'), create_date('end_time'),
 	create_int('is_finished', False),
 	create_tenant_id(), *create_tuple_audit_columns()
 )
+table_trigger_module = Table(
+	'trigger_module', meta_data,
+	create_pk('module_trigger_id', Integer),
+	create_str('module_name', 50), create_int('priority', False),
+	create_int('is_finished', False),
+	create_int('event_trigger_id', False),
+	create_tenant_id(), *create_tuple_audit_columns()
+)
 table_trigger_model = Table(
 	'trigger_model', meta_data,
 	create_pk('model_trigger_id', Integer),
-	create_str('model_name', 50),
+	create_str('model_name', 50), create_int('priority', False),
 	create_int('is_finished', False),
+	create_int('module_trigger_id', False),
 	create_int('event_trigger_id', False),
 	create_tenant_id(), *create_tuple_audit_columns()
 )
 table_trigger_table = Table(
 	'trigger_table', meta_data,
 	create_pk('table_trigger_id', Integer), create_str('table_name', 50),
 	create_str('model_name', 50), create_int('data_count'),
 	create_int('is_extracted', False),
 	create_int('model_trigger_id', False),
+	create_int('module_trigger_id', False),
 	create_int('event_trigger_id', False),
 	create_tenant_id(), *create_tuple_audit_columns()
 )
 table_change_data_record = Table(
 	'change_data_record', meta_data,
 	create_pk('change_record_id', Integer), create_str('model_name', 50), create_str('table_name', 50),
 	create_json('data_id'), create_str('root_table_name', 50), create_json('root_data_id'),
 	create_int('is_merged', False), create_json('result'),
-	create_int('table_trigger_id', False), create_int('model_trigger_id', False), create_int('event_trigger_id', False),
+	create_int('table_trigger_id', False), create_int('model_trigger_id', False),
+	create_int('module_trigger_id', False), create_int('event_trigger_id', False),
 	create_tenant_id(), *create_tuple_audit_columns()
 )
 table_change_data_record_history = Table(
 	'change_data_record_history', meta_data,
 	create_pk('change_record_id', Integer), create_str('model_name', 50), create_str('table_name', 50),
 	create_json('data_id'), create_str('root_table_name', 50), create_json('root_data_id'),
 	create_int('is_merged', False), create_json('result'),
-	create_int('table_trigger_id', False), create_int('model_trigger_id', False), create_int('event_trigger_id', False),
+	create_int('table_trigger_id', False), create_int('model_trigger_id', False),
+	create_int('module_trigger_id', False), create_int('event_trigger_id', False),
 	create_tenant_id(), *create_tuple_audit_columns()
 )
 table_change_data_json = Table(
 	'change_data_json', meta_data,
 	create_pk('change_json_id', Integer), create_str('resource_id', 100),
 	create_str('model_name', 50), create_str('object_id', 50),
 	create_str('table_name', 50), create_json('data_id'),
 	create_json('content'), create_json('depend_on'), create_int('is_posted', False), create_int('task_id', True),
 	create_json('result'),
-	create_int('table_trigger_id', False), create_int('model_trigger_id', False), create_int('event_trigger_id', False),
+	create_int('table_trigger_id', False), create_int('model_trigger_id', False),
+	create_int('module_trigger_id', False), create_int('event_trigger_id', False),
 	create_tenant_id(), *create_tuple_audit_columns()
 )
 table_change_data_json_history = Table(
 	'change_data_json_history', meta_data,
 	create_pk('change_json_id', Integer), create_str('resource_id', 100),
 	create_str('model_name', 50), create_str('object_id', 50),
 	create_str('table_name', 50), create_json('data_id'),
 	create_json('content'), create_json('depend_on'), create_int('is_posted', False), create_int('task_id', True),
 	create_json('result'),
-	create_int('table_trigger_id', False), create_int('model_trigger_id', False), create_int('event_trigger_id', False),
+	create_int('table_trigger_id', False), create_int('model_trigger_id', False),
+	create_int('module_trigger_id', False), create_int('event_trigger_id', False),
 	create_tenant_id(), *create_tuple_audit_columns()
 )
 table_operations = Table(
 	'operations', meta_data,
 	create_pk('record_id'), create_str('operation_type', 20),
 	create_str('tuple_type', 20), create_str('tuple_key', 20),
 	create_str('tuple_id', 50), create_json('content'), create_str('version_num', 50),
@@ -500,17 +522,19 @@
 	'operations': table_operations,
 	'package_versions': table_package_versions,
 	# webhook
 	'subscription_event_locks': table_subscription_event_locks,
 	'subscription_events': table_subscription_event,
 	'notification_definitions': table_notification_definition,
 	# collector
+	'collector_module_config': table_collector_module_config,
 	'collector_model_config': table_collector_model_config,
 	'collector_table_config': table_collector_table_config,
 	'trigger_event': table_trigger_event,
+	'trigger_module': table_trigger_module,
 	'trigger_model': table_trigger_model,
 	'trigger_table': table_trigger_table,
 	'change_data_record': table_change_data_record,
 	'change_data_record_history': table_change_data_record_history,
 	'change_data_json': table_change_data_json,
 	'change_data_json_history': table_change_data_json_history
 }
```

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/table_defs_helper.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/table_defs_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/topic_data_storage_rds.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/topic_data_storage_rds.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from watchmen_storage.settings import ask_sql_analyzer_on
 from watchmen_storage.sql_analysis.ast_visitor import QueryPerformance
 from watchmen_storage.sql_analysis.parse_sql import SqlParser
 from watchmen_utilities import ArrayHelper, is_not_blank
 from .storage_rds import StorageRDS
 from .table_defs import register_table
 from .types import SQLAlchemyStatement
+from .table_reflector import ask_columns
 
 logger = getLogger(__name__)
 
 
 class TopicDataStorageRDS(StorageRDS, TopicDataStorageSPI):
 	# noinspection PyMethodMayBeStatic
 	def register_topic(self, topic: Topic) -> None:
@@ -123,14 +124,21 @@
 			self.connect()
 			factors = self.ask_synonym_columns(table_name)
 			self.build_index_group_by_synonym(table_name, factors)
 			return factors
 		finally:
 			self.close()
 
+	def ask_reflect_factors(self, table_name: str) -> List[Factor]:
+		columns = ask_columns(table_name, self.engine)
+		factors = ArrayHelper(columns) \
+			.map_with_index(lambda x, index: self.schema_column_to_factor(x, index + 1)) \
+			.to_list()
+		return factors
+
 	# noinspection PyMethodMayBeStatic
 	def build_single_on(self, join: FreeJoin, primary_table: Table, secondary_table: Table) -> Any:
 		primary_column = primary_table.c[join.primary.columnName]
 		secondary_column = secondary_table.c[join.secondary.columnName]
 		return primary_column == secondary_column
 
 	def try_to_join(self, groups: Dict[TopicId, List[FreeJoin]], tables: List[Table], built=None) -> Join:
```

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/topic_table_generate.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/topic_table_generate.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.8/src/watchmen_storage_rds/types.py` & `watchmen_storage_rds-16.5.9/src/watchmen_storage_rds/types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.8/PKG-INFO` & `watchmen_storage_rds-16.5.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-rds
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
 Requires-Dist: SQLAlchemy (==1.4.35)
-Requires-Dist: watchmen-storage (==16.5.8)
+Requires-Dist: watchmen-storage (==16.5.9)
```

