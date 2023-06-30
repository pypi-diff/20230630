# Comparing `tmp/watchmen_collector_kernel-16.5.8.tar.gz` & `tmp/watchmen_collector_kernel-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_collector_kernel-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_collector_kernel-16.5.9.tar", max compression
```

## Comparing `watchmen_collector_kernel-16.5.8.tar` & `watchmen_collector_kernel-16.5.9.tar`

### file list

```diff
@@ -1,44 +1,48 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/LICENSE
--rw-r--r--   0        0        0     1197 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/__init__.py
--rw-r--r--   0        0        0      263 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/common/__init__.py
--rw-r--r--   0        0        0      302 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/common/constants.py
--rw-r--r--   0        0        0      697 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/common/settings.py
--rw-r--r--   0        0        0      666 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/__init__.py
--rw-r--r--   0        0        0      495 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/change_data_json.py
--rw-r--r--   0        0        0       99 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/change_data_json_history.py
--rw-r--r--   0        0        0      330 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/change_data_record.py
--rw-r--r--   0        0        0      106 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/change_data_record_history.py
--rw-r--r--   0        0        0      288 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/collector_model_config.py
--rw-r--r--   0        0        0     2907 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/collector_table_config.py
--rw-r--r--   0        0        0      264 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/competitive_lock.py
--rw-r--r--   0        0        0     1942 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/condition.py
--rw-r--r--   0        0        0     1362 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/scheduled_task.py
--rw-r--r--   0        0        0       93 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/scheduled_task_history.py
--rw-r--r--   0        0        0      251 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/trigger_event.py
--rw-r--r--   0        0        0      175 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/trigger_model.py
--rw-r--r--   0        0        0      229 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/trigger_table.py
--rw-r--r--   0        0        0      426 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/__init__.py
--rw-r--r--   0        0        0     2360 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/criteria_builder.py
--rw-r--r--   0        0        0     2873 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/data_capture.py
--rw-r--r--   0        0        0     6560 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/extract_source.py
--rw-r--r--   0        0        0     2452 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/extract_utils.py
--rw-r--r--   0        0        0     1142 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/lock_clean.py
--rw-r--r--   0        0        0      842 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/lock_helper.py
--rw-r--r--   0        0        0     1673 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/task_housekeeping.py
--rw-r--r--   0        0        0     3821 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/task_service.py
--rw-r--r--   0        0        0     6790 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/trigger_collector.py
--rw-r--r--   0        0        0     1173 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1774 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/change_data_json_history_service.py
--rw-r--r--   0        0        0     8464 2023-06-08 03:33:39.183630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/change_data_json_service.py
--rw-r--r--   0        0        0     1845 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/change_data_record_history_service.py
--rw-r--r--   0        0        0     7953 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/change_data_record_service.py
--rw-r--r--   0        0        0     3830 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/collector_model_config_service.py
--rw-r--r--   0        0        0     5882 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/collector_table_config_service.py
--rw-r--r--   0        0        0     2534 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/competitive_lock_service.py
--rw-r--r--   0        0        0     1586 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py
--rw-r--r--   0        0        0     6825 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/scheduled_task_service.py
--rw-r--r--   0        0        0     3099 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/trigger_event_service.py
--rw-r--r--   0        0        0     3219 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/trigger_model_service.py
--rw-r--r--   0        0        0     3779 2023-06-08 03:33:39.187630 watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/trigger_table_service.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 watchmen_collector_kernel-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/LICENSE
+-rw-r--r--   0        0        0     1197 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/__init__.py
+-rw-r--r--   0        0        0      263 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/common/__init__.py
+-rw-r--r--   0        0        0      302 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/common/constants.py
+-rw-r--r--   0        0        0      695 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/common/settings.py
+-rw-r--r--   0        0        0      767 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/change_data_json.py
+-rw-r--r--   0        0        0       99 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/change_data_json_history.py
+-rw-r--r--   0        0        0      352 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/change_data_record.py
+-rw-r--r--   0        0        0      106 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/change_data_record_history.py
+-rw-r--r--   0        0        0      322 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/collector_model_config.py
+-rw-r--r--   0        0        0      250 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/collector_module_config.py
+-rw-r--r--   0        0        0     2935 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/collector_table_config.py
+-rw-r--r--   0        0        0      264 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/competitive_lock.py
+-rw-r--r--   0        0        0     1942 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/condition.py
+-rw-r--r--   0        0        0     1362 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/scheduled_task.py
+-rw-r--r--   0        0        0       93 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/scheduled_task_history.py
+-rw-r--r--   0        0        0      251 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/trigger_event.py
+-rw-r--r--   0        0        0      213 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/trigger_model.py
+-rw-r--r--   0        0        0      193 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/trigger_module.py
+-rw-r--r--   0        0        0      251 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/trigger_table.py
+-rw-r--r--   0        0        0      426 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/__init__.py
+-rw-r--r--   0        0        0     2360 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/criteria_builder.py
+-rw-r--r--   0        0        0     2873 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/data_capture.py
+-rw-r--r--   0        0        0     7622 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/extract_source.py
+-rw-r--r--   0        0        0     2452 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/extract_utils.py
+-rw-r--r--   0        0        0     1142 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/lock_clean.py
+-rw-r--r--   0        0        0      901 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/lock_helper.py
+-rw-r--r--   0        0        0     1673 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/task_housekeeping.py
+-rw-r--r--   0        0        0     3779 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/task_service.py
+-rw-r--r--   0        0        0    10348 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/trigger_collector.py
+-rw-r--r--   0        0        0     1369 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1774 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/change_data_json_history_service.py
+-rw-r--r--   0        0        0     9102 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/change_data_json_service.py
+-rw-r--r--   0        0        0     1845 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/change_data_record_history_service.py
+-rw-r--r--   0        0        0     8621 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/change_data_record_service.py
+-rw-r--r--   0        0        0     4245 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/collector_model_config_service.py
+-rw-r--r--   0        0        0     3711 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/collector_module_config_service.py
+-rw-r--r--   0        0        0     5882 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/collector_table_config_service.py
+-rw-r--r--   0        0        0     2534 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/competitive_lock_service.py
+-rw-r--r--   0        0        0     1586 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py
+-rw-r--r--   0        0        0     6825 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/scheduled_task_service.py
+-rw-r--r--   0        0        0     3099 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/trigger_event_service.py
+-rw-r--r--   0        0        0     3760 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/trigger_model_service.py
+-rw-r--r--   0        0        0     3377 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/trigger_module_service.py
+-rw-r--r--   0        0        0     3876 2023-06-10 16:48:37.867968 watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/trigger_table_service.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 watchmen_collector_kernel-16.5.9/PKG-INFO
```

### Comparing `watchmen_collector_kernel-16.5.8/LICENSE` & `watchmen_collector_kernel-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/pyproject.toml` & `watchmen_collector_kernel-16.5.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-collector-kernel"
-version = "16.5.8"
+version = "16.5.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_collector_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.3"
-watchmen-data-kernel = "16.5.8"
-watchmen-storage-mysql = { version = "16.5.8", optional = true }
-watchmen-storage-oracle = { version = "16.5.8", optional = true }
-watchmen-storage-mongodb = { version = "16.5.8", optional = true }
-watchmen-storage-mssql = { version = "16.5.8", optional = true }
-watchmen-storage-postgresql = { version = "16.5.8", optional = true }
-watchmen-storage-oss = { version = "16.5.8", optional = true }
-watchmen-storage-s3 = { version = "16.5.8", optional = true }
+watchmen-data-kernel = "16.5.9"
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
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/common/settings.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/common/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 logger = getLogger(__name__)
 
 
 class CollectorSettings(BaseSettings):
 	LOCK_CLEAN_INTERVAL: int = 60
 	LOCK_CLEAN_TIMEOUT: int = 3600
-	PARTIAL_SIZE: int = 10000
+	PARTIAL_SIZE: int = 100
 
 	class Config:
 		# secrets_dir = '/var/run'
 		env_file = '.env'
 		env_file_encoding = 'utf-8'
 		case_sensitive = True
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/__init__.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .competitive_lock import CompetitiveLock
 from .scheduled_task import ScheduledTask
 
+from .collector_module_config import CollectorModuleConfig
 from .collector_model_config import CollectorModelConfig
 from .collector_table_config import CollectorTableConfig
 
 from .trigger_event import TriggerEvent
+from .trigger_module import TriggerModule
 from .trigger_model import TriggerModel
 from .trigger_table import TriggerTable
 
 from .change_data_record import ChangeDataRecord
 from .change_data_record_history import ChangeDataRecordHistory
 from .change_data_json import ChangeDataJson
 from .change_data_json_history import ChangeDataJsonHistory
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/collector_table_config.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/collector_table_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 class JsonColumn(Storable, BaseModel):
 	columnName: str = None
 	ignoredPath: List[str] = None
 	needFlatten: bool = None
 	flattenPath: List[str] = None
+	jsonPath: List[str] = None
 
 
 def construct_json_column(json_column: Union[JsonColumn, Dict]) -> Optional[JsonColumn]:
 	if json_column is None:
 		return None
 	elif isinstance(json_column, JsonColumn):
 		return json_column
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/condition.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/condition.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/model/scheduled_task.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/model/scheduled_task.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/criteria_builder.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/criteria_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/data_capture.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/data_capture.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/extract_source.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/extract_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 		topic = Topic(topicId=self.fake_topic_id(config.configId),
 		              name=config.tableName,
 		              dataSourceId=config.dataSourceId,
 		              kind=TopicKind.SYNONYM,
 		              tenantId=self.principal_service.tenantId
 		              )
 		topic_storage = ask_topic_storage(topic, self.principal_service)
-		factors = topic_storage.ask_synonym_factors(config.tableName)
+		factors = topic_storage.ask_reflect_factors(config.tableName)
 		topic.factors = factors
 		now = get_current_time_in_seconds()
 		topic.createdAt = now
 		topic.createdBy = self.principal_service.get_user_id()
 		topic.lastModifiedAt = now
 		topic.lastModifiedBy = self.principal_service.get_user_id()
 		return topic
@@ -153,14 +153,42 @@
 					else:
 						return data_flattened
 
 				return flatten(data_need_flatten, flatten_link_head)
 
 			return ArrayHelper(flatten_path_list).reduce(flatten_path, data_dict)
 
+		def process_json_path(inner_json_path_list: List[str], data_dict: Dict) -> Dict:
+
+			def json_path(data_need_load: Dict, inner_json_path: str) -> Dict:
+				json_path_list = inner_json_path.split(".")
+				json_path_link_head = LinkList().create_tail(json_path_list)
+
+				def load(data_loaded: Dict, node: LinkNode) -> Optional[Dict]:
+					if data_loaded is None:
+						return None
+					if node.item in data_loaded:
+						if node.next is not None:
+							temp = data_loaded[node.item]
+							data_loaded[node.item] = load(temp, node.next)
+							return data_loaded
+						else:
+							if data_loaded[node.item]:
+								try:
+									data_loaded[node.item] = json.loads(data_loaded[node.item])
+									return data_loaded
+								except ValueError:
+									logger.error(f'json node name: {node.item}')
+					else:
+						return data_loaded
+
+				return load(data_need_load, json_path_link_head)
+
+			return ArrayHelper(inner_json_path_list).reduce(json_path, data_dict)
+
 		def change_column_value(row: Dict) -> Dict:
 			for key, value in row.items():
 				for column in json_columns:
 					if key == column.columnName:
 						if value:
 							try:
 								tmp_data = json.loads(value)
@@ -171,14 +199,18 @@
 								tmp_data = process_need_flatten(tmp_data)
 							else:
 								if column.ignoredPath:
 									tmp_data = process_json_ignored(column.ignoredPath, tmp_data)
 
 								if column.flattenPath:
 									tmp_data = process_flatten_path(column.flattenPath, tmp_data)
+
+								if column.jsonPath:
+									tmp_data = process_json_path(column.jsonPath, tmp_data)
+
 							row[key] = tmp_data
 						else:
 							pass
 			return row
 
 		if json_columns:
 			return ArrayHelper(data_).map(lambda row: change_column_value(row)).to_list()
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/extract_utils.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/extract_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/lock_clean.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/lock_clean.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/lock_helper.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/lock_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Union
 
-from sqlalchemy.exc import IntegrityError
+from sqlalchemy.exc import IntegrityError, OperationalError
 
 from watchmen_collector_kernel.model import CompetitiveLock
 from watchmen_collector_kernel.storage.competitive_lock_service import CompetitiveLockService
 from watchmen_utilities import get_current_time_in_seconds
 
 
 def try_lock_nowait(lock_service: CompetitiveLockService, lock: CompetitiveLock) -> bool:
 	try:
 		lock_service.insert_one(lock)
 		return True
+	except OperationalError:
+		return False
 	except IntegrityError:
 		return False
 
 
 def unlock(lock_service: CompetitiveLockService, lock: CompetitiveLock) -> bool:
 	lock_service.delete_by_id(lock.lockId)
 	return True
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/task_housekeeping.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/task_housekeeping.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/service/task_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/service/task_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,16 @@
 	# noinspection PyMethodMayBeStatic
 	def consume_task(self, task: ScheduledTask, executed: Callable[[str, Dict, str], None]) -> ScheduledTask:
 		try:
 			executed(task.topicCode, task.content, task.tenantId)
 			return self.update_task_result(task)
 		except Exception as e:
 			logger.error(e, exc_info=True, stack_info=True)
-			task.isFinished = True
 			task.result = format_exc()
-			return self.scheduled_task_service.update_task(task)
+			return self.update_task_result(task)
 
 	def update_task_result(self, task: ScheduledTask) -> ScheduledTask:
 		self.scheduled_task_service.begin_transaction()
 		try:
 			task.isFinished = True
 			self.scheduled_task_history_service.create(task)
 			self.scheduled_task_service.delete(task.taskId)
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/__init__.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from .competitive_lock_service import get_competitive_lock_service, CompetitiveLockService
 from .scheduled_task_service import get_scheduled_task_service, ScheduledTaskService
 from .scheduled_task_history_service import get_scheduled_task_history_service, ScheduledTaskHistoryService
 
 
+from .collector_module_config_service import get_collector_module_config_service, CollectorModuleConfigService
 from .collector_model_config_service import get_collector_model_config_service, CollectorModelConfigService
 from .collector_table_config_service import get_collector_table_config_service, CollectorTableConfigService
 
 
 from .trigger_event_service import get_trigger_event_service, TriggerEventService
+from .trigger_module_service import get_trigger_module_service, TriggerModuleService
 from .trigger_model_service import get_trigger_model_service, TriggerModelService
 from .trigger_table_service import get_trigger_table_service, TriggerTableService
 
 from .change_data_record_service import get_change_data_record_service, ChangeDataRecordService
 from .change_data_record_history_service import get_change_data_record_history_service, ChangeDataRecordHistoryService
 from .change_data_json_service import get_change_data_json_service, ChangeDataJsonService
 from .change_data_json_history_service import get_change_data_json_history_service, ChangeDataJsonHistoryService
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/change_data_json_history_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/change_data_json_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/change_data_json_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/change_data_json_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 			                                          'content': entity.content,
 			                                          'depend_on': entity.dependOn,
 			                                          'is_posted': entity.isPosted,
 			                                          'result': entity.result,
 			                                          'task_id': entity.taskId,
 			                                          'table_trigger_id': entity.tableTriggerId,
 			                                          'model_trigger_id': entity.modelTriggerId,
+			                                          'module_trigger_id': entity.moduleTriggerId,
 			                                          'event_trigger_id': entity.eventTriggerId
 		                                          })
 
 	def deserialize(self, row: EntityRow) -> ChangeDataJson:
 		# noinspection PyTypeChecker
 		return TupleShaper.deserialize_tenant_based(row,
 		                                            ChangeDataJson(
@@ -44,14 +45,15 @@
 			                                            content=row.get('content'),
 			                                            dependOn=row.get('depend_on'),
 			                                            isPosted=row.get('is_posted'),
 			                                            result=row.get('result'),
 			                                            taskId=row.get('task_id'),
 			                                            tableTriggerId=row.get('table_trigger_id'),
 			                                            modelTriggerId=row.get('model_trigger_id'),
+			                                            moduleTriggerId=row.get('module_trigger_id'),
 			                                            eventTriggerId=row.get('event_trigger_id')
 		                                            ))
 
 
 CHANGE_DATA_JSON_TABLE = 'change_data_json'
 CHANGE_DATA_JSON_ENTITY_SHAPER = ChangeDataJsonShaper()
 
@@ -190,13 +192,26 @@
 					EntityCriteriaExpression(left=ColumnNameLiteral(columnName='model_trigger_id'), right=model_trigger_id),
 					EntityCriteriaExpression(left=ColumnNameLiteral(columnName=IS_POSTED), right=False)
 				]
 			)) == 0
 		finally:
 			self.close_transaction()
 
+	def is_module_finished(self, module_trigger_id: int) -> bool:
+		self.begin_transaction()
+		try:
+			# noinspection PyTypeChecker
+			return self.storage.count(self.get_entity_finder(
+				criteria=[
+					EntityCriteriaExpression(left=ColumnNameLiteral(columnName='module_trigger_id'), right=module_trigger_id),
+					EntityCriteriaExpression(left=ColumnNameLiteral(columnName=IS_POSTED), right=False)
+				]
+			)) == 0
+		finally:
+			self.close_transaction()
+
 
 def get_change_data_json_service(storage: TransactionalStorageSPI,
                                  snowflake_generator: SnowflakeGenerator,
                                  principal_service: PrincipalService
                                  ) -> ChangeDataJsonService:
 	return ChangeDataJsonService(storage, snowflake_generator, principal_service)
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/change_data_record_history_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/change_data_record_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/change_data_record_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/change_data_record_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 			                                          'data_id': entity.dataId,
 			                                          'root_table_name': entity.rootTableName,
 			                                          'root_data_id': entity.rootDataId,
 			                                          'is_merged': entity.isMerged,
 			                                          'result': entity.result,
 			                                          'table_trigger_id': entity.tableTriggerId,
 			                                          'model_trigger_id': entity.modelTriggerId,
+			                                          'module_trigger_id': entity.moduleTriggerId,
 			                                          'event_trigger_id': entity.eventTriggerId
 		                                          })
 
 	def deserialize(self, row: EntityRow) -> ChangeDataRecord:
 		# noinspection PyTypeChecker
 		return TupleShaper.deserialize_tenant_based(row,
 		                                            ChangeDataRecord(
@@ -39,14 +40,15 @@
 			                                            dataId=row.get('data_id'),
 			                                            rootTableName=row.get('root_table_name'),
 			                                            rootDataId=row.get('root_data_id'),
 			                                            isMerged=row.get('is_merged'),
 			                                            result=row.get('result'),
 			                                            tableTriggerId=row.get('table_trigger_id'),
 			                                            modelTriggerId=row.get('model_trigger_id'),
+			                                            moduleTriggerId=row.get('module_trigger_id'),
 			                                            eventTriggerId=row.get('event_trigger_id')
 		                                            ))
 
 
 CHANGE_DATA_RECORD_TABLE = 'change_data_record'
 CHANGE_DATA_RECORD_ENTITY_SHAPER = ChangeDataRecordShaper()
 
@@ -189,13 +191,27 @@
 					                         right=model_trigger_id),
 					EntityCriteriaExpression(left=ColumnNameLiteral(columnName=IS_MERGED), right=False)
 				]
 			)) == 0
 		finally:
 			self.close_transaction()
 
+	def is_module_finished(self, module_trigger_id: int) -> bool:
+		self.begin_transaction()
+		try:
+			# noinspection PyTypeChecker
+			return self.storage.count(self.get_entity_finder(
+				criteria=[
+					EntityCriteriaExpression(left=ColumnNameLiteral(columnName='module_trigger_id'),
+					                         right=module_trigger_id),
+					EntityCriteriaExpression(left=ColumnNameLiteral(columnName=IS_MERGED), right=False)
+				]
+			)) == 0
+		finally:
+			self.close_transaction()
+
 
 def get_change_data_record_service(storage: TransactionalStorageSPI,
                                    snowflake_generator: SnowflakeGenerator,
                                    principal_service: PrincipalService
                                    ) -> ChangeDataRecordService:
 	return ChangeDataRecordService(storage, snowflake_generator, principal_service)
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/collector_model_config_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/collector_model_config_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,29 @@
 
 
 class CollectorModelConfigShaper(EntityShaper):
 	def serialize(self, config: CollectorModelConfig) -> EntityRow:
 		return TupleShaper.serialize_tenant_based(config, {
 			'model_id': config.modelId,
 			'model_name': config.modelName,
+			'module_id': config.moduleId,
 			'depend_on': config.dependOn,
+			'priority': config.priority,
 			'raw_topic_code': config.rawTopicCode,
 			'is_paralleled': config.isParalleled
 		})
 
 	def deserialize(self, row: EntityRow) -> CollectorModelConfig:
 		# noinspection PyTypeChecker
 		return TupleShaper.deserialize_tenant_based(row, CollectorModelConfig(
 			modelId=row.get('model_id'),
 			modelName=row.get('model_name'),
+			moduleId=row.get('module_id'),
 			dependOn=row.get('depend_on'),
+			priority=row.get('priority'),
 			rawTopicCode=row.get('raw_topic_code'),
 			isParalleled=row.get('is_paralleled')
 		))
 
 
 COLLECTOR_MODEL_CONFIG_ENTITY_NAME = 'collector_model_config'
 COLLECTOR_MODEL_CONFIG_ENTITY_SHAPER = CollectorModelConfigShaper()
@@ -95,13 +99,20 @@
 			return self.storage.find_one(self.get_entity_finder(
 				criteria=[
 					EntityCriteriaExpression(left=ColumnNameLiteral(columnName='model_name'), right=model_name)]
 			))
 		finally:
 			self.close_transaction()
 
+	def find_by_module_id(self, module_id: str) -> Optional[List[CollectorModelConfig]]:
+		# noinspection PyTypeChecker
+		return self.storage.find(self.get_entity_finder(
+			criteria=[
+				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='module_id'), right=module_id)]
+		))
+
 
 def get_collector_model_config_service(storage: TransactionalStorageSPI,
                                        snowflake_generator: SnowflakeGenerator,
                                        principal_service: PrincipalService
                                        ) -> CollectorModelConfigService:
 	return CollectorModelConfigService(storage, snowflake_generator, principal_service)
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/collector_table_config_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/collector_table_config_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/competitive_lock_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/competitive_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/scheduled_task_history_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/scheduled_task_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/scheduled_task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/trigger_event_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/trigger_event_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/trigger_model_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/trigger_model_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,24 +12,28 @@
 
 class TriggerModelShaper(EntityShaper):
 
 	def serialize(self, entity: TriggerModel) -> EntityRow:
 		return TupleShaper.serialize_tenant_based(entity, {
 			'model_trigger_id': entity.modelTriggerId,
 			'model_name': entity.modelName,
+			'priority': entity.priority,
 			'is_finished': entity.isFinished,
+			'module_trigger_id': entity.moduleTriggerId,
 			'event_trigger_id': entity.eventTriggerId
 		})
 
 	def deserialize(self, row: EntityRow) -> TriggerModel:
 		# noinspection PyTypeChecker
 		return TupleShaper.deserialize_tenant_based(row, TriggerModel(
 			modelTriggerId=row.get('model_trigger_id'),
 			modelName=row.get('model_name'),
+			priority=row.get('priority'),
 			isFinished=row.get('is_finished'),
+			moduleTriggerId=row.get('module_trigger_id'),
 			eventTriggerId=row.get('event_trigger_id')
 		))
 
 
 TRIGGER_MODEL_TABLE = 'trigger_model'
 TRIGGER_MODEL_ENTITY_SHAPER = TriggerModelShaper()
 
@@ -84,13 +88,24 @@
 				criteria=[
 					EntityCriteriaExpression(left=ColumnNameLiteral(columnName='event_trigger_id'), right=event_trigger_id)
 				]
 			))
 		finally:
 			self.close_transaction()
 
+	def find_by_module_trigger_id(self, module_trigger_id: int) -> List[TriggerModel]:
+		self.begin_transaction()
+		try:
+			# noinspection PyTypeChecker
+			return self.storage.find(self.get_entity_finder(
+				criteria=[
+					EntityCriteriaExpression(left=ColumnNameLiteral(columnName='module_trigger_id'), right=module_trigger_id)
+				]
+			))
+		finally:
+			self.close_transaction()
 
 def get_trigger_model_service(storage: TransactionalStorageSPI,
                               snowflake_generator: SnowflakeGenerator,
                               principal_service: PrincipalService
                               ) -> TriggerModelService:
 	return TriggerModelService(storage, snowflake_generator, principal_service)
```

### Comparing `watchmen_collector_kernel-16.5.8/src/watchmen_collector_kernel/storage/trigger_table_service.py` & `watchmen_collector_kernel-16.5.9/src/watchmen_collector_kernel/storage/trigger_table_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 		return TupleShaper.serialize_tenant_based(entity, {
 			'table_trigger_id': entity.tableTriggerId,
 			'table_name': entity.tableName,
 			'model_name': entity.modelName,
 			'is_extracted': entity.isExtracted,
 			'data_count': entity.dataCount,
 			'model_trigger_id': entity.modelTriggerId,
+			'module_trigger_id': entity.moduleTriggerId,
 			'event_trigger_id': entity.eventTriggerId
 		})
 
 	def deserialize(self, row: EntityRow) -> TriggerTable:
 		# noinspection PyTypeChecker
 		return TupleShaper.deserialize_tenant_based(row, TriggerTable(
 			tableTriggerId=row.get('table_trigger_id'),
 			tableName=row.get('table_name'),
 			modelName=row.get('model_name'),
 			isExtracted=row.get('is_extracted'),
 			dataCount=row.get('data_count'),
 			modelTriggerId=row.get('model_trigger_id'),
+			moduleTriggerId=row.get('module_trigger_id'),
 			eventTriggerId=row.get('event_trigger_id')
 		))
 
 
 TRIGGER_TABLE_TABLE = 'trigger_table'
 TRIGGER_TABLE_ENTITY_SHAPER = TriggerTableShaper()
```

### Comparing `watchmen_collector_kernel-16.5.8/PKG-INFO` & `watchmen_collector_kernel-16.5.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-collector-kernel
-Version: 16.5.8
+Version: 16.5.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
-Requires-Dist: watchmen-data-kernel (==16.5.8)
-Requires-Dist: watchmen-storage-mongodb (==16.5.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.8) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.5.9)
+Requires-Dist: watchmen-storage-mongodb (==16.5.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.9) ; extra == "s3"
```

