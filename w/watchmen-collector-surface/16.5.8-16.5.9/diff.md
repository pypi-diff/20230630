# Comparing `tmp/watchmen_collector_surface-16.5.8.tar.gz` & `tmp/watchmen_collector_surface-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_collector_surface-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_collector_surface-16.5.9.tar", max compression
```

## Comparing `watchmen_collector_surface-16.5.8.tar` & `watchmen_collector_surface-16.5.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/LICENSE
--rw-r--r--   0        0        0     1247 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/pyproject.toml
--rw-r--r--   0        0        0      106 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/__init__.py
--rw-r--r--   0        0        0      188 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/__init__.py
--rw-r--r--   0        0        0     5306 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/monitor_event.py
--rw-r--r--   0        0        0    11506 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/post_json.py
--rw-r--r--   0        0        0    10062 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/record_to_json.py
--rw-r--r--   0        0        0     7551 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/table_extractor.py
--rw-r--r--   0        0        0       65 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/connects/__init__.py
--rw-r--r--   0        0        0     4829 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/connects/s3_connector.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/data/__init__.py
--rw-r--r--   0        0        0     3988 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/data/config_router.py
--rw-r--r--   0        0        0     2034 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/data/task_router.py
--rw-r--r--   0        0        0     1450 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/data/trigger_router.py
--rw-r--r--   0        0        0      258 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/main.py
--rw-r--r--   0        0        0     1716 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/settings.py
--rw-r--r--   0        0        0     1230 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/surface.py
--rw-r--r--   0        0        0       46 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/task/__init__.py
--rw-r--r--   0        0        0     2329 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/task/handler.py
--rw-r--r--   0        0        0     2737 2023-06-08 03:33:39.187630 watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/task/task_listener.py
--rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 watchmen_collector_surface-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/LICENSE
+-rw-r--r--   0        0        0     1247 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/__init__.py
+-rw-r--r--   0        0        0      188 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/__init__.py
+-rw-r--r--   0        0        0     6392 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/monitor_event.py
+-rw-r--r--   0        0        0    13682 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/post_json.py
+-rw-r--r--   0        0        0     9528 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/record_to_json.py
+-rw-r--r--   0        0        0     7675 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/table_extractor.py
+-rw-r--r--   0        0        0       65 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/connects/__init__.py
+-rw-r--r--   0        0        0     4829 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/connects/s3_connector.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/data/__init__.py
+-rw-r--r--   0        0        0     5809 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/data/config_router.py
+-rw-r--r--   0        0        0     2034 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/data/task_router.py
+-rw-r--r--   0        0        0     1450 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/data/trigger_router.py
+-rw-r--r--   0        0        0      258 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/main.py
+-rw-r--r--   0        0        0     1653 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/settings.py
+-rw-r--r--   0        0        0     1230 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/surface.py
+-rw-r--r--   0        0        0       46 2023-06-10 16:48:37.867968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/task/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-10 16:48:37.871968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/task/handler.py
+-rw-r--r--   0        0        0     2498 2023-06-10 16:48:37.871968 watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/task/task_listener.py
+-rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 watchmen_collector_surface-16.5.9/PKG-INFO
```

### Comparing `watchmen_collector_surface-16.5.8/LICENSE` & `watchmen_collector_surface-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.8/pyproject.toml` & `watchmen_collector_surface-16.5.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-collector-surface"
-version = "16.5.8"
+version = "16.5.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_collector_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-collector-kernel = "16.5.8"
-watchmen-pipeline-kernel = "16.5.8"
-watchmen-rest = "16.5.8"
-watchmen-storage-mysql = { version = "16.5.8", optional = true }
-watchmen-storage-oracle = { version = "16.5.8", optional = true }
-watchmen-storage-mongodb = { version = "16.5.8", optional = true }
-watchmen-storage-mssql = { version = "16.5.8", optional = true }
-watchmen-storage-postgresql = { version = "16.5.8", optional = true }
-watchmen-storage-oss = { version = "16.5.8", optional = true }
-watchmen-storage-s3 = { version = "16.5.8", optional = true }
+watchmen-collector-kernel = "16.5.9"
+watchmen-pipeline-kernel = "16.5.9"
+watchmen-rest = "16.5.9"
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

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/monitor_event.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/monitor_event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from logging import getLogger
 from threading import Thread
 from time import sleep
 
 from watchmen_collector_kernel.common import TENANT_ID
-from watchmen_collector_kernel.model import TriggerEvent, TriggerModel, TriggerTable
+from watchmen_collector_kernel.model import TriggerEvent, TriggerModel, TriggerTable, TriggerModule
 from watchmen_collector_kernel.service import try_lock_nowait, unlock
 from watchmen_collector_kernel.service.lock_helper import get_resource_lock
 from watchmen_collector_kernel.storage import get_competitive_lock_service, get_trigger_event_service, \
-	get_trigger_model_service, get_trigger_table_service, get_change_data_record_service, get_change_data_json_service
+	get_trigger_model_service, get_trigger_table_service, get_change_data_record_service, get_change_data_json_service, \
+	get_trigger_module_service
 from watchmen_meta.common import ask_snowflake_generator, ask_super_admin, ask_meta_storage
 from watchmen_utilities import ArrayHelper
 
 logger = getLogger(__name__)
 
 
 def init_event_listener():
@@ -24,14 +25,17 @@
 		self.storage = ask_meta_storage()
 		self.snowflake_generator = ask_snowflake_generator()
 		self.principle_service = ask_super_admin()
 		self.competitive_lock_service = get_competitive_lock_service(self.storage)
 		self.trigger_event_service = get_trigger_event_service(self.storage,
 		                                                       self.snowflake_generator,
 		                                                       self.principle_service)
+		self.trigger_module_service = get_trigger_module_service(self.storage,
+		                                                       self.snowflake_generator,
+		                                                       self.principle_service)
 		self.trigger_model_service = get_trigger_model_service(self.storage,
 		                                                       self.snowflake_generator,
 		                                                       self.principle_service)
 		self.trigger_table_service = get_trigger_table_service(self.storage,
 		                                                       self.snowflake_generator,
 		                                                       self.principle_service)
 		self.data_record_service = get_change_data_record_service(self.storage,
@@ -50,17 +54,40 @@
 				self.event_listener()
 				sleep(60)
 		except Exception as e:
 			logger.error(e, exc_info=True, stack_info=True)
 			sleep(60)
 			self.create_thread()
 
-	def is_all_models_finished(self, event: TriggerEvent) -> bool:
+	def is_all_modules_finished(self, event: TriggerEvent) -> bool:
+		return ArrayHelper(
+			self.trigger_module_service.find_by_event_trigger_id(event.eventTriggerId)).every(
+			lambda trigger_module: self.is_trigger_module_finished(trigger_module)
+		)
+
+	def is_trigger_module_finished(self, trigger_module: TriggerModule) -> bool:
+		if trigger_module.isFinished:
+			return True
+		else:
+			if self.is_all_models_finished(trigger_module):
+				trigger_module.isFinished = True
+				self.trigger_module_service.begin_transaction()
+				try:
+					self.trigger_module_service.update(trigger_module)
+					self.trigger_model_service.commit_transaction()
+				except Exception as e:
+					self.trigger_event_service.rollback_transaction()
+					raise e
+				return True
+			else:
+				return False
+
+	def is_all_models_finished(self, trigger_module: TriggerModule) -> bool:
 		return ArrayHelper(
-			self.trigger_model_service.find_by_event_trigger_id(event.eventTriggerId)
+			self.trigger_model_service.find_by_module_trigger_id(trigger_module.moduleTriggerId)
 		).every(lambda trigger_model: self.is_trigger_model_finished(trigger_model))
 
 	def is_trigger_model_finished(self, trigger_model: TriggerModel) -> bool:
 		if trigger_model.isFinished:
 			return True
 		else:
 			if self.is_all_tables_extracted(trigger_model):
@@ -104,15 +131,15 @@
 				                         unfinished_event.get(TENANT_ID))
 				try:
 					if try_lock_nowait(self.competitive_lock_service, lock):
 						event = self.trigger_event_service.find_event_by_id(unfinished_event.get('event_trigger_id'))
 						if self.is_finished(event):
 							continue
 						else:
-							if self.is_all_models_finished(event) and self.is_all_records_merged(event) and self.is_all_json_posted(event):
+							if self.is_all_modules_finished(event) and self.is_all_records_merged(event) and self.is_all_json_posted(event):
 								event.isFinished = True
 								self.trigger_event_service.begin_transaction()
 								try:
 									self.trigger_event_service.update(event)
 									self.trigger_event_service.commit_transaction()
 								except Exception as e:
 									self.trigger_event_service.rollback_transaction()
```

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/post_json.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/post_json.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from logging import getLogger
 from threading import Thread
 from time import sleep
 from traceback import format_exc
 from typing import List
 
-from watchmen_collector_kernel.common import TENANT_ID, CHANGE_JSON_ID, WAVE
+from watchmen_collector_kernel.common import WAVE
 from watchmen_collector_kernel.model import ChangeDataJson, ScheduledTask, TriggerModel, \
-	CollectorModelConfig, TriggerEvent
+	CollectorModelConfig, TriggerEvent, TriggerModule
 
 from watchmen_collector_kernel.service.lock_helper import get_resource_lock, try_lock_nowait, unlock
 from watchmen_collector_kernel.storage import get_change_data_json_service, get_competitive_lock_service, \
 	get_scheduled_task_service, get_collector_model_config_service, get_trigger_model_service, \
-	get_trigger_event_service, get_change_data_record_service, get_change_data_json_history_service
+	get_trigger_event_service, get_change_data_record_service, get_change_data_json_history_service, \
+	get_collector_module_config_service, get_trigger_module_service
+
 from watchmen_meta.common import ask_meta_storage, ask_snowflake_generator, ask_super_admin
 from watchmen_utilities import ArrayHelper
 
 logger = getLogger(__name__)
 
 
 def init_json_listener():
@@ -37,17 +39,23 @@
 		                                                        self.principle_service)
 		self.change_json_history_service = get_change_data_json_history_service(self.storage,
 		                                                                        self.snowflake_generator,
 		                                                                        self.principle_service)
 		self.scheduled_task_service = get_scheduled_task_service(self.storage,
 		                                                         self.snowflake_generator,
 		                                                         self.principle_service)
+		self.module_config_service = get_collector_module_config_service(self.storage,
+		                                                                 self.snowflake_generator,
+		                                                                 self.principle_service)
 		self.model_config_service = get_collector_model_config_service(self.storage,
 		                                                               self.snowflake_generator,
 		                                                               self.principle_service)
+		self.trigger_module_service = get_trigger_module_service(self.storage,
+		                                                       self.snowflake_generator,
+		                                                       self.principle_service)
 		self.trigger_model_service = get_trigger_model_service(self.storage,
 		                                                       self.snowflake_generator,
 		                                                       self.principle_service)
 		self.trigger_event_service = get_trigger_event_service(self.storage,
 		                                                       self.snowflake_generator,
 		                                                       self.principle_service)
 
@@ -64,66 +72,99 @@
 			self.create_thread()
 
 	def change_data_json_listener(self):
 		unfinished_events = self.trigger_event_service.find_unfinished_events()
 		if len(unfinished_events) == 0:
 			sleep(5)
 		else:
-			ArrayHelper(unfinished_events).each(self.process_models)
+			ArrayHelper(unfinished_events).each(self.process_modules)
+
+	def process_modules(self, unfinished_event: TriggerEvent):
+		trigger_modules = self.trigger_module_service.find_by_event_trigger_id(unfinished_event.get('event_trigger_id'))
 
-	def process_models(self, unfinished_event: TriggerEvent):
-		trigger_models = self.trigger_model_service.find_by_event_trigger_id(unfinished_event.get('event_trigger_id'))
+		def is_higher_priority_module(trigger_module: TriggerModule, current_trigger_module: TriggerModule) -> bool:
+			if trigger_module.priority < current_trigger_module.priority:
+				return True
+			else:
+				return False
+
+		def check_module_priority(trigger_module: TriggerModule) -> bool:
+			if trigger_module.priority == 0:
+				return True
+			else:
+				all_trigger_modules = self.trigger_module_service.find_by_event_trigger_id(trigger_module.eventTriggerId)
+				return ArrayHelper(all_trigger_modules).filter(
+					lambda trigger: is_higher_priority_module(trigger, trigger_module)
+				).every(self.is_trigger_module_finished)
+
+		def process_module(trigger_module: TriggerModule):
+			if check_module_priority(trigger_module):
+				self.process_models(trigger_module)
+			else:
+				logger.debug(f'module {trigger_module.moduleName} priority not fit: {trigger_module.priority}')
+
+		ArrayHelper(trigger_modules).each(process_module)
+
+	def process_models(self, trigger_module: TriggerModule):
+		trigger_models = self.trigger_model_service.find_by_module_trigger_id(trigger_module.moduleTriggerId)
 
 		def process_model(trigger_model: TriggerModel):
 			model_config = self.model_config_service.find_by_name(trigger_model.modelName)
-			if model_config.dependOn is None or self.is_all_dependent_trigger_model_finished(model_config,
-			                                                                                 trigger_model):
-				if model_config.isParalleled or self.is_sequenced_trigger_model_finished(trigger_model):
+			if check_priority(trigger_model):
+				if model_config.isParalleled or self.is_sequenced_trigger_model_record_to_json_finished(trigger_model):
 					self.process_change_data_json(model_config, trigger_model)
 				else:
-					logger.debug(f'model config is paralleled: {model_config.isParalleled}')
+					logger.debug(
+						f'model is not paralleled, and wait for finish record to json: {model_config.isParalleled}')
 			else:
-				logger.debug(f'depend on: {model_config.dependOn}')
+				logger.debug(f'priority not fit: {trigger_model.priority}')
+
+		def check_priority(trigger_model: TriggerModel) -> bool:
+			if trigger_model.priority == 0:
+				return True
+			else:
+				all_trigger_model = self.trigger_model_service.find_by_module_trigger_id(trigger_model.moduleTriggerId)
+				return ArrayHelper(all_trigger_model).filter(
+					lambda trigger: is_higher_priority_model(trigger, trigger_model)
+				).every(self.is_trigger_model_post_json_finished)
+
+		def is_higher_priority_model(trigger_model: TriggerModel, current_trigger_model: TriggerModel) -> bool:
+			if trigger_model.priority < current_trigger_model.priority:
+				return True
+			else:
+				return False
 
 		ArrayHelper(trigger_models).each(process_model)
 
 	def process_change_data_json(self, model_config: CollectorModelConfig, trigger_model: TriggerModel):
-		# not_posted_json = self.change_json_service.find_not_posted_json(trigger_model.modelTriggerId)
 		not_posted_json = self.change_json_service.find_partial_json(trigger_model.modelTriggerId)
-		if len(not_posted_json) == 0:
-			sleep(1)
-		else:
-			for json_record in not_posted_json:
-				lock = get_resource_lock(self.snowflake_generator.next_id(),
-				                         json_record.changeJsonId,
-				                         json_record.tenantId)
-				try:
-					if try_lock_nowait(self.competitive_lock_service, lock):
-						"""
-						change_data_json = self.change_json_service.find_json_by_id(
-							json_record.get(CHANGE_JSON_ID))
-						"""
-						change_data_json = json_record
-						# perhaps have been processed by other dolls, remove to history table.
-						# and also need to consider duplicated json record.
-						if self.change_json_service.is_existed(change_data_json):
-							if not self.is_duplicated(change_data_json):
-								try:
-									if self.can_post(model_config, change_data_json):
-										self.post_json(model_config, change_data_json)
-								except Exception as e:
-									logger.error(e, exc_info=True, stack_info=True)
-									change_data_json.isPosted = True
-									change_data_json.result = format_exc()
-									self.update_result(change_data_json)
-							else:
+		for json_record in not_posted_json:
+			lock = get_resource_lock(self.snowflake_generator.next_id(),
+			                         json_record.changeJsonId,
+			                         json_record.tenantId)
+			try:
+				if try_lock_nowait(self.competitive_lock_service, lock):
+					change_data_json = json_record
+					# perhaps have been processed by other dolls, have remove to history table.
+					# and also need to consider duplicated json record.
+					if self.change_json_service.is_existed(change_data_json):
+						if not self.is_duplicated(change_data_json):
+							try:
+								if self.can_post(model_config, change_data_json):
+									self.post_json(model_config, change_data_json)
+							except Exception as e:
+								logger.error(e, exc_info=True, stack_info=True)
 								change_data_json.isPosted = True
-								self.update_result(change_data_json, True)
-				finally:
-					unlock(self.competitive_lock_service, lock)
+								change_data_json.result = format_exc()
+								self.update_result(change_data_json)
+						else:
+							change_data_json.isPosted = True
+							self.update_result(change_data_json, True)
+			finally:
+				unlock(self.competitive_lock_service, lock)
 
 	def is_duplicated(self, change_data_json: ChangeDataJson) -> bool:
 		existed_json = self.change_json_history_service.find_by_resource_id(change_data_json.resourceId)
 		if existed_json:
 			return True
 		else:
 			return False
@@ -149,31 +190,35 @@
 
 	def is_all_dependent_trigger_model_finished(self, model_config: CollectorModelConfig,
 	                                            trigger_model: TriggerModel) -> bool:
 		if model_config.dependOn:
 			all_trigger_model = self.trigger_model_service.find_by_event_trigger_id(trigger_model.eventTriggerId)
 			return ArrayHelper(all_trigger_model).filter(
 				lambda trigger: self.is_dependent_model(trigger, model_config)
-			).every(self.is_trigger_model_finished)
+			).every(self.is_trigger_model_post_json_finished)
 		else:
 			return True
 
 	# noinspection PyMethodMayBeStatic
 	def is_dependent_model(self, trigger_model: TriggerModel, model_config: CollectorModelConfig) -> bool:
 		if trigger_model.modelName in model_config.dependOn:
 			return True
 		else:
 			return False
 
-	def is_trigger_model_finished(self, trigger_model: TriggerModel) -> bool:
+	def is_trigger_module_finished(self, trigger_module: TriggerModule) -> bool:
+		return trigger_module.isFinished and self.change_record_service.is_module_finished(trigger_module.moduleTriggerId) \
+		       and self.change_json_service.is_module_finished(trigger_module.moduleTriggerId)
+
+	def is_trigger_model_post_json_finished(self, trigger_model: TriggerModel) -> bool:
 		return trigger_model.isFinished and self.change_record_service.is_model_finished(trigger_model.modelTriggerId) \
 		       and self.change_json_service.is_model_finished(trigger_model.modelTriggerId)
 
-	def is_sequenced_trigger_model_finished(self, trigger_model: TriggerModel) -> bool:
-		if self.is_trigger_model_finished(trigger_model):
+	def is_sequenced_trigger_model_record_to_json_finished(self, trigger_model: TriggerModel) -> bool:
+		if trigger_model.isFinished:
 			return self.change_record_service.is_model_finished(trigger_model.modelTriggerId)
 		else:
 			return False
 
 	def can_post(self, model_config: CollectorModelConfig, change_json: ChangeDataJson) -> bool:
 		if model_config.isParalleled:
 			return True
```

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/record_to_json.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/record_to_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from traceback import format_exc
 from typing import Dict, Tuple, Optional, List, Any
 
-from watchmen_collector_kernel.common import CHANGE_RECORD_ID, TENANT_ID, WAVE
+from watchmen_collector_kernel.common import WAVE
 from watchmen_collector_kernel.model import CollectorTableConfig, \
 	ChangeDataRecord, ChangeDataJson
 from watchmen_collector_kernel.model.change_data_json import Dependence
 from watchmen_collector_kernel.model.collector_table_config import Dependence as DependenceConfig
 from watchmen_collector_kernel.service import try_lock_nowait, unlock, \
 	DataCaptureService
 from logging import getLogger
@@ -67,38 +67,26 @@
 			self.create_thread()
 
 	# noinspection PyMethodMayBeStatic
 	def is_merged(self, change_record: ChangeDataRecord) -> bool:
 		return change_record.isMerged
 
 	def change_data_record_listener(self):
-		# unmerged_records = self.change_record_service.find_unmerged_records()
 		unmerged_records = self.change_record_service.find_partial_records()
 		if len(unmerged_records) == 0:
 			sleep(5)
 		else:
 			for unmerged_record in unmerged_records:
-				# Not a complete record, just change_record_id and tenant_id
-				# Can not use for record operation.
-				"""
-				lock = get_resource_lock(self.snowflake_generator.next_id(),
-				                         unmerged_record.get(CHANGE_RECORD_ID),
-				                         unmerged_record.get(TENANT_ID))
-				"""
 				lock = get_resource_lock(self.snowflake_generator.next_id(),
 				                         unmerged_record.changeRecordId,
 				                         unmerged_record.tenantId)
 				try:
 					if try_lock_nowait(self.competitive_lock_service, lock):
-						"""
-						change_data_record = self.change_record_service.find_change_record_by_id(
-							unmerged_record.get(CHANGE_RECORD_ID))
-						"""
 						change_data_record = unmerged_record
-						# perhaps have been processed by other dolls, remove to history table.
+						# perhaps have been processed by other dolls.
 						if self.change_record_service.is_existed(change_data_record):
 							try:
 								self.process_record(change_data_record)
 							except Exception as e:
 								logger.error(e, exc_info=True, stack_info=True)
 								self.update_result(change_data_record, format_exc())
 				finally:
@@ -184,14 +172,15 @@
 			tableName=root_config.tableName,
 			dataId=get_data_id(root_config.primaryKey, root_data),
 			content=content,
 			dependOn=self.get_dependencies(root_config, root_data),
 			isPosted=False,
 			tableTriggerId=change_data_record.tableTriggerId,
 			modelTriggerId=change_data_record.modelTriggerId,
+			moduleTriggerId=change_data_record.moduleTriggerId,
 			eventTriggerId=change_data_record.eventTriggerId,
 			tenantId=change_data_record.tenantId
 		)
 
 	# noinspection PyMethodMayBeStatic
 	def generate_resource_id(self, change_record: ChangeDataRecord) -> str:
 		resource_id_list = []
```

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/cdc/table_extractor.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/cdc/table_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,33 +135,36 @@
 		return self.get_change_data_record(
 			trigger_table.modelName,
 			trigger_table.tableName,
 			data_id,
 			trigger_table.tenantId,
 			trigger_table.tableTriggerId,
 			trigger_table.modelTriggerId,
+			trigger_table.moduleTriggerId,
 			trigger_table.eventTriggerId
 		)
 
 	def get_change_data_record(self,
 	                           model_name: str,
 	                           table_name: str,
 	                           data_id: Dict,
 	                           tenant_id: str,
 	                           table_trigger_id: int,
 	                           model_trigger_id: int,
+	                           module_trigger_id: int,
 	                           event_trigger_id: int) -> ChangeDataRecord:
 		return ChangeDataRecord(
 			changeRecordId=self.snowflake_generator.next_id(),
 			modelName=model_name,
 			tableName=table_name,
 			dataId=data_id,
 			isMerged=False,
 			tableTriggerId=table_trigger_id,
 			modelTriggerId=model_trigger_id,
+			moduleTriggerId=module_trigger_id,
 			eventTriggerId=event_trigger_id,
 			tenantId=tenant_id
 		)
 
 	# noinspection PyMethodMayBeStatic
 	def get_diff(self, source_records, existed_records) -> Any:
 		source_array = np.asarray(
```

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/connects/s3_connector.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/connects/s3_connector.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/data/config_router.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/data/config_router.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Callable, Optional
 
 from fastapi import APIRouter, Depends
 
 from watchmen_auth import PrincipalService
-from watchmen_collector_kernel.model import CollectorTableConfig, CollectorModelConfig
+from watchmen_collector_kernel.model import CollectorTableConfig, CollectorModelConfig, CollectorModuleConfig
 from watchmen_collector_kernel.storage import get_collector_model_config_service, CollectorModelConfigService, \
-	get_collector_table_config_service, CollectorTableConfigService
+	get_collector_table_config_service, CollectorTableConfigService, get_collector_module_config_service, \
+	CollectorModuleConfigService
 from watchmen_meta.common import ask_meta_storage, ask_snowflake_generator
 from watchmen_model.admin import UserRole
 from watchmen_rest import get_any_admin_principal
 from watchmen_rest.util import validate_tenant_id, raise_403
 
 router = APIRouter()
 
@@ -34,15 +35,16 @@
 	def action(config: CollectorTableConfig) -> CollectorTableConfig:
 		if collector_table_config_service.is_storable_id_faked(config.configId):
 			collector_table_config_service.redress_storable_id(config)
 			# noinspection PyTypeChecker
 			config = collector_table_config_service.create_config(config)
 		else:
 			# noinspection PyTypeChecker
-			existing_table_config: Optional[CollectorTableConfig] = collector_table_config_service.find_config_by_id(config.configId)
+			existing_table_config: Optional[CollectorTableConfig] = collector_table_config_service.find_config_by_id(
+				config.configId)
 			if existing_table_config is not None:
 				if existing_table_config.tenantId != config.tenantId:
 					raise_403()
 			# noinspection PyTypeChecker
 			config = collector_table_config_service.update_config(config)
 
 		return config
@@ -82,7 +84,45 @@
 			# noinspection PyTypeChecker
 			config: CollectorModelConfig = \
 				model_config_service.update_model_config(config)
 
 		return config
 
 	return action
+
+
+@router.post('/collector/module/config', tags=[UserRole.ADMIN, UserRole.SUPER_ADMIN],
+             response_model=CollectorModuleConfig)
+async def save_module_config(config: CollectorModuleConfig,
+                             principal_service: PrincipalService = Depends(
+	                             get_any_admin_principal)) -> CollectorModuleConfig:
+	validate_tenant_id(config, principal_service)
+	module_config_service = get_collector_module_config_service(ask_meta_storage(),
+	                                                            ask_snowflake_generator(),
+	                                                            principal_service)
+	action = ask_save_module_config_action(module_config_service, principal_service)
+	return action(config)
+
+
+# noinspection PyUnusedLocal
+def ask_save_module_config_action(
+		module_config_service: CollectorModuleConfigService, principal_service: PrincipalService
+) -> Callable[[CollectorModuleConfig], CollectorModuleConfig]:
+	def action(config: CollectorModuleConfig) -> CollectorModuleConfig:
+		if module_config_service.is_storable_id_faked(config.moduleId):
+			module_config_service.redress_storable_id(config)
+			# noinspection PyTypeChecker
+			config: CollectorModuleConfig = module_config_service.create_module_config(config)
+		else:
+			# noinspection PyTypeChecker
+			existing_module_config: Optional[CollectorModuleConfig] = \
+				module_config_service.find_by_module_id(config.moduleId)
+			if existing_module_config is not None:
+				if existing_module_config.tenantId != config.tenantId:
+					raise_403()
+			# noinspection PyTypeChecker
+			config: CollectorModuleConfig = \
+				module_config_service.update_module_config(config)
+
+		return config
+
+	return action
```

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/data/task_router.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/data/task_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/data/trigger_router.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/data/trigger_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/settings.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 		# secrets_dir = '/var/run'
 		env_file = '.env'
 		env_file_encoding = 'utf-8'
 		case_sensitive = True
 
 
 settings = CollectorSurfaceSettings()
-logger.info(f'Collector surface settings[{settings.dict()}].')
 
 
 def ask_query_based_change_data_capture_enabled() -> bool:
 	return settings.QUERY_BASED_CHANGE_DATA_CAPTURE
 
 
 def ask_task_listener_enabled() -> bool:
```

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/surface.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/surface.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/task/handler.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/task/handler.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.8/src/watchmen_collector_surface/task/task_listener.py` & `watchmen_collector_surface-16.5.9/src/watchmen_collector_surface/task/task_listener.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,25 +41,23 @@
 				self.task_listener()
 		except Exception as e:
 			logger.error(e, exc_info=True, stack_info=True)
 			sleep(60)
 			self.create_thread()
 
 	def task_listener(self) -> None:
-		# unfinished_tasks = self.scheduled_task_service.find_unfinished_tasks()
 		unfinished_tasks = self.scheduled_task_service.find_partial_tasks()
+		if len(unfinished_tasks) == 0:
+			sleep(5)
 		for unfinished_task in unfinished_tasks:
 			lock = get_resource_lock(self.snowflake_generator.next_id(),
 			                         unfinished_task.resourceId,
 			                         unfinished_task.tenantId)
 			try:
 				if try_lock_nowait(self.competitive_lock_service, lock):
-					# noinspection PyUnresolvedReferences
-					# task = self.scheduled_task_service.find_task_by_id(unfinished_task.get('task_id'))
-					# perhaps have been processed by other dolls, remove to history table.
 					if self.scheduled_task_service.is_existed(unfinished_task):
 						if self.task_service.is_dependencies_finished(unfinished_task):
 							self.task_service.consume_task(unfinished_task, pipeline_data)
 							break
 						else:
 							continue
 			finally:
```

### Comparing `watchmen_collector_surface-16.5.8/PKG-INFO` & `watchmen_collector_surface-16.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-collector-surface
-Version: 16.5.8
+Version: 16.5.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,17 +14,17 @@
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
-Requires-Dist: watchmen-collector-kernel (==16.5.8)
-Requires-Dist: watchmen-pipeline-kernel (==16.5.8)
-Requires-Dist: watchmen-rest (==16.5.8)
-Requires-Dist: watchmen-storage-mongodb (==16.5.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.8) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.8) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.8) ; extra == "s3"
+Requires-Dist: watchmen-collector-kernel (==16.5.9)
+Requires-Dist: watchmen-pipeline-kernel (==16.5.9)
+Requires-Dist: watchmen-rest (==16.5.9)
+Requires-Dist: watchmen-storage-mongodb (==16.5.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.9) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.9) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.9) ; extra == "s3"
```

