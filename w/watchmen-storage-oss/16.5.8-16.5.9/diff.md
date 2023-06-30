# Comparing `tmp/watchmen_storage_oss-16.5.8.tar.gz` & `tmp/watchmen_storage_oss-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_oss-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_storage_oss-16.5.9.tar", max compression
```

## Comparing `watchmen_storage_oss-16.5.8.tar` & `watchmen_storage_oss-16.5.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.231631 watchmen_storage_oss-16.5.8/LICENSE
--rw-r--r--   0        0        0      449 2023-06-08 03:33:39.231631 watchmen_storage_oss-16.5.8/pyproject.toml
--rw-r--r--   0        0        0      112 2023-06-08 03:33:39.231631 watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-08 03:33:39.231631 watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/data_source_oss.py
--rw-r--r--   0        0        0      495 2023-06-08 03:33:39.231631 watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/object_defs_oss.py
--rw-r--r--   0        0        0     1657 2023-06-08 03:33:39.231631 watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/object_storage_service.py
--rw-r--r--   0        0        0     8903 2023-06-08 03:33:39.231631 watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/storage_oss.py
--rw-r--r--   0        0        0     1836 2023-06-08 03:33:39.231631 watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/storage_oss_configuration.py
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.911968 watchmen_storage_oss-16.5.9/LICENSE
+-rw-r--r--   0        0        0      449 2023-06-10 16:48:37.911968 watchmen_storage_oss-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-06-10 16:48:37.911968 watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-10 16:48:37.911968 watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/data_source_oss.py
+-rw-r--r--   0        0        0      495 2023-06-10 16:48:37.911968 watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/object_defs_oss.py
+-rw-r--r--   0        0        0     1657 2023-06-10 16:48:37.911968 watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/object_storage_service.py
+-rw-r--r--   0        0        0     9324 2023-06-10 16:48:37.911968 watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/storage_oss.py
+-rw-r--r--   0        0        0     1836 2023-06-10 16:48:37.911968 watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/storage_oss_configuration.py
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.5.9/PKG-INFO
```

### Comparing `watchmen_storage_oss-16.5.8/LICENSE` & `watchmen_storage_oss-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/data_source_oss.py` & `watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/data_source_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/object_storage_service.py` & `watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/object_storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/storage_oss.py` & `watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/storage_oss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from logging import getLogger
 from typing import Any, Dict, List, Optional
 
 from watchmen_model.admin import Factor, Topic
 from watchmen_model.common import DataPage
 from watchmen_storage import Entity, EntityDeleter, EntityDistinctValuesFinder, EntityFinder, EntityHelper, EntityId, \
 	EntityIdHelper, EntityList, EntityPager, EntityStraightValuesFinder, EntityUpdater, FreeAggregatePager, \
-	FreeAggregator, FreeFinder, FreePager, TopicDataStorageSPI, TransactionalStorageSPI, UnexpectedStorageException
+	FreeAggregator, FreeFinder, FreePager, TopicDataStorageSPI, TransactionalStorageSPI, UnexpectedStorageException, \
+	EntityLimitedFinder
 from .object_defs_oss import find_directory, register_directory
 from .object_storage_service import ObjectStorageService
 
 logger = getLogger(__name__)
 
 
 class StorageOss(TransactionalStorageSPI):
+
 	def __init__(self, oss_client: ObjectStorageService):
 		self.oss_client = oss_client
 
 	def begin(self) -> None:
 		# begin is not required in oss
 		pass
 
@@ -194,14 +196,20 @@
 		And when there is aggregated columns, other columns will be used in group by
 		"""
 		"""
 		not supported by oss
 		"""
 		raise UnexpectedStorageException('Method[find_straight_values] does not support by oss storage.')
 
+	def find_limited(self, finder: EntityLimitedFinder) -> EntityList:
+		"""
+		not supported by oss
+		"""
+		raise UnexpectedStorageException('Method[find_limited] does not support by oss storage.')
+
 	def find_all(self, helper: EntityHelper) -> EntityList:
 		"""
 		not supported by oss
 		"""
 		raise UnexpectedStorageException('Method[find_all] does not support by oss storage.')
 
 	def page(self, pager: EntityPager) -> DataPage:
@@ -246,14 +254,20 @@
 
 	def ask_synonym_factors(self, table_name: str) -> List[Factor]:
 		"""
 		not supported by oss
 		"""
 		raise UnexpectedStorageException('Method[ask_synonym_factors] does not support by oss storage.')
 
+	def ask_reflect_factors(self, table_name: str) -> List[Factor]:
+		"""
+		not supported by oss
+		"""
+		raise UnexpectedStorageException('Method[ask_reflect_factors] does not support by oss storage.')
+
 	# noinspection PyMethodMayBeStatic
 	def is_free_find_supported(self) -> bool:
 		return False
 
 	def free_find(self, finder: FreeFinder) -> List[Dict[str, Any]]:
 		"""
 		not supported by oss
```

### Comparing `watchmen_storage_oss-16.5.8/src/watchmen_storage_oss/storage_oss_configuration.py` & `watchmen_storage_oss-16.5.9/src/watchmen_storage_oss/storage_oss_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.8/PKG-INFO` & `watchmen_storage_oss-16.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-oss
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
 Requires-Dist: oss2 (==2.15.0)
-Requires-Dist: watchmen-storage (==16.5.8)
+Requires-Dist: watchmen-storage (==16.5.9)
```

