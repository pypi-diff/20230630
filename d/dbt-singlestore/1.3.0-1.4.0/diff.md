# Comparing `tmp/dbt-singlestore-1.3.0.tar.gz` & `tmp/dbt-singlestore-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-singlestore-1.3.0.tar", last modified: Wed Jun 14 14:34:00 2023, max compression
+gzip compressed data, was "dbt-singlestore-1.4.0.tar", last modified: Fri Jun 30 13:41:57 2023, max compression
```

## Comparing `dbt-singlestore-1.3.0.tar` & `dbt-singlestore-1.4.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)    11356 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/LICENSE
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       46 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/MANIFEST.in
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      321 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/PKG-INFO
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     3304 2023-06-14 09:44:17.000000 dbt-singlestore-1.3.0/README.md
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        2 2023-06-14 09:44:17.000000 dbt-singlestore-1.3.0/dbt/__init__.py
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/adapters/
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/adapters/singlestore/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      433 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/__init__.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       18 2023-06-14 09:44:17.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/__version__.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      751 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/column.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     2993 2023-06-14 14:33:19.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/connections.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     6075 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/impl.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      952 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/relation.py
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/include/
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.316879 dbt-singlestore-1.3.0/dbt/include/singlestore/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       51 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/__init__.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       79 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/dbt_project.yml
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.316879 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1554 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/catalog.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      806 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/columns.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     9224 2023-06-14 09:44:17.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/common.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      606 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/grants.sql
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.316879 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4394 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4373 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      916 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      224 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       90 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/bool_or.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      135 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      203 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/dateadd.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      193 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/datediff.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      122 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/hash.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      624 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/listagg.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       94 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/safe_cast.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      389 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/split_part.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      482 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/profile_template.yml
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      420 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/sample_profiles.yml
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      321 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/PKG-INFO
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1497 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/SOURCES.txt
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        1 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/dependency_links.txt
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       55 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/requires.txt
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        4 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/top_level.txt
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       38 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/setup.cfg
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      765 2023-06-14 14:33:19.000000 dbt-singlestore-1.3.0/setup.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.308136 dbt-singlestore-1.4.0/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)    11356 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/LICENSE
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       46 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/MANIFEST.in
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      321 2023-06-30 13:41:57.308136 dbt-singlestore-1.4.0/PKG-INFO
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     3304 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/README.md
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.300136 dbt-singlestore-1.4.0/dbt/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        2 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/__init__.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.300136 dbt-singlestore-1.4.0/dbt/adapters/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.304136 dbt-singlestore-1.4.0/dbt/adapters/singlestore/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      433 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/dbt/adapters/singlestore/__init__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       18 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/dbt/adapters/singlestore/__version__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      751 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/dbt/adapters/singlestore/column.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     2991 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/dbt/adapters/singlestore/connections.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     6149 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/dbt/adapters/singlestore/impl.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      985 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/dbt/adapters/singlestore/relation.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.300136 dbt-singlestore-1.4.0/dbt/include/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.304136 dbt-singlestore-1.4.0/dbt/include/singlestore/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       51 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/__init__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       79 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/dbt_project.yml
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.304136 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1554 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/catalog.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      806 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/columns.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     9026 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/common.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      606 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/grants.sql
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.300136 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.304136 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/incremental/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      259 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/incremental/incremental.sql
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.304136 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/snapshot/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4231 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4373 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      916 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      224 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.304136 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       90 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/bool_or.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      135 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      203 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/dateadd.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      193 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/datediff.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      122 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/hash.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      624 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/listagg.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       94 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/safe_cast.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      389 2023-06-29 14:15:32.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/split_part.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      361 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/timestamps.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      482 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/profile_template.yml
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      420 2023-05-19 09:49:48.000000 dbt-singlestore-1.4.0/dbt/include/singlestore/sample_profiles.yml
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-30 13:41:57.304136 dbt-singlestore-1.4.0/dbt_singlestore.egg-info/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      321 2023-06-30 13:41:57.000000 dbt-singlestore-1.4.0/dbt_singlestore.egg-info/PKG-INFO
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1625 2023-06-30 13:41:57.000000 dbt-singlestore-1.4.0/dbt_singlestore.egg-info/SOURCES.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        1 2023-06-30 13:41:57.000000 dbt-singlestore-1.4.0/dbt_singlestore.egg-info/dependency_links.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       55 2023-06-30 13:41:57.000000 dbt-singlestore-1.4.0/dbt_singlestore.egg-info/requires.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        4 2023-06-30 13:41:57.000000 dbt-singlestore-1.4.0/dbt_singlestore.egg-info/top_level.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       38 2023-06-30 13:41:57.308136 dbt-singlestore-1.4.0/setup.cfg
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      765 2023-06-30 13:22:15.000000 dbt-singlestore-1.4.0/setup.py
```

### Comparing `dbt-singlestore-1.3.0/LICENSE` & `dbt-singlestore-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/README.md` & `dbt-singlestore-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/dbt/adapters/singlestore/column.py` & `dbt-singlestore-1.4.0/dbt/adapters/singlestore/column.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/dbt/adapters/singlestore/connections.py` & `dbt-singlestore-1.4.0/dbt/adapters/singlestore/connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,12 +95,12 @@
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
 
         except pymysql.DatabaseError as e:
             logger.debug('Database error: {}'.format(str(e)))
-            raise dbt.exceptions.DatabaseException(str(e).strip()) from e
+            raise dbt.exceptions.DbtDatabaseError(str(e).strip()) from e
 
         except Exception as e:
             logger.debug("Error running SQL: {}", sql)
-            raise dbt.exceptions.RuntimeException(e) from e
+            raise dbt.exceptions.DbtRuntimeError(e) from e
```

### Comparing `dbt-singlestore-1.3.0/dbt/adapters/singlestore/impl.py` & `dbt-singlestore-1.4.0/dbt/adapters/singlestore/impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dbt.adapters.singlestore import SingleStoreConnectionManager
 from dbt.adapters.singlestore.column import SingleStoreColumn
 from dbt.adapters.singlestore.relation import SingleStoreRelation
 
 from dbt.adapters.base.meta import available
 from dbt.adapters.sql import SQLAdapter
 from dbt.dataclass_schema import dbtClassMixin, ValidationError
-from dbt.exceptions import RuntimeException, raise_compiler_error
+from dbt.exceptions import DbtRuntimeError, CompilationError
 from dbt.logger import GLOBAL_LOGGER as logger
 
 import dbt.utils
 
 
 @dataclass
 class SingleStoreIndexConfig(dbtClassMixin):
@@ -37,17 +37,17 @@
         if raw_index is None:
             return None
         try:
             cls.validate(raw_index)
             return cls.from_dict(raw_index)
         except ValidationError as exc:
             msg = dbt.exceptions.validator_error_message(exc)
-            raise_compiler_error(f"Could not parse index config: {msg}")
+            raise CompilationError(f"Could not parse index config: {msg}")
         except TypeError:
-            raise_compiler_error(f"Invalid index config:\n  Got: {raw_index}\n"
+            raise CompilationError(f"Invalid index config:\n  Got: {raw_index}\n"
                                  f"  Expected a dictionary with at minimum a \"columns\" key")
 
 
 class SingleStoreAdapter(SQLAdapter):
     ConnectionManager = SingleStoreConnectionManager
     Relation = SingleStoreRelation
     Column = SingleStoreColumn
@@ -104,23 +104,23 @@
     ) -> List[SingleStoreRelation]:
         kwargs = {'schema_relation': schema_relation}
         try:
             results = self.execute_macro(
                 'list_relations_without_caching',
                 kwargs=kwargs
             )
-        except RuntimeException as e:
+        except DbtRuntimeError as e:
             description = "Error while retrieving information about"
             logger.debug(f"{description} {schema_relation}: {e.msg}")
             return []
 
         relations = []
         for row in results:
             if len(row) != 4:
-                raise RuntimeException(
+                raise DbtRuntimeError(
                     f'Invalid value from "singlestore__list_relations_without_caching({kwargs})", '
                     f'got {len(row)} values, expected 4'
                 )
             database, name, schema, relation_type = row
             relation = self.Relation.create(
                 database=database,
                 schema=schema,
@@ -160,10 +160,13 @@
         self, add_to: str, value: str, location='append',
     ) -> str:
         if location == 'append':
             return f"concat({add_to}, '{value}')"
         elif location == 'prepend':
             return f"concat({value}, '{add_to}')"
         else:
-            raise RuntimeException(
+            raise DbtRuntimeError(
                 f'Got an unexpected location value of "{location}"'
             )
+
+    def valid_incremental_strategies(self):
+        return ["delete+insert"]
```

### Comparing `dbt-singlestore-1.3.0/dbt/adapters/singlestore/relation.py` & `dbt-singlestore-1.4.0/dbt/adapters/singlestore/relation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 from dbt.adapters.base.relation import BaseRelation, Policy
-from dbt.exceptions import RuntimeException
+from dbt.exceptions import DbtRuntimeError
 
 
 @dataclass
 class SingleStoreQuotePolicy(Policy):
     database: bool = True
     schema: bool = False
     identifier: bool = True
@@ -16,18 +16,18 @@
     database: bool = True
     schema: bool = False
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class SingleStoreRelation(BaseRelation):
-    quote_policy: SingleStoreQuotePolicy = SingleStoreQuotePolicy()
-    include_policy: SingleStoreIncludePolicy = SingleStoreIncludePolicy()
+    quote_policy: Policy = field(default_factory=lambda: SingleStoreQuotePolicy())
+    include_policy: Policy = field(default_factory=lambda: SingleStoreIncludePolicy())
     quote_character: str = '`'
 
     def render(self):
         if self.include_policy.database and self.include_policy.schema:
-            raise RuntimeException(
+            raise DbtRuntimeError(
                 "Got a relation with schema and database set to True"
                 "but only one can be set"
             )
         return super().render()
```

### Comparing `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/catalog.sql` & `dbt-singlestore-1.4.0/dbt/include/singlestore/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/columns.sql` & `dbt-singlestore-1.4.0/dbt/include/singlestore/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/common.sql` & `dbt-singlestore-1.4.0/dbt/include/singlestore/macros/common.sql`

 * *Files 6% similar despite different names*

```diff
@@ -201,25 +201,15 @@
     {% call statement('drop_relation') %}
         {% if from_type == 'view' -%}
             drop view {{ from_relation }}
         {% endif -%}
     {% endcall %}
 {% endmacro %}
 
-
-{% macro singlestore__current_timestamp() -%}
-    current_timestamp()
-{%- endmacro %}
-
-
-{%- macro singlestore__current_timestamp_in_utc_backcompat() -%}
-    UTC_TIMESTAMP()
-{%- endmacro -%}
-
-       
+ 
 {% macro singlestore__create_view_as(relation, sql) -%}
     {%- set sql_header = config.get('sql_header', none) -%}
     {{ sql_header if sql_header is not none }}
     create view {{ relation }} as
         {{ sql }}
 {%- endmacro %}
```

### Comparing `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/grants.sql` & `dbt-singlestore-1.4.0/dbt/include/singlestore/macros/grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql` & `dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-{% macro singlestore__snapshot_string_as_time(timestamp) -%}
-    {%- set result = "'" ~ timestamp ~ "' :> datetime" -%}
-    {{ return(result) }}
-{%- endmacro %}
-
-
 {% macro singlestore__snapshot_staging_table_deletes(strategy, source_sql, target_relation) -%}
     with snapshot_query as (
         {{ source_sql }}
     ),
     snapshotted_data as (
         select *,
             {{ strategy.unique_key }} as dbt_unique_key
```

### Comparing `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql` & `dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-singlestore-1.4.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/listagg.sql` & `dbt-singlestore-1.4.0/dbt/include/singlestore/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.3.0/dbt_singlestore.egg-info/SOURCES.txt` & `dbt-singlestore-1.4.0/dbt_singlestore.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 dbt/include/singlestore/dbt_project.yml
 dbt/include/singlestore/profile_template.yml
 dbt/include/singlestore/sample_profiles.yml
 dbt/include/singlestore/macros/catalog.sql
 dbt/include/singlestore/macros/columns.sql
 dbt/include/singlestore/macros/common.sql
 dbt/include/singlestore/macros/grants.sql
+dbt/include/singlestore/macros/materializations/incremental/incremental.sql
 dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
 dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
 dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
 dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
 dbt/include/singlestore/macros/utils/bool_or.sql
 dbt/include/singlestore/macros/utils/cast_bool_to_text.sql
 dbt/include/singlestore/macros/utils/dateadd.sql
 dbt/include/singlestore/macros/utils/datediff.sql
 dbt/include/singlestore/macros/utils/hash.sql
 dbt/include/singlestore/macros/utils/listagg.sql
 dbt/include/singlestore/macros/utils/safe_cast.sql
 dbt/include/singlestore/macros/utils/split_part.sql
+dbt/include/singlestore/macros/utils/timestamps.sql
 dbt_singlestore.egg-info/PKG-INFO
 dbt_singlestore.egg-info/SOURCES.txt
 dbt_singlestore.egg-info/dependency_links.txt
 dbt_singlestore.egg-info/requires.txt
 dbt_singlestore.egg-info/top_level.txt
```

### Comparing `dbt-singlestore-1.3.0/setup.py` & `dbt-singlestore-1.4.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_namespace_packages, setup
 
 package_name = "dbt-singlestore"
 # make sure this always matches dbt/adapters/singlestore/__version__.py
-package_version = "1.3.0"
+package_version = "1.4.0"
 description = """The singlestore adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=description,
```

