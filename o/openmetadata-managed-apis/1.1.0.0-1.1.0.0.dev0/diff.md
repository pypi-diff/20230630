# Comparing `tmp/openmetadata_managed_apis-1.1.0.0.tar.gz` & `tmp/openmetadata_managed_apis-1.1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata_managed_apis-1.1.0.0.tar", last modified: Fri Jun 30 09:15:37 2023, max compression
+gzip compressed data, was "openmetadata_managed_apis-1.1.0.0.dev0.tar", last modified: Mon Jun 26 12:17:36 2023, max compression
```

## Comparing `openmetadata_managed_apis-1.1.0.0.tar` & `openmetadata_managed_apis-1.1.0.0.dev0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.727718 openmetadata_managed_apis-1.1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-30 09:15:37.727718 openmetadata_managed_apis-1.1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.719718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.723718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/apis_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.723718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/health_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/run_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.723718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/kill_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.723718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/resources/dag_runner.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.723718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.723718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/views/rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.719718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.723718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/views/templates/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/views/templates/rest_api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.727718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.727718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/data_insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/workflow_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:37.719718 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-30 09:15:33.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-30 09:15:33.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:15:33.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 09:15:33.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:15:19.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-30 09:15:33.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 09:15:33.000000 openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:15:37.727718 openmetadata_managed_apis-1.1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-30 09:14:00.000000 openmetadata_managed_apis-1.1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.770165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/apis_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/health_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/run_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/kill_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/resources/dag_runner.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.770165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/templates/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/templates/rest_api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/data_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/workflow_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.770165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:17:18.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/setup.py
```

### Comparing `openmetadata_managed_apis-1.1.0.0/PKG-INFO` & `openmetadata_managed_apis-1.1.0.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata_managed_apis
-Version: 1.1.0.0
+Version: 1.1.0.0.dev0
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.1.0.0/README.md` & `openmetadata_managed_apis-1.1.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/__init__.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/apis_metadata.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/apis_metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/app.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/app.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/config.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/error_handlers.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/error_handlers.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/response.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/response.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/delete.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/deploy.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/disable.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/disable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/enable.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/enable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/health.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/health.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/health_auth.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/health_auth.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/ip.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/ip.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/kill.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/kill.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/last_dag_logs.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/run_automation.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/run_automation.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/status.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/routes/trigger.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/api/utils.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/delete.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/deploy.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/health.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/health.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/kill_all.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/kill_all.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/last_dag_logs.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/state.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/state.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/status.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/operations/trigger.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/plugin.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/plugin.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/utils/logger.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/utils/parser.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/parser.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/views/rest_api.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/rest_api.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/views/templates/rest_api/index.html` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/templates/rest_api/index.html`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/config.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/common.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,19 +79,17 @@
 class GetServiceException(Exception):
     """
     Exception to be thrown when couldn't fetch the service from server
     """
 
     def __init__(self, service_type: str, service_name: str):
         self.message = (
-            f"Could not get service from type [{service_type}]. This means that the"
+            f"Could not get service from type {service_type}. This means that the"
             " OpenMetadata client running in the Airflow host had issues getting"
-            f" the service [{service_name}]. Make sure the ingestion-bot JWT token"
-            " is valid and that the Workflow is deployed with the latest one. If this error"
-            " persists, recreate the JWT token and redeploy the Workflow."
+            f" the service {service_name}. Validate your ingestion-bot authentication."
         )
         super().__init__(self.message)
 
 
 class ClientInitializationError(Exception):
     """
     Exception to be thrown when couldn't initialize the Openmetadata Client
```

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/data_insight.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/data_insight.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 """
 import json
 
 from airflow import DAG
 from openmetadata_managed_apis.utils.logger import set_operator_logger
 from openmetadata_managed_apis.workflows.ingestion.common import (
     ClientInitializationError,
-    GetServiceException,
     build_dag,
 )
 from openmetadata_managed_apis.workflows.ingestion.elasticsearch_sink import (
     build_elasticsearch_sink,
 )
 
 from metadata.data_insight.api.workflow import DataInsightWorkflow
@@ -80,15 +79,17 @@
         raise ClientInitializationError(f"Failed to initialize the client: {exc}")
 
     openmetadata_service = metadata.get_by_name(
         entity=MetadataService, fqn=ingestion_pipeline.service.fullyQualifiedName
     )
 
     if not openmetadata_service:
-        raise GetServiceException(service_type="metadata", service_name="OpenMetadata")
+        raise ValueError(
+            "Could not retrieve the OpenMetadata service! This should not happen."
+        )
 
     sink = build_elasticsearch_sink(
         openmetadata_service.connection.config, ingestion_pipeline
     )
 
     workflow_config = OpenMetadataWorkflowConfig(
         source=WorkflowSource(
```

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/dbt.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/dbt.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #  limitations under the License.
 """
 ElasticSearch reindex DAG function builder
 """
 from airflow import DAG
 from openmetadata_managed_apis.workflows.ingestion.common import (
     ClientInitializationError,
-    GetServiceException,
     build_dag,
     metadata_ingestion_workflow,
 )
 
 from metadata.generated.schema.entity.services.connections.metadata.metadataESConnection import (
     MetadataESConnection,
 )
@@ -53,15 +52,17 @@
     except Exception as exc:
         raise ClientInitializationError(f"Failed to initialize the client: {exc}")
 
     openmetadata_service: MetadataService = metadata.get_by_name(
         entity=MetadataService, fqn=ingestion_pipeline.service.fullyQualifiedName
     )
     if not openmetadata_service:
-        raise GetServiceException(service_type="metadata", service_name="OpenMetadata")
+        raise ValueError(
+            "Could not retrieve the OpenMetadata service! This should not happen."
+        )
 
     sink = Sink(type="metadata-rest", config={})
 
     workflow_config = OpenMetadataWorkflowConfig(
         source=WorkflowSource(
             type="metadata_elasticsearch",
             serviceName=ingestion_pipeline.service.fullyQualifiedName,
```

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/lineage.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/lineage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/metadata.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/profiler.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/profiler.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/registry.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/registry.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/test_suite.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/test_suite.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/ingestion/usage.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/usage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/workflow_builder.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/workflow_builder.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis/workflows/workflow_factory.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/workflow_factory.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/PKG-INFO` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata-managed-apis
-Version: 1.1.0.0
+Version: 1.1.0.0.dev0
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.1.0.0/openmetadata_managed_apis.egg-info/SOURCES.txt` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.1.0.0/setup.py` & `openmetadata_managed_apis-1.1.0.0.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 }
 
 setup(
     name=PLUGIN_NAME,
     packages=find_packages(include=[f"{PLUGIN_NAME}.*", PLUGIN_NAME]),
     include_package_data=True,
     package_data={PLUGIN_NAME: get_package_data()},
-    version="1.1.0.0",
+    version="1.1.0.0.dev0",
     url="https://open-metadata.org/",
     author="OpenMetadata Committers",
     license="Apache License 2.0",
     description="Airflow REST APIs to create and manage DAGS",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     entry_points={
```

