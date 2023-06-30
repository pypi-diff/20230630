# Comparing `tmp/data_diff-0.7.8.tar.gz` & `tmp/data_diff-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.8.tar", max compression
+gzip compressed data, was "data_diff-0.7.9.tar", max compression
```

## Comparing `data_diff-0.7.8.tar` & `data_diff-0.7.9.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.8/LICENSE
--rw-r--r--   0        0        0     2696 2023-05-11 19:39:43.703801 data_diff-0.7.8/README.md
--rw-r--r--   0        0        0     8710 2023-05-24 18:36:17.565800 data_diff-0.7.8/data_diff/__init__.py
--rw-r--r--   0        0        0    16024 2023-05-05 21:08:17.222127 data_diff-0.7.8/data_diff/__main__.py
--rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.7.8/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.8/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0    10067 2023-05-15 21:10:13.082649 data_diff-0.7.8/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.8/data_diff/config.py
--rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.8/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.8/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.8/data_diff/databases/base.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.8/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.8/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.8/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.8/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.8/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.8/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.8/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.8/data_diff/databases/presto.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.8/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.8/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.8/data_diff/databases/trino.py
--rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.8/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    14911 2023-05-24 18:36:17.566053 data_diff-0.7.8/data_diff/dbt.py
--rw-r--r--   0        0        0    18022 2023-05-24 18:36:17.566418 data_diff-0.7.8/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.8/data_diff/diff_tables.py
--rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.8/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.8/data_diff/info_tree.py
--rw-r--r--   0        0        0    15337 2023-05-24 18:36:17.566783 data_diff-0.7.8/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.8/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.8/data_diff/parse_time.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.8/data_diff/query_utils.py
--rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.8/data_diff/sqeleton/__init__.py
--rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.8/data_diff/sqeleton/__main__.py
--rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.8/data_diff/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.8/data_diff/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.8/data_diff/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.8/data_diff/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.8/data_diff/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.8/data_diff/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9245 2023-05-15 21:10:13.083663 data_diff-0.7.8/data_diff/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.7.8/data_diff/sqeleton/databases/base.py
--rw-r--r--   0        0        0    10135 2023-05-05 21:08:17.223531 data_diff-0.7.8/data_diff/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.8/data_diff/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.8/data_diff/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.8/data_diff/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.8/data_diff/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.8/data_diff/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.8/data_diff/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.8/data_diff/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.8/data_diff/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     6297 2023-05-24 18:36:17.567499 data_diff-0.7.8/data_diff/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.8/data_diff/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.8/data_diff/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.8/data_diff/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.8/data_diff/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.8/data_diff/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.8/data_diff/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.8/data_diff/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.8/data_diff/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.8/data_diff/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.8/data_diff/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.8/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.8/data_diff/sqeleton/schema.py
--rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.8/data_diff/sqeleton/utils.py
--rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.8/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.8/data_diff/thread_utils.py
--rw-r--r--   0        0        0     4322 2023-05-15 21:10:13.084169 data_diff-0.7.8/data_diff/tracking.py
--rw-r--r--   0        0        0     6600 2023-05-24 18:36:17.567734 data_diff-0.7.8/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-05-24 18:36:17.567903 data_diff-0.7.8/data_diff/version.py
--rwxr-xr-x   0        0        0     2849 2023-05-24 18:36:17.569021 data_diff-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     5332 1970-01-01 00:00:00.000000 data_diff-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.9/LICENSE
+-rw-r--r--   0        0        0     2696 2023-05-11 19:39:43.703801 data_diff-0.7.9/README.md
+-rw-r--r--   0        0        0     8710 2023-05-24 18:36:17.565800 data_diff-0.7.9/data_diff/__init__.py
+-rw-r--r--   0        0        0    16825 2023-06-14 23:21:12.728962 data_diff-0.7.9/data_diff/__main__.py
+-rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.7.9/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11568 2023-06-14 23:21:12.729167 data_diff-0.7.9/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0    10067 2023-05-15 21:10:13.082649 data_diff-0.7.9/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.9/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.9/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.9/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.9/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.9/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.9/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.9/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.9/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.9/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.9/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.9/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.9/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.9/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.9/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.9/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.9/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    17316 2023-06-14 23:21:12.729369 data_diff-0.7.9/data_diff/dbt.py
+-rw-r--r--   0        0        0    20102 2023-06-14 23:21:12.729586 data_diff-0.7.9/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.9/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     1753 2023-06-14 23:21:12.729730 data_diff-0.7.9/data_diff/errors.py
+-rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.9/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1477 2023-06-14 16:32:15.976930 data_diff-0.7.9/data_diff/info_tree.py
+-rw-r--r--   0        0        0    15337 2023-06-14 16:32:15.977221 data_diff-0.7.9/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.9/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.9/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.9/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.9/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.9/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.9/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.9/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.9/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.9/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.9/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.9/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9245 2023-05-15 21:10:13.083663 data_diff-0.7.9/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.7.9/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0    10648 2023-06-14 23:21:12.731092 data_diff-0.7.9/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.9/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.9/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.9/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.9/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.9/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.9/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.9/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.9/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     6297 2023-05-24 18:36:17.567499 data_diff-0.7.9/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.9/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.9/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.9/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.9/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.9/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.9/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.9/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.9/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.9/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.9/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.9/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.9/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.9/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.9/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.9/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     5481 2023-06-14 22:17:36.188033 data_diff-0.7.9/data_diff/tracking.py
+-rw-r--r--   0        0        0     6637 2023-06-08 19:44:38.931340 data_diff-0.7.9/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-06-14 23:23:45.736859 data_diff-0.7.9/data_diff/version.py
+-rwxr-xr-x   0        0        0     2851 2023-06-14 23:23:47.177863 data_diff-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 data_diff-0.7.9/PKG-INFO
```

### Comparing `data_diff-0.7.8/LICENSE` & `data_diff-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/README.md` & `data_diff-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/__init__.py` & `data_diff-0.7.9/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/__main__.py` & `data_diff-0.7.9/data_diff/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from copy import deepcopy
 from datetime import datetime
+import os
 import sys
 import time
 import json
 import logging
 from itertools import islice
 from typing import Optional
 
@@ -229,15 +230,22 @@
     help="Which directory to look in for the dbt_project.yml file. Default is the current working directory and its parents.",
 )
 @click.option(
     "--select",
     "-s",
     default=None,
     metavar="PATH",
-    help="select dbt resources to compare using dbt selection syntax",
+    help="select dbt resources to compare using dbt selection syntax.",
+)
+@click.option(
+    "--state",
+    "-s",
+    default=None,
+    metavar="PATH",
+    help="Specify manifest to utilize for 'prod' comparison paths instead of using configuration.",
 )
 def main(conf, run, **kw):
     if kw["table2"] is None and kw["database2"]:
         # Use the "database table table" form
         kw["table2"] = kw["database2"]
         kw["database2"] = kw["database1"]
 
@@ -262,23 +270,35 @@
             logging.debug(f"Applied run configuration: {kw['__conf__']}")
     elif kw.get("verbose"):
         logging.basicConfig(level=logging.INFO, format=LOG_FORMAT, datefmt=DATE_FORMAT)
     else:
         logging.basicConfig(level=logging.WARNING, format=LOG_FORMAT, datefmt=DATE_FORMAT)
 
     try:
+        state = kw.pop("state", None)
+        if state:
+            state = os.path.expanduser(state)
+        profiles_dir_override = kw.pop("dbt_profiles_dir", None)
+        if profiles_dir_override:
+            profiles_dir_override = os.path.expanduser(profiles_dir_override)
+        project_dir_override = kw.pop("dbt_project_dir", None)
+        if project_dir_override:
+            project_dir_override = os.path.expanduser(project_dir_override)
         if kw["dbt"]:
             dbt_diff(
-                profiles_dir_override=kw["dbt_profiles_dir"],
-                project_dir_override=kw["dbt_project_dir"],
+                profiles_dir_override=profiles_dir_override,
+                project_dir_override=project_dir_override,
                 is_cloud=kw["cloud"],
                 dbt_selection=kw["select"],
+                state=state,
             )
         else:
-            return _data_diff(**kw)
+            return _data_diff(
+                dbt_project_dir=project_dir_override, dbt_profiles_dir=profiles_dir_override, state=state, **kw
+            )
     except Exception as e:
         logging.error(e)
         if kw["debug"]:
             raise
 
 
 def _data_diff(
@@ -311,14 +331,15 @@
     table_write_limit,
     materialize_to_table,
     dbt,
     cloud,
     dbt_profiles_dir,
     dbt_project_dir,
     select,
+    state,
     threads1=None,
     threads2=None,
     __conf__=None,
 ):
     if limit and stats:
         logging.error("Cannot specify a limit when using the -s/--stats switch")
         return
```

### Comparing `data_diff-0.7.8/data_diff/cloud/data_source.py` & `data_diff-0.7.9/data_diff/cloud/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 
 def _validate_temp_schema(temp_schema: str):
     if len(temp_schema.split(".")) != 2:
         raise ValueError("Temporary schema should have a format <database>.<schema>")
 
 
 def _get_temp_schema(dbt_parser: DbtParser, db_type: str) -> Optional[str]:
-    diff_vars = dbt_parser.get_datadiff_variables()
-    config_prod_database = diff_vars.get("prod_database")
-    config_prod_schema = diff_vars.get("prod_schema")
+    config = dbt_parser.get_datadiff_config()
+    config_prod_database = config.prod_database
+    config_prod_schema = config.prod_schema
     if config_prod_database is not None and config_prod_schema is not None:
         temp_schema = f"{config_prod_database}.{config_prod_schema}"
         if db_type == "snowflake":
             return temp_schema.upper()
         elif db_type in {"pg", "postgres_aurora", "postgres_aws_rds", "redshift"}:
             return temp_schema.lower()
         return temp_schema
```

### Comparing `data_diff-0.7.8/data_diff/cloud/datafold_api.py` & `data_diff-0.7.9/data_diff/cloud/datafold_api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/config.py` & `data_diff-0.7.9/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/databases/_connect.py` & `data_diff-0.7.9/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/dbt.py` & `data_diff-0.7.9/data_diff/dbt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os
+import re
 import time
 import webbrowser
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Tuple, Union
 import keyring
-
 import pydantic
 import rich
-from rich.prompt import Confirm
+from rich.prompt import Confirm, Prompt
+
+from data_diff.errors import DataDiffCustomSchemaNoConfigError, DataDiffDbtProjectVarsNotFoundError
 
 from . import connect_to_table, diff_tables, Algorithm
 from .cloud import DatafoldAPI, TCloudApiDataDiff, TCloudApiOrgMeta, get_or_create_data_source
-from .dbt_parser import DbtParser, PROJECT_FILE
+from .dbt_parser import DbtParser, PROJECT_FILE, TDatadiffConfig
 from .tracking import (
+    bool_ask_for_email,
+    create_email_signup_event_json,
     set_entrypoint_name,
     set_dbt_user_id,
     set_dbt_version,
     set_dbt_project_id,
     create_end_event_json,
     create_start_event_json,
     send_event_json,
@@ -48,73 +52,78 @@
 
 
 def dbt_diff(
     profiles_dir_override: Optional[str] = None,
     project_dir_override: Optional[str] = None,
     is_cloud: bool = False,
     dbt_selection: Optional[str] = None,
+    state: Optional[str] = None,
 ) -> None:
     print_version_info()
     diff_threads = []
     set_entrypoint_name("CLI-dbt")
-    dbt_parser = DbtParser(profiles_dir_override, project_dir_override)
+    dbt_parser = DbtParser(profiles_dir_override, project_dir_override, state)
     models = dbt_parser.get_models(dbt_selection)
-    datadiff_variables = dbt_parser.get_datadiff_variables()
-    config_prod_database = datadiff_variables.get("prod_database")
-    config_prod_schema = datadiff_variables.get("prod_schema")
-    config_prod_custom_schema = datadiff_variables.get("prod_custom_schema")
-    datasource_id = datadiff_variables.get("datasource_id")
-    set_dbt_user_id(dbt_parser.dbt_user_id)
-    set_dbt_version(dbt_parser.dbt_version)
-    set_dbt_project_id(dbt_parser.dbt_project_id)
-
-    if datadiff_variables.get("custom_schemas") is not None:
-        logger.warning(
-            "vars: data_diff: custom_schemas: is no longer used and can be removed.\nTo utilize custom schemas, see the documentation here: https://docs.datafold.com/development_testing/open_source"
+    config = dbt_parser.get_datadiff_config()
+    _initialize_events(dbt_parser.dbt_user_id, dbt_parser.dbt_version, dbt_parser.dbt_project_id)
+
+
+    if not state and not (config.prod_database or config.prod_schema):
+        doc_url = "https://docs.datafold.com/development_testing/open_source#configure-your-dbt-project"
+        raise DataDiffDbtProjectVarsNotFoundError(
+            f"""vars: data_diff: section not found in dbt_project.yml.\n\nTo solve this, please configure your dbt project: \n{doc_url}\n\nOr specify a production manifest using the `--state` flag."""
         )
 
     if is_cloud:
         api = _initialize_api()
         # exit so the user can set the key
         if not api:
             return
         org_meta = api.get_org_meta()
 
-        if datasource_id is None:
+        if config.datasource_id is None:
             rich.print("[red]Data source ID not found in dbt_project.yml")
             is_create_data_source = Confirm.ask("Would you like to create a new data source?")
             if is_create_data_source:
-                datasource_id = get_or_create_data_source(api=api, dbt_parser=dbt_parser)
+                config.datasource_id = get_or_create_data_source(api=api, dbt_parser=dbt_parser)
                 rich.print(f'To use the data source in next runs, please, update your "{PROJECT_FILE}" with a block:')
-                rich.print(f"[green]vars:\n  data_diff:\n    datasource_id: {datasource_id}\n")
+                rich.print(f"[green]vars:\n  data_diff:\n    datasource_id: {config.datasource_id}\n")
                 rich.print(
                     "Read more about Datafold vars in docs: "
                     "https://docs.datafold.com/os_diff/dbt_integration/#configure-a-data-source\n"
                 )
             else:
                 raise ValueError(
                     "Datasource ID not found, include it as a dbt variable in the dbt_project.yml. "
                     "\nvars:\n data_diff:\n   datasource_id: 1234"
                 )
 
-        data_source = api.get_data_source(datasource_id)
+        data_source = api.get_data_source(config.datasource_id)
         dbt_parser.set_casing_policy_for(connection_type=data_source.type)
         rich.print("[green][bold]\nDiffs in progress...[/][/]\n")
 
     else:
         dbt_parser.set_connection()
 
     for model in models:
-        diff_vars = _get_diff_vars(
-            dbt_parser, config_prod_database, config_prod_schema, config_prod_custom_schema, model
-        )
+        diff_vars = _get_diff_vars(dbt_parser, config, model)
+
+        # we won't always have a prod path when using state
+        # when the model DNE in prod manifest, skip the model diff
+        if (
+            state and len(diff_vars.prod_path) < 2
+        ):  # < 2 because some providers like databricks can legitimately have *only* 2
+            diff_output_str = _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
+            diff_output_str += "[green]New model: nothing to diff![/] \n"
+            rich.print(diff_output_str)
+            continue
 
         if diff_vars.primary_keys:
             if is_cloud:
-                diff_thread = run_as_daemon(_cloud_diff, diff_vars, datasource_id, api, org_meta)
+                diff_thread = run_as_daemon(_cloud_diff, diff_vars, config.datasource_id, api, org_meta)
                 diff_threads.append(diff_thread)
             else:
                 _local_diff(diff_vars)
         else:
             rich.print(
                 _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
                 + "Skipped due to unknown primary key. Add uniqueness tests, meta, or tags.\n"
@@ -124,49 +133,27 @@
     if diff_threads:
         for thread in diff_threads:
             thread.join()
 
 
 def _get_diff_vars(
     dbt_parser: "DbtParser",
-    config_prod_database: Optional[str],
-    config_prod_schema: Optional[str],
-    config_prod_custom_schema: Optional[str],
+    config: TDatadiffConfig,
     model,
 ) -> TDiffVars:
     dev_database = model.database
     dev_schema = model.schema_
 
     primary_keys = dbt_parser.get_pk_from_model(model, dbt_parser.unique_columns, "primary-key")
 
-    # "custom" dbt config database
-    if model.config.database:
-        prod_database = model.config.database
-    elif config_prod_database:
-        prod_database = config_prod_database
+    # prod path is constructed via configuration or the prod manifest via --state
+    if dbt_parser.prod_manifest_obj:
+        prod_database, prod_schema = _get_prod_path_from_manifest(model, dbt_parser.prod_manifest_obj)
     else:
-        prod_database = dev_database
-
-    # prod schema name differs from dev schema name
-    if config_prod_schema:
-        custom_schema = model.config.schema_
-
-        # the model has a custom schema config(schema='some_schema')
-        if custom_schema:
-            if not config_prod_custom_schema:
-                raise ValueError(
-                    f"Found a custom schema on model {model.name}, but no value for\nvars:\n  data_diff:\n    prod_custom_schema:\nPlease set a value!\n"
-                    + "For more details see: https://docs.datafold.com/development_testing/open_source"
-                )
-            prod_schema = config_prod_custom_schema.replace("<custom_schema>", custom_schema)
-        # no custom schema, use the default
-        else:
-            prod_schema = config_prod_schema
-    else:
-        prod_schema = dev_schema
+        prod_database, prod_schema = _get_prod_path_from_config(config, model, dev_database, dev_schema)
 
     if dbt_parser.requires_upper:
         dev_qualified_list = [x.upper() for x in [dev_database, dev_schema, model.alias] if x]
         prod_qualified_list = [x.upper() for x in [prod_database, prod_schema, model.alias] if x]
         primary_keys = [x.upper() for x in primary_keys]
     else:
         dev_qualified_list = [x for x in [dev_database, dev_schema, model.alias] if x]
@@ -182,14 +169,53 @@
         threads=dbt_parser.threads,
         where_filter=datadiff_model_config.where_filter,
         include_columns=datadiff_model_config.include_columns,
         exclude_columns=datadiff_model_config.exclude_columns,
     )
 
 
+def _get_prod_path_from_config(config, model, dev_database, dev_schema) -> Tuple[str, str]:
+    # "custom" dbt config database
+    if model.config.database:
+        prod_database = model.config.database
+    elif config.prod_database:
+        prod_database = config.prod_database
+    else:
+        prod_database = dev_database
+
+    # prod schema name differs from dev schema name
+    if config.prod_schema:
+        custom_schema = model.config.schema_
+
+        # the model has a custom schema config(schema='some_schema')
+        if custom_schema:
+            if not config.prod_custom_schema:
+                raise DataDiffCustomSchemaNoConfigError(
+                    f"Found a custom schema on model {model.name}, but no value for\nvars:\n  data_diff:\n    prod_custom_schema:\nPlease set a value or utilize the `--state` flag!\n\n"
+                    + "For more details see: https://docs.datafold.com/development_testing/open_source"
+                )
+            prod_schema = config.prod_custom_schema.replace("<custom_schema>", custom_schema)
+            # no custom schema, use the default
+        else:
+            prod_schema = config.prod_schema
+    else:
+        prod_schema = dev_schema
+    return prod_database, prod_schema
+
+
+def _get_prod_path_from_manifest(model, prod_manifest) -> Union[Tuple[str, str], Tuple[None, None]]:
+    prod_database = None
+    prod_schema = None
+    prod_model = prod_manifest.nodes.get(model.unique_id, None)
+    if prod_model:
+        prod_database = prod_model.database
+        prod_schema = prod_model.schema_
+    return prod_database, prod_schema
+
+
 def _local_diff(diff_vars: TDiffVars) -> None:
     dev_qualified_str = ".".join(diff_vars.dev_path)
     prod_qualified_str = ".".join(diff_vars.prod_path)
     diff_output_str = _diff_output_base(dev_qualified_str, prod_qualified_str)
 
     table1 = connect_to_table(diff_vars.connection, dev_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads)
     table2 = connect_to_table(
@@ -385,7 +411,38 @@
                 diff_url = f"{api.host}/datadiffs/{diff_id}/overview"
                 rich.print(f"{diff_url} \n")
             logger.error(error)
 
 
 def _diff_output_base(dev_path: str, prod_path: str) -> str:
     return f"\n[green]{prod_path} <> {dev_path}[/] \n"
+
+
+def _initialize_events(dbt_user_id: Optional[str], dbt_version: Optional[str], dbt_project_id: Optional[str]) -> None:
+    set_dbt_user_id(dbt_user_id)
+    set_dbt_version(dbt_version)
+    set_dbt_project_id(dbt_project_id)
+    _email_signup()
+
+
+def _email_signup() -> None:
+    email_regex = r'^[\w\.\+-]+@[\w\.-]+\.\w+$'
+    prompt = "\nWould you like to be notified when a new data-diff version is available?\n\nEnter email or leave blank to opt out (we'll only ask once).\n"
+
+    if bool_ask_for_email():
+        while True:
+            email_input = Prompt.ask(
+                prompt=prompt,
+                default="",
+                show_default=False,
+            )
+            email = email_input.strip()
+
+            if email == "" or re.match(email_regex, email):
+                break
+
+            prompt = ""
+            rich.print("[red]Invalid email. Please enter a valid email or leave it blank to opt out.[/]")
+
+        if email:
+            event_json = create_email_signup_event_json(email)
+            run_as_daemon(send_event_json, event_json)
```

### Comparing `data_diff-0.7.8/data_diff/dbt_parser.py` & `data_diff-0.7.9/data_diff/dbt_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,28 @@
 import yaml
 
 from packaging.version import parse as parse_version
 import pydantic
 from dbt_artifacts_parser.parser import parse_run_results, parse_manifest
 from dbt.config.renderer import ProfileRenderer
 
+from data_diff.errors import (
+    DataDiffDbtBigQueryUnsupportedMethodError,
+    DataDiffDbtConnectionNotImplementedError,
+    DataDiffDbtCoreNoRunnerError,
+    DataDiffDbtNoSuccessfulModelsInRunError,
+    DataDiffDbtProfileNotFoundError,
+    DataDiffDbtRedshiftPasswordOnlyError,
+    DataDiffDbtRunResultsVersionError,
+    DataDiffDbtSelectNoMatchingModelsError,
+    DataDiffDbtSelectUnexpectedError,
+    DataDiffDbtSelectVersionTooLowError,
+    DataDiffDbtSnowflakeSetConnectionError,
+)
+
 from .utils import getLogger, get_from_dict_with_raise
 
 
 logger = getLogger(__name__)
 
 
 # getting this dbt_runner will only succeed in dbt-core>=1.5
@@ -69,35 +83,60 @@
 
 class TDatadiffModelConfig(pydantic.BaseModel):
     where_filter: Optional[str] = None
     include_columns: List[str] = []
     exclude_columns: List[str] = []
 
 
+class TDatadiffConfig(pydantic.BaseModel):
+    prod_database: Optional[str] = None
+    prod_schema: Optional[str] = None
+    prod_custom_schema: Optional[str] = None
+    datasource_id: Optional[int] = None
+
+
 class DbtParser:
-    def __init__(self, profiles_dir_override: str, project_dir_override: str) -> None:
+    def __init__(
+        self,
+        profiles_dir_override: Optional[str] = None,
+        project_dir_override: Optional[str] = None,
+        state: Optional[str] = None,
+    ) -> None:
         try_set_dbt_flags()
         self.dbt_runner = try_get_dbt_runner()
         self.profiles_dir = Path(profiles_dir_override or default_profiles_dir())
         self.project_dir = Path(project_dir_override or default_project_dir())
         self.connection = {}
         self.project_dict = self.get_project_dict()
-        self.manifest_obj = self.get_manifest_obj()
-        self.dbt_user_id = self.manifest_obj.metadata.user_id
-        self.dbt_version = self.manifest_obj.metadata.dbt_version
-        self.dbt_project_id = self.manifest_obj.metadata.project_id
+        self.dev_manifest_obj = self.get_manifest_obj(self.project_dir / MANIFEST_PATH)
+        self.prod_manifest_obj = None
+        if state:
+            self.prod_manifest_obj = self.get_manifest_obj(Path(state))
+
+        self.dbt_user_id = self.dev_manifest_obj.metadata.user_id
+        self.dbt_version = self.dev_manifest_obj.metadata.dbt_version
+        self.dbt_project_id = self.dev_manifest_obj.metadata.project_id
         self.requires_upper = False
         self.threads = None
         self.unique_columns = self.get_unique_columns()
 
-    def get_datadiff_variables(self) -> dict:
-        doc_url = "https://docs.datafold.com/development_testing/open_source#configure-your-dbt-project"
-        error_message = f"vars: data_diff: section not found in dbt_project.yml.\n\nTo solve this, please configure your dbt project: \n{doc_url}\n"
-        vars = get_from_dict_with_raise(self.project_dict, "vars", error_message)
-        return get_from_dict_with_raise(vars, "data_diff", error_message)
+    def get_datadiff_config(self) -> TDatadiffConfig:
+        data_diff_vars = self.project_dict.get("vars", {}).get("data_diff", {})
+        prod_database = data_diff_vars.get("prod_database")
+        prod_schema = data_diff_vars.get("prod_schema")
+        prod_custom_schema = data_diff_vars.get("prod_custom_schema")
+        datasource_id = data_diff_vars.get("datasource_id")
+        config = TDatadiffConfig(
+            prod_database=prod_database,
+            prod_schema=prod_schema,
+            prod_custom_schema=prod_custom_schema,
+            datasource_id=datasource_id,
+        )
+        logger.info(f"config: {config}")
+        return config
 
     def get_datadiff_model_config(self, model_meta: dict) -> TDatadiffModelConfig:
         where_filter = None
         include_columns = []
         exclude_columns = []
 
         if "datafold" in model_meta and "datadiff" in model_meta["datafold"]:
@@ -114,19 +153,19 @@
         dbt_version = parse_version(self.dbt_version)
         if dbt_selection:
             if (dbt_version.major, dbt_version.minor) >= (1, 5):
                 if self.dbt_runner:
                     return self.get_dbt_selection_models(dbt_selection)
                 # edge case if running data-diff from a separate env than dbt (likely local development)
                 else:
-                    raise Exception(
+                    raise DataDiffDbtCoreNoRunnerError(
                         "data-diff is using a dbt-core version < 1.5, update the environment's dbt-core version via pip install 'dbt-core>=1.5' in order to use `--select`"
                     )
             else:
-                raise Exception(
+                raise DataDiffDbtSelectVersionTooLowError(
                     f"The `--select` feature requires dbt >= 1.5, but your project's manifest.json is from dbt v{dbt_version}. Please follow these steps to use the `--select` feature: \n 1. Update your dbt-core version via pip install 'dbt-core>=1.5'. Details: https://docs.getdbt.com/docs/core/pip-install#change-dbt-core-versions \n 2. Execute any `dbt` command (`run`, `compile`, `build`) to create a new manifest.json."
                 )
         else:
             return self.get_run_results_models()
 
     def get_dbt_selection_models(self, dbt_selection: str) -> List[str]:
         # log level and format settings needed to prevent dbt from printing to stdout
@@ -148,52 +187,58 @@
                 "unique_id",
                 "--project-dir",
                 self.project_dir,
             ]
         )
         if results.exception:
             raise results.exception
-        elif results.success and results.result:
+
+        if results.success and results.result:
             model_list = [json.loads(model)["unique_id"] for model in results.result]
-            models = [self.manifest_obj.nodes.get(x) for x in model_list]
+            models = [self.dev_manifest_obj.nodes.get(x) for x in model_list]
             return models
-        elif not results.result:
-            raise Exception(f"No dbt models found for `--select {dbt_selection}`")
-        else:
-            logger.debug(str(results))
-            raise Exception("Encountered an unexpected error while finding `--select` models")
+
+        if not results.result:
+            raise DataDiffDbtSelectNoMatchingModelsError(f"No dbt models found for `--select {dbt_selection}`")
+
+        logger.debug(str(results))
+        raise DataDiffDbtSelectUnexpectedError("Encountered an unexpected error while finding `--select` models")
 
     def get_run_results_models(self):
         with open(self.project_dir / RUN_RESULTS_PATH) as run_results:
             logger.info(f"Parsing file {RUN_RESULTS_PATH}")
             run_results_dict = json.load(run_results)
             run_results_obj = parse_run_results(run_results=run_results_dict)
 
         dbt_version = parse_version(run_results_obj.metadata.dbt_version)
 
         if dbt_version < parse_version("1.3.0"):
             self.profiles_dir = legacy_profiles_dir()
 
         if dbt_version < parse_version(LOWER_DBT_V):
-            raise Exception(f"Found dbt: v{dbt_version} Expected the dbt project's version to be >= {LOWER_DBT_V}")
-        elif dbt_version >= parse_version(UPPER_DBT_V):
+            raise DataDiffDbtRunResultsVersionError(
+                f"Found dbt: v{dbt_version} Expected the dbt project's version to be >= {LOWER_DBT_V}"
+            )
+        if dbt_version >= parse_version(UPPER_DBT_V):
             logger.warning(
                 f"{dbt_version} is a recent version of dbt and may not be fully tested with data-diff! \nPlease report any issues to https://github.com/datafold/data-diff/issues"
             )
 
         success_models = [x.unique_id for x in run_results_obj.results if x.status.name == "success"]
-        models = [self.manifest_obj.nodes.get(x) for x in success_models]
+        models = [self.dev_manifest_obj.nodes.get(x) for x in success_models]
         if not models:
-            raise ValueError("Expected > 0 successful models runs from the last dbt command.")
+            raise DataDiffDbtNoSuccessfulModelsInRunError(
+                "Expected > 0 successful models runs from the last dbt command."
+            )
 
         return models
 
-    def get_manifest_obj(self):
-        with open(self.project_dir / MANIFEST_PATH) as manifest:
-            logger.info(f"Parsing file {MANIFEST_PATH}")
+    def get_manifest_obj(self, path: Path):
+        with open(path) as manifest:
+            logger.info(f"Parsing file {path}")
             manifest_dict = json.load(manifest)
             manifest_obj = parse_manifest(manifest=manifest_dict)
         return manifest_obj
 
     def get_project_dict(self):
         with open(self.project_dir / PROJECT_FILE) as project:
             logger.info(f"Parsing file {PROJECT_FILE}")
@@ -205,33 +250,43 @@
         with open(profiles_path) as profiles:
             logger.info(f"Parsing file {profiles_path}")
             profiles = yaml.safe_load(profiles)
 
         dbt_profile_var = self.project_dict.get("profile")
 
         profile = get_from_dict_with_raise(
-            profiles, dbt_profile_var, f"No profile '{dbt_profile_var}' found in '{profiles_path}'."
+            profiles,
+            dbt_profile_var,
+            DataDiffDbtProfileNotFoundError(f"No profile '{dbt_profile_var}' found in '{profiles_path}'."),
         )
         # values can contain env_vars
         rendered_profile = ProfileRenderer().render_data(profile)
         profile_target = get_from_dict_with_raise(
-            rendered_profile, "target", f"No target found in profile '{dbt_profile_var}' in '{profiles_path}'."
+            rendered_profile,
+            "target",
+            DataDiffDbtProfileNotFoundError(f"No target found in profile '{dbt_profile_var}' in '{profiles_path}'."),
         )
         outputs = get_from_dict_with_raise(
-            rendered_profile, "outputs", f"No outputs found in profile '{dbt_profile_var}' in '{profiles_path}'."
+            rendered_profile,
+            "outputs",
+            DataDiffDbtProfileNotFoundError(f"No outputs found in profile '{dbt_profile_var}' in '{profiles_path}'."),
         )
         credentials = get_from_dict_with_raise(
             outputs,
             profile_target,
-            f"No credentials found for target '{profile_target}' in profile '{dbt_profile_var}' in '{profiles_path}'.",
+            DataDiffDbtProfileNotFoundError(
+                f"No credentials found for target '{profile_target}' in profile '{dbt_profile_var}' in '{profiles_path}'."
+            ),
         )
         conn_type = get_from_dict_with_raise(
             credentials,
             "type",
-            f"No type found for target '{profile_target}' in profile '{dbt_profile_var}' in '{profiles_path}'.",
+            DataDiffDbtProfileNotFoundError(
+                f"No type found for target '{profile_target}' in profile '{dbt_profile_var}' in '{profiles_path}'."
+            ),
         )
         conn_type = conn_type.lower()
 
         return credentials, conn_type
 
     def set_connection(self):
         credentials, conn_type = self.get_connection_creds()
@@ -249,46 +304,56 @@
                 "insecure_mode": credentials.get("insecure_mode", False),
                 "client_session_keep_alive": credentials.get("client_session_keep_alive", False),
             }
             self.threads = credentials.get("threads")
 
             if credentials.get("private_key_path") is not None:
                 if credentials.get("password") is not None:
-                    raise Exception("Cannot use password and key at the same time")
+                    raise DataDiffDbtSnowflakeSetConnectionError("Cannot use password and key at the same time")
                 conn_info["key"] = credentials.get("private_key_path")
                 conn_info["private_key_passphrase"] = credentials.get("private_key_passphrase")
             elif credentials.get("authenticator") is not None:
                 conn_info["authenticator"] = credentials.get("authenticator")
                 conn_info["password"] = credentials.get("password")
             elif credentials.get("password") is not None:
                 conn_info["password"] = credentials.get("password")
             else:
-                raise Exception("Snowflake: unsupported auth method")
+                raise DataDiffDbtSnowflakeSetConnectionError("Snowflake: unsupported auth method")
         elif conn_type == "bigquery":
+            supported_methods = ["oauth", "service-account"]
             method = credentials.get("method")
             # there are many connection types https://docs.getdbt.com/reference/warehouse-setups/bigquery-setup#oauth-via-gcloud
             # this assumes that the user is auth'd via `gcloud auth application-default login`
-            if method is None or method != "oauth":
-                raise Exception("Oauth is the current method supported for Big Query.")
+            if method not in supported_methods:
+                raise DataDiffDbtBigQueryUnsupportedMethodError(
+                    f"Method: {method} is not in the current methods supported for Big Query ({supported_methods})."
+                )
+
             conn_info = {
                 "driver": conn_type,
                 "project": credentials.get("project"),
                 "dataset": credentials.get("dataset"),
             }
+
             self.threads = credentials.get("threads")
+            if method == supported_methods[1]:
+                conn_info["keyfile"] = credentials.get("keyfile")
+
         elif conn_type == "duckdb":
             conn_info = {
                 "driver": conn_type,
                 "filepath": credentials.get("path"),
             }
         elif conn_type == "redshift":
             if (credentials.get("pass") is None and credentials.get("password") is None) or credentials.get(
                 "method"
             ) == "iam":
-                raise Exception("Only password authentication is currently supported for Redshift.")
+                raise DataDiffDbtRedshiftPasswordOnlyError(
+                    "Only password authentication is currently supported for Redshift."
+                )
             conn_info = {
                 "driver": conn_type,
                 "host": credentials.get("host"),
                 "user": credentials.get("user"),
                 "password": credentials.get("password") or credentials.get("pass"),
                 "port": credentials.get("port"),
                 "dbname": credentials.get("dbname"),
@@ -311,15 +376,15 @@
                 "user": credentials.get("user"),
                 "password": credentials.get("password"),
                 "port": credentials.get("port"),
                 "dbname": credentials.get("dbname") or credentials.get("database"),
             }
             self.threads = credentials.get("threads")
         else:
-            raise NotImplementedError(f"Provider {conn_type} is not yet supported for dbt diffs")
+            raise DataDiffDbtConnectionNotImplementedError(f"Provider {conn_type} is not yet supported for dbt diffs")
 
         self.connection = conn_info
 
     def get_pk_from_model(self, node, unique_columns: dict, pk_tag: str) -> List[str]:
         try:
             # Get a set of all the column names
             column_names = {name for name, params in node.columns.items()}
@@ -351,15 +416,15 @@
         except (KeyError, IndexError, TypeError) as e:
             raise e
 
         logger.debug("Found no PKs")
         return []
 
     def get_unique_columns(self) -> Dict[str, Set[str]]:
-        manifest = self.manifest_obj
+        manifest = self.dev_manifest_obj
         cols_by_uid = defaultdict(set)
         for node in manifest.nodes.values():
             try:
                 if not (node.resource_type.value == "test" and hasattr(node, "test_metadata")):
                     continue
 
                 if not node.depends_on or not node.depends_on.nodes:
```

### Comparing `data_diff-0.7.8/data_diff/diff_tables.py` & `data_diff-0.7.9/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/hashdiff_tables.py` & `data_diff-0.7.9/data_diff/hashdiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/info_tree.py` & `data_diff-0.7.9/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/joindiff_tables.py` & `data_diff-0.7.9/data_diff/joindiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/lexicographic_space.py` & `data_diff-0.7.9/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/parse_time.py` & `data_diff-0.7.9/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/query_utils.py` & `data_diff-0.7.9/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/abcs/database_types.py` & `data_diff-0.7.9/data_diff/sqeleton/abcs/database_types.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/abcs/mixins.py` & `data_diff-0.7.9/data_diff/sqeleton/abcs/mixins.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/bound_exprs.py` & `data_diff-0.7.9/data_diff/sqeleton/bound_exprs.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/__init__.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/_connect.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/base.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/base.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/bigquery.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,26 @@
 @import_helper(text="Please install BigQuery and configure your google-cloud access.")
 def import_bigquery():
     from google.cloud import bigquery
 
     return bigquery
 
 
+def import_bigquery_service_account():
+    from google.oauth2 import service_account
+
+    return service_account
+
+
 class Mixin_MD5(AbstractMixin_MD5):
     def md5_as_int(self, s: str) -> str:
         return f"cast(cast( ('0x' || substr(TO_HEX(md5({s})), 18)) as int64) as numeric)"
 
 
 class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
-
     def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
         if coltype.rounds:
             timestamp = f"timestamp_micros(cast(round(unix_micros(cast({value} as timestamp))/1000000, {coltype.precision})*1000000 as int))"
             return f"FORMAT_TIMESTAMP('%F %H:%M:%E6S', {timestamp})"
 
         if coltype.precision == 0:
             return f"FORMAT_TIMESTAMP('%F %H:%M:%S.000000', {value})"
@@ -140,16 +145,16 @@
         "BIGNUMERIC": Decimal,
         "FLOAT64": Float,
         "FLOAT32": Float,
         "STRING": Text,
         "BOOL": Boolean,
         "JSON": JSON,
     }
-    TYPE_ARRAY_RE = re.compile(r'ARRAY<(.+)>')
-    TYPE_STRUCT_RE = re.compile(r'STRUCT<(.+)>')
+    TYPE_ARRAY_RE = re.compile(r"ARRAY<(.+)>")
+    TYPE_STRUCT_RE = re.compile(r"STRUCT<(.+)>")
     MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_TimeTravel, Mixin_RandomSample}
 
     def random(self) -> str:
         return "RAND()"
 
     def quote(self, s: str):
         return f"`{s}`"
@@ -169,15 +174,14 @@
         col_name: str,
         type_repr: str,
         *args: Any,  # pass-through args
         **kwargs: Any,  # pass-through args
     ) -> ColType:
         col_type = super().parse_type(table_path, col_name, type_repr, *args, **kwargs)
         if isinstance(col_type, UnknownColType):
-
             m = self.TYPE_ARRAY_RE.fullmatch(type_repr)
             if m:
                 item_type = self.parse_type(table_path, col_name, m.group(1), *args, **kwargs)
                 col_type = Array(item_type=item_type)
 
             # We currently ignore structs' structure, but later can parse it too. Examples:
             # - STRUCT<INT64, STRING(10)> (unnamed)
@@ -203,17 +207,26 @@
 
 class BigQuery(Database):
     CONNECT_URI_HELP = "bigquery://<project>/<dataset>"
     CONNECT_URI_PARAMS = ["dataset"]
     dialect = Dialect()
 
     def __init__(self, project, *, dataset, **kw):
+        credentials = None
         bigquery = import_bigquery()
 
-        self._client = bigquery.Client(project, **kw)
+        keyfile = kw.pop("keyfile", None)
+        if keyfile:
+            bigquery_service_account = import_bigquery_service_account()
+            credentials = bigquery_service_account.Credentials.from_service_account_file(
+                keyfile,
+                scopes=["https://www.googleapis.com/auth/cloud-platform"],
+            )
+
+        self._client = bigquery.Client(project=project, credentials=credentials, **kw)
         self.project = project
         self.dataset = dataset
 
         self.default_schema = dataset
 
     def _normalize_returned_value(self, value):
         if isinstance(value, bytes):
```

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/clickhouse.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/databricks.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/duckdb.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/mssql.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/mysql.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/oracle.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/oracle.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/postgresql.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/presto.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/redshift.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/redshift.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/snowflake.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/trino.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/databases/vertica.py` & `data_diff-0.7.9/data_diff/sqeleton/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/queries/api.py` & `data_diff-0.7.9/data_diff/sqeleton/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/queries/ast_classes.py` & `data_diff-0.7.9/data_diff/sqeleton/queries/ast_classes.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/queries/compiler.py` & `data_diff-0.7.9/data_diff/sqeleton/queries/compiler.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/queries/extras.py` & `data_diff-0.7.9/data_diff/sqeleton/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/query_utils.py` & `data_diff-0.7.9/data_diff/sqeleton/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/repl.py` & `data_diff-0.7.9/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/schema.py` & `data_diff-0.7.9/data_diff/sqeleton/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/sqeleton/utils.py` & `data_diff-0.7.9/data_diff/sqeleton/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/table_segment.py` & `data_diff-0.7.9/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/thread_utils.py` & `data_diff-0.7.9/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.8/data_diff/tracking.py` & `data_diff-0.7.9/data_diff/tracking.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,38 @@
     if "anonymous_id" not in conf:
         conf["anonymous_id"] = str(uuid4())
         with open(DEFAULT_PROFILE, "w") as f:
             toml.dump(conf, f)
     return conf
 
 
+def bool_ask_for_email() -> bool:
+    """
+    Checks the .datadiff.toml profile file for the asked_for_email key
+
+    Returns False immediately if --no-tracking
+
+    If found, return False (already asked for email)
+
+    If not found, add a key "asked_for_email", and return True (we should ask for email)
+
+    Returns:
+        bool: decision on whether to prompt the user for their email
+    """
+    if g_tracking_enabled:
+        profile = _load_profile()
+
+        if "asked_for_email" not in profile:
+            profile["asked_for_email"] = ""
+            with open(DEFAULT_PROFILE, "w") as conf:
+                toml.dump(profile, conf)
+            return True
+    return False
+
+
 g_tracking_enabled = True
 g_anonymous_id = None
 
 entrypoint_name = "Python API"
 
 
 def disable_tracking():
@@ -144,14 +168,30 @@
             "org_id": org_id,
             "org_name": org_name,
             "user_id": user_id,
         },
     }
 
 
+def create_email_signup_event_json(email: str) -> Dict[str, Any]:
+    return {
+        "event": "os_diff_email_opt_in",
+        "properties": {
+            "distinct_id": get_anonymous_id(),
+            "token": TOKEN,
+            "time": time(),
+            "data_diff_version:": __version__,
+            "entrypoint_name": entrypoint_name,
+            "email": email,
+            "dbt_user_id": dbt_user_id,
+            "dbt_project_id": dbt_project_id,
+        },
+    }
+
+
 def send_event_json(event_json):
     if not g_tracking_enabled:
         raise RuntimeError("Won't send; tracking is disabled!")
 
     headers = {
         "Content-Type": "application/json",
         "Authorization": "Basic MkhndE00SGNxOUJtZWlDcU5ZaHo3Tzl0a2pNOg==",
```

### Comparing `data_diff-0.7.8/data_diff/utils.py` & `data_diff-0.7.9/data_diff/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,18 +80,20 @@
 
 
 def truncate_error(error: str):
     first_line = error.split("\n", 1)[0]
     return re.sub("'(.*?)'", "'***'", first_line)
 
 
-def get_from_dict_with_raise(dictionary: Dict, key: str, error_message: str):
+def get_from_dict_with_raise(dictionary: Dict, key: str, exception: Exception):
+    if dictionary is None:
+        raise exception
     result = dictionary.get(key)
     if result is None:
-        raise ValueError(error_message)
+        raise exception
     return result
 
 
 class Vector(tuple):
 
     """Immutable implementation of a regular vector over any arithmetic value
```

### Comparing `data_diff-0.7.8/pyproject.toml` & `data_diff-0.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.8"
+version = "0.7.9"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
@@ -19,26 +19,26 @@
     "Environment :: Console",
     "Topic :: Database :: Database Engines/Servers",
     "Typing :: Typed"
 ]
 packages = [{ include = "data_diff" }]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.2"
 runtype = "^0.2.6"
 dsnparse = [
     { version = "<0.2.0", markers = "python_version < '3.8.0'" },
     { version = "*", markers = "python_version >= '3.8.0'" }
 ]
 click = "^8.1"
 rich = "*"
 toml = "^0.10.2"
 mysql-connector-python = {version="8.0.29", optional=true}
 psycopg2 = {version="*", optional=true}
-snowflake-connector-python = {version = ">=2.7.2,<4.0.0", optional=true}
+snowflake-connector-python = {version = ">=3.0.2,<4.0.0", optional=true}
 cryptography = {version="*", optional=true}
 trino = {version="^0.314.0", optional=true}
 presto-python-client = {version="*", optional=true}
 clickhouse-driver = {version="*", optional=true}
 duckdb = {version="^0.7.0", optional=true}
 dbt-artifacts-parser = {version="^0.3.0"}
 dbt-core = {version="^1.0.0"}
@@ -51,15 +51,15 @@
 
 [tool.poetry.dev-dependencies]
 parameterized = "*"
 unittest-parallel = "*"
 preql = "^0.2.19"
 mysql-connector-python = "*"
 psycopg2 = "*"
-snowflake-connector-python = ">=2.7.2,<4.0.0"
+snowflake-connector-python = ">=3.0.2,<4.0.0"
 cryptography = "*"
 trino = "^0.314.0"
 presto-python-client = "*"
 clickhouse-driver = "*"
 vertica-python = "*"
 duckdb = "^0.7.0"
 dbt-artifacts-parser = "^0.3.0"
```

### Comparing `data_diff-0.7.8/PKG-INFO` & `data_diff-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.7.8
+Version: 0.7.9
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -48,15 +47,15 @@
 Requires-Dist: keyring
 Requires-Dist: mysql-connector-python (==8.0.29) ; extra == "mysql"
 Requires-Dist: preql (>=0.2.19,<0.3.0) ; extra == "preql"
 Requires-Dist: presto-python-client ; extra == "presto"
 Requires-Dist: psycopg2 ; extra == "postgresql" or extra == "redshift"
 Requires-Dist: rich
 Requires-Dist: runtype (>=0.2.6,<0.3.0)
-Requires-Dist: snowflake-connector-python (>=2.7.2,<4.0.0) ; extra == "snowflake"
+Requires-Dist: snowflake-connector-python (>=3.0.2,<4.0.0) ; extra == "snowflake"
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: trino (>=0.314.0,<0.315.0) ; extra == "trino"
 Requires-Dist: urllib3 (<2)
 Requires-Dist: vertica-python ; extra == "vertica"
 Project-URL: Repository, https://github.com/datafold/data-diff
 Description-Content-Type: text/markdown
```

