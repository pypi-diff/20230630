# Comparing `tmp/evadb-0.3.0.tar.gz` & `tmp/evadb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evadb-0.3.0.tar", last modified: Tue Jun 27 23:59:46 2023, max compression
+gzip compressed data, was "evadb-0.3.1.tar", last modified: Fri Jun 30 04:21:39 2023, max compression
```

## Comparing `evadb-0.3.0.tar` & `evadb-0.3.1.tar`

### file list

```diff
@@ -1,472 +1,473 @@
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.689784 evadb-0.3.0/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11357 2023-06-08 04:02:21.000000 evadb-0.3.0/LICENSE.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13108 2023-06-27 23:59:46.689784 evadb-0.3.0/PKG-INFO
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12298 2023-06-27 00:54:48.000000 evadb-0.3.0/README.md
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.645783 evadb-0.3.0/evadb/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      905 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.645783 evadb-0.3.0/evadb/binder/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/binder/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8749 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/binder/binder_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14313 2023-06-27 00:54:47.000000 evadb-0.3.0/evadb/binder/statement_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7978 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/binder/statement_binder_context.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.649783 evadb-0.3.0/evadb/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19545 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/catalog/catalog_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3373 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/catalog/catalog_type.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10319 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/catalog/catalog_utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.649783 evadb-0.3.0/evadb/catalog/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1503 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/association_models.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4751 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/base_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4551 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/column_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2871 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/index_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2441 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/table_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3022 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/udf_cache_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3101 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/udf_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1804 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/udf_cost_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3923 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/udf_io_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2205 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/udf_metadata_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6789 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/models/utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2126 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/schema_utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.649783 evadb-0.3.0/evadb/catalog/services/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1291 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/base_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3377 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/column_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2970 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/index_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4961 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/table_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3999 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/udf_cache_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3249 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/udf_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3036 2023-06-25 03:38:24.000000 evadb-0.3.0/evadb/catalog/services/udf_cost_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2934 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/udf_io_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2226 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/catalog/services/udf_metadata_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2793 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/catalog/sql_config.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.649783 evadb-0.3.0/evadb/configuration/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      622 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/configuration/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5035 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/configuration/bootstrap_environment.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2508 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/configuration/configuration_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1055 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/configuration/constants.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      884 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/constants.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1964 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/database.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      570 2023-06-26 03:28:32.000000 evadb-0.3.0/evadb/evadb.yml
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2018 2023-06-08 22:16:07.000000 evadb-0.3.0/evadb/evadb_cmd_client.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2023-06-08 22:16:07.000000 evadb-0.3.0/evadb/evadb_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.653783 evadb-0.3.0/evadb/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      617 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3803 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/abstract_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2324 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/apply_and_merge_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2034 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/executor/create_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5099 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/create_index_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7395 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/executor/create_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4732 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/executor/delete_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4959 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/executor/drop_object_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3635 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/executor/exchange_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3025 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/execution_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5513 2023-06-25 22:35:38.000000 evadb-0.3.0/evadb/executor/executor_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1596 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/explain_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2005 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/function_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1897 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/groupby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1944 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/hash_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2243 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/executor/insert_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1688 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/join_build_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1843 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/lateral_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1655 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/limit_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3080 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/executor/load_csv_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1742 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6141 2023-06-26 03:15:21.000000 evadb-0.3.0/evadb/executor/load_multimedia_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/nested_loop_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4263 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/orderby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8299 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/executor/plan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1716 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/pp_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1367 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/predicate_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1362 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/project_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2443 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/executor/ray_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1267 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/rename_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1485 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/sample_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1918 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/seq_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1846 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/show_info_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2646 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/executor/storage_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1336 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/union_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4395 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/executor/vector_index_scan_executor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.653783 evadb-0.3.0/evadb/expression/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      619 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/expression/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5561 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/expression/abstract_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3979 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/expression/aggregation_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1624 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/expression/arithmetic_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4357 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/expression/comparison_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2550 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/expression/constant_value_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10445 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/expression/expression_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10064 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/expression/function_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3059 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/expression/logical_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4330 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/expression/tuple_value_expression.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.653783 evadb-0.3.0/evadb/interfaces/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/interfaces/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.657783 evadb-0.3.0/evadb/interfaces/relational/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/interfaces/relational/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19500 2023-06-26 14:59:01.000000 evadb-0.3.0/evadb/interfaces/relational/db.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7755 2023-06-22 16:24:39.000000 evadb-0.3.0/evadb/interfaces/relational/relation.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4596 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/interfaces/relational/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.657783 evadb-0.3.0/evadb/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      637 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/models/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.657783 evadb-0.3.0/evadb/models/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/models/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1336 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/models/catalog/frame_info.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      859 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/models/catalog/properties.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.657783 evadb-0.3.0/evadb/models/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/models/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1971 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/models/server/response.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.657783 evadb-0.3.0/evadb/models/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/models/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15331 2023-06-09 18:53:37.000000 evadb-0.3.0/evadb/models/storage/batch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.657783 evadb-0.3.0/evadb/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      624 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3269 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2145 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/cost_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3460 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/group.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2677 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/group_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4347 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/memo.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    35384 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/optimizer/operators.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4040 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/optimizer_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      986 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/optimizer_task_stack.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12600 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/optimizer_tasks.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11286 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/optimizer/optimizer_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4184 2023-06-26 14:59:01.000000 evadb-0.3.0/evadb/optimizer/plan_generator.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1171 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/property.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.657783 evadb-0.3.0/evadb/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1023 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/optimizer/rules/pattern.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    48746 2023-06-27 00:54:47.000000 evadb-0.3.0/evadb/optimizer/rules/rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7274 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/optimizer/rules/rules_base.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7741 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/optimizer/rules/rules_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12770 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/optimizer/statement_to_opr_converter.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.661783 evadb-0.3.0/evadb/parser/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1362 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/alias.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2754 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/create_index_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5324 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/create_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4436 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/create_udf_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2058 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/delete_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2131 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/drop_object_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19665 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/parser/evadb.lark
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1390 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/explain_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2932 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/insert_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1724 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_parser.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.661783 evadb-0.3.0/evadb/parser/lark_visitor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_visitor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2163 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/parser/lark_visitor/_common_clauses_ids.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9784 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/parser/lark_visitor/_create_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1410 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_visitor/_delete_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2007 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_visitor/_drop_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1010 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_visitor/_explain_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5894 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/parser/lark_visitor/_expressions.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5776 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/parser/lark_visitor/_functions.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2510 2023-06-26 14:59:01.000000 evadb-0.3.0/evadb/parser/lark_visitor/_insert_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2247 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_visitor/_load_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      938 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_visitor/_rename_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2149 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_visitor/_select_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1118 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/lark_visitor/_show_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9562 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/parser/lark_visitor/_table_sources.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3224 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/load_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1233 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/parser.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2015 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/rename_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6258 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/select_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1466 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/show_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1430 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/parser/statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9180 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/parser/table_ref.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1849 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/parser/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6234 2023-06-22 16:24:39.000000 evadb-0.3.0/evadb/parser/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.665784 evadb-0.3.0/evadb/plan_nodes/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1699 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/abstract_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3457 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/abstract_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1463 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/abstract_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1940 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/apply_and_merge_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2483 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/create_index_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2210 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/create_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3483 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/create_udf_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/delete_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/drop_object_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2063 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/exchange_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1039 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/explain_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1763 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/function_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1507 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/groupby_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1722 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/hash_join_build_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2191 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/hash_join_probe_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2033 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/insert_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1418 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/lateral_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1476 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/limit_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2720 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/load_data_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1520 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/nested_loop_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1570 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/orderby_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1185 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/pp_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1253 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/predicate_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1257 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/project_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1624 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/rename_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1477 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/sample_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1768 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/seq_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1209 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/show_info_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4559 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/plan_nodes/storage_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1370 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/plan_nodes/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1251 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/union_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2732 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/plan_nodes/vector_index_scan_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.665784 evadb-0.3.0/evadb/readers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/readers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2328 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/readers/abstract_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2620 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/readers/csv_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5877 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/readers/decord_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.665784 evadb-0.3.0/evadb/readers/document/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/readers/document/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2079 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/readers/document/document_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2109 2023-06-22 16:24:39.000000 evadb-0.3.0/evadb/readers/document/registry.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.665784 evadb-0.3.0/evadb/readers/image/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/readers/image/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1163 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/readers/image/opencv_image_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2139 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/readers/pdf_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.665784 evadb-0.3.0/evadb/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      625 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3871 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/server/command_handler.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3641 2023-06-26 14:59:01.000000 evadb-0.3.0/evadb/server/interpreter.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3393 2023-06-26 14:59:01.000000 evadb-0.3.0/evadb/server/server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.669784 evadb-0.3.0/evadb/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6187 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/storage/abstract_media_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2497 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/storage/abstract_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1870 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/storage/document_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1789 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/storage/image_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1764 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/storage/pdf_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9483 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/storage/sqlite_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2066 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/storage/storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2562 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/storage/video_storage_engine.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.669784 evadb-0.3.0/evadb/third_party/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      607 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/third_party/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.669784 evadb-0.3.0/evadb/third_party/huggingface/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      614 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/third_party/huggingface/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1428 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/third_party/huggingface/binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6593 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/third_party/huggingface/create.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2697 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/third_party/huggingface/model.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.669784 evadb-0.3.0/evadb/third_party/vector_stores/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      609 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/third_party/vector_stores/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2919 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/third_party/vector_stores/faiss.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2852 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/third_party/vector_stores/qdrant.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1378 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/third_party/vector_stores/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1608 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/third_party/vector_stores/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.669784 evadb-0.3.0/evadb/udfs/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.669784 evadb-0.3.0/evadb/udfs/abstract/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      627 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/abstract/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2446 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/abstract/abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4249 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/abstract/hf_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4067 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/abstract/pytorch_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3928 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/abstract/tracker_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3462 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/asl_action_recognition.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4684 2023-06-27 00:54:47.000000 evadb-0.3.0/evadb/udfs/chatgpt.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.673784 evadb-0.3.0/evadb/udfs/decorators/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/decorators/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2192 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/decorators/decorators.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.673784 evadb-0.3.0/evadb/udfs/decorators/io_descriptors/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2761 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/decorators/io_descriptors/abstract_types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3386 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/decorators/io_descriptors/data_types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2073 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/decorators/utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6056 2023-06-25 23:15:30.000000 evadb-0.3.0/evadb/udfs/emotion_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2886 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/face_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5851 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/fastrcnn_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1826 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2516 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1030 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/gpu_compatible.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3993 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/mnist_image_classifier.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2183 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/mvit_action_recognition.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.673784 evadb-0.3.0/evadb/udfs/ndarray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      640 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/ndarray/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2582 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/ndarray/annotate.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2572 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/ndarray/array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1651 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/ndarray/crop.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1183 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/ndarray/fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2310 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/ndarray/gaussian_blur.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2327 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/ndarray/horizontal_flip.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1662 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/ndarray/open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1887 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/ndarray/similarity.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2233 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/ndarray/to_grayscale.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2313 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/ndarray/vertical_flip.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2705 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/saliency_feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2545 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/sentence_feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3159 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/sift_feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2176 2023-06-27 23:59:04.000000 evadb-0.3.0/evadb/udfs/text_filter_keyword.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.673784 evadb-0.3.0/evadb/udfs/trackers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/udfs/trackers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2506 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/trackers/nor_fair.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8714 2023-06-27 00:54:47.000000 evadb-0.3.0/evadb/udfs/udf_bootstrap_queries.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3825 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/udfs/yolo_object_detector.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.673784 evadb-0.3.0/evadb/utils/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      615 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/utils/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      911 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/utils/errors.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12289 2023-06-27 00:54:47.000000 evadb-0.3.0/evadb/utils/generic_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1958 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/utils/kv_cache.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      987 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/utils/logging_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1390 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/utils/math_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1651 2023-06-21 17:21:29.000000 evadb-0.3.0/evadb/utils/s3_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1696 2023-06-08 22:16:06.000000 evadb-0.3.0/evadb/utils/stats.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      123 2023-06-27 23:59:44.000000 evadb-0.3.0/evadb/version.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.645783 evadb-0.3.0/evadb.egg-info/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13108 2023-06-27 23:59:46.000000 evadb-0.3.0/evadb.egg-info/PKG-INFO
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14257 2023-06-27 23:59:46.000000 evadb-0.3.0/evadb.egg-info/SOURCES.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        1 2023-06-27 23:59:46.000000 evadb-0.3.0/evadb.egg-info/dependency_links.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      100 2023-06-27 23:59:46.000000 evadb-0.3.0/evadb.egg-info/entry_points.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1418 2023-06-27 23:59:46.000000 evadb-0.3.0/evadb.egg-info/requires.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       23 2023-06-27 23:59:46.000000 evadb-0.3.0/evadb.egg-info/top_level.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       90 2023-06-08 04:02:21.000000 evadb-0.3.0/pyproject.toml
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       38 2023-06-27 23:59:46.689784 evadb-0.3.0/setup.cfg
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4769 2023-06-27 23:59:01.000000 evadb-0.3.0/setup.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.673784 evadb-0.3.0/test/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.673784 evadb-0.3.0/test/app_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-21 17:21:29.000000 evadb-0.3.0/test/app_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1799 2023-06-26 03:15:21.000000 evadb-0.3.0/test/app_tests/test_pandas_qa.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3237 2023-06-21 17:21:29.000000 evadb-0.3.0/test/app_tests/test_privategpt.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2022 2023-06-27 00:54:47.000000 evadb-0.3.0/test/app_tests/test_youtube_channel_qa.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2025 2023-06-22 16:24:39.000000 evadb-0.3.0/test/app_tests/test_youtube_qa.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.677784 evadb-0.3.0/test/benchmark_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/benchmark_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1265 2023-06-08 22:16:06.000000 evadb-0.3.0/test/benchmark_tests/conftest.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6923 2023-06-25 23:15:30.000000 evadb-0.3.0/test/benchmark_tests/test_benchmark_pytorch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.677784 evadb-0.3.0/test/binder/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/binder/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14091 2023-06-25 23:15:30.000000 evadb-0.3.0/test/binder/test_statement_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8188 2023-06-21 17:21:29.000000 evadb-0.3.0/test/binder/test_statement_binder_context.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.677784 evadb-0.3.0/test/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/catalog/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.677784 evadb-0.3.0/test/catalog/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/catalog/models/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7252 2023-06-08 22:16:06.000000 evadb-0.3.0/test/catalog/models/test_models.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7355 2023-06-08 22:16:06.000000 evadb-0.3.0/test/catalog/test_catalog_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1406 2023-06-08 22:16:06.000000 evadb-0.3.0/test/catalog/test_column_type.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.677784 evadb-0.3.0/test/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1110 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/test_abstract_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4081 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/test_create_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4273 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/test_execution_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4747 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/test_limit_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2936 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/test_orderby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9933 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/test_plan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1867 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/test_sample_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3037 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/test_seq_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      851 2023-06-08 22:16:06.000000 evadb-0.3.0/test/executor/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.677784 evadb-0.3.0/test/expression/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/expression/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3734 2023-06-08 22:16:06.000000 evadb-0.3.0/test/expression/test_abstract_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5123 2023-06-21 17:21:29.000000 evadb-0.3.0/test/expression/test_aggregation.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2985 2023-06-08 22:16:06.000000 evadb-0.3.0/test/expression/test_arithmetic.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5590 2023-06-08 22:16:06.000000 evadb-0.3.0/test/expression/test_comparison.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2871 2023-06-21 17:21:29.000000 evadb-0.3.0/test/expression/test_expression_tree.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7567 2023-06-21 17:21:29.000000 evadb-0.3.0/test/expression/test_expression_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2701 2023-06-08 22:16:06.000000 evadb-0.3.0/test/expression/test_function_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10224 2023-06-21 17:21:29.000000 evadb-0.3.0/test/expression/test_logical.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.681784 evadb-0.3.0/test/integration_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3703 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/test_array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6362 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_create_index_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3966 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_create_table_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5271 2023-06-21 17:21:29.000000 evadb-0.3.0/test/integration_tests/test_delete_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7282 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_drop_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2373 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_error_handling_with_ray.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3683 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/test_explain_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2862 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/test_fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17606 2023-06-27 00:54:47.000000 evadb-0.3.0/test/integration_tests/test_huggingface_udfs.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3964 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/test_insert_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3100 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/test_like.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    23292 2023-06-27 23:59:04.000000 evadb-0.3.0/test/integration_tests/test_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2028 2023-06-27 23:59:04.000000 evadb-0.3.0/test/integration_tests/test_load_pdf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2667 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/test_open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11073 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_optimizer_rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15830 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_pytorch.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3083 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/test_rename_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10968 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_reuse.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5432 2023-06-21 17:21:29.000000 evadb-0.3.0/test/integration_tests/test_s3_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2416 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_saliency.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    32438 2023-06-25 23:15:30.000000 evadb-0.3.0/test/integration_tests/test_select_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3452 2023-06-08 22:16:06.000000 evadb-0.3.0/test/integration_tests/test_show_info_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    16799 2023-06-27 00:54:47.000000 evadb-0.3.0/test/integration_tests/test_similarity.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2069 2023-06-27 23:59:04.000000 evadb-0.3.0/test/integration_tests/test_text_filtering.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12693 2023-06-27 00:54:47.000000 evadb-0.3.0/test/integration_tests/test_udf_executor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.681784 evadb-0.3.0/test/interfaces/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/interfaces/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.681784 evadb-0.3.0/test/interfaces/relational/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/interfaces/relational/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15497 2023-06-27 23:59:01.000000 evadb-0.3.0/test/interfaces/relational/test_relational_api.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1874 2023-06-27 23:59:01.000000 evadb-0.3.0/test/markers.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.681784 evadb-0.3.0/test/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/models/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.681784 evadb-0.3.0/test/models/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/models/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1016 2023-06-08 22:16:06.000000 evadb-0.3.0/test/models/catalog/test_frame_info.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.681784 evadb-0.3.0/test/models/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/models/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5925 2023-06-08 22:16:06.000000 evadb-0.3.0/test/models/storage/test_batch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.681784 evadb-0.3.0/test/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11782 2023-06-25 23:15:30.000000 evadb-0.3.0/test/optimizer/rules/test_rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4246 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/test_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2329 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/test_cascade_optimizer.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4512 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/test_cost_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2697 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/test_group.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2002 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/test_memo.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1053 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/test_optimizer_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5668 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/test_optimizer_task.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2008 2023-06-08 22:16:06.000000 evadb-0.3.0/test/optimizer/test_optimizer_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12882 2023-06-25 23:15:30.000000 evadb-0.3.0/test/optimizer/test_statement_to_opr_converter.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/parser/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/parser/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    35519 2023-06-25 23:15:30.000000 evadb-0.3.0/test/parser/test_parser.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7747 2023-06-25 23:15:30.000000 evadb-0.3.0/test/parser/test_parser_statements.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/plan_nodes/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/plan_nodes/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5540 2023-06-25 23:15:30.000000 evadb-0.3.0/test/plan_nodes/test_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/readers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/readers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1682 2023-06-21 17:21:29.000000 evadb-0.3.0/test/readers/test_csv_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8218 2023-06-21 17:21:29.000000 evadb-0.3.0/test/readers/test_decord_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1278 2023-06-08 22:16:06.000000 evadb-0.3.0/test/server/test_command_handler.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1252 2023-06-27 00:55:06.000000 evadb-0.3.0/test/server/test_configuration_file.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5221 2023-06-08 22:16:06.000000 evadb-0.3.0/test/server/test_db_api.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2687 2023-06-21 17:21:29.000000 evadb-0.3.0/test/server/test_interpreter.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2171 2023-06-08 22:16:06.000000 evadb-0.3.0/test/server/test_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4512 2023-06-08 22:16:06.000000 evadb-0.3.0/test/storage/test_sqlite_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4165 2023-06-08 22:16:06.000000 evadb-0.3.0/test/storage/test_video_storage.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3341 2023-06-08 22:16:06.000000 evadb-0.3.0/test/test_eva_cmd_client.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1310 2023-06-08 22:16:06.000000 evadb-0.3.0/test/test_eva_imports.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1427 2023-06-08 22:16:06.000000 evadb-0.3.0/test/test_eva_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/udfs/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      640 2023-06-08 22:16:06.000000 evadb-0.3.0/test/udfs/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/udfs/decorators/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/udfs/decorators/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.685784 evadb-0.3.0/test/udfs/decorators/io_descriptors/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7437 2023-06-08 22:16:06.000000 evadb-0.3.0/test/udfs/decorators/io_descriptors/test_descriptors.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2145 2023-06-08 22:16:06.000000 evadb-0.3.0/test/udfs/decorators/test_decorators.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.689784 evadb-0.3.0/test/udfs/ndarray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      650 2023-06-08 22:16:06.000000 evadb-0.3.0/test/udfs/ndarray/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1951 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/ndarray/test_annotate.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      853 2023-06-08 22:16:06.000000 evadb-0.3.0/test/udfs/ndarray/test_array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2414 2023-06-08 22:16:06.000000 evadb-0.3.0/test/udfs/ndarray/test_crop.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2187 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/ndarray/test_flips.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1764 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/ndarray/test_gaussian_blur.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2362 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/ndarray/test_open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1761 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/ndarray/test_to_grayscale.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4499 2023-06-27 23:59:01.000000 evadb-0.3.0/test/udfs/test_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2913 2023-06-25 04:22:18.000000 evadb-0.3.0/test/udfs/test_chatgpt.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2257 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/test_emotion_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2892 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/test_facenet_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1938 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/test_fastrcnn_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2920 2023-06-21 17:21:29.000000 evadb-0.3.0/test/udfs/test_yolo_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    18203 2023-06-27 00:54:47.000000 evadb-0.3.0/test/util.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.689784 evadb-0.3.0/test/utils/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.0/test/utils/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3939 2023-06-08 22:16:06.000000 evadb-0.3.0/test/utils/test_generic_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2283 2023-06-08 22:16:06.000000 evadb-0.3.0/test/utils/test_timer.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-27 23:59:46.689784 evadb-0.3.0/third_party/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 04:02:21.000000 evadb-0.3.0/third_party/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11357 2023-06-08 04:02:21.000000 evadb-0.3.1/LICENSE.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13372 2023-06-30 04:21:39.564039 evadb-0.3.1/PKG-INFO
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12562 2023-06-30 04:21:37.000000 evadb-0.3.1/README.md
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.520037 evadb-0.3.1/evadb/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      905 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.524037 evadb-0.3.1/evadb/binder/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/binder/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8749 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/binder/binder_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14313 2023-06-27 00:54:47.000000 evadb-0.3.1/evadb/binder/statement_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7978 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/binder/statement_binder_context.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.524037 evadb-0.3.1/evadb/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19545 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/catalog/catalog_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3373 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/catalog/catalog_type.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10319 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/catalog/catalog_utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.524037 evadb-0.3.1/evadb/catalog/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1503 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/association_models.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4751 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/base_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4551 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/column_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2871 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/index_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2441 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/table_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3022 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/udf_cache_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3101 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/udf_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1804 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/udf_cost_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3923 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/udf_io_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2205 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/udf_metadata_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6789 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/models/utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2126 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/schema_utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.524037 evadb-0.3.1/evadb/catalog/services/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1291 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/base_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3377 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/column_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2970 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/index_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4961 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/table_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3999 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/udf_cache_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3249 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/udf_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3036 2023-06-25 03:38:24.000000 evadb-0.3.1/evadb/catalog/services/udf_cost_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2934 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/udf_io_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2226 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/catalog/services/udf_metadata_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2793 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/catalog/sql_config.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.528037 evadb-0.3.1/evadb/configuration/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      622 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/configuration/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5035 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/configuration/bootstrap_environment.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2508 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/configuration/configuration_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1055 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/configuration/constants.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      884 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/constants.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1964 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/database.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      570 2023-06-26 03:28:32.000000 evadb-0.3.1/evadb/evadb.yml
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2018 2023-06-08 22:16:07.000000 evadb-0.3.1/evadb/evadb_cmd_client.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2023-06-08 22:16:07.000000 evadb-0.3.1/evadb/evadb_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.532038 evadb-0.3.1/evadb/executor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      617 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3803 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/abstract_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2324 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/apply_and_merge_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2034 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/executor/create_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5099 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/create_index_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7395 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/executor/create_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4732 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/executor/delete_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4959 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/executor/drop_object_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3635 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/executor/exchange_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3025 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/execution_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5513 2023-06-25 22:35:38.000000 evadb-0.3.1/evadb/executor/executor_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1596 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/explain_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2005 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/function_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1897 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/groupby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1944 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/hash_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2243 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/executor/insert_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1688 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/join_build_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1843 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/lateral_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1655 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/limit_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3080 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/executor/load_csv_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1742 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6141 2023-06-26 03:15:21.000000 evadb-0.3.1/evadb/executor/load_multimedia_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/nested_loop_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4263 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/orderby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8299 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/executor/plan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1716 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/pp_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1367 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/predicate_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1362 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/project_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2443 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/executor/ray_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1267 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/rename_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1485 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/sample_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1918 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/seq_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1846 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/show_info_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2646 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/executor/storage_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1336 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/union_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4395 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/executor/vector_index_scan_executor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.532038 evadb-0.3.1/evadb/expression/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      619 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/expression/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5561 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/expression/abstract_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3979 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/expression/aggregation_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1624 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/expression/arithmetic_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4357 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/expression/comparison_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2550 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/expression/constant_value_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10445 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/expression/expression_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10064 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/expression/function_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3059 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/expression/logical_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4330 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/expression/tuple_value_expression.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.532038 evadb-0.3.1/evadb/interfaces/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/interfaces/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.532038 evadb-0.3.1/evadb/interfaces/relational/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/interfaces/relational/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    20428 2023-06-30 03:57:31.000000 evadb-0.3.1/evadb/interfaces/relational/db.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7755 2023-06-22 16:24:39.000000 evadb-0.3.1/evadb/interfaces/relational/relation.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4596 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/interfaces/relational/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.532038 evadb-0.3.1/evadb/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      637 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/models/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.532038 evadb-0.3.1/evadb/models/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/models/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1336 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/models/catalog/frame_info.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      859 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/models/catalog/properties.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.532038 evadb-0.3.1/evadb/models/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/models/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1971 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/models/server/response.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.532038 evadb-0.3.1/evadb/models/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/models/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15331 2023-06-09 18:53:37.000000 evadb-0.3.1/evadb/models/storage/batch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.536038 evadb-0.3.1/evadb/optimizer/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      624 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3269 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2145 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/cost_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3460 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/group.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2677 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/group_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4347 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/memo.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    35384 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/optimizer/operators.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4040 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/optimizer_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      986 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/optimizer_task_stack.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12600 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/optimizer_tasks.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11286 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/optimizer/optimizer_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4184 2023-06-26 14:59:01.000000 evadb-0.3.1/evadb/optimizer/plan_generator.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1171 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/property.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.536038 evadb-0.3.1/evadb/optimizer/rules/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/rules/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1023 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/optimizer/rules/pattern.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    48852 2023-06-30 04:21:37.000000 evadb-0.3.1/evadb/optimizer/rules/rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7274 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/optimizer/rules/rules_base.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7741 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/optimizer/rules/rules_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12770 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/optimizer/statement_to_opr_converter.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.536038 evadb-0.3.1/evadb/parser/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1362 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/alias.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2754 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/create_index_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5324 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/create_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4436 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/create_udf_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2058 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/delete_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2131 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/drop_object_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19665 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/parser/evadb.lark
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1390 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/explain_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2932 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/insert_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1724 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_parser.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.540038 evadb-0.3.1/evadb/parser/lark_visitor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_visitor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2163 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/parser/lark_visitor/_common_clauses_ids.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9784 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/parser/lark_visitor/_create_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1410 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_visitor/_delete_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2007 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_visitor/_drop_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1010 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_visitor/_explain_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5894 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/parser/lark_visitor/_expressions.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5776 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/parser/lark_visitor/_functions.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2510 2023-06-26 14:59:01.000000 evadb-0.3.1/evadb/parser/lark_visitor/_insert_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2247 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_visitor/_load_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      938 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_visitor/_rename_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2149 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_visitor/_select_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1118 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/lark_visitor/_show_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9562 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/parser/lark_visitor/_table_sources.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3224 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/load_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1233 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/parser.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2015 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/rename_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6258 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/select_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1466 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/show_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1430 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/parser/statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9180 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/parser/table_ref.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1849 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/parser/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6234 2023-06-22 16:24:39.000000 evadb-0.3.1/evadb/parser/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/plan_nodes/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1699 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/abstract_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3457 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/abstract_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1463 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/abstract_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1940 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/apply_and_merge_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2232 2023-06-30 04:21:37.000000 evadb-0.3.1/evadb/plan_nodes/create_from_select_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2483 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/create_index_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2210 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/create_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3483 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/create_udf_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/delete_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/drop_object_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2063 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/exchange_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1039 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/explain_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1763 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/function_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1507 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/groupby_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1722 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/hash_join_build_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2191 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/hash_join_probe_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2033 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/insert_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1418 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/lateral_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1476 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/limit_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2720 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/load_data_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1520 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/nested_loop_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1570 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/orderby_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1185 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/pp_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1253 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/predicate_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1257 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/project_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1624 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/rename_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1477 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/sample_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1768 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/seq_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1209 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/show_info_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4559 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/plan_nodes/storage_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1370 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/plan_nodes/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1251 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/union_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2732 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/plan_nodes/vector_index_scan_plan.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/readers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/readers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2328 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/readers/abstract_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2620 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/readers/csv_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5877 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/readers/decord_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/readers/document/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/readers/document/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2079 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/readers/document/document_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2109 2023-06-22 16:24:39.000000 evadb-0.3.1/evadb/readers/document/registry.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/readers/image/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/readers/image/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1163 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/readers/image/opencv_image_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2139 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/readers/pdf_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      625 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3871 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/server/command_handler.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3641 2023-06-26 14:59:01.000000 evadb-0.3.1/evadb/server/interpreter.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3393 2023-06-26 14:59:01.000000 evadb-0.3.1/evadb/server/server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6187 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/storage/abstract_media_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2497 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/storage/abstract_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1870 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/storage/document_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1789 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/storage/image_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1764 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/storage/pdf_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9467 2023-06-30 00:37:21.000000 evadb-0.3.1/evadb/storage/sqlite_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2066 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/storage/storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2562 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/storage/video_storage_engine.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/third_party/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      607 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/third_party/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/third_party/huggingface/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      614 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/third_party/huggingface/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1428 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/third_party/huggingface/binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6593 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/third_party/huggingface/create.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2697 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/third_party/huggingface/model.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.544038 evadb-0.3.1/evadb/third_party/vector_stores/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      609 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/third_party/vector_stores/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2919 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/third_party/vector_stores/faiss.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2852 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/third_party/vector_stores/qdrant.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1378 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/third_party/vector_stores/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1608 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/third_party/vector_stores/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.548038 evadb-0.3.1/evadb/udfs/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.548038 evadb-0.3.1/evadb/udfs/abstract/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      627 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/abstract/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2446 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/abstract/abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4249 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/abstract/hf_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4067 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/abstract/pytorch_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3928 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/abstract/tracker_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3462 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/asl_action_recognition.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6971 2023-06-30 03:38:56.000000 evadb-0.3.1/evadb/udfs/chatgpt.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.548038 evadb-0.3.1/evadb/udfs/decorators/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/decorators/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2192 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/decorators/decorators.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.548038 evadb-0.3.1/evadb/udfs/decorators/io_descriptors/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2761 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/decorators/io_descriptors/abstract_types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3386 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/decorators/io_descriptors/data_types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2073 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/decorators/utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6056 2023-06-25 23:15:30.000000 evadb-0.3.1/evadb/udfs/emotion_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2886 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/face_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5851 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/fastrcnn_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1826 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2516 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1030 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/gpu_compatible.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3993 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/mnist_image_classifier.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2183 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/mvit_action_recognition.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.548038 evadb-0.3.1/evadb/udfs/ndarray/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      640 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/ndarray/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2582 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/ndarray/annotate.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2572 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/ndarray/array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1651 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/ndarray/crop.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1183 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/ndarray/fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2310 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/ndarray/gaussian_blur.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2327 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/ndarray/horizontal_flip.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1662 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/ndarray/open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1887 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/ndarray/similarity.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2233 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/ndarray/to_grayscale.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2313 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/ndarray/vertical_flip.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2705 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/saliency_feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2545 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/sentence_feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3159 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/sift_feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2176 2023-06-27 23:59:04.000000 evadb-0.3.1/evadb/udfs/text_filter_keyword.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.552038 evadb-0.3.1/evadb/udfs/trackers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/udfs/trackers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2506 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/trackers/nor_fair.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8714 2023-06-27 00:54:47.000000 evadb-0.3.1/evadb/udfs/udf_bootstrap_queries.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3825 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/udfs/yolo_object_detector.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.552038 evadb-0.3.1/evadb/utils/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      615 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/utils/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      911 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/utils/errors.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12499 2023-06-30 03:32:27.000000 evadb-0.3.1/evadb/utils/generic_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1958 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/utils/kv_cache.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      987 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/utils/logging_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1390 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/utils/math_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1651 2023-06-21 17:21:29.000000 evadb-0.3.1/evadb/utils/s3_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1696 2023-06-08 22:16:06.000000 evadb-0.3.1/evadb/utils/stats.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      123 2023-06-30 04:21:37.000000 evadb-0.3.1/evadb/version.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.524037 evadb-0.3.1/evadb.egg-info/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13372 2023-06-30 04:21:39.000000 evadb-0.3.1/evadb.egg-info/PKG-INFO
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14301 2023-06-30 04:21:39.000000 evadb-0.3.1/evadb.egg-info/SOURCES.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        1 2023-06-30 04:21:39.000000 evadb-0.3.1/evadb.egg-info/dependency_links.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      100 2023-06-30 04:21:39.000000 evadb-0.3.1/evadb.egg-info/entry_points.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1403 2023-06-30 04:21:39.000000 evadb-0.3.1/evadb.egg-info/requires.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       23 2023-06-30 04:21:39.000000 evadb-0.3.1/evadb.egg-info/top_level.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       90 2023-06-08 04:02:21.000000 evadb-0.3.1/pyproject.toml
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       38 2023-06-30 04:21:39.564039 evadb-0.3.1/setup.cfg
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4707 2023-06-30 03:31:51.000000 evadb-0.3.1/setup.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.552038 evadb-0.3.1/test/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.552038 evadb-0.3.1/test/app_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-21 17:21:29.000000 evadb-0.3.1/test/app_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1869 2023-06-30 03:57:31.000000 evadb-0.3.1/test/app_tests/test_pandas_qa.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3237 2023-06-21 17:21:29.000000 evadb-0.3.1/test/app_tests/test_privategpt.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2022 2023-06-27 00:54:47.000000 evadb-0.3.1/test/app_tests/test_youtube_channel_qa.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2095 2023-06-30 03:43:49.000000 evadb-0.3.1/test/app_tests/test_youtube_qa.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.552038 evadb-0.3.1/test/benchmark_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/benchmark_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1265 2023-06-08 22:16:06.000000 evadb-0.3.1/test/benchmark_tests/conftest.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6923 2023-06-25 23:15:30.000000 evadb-0.3.1/test/benchmark_tests/test_benchmark_pytorch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.552038 evadb-0.3.1/test/binder/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/binder/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14091 2023-06-25 23:15:30.000000 evadb-0.3.1/test/binder/test_statement_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8188 2023-06-21 17:21:29.000000 evadb-0.3.1/test/binder/test_statement_binder_context.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.552038 evadb-0.3.1/test/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/catalog/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.552038 evadb-0.3.1/test/catalog/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/catalog/models/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7252 2023-06-08 22:16:06.000000 evadb-0.3.1/test/catalog/models/test_models.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7355 2023-06-08 22:16:06.000000 evadb-0.3.1/test/catalog/test_catalog_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1406 2023-06-08 22:16:06.000000 evadb-0.3.1/test/catalog/test_column_type.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.556038 evadb-0.3.1/test/executor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1110 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/test_abstract_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4081 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/test_create_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4273 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/test_execution_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4747 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/test_limit_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2936 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/test_orderby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9933 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/test_plan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1867 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/test_sample_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3037 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/test_seq_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      851 2023-06-08 22:16:06.000000 evadb-0.3.1/test/executor/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.556038 evadb-0.3.1/test/expression/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/expression/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3734 2023-06-08 22:16:06.000000 evadb-0.3.1/test/expression/test_abstract_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5123 2023-06-21 17:21:29.000000 evadb-0.3.1/test/expression/test_aggregation.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2985 2023-06-08 22:16:06.000000 evadb-0.3.1/test/expression/test_arithmetic.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5590 2023-06-08 22:16:06.000000 evadb-0.3.1/test/expression/test_comparison.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2871 2023-06-21 17:21:29.000000 evadb-0.3.1/test/expression/test_expression_tree.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7567 2023-06-21 17:21:29.000000 evadb-0.3.1/test/expression/test_expression_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2701 2023-06-08 22:16:06.000000 evadb-0.3.1/test/expression/test_function_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10224 2023-06-21 17:21:29.000000 evadb-0.3.1/test/expression/test_logical.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/integration_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3703 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/test_array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6362 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_create_index_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3966 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_create_table_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5205 2023-06-30 00:37:21.000000 evadb-0.3.1/test/integration_tests/test_delete_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7282 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_drop_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2373 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_error_handling_with_ray.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3683 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/test_explain_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2862 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/test_fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17606 2023-06-27 00:54:47.000000 evadb-0.3.1/test/integration_tests/test_huggingface_udfs.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3964 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/test_insert_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3100 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/test_like.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    23292 2023-06-27 23:59:04.000000 evadb-0.3.1/test/integration_tests/test_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2028 2023-06-27 23:59:04.000000 evadb-0.3.1/test/integration_tests/test_load_pdf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2667 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/test_open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11073 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_optimizer_rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15830 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_pytorch.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3083 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/test_rename_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10968 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_reuse.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5432 2023-06-21 17:21:29.000000 evadb-0.3.1/test/integration_tests/test_s3_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2416 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_saliency.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    32438 2023-06-25 23:15:30.000000 evadb-0.3.1/test/integration_tests/test_select_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3452 2023-06-08 22:16:06.000000 evadb-0.3.1/test/integration_tests/test_show_info_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    16799 2023-06-27 00:54:47.000000 evadb-0.3.1/test/integration_tests/test_similarity.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2074 2023-06-30 03:37:35.000000 evadb-0.3.1/test/integration_tests/test_text_filtering.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12693 2023-06-27 00:54:47.000000 evadb-0.3.1/test/integration_tests/test_udf_executor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/interfaces/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/interfaces/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/interfaces/relational/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/interfaces/relational/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15542 2023-06-30 00:37:21.000000 evadb-0.3.1/test/interfaces/relational/test_relational_api.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1948 2023-06-30 03:41:40.000000 evadb-0.3.1/test/markers.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/models/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/models/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/models/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1016 2023-06-08 22:16:06.000000 evadb-0.3.1/test/models/catalog/test_frame_info.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/models/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/models/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5925 2023-06-08 22:16:06.000000 evadb-0.3.1/test/models/storage/test_batch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/optimizer/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/optimizer/rules/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/rules/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11782 2023-06-25 23:15:30.000000 evadb-0.3.1/test/optimizer/rules/test_rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4246 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/test_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2329 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/test_cascade_optimizer.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4512 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/test_cost_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2697 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/test_group.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2002 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/test_memo.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1053 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/test_optimizer_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5668 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/test_optimizer_task.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2008 2023-06-08 22:16:06.000000 evadb-0.3.1/test/optimizer/test_optimizer_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12882 2023-06-25 23:15:30.000000 evadb-0.3.1/test/optimizer/test_statement_to_opr_converter.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/parser/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/parser/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    35519 2023-06-25 23:15:30.000000 evadb-0.3.1/test/parser/test_parser.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7747 2023-06-25 23:15:30.000000 evadb-0.3.1/test/parser/test_parser_statements.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/plan_nodes/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/plan_nodes/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5540 2023-06-25 23:15:30.000000 evadb-0.3.1/test/plan_nodes/test_plan.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.560038 evadb-0.3.1/test/readers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/readers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1682 2023-06-21 17:21:29.000000 evadb-0.3.1/test/readers/test_csv_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8218 2023-06-21 17:21:29.000000 evadb-0.3.1/test/readers/test_decord_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/test/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1278 2023-06-08 22:16:06.000000 evadb-0.3.1/test/server/test_command_handler.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1252 2023-06-27 00:55:06.000000 evadb-0.3.1/test/server/test_configuration_file.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5164 2023-06-30 03:57:22.000000 evadb-0.3.1/test/server/test_db_api.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2687 2023-06-21 17:21:29.000000 evadb-0.3.1/test/server/test_interpreter.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2171 2023-06-08 22:16:06.000000 evadb-0.3.1/test/server/test_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/test/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4512 2023-06-08 22:16:06.000000 evadb-0.3.1/test/storage/test_sqlite_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4165 2023-06-08 22:16:06.000000 evadb-0.3.1/test/storage/test_video_storage.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3341 2023-06-08 22:16:06.000000 evadb-0.3.1/test/test_eva_cmd_client.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1310 2023-06-08 22:16:06.000000 evadb-0.3.1/test/test_eva_imports.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1427 2023-06-08 22:16:06.000000 evadb-0.3.1/test/test_eva_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/test/udfs/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      640 2023-06-08 22:16:06.000000 evadb-0.3.1/test/udfs/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/test/udfs/decorators/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/udfs/decorators/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/test/udfs/decorators/io_descriptors/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7437 2023-06-08 22:16:06.000000 evadb-0.3.1/test/udfs/decorators/io_descriptors/test_descriptors.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2145 2023-06-08 22:16:06.000000 evadb-0.3.1/test/udfs/decorators/test_decorators.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/test/udfs/ndarray/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      650 2023-06-08 22:16:06.000000 evadb-0.3.1/test/udfs/ndarray/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1951 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/ndarray/test_annotate.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      853 2023-06-08 22:16:06.000000 evadb-0.3.1/test/udfs/ndarray/test_array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2414 2023-06-08 22:16:06.000000 evadb-0.3.1/test/udfs/ndarray/test_crop.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2187 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/ndarray/test_flips.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1764 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/ndarray/test_gaussian_blur.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2362 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/ndarray/test_open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1761 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/ndarray/test_to_grayscale.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4499 2023-06-27 23:59:01.000000 evadb-0.3.1/test/udfs/test_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2983 2023-06-30 03:43:49.000000 evadb-0.3.1/test/udfs/test_chatgpt.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2257 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/test_emotion_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2892 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/test_facenet_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1938 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/test_fastrcnn_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2920 2023-06-21 17:21:29.000000 evadb-0.3.1/test/udfs/test_yolo_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    18203 2023-06-30 03:27:03.000000 evadb-0.3.1/test/util.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/test/utils/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.3.1/test/utils/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3939 2023-06-08 22:16:06.000000 evadb-0.3.1/test/utils/test_generic_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2283 2023-06-08 22:16:06.000000 evadb-0.3.1/test/utils/test_timer.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-30 04:21:39.564039 evadb-0.3.1/third_party/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 04:02:21.000000 evadb-0.3.1/third_party/__init__.py
```

### Comparing `evadb-0.3.0/LICENSE.txt` & `evadb-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/PKG-INFO` & `evadb-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,8 @@
-Metadata-Version: 2.1
-Name: evadb
-Version: 0.3.0
-Summary: EvaDB AI-Relational Database System
-Home-page: https://github.com/georgia-tech-db/eva
-Download-URL: https://github.com/georgia-tech-db/eva
-Author: Georgia Tech Database Group
-Author-email: arulraj@gatech.edu
-License: Apache License 2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: ray
-Provides-Extra: vision
-Provides-Extra: document
-Provides-Extra: udf
-Provides-Extra: notebook
-Provides-Extra: qdrant
-Provides-Extra: dev
-License-File: LICENSE.txt
-
-# EvaDB AI-SQL Database System
+# EvaDB: Database System for AI Apps
 
 <div>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
             <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EvaDB on Colab"/>
         </a>
         <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
             <img alt="Slack" src="https://img.shields.io/badge/slack-evadb-ff69b4.svg?logo=slack">
@@ -40,44 +15,44 @@
         </a>
         <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
         <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
         <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
         <a href="https://pepy.tech/project/evadb">
           <img alt="Downloads" src="https://static.pepy.tech/badge/evadb"/>
         </a>
-        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
+        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10|%203.11-brightgreen"/>       
 </div>
 
 <p align="center"> <b><h3>EvaDB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
 
-EvaDB is a database system for developing AI apps. We aim to simplify the development and deployment of AI-powered apps that operate on unstructured data (text documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector index).
+EvaDB is a database system for developing AI apps. We aim to simplify the development and deployment of AI apps that operate on unstructured data (text documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector index).
 
-The high-level Python and SQL APIs allow beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under the Apache license.
+The high-level Python and SQL APIs allow beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under an Apache license.
 
 ## Quick Links
 
 - [Features](#features)
 - [Quick Start](#quick-start)
 - [Documentation](#documentation)
 - [Community and Support](#community-and-support)
 - [Twitter](https://twitter.com/evadb_ai)
 
 ## Features
 
-- 🔮 Build simpler AI-powered applications using Python functions or SQL queries
+- 🔮 Build simpler AI-powered apps using Python functions or SQL queries
 - ⚡️ 10x faster applications using AI-centric query optimization  
-- 💰 Save money spent on GPUs
+- 💰 Save money spent on inference
 - 🚀 First-class support for your custom deep learning models through user-defined functions
 - 📦 Built-in caching to eliminate redundant model invocations across queries
-- ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
+- ⌨️ Integrations for PyTorch, Hugging Face, YOLO, and Open AI models
 - 🐍 Installable via pip and fully implemented in Python
 
 ## Illustrative Applications
 
-Here are some illustrative EvaDB-powered applications (each Jupyter notebook can be opened on Google Colab):
+Here are some illustrative AI apps built using EvaDB (each notebook can be opened on Google Colab):
 
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/13-privategpt.html">PrivateGPT</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">ChatGPT-based Video Question Answering</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html">Querying PDF Documents</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing Traffic Flow with YOLO</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining Emotions of Movie</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation with Hugging Face</a>
@@ -89,51 +64,49 @@
   - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/13-privategpt.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EvaDB. Each notebook includes a link to Google Colab, where you can run the code yourself.
 * [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
 * [Follow us on Twitter](https://twitter.com/evadb_ai)
 * [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
 
 ## Quick Start
 
-- Step 1: Install EvaDB using pip. EvaDB supports Python versions >= `3.8`:
+- Step 1: Install EvaDB using `pip`. EvaDB supports Python versions >= `3.8`:
 
 ```shell
 pip install evadb
 ```
 
-- Step 2: Write your AI app!
+- Step 2: It's time to write an AI app.
 
 ```python
 import evadb
 
-# Grab a EvaDB cursor to load data and run queries
+# Grab a EvaDB cursor to load data into tables and run AI queries
 cursor = evadb.connect().cursor()
 
 # Load a collection of news videos into the 'news_videos' table
-# This command returns a Pandas Dataframe with the query's output
-# In this case, the output indicates the number of loaded videos
+# This function returns a Pandas dataframe with the query's output
+# In this case, the output dataframe indicates the number of loaded videos
 cursor.load(
     file_regex="news_videos/*.mp4",
     format="VIDEO",
     table_name="news_videos"
 ).df()
 
 # Define a function that wraps around your deep learning model
-# Here, this function wraps around an off-the-shelf speech-to-text (Whisper) model
-# Such functions are known as user-defined functions or UDFs
-# So, we are creating a Whisper UDF here
-# After creating the UDF, we can use the function in any query
-cursor.create_udf(
+# Here, this function wraps around a speech-to-text model
+# After registering the function, we can use the registered function in subsequent queries
+cursor.create_function(
     udf_name="SpeechRecognizer",
     type="HuggingFace",
     task='automatic-speech-recognition',
     model='openai/whisper-base'
 ).df()
 
-# EvaDB automatically extract the audio from the video
-# We only need to run the SpeechRecongizer UDF on the 'audio' column
+# EvaDB automatically extracts the audio from the video
+# We only need to run the SpeechRecongizer function on the 'audio' column
 # to get the transcript and persist it in a table called 'transcripts'
 cursor.query(
     """CREATE TABLE transcripts AS
        SELECT SpeechRecognizer(audio) from news_videos;"""
 ).df()
 
 # We next incrementally construct the ChatGPT query using EvaDB's Python API
@@ -144,45 +117,53 @@
 # Since ChatGPT is a built-in function, we don't have to define it
 # We can just directly use it in the query
 # We need to set the OPENAI_KEY as an environment variable
 os.environ["OPENAI_KEY"] = OPENAI_KEY
 query = query.select("ChatGPT('Is this video summary related to LLMs', text)")
 
 # Finally, we run the query to get the results as a dataframe
+# You can then post-process the dataframe using other Python libraries
 response = query.df()
 ```
 
-- **Chain multiple models in a single query to set up useful AI pipelines**
+- **Incrementally build an AI query that chains together multiple models**
+
+Here is a AI query that analyses emotions of actors in an `Interstellar` movie clip using multiple PyTorch models.
 
 ```python
-# Analyse emotions of actors in an Interstellar movie clip using PyTorch models
+# Access the Interstellar movie clip table using a cursor
 query = cursor.table("Interstellar")
 # Get faces using a `FaceDetector` function
 query = query.cross_apply("UNNEST(FaceDetector(data))", "Face(bounding_box, confidence)")
 # Focus only on frames 100 through 200 in the clip
 query = query.filter("id > 100 AND id < 200")
 # Get the emotions of the detected faces using a `EmotionDetector` function
 query = query.select("id, bbox, EmotionDetector(Crop(data, bounding_box))")
 
 # Run the query and get the query result as a dataframe
+# At each of the above steps, you can run the query and see the output
+# If you are familiar with SQL, you can get the SQL query with query.sql_query()
 response = query.df()
 ```
-- **EvaDB runs AI apps 10--100x faster using its AI-centric query optimizer**. Three key built-in optimizations are:
+
+- **EvaDB runs AI apps 10x faster using its AI-centric query optimizer**.
+
+  Three key built-in optimizations are:
 
    💾 **Caching**: EvaDB automatically caches and reuses model inference results.
 
    ⚡️ **Parallel Query Execution**: EvaDB runs the app in parallel on all the available hardware resources (CPUs and GPUs).
 
    🎯 **Model Ordering**: EvaDB optimizes the order in which models are evaluated (e.g., runs the faster, more selective model first).
 
 ## Architecture Diagram
 
 This diagram presents the key components of EvaDB. EvaDB's AI-centric query optimizer takes a query as input and generates a query plan that is executed by the query engine. The query engine hits the relevant storage engines to quickly retrieve the data required for efficiently running the query:
 1. Structured data (SQL database system connected via `sqlalchemy`).
-2. Unstructured media data (on cloud buckets/local filesystem).
+2. Unstructured media data (PDFs, videos, etc. on cloud/local filesystem).
 3. Feature data (vector database system).
 
 <img width="500" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
 
 ## Screenshots
 
 ### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
@@ -233,9 +214,9 @@
 
 EvaDB is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EvaDB are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
 
 For more information, see our
 [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
 
 ## License
-Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
+Copyright (c) 2018--present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
 Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,98 +1,91 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.3.0 Summary: EvaDB AI-Relational
-Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
-https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
-Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: ray Provides-Extra: vision Provides-Extra:
-document Provides-Extra: udf Provides-Extra: notebook Provides-Extra: qdrant
-Provides-Extra: dev License-File: LICENSE.txt # EvaDB AI-SQL Database System
+# EvaDB: Database System for AI Apps
 [Open_EvaDB_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
 Status] [Downloads] [Python Versions]
 **** EvaDB is a database system for building simpler and faster AI-powered
 applications. ****
 EvaDB is a database system for developing AI apps. We aim to simplify the
-development and deployment of AI-powered apps that operate on unstructured data
-(text documents, videos, PDFs, podcasts, etc.) and structured data (tables,
-vector index). The high-level Python and SQL APIs allow beginners to use EvaDB
-in a few lines of code. Advanced users can define custom user-defined functions
-that wrap around any AI model or Python library. EvaDB is fully implemented in
-Python and licensed under the Apache license. ## Quick Links - [Features]
+development and deployment of AI apps that operate on unstructured data (text
+documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector
+index). The high-level Python and SQL APIs allow beginners to use EvaDB in a
+few lines of code. Advanced users can define custom user-defined functions that
+wrap around any AI model or Python library. EvaDB is fully implemented in
+Python and licensed under an Apache license. ## Quick Links - [Features]
 (#features) - [Quick Start](#quick-start) - [Documentation](#documentation) -
 [Community and Support](#community-and-support) - [Twitter](https://
-twitter.com/evadb_ai) ## Features - ð® Build simpler AI-powered applications
-using Python functions or SQL queries - â¡ï¸ 10x faster applications using
-AI-centric query optimization - ð° Save money spent on GPUs - ð First-
+twitter.com/evadb_ai) ## Features - ð® Build simpler AI-powered apps using
+Python functions or SQL queries - â¡ï¸ 10x faster applications using AI-
+centric query optimization - ð° Save money spent on inference - ð First-
 class support for your custom deep learning models through user-defined
 functions - ð¦ Built-in caching to eliminate redundant model invocations
-across queries - â¨ï¸ First-class support for PyTorch, Hugging Face, YOLO,
-and Open AI models - ð Installable via pip and fully implemented in Python
-## Illustrative Applications Here are some illustrative EvaDB-powered
-applications (each Jupyter notebook can be opened on Google Colab): * ð®
-PrivateGPT * ð® ChatGPT-based_Video_Question_Answering * ð® Querying_PDF
-Documents * ð® Analysing_Traffic_Flow_with_YOLO * ð® Examining_Emotions_of
-Movie * ð® Image_Segmentation_with_Hugging_Face ## Documentation *
-[Documentation](https://evadb.readthedocs.io/) - The Getting_Started page shows
-how you can use EvaDB for different AI tasks and how you can easily extend
-EvaDB to support your custom deep learning model through user-defined
-functions. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EvaDB. Each notebook includes a link
-to Google Colab, where you can run the code yourself. * [Join us on Slack]
-(https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/evadb_ai)
-* [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3) ## Quick Start
-- Step 1: Install EvaDB using pip. EvaDB supports Python versions >= `3.8`:
-```shell pip install evadb ``` - Step 2: Write your AI app! ```python import
-evadb # Grab a EvaDB cursor to load data and run queries cursor = evadb.connect
-().cursor() # Load a collection of news videos into the 'news_videos' table #
-This command returns a Pandas Dataframe with the query's output # In this case,
-the output indicates the number of loaded videos cursor.load
+across queries - â¨ï¸ Integrations for PyTorch, Hugging Face, YOLO, and Open
+AI models - ð Installable via pip and fully implemented in Python ##
+Illustrative Applications Here are some illustrative AI apps built using EvaDB
+(each notebook can be opened on Google Colab): * ð® PrivateGPT * ð®
+ChatGPT-based_Video_Question_Answering * ð® Querying_PDF_Documents * ð®
+Analysing_Traffic_Flow_with_YOLO * ð® Examining_Emotions_of_Movie * ð®
+Image_Segmentation_with_Hugging_Face ## Documentation * [Documentation](https:/
+/evadb.readthedocs.io/) - The Getting_Started page shows how you can use EvaDB
+for different AI tasks and how you can easily extend EvaDB to support your
+custom deep learning model through user-defined functions. - The User_Guides
+section contains Jupyter Notebooks that demonstrate how to use various features
+of EvaDB. Each notebook includes a link to Google Colab, where you can run the
+code yourself. * [Join us on Slack](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter]
+(https://twitter.com/evadb_ai) * [Roadmap](https://github.com/orgs/georgia-
+tech-db/projects/3) ## Quick Start - Step 1: Install EvaDB using `pip`. EvaDB
+supports Python versions >= `3.8`: ```shell pip install evadb ``` - Step 2:
+It's time to write an AI app. ```python import evadb # Grab a EvaDB cursor to
+load data into tables and run AI queries cursor = evadb.connect().cursor() #
+Load a collection of news videos into the 'news_videos' table # This function
+returns a Pandas dataframe with the query's output # In this case, the output
+dataframe indicates the number of loaded videos cursor.load
 ( file_regex="news_videos/*.mp4", format="VIDEO", table_name="news_videos" ).df
 () # Define a function that wraps around your deep learning model # Here, this
-function wraps around an off-the-shelf speech-to-text (Whisper) model # Such
-functions are known as user-defined functions or UDFs # So, we are creating a
-Whisper UDF here # After creating the UDF, we can use the function in any query
-cursor.create_udf( udf_name="SpeechRecognizer", type="HuggingFace",
-task='automatic-speech-recognition', model='openai/whisper-base' ).df() # EvaDB
-automatically extract the audio from the video # We only need to run the
-SpeechRecongizer UDF on the 'audio' column # to get the transcript and persist
-it in a table called 'transcripts' cursor.query( """CREATE TABLE transcripts AS
-SELECT SpeechRecognizer(audio) from news_videos;""" ).df() # We next
-incrementally construct the ChatGPT query using EvaDB's Python API # The query
-is based on the 'transcripts' table # This table has a column called 'text'
-with the transcript text query = cursor.table('transcripts') # Since ChatGPT is
-a built-in function, we don't have to define it # We can just directly use it
-in the query # We need to set the OPENAI_KEY as an environment variable
-os.environ["OPENAI_KEY"] = OPENAI_KEY query = query.select("ChatGPT('Is this
-video summary related to LLMs', text)") # Finally, we run the query to get the
-results as a dataframe response = query.df() ``` - **Chain multiple models in a
-single query to set up useful AI pipelines** ```python # Analyse emotions of
-actors in an Interstellar movie clip using PyTorch models query = cursor.table
-("Interstellar") # Get faces using a `FaceDetector` function query =
-query.cross_apply("UNNEST(FaceDetector(data))", "Face(bounding_box,
-confidence)") # Focus only on frames 100 through 200 in the clip query =
-query.filter("id > 100 AND id < 200") # Get the emotions of the detected faces
-using a `EmotionDetector` function query = query.select("id, bbox,
-EmotionDetector(Crop(data, bounding_box))") # Run the query and get the query
-result as a dataframe response = query.df() ``` - **EvaDB runs AI apps 10--100x
+function wraps around a speech-to-text model # After registering the function,
+we can use the registered function in subsequent queries cursor.create_function
+( udf_name="SpeechRecognizer", type="HuggingFace", task='automatic-speech-
+recognition', model='openai/whisper-base' ).df() # EvaDB automatically extracts
+the audio from the video # We only need to run the SpeechRecongizer function on
+the 'audio' column # to get the transcript and persist it in a table called
+'transcripts' cursor.query( """CREATE TABLE transcripts AS SELECT
+SpeechRecognizer(audio) from news_videos;""" ).df() # We next incrementally
+construct the ChatGPT query using EvaDB's Python API # The query is based on
+the 'transcripts' table # This table has a column called 'text' with the
+transcript text query = cursor.table('transcripts') # Since ChatGPT is a built-
+in function, we don't have to define it # We can just directly use it in the
+query # We need to set the OPENAI_KEY as an environment variable os.environ
+["OPENAI_KEY"] = OPENAI_KEY query = query.select("ChatGPT('Is this video
+summary related to LLMs', text)") # Finally, we run the query to get the
+results as a dataframe # You can then post-process the dataframe using other
+Python libraries response = query.df() ``` - **Incrementally build an AI query
+that chains together multiple models** Here is a AI query that analyses
+emotions of actors in an `Interstellar` movie clip using multiple PyTorch
+models. ```python # Access the Interstellar movie clip table using a cursor
+query = cursor.table("Interstellar") # Get faces using a `FaceDetector`
+function query = query.cross_apply("UNNEST(FaceDetector(data))", "Face
+(bounding_box, confidence)") # Focus only on frames 100 through 200 in the clip
+query = query.filter("id > 100 AND id < 200") # Get the emotions of the
+detected faces using a `EmotionDetector` function query = query.select("id,
+bbox, EmotionDetector(Crop(data, bounding_box))") # Run the query and get the
+query result as a dataframe # At each of the above steps, you can run the query
+and see the output # If you are familiar with SQL, you can get the SQL query
+with query.sql_query() response = query.df() ``` - **EvaDB runs AI apps 10x
 faster using its AI-centric query optimizer**. Three key built-in optimizations
 are: ð¾ **Caching**: EvaDB automatically caches and reuses model inference
 results. â¡ï¸ **Parallel Query Execution**: EvaDB runs the app in parallel on
 all the available hardware resources (CPUs and GPUs). ð¯ **Model Ordering**:
 EvaDB optimizes the order in which models are evaluated (e.g., runs the faster,
 more selective model first). ## Architecture Diagram This diagram presents the
 key components of EvaDB. EvaDB's AI-centric query optimizer takes a query as
 input and generates a query plan that is executed by the query engine. The
 query engine hits the relevant storage engines to quickly retrieve the data
 required for efficiently running the query: 1. Structured data (SQL database
-system connected via `sqlalchemy`). 2. Unstructured media data (on cloud
-buckets/local filesystem). 3. Feature data (vector database system).
+system connected via `sqlalchemy`). 2. Unstructured media data (PDFs, videos,
+etc. on cloud/local filesystem). 3. Feature data (vector database system).
 [Architecture Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
 ---------| |[Source Video] |[Query Result] | ### ð® [PDF Question Answering]
 (https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html)
 (Question Answering Model) | App | |-----| |[Source Video] | ### ð® [MNIST
 Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
@@ -119,10 +112,10 @@
 /circleci.com/gh/georgia-tech-db/eva) [![Documentation Status](https://
 readthedocs.org/projects/evadb/badge/?version=latest)](https://
 evadb.readthedocs.io/en/latest/index.html) EvaDB is the beneficiary of many
 [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
 kinds of contributions to EvaDB are appreciated. To file a bug or to request a
 feature, please use GitHub_issues. Pull_requests are welcome. For more
 information, see our [contribution guide](https://evadb.readthedocs.io/en/
-stable/source/contribute/index.html). ## License Copyright (c) 2018-present
+stable/source/contribute/index.html). ## License Copyright (c) 2018--present
 [Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
 License](LICENSE).
```

### Comparing `evadb-0.3.0/README.md` & `evadb-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,33 @@
-# EvaDB AI-SQL Database System
+Metadata-Version: 2.1
+Name: evadb
+Version: 0.3.1
+Summary: EvaDB AI-Relational Database System
+Home-page: https://github.com/georgia-tech-db/eva
+Download-URL: https://github.com/georgia-tech-db/eva
+Author: Georgia Tech Database Group
+Author-email: arulraj@gatech.edu
+License: Apache License 2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: ray
+Provides-Extra: vision
+Provides-Extra: document
+Provides-Extra: udf
+Provides-Extra: notebook
+Provides-Extra: qdrant
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+# EvaDB: Database System for AI Apps
 
 <div>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
             <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EvaDB on Colab"/>
         </a>
         <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
             <img alt="Slack" src="https://img.shields.io/badge/slack-evadb-ff69b4.svg?logo=slack">
@@ -15,44 +40,44 @@
         </a>
         <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
         <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
         <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
         <a href="https://pepy.tech/project/evadb">
           <img alt="Downloads" src="https://static.pepy.tech/badge/evadb"/>
         </a>
-        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
+        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10|%203.11-brightgreen"/>       
 </div>
 
 <p align="center"> <b><h3>EvaDB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
 
-EvaDB is a database system for developing AI apps. We aim to simplify the development and deployment of AI-powered apps that operate on unstructured data (text documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector index).
+EvaDB is a database system for developing AI apps. We aim to simplify the development and deployment of AI apps that operate on unstructured data (text documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector index).
 
-The high-level Python and SQL APIs allow beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under the Apache license.
+The high-level Python and SQL APIs allow beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under an Apache license.
 
 ## Quick Links
 
 - [Features](#features)
 - [Quick Start](#quick-start)
 - [Documentation](#documentation)
 - [Community and Support](#community-and-support)
 - [Twitter](https://twitter.com/evadb_ai)
 
 ## Features
 
-- 🔮 Build simpler AI-powered applications using Python functions or SQL queries
+- 🔮 Build simpler AI-powered apps using Python functions or SQL queries
 - ⚡️ 10x faster applications using AI-centric query optimization  
-- 💰 Save money spent on GPUs
+- 💰 Save money spent on inference
 - 🚀 First-class support for your custom deep learning models through user-defined functions
 - 📦 Built-in caching to eliminate redundant model invocations across queries
-- ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
+- ⌨️ Integrations for PyTorch, Hugging Face, YOLO, and Open AI models
 - 🐍 Installable via pip and fully implemented in Python
 
 ## Illustrative Applications
 
-Here are some illustrative EvaDB-powered applications (each Jupyter notebook can be opened on Google Colab):
+Here are some illustrative AI apps built using EvaDB (each notebook can be opened on Google Colab):
 
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/13-privategpt.html">PrivateGPT</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">ChatGPT-based Video Question Answering</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html">Querying PDF Documents</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing Traffic Flow with YOLO</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining Emotions of Movie</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation with Hugging Face</a>
@@ -64,51 +89,49 @@
   - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/13-privategpt.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EvaDB. Each notebook includes a link to Google Colab, where you can run the code yourself.
 * [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
 * [Follow us on Twitter](https://twitter.com/evadb_ai)
 * [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
 
 ## Quick Start
 
-- Step 1: Install EvaDB using pip. EvaDB supports Python versions >= `3.8`:
+- Step 1: Install EvaDB using `pip`. EvaDB supports Python versions >= `3.8`:
 
 ```shell
 pip install evadb
 ```
 
-- Step 2: Write your AI app!
+- Step 2: It's time to write an AI app.
 
 ```python
 import evadb
 
-# Grab a EvaDB cursor to load data and run queries
+# Grab a EvaDB cursor to load data into tables and run AI queries
 cursor = evadb.connect().cursor()
 
 # Load a collection of news videos into the 'news_videos' table
-# This command returns a Pandas Dataframe with the query's output
-# In this case, the output indicates the number of loaded videos
+# This function returns a Pandas dataframe with the query's output
+# In this case, the output dataframe indicates the number of loaded videos
 cursor.load(
     file_regex="news_videos/*.mp4",
     format="VIDEO",
     table_name="news_videos"
 ).df()
 
 # Define a function that wraps around your deep learning model
-# Here, this function wraps around an off-the-shelf speech-to-text (Whisper) model
-# Such functions are known as user-defined functions or UDFs
-# So, we are creating a Whisper UDF here
-# After creating the UDF, we can use the function in any query
-cursor.create_udf(
+# Here, this function wraps around a speech-to-text model
+# After registering the function, we can use the registered function in subsequent queries
+cursor.create_function(
     udf_name="SpeechRecognizer",
     type="HuggingFace",
     task='automatic-speech-recognition',
     model='openai/whisper-base'
 ).df()
 
-# EvaDB automatically extract the audio from the video
-# We only need to run the SpeechRecongizer UDF on the 'audio' column
+# EvaDB automatically extracts the audio from the video
+# We only need to run the SpeechRecongizer function on the 'audio' column
 # to get the transcript and persist it in a table called 'transcripts'
 cursor.query(
     """CREATE TABLE transcripts AS
        SELECT SpeechRecognizer(audio) from news_videos;"""
 ).df()
 
 # We next incrementally construct the ChatGPT query using EvaDB's Python API
@@ -119,45 +142,53 @@
 # Since ChatGPT is a built-in function, we don't have to define it
 # We can just directly use it in the query
 # We need to set the OPENAI_KEY as an environment variable
 os.environ["OPENAI_KEY"] = OPENAI_KEY
 query = query.select("ChatGPT('Is this video summary related to LLMs', text)")
 
 # Finally, we run the query to get the results as a dataframe
+# You can then post-process the dataframe using other Python libraries
 response = query.df()
 ```
 
-- **Chain multiple models in a single query to set up useful AI pipelines**
+- **Incrementally build an AI query that chains together multiple models**
+
+Here is a AI query that analyses emotions of actors in an `Interstellar` movie clip using multiple PyTorch models.
 
 ```python
-# Analyse emotions of actors in an Interstellar movie clip using PyTorch models
+# Access the Interstellar movie clip table using a cursor
 query = cursor.table("Interstellar")
 # Get faces using a `FaceDetector` function
 query = query.cross_apply("UNNEST(FaceDetector(data))", "Face(bounding_box, confidence)")
 # Focus only on frames 100 through 200 in the clip
 query = query.filter("id > 100 AND id < 200")
 # Get the emotions of the detected faces using a `EmotionDetector` function
 query = query.select("id, bbox, EmotionDetector(Crop(data, bounding_box))")
 
 # Run the query and get the query result as a dataframe
+# At each of the above steps, you can run the query and see the output
+# If you are familiar with SQL, you can get the SQL query with query.sql_query()
 response = query.df()
 ```
-- **EvaDB runs AI apps 10--100x faster using its AI-centric query optimizer**. Three key built-in optimizations are:
+
+- **EvaDB runs AI apps 10x faster using its AI-centric query optimizer**.
+
+  Three key built-in optimizations are:
 
    💾 **Caching**: EvaDB automatically caches and reuses model inference results.
 
    ⚡️ **Parallel Query Execution**: EvaDB runs the app in parallel on all the available hardware resources (CPUs and GPUs).
 
    🎯 **Model Ordering**: EvaDB optimizes the order in which models are evaluated (e.g., runs the faster, more selective model first).
 
 ## Architecture Diagram
 
 This diagram presents the key components of EvaDB. EvaDB's AI-centric query optimizer takes a query as input and generates a query plan that is executed by the query engine. The query engine hits the relevant storage engines to quickly retrieve the data required for efficiently running the query:
 1. Structured data (SQL database system connected via `sqlalchemy`).
-2. Unstructured media data (on cloud buckets/local filesystem).
+2. Unstructured media data (PDFs, videos, etc. on cloud/local filesystem).
 3. Feature data (vector database system).
 
 <img width="500" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
 
 ## Screenshots
 
 ### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
@@ -208,9 +239,9 @@
 
 EvaDB is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EvaDB are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
 
 For more information, see our
 [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
 
 ## License
-Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
+Copyright (c) 2018--present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
 Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,88 +1,102 @@
-# EvaDB AI-SQL Database System
+Metadata-Version: 2.1 Name: evadb Version: 0.3.1 Summary: EvaDB AI-Relational
+Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
+https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
+Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
+text/markdown Provides-Extra: ray Provides-Extra: vision Provides-Extra:
+document Provides-Extra: udf Provides-Extra: notebook Provides-Extra: qdrant
+Provides-Extra: dev License-File: LICENSE.txt # EvaDB: Database System for AI
+Apps
 [Open_EvaDB_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
 Status] [Downloads] [Python Versions]
 **** EvaDB is a database system for building simpler and faster AI-powered
 applications. ****
 EvaDB is a database system for developing AI apps. We aim to simplify the
-development and deployment of AI-powered apps that operate on unstructured data
-(text documents, videos, PDFs, podcasts, etc.) and structured data (tables,
-vector index). The high-level Python and SQL APIs allow beginners to use EvaDB
-in a few lines of code. Advanced users can define custom user-defined functions
-that wrap around any AI model or Python library. EvaDB is fully implemented in
-Python and licensed under the Apache license. ## Quick Links - [Features]
+development and deployment of AI apps that operate on unstructured data (text
+documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector
+index). The high-level Python and SQL APIs allow beginners to use EvaDB in a
+few lines of code. Advanced users can define custom user-defined functions that
+wrap around any AI model or Python library. EvaDB is fully implemented in
+Python and licensed under an Apache license. ## Quick Links - [Features]
 (#features) - [Quick Start](#quick-start) - [Documentation](#documentation) -
 [Community and Support](#community-and-support) - [Twitter](https://
-twitter.com/evadb_ai) ## Features - ð® Build simpler AI-powered applications
-using Python functions or SQL queries - â¡ï¸ 10x faster applications using
-AI-centric query optimization - ð° Save money spent on GPUs - ð First-
+twitter.com/evadb_ai) ## Features - ð® Build simpler AI-powered apps using
+Python functions or SQL queries - â¡ï¸ 10x faster applications using AI-
+centric query optimization - ð° Save money spent on inference - ð First-
 class support for your custom deep learning models through user-defined
 functions - ð¦ Built-in caching to eliminate redundant model invocations
-across queries - â¨ï¸ First-class support for PyTorch, Hugging Face, YOLO,
-and Open AI models - ð Installable via pip and fully implemented in Python
-## Illustrative Applications Here are some illustrative EvaDB-powered
-applications (each Jupyter notebook can be opened on Google Colab): * ð®
-PrivateGPT * ð® ChatGPT-based_Video_Question_Answering * ð® Querying_PDF
-Documents * ð® Analysing_Traffic_Flow_with_YOLO * ð® Examining_Emotions_of
-Movie * ð® Image_Segmentation_with_Hugging_Face ## Documentation *
-[Documentation](https://evadb.readthedocs.io/) - The Getting_Started page shows
-how you can use EvaDB for different AI tasks and how you can easily extend
-EvaDB to support your custom deep learning model through user-defined
-functions. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EvaDB. Each notebook includes a link
-to Google Colab, where you can run the code yourself. * [Join us on Slack]
-(https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/evadb_ai)
-* [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3) ## Quick Start
-- Step 1: Install EvaDB using pip. EvaDB supports Python versions >= `3.8`:
-```shell pip install evadb ``` - Step 2: Write your AI app! ```python import
-evadb # Grab a EvaDB cursor to load data and run queries cursor = evadb.connect
-().cursor() # Load a collection of news videos into the 'news_videos' table #
-This command returns a Pandas Dataframe with the query's output # In this case,
-the output indicates the number of loaded videos cursor.load
+across queries - â¨ï¸ Integrations for PyTorch, Hugging Face, YOLO, and Open
+AI models - ð Installable via pip and fully implemented in Python ##
+Illustrative Applications Here are some illustrative AI apps built using EvaDB
+(each notebook can be opened on Google Colab): * ð® PrivateGPT * ð®
+ChatGPT-based_Video_Question_Answering * ð® Querying_PDF_Documents * ð®
+Analysing_Traffic_Flow_with_YOLO * ð® Examining_Emotions_of_Movie * ð®
+Image_Segmentation_with_Hugging_Face ## Documentation * [Documentation](https:/
+/evadb.readthedocs.io/) - The Getting_Started page shows how you can use EvaDB
+for different AI tasks and how you can easily extend EvaDB to support your
+custom deep learning model through user-defined functions. - The User_Guides
+section contains Jupyter Notebooks that demonstrate how to use various features
+of EvaDB. Each notebook includes a link to Google Colab, where you can run the
+code yourself. * [Join us on Slack](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter]
+(https://twitter.com/evadb_ai) * [Roadmap](https://github.com/orgs/georgia-
+tech-db/projects/3) ## Quick Start - Step 1: Install EvaDB using `pip`. EvaDB
+supports Python versions >= `3.8`: ```shell pip install evadb ``` - Step 2:
+It's time to write an AI app. ```python import evadb # Grab a EvaDB cursor to
+load data into tables and run AI queries cursor = evadb.connect().cursor() #
+Load a collection of news videos into the 'news_videos' table # This function
+returns a Pandas dataframe with the query's output # In this case, the output
+dataframe indicates the number of loaded videos cursor.load
 ( file_regex="news_videos/*.mp4", format="VIDEO", table_name="news_videos" ).df
 () # Define a function that wraps around your deep learning model # Here, this
-function wraps around an off-the-shelf speech-to-text (Whisper) model # Such
-functions are known as user-defined functions or UDFs # So, we are creating a
-Whisper UDF here # After creating the UDF, we can use the function in any query
-cursor.create_udf( udf_name="SpeechRecognizer", type="HuggingFace",
-task='automatic-speech-recognition', model='openai/whisper-base' ).df() # EvaDB
-automatically extract the audio from the video # We only need to run the
-SpeechRecongizer UDF on the 'audio' column # to get the transcript and persist
-it in a table called 'transcripts' cursor.query( """CREATE TABLE transcripts AS
-SELECT SpeechRecognizer(audio) from news_videos;""" ).df() # We next
-incrementally construct the ChatGPT query using EvaDB's Python API # The query
-is based on the 'transcripts' table # This table has a column called 'text'
-with the transcript text query = cursor.table('transcripts') # Since ChatGPT is
-a built-in function, we don't have to define it # We can just directly use it
-in the query # We need to set the OPENAI_KEY as an environment variable
-os.environ["OPENAI_KEY"] = OPENAI_KEY query = query.select("ChatGPT('Is this
-video summary related to LLMs', text)") # Finally, we run the query to get the
-results as a dataframe response = query.df() ``` - **Chain multiple models in a
-single query to set up useful AI pipelines** ```python # Analyse emotions of
-actors in an Interstellar movie clip using PyTorch models query = cursor.table
-("Interstellar") # Get faces using a `FaceDetector` function query =
-query.cross_apply("UNNEST(FaceDetector(data))", "Face(bounding_box,
-confidence)") # Focus only on frames 100 through 200 in the clip query =
-query.filter("id > 100 AND id < 200") # Get the emotions of the detected faces
-using a `EmotionDetector` function query = query.select("id, bbox,
-EmotionDetector(Crop(data, bounding_box))") # Run the query and get the query
-result as a dataframe response = query.df() ``` - **EvaDB runs AI apps 10--100x
+function wraps around a speech-to-text model # After registering the function,
+we can use the registered function in subsequent queries cursor.create_function
+( udf_name="SpeechRecognizer", type="HuggingFace", task='automatic-speech-
+recognition', model='openai/whisper-base' ).df() # EvaDB automatically extracts
+the audio from the video # We only need to run the SpeechRecongizer function on
+the 'audio' column # to get the transcript and persist it in a table called
+'transcripts' cursor.query( """CREATE TABLE transcripts AS SELECT
+SpeechRecognizer(audio) from news_videos;""" ).df() # We next incrementally
+construct the ChatGPT query using EvaDB's Python API # The query is based on
+the 'transcripts' table # This table has a column called 'text' with the
+transcript text query = cursor.table('transcripts') # Since ChatGPT is a built-
+in function, we don't have to define it # We can just directly use it in the
+query # We need to set the OPENAI_KEY as an environment variable os.environ
+["OPENAI_KEY"] = OPENAI_KEY query = query.select("ChatGPT('Is this video
+summary related to LLMs', text)") # Finally, we run the query to get the
+results as a dataframe # You can then post-process the dataframe using other
+Python libraries response = query.df() ``` - **Incrementally build an AI query
+that chains together multiple models** Here is a AI query that analyses
+emotions of actors in an `Interstellar` movie clip using multiple PyTorch
+models. ```python # Access the Interstellar movie clip table using a cursor
+query = cursor.table("Interstellar") # Get faces using a `FaceDetector`
+function query = query.cross_apply("UNNEST(FaceDetector(data))", "Face
+(bounding_box, confidence)") # Focus only on frames 100 through 200 in the clip
+query = query.filter("id > 100 AND id < 200") # Get the emotions of the
+detected faces using a `EmotionDetector` function query = query.select("id,
+bbox, EmotionDetector(Crop(data, bounding_box))") # Run the query and get the
+query result as a dataframe # At each of the above steps, you can run the query
+and see the output # If you are familiar with SQL, you can get the SQL query
+with query.sql_query() response = query.df() ``` - **EvaDB runs AI apps 10x
 faster using its AI-centric query optimizer**. Three key built-in optimizations
 are: ð¾ **Caching**: EvaDB automatically caches and reuses model inference
 results. â¡ï¸ **Parallel Query Execution**: EvaDB runs the app in parallel on
 all the available hardware resources (CPUs and GPUs). ð¯ **Model Ordering**:
 EvaDB optimizes the order in which models are evaluated (e.g., runs the faster,
 more selective model first). ## Architecture Diagram This diagram presents the
 key components of EvaDB. EvaDB's AI-centric query optimizer takes a query as
 input and generates a query plan that is executed by the query engine. The
 query engine hits the relevant storage engines to quickly retrieve the data
 required for efficiently running the query: 1. Structured data (SQL database
-system connected via `sqlalchemy`). 2. Unstructured media data (on cloud
-buckets/local filesystem). 3. Feature data (vector database system).
+system connected via `sqlalchemy`). 2. Unstructured media data (PDFs, videos,
+etc. on cloud/local filesystem). 3. Feature data (vector database system).
 [Architecture Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
 ---------| |[Source Video] |[Query Result] | ### ð® [PDF Question Answering]
 (https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html)
 (Question Answering Model) | App | |-----| |[Source Video] | ### ð® [MNIST
 Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
@@ -109,10 +123,10 @@
 /circleci.com/gh/georgia-tech-db/eva) [![Documentation Status](https://
 readthedocs.org/projects/evadb/badge/?version=latest)](https://
 evadb.readthedocs.io/en/latest/index.html) EvaDB is the beneficiary of many
 [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
 kinds of contributions to EvaDB are appreciated. To file a bug or to request a
 feature, please use GitHub_issues. Pull_requests are welcome. For more
 information, see our [contribution guide](https://evadb.readthedocs.io/en/
-stable/source/contribute/index.html). ## License Copyright (c) 2018-present
+stable/source/contribute/index.html). ## License Copyright (c) 2018--present
 [Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
 License](LICENSE).
```

### Comparing `evadb-0.3.0/evadb/__init__.py` & `evadb-0.3.1/evadb/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/binder/__init__.py` & `evadb-0.3.1/evadb/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/binder/binder_utils.py` & `evadb-0.3.1/evadb/binder/binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/binder/statement_binder.py` & `evadb-0.3.1/evadb/binder/statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/binder/statement_binder_context.py` & `evadb-0.3.1/evadb/binder/statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/__init__.py` & `evadb-0.3.1/evadb/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/catalog_manager.py` & `evadb-0.3.1/evadb/catalog/catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/catalog_type.py` & `evadb-0.3.1/evadb/catalog/catalog_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/catalog_utils.py` & `evadb-0.3.1/evadb/catalog/catalog_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/__init__.py` & `evadb-0.3.1/evadb/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/association_models.py` & `evadb-0.3.1/evadb/catalog/models/association_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/base_model.py` & `evadb-0.3.1/evadb/catalog/models/base_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/column_catalog.py` & `evadb-0.3.1/evadb/catalog/models/column_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/index_catalog.py` & `evadb-0.3.1/evadb/catalog/models/index_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/table_catalog.py` & `evadb-0.3.1/evadb/catalog/models/table_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/udf_cache_catalog.py` & `evadb-0.3.1/evadb/catalog/models/udf_cache_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/udf_catalog.py` & `evadb-0.3.1/evadb/catalog/models/udf_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/udf_cost_catalog.py` & `evadb-0.3.1/evadb/catalog/models/udf_cost_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/udf_io_catalog.py` & `evadb-0.3.1/evadb/catalog/models/udf_io_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/udf_metadata_catalog.py` & `evadb-0.3.1/evadb/catalog/models/udf_metadata_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/models/utils.py` & `evadb-0.3.1/evadb/catalog/models/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/schema_utils.py` & `evadb-0.3.1/evadb/catalog/schema_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/__init__.py` & `evadb-0.3.1/evadb/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/base_service.py` & `evadb-0.3.1/evadb/catalog/services/base_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/column_catalog_service.py` & `evadb-0.3.1/evadb/catalog/services/column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/index_catalog_service.py` & `evadb-0.3.1/evadb/catalog/services/index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/table_catalog_service.py` & `evadb-0.3.1/evadb/catalog/services/table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/udf_cache_catalog_service.py` & `evadb-0.3.1/evadb/catalog/services/udf_cache_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/udf_catalog_service.py` & `evadb-0.3.1/evadb/catalog/services/udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/udf_cost_catalog_service.py` & `evadb-0.3.1/evadb/catalog/services/udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/udf_io_catalog_service.py` & `evadb-0.3.1/evadb/catalog/services/udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/services/udf_metadata_catalog_service.py` & `evadb-0.3.1/evadb/catalog/services/udf_metadata_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/catalog/sql_config.py` & `evadb-0.3.1/evadb/catalog/sql_config.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/configuration/__init__.py` & `evadb-0.3.1/evadb/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/configuration/bootstrap_environment.py` & `evadb-0.3.1/evadb/configuration/bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/configuration/configuration_manager.py` & `evadb-0.3.1/evadb/configuration/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/configuration/constants.py` & `evadb-0.3.1/evadb/configuration/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/constants.py` & `evadb-0.3.1/evadb/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/database.py` & `evadb-0.3.1/evadb/database.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/evadb.yml` & `evadb-0.3.1/evadb/evadb.yml`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/evadb_cmd_client.py` & `evadb-0.3.1/evadb/evadb_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/evadb_server.py` & `evadb-0.3.1/evadb/evadb_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/__init__.py` & `evadb-0.3.1/evadb/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/abstract_executor.py` & `evadb-0.3.1/evadb/executor/abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/apply_and_merge_executor.py` & `evadb-0.3.1/evadb/executor/apply_and_merge_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/create_executor.py` & `evadb-0.3.1/evadb/executor/create_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/create_index_executor.py` & `evadb-0.3.1/evadb/executor/create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/create_udf_executor.py` & `evadb-0.3.1/evadb/executor/create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/delete_executor.py` & `evadb-0.3.1/evadb/executor/delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/drop_object_executor.py` & `evadb-0.3.1/evadb/executor/drop_object_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/exchange_executor.py` & `evadb-0.3.1/evadb/executor/exchange_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/execution_context.py` & `evadb-0.3.1/evadb/executor/execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/executor_utils.py` & `evadb-0.3.1/evadb/executor/executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/explain_executor.py` & `evadb-0.3.1/evadb/executor/explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/function_scan_executor.py` & `evadb-0.3.1/evadb/executor/function_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/groupby_executor.py` & `evadb-0.3.1/evadb/executor/groupby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/hash_join_executor.py` & `evadb-0.3.1/evadb/executor/hash_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/insert_executor.py` & `evadb-0.3.1/evadb/executor/insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/join_build_executor.py` & `evadb-0.3.1/evadb/executor/join_build_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/lateral_join_executor.py` & `evadb-0.3.1/evadb/executor/lateral_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/limit_executor.py` & `evadb-0.3.1/evadb/executor/limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/load_csv_executor.py` & `evadb-0.3.1/evadb/executor/load_csv_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/load_executor.py` & `evadb-0.3.1/evadb/executor/load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/load_multimedia_executor.py` & `evadb-0.3.1/evadb/executor/load_multimedia_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/nested_loop_join_executor.py` & `evadb-0.3.1/evadb/executor/nested_loop_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/orderby_executor.py` & `evadb-0.3.1/evadb/executor/orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/plan_executor.py` & `evadb-0.3.1/evadb/executor/plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/pp_executor.py` & `evadb-0.3.1/evadb/executor/pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/predicate_executor.py` & `evadb-0.3.1/evadb/executor/predicate_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/project_executor.py` & `evadb-0.3.1/evadb/executor/project_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/ray_utils.py` & `evadb-0.3.1/evadb/executor/ray_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/rename_executor.py` & `evadb-0.3.1/evadb/executor/rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/sample_executor.py` & `evadb-0.3.1/evadb/executor/sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/seq_scan_executor.py` & `evadb-0.3.1/evadb/executor/seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/show_info_executor.py` & `evadb-0.3.1/evadb/executor/show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/storage_executor.py` & `evadb-0.3.1/evadb/executor/storage_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/union_executor.py` & `evadb-0.3.1/evadb/executor/union_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/executor/vector_index_scan_executor.py` & `evadb-0.3.1/evadb/executor/vector_index_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/__init__.py` & `evadb-0.3.1/evadb/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/abstract_expression.py` & `evadb-0.3.1/evadb/expression/abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/aggregation_expression.py` & `evadb-0.3.1/evadb/expression/aggregation_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/arithmetic_expression.py` & `evadb-0.3.1/evadb/expression/arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/comparison_expression.py` & `evadb-0.3.1/evadb/expression/comparison_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/constant_value_expression.py` & `evadb-0.3.1/evadb/expression/constant_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/expression_utils.py` & `evadb-0.3.1/evadb/expression/expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/function_expression.py` & `evadb-0.3.1/evadb/expression/function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/logical_expression.py` & `evadb-0.3.1/evadb/expression/logical_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/expression/tuple_value_expression.py` & `evadb-0.3.1/evadb/expression/tuple_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/interfaces/__init__.py` & `evadb-0.3.1/evadb/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/interfaces/relational/__init__.py` & `evadb-0.3.1/evadb/interfaces/relational/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/interfaces/relational/db.py` & `evadb-0.3.1/evadb/interfaces/relational/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     parse_load,
     parse_query,
     parse_rename,
     parse_show,
     parse_table_clause,
 )
 from evadb.udfs.udf_bootstrap_queries import init_builtin_udfs
-from evadb.utils.generic_utils import is_ray_enabled_and_installed
+from evadb.utils.generic_utils import find_nearest_word, is_ray_enabled_and_installed
 from evadb.utils.logging_manager import logger
 
 
 class EvaDBConnection:
     def __init__(self, evadb: EvaDBDatabase, reader, writer):
         self._reader = reader
         self._writer = writer
@@ -133,14 +133,38 @@
         self._pending_query = False
 
     def __getattr__(self, name):
         """
         Auto generate sync function calls from async
         Sync function calls should not be used in an async environment.
         """
+        function_name_list = [
+            "table",
+            "load",
+            "execute",
+            "query",
+            "create_function",
+            "create_table",
+            "create_vector_index",
+            "drop_table",
+            "drop_function",
+            "drop_index",
+            "df",
+            "show",
+            "insert" "explain",
+            "rename",
+            "fetch_one",
+        ]
+
+        if name not in function_name_list:
+            nearest_function = find_nearest_word(name, function_name_list)
+            raise AttributeError(
+                f"EvaDBCursor does not contain a function named: '{name}'. Did you mean to run: '{nearest_function}()'?"
+            )
+
         try:
             func = object.__getattribute__(self, "%s_async" % name)
         except Exception as e:
             raise e
 
         def func_sync(*args, **kwargs):
             loop = asyncio.get_event_loop()
@@ -211,14 +235,16 @@
         return self._result.frames
 
     def create_vector_index(
         self, index_name: str, table_name: str, expr: str, using: str
     ) -> "EvaDBCursor":
         """
         Creates a vector index using the provided expr on the table.
+        This feature directly works on IMAGE tables.
+        For VIDEO tables, the feature should be extracted first and stored in an intermediate table, before creating the index.
 
         Args:
             index_name (str): Name of the index.
             table_name (str): Name of the table.
             expr (str): Expression used to build the vector index.
             using (str): Method used for indexing, can be `FAISS` or `QDRANT`.
 
@@ -290,29 +316,29 @@
             >>> cursor.drop_table("sample_table", if_exists = True).df()
                 0
             0	Table Successfully dropped: sample_table
         """
         stmt = parse_drop_table(table_name, if_exists)
         return EvaDBQuery(self._evadb, stmt)
 
-    def drop_udf(self, udf_name: str, if_exists: bool = True) -> "EvaDBQuery":
+    def drop_function(self, udf_name: str, if_exists: bool = True) -> "EvaDBQuery":
         """
         Drop a udf in the database.
 
         Args:
             udf_name (str): Name of the udf to be dropped.
             if_exists (bool): If True, do not raise an error if the UDF does not already exist. If False, raise an error.
 
         Returns:
             EvaDBQuery: The EvaDBQuery object representing the DROP UDF.
 
         Examples:
             Drop UDF 'ObjectDetector'
 
-            >>> cursor.drop_udf("ObjectDetector", if_exists = True)
+            >>> cursor.drop_function("ObjectDetector", if_exists = True)
                 0
             0	UDF Successfully dropped: ObjectDetector
         """
         stmt = parse_drop_udf(udf_name, if_exists)
         return EvaDBQuery(self._evadb, stmt)
 
     def drop_index(self, index_name: str, if_exists: bool = True) -> "EvaDBQuery":
@@ -330,21 +356,21 @@
             Drop the index with name 'faiss_index'
 
             >>> cursor.drop_index("faiss_index", if_exists = True)
         """
         stmt = parse_drop_index(index_name, if_exists)
         return EvaDBQuery(self._evadb, stmt)
 
-    def create_udf(
+    def create_function(
         self,
         udf_name: str,
         if_not_exists: bool = True,
         impl_path: str = None,
         type: str = None,
-        **kwargs
+        **kwargs,
     ) -> "EvaDBQuery":
         """
         Create a udf in the database.
 
         Args:
             udf_name (str): Name of the udf to be created.
             if_not_exists (bool): If True, do not raise an error if the UDF already exist. If False, raise an error.
@@ -352,15 +378,15 @@
             type (str): Type of the udf (e.g. HuggingFace).
             **kwargs: Additional keyword arguments for configuring the create udf operation.
 
         Returns:
             EvaDBQuery: The EvaDBQuery object representing the UDF created.
 
         Examples:
-            >>> cursor.create_udf("MnistImageClassifier", if_exists = True, 'mnist_image_classifier.py')
+            >>> cursor.create_function("MnistImageClassifier", if_exists = True, 'mnist_image_classifier.py')
                 0
             0	UDF Successfully created: MnistImageClassifier
         """
         stmt = parse_create_udf(udf_name, if_not_exists, impl_path, type, **kwargs)
         return EvaDBQuery(self._evadb, stmt)
 
     def create_table(
```

### Comparing `evadb-0.3.0/evadb/interfaces/relational/relation.py` & `evadb-0.3.1/evadb/interfaces/relational/relation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/interfaces/relational/utils.py` & `evadb-0.3.1/evadb/interfaces/relational/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/models/__init__.py` & `evadb-0.3.1/evadb/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/models/catalog/__init__.py` & `evadb-0.3.1/evadb/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/models/catalog/frame_info.py` & `evadb-0.3.1/evadb/models/catalog/frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/models/catalog/properties.py` & `evadb-0.3.1/evadb/models/catalog/properties.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/models/server/__init__.py` & `evadb-0.3.1/evadb/models/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/models/server/response.py` & `evadb-0.3.1/evadb/models/server/response.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/models/storage/__init__.py` & `evadb-0.3.1/evadb/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/models/storage/batch.py` & `evadb-0.3.1/evadb/models/storage/batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/__init__.py` & `evadb-0.3.1/evadb/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/binder.py` & `evadb-0.3.1/evadb/optimizer/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/cost_model.py` & `evadb-0.3.1/evadb/optimizer/cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/group.py` & `evadb-0.3.1/evadb/optimizer/group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/group_expression.py` & `evadb-0.3.1/evadb/optimizer/group_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/memo.py` & `evadb-0.3.1/evadb/optimizer/memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/operators.py` & `evadb-0.3.1/evadb/optimizer/operators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/optimizer_context.py` & `evadb-0.3.1/evadb/optimizer/optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/optimizer_task_stack.py` & `evadb-0.3.1/evadb/optimizer/optimizer_task_stack.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/optimizer_tasks.py` & `evadb-0.3.1/evadb/optimizer/optimizer_tasks.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/optimizer_utils.py` & `evadb-0.3.1/evadb/optimizer/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/plan_generator.py` & `evadb-0.3.1/evadb/optimizer/plan_generator.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/property.py` & `evadb-0.3.1/evadb/optimizer/property.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/rules/__init__.py` & `evadb-0.3.1/evadb/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/rules/pattern.py` & `evadb-0.3.1/evadb/optimizer/rules/pattern.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/rules/rules.py` & `evadb-0.3.1/evadb/optimizer/rules/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     extract_pushdown_predicate_for_alias,
     get_expression_execution_cost,
 )
 from evadb.optimizer.rules.pattern import Pattern
 from evadb.optimizer.rules.rules_base import Promise, Rule, RuleType
 from evadb.parser.types import JoinType, ParserOrderBySortType
 from evadb.plan_nodes.apply_and_merge_plan import ApplyAndMergePlan
+from evadb.plan_nodes.create_from_select_plan import CreateFromSelectPlan
 from evadb.plan_nodes.exchange_plan import ExchangePlan
 from evadb.plan_nodes.explain_plan import ExplainPlan
 from evadb.plan_nodes.hash_join_build_plan import HashJoinBuildPlan
 from evadb.plan_nodes.nested_loop_join_plan import NestedLoopJoinPlan
 from evadb.plan_nodes.predicate_plan import PredicatePlan
 from evadb.plan_nodes.project_plan import ProjectPlan
 from evadb.plan_nodes.show_info_plan import ShowInfoPlan
@@ -712,15 +713,17 @@
     def promise(self):
         return Promise.LOGICAL_CREATE_FROM_SELECT_TO_PHYSICAL
 
     def check(self, before: Operator, context: OptimizerContext):
         return True
 
     def apply(self, before: LogicalCreate, context: OptimizerContext):
-        after = CreatePlan(before.video, before.column_list, before.if_not_exists)
+        after = CreateFromSelectPlan(
+            before.video, before.column_list, before.if_not_exists
+        )
         for child in before.children:
             after.append_child(child)
         yield after
 
 
 class LogicalRenameToPhysical(Rule):
     def __init__(self):
```

### Comparing `evadb-0.3.0/evadb/optimizer/rules/rules_base.py` & `evadb-0.3.1/evadb/optimizer/rules/rules_base.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/rules/rules_manager.py` & `evadb-0.3.1/evadb/optimizer/rules/rules_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/optimizer/statement_to_opr_converter.py` & `evadb-0.3.1/evadb/optimizer/statement_to_opr_converter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/__init__.py` & `evadb-0.3.1/evadb/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/alias.py` & `evadb-0.3.1/evadb/parser/alias.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/create_index_statement.py` & `evadb-0.3.1/evadb/parser/create_index_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/create_statement.py` & `evadb-0.3.1/evadb/parser/create_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/create_udf_statement.py` & `evadb-0.3.1/evadb/parser/create_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/delete_statement.py` & `evadb-0.3.1/evadb/parser/delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/drop_object_statement.py` & `evadb-0.3.1/evadb/parser/drop_object_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/evadb.lark` & `evadb-0.3.1/evadb/parser/evadb.lark`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/explain_statement.py` & `evadb-0.3.1/evadb/parser/explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/insert_statement.py` & `evadb-0.3.1/evadb/parser/insert_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_parser.py` & `evadb-0.3.1/evadb/parser/lark_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/__init__.py` & `evadb-0.3.1/evadb/parser/lark_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_common_clauses_ids.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_common_clauses_ids.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_create_statements.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_create_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_delete_statement.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_drop_statement.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_explain_statement.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_expressions.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_expressions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_functions.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_functions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_insert_statements.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_insert_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_load_statement.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_rename_statement.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_select_statement.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_show_statements.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_show_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/lark_visitor/_table_sources.py` & `evadb-0.3.1/evadb/parser/lark_visitor/_table_sources.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/load_statement.py` & `evadb-0.3.1/evadb/parser/load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/parser.py` & `evadb-0.3.1/evadb/parser/parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/rename_statement.py` & `evadb-0.3.1/evadb/parser/rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/select_statement.py` & `evadb-0.3.1/evadb/parser/select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/show_statement.py` & `evadb-0.3.1/evadb/parser/show_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/statement.py` & `evadb-0.3.1/evadb/parser/statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/table_ref.py` & `evadb-0.3.1/evadb/parser/table_ref.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/types.py` & `evadb-0.3.1/evadb/parser/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/parser/utils.py` & `evadb-0.3.1/evadb/parser/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/__init__.py` & `evadb-0.3.1/evadb/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/abstract_join_plan.py` & `evadb-0.3.1/evadb/plan_nodes/abstract_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/abstract_plan.py` & `evadb-0.3.1/evadb/plan_nodes/abstract_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/abstract_scan_plan.py` & `evadb-0.3.1/evadb/plan_nodes/abstract_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/apply_and_merge_plan.py` & `evadb-0.3.1/evadb/plan_nodes/apply_and_merge_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/create_index_plan.py` & `evadb-0.3.1/evadb/plan_nodes/create_index_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/create_plan.py` & `evadb-0.3.1/evadb/plan_nodes/create_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/create_udf_plan.py` & `evadb-0.3.1/evadb/plan_nodes/create_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/delete_plan.py` & `evadb-0.3.1/evadb/plan_nodes/delete_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/drop_object_plan.py` & `evadb-0.3.1/evadb/plan_nodes/drop_object_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/exchange_plan.py` & `evadb-0.3.1/evadb/plan_nodes/exchange_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/explain_plan.py` & `evadb-0.3.1/evadb/plan_nodes/explain_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/function_scan_plan.py` & `evadb-0.3.1/evadb/plan_nodes/function_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/groupby_plan.py` & `evadb-0.3.1/evadb/plan_nodes/groupby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/hash_join_build_plan.py` & `evadb-0.3.1/evadb/plan_nodes/hash_join_build_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/hash_join_probe_plan.py` & `evadb-0.3.1/evadb/plan_nodes/hash_join_probe_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/insert_plan.py` & `evadb-0.3.1/evadb/plan_nodes/insert_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/lateral_join_plan.py` & `evadb-0.3.1/evadb/plan_nodes/lateral_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/limit_plan.py` & `evadb-0.3.1/evadb/plan_nodes/limit_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/load_data_plan.py` & `evadb-0.3.1/evadb/plan_nodes/load_data_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/nested_loop_join_plan.py` & `evadb-0.3.1/evadb/plan_nodes/nested_loop_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/orderby_plan.py` & `evadb-0.3.1/evadb/plan_nodes/orderby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/pp_plan.py` & `evadb-0.3.1/evadb/plan_nodes/pp_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/predicate_plan.py` & `evadb-0.3.1/evadb/plan_nodes/predicate_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/project_plan.py` & `evadb-0.3.1/evadb/plan_nodes/project_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/rename_plan.py` & `evadb-0.3.1/evadb/plan_nodes/rename_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/sample_plan.py` & `evadb-0.3.1/evadb/plan_nodes/sample_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/seq_scan_plan.py` & `evadb-0.3.1/evadb/plan_nodes/seq_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/show_info_plan.py` & `evadb-0.3.1/evadb/plan_nodes/show_info_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/storage_plan.py` & `evadb-0.3.1/evadb/plan_nodes/storage_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/types.py` & `evadb-0.3.1/evadb/plan_nodes/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/union_plan.py` & `evadb-0.3.1/evadb/plan_nodes/union_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/plan_nodes/vector_index_scan_plan.py` & `evadb-0.3.1/evadb/plan_nodes/vector_index_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/__init__.py` & `evadb-0.3.1/evadb/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/abstract_reader.py` & `evadb-0.3.1/evadb/readers/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/csv_reader.py` & `evadb-0.3.1/evadb/readers/csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/decord_reader.py` & `evadb-0.3.1/evadb/readers/decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/document/__init__.py` & `evadb-0.3.1/evadb/readers/document/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/document/document_reader.py` & `evadb-0.3.1/evadb/readers/document/document_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/document/registry.py` & `evadb-0.3.1/evadb/readers/document/registry.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/image/__init__.py` & `evadb-0.3.1/evadb/readers/image/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/image/opencv_image_reader.py` & `evadb-0.3.1/evadb/readers/image/opencv_image_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/readers/pdf_reader.py` & `evadb-0.3.1/evadb/readers/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/server/__init__.py` & `evadb-0.3.1/evadb/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/server/command_handler.py` & `evadb-0.3.1/evadb/server/command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/server/interpreter.py` & `evadb-0.3.1/evadb/server/interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/server/server.py` & `evadb-0.3.1/evadb/server/server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/storage/__init__.py` & `evadb-0.3.1/evadb/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/storage/abstract_media_storage_engine.py` & `evadb-0.3.1/evadb/storage/abstract_media_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/storage/abstract_storage_engine.py` & `evadb-0.3.1/evadb/storage/abstract_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/storage/document_storage_engine.py` & `evadb-0.3.1/evadb/storage/document_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/storage/image_storage_engine.py` & `evadb-0.3.1/evadb/storage/image_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/storage/pdf_storage_engine.py` & `evadb-0.3.1/evadb/storage/pdf_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/storage/sqlite_storage_engine.py` & `evadb-0.3.1/evadb/storage/sqlite_storage_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,22 +55,22 @@
                 # Sqlalchemy does not consume numpy generic data types
                 # convert numpy datatype to python generic datatype using tolist()
                 # eg. np.int64 -> int
                 # https://stackoverflow.com/a/53067954
                 dict_row[col.name] = dict_row[col.name].tolist()
         return dict_row
 
-    def _sql_row_to_dict(self, sql_row: tuple, columns: List[ColumnCatalogEntry]):
+    def _deserialize_sql_row(self, sql_row: dict, columns: List[ColumnCatalogEntry]):
         # Deserialize numpy data
         dict_row = {}
         for idx, col in enumerate(columns):
             if col.type == ColumnType.NDARRAY:
-                dict_row[col.name] = self._serializer.deserialize(sql_row[idx])
+                dict_row[col.name] = self._serializer.deserialize(sql_row[col.name])
             else:
-                dict_row[col.name] = sql_row[idx]
+                dict_row[col.name] = sql_row[col.name]
         return dict_row
 
     def _try_loading_table_via_reflection(self, table_name: str):
         metadata_obj = BaseModel.metadata
         if table_name in metadata_obj.tables:
             return metadata_obj.tables[table_name]
         # reflection
@@ -173,22 +173,23 @@
             table: table metadata object of the table to read
             batch_mem_size (int): memory size of the batch read from storage
         Return:
             Iterator of Batch read.
         """
         try:
             table_to_read = self._try_loading_table_via_reflection(table.name)
-            result = self._sql_engine.execute(table_to_read.select())
+            result = self._sql_session.execute(table_to_read.select())
             data_batch = []
             row_size = None
             for row in result:
-                # Todo: Verify the order of columns in row matches the table.columns
                 # For table read, we provide row_id so that user can also retrieve
                 # row_id from the table.
-                data_batch.append(self._sql_row_to_dict(row, table.columns))
+                data_batch.append(
+                    self._deserialize_sql_row(row._asdict(), table.columns)
+                )
                 if row_size is None:
                     row_size = 0
                     row_size = get_size(data_batch)
                 if len(data_batch) * row_size >= batch_mem_size:
                     yield Batch(pd.DataFrame(data_batch))
                     data_batch = []
             if data_batch:
@@ -196,27 +197,27 @@
 
         except Exception as e:
             err_msg = f"Failed to read the table {table.name} with exception {str(e)}"
             logger.exception(err_msg)
             raise Exception(err_msg)
 
     def delete(
-        self, table: TableCatalogEntry, sqlalchemy_filter_clause: ColumnElement[bool]
+        self, table: TableCatalogEntry, sqlalchemy_filter_clause: "ColumnElement[bool]"
     ):
         """Delete tuples from the table where rows satisfy the where_clause.
         The current implementation only handles equality predicates.
 
         Argument:
             table: table metadata object of the table
             where_clause: clause used to find the tuples to remove.
         """
         try:
             table_to_delete_from = self._try_loading_table_via_reflection(table.name)
             d = table_to_delete_from.delete().where(sqlalchemy_filter_clause)
-            self._sql_engine.execute(d)
+            self._sql_session.execute(d)
             self._sql_session.commit()
         except Exception as e:
             err_msg = (
                 f"Failed to delete from the table {table.name} with exception {str(e)}"
             )
             logger.exception(err_msg)
             raise Exception(err_msg)
```

### Comparing `evadb-0.3.0/evadb/storage/storage_engine.py` & `evadb-0.3.1/evadb/storage/storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/storage/video_storage_engine.py` & `evadb-0.3.1/evadb/storage/video_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/__init__.py` & `evadb-0.3.1/evadb/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/huggingface/__init__.py` & `evadb-0.3.1/evadb/third_party/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/huggingface/binder.py` & `evadb-0.3.1/evadb/third_party/huggingface/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/huggingface/create.py` & `evadb-0.3.1/evadb/third_party/huggingface/create.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/huggingface/model.py` & `evadb-0.3.1/evadb/third_party/huggingface/model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/vector_stores/__init__.py` & `evadb-0.3.1/evadb/third_party/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/vector_stores/faiss.py` & `evadb-0.3.1/evadb/third_party/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/vector_stores/qdrant.py` & `evadb-0.3.1/evadb/third_party/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/vector_stores/types.py` & `evadb-0.3.1/evadb/third_party/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/third_party/vector_stores/utils.py` & `evadb-0.3.1/evadb/third_party/vector_stores/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/__init__.py` & `evadb-0.3.1/evadb/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/abstract/__init__.py` & `evadb-0.3.1/evadb/udfs/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/abstract/abstract_udf.py` & `evadb-0.3.1/evadb/udfs/abstract/abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/abstract/hf_abstract_udf.py` & `evadb-0.3.1/evadb/udfs/abstract/hf_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/abstract/pytorch_abstract_udf.py` & `evadb-0.3.1/evadb/udfs/abstract/pytorch_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/abstract/tracker_abstract_udf.py` & `evadb-0.3.1/evadb/udfs/abstract/tracker_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/asl_action_recognition.py` & `evadb-0.3.1/evadb/udfs/asl_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/decorators/__init__.py` & `evadb-0.3.1/evadb/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/decorators/decorators.py` & `evadb-0.3.1/evadb/udfs/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.3.1/evadb/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/decorators/io_descriptors/abstract_types.py` & `evadb-0.3.1/evadb/udfs/decorators/io_descriptors/abstract_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/decorators/io_descriptors/data_types.py` & `evadb-0.3.1/evadb/udfs/decorators/io_descriptors/data_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/decorators/utils.py` & `evadb-0.3.1/evadb/udfs/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/emotion_detector.py` & `evadb-0.3.1/evadb/udfs/emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/face_detector.py` & `evadb-0.3.1/evadb/udfs/face_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/fastrcnn_object_detector.py` & `evadb-0.3.1/evadb/udfs/fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/feature_extractor.py` & `evadb-0.3.1/evadb/udfs/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/fuzzy_join.py` & `evadb-0.3.1/evadb/udfs/fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/gpu_compatible.py` & `evadb-0.3.1/evadb/udfs/gpu_compatible.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/mnist_image_classifier.py` & `evadb-0.3.1/evadb/udfs/mnist_image_classifier.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/mvit_action_recognition.py` & `evadb-0.3.1/evadb/udfs/mvit_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/__init__.py` & `evadb-0.3.1/evadb/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/annotate.py` & `evadb-0.3.1/evadb/udfs/ndarray/annotate.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/array_count.py` & `evadb-0.3.1/evadb/udfs/ndarray/array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/crop.py` & `evadb-0.3.1/evadb/udfs/ndarray/crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/fuzzy_join.py` & `evadb-0.3.1/evadb/udfs/ndarray/fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/gaussian_blur.py` & `evadb-0.3.1/evadb/udfs/ndarray/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/horizontal_flip.py` & `evadb-0.3.1/evadb/udfs/ndarray/horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/open.py` & `evadb-0.3.1/evadb/udfs/ndarray/open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/similarity.py` & `evadb-0.3.1/evadb/udfs/ndarray/similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/to_grayscale.py` & `evadb-0.3.1/evadb/udfs/ndarray/to_grayscale.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/ndarray/vertical_flip.py` & `evadb-0.3.1/evadb/udfs/ndarray/vertical_flip.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/saliency_feature_extractor.py` & `evadb-0.3.1/evadb/udfs/saliency_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/sentence_feature_extractor.py` & `evadb-0.3.1/evadb/udfs/sentence_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/sift_feature_extractor.py` & `evadb-0.3.1/evadb/udfs/sift_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/text_filter_keyword.py` & `evadb-0.3.1/evadb/udfs/text_filter_keyword.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/trackers/__init__.py` & `evadb-0.3.1/evadb/udfs/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/trackers/nor_fair.py` & `evadb-0.3.1/evadb/udfs/trackers/nor_fair.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/udf_bootstrap_queries.py` & `evadb-0.3.1/evadb/udfs/udf_bootstrap_queries.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/udfs/yolo_object_detector.py` & `evadb-0.3.1/evadb/udfs/yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/utils/__init__.py` & `evadb-0.3.1/evadb/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/utils/errors.py` & `evadb-0.3.1/evadb/utils/errors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/utils/generic_utils.py` & `evadb-0.3.1/evadb/utils/generic_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,23 @@
                     os.unlink(file_path)
                 elif os.path.isdir(file_path):
                     shutil.rmtree(file_path)
             except Exception as e:
                 logger.warning(f"Failed to delete {file_path}. Reason: {str(e)}")
 
 
+def find_nearest_word(word, word_list):
+    from thefuzz import process
+
+    nearest_word_and_score = process.extractOne(word, word_list)
+    nearest_word = nearest_word_and_score[0]
+
+    return nearest_word
+
+
 ##############################
 ## TRY TO IMPORT PACKAGES
 ##############################
 
 
 def try_to_import_ray():
     try:
```

### Comparing `evadb-0.3.0/evadb/utils/kv_cache.py` & `evadb-0.3.1/evadb/utils/kv_cache.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/utils/logging_manager.py` & `evadb-0.3.1/evadb/utils/logging_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/utils/math_utils.py` & `evadb-0.3.1/evadb/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/utils/s3_utils.py` & `evadb-0.3.1/evadb/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb/utils/stats.py` & `evadb-0.3.1/evadb/utils/stats.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/evadb.egg-info/PKG-INFO` & `evadb-0.3.1/evadb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.3.0
+Version: 0.3.1
 Summary: EvaDB AI-Relational Database System
 Home-page: https://github.com/georgia-tech-db/eva
 Download-URL: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Provides-Extra: document
 Provides-Extra: udf
 Provides-Extra: notebook
 Provides-Extra: qdrant
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# EvaDB AI-SQL Database System
+# EvaDB: Database System for AI Apps
 
 <div>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
             <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EvaDB on Colab"/>
         </a>
         <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
             <img alt="Slack" src="https://img.shields.io/badge/slack-evadb-ff69b4.svg?logo=slack">
@@ -40,44 +40,44 @@
         </a>
         <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
         <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
         <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
         <a href="https://pepy.tech/project/evadb">
           <img alt="Downloads" src="https://static.pepy.tech/badge/evadb"/>
         </a>
-        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
+        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10|%203.11-brightgreen"/>       
 </div>
 
 <p align="center"> <b><h3>EvaDB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
 
-EvaDB is a database system for developing AI apps. We aim to simplify the development and deployment of AI-powered apps that operate on unstructured data (text documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector index).
+EvaDB is a database system for developing AI apps. We aim to simplify the development and deployment of AI apps that operate on unstructured data (text documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector index).
 
-The high-level Python and SQL APIs allow beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under the Apache license.
+The high-level Python and SQL APIs allow beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under an Apache license.
 
 ## Quick Links
 
 - [Features](#features)
 - [Quick Start](#quick-start)
 - [Documentation](#documentation)
 - [Community and Support](#community-and-support)
 - [Twitter](https://twitter.com/evadb_ai)
 
 ## Features
 
-- 🔮 Build simpler AI-powered applications using Python functions or SQL queries
+- 🔮 Build simpler AI-powered apps using Python functions or SQL queries
 - ⚡️ 10x faster applications using AI-centric query optimization  
-- 💰 Save money spent on GPUs
+- 💰 Save money spent on inference
 - 🚀 First-class support for your custom deep learning models through user-defined functions
 - 📦 Built-in caching to eliminate redundant model invocations across queries
-- ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
+- ⌨️ Integrations for PyTorch, Hugging Face, YOLO, and Open AI models
 - 🐍 Installable via pip and fully implemented in Python
 
 ## Illustrative Applications
 
-Here are some illustrative EvaDB-powered applications (each Jupyter notebook can be opened on Google Colab):
+Here are some illustrative AI apps built using EvaDB (each notebook can be opened on Google Colab):
 
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/13-privategpt.html">PrivateGPT</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">ChatGPT-based Video Question Answering</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html">Querying PDF Documents</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing Traffic Flow with YOLO</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining Emotions of Movie</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation with Hugging Face</a>
@@ -89,51 +89,49 @@
   - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/13-privategpt.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EvaDB. Each notebook includes a link to Google Colab, where you can run the code yourself.
 * [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
 * [Follow us on Twitter](https://twitter.com/evadb_ai)
 * [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
 
 ## Quick Start
 
-- Step 1: Install EvaDB using pip. EvaDB supports Python versions >= `3.8`:
+- Step 1: Install EvaDB using `pip`. EvaDB supports Python versions >= `3.8`:
 
 ```shell
 pip install evadb
 ```
 
-- Step 2: Write your AI app!
+- Step 2: It's time to write an AI app.
 
 ```python
 import evadb
 
-# Grab a EvaDB cursor to load data and run queries
+# Grab a EvaDB cursor to load data into tables and run AI queries
 cursor = evadb.connect().cursor()
 
 # Load a collection of news videos into the 'news_videos' table
-# This command returns a Pandas Dataframe with the query's output
-# In this case, the output indicates the number of loaded videos
+# This function returns a Pandas dataframe with the query's output
+# In this case, the output dataframe indicates the number of loaded videos
 cursor.load(
     file_regex="news_videos/*.mp4",
     format="VIDEO",
     table_name="news_videos"
 ).df()
 
 # Define a function that wraps around your deep learning model
-# Here, this function wraps around an off-the-shelf speech-to-text (Whisper) model
-# Such functions are known as user-defined functions or UDFs
-# So, we are creating a Whisper UDF here
-# After creating the UDF, we can use the function in any query
-cursor.create_udf(
+# Here, this function wraps around a speech-to-text model
+# After registering the function, we can use the registered function in subsequent queries
+cursor.create_function(
     udf_name="SpeechRecognizer",
     type="HuggingFace",
     task='automatic-speech-recognition',
     model='openai/whisper-base'
 ).df()
 
-# EvaDB automatically extract the audio from the video
-# We only need to run the SpeechRecongizer UDF on the 'audio' column
+# EvaDB automatically extracts the audio from the video
+# We only need to run the SpeechRecongizer function on the 'audio' column
 # to get the transcript and persist it in a table called 'transcripts'
 cursor.query(
     """CREATE TABLE transcripts AS
        SELECT SpeechRecognizer(audio) from news_videos;"""
 ).df()
 
 # We next incrementally construct the ChatGPT query using EvaDB's Python API
@@ -144,45 +142,53 @@
 # Since ChatGPT is a built-in function, we don't have to define it
 # We can just directly use it in the query
 # We need to set the OPENAI_KEY as an environment variable
 os.environ["OPENAI_KEY"] = OPENAI_KEY
 query = query.select("ChatGPT('Is this video summary related to LLMs', text)")
 
 # Finally, we run the query to get the results as a dataframe
+# You can then post-process the dataframe using other Python libraries
 response = query.df()
 ```
 
-- **Chain multiple models in a single query to set up useful AI pipelines**
+- **Incrementally build an AI query that chains together multiple models**
+
+Here is a AI query that analyses emotions of actors in an `Interstellar` movie clip using multiple PyTorch models.
 
 ```python
-# Analyse emotions of actors in an Interstellar movie clip using PyTorch models
+# Access the Interstellar movie clip table using a cursor
 query = cursor.table("Interstellar")
 # Get faces using a `FaceDetector` function
 query = query.cross_apply("UNNEST(FaceDetector(data))", "Face(bounding_box, confidence)")
 # Focus only on frames 100 through 200 in the clip
 query = query.filter("id > 100 AND id < 200")
 # Get the emotions of the detected faces using a `EmotionDetector` function
 query = query.select("id, bbox, EmotionDetector(Crop(data, bounding_box))")
 
 # Run the query and get the query result as a dataframe
+# At each of the above steps, you can run the query and see the output
+# If you are familiar with SQL, you can get the SQL query with query.sql_query()
 response = query.df()
 ```
-- **EvaDB runs AI apps 10--100x faster using its AI-centric query optimizer**. Three key built-in optimizations are:
+
+- **EvaDB runs AI apps 10x faster using its AI-centric query optimizer**.
+
+  Three key built-in optimizations are:
 
    💾 **Caching**: EvaDB automatically caches and reuses model inference results.
 
    ⚡️ **Parallel Query Execution**: EvaDB runs the app in parallel on all the available hardware resources (CPUs and GPUs).
 
    🎯 **Model Ordering**: EvaDB optimizes the order in which models are evaluated (e.g., runs the faster, more selective model first).
 
 ## Architecture Diagram
 
 This diagram presents the key components of EvaDB. EvaDB's AI-centric query optimizer takes a query as input and generates a query plan that is executed by the query engine. The query engine hits the relevant storage engines to quickly retrieve the data required for efficiently running the query:
 1. Structured data (SQL database system connected via `sqlalchemy`).
-2. Unstructured media data (on cloud buckets/local filesystem).
+2. Unstructured media data (PDFs, videos, etc. on cloud/local filesystem).
 3. Feature data (vector database system).
 
 <img width="500" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
 
 ## Screenshots
 
 ### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
@@ -233,9 +239,9 @@
 
 EvaDB is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EvaDB are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
 
 For more information, see our
 [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
 
 ## License
-Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
+Copyright (c) 2018--present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
 Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,98 +1,102 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.3.0 Summary: EvaDB AI-Relational
+Metadata-Version: 2.1 Name: evadb Version: 0.3.1 Summary: EvaDB AI-Relational
 Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
 https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: ray Provides-Extra: vision Provides-Extra:
 document Provides-Extra: udf Provides-Extra: notebook Provides-Extra: qdrant
-Provides-Extra: dev License-File: LICENSE.txt # EvaDB AI-SQL Database System
+Provides-Extra: dev License-File: LICENSE.txt # EvaDB: Database System for AI
+Apps
 [Open_EvaDB_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
 Status] [Downloads] [Python Versions]
 **** EvaDB is a database system for building simpler and faster AI-powered
 applications. ****
 EvaDB is a database system for developing AI apps. We aim to simplify the
-development and deployment of AI-powered apps that operate on unstructured data
-(text documents, videos, PDFs, podcasts, etc.) and structured data (tables,
-vector index). The high-level Python and SQL APIs allow beginners to use EvaDB
-in a few lines of code. Advanced users can define custom user-defined functions
-that wrap around any AI model or Python library. EvaDB is fully implemented in
-Python and licensed under the Apache license. ## Quick Links - [Features]
+development and deployment of AI apps that operate on unstructured data (text
+documents, videos, PDFs, podcasts, etc.) and structured data (tables, vector
+index). The high-level Python and SQL APIs allow beginners to use EvaDB in a
+few lines of code. Advanced users can define custom user-defined functions that
+wrap around any AI model or Python library. EvaDB is fully implemented in
+Python and licensed under an Apache license. ## Quick Links - [Features]
 (#features) - [Quick Start](#quick-start) - [Documentation](#documentation) -
 [Community and Support](#community-and-support) - [Twitter](https://
-twitter.com/evadb_ai) ## Features - ð® Build simpler AI-powered applications
-using Python functions or SQL queries - â¡ï¸ 10x faster applications using
-AI-centric query optimization - ð° Save money spent on GPUs - ð First-
+twitter.com/evadb_ai) ## Features - ð® Build simpler AI-powered apps using
+Python functions or SQL queries - â¡ï¸ 10x faster applications using AI-
+centric query optimization - ð° Save money spent on inference - ð First-
 class support for your custom deep learning models through user-defined
 functions - ð¦ Built-in caching to eliminate redundant model invocations
-across queries - â¨ï¸ First-class support for PyTorch, Hugging Face, YOLO,
-and Open AI models - ð Installable via pip and fully implemented in Python
-## Illustrative Applications Here are some illustrative EvaDB-powered
-applications (each Jupyter notebook can be opened on Google Colab): * ð®
-PrivateGPT * ð® ChatGPT-based_Video_Question_Answering * ð® Querying_PDF
-Documents * ð® Analysing_Traffic_Flow_with_YOLO * ð® Examining_Emotions_of
-Movie * ð® Image_Segmentation_with_Hugging_Face ## Documentation *
-[Documentation](https://evadb.readthedocs.io/) - The Getting_Started page shows
-how you can use EvaDB for different AI tasks and how you can easily extend
-EvaDB to support your custom deep learning model through user-defined
-functions. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EvaDB. Each notebook includes a link
-to Google Colab, where you can run the code yourself. * [Join us on Slack]
-(https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/evadb_ai)
-* [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3) ## Quick Start
-- Step 1: Install EvaDB using pip. EvaDB supports Python versions >= `3.8`:
-```shell pip install evadb ``` - Step 2: Write your AI app! ```python import
-evadb # Grab a EvaDB cursor to load data and run queries cursor = evadb.connect
-().cursor() # Load a collection of news videos into the 'news_videos' table #
-This command returns a Pandas Dataframe with the query's output # In this case,
-the output indicates the number of loaded videos cursor.load
+across queries - â¨ï¸ Integrations for PyTorch, Hugging Face, YOLO, and Open
+AI models - ð Installable via pip and fully implemented in Python ##
+Illustrative Applications Here are some illustrative AI apps built using EvaDB
+(each notebook can be opened on Google Colab): * ð® PrivateGPT * ð®
+ChatGPT-based_Video_Question_Answering * ð® Querying_PDF_Documents * ð®
+Analysing_Traffic_Flow_with_YOLO * ð® Examining_Emotions_of_Movie * ð®
+Image_Segmentation_with_Hugging_Face ## Documentation * [Documentation](https:/
+/evadb.readthedocs.io/) - The Getting_Started page shows how you can use EvaDB
+for different AI tasks and how you can easily extend EvaDB to support your
+custom deep learning model through user-defined functions. - The User_Guides
+section contains Jupyter Notebooks that demonstrate how to use various features
+of EvaDB. Each notebook includes a link to Google Colab, where you can run the
+code yourself. * [Join us on Slack](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter]
+(https://twitter.com/evadb_ai) * [Roadmap](https://github.com/orgs/georgia-
+tech-db/projects/3) ## Quick Start - Step 1: Install EvaDB using `pip`. EvaDB
+supports Python versions >= `3.8`: ```shell pip install evadb ``` - Step 2:
+It's time to write an AI app. ```python import evadb # Grab a EvaDB cursor to
+load data into tables and run AI queries cursor = evadb.connect().cursor() #
+Load a collection of news videos into the 'news_videos' table # This function
+returns a Pandas dataframe with the query's output # In this case, the output
+dataframe indicates the number of loaded videos cursor.load
 ( file_regex="news_videos/*.mp4", format="VIDEO", table_name="news_videos" ).df
 () # Define a function that wraps around your deep learning model # Here, this
-function wraps around an off-the-shelf speech-to-text (Whisper) model # Such
-functions are known as user-defined functions or UDFs # So, we are creating a
-Whisper UDF here # After creating the UDF, we can use the function in any query
-cursor.create_udf( udf_name="SpeechRecognizer", type="HuggingFace",
-task='automatic-speech-recognition', model='openai/whisper-base' ).df() # EvaDB
-automatically extract the audio from the video # We only need to run the
-SpeechRecongizer UDF on the 'audio' column # to get the transcript and persist
-it in a table called 'transcripts' cursor.query( """CREATE TABLE transcripts AS
-SELECT SpeechRecognizer(audio) from news_videos;""" ).df() # We next
-incrementally construct the ChatGPT query using EvaDB's Python API # The query
-is based on the 'transcripts' table # This table has a column called 'text'
-with the transcript text query = cursor.table('transcripts') # Since ChatGPT is
-a built-in function, we don't have to define it # We can just directly use it
-in the query # We need to set the OPENAI_KEY as an environment variable
-os.environ["OPENAI_KEY"] = OPENAI_KEY query = query.select("ChatGPT('Is this
-video summary related to LLMs', text)") # Finally, we run the query to get the
-results as a dataframe response = query.df() ``` - **Chain multiple models in a
-single query to set up useful AI pipelines** ```python # Analyse emotions of
-actors in an Interstellar movie clip using PyTorch models query = cursor.table
-("Interstellar") # Get faces using a `FaceDetector` function query =
-query.cross_apply("UNNEST(FaceDetector(data))", "Face(bounding_box,
-confidence)") # Focus only on frames 100 through 200 in the clip query =
-query.filter("id > 100 AND id < 200") # Get the emotions of the detected faces
-using a `EmotionDetector` function query = query.select("id, bbox,
-EmotionDetector(Crop(data, bounding_box))") # Run the query and get the query
-result as a dataframe response = query.df() ``` - **EvaDB runs AI apps 10--100x
+function wraps around a speech-to-text model # After registering the function,
+we can use the registered function in subsequent queries cursor.create_function
+( udf_name="SpeechRecognizer", type="HuggingFace", task='automatic-speech-
+recognition', model='openai/whisper-base' ).df() # EvaDB automatically extracts
+the audio from the video # We only need to run the SpeechRecongizer function on
+the 'audio' column # to get the transcript and persist it in a table called
+'transcripts' cursor.query( """CREATE TABLE transcripts AS SELECT
+SpeechRecognizer(audio) from news_videos;""" ).df() # We next incrementally
+construct the ChatGPT query using EvaDB's Python API # The query is based on
+the 'transcripts' table # This table has a column called 'text' with the
+transcript text query = cursor.table('transcripts') # Since ChatGPT is a built-
+in function, we don't have to define it # We can just directly use it in the
+query # We need to set the OPENAI_KEY as an environment variable os.environ
+["OPENAI_KEY"] = OPENAI_KEY query = query.select("ChatGPT('Is this video
+summary related to LLMs', text)") # Finally, we run the query to get the
+results as a dataframe # You can then post-process the dataframe using other
+Python libraries response = query.df() ``` - **Incrementally build an AI query
+that chains together multiple models** Here is a AI query that analyses
+emotions of actors in an `Interstellar` movie clip using multiple PyTorch
+models. ```python # Access the Interstellar movie clip table using a cursor
+query = cursor.table("Interstellar") # Get faces using a `FaceDetector`
+function query = query.cross_apply("UNNEST(FaceDetector(data))", "Face
+(bounding_box, confidence)") # Focus only on frames 100 through 200 in the clip
+query = query.filter("id > 100 AND id < 200") # Get the emotions of the
+detected faces using a `EmotionDetector` function query = query.select("id,
+bbox, EmotionDetector(Crop(data, bounding_box))") # Run the query and get the
+query result as a dataframe # At each of the above steps, you can run the query
+and see the output # If you are familiar with SQL, you can get the SQL query
+with query.sql_query() response = query.df() ``` - **EvaDB runs AI apps 10x
 faster using its AI-centric query optimizer**. Three key built-in optimizations
 are: ð¾ **Caching**: EvaDB automatically caches and reuses model inference
 results. â¡ï¸ **Parallel Query Execution**: EvaDB runs the app in parallel on
 all the available hardware resources (CPUs and GPUs). ð¯ **Model Ordering**:
 EvaDB optimizes the order in which models are evaluated (e.g., runs the faster,
 more selective model first). ## Architecture Diagram This diagram presents the
 key components of EvaDB. EvaDB's AI-centric query optimizer takes a query as
 input and generates a query plan that is executed by the query engine. The
 query engine hits the relevant storage engines to quickly retrieve the data
 required for efficiently running the query: 1. Structured data (SQL database
-system connected via `sqlalchemy`). 2. Unstructured media data (on cloud
-buckets/local filesystem). 3. Feature data (vector database system).
+system connected via `sqlalchemy`). 2. Unstructured media data (PDFs, videos,
+etc. on cloud/local filesystem). 3. Feature data (vector database system).
 [Architecture Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
 ---------| |[Source Video] |[Query Result] | ### ð® [PDF Question Answering]
 (https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html)
 (Question Answering Model) | App | |-----| |[Source Video] | ### ð® [MNIST
 Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
@@ -119,10 +123,10 @@
 /circleci.com/gh/georgia-tech-db/eva) [![Documentation Status](https://
 readthedocs.org/projects/evadb/badge/?version=latest)](https://
 evadb.readthedocs.io/en/latest/index.html) EvaDB is the beneficiary of many
 [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
 kinds of contributions to EvaDB are appreciated. To file a bug or to request a
 feature, please use GitHub_issues. Pull_requests are welcome. For more
 information, see our [contribution guide](https://evadb.readthedocs.io/en/
-stable/source/contribute/index.html). ## License Copyright (c) 2018-present
+stable/source/contribute/index.html). ## License Copyright (c) 2018--present
 [Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
 License](LICENSE).
```

### Comparing `evadb-0.3.0/evadb.egg-info/SOURCES.txt` & `evadb-0.3.1/evadb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 evadb/parser/lark_visitor/_show_statements.py
 evadb/parser/lark_visitor/_table_sources.py
 evadb/plan_nodes/__init__.py
 evadb/plan_nodes/abstract_join_plan.py
 evadb/plan_nodes/abstract_plan.py
 evadb/plan_nodes/abstract_scan_plan.py
 evadb/plan_nodes/apply_and_merge_plan.py
+evadb/plan_nodes/create_from_select_plan.py
 evadb/plan_nodes/create_index_plan.py
 evadb/plan_nodes/create_plan.py
 evadb/plan_nodes/create_udf_plan.py
 evadb/plan_nodes/delete_plan.py
 evadb/plan_nodes/drop_object_plan.py
 evadb/plan_nodes/exchange_plan.py
 evadb/plan_nodes/explain_plan.py
```

### Comparing `evadb-0.3.0/evadb.egg-info/requires.txt` & `evadb-0.3.1/evadb.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 numpy>=1.19.5
 pandas>=1.1.5
-sqlalchemy<2.0.0,>=1.4.0
+sqlalchemy>=2.0.0
 sqlalchemy-utils>=0.36.6
 lark>=1.0.0
 pyyaml>=5.1
 aenum>=2.2.0
 diskcache>=5.4.0
 retry>=0.9.2
 psutil
+thefuzz
 
 [dev]
 pytest>=6.1.2
 pytest-cov>=2.11.1
 mock
 coveralls>=3.0.1
 moto[s3]>=4.1.1
@@ -41,15 +42,14 @@
 pdfminer.six
 sentence-transformers
 protobuf<=3.20.1
 bs4
 openai>=0.27.4
 gpt4all
 facenet-pytorch>=2.5.2
-thefuzz
 pytube
 youtube-transcript-api
 boto3
 norfair>=2.2.0
 kornia
 ipython<8.13.0
 ipywidgets>=7.7.2
@@ -81,15 +81,14 @@
 qdrant_client
 
 [ray]
 ray<2.5.0,>=1.13.0
 
 [udf]
 facenet-pytorch>=2.5.2
-thefuzz
 pytube
 youtube-transcript-api
 boto3
 norfair>=2.2.0
 kornia
 
 [vision]
```

### Comparing `evadb-0.3.0/setup.py` & `evadb-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,23 @@
 DOWNLOAD_URL = "https://github.com/georgia-tech-db/eva"
 LICENSE = "Apache License 2.0"
 VERSION = VERSION_DICT["VERSION"]
 
 minimal_requirements = [
     "numpy>=1.19.5",
     "pandas>=1.1.5",
-    "sqlalchemy>=1.4.0,<2.0.0",  # BREAKING CHANGES IN 2.0.0
+    "sqlalchemy>=2.0.0",
     "sqlalchemy-utils>=0.36.6",
     "lark>=1.0.0",
     "pyyaml>=5.1",
     "aenum>=2.2.0",
     "diskcache>=5.4.0",
     "retry>=0.9.2",
     "psutil",
+    "thefuzz"
 ]
 
 vision_libs = [
     "torch>=1.10.0",
     "torchvision>=0.11.1",
     "transformers>=4.27.4,<4.30.2",  # HUGGINGFACE
     "faiss-cpu",  # DEFAULT VECTOR INDEX
@@ -80,15 +81,14 @@
     "openai>=0.27.4",  # CHATGPT
     "gpt4all",  # PRIVATE GPT
     "sentencepiece",  # TRANSFORMERS
 ]
 
 udf_libs = [
     "facenet-pytorch>=2.5.2",  # FACE DETECTION
-    "thefuzz",  # FUZZY STRING MATCHING
     "pytube",  # YOUTUBE QA APP
     "youtube-transcript-api",  # YOUTUBE QA APP
     "boto3",  # AWS
     "norfair>=2.2.0",  # OBJECT TRACKING
     "kornia",  # SIFT FEATURES
 ]
```

### Comparing `evadb-0.3.0/test/__init__.py` & `evadb-0.3.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/app_tests/__init__.py` & `evadb-0.3.1/test/app_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/app_tests/test_pandas_qa.py` & `evadb-0.3.1/test/app_tests/test_pandas_qa.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import subprocess
 import unittest
 from pathlib import Path
+from test.markers import chatgpt_skip_marker
 from test.util import get_evadb_for_testing, shutdown_ray
 
 
 class PandasQATest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.evadb = get_evadb_for_testing()
@@ -32,14 +33,15 @@
 
     def setUp(self):
         pass
 
     def tearDown(self) -> None:
         shutdown_ray()
 
+    @chatgpt_skip_marker
     def test_should_run_pandas_qa_app(self):
         app_path = Path("apps", "pandas_qa", "pandas_qa.py")
         input1 = "\n"  # use default csv
         input2 = "Print country with highest gdp\n\n"  # what to do with the csv
         input3 = "yes\n\n"  # run the script
         inputs = input1 + input2 + input3
         command = ["python", app_path]
```

### Comparing `evadb-0.3.0/test/app_tests/test_privategpt.py` & `evadb-0.3.1/test/app_tests/test_privategpt.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/app_tests/test_youtube_channel_qa.py` & `evadb-0.3.1/test/app_tests/test_youtube_channel_qa.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/app_tests/test_youtube_qa.py` & `evadb-0.3.1/test/app_tests/test_youtube_qa.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import subprocess
 import unittest
 from pathlib import Path
+from test.markers import chatgpt_skip_marker
 from test.util import get_evadb_for_testing, shutdown_ray
 
 
 class YoutubeQATest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.evadb = get_evadb_for_testing()
@@ -32,14 +33,15 @@
 
     def setUp(self):
         pass
 
     def tearDown(self) -> None:
         shutdown_ray()
 
+    @chatgpt_skip_marker
     def test_should_run_youtube_qa_app(self):
         app_path = Path("apps", "youtube_qa", "youtube_qa.py")
         input1 = "yes\n\n"  # Go with online video and default URL
         # Assuming that OPENAI_KEY is already set as an environment variable
         input2 = "What is this video on?\n"  # Question
         input3 = "exit\nexit\n"  # Exit
         inputs = input1 + input2 + input3
```

### Comparing `evadb-0.3.0/test/benchmark_tests/__init__.py` & `evadb-0.3.1/test/benchmark_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/benchmark_tests/conftest.py` & `evadb-0.3.1/test/benchmark_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/benchmark_tests/test_benchmark_pytorch.py` & `evadb-0.3.1/test/benchmark_tests/test_benchmark_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/binder/__init__.py` & `evadb-0.3.1/test/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/binder/test_statement_binder.py` & `evadb-0.3.1/test/binder/test_statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/binder/test_statement_binder_context.py` & `evadb-0.3.1/test/binder/test_statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/catalog/__init__.py` & `evadb-0.3.1/test/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/catalog/models/__init__.py` & `evadb-0.3.1/test/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/catalog/models/test_models.py` & `evadb-0.3.1/test/catalog/models/test_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/catalog/test_catalog_manager.py` & `evadb-0.3.1/test/catalog/test_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/catalog/test_column_type.py` & `evadb-0.3.1/test/catalog/test_column_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/__init__.py` & `evadb-0.3.1/test/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/test_abstract_executor.py` & `evadb-0.3.1/test/executor/test_abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/test_create_udf_executor.py` & `evadb-0.3.1/test/executor/test_create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/test_execution_context.py` & `evadb-0.3.1/test/executor/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/test_limit_executor.py` & `evadb-0.3.1/test/executor/test_limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/test_orderby_executor.py` & `evadb-0.3.1/test/executor/test_orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/test_plan_executor.py` & `evadb-0.3.1/test/executor/test_plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/test_sample_executor.py` & `evadb-0.3.1/test/executor/test_sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/test_seq_scan_executor.py` & `evadb-0.3.1/test/executor/test_seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/executor/utils.py` & `evadb-0.3.1/test/executor/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/__init__.py` & `evadb-0.3.1/test/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/test_abstract_expression.py` & `evadb-0.3.1/test/expression/test_abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/test_aggregation.py` & `evadb-0.3.1/test/expression/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/test_arithmetic.py` & `evadb-0.3.1/test/expression/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/test_comparison.py` & `evadb-0.3.1/test/expression/test_comparison.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/test_expression_tree.py` & `evadb-0.3.1/test/expression/test_expression_tree.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/test_expression_utils.py` & `evadb-0.3.1/test/expression/test_expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/test_function_expression.py` & `evadb-0.3.1/test/expression/test_function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/expression/test_logical.py` & `evadb-0.3.1/test/expression/test_logical.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/__init__.py` & `evadb-0.3.1/test/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_array_count.py` & `evadb-0.3.1/test/integration_tests/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_create_index_executor.py` & `evadb-0.3.1/test/integration_tests/test_create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_create_table_executor.py` & `evadb-0.3.1/test/integration_tests/test_create_table_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_delete_executor.py` & `evadb-0.3.1/test/integration_tests/test_delete_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
-from test.markers import macos_skip_marker
 from test.util import (
     file_remove,
     get_evadb_for_testing,
     load_udfs_for_testing,
     shutdown_ray,
 )
 
@@ -119,15 +118,14 @@
         self.assertIsNone(
             np.testing.assert_array_equal(
                 batch.frames["data"][0],
                 np.array([[[41, 41, 41], [41, 41, 41]], [[41, 41, 41], [41, 41, 41]]]),
             )
         )
 
-    @macos_skip_marker
     def test_should_delete_tuple_in_table(self):
         delete_query = """DELETE FROM testDeleteOne WHERE
                id < 20 OR dummyfloat < 2 AND id < 5 AND 20 > id
                AND id <= 20 AND id >= 5 OR id != 15 OR id = 15;"""
         batch = execute_query_fetch_all(self.evadb, delete_query)
 
         query = "SELECT * FROM testDeleteOne;"
```

### Comparing `evadb-0.3.0/test/integration_tests/test_drop_executor.py` & `evadb-0.3.1/test/integration_tests/test_drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_error_handling_with_ray.py` & `evadb-0.3.1/test/integration_tests/test_error_handling_with_ray.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_explain_executor.py` & `evadb-0.3.1/test/integration_tests/test_explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_fuzzy_join.py` & `evadb-0.3.1/test/integration_tests/test_fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_huggingface_udfs.py` & `evadb-0.3.1/test/integration_tests/test_huggingface_udfs.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_insert_executor.py` & `evadb-0.3.1/test/integration_tests/test_insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_like.py` & `evadb-0.3.1/test/integration_tests/test_like.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_load_executor.py` & `evadb-0.3.1/test/integration_tests/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_load_pdf_executor.py` & `evadb-0.3.1/test/integration_tests/test_load_pdf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_open.py` & `evadb-0.3.1/test/integration_tests/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_optimizer_rules.py` & `evadb-0.3.1/test/integration_tests/test_optimizer_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_pytorch.py` & `evadb-0.3.1/test/integration_tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_rename_executor.py` & `evadb-0.3.1/test/integration_tests/test_rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_reuse.py` & `evadb-0.3.1/test/integration_tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_s3_load_executor.py` & `evadb-0.3.1/test/integration_tests/test_s3_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_saliency.py` & `evadb-0.3.1/test/integration_tests/test_saliency.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_select_executor.py` & `evadb-0.3.1/test/integration_tests/test_select_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_show_info_executor.py` & `evadb-0.3.1/test/integration_tests/test_show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_similarity.py` & `evadb-0.3.1/test/integration_tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/integration_tests/test_text_filtering.py` & `evadb-0.3.1/test/integration_tests/test_text_filtering.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         execute_query_fetch_all(self.evadb, "DROP TABLE IF EXISTS MyPDFs;")
 
     def test_text_filter(self):
         pdf_path = f"{EvaDB_ROOT_DIR}/data/documents/layout-parser-paper.pdf"
         cursor = self.conn.cursor()
         cursor.load(pdf_path, "MyPDFs", "pdf").df()
         load_pdf_data = cursor.table("MyPDFs").df()
-        cursor.create_udf(
+        cursor.create_function(
             "TextFilterKeyword",
             True,
             f"{EvaDB_ROOT_DIR}/evadb/udfs/text_filter_keyword.py",
         ).df()
         filtered_data = (
             cursor.table("MyPDFs")
             .cross_apply("TextFilterKeyword(data, ['References'])", "objs(filtered)")
```

### Comparing `evadb-0.3.0/test/integration_tests/test_udf_executor.py` & `evadb-0.3.1/test/integration_tests/test_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/interfaces/__init__.py` & `evadb-0.3.1/test/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/interfaces/relational/__init__.py` & `evadb-0.3.1/test/interfaces/relational/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/interfaces/relational/test_relational_api.py` & `evadb-0.3.1/test/interfaces/relational/test_relational_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,33 +214,33 @@
         rel = cursor.load(
             video_file_path,
             table_name="dummy_video",
             format="video",
         )
         rel.execute()
 
-        create_dummy_object_detector_udf = cursor.create_udf(
+        create_dummy_object_detector_udf = cursor.create_function(
             "DummyObjectDetector", if_not_exists=True, impl_path="test/util.py"
         )
         create_dummy_object_detector_udf.execute()
 
         args = {"task": "automatic-speech-recognition", "model": "openai/whisper-base"}
 
-        create_speech_recognizer_udf_if_not_exists = cursor.create_udf(
+        create_speech_recognizer_udf_if_not_exists = cursor.create_function(
             "SpeechRecognizer", if_not_exists=True, type="HuggingFace", **args
         )
         query = create_speech_recognizer_udf_if_not_exists.sql_query()
         self.assertEqual(
             query,
             """CREATE UDF SpeechRecognizer IF NOT EXISTS TYPE HuggingFace 'task' 'automatic-speech-recognition' 'model' 'openai/whisper-base'""",
         )
         create_speech_recognizer_udf_if_not_exists.execute()
 
         # check if next create call of same UDF raises error
-        create_speech_recognizer_udf = cursor.create_udf(
+        create_speech_recognizer_udf = cursor.create_function(
             "SpeechRecognizer", if_not_exists=False, type="HuggingFace", **args
         )
         query = create_speech_recognizer_udf.sql_query()
         self.assertEqual(
             query,
             "CREATE UDF SpeechRecognizer TYPE HuggingFace 'task' 'automatic-speech-recognition' 'model' 'openai/whisper-base'",
         )
@@ -271,40 +271,40 @@
             video_file_path,
             table_name="dummy_video",
             format="video",
         )
         rel.execute()
 
         # Create dummy udf
-        create_dummy_object_detector_udf = cursor.create_udf(
+        create_dummy_object_detector_udf = cursor.create_function(
             "DummyObjectDetector", if_not_exists=True, impl_path="test/util.py"
         )
         create_dummy_object_detector_udf.execute()
 
         # drop dummy udf
-        drop_dummy_object_detector_udf = cursor.drop_udf(
+        drop_dummy_object_detector_udf = cursor.drop_function(
             "DummyObjectDetector", if_exists=True
         )
         drop_dummy_object_detector_udf.execute()
 
         # Check if deleted successfully
         select_query_sql = (
             "SELECT id, DummyObjectDetector(data) FROM dummy_video ORDER BY id;"
         )
         with self.assertRaises(BinderError):
             cursor.query(select_query_sql).execute()
 
         # drop non existing udf with if_exists=True should not raise error
-        drop_dummy_object_detector_udf = cursor.drop_udf(
+        drop_dummy_object_detector_udf = cursor.drop_function(
             "DummyObjectDetector", if_exists=True
         )
         drop_dummy_object_detector_udf.execute()
 
         # if_exists=False should raise error
-        drop_dummy_object_detector_udf = cursor.drop_udf(
+        drop_dummy_object_detector_udf = cursor.drop_function(
             "DummyObjectDetector", if_exists=False
         )
         with self.assertRaises(ExecutorError):
             drop_dummy_object_detector_udf.execute()
 
         # drop existing table
         drop_table = cursor.drop_table("dummy_video", if_exists=True)
@@ -328,17 +328,17 @@
         conn = connect()
         cursor = conn.cursor()
         pdf_path = f"{EvaDB_ROOT_DIR}/data/documents/state_of_the_union.pdf"
 
         load_pdf = cursor.load(file_regex=pdf_path, format="PDF", table_name="PDFs")
         load_pdf.execute()
 
-        udf_check = cursor.drop_udf("SentenceFeatureExtractor")
+        udf_check = cursor.drop_function("SentenceFeatureExtractor")
         udf_check.df()
-        udf = cursor.create_udf(
+        udf = cursor.create_function(
             "SentenceFeatureExtractor",
             True,
             f"{EvaDB_ROOT_DIR}/evadb/udfs/sentence_feature_extractor.py",
         )
         udf.execute()
 
         cursor.create_vector_index(
```

### Comparing `evadb-0.3.0/test/markers.py` & `evadb-0.3.1/test/markers.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,7 +57,11 @@
 ocr_skip_marker = pytest.mark.skip(
     reason="We do not have built-in support for OCR",
 )
 
 gpu_skip_marker = pytest.mark.skipif(
     is_gpu_available() is False, reason="Run only if gpu is available"
 )
+
+chatgpt_skip_marker = pytest.mark.skip(
+    reason="requires chatgpt",
+)
```

### Comparing `evadb-0.3.0/test/models/__init__.py` & `evadb-0.3.1/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/models/catalog/__init__.py` & `evadb-0.3.1/test/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/models/catalog/test_frame_info.py` & `evadb-0.3.1/test/models/catalog/test_frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/models/storage/__init__.py` & `evadb-0.3.1/test/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/models/storage/test_batch.py` & `evadb-0.3.1/test/models/storage/test_batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/__init__.py` & `evadb-0.3.1/test/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/rules/__init__.py` & `evadb-0.3.1/test/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/rules/test_rules.py` & `evadb-0.3.1/test/optimizer/rules/test_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_binder.py` & `evadb-0.3.1/test/optimizer/test_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_cascade_optimizer.py` & `evadb-0.3.1/test/optimizer/test_cascade_optimizer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_cost_model.py` & `evadb-0.3.1/test/optimizer/test_cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_group.py` & `evadb-0.3.1/test/optimizer/test_group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_memo.py` & `evadb-0.3.1/test/optimizer/test_memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_optimizer_context.py` & `evadb-0.3.1/test/optimizer/test_optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_optimizer_task.py` & `evadb-0.3.1/test/optimizer/test_optimizer_task.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_optimizer_utils.py` & `evadb-0.3.1/test/optimizer/test_optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/optimizer/test_statement_to_opr_converter.py` & `evadb-0.3.1/test/optimizer/test_statement_to_opr_converter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/parser/__init__.py` & `evadb-0.3.1/test/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/parser/test_parser.py` & `evadb-0.3.1/test/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/parser/test_parser_statements.py` & `evadb-0.3.1/test/parser/test_parser_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/plan_nodes/__init__.py` & `evadb-0.3.1/test/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/plan_nodes/test_plan.py` & `evadb-0.3.1/test/plan_nodes/test_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/readers/__init__.py` & `evadb-0.3.1/test/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/readers/test_csv_reader.py` & `evadb-0.3.1/test/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/readers/test_decord_reader.py` & `evadb-0.3.1/test/readers/test_decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/server/__init__.py` & `evadb-0.3.1/test/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/server/test_command_handler.py` & `evadb-0.3.1/test/server/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/server/test_configuration_file.py` & `evadb-0.3.1/test/server/test_configuration_file.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/server/test_db_api.py` & `evadb-0.3.1/test/server/test_db_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,22 +28,20 @@
     from unittest.mock import AsyncMock
 
     class DBAPITests(unittest.IsolatedAsyncioTestCase):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
         def setUp(self) -> None:
-            print("setUp")
             f = open(suffix_pytest_xdist_worker_id_to_dir("upload.txt"), "w")
             f.write("dummy data")
             f.close()
             return super().setUp()
 
         def tearDown(self) -> None:
-            print("tearDown")
             os.remove(suffix_pytest_xdist_worker_id_to_dir("upload.txt"))
             return super().tearDown()
 
         def test_evadb_cursor_execute_async(self):
             connection = AsyncMock()
             evadb_cursor = EvaDBCursor(connection)
             query = "test_query"
```

### Comparing `evadb-0.3.0/test/server/test_interpreter.py` & `evadb-0.3.1/test/server/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/server/test_server.py` & `evadb-0.3.1/test/server/test_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/storage/__init__.py` & `evadb-0.3.1/test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/storage/test_sqlite_storage_engine.py` & `evadb-0.3.1/test/storage/test_sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/storage/test_video_storage.py` & `evadb-0.3.1/test/storage/test_video_storage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/test_eva_cmd_client.py` & `evadb-0.3.1/test/test_eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/test_eva_imports.py` & `evadb-0.3.1/test/test_eva_imports.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/test_eva_server.py` & `evadb-0.3.1/test/test_eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/__init__.py` & `evadb-0.3.1/test/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/decorators/__init__.py` & `evadb-0.3.1/test/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.3.1/test/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/decorators/io_descriptors/test_descriptors.py` & `evadb-0.3.1/test/udfs/decorators/io_descriptors/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/decorators/test_decorators.py` & `evadb-0.3.1/test/udfs/decorators/test_decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/ndarray/__init__.py` & `evadb-0.3.1/test/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/ndarray/test_annotate.py` & `evadb-0.3.1/test/udfs/ndarray/test_annotate.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/ndarray/test_array_count.py` & `evadb-0.3.1/test/udfs/ndarray/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/ndarray/test_crop.py` & `evadb-0.3.1/test/udfs/ndarray/test_crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/ndarray/test_flips.py` & `evadb-0.3.1/test/udfs/ndarray/test_flips.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/ndarray/test_gaussian_blur.py` & `evadb-0.3.1/test/udfs/ndarray/test_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/ndarray/test_open.py` & `evadb-0.3.1/test/udfs/ndarray/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/ndarray/test_to_grayscale.py` & `evadb-0.3.1/test/udfs/ndarray/test_to_grayscale.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/test_abstract_udf.py` & `evadb-0.3.1/test/udfs/test_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/test_chatgpt.py` & `evadb-0.3.1/test/udfs/test_chatgpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
+from test.markers import chatgpt_skip_marker
 from test.util import get_evadb_for_testing
 
 import pandas as pd
 
 from evadb.server.command_handler import execute_query_fetch_all
 
 
@@ -52,14 +53,15 @@
 
         csv_query = f"""LOAD CSV '{self.csv_file_path}' INTO MyTextCSV;"""
         execute_query_fetch_all(self.evadb, csv_query)
 
     def tearDown(self) -> None:
         execute_query_fetch_all(self.evadb, "DROP TABLE IF EXISTS MyTextCSV;")
 
+    @chatgpt_skip_marker
     def test_openai_chat_completion_udf(self):
         udf_name = "OpenAIChatCompletion"
         execute_query_fetch_all(self.evadb, f"DROP UDF IF EXISTS {udf_name};")
 
         create_udf_query = f"""CREATE UDF IF NOT EXISTS{udf_name}
             IMPL 'evadb/udfs/chatgpt.py';
         """
```

### Comparing `evadb-0.3.0/test/udfs/test_emotion_detector.py` & `evadb-0.3.1/test/udfs/test_emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/test_facenet_udf.py` & `evadb-0.3.1/test/udfs/test_facenet_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/test_fastrcnn_object_detector.py` & `evadb-0.3.1/test/udfs/test_fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/udfs/test_yolo_object_detector.py` & `evadb-0.3.1/test/udfs/test_yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/util.py` & `evadb-0.3.1/test/util.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/utils/__init__.py` & `evadb-0.3.1/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/utils/test_generic_utils.py` & `evadb-0.3.1/test/utils/test_generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.3.0/test/utils/test_timer.py` & `evadb-0.3.1/test/utils/test_timer.py`

 * *Files identical despite different names*

