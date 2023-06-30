# Comparing `tmp/watchmen_storage_mssql-16.5.8.tar.gz` & `tmp/watchmen_storage_mssql-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mssql-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_storage_mssql-16.5.9.tar", max compression
```

## Comparing `watchmen_storage_mssql-16.5.8.tar` & `watchmen_storage_mssql-16.5.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.219631 watchmen_storage_mssql-16.5.8/LICENSE
--rw-r--r--   0        0        0      460 2023-06-08 03:33:39.223631 watchmen_storage_mssql-16.5.8/pyproject.toml
--rw-r--r--   0        0        0      259 2023-06-08 03:33:39.223631 watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/__init__.py
--rw-r--r--   0        0        0     2294 2023-06-08 03:33:39.223631 watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/data_source_mssql.py
--rw-r--r--   0        0        0     2450 2023-06-08 03:33:39.223631 watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/script_builder_mssql.py
--rw-r--r--   0        0        0     7773 2023-06-08 03:33:39.223631 watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/storage_mssql.py
--rw-r--r--   0        0        0     2085 2023-06-08 03:33:39.223631 watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/storage_mssql_configuration.py
--rw-r--r--   0        0        0     7971 2023-06-08 03:33:39.223631 watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/table_creator.py
--rw-r--r--   0        0        0    12465 2023-06-08 03:33:39.223631 watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/where_build.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 watchmen_storage_mssql-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.899968 watchmen_storage_mssql-16.5.9/LICENSE
+-rw-r--r--   0        0        0      460 2023-06-10 16:48:37.903967 watchmen_storage_mssql-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-06-10 16:48:37.903967 watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/__init__.py
+-rw-r--r--   0        0        0     2294 2023-06-10 16:48:37.903967 watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/data_source_mssql.py
+-rw-r--r--   0        0        0     2450 2023-06-10 16:48:37.903967 watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/script_builder_mssql.py
+-rw-r--r--   0        0        0     7773 2023-06-10 16:48:37.903967 watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/storage_mssql.py
+-rw-r--r--   0        0        0     2085 2023-06-10 16:48:37.903967 watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/storage_mssql_configuration.py
+-rw-r--r--   0        0        0     7971 2023-06-10 16:48:37.903967 watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/table_creator.py
+-rw-r--r--   0        0        0    12465 2023-06-10 16:48:37.903967 watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/where_build.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 watchmen_storage_mssql-16.5.9/PKG-INFO
```

### Comparing `watchmen_storage_mssql-16.5.8/LICENSE` & `watchmen_storage_mssql-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/data_source_mssql.py` & `watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/data_source_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/script_builder_mssql.py` & `watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/script_builder_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/storage_mssql.py` & `watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/storage_mssql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/storage_mssql_configuration.py` & `watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/storage_mssql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/table_creator.py` & `watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mssql-16.5.8/src/watchmen_storage_mssql/where_build.py` & `watchmen_storage_mssql-16.5.9/src/watchmen_storage_mssql/where_build.py`

 * *Files identical despite different names*

