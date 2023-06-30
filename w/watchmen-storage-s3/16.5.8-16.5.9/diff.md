# Comparing `tmp/watchmen_storage_s3-16.5.8.tar.gz` & `tmp/watchmen_storage_s3-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_s3-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_storage_s3-16.5.9.tar", max compression
```

## Comparing `watchmen_storage_s3-16.5.8.tar` & `watchmen_storage_s3-16.5.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.235631 watchmen_storage_s3-16.5.8/LICENSE
--rw-r--r--   0        0        0      431 2023-06-08 03:33:39.235631 watchmen_storage_s3-16.5.8/pyproject.toml
--rw-r--r--   0        0        0      180 2023-06-08 03:33:39.235631 watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/__init__.py
--rw-r--r--   0        0        0     1308 2023-06-08 03:33:39.235631 watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/data_source_s3.py
--rw-r--r--   0        0        0     1001 2023-06-08 03:33:39.235631 watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/object_defs_s3.py
--rw-r--r--   0        0        0     3750 2023-06-08 03:33:39.235631 watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/simple_storage_service.py
--rw-r--r--   0        0        0     8836 2023-06-08 03:33:39.235631 watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/storage_s3.py
--rw-r--r--   0        0        0     1818 2023-06-08 03:33:39.235631 watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/storage_s3_configuration.py
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 watchmen_storage_s3-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.915968 watchmen_storage_s3-16.5.9/LICENSE
+-rw-r--r--   0        0        0      431 2023-06-10 16:48:37.915968 watchmen_storage_s3-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-06-10 16:48:37.915968 watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/__init__.py
+-rw-r--r--   0        0        0     1308 2023-06-10 16:48:37.915968 watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/data_source_s3.py
+-rw-r--r--   0        0        0     1001 2023-06-10 16:48:37.915968 watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/object_defs_s3.py
+-rw-r--r--   0        0        0     3750 2023-06-10 16:48:37.915968 watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/simple_storage_service.py
+-rw-r--r--   0        0        0     9253 2023-06-10 16:48:37.915968 watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/storage_s3.py
+-rw-r--r--   0        0        0     1818 2023-06-10 16:48:37.915968 watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/storage_s3_configuration.py
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 watchmen_storage_s3-16.5.9/PKG-INFO
```

### Comparing `watchmen_storage_s3-16.5.8/LICENSE` & `watchmen_storage_s3-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/data_source_s3.py` & `watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/data_source_s3.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/object_defs_s3.py` & `watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/object_defs_s3.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/simple_storage_service.py` & `watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/simple_storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/storage_s3.py` & `watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/storage_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from logging import getLogger
 from typing import Any, Dict, List, Optional
 
 from watchmen_model.admin import Factor, Topic
 from watchmen_model.common import DataPage
 from watchmen_storage import Entity, EntityDeleter, EntityDistinctValuesFinder, EntityFinder, EntityHelper, EntityId, \
 	EntityIdHelper, EntityList, EntityPager, EntityStraightValuesFinder, EntityUpdater, FreeAggregatePager, \
-	FreeAggregator, FreeFinder, FreePager, TopicDataStorageSPI, TransactionalStorageSPI, UnexpectedStorageException
+	FreeAggregator, FreeFinder, FreePager, TopicDataStorageSPI, TransactionalStorageSPI, UnexpectedStorageException, \
+	EntityLimitedFinder
 from .object_defs_s3 import find_directory, register_directory
 from .simple_storage_service import SimpleStorageService
 
 logger = getLogger(__name__)
 
 
 class StorageS3(TransactionalStorageSPI):
@@ -194,14 +195,20 @@
 		And when there is aggregated columns, other columns will be used in group by
 		"""
 		"""
 		not supported by S3
 		"""
 		raise UnexpectedStorageException('Method[find_straight_values] does not support by S3 storage.')
 
+	def find_limited(self, finder: EntityLimitedFinder) -> EntityList:
+		"""
+		not supported by S3
+		"""
+		raise UnexpectedStorageException('Method[find_limited] does not support by S3 storage.')
+
 	def find_all(self, helper: EntityHelper) -> EntityList:
 		"""
 		not supported by S3
 		"""
 		raise UnexpectedStorageException('Method[find_all] does not support by S3 storage.')
 
 	def page(self, pager: EntityPager) -> DataPage:
@@ -221,14 +228,15 @@
 		not supported by S3
 		"""
 		raise UnexpectedStorageException('Method[count] does not support by S3 storage.')
 
 
 # noinspection DuplicatedCode
 class TopicDataStorageS3(StorageS3, TopicDataStorageSPI):
+
 	def register_topic(self, topic: Topic) -> None:
 		register_directory(topic)
 
 	def create_topic_entity(self, topic: Topic) -> None:
 		# create_topic_entity is not required in S3
 		pass
 
@@ -246,14 +254,20 @@
 
 	def ask_synonym_factors(self, table_name: str) -> List[Factor]:
 		"""
 		not supported by S3
 		"""
 		raise UnexpectedStorageException('Method[ask_synonym_factors] does not support by S3 storage.')
 
+	def ask_reflect_factors(self, table_name: str) -> List[Factor]:
+		"""
+		not supported by S3
+		"""
+		raise UnexpectedStorageException('Method[ask_reflect_factors] does not support by S3 storage.')
+
 	# noinspection PyMethodMayBeStatic
 	def is_free_find_supported(self) -> bool:
 		return False
 
 	def free_find(self, finder: FreeFinder) -> List[Dict[str, Any]]:
 		"""
 		not supported by S3
```

### Comparing `watchmen_storage_s3-16.5.8/src/watchmen_storage_s3/storage_s3_configuration.py` & `watchmen_storage_s3-16.5.9/src/watchmen_storage_s3/storage_s3_configuration.py`

 * *Files identical despite different names*

