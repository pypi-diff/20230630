# Comparing `tmp/watchmen_lineage-16.5.8.tar.gz` & `tmp/watchmen_lineage-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_lineage-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_lineage-16.5.9.tar", max compression
```

## Comparing `watchmen_lineage-16.5.8.tar` & `watchmen_lineage-16.5.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/LICENSE
--rw-r--r--   0        0        0       46 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/README.md
--rw-r--r--   0        0        0      633 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/__init__.py
--rw-r--r--   0        0        0     1371 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/index.py
--rw-r--r--   0        0        0      548 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/lineage_setting.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/ml/__init__.py
--rw-r--r--   0        0        0      911 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/ml/mapping_similar.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/model/__init__.py
--rw-r--r--   0        0        0      676 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/model/ast.py
--rw-r--r--   0        0        0     5521 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/model/lineage.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/router/__init__.py
--rw-r--r--   0        0        0     1564 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/router/lineage_router.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/__init__.py
--rw-r--r--   0        0        0     4777 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/graphic_builder.py
--rw-r--r--   0        0        0     1179 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/index.py
--rw-r--r--   0        0        0     5696 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/indicator_lineage.py
--rw-r--r--   0        0        0      581 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/loader.py
--rw-r--r--   0        0        0    10390 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/objective_lineage.py
--rw-r--r--   0        0        0     7469 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/pipeline_lineage.py
--rw-r--r--   0        0        0     6522 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/subject_lineage.py
--rw-r--r--   0        0        0     2896 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/topic_lineage.py
--rw-r--r--   0        0        0      291 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/compute_service.py
--rw-r--r--   0        0        0     1027 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/lineage_cache.py
--rw-r--r--   0        0        0    12852 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/lineage_service.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/memory/__init__.py
--rw-r--r--   0        0        0      141 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/memory/memory_compute_service.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/table/__init__.py
--rw-r--r--   0        0        0      140 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/service/table/table_compute_service.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/storage/__init__.py
--rw-r--r--   0        0        0      247 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/storage/lineage_storage.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/utils/__init__.py
--rw-r--r--   0        0        0     7971 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/utils/constant_utils.py
--rw-r--r--   0        0        0     1991 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/utils/id_utils.py
--rw-r--r--   0        0        0     1453 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/utils/size_utils.py
--rw-r--r--   0        0        0    11880 2023-06-08 03:33:39.199630 watchmen_lineage-16.5.8/src/watchmen_lineage/utils/utils.py
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 watchmen_lineage-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/LICENSE
+-rw-r--r--   0        0        0       46 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/README.md
+-rw-r--r--   0        0        0      633 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/__init__.py
+-rw-r--r--   0        0        0     1371 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/index.py
+-rw-r--r--   0        0        0      550 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/lineage_setting.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/ml/__init__.py
+-rw-r--r--   0        0        0      911 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/ml/mapping_similar.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/model/__init__.py
+-rw-r--r--   0        0        0      676 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/model/ast.py
+-rw-r--r--   0        0        0     5521 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/model/lineage.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/router/__init__.py
+-rw-r--r--   0        0        0     1564 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/router/lineage_router.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/__init__.py
+-rw-r--r--   0        0        0     4777 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/graphic_builder.py
+-rw-r--r--   0        0        0     1179 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/index.py
+-rw-r--r--   0        0        0     5696 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/indicator_lineage.py
+-rw-r--r--   0        0        0      581 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/loader.py
+-rw-r--r--   0        0        0    10390 2023-06-10 16:48:37.879968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/objective_lineage.py
+-rw-r--r--   0        0        0     7469 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/pipeline_lineage.py
+-rw-r--r--   0        0        0     6522 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/subject_lineage.py
+-rw-r--r--   0        0        0     2896 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/topic_lineage.py
+-rw-r--r--   0        0        0      291 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/compute_service.py
+-rw-r--r--   0        0        0     1027 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/lineage_cache.py
+-rw-r--r--   0        0        0    12852 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/lineage_service.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/memory/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/memory/memory_compute_service.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/table/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/service/table/table_compute_service.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/storage/__init__.py
+-rw-r--r--   0        0        0      247 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/storage/lineage_storage.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/utils/__init__.py
+-rw-r--r--   0        0        0     7971 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/utils/constant_utils.py
+-rw-r--r--   0        0        0     1991 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/utils/id_utils.py
+-rw-r--r--   0        0        0     1453 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/utils/size_utils.py
+-rw-r--r--   0        0        0    11880 2023-06-10 16:48:37.883968 watchmen_lineage-16.5.9/src/watchmen_lineage/utils/utils.py
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 watchmen_lineage-16.5.9/PKG-INFO
```

### Comparing `watchmen_lineage-16.5.8/LICENSE` & `watchmen_lineage-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/pyproject.toml` & `watchmen_lineage-16.5.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "watchmen-lineage"
-version = "16.5.8"
+version = "16.5.9"
 description = ""
 authors = ["luke0623 <luke0623@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "watchmen_lineage", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-surface = "16.5.8"
-watchmen-pipeline-surface = "16.5.8"
-watchmen-inquiry-surface = "16.5.8"
-watchmen-inquiry-trino = { version = "16.5.8", optional = true }
-watchmen-indicator-surface = "16.5.8"
-watchmen-storage-mysql = { version = "16.5.8", optional = true }
+watchmen-data-surface = "16.5.9"
+watchmen-pipeline-surface = "16.5.9"
+watchmen-inquiry-surface = "16.5.9"
+watchmen-inquiry-trino = { version = "16.5.9", optional = true }
+watchmen-indicator-surface = "16.5.9"
+watchmen-storage-mysql = { version = "16.5.9", optional = true }
 networkx = "^2.8.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/index.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/index.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/lineage_setting.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/lineage_setting.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class LineageSettings(BaseSettings):
 	LINEAGE_FLAG: bool = False
 	IS_CACHE_LINEAGE_GRAPH: bool = False
 	SYSTEM_TOPIC_LINEAGE: bool = False
 
 
 settings = LineageSettings()
-logger.info(f'Inquiry trino settings[{settings.dict()}].')
+# logger.info(f'Inquiry trino settings[{settings.dict()}].')
 
 
 def ask_lineage_flag() -> bool:
 	return settings.LINEAGE_FLAG
 
 
 def ask_is_cache_lineage() -> bool:
```

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/ml/mapping_similar.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/ml/mapping_similar.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/model/ast.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/model/ast.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/model/lineage.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/model/lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/router/lineage_router.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/router/lineage_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/graphic_builder.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/graphic_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/index.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/index.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/indicator_lineage.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/indicator_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/loader.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/loader.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/objective_lineage.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/objective_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/pipeline_lineage.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/pipeline_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/subject_lineage.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/subject_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/builder/topic_lineage.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/builder/topic_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/lineage_cache.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/lineage_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/service/lineage_service.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/service/lineage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/utils/constant_utils.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/utils/constant_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/utils/id_utils.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/utils/id_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/utils/size_utils.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/utils/size_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.8/src/watchmen_lineage/utils/utils.py` & `watchmen_lineage-16.5.9/src/watchmen_lineage/utils/utils.py`

 * *Files identical despite different names*

