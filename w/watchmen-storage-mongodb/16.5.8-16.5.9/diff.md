# Comparing `tmp/watchmen_storage_mongodb-16.5.8.tar.gz` & `tmp/watchmen_storage_mongodb-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mongodb-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_storage_mongodb-16.5.9.tar", max compression
```

## Comparing `watchmen_storage_mongodb-16.5.8.tar` & `watchmen_storage_mongodb-16.5.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/LICENSE
--rw-r--r--   0        0        0      460 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/pyproject.toml
--rw-r--r--   0        0        0      210 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/__init__.py
--rw-r--r--   0        0        0      703 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/codes_options.py
--rw-r--r--   0        0        0     1308 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/data_source_mongo.py
--rw-r--r--   0        0        0     2540 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/document_defs_helper.py
--rw-r--r--   0        0        0    17673 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/document_defs_mongo.py
--rw-r--r--   0        0        0     2541 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/document_mongo.py
--rw-r--r--   0        0        0     5220 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/engine_mongo.py
--rw-r--r--   0        0        0      509 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/sort_build.py
--rw-r--r--   0        0        0    21084 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/storage_mongo.py
--rw-r--r--   0        0        0     1899 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/storage_mongo_configuration.py
--rw-r--r--   0        0        0    11657 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/topic_document_generate.py
--rw-r--r--   0        0        0    24666 2023-06-08 03:33:39.219631 watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/where_build.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 watchmen_storage_mongodb-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/LICENSE
+-rw-r--r--   0        0        0      460 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/__init__.py
+-rw-r--r--   0        0        0      703 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/codes_options.py
+-rw-r--r--   0        0        0     1308 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/data_source_mongo.py
+-rw-r--r--   0        0        0     2540 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/document_defs_helper.py
+-rw-r--r--   0        0        0    17673 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/document_defs_mongo.py
+-rw-r--r--   0        0        0     2541 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/document_mongo.py
+-rw-r--r--   0        0        0     5632 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/engine_mongo.py
+-rw-r--r--   0        0        0      509 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/sort_build.py
+-rw-r--r--   0        0        0    21748 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/storage_mongo.py
+-rw-r--r--   0        0        0     1899 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/storage_mongo_configuration.py
+-rw-r--r--   0        0        0    11657 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/topic_document_generate.py
+-rw-r--r--   0        0        0    24666 2023-06-10 16:48:37.899968 watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/where_build.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 watchmen_storage_mongodb-16.5.9/PKG-INFO
```

### Comparing `watchmen_storage_mongodb-16.5.8/LICENSE` & `watchmen_storage_mongodb-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/codes_options.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/codes_options.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/data_source_mongo.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/data_source_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/document_defs_helper.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/document_defs_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/document_defs_mongo.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/document_defs_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/document_mongo.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/document_mongo.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/engine_mongo.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/engine_mongo.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
 	def insert_one(self, document: MongoDocument, data: Dict[str, Any]) -> None:
 		self.collection(document.name).insert_one(data)
 
 	def insert_many(self, document: MongoDocument, data: List[Dict[str, Any]]) -> None:
 		self.collection(document.name).insert_many(data)
 
-	def update_by_id(self, document: MongoDocument, data: Dict[str, Any], object_id: Union[ObjectId, str, int]) -> UpdateResult:
+	def update_by_id(self, document: MongoDocument, data: Dict[str, Any],
+	                 object_id: Union[ObjectId, str, int]) -> UpdateResult:
 		return self.collection(document.name).update_many({'_id': object_id}, {'$set': data})
 
 	def update_many(self, document: MongoDocument, data: Dict[str, Any], criteria: Dict[str, Any]) -> UpdateResult:
 		return self.collection(document.name).update_many(
 			filter={'$expr': criteria},
 			update={'$set': data},
 			upsert=False
@@ -99,14 +100,21 @@
 			if '_id' in item:
 				# noinspection PyProtectedMember
 				item[column_name] = item._id
 				# noinspection PyProtectedMember
 				del item['_id']
 		return results
 
+	def find_limited(self, document: MongoDocument, limit: int,
+	                 criteria: Dict[str, Any], sort: Optional[Dict[str, Any]] = None) -> List[Dict[str, Any]]:
+		if sort is None:
+			return list(self.collection(document.name).find(filter={'$expr': criteria}).limit(limit))
+		else:
+			return list(self.collection(document.name).find(filter={'$expr': criteria}, sort=sort).limit(limit))
+
 	def exists(self, document: MongoDocument, criteria: Dict[str, any]) -> bool:
 		return self.count(document, criteria) != 0
 
 	def count(self, document: MongoDocument, criteria: Dict[str, any]) -> int:
 		if criteria:
 			results = list(self.collection(document.name).aggregate([
 				{'$match': {'$expr': criteria}},
```

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/storage_mongo.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/storage_mongo.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from watchmen_model.admin import Factor, Topic
 from watchmen_model.common import DataPage, Storable
 from watchmen_storage import as_table_name, Entity, EntityColumnAggregateArithmetic, EntityDeleter, \
 	EntityDistinctValuesFinder, EntityFinder, EntityHelper, EntityId, EntityIdHelper, EntityList, \
 	EntityNotFoundException, EntityPager, EntityRow, EntityStraightAggregateColumn, EntityStraightColumn, \
 	EntityStraightValuesFinder, EntityUpdater, FreeAggregatePager, FreeAggregator, FreeFinder, FreePager, \
 	TooManyEntitiesFoundException, TopicDataStorageSPI, TransactionalStorageSPI, UnexpectedStorageException, \
-	UnsupportedStraightColumnException
+	UnsupportedStraightColumnException, EntityLimitedFinder
 from watchmen_utilities import ArrayHelper, is_blank
 from .document_defs_mongo import find_document, register_document
 from .document_mongo import MongoDocument
 from .engine_mongo import MongoConnection, MongoEngine
 from .sort_build import build_sort_for_statement
 from .topic_document_generate import build_to_trino_fields
 from .where_build import build_criteria_for_statement
@@ -291,14 +291,25 @@
 		sort = build_sort_for_statement(finder.sort)
 		results = self.connection.find(document, where, sort)
 		return ArrayHelper(results) \
 			.map(self.remove_object_id) \
 			.map(finder.shaper.deserialize) \
 			.to_list()
 
+	def find_limited(self, finder: EntityLimitedFinder) -> EntityList:
+		document = self.find_document(finder.name)
+		where = build_criteria_for_statement([document], finder.criteria)
+		sort = build_sort_for_statement(finder.sort)
+		limit = finder.limit
+		results = self.connection.find_limited(document, limit, where, sort)
+		return ArrayHelper(results) \
+			.map(self.remove_object_id) \
+			.map(finder.shaper.deserialize) \
+			.to_list()
+
 	def find_distinct_values(self, finder: EntityDistinctValuesFinder) -> EntityList:
 		document = self.find_document(finder.name)
 		where = build_criteria_for_statement([document], finder.criteria)
 		if len(finder.distinctColumnNames) != 1 or not finder.distinctValueOnSingleColumn:
 			def add_column(columns: Dict[str, int], column_name: str) -> Dict[str, int]:
 				columns[column_name] = 1
 				return columns
@@ -528,14 +539,20 @@
 
 	def ask_synonym_factors(self, table_name: str) -> List[Factor]:
 		"""
 		not supported by mongo
 		"""
 		raise UnexpectedStorageException('Method[ask_synonym_factors] does not support by mongo storage.')
 
+	def ask_reflect_factors(self, table_name: str) -> List[Factor]:
+		"""
+		not supported by mongo
+		"""
+		raise UnexpectedStorageException('Method[ask_reflect_factors] does not support by mongo storage.')
+
 	def is_free_find_supported(self) -> bool:
 		return False
 
 	def append_topic_to_trino(self, topic: Topic) -> None:
 		self.connect()
 		self.connection.insert_one(self.find_document('_schema'), {
 			'table': as_table_name(topic),
```

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/storage_mongo_configuration.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/storage_mongo_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/topic_document_generate.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/topic_document_generate.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/src/watchmen_storage_mongodb/where_build.py` & `watchmen_storage_mongodb-16.5.9/src/watchmen_storage_mongodb/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mongodb-16.5.8/PKG-INFO` & `watchmen_storage_mongodb-16.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-mongodb
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
 Requires-Dist: pymongo (>=4.1.0,<5.0.0)
-Requires-Dist: watchmen-storage (==16.5.8)
+Requires-Dist: watchmen-storage (==16.5.9)
```

