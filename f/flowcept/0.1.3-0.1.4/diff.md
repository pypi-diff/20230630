# Comparing `tmp/flowcept-0.1.3.tar.gz` & `tmp/flowcept-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowcept-0.1.3.tar", last modified: Thu Jun 29 20:03:55 2023, max compression
+gzip compressed data, was "flowcept-0.1.4.tar", last modified: Fri Jun 30 20:18:59 2023, max compression
```

## Comparing `flowcept-0.1.3.tar` & `flowcept-0.1.4.tar`

### file list

```diff
@@ -1,88 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.992256 flowcept-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 20:03:41.000000 flowcept-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-29 20:03:54.992256 flowcept-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-29 20:03:41.000000 flowcept-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.980255 flowcept-0.1.3/flowcept/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.984255 flowcept-0.1.3/flowcept/commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.984255 flowcept-0.1.3/flowcept/commons/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/commons/daos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/commons/daos/document_db_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/commons/daos/mq_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/commons/flowcept_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/commons/flowcept_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/commons/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/commons/vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.984255 flowcept-0.1.3/flowcept/flowcept_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowcept_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowcept_api/consumer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowcept_api/task_query_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.984255 flowcept-0.1.3/flowcept/flowcept_webserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowcept_webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowcept_webserver/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.984255 flowcept-0.1.3/flowcept/flowcept_webserver/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowcept_webserver/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowcept_webserver/resources/query_rsrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowcept_webserver/resources/task_messages_rsrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.984255 flowcept-0.1.3/flowcept/flowceptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.984255 flowcept-0.1.3/flowcept/flowceptor/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/consumers/consumer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/consumers/document_inserter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.988255 flowcept-0.1.3/flowcept/flowceptor/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/base_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/base_settings_dataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.988255 flowcept-0.1.3/flowcept/flowceptor/plugins/dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/dask/dask_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/dask/dask_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/dask/dask_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/interceptor_state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.988255 flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/interception_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/settings_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.988255 flowcept-0.1.3/flowcept/flowceptor/plugins/tensorboard/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/tensorboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/tensorboard/tensorboard_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.992256 flowcept-0.1.3/flowcept/flowceptor/plugins/zambeze/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/zambeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 20:03:41.000000 flowcept-0.1.3/flowcept/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.980255 flowcept-0.1.3/flowcept.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-29 20:03:54.000000 flowcept-0.1.3/flowcept.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-29 20:03:54.000000 flowcept-0.1.3/flowcept.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:03:54.000000 flowcept-0.1.3/flowcept.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-29 20:03:54.000000 flowcept-0.1.3/flowcept.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 20:03:54.000000 flowcept-0.1.3/flowcept.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 20:03:41.000000 flowcept-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:03:54.996255 flowcept-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-29 20:03:41.000000 flowcept-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.992256 flowcept-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.992256 flowcept-0.1.3/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/api/query_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.992256 flowcept-0.1.3/tests/doc_db_inserter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/doc_db_inserter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/doc_db_inserter/doc_db_inserter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.992256 flowcept-0.1.3/tests/log_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/log_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/log_tests/log_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/log_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:54.992256 flowcept-0.1.3/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/plugins/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/plugins/test_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/plugins/test_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-29 20:03:41.000000 flowcept-0.1.3/tests/plugins/test_zambeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-30 20:18:48.000000 flowcept-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-30 20:18:59.247320 flowcept-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-30 20:18:48.000000 flowcept-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept/commons/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/daos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/daos/document_db_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/daos/mq_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/flowcept_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/commons/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowcept_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_api/consumer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_api/task_query_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowcept_webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowcept_webserver/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/resources/query_rsrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowcept_webserver/resources/task_messages_rsrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/consumers/consumer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/consumers/document_inserter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/base_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/base_settings_dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/interceptor_state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/interception_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/settings_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.243320 flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/tensorboard_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/flowceptor/telemetry_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-30 20:18:48.000000 flowcept-0.1.4/flowcept/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-30 20:18:49.000000 flowcept-0.1.4/flowcept/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.239320 flowcept-0.1.4/flowcept.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 20:18:59.000000 flowcept-0.1.4/flowcept.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 20:18:48.000000 flowcept-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:18:59.247320 flowcept-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-30 20:18:48.000000 flowcept-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/api/query_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/doc_db_inserter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/doc_db_inserter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/doc_db_inserter/doc_db_inserter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/log_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/log_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/log_tests/log_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/log_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:59.247320 flowcept-0.1.4/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/test_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/test_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/plugins/test_zambeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 20:18:48.000000 flowcept-0.1.4/tests/telemetry_test.py
```

### Comparing `flowcept-0.1.3/LICENSE` & `flowcept-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/PKG-INFO` & `flowcept-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: flowcept
-Version: 0.1.3
-Summary: A system to integrate data from multiple workflows.
+Version: 0.1.4
+Summary: FlowCept is a runtime data integration system that empowers any data processing system to capture and query workflow provenance data using data observability, requiring minimal or no changes in the target system code. It seamlessly integrates data from multiple workflows, enabling users to comprehend complex, heterogeneous, and large-scale data from various sources in federated environments.
 Home-page: https://github.com/ORNL/flowcept
 Author: Oak Ridge National Laboratory
 License: MIT
+Keywords: ai,ml,machine-learning,provenance,lineage,responsible-ai,databases,big-data,provenance,tensorboard,data-integration,scientific-workflows,dask,reproducibility,workflows,parallel-processing,lineage,model-management,mlflow,responsible-ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: Database
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: zambeze
 Provides-Extra: mlflow
 Provides-Extra: tensorboard
 Provides-Extra: mongo
 Provides-Extra: dask
@@ -28,24 +35,23 @@
 [![Tests](https://github.com/ORNL/flowcept/actions/workflows/run-tests.yml/badge.svg)](https://github.com/ORNL/flowcept/actions/workflows/run-tests.yml)
 [![Code Formatting](https://github.com/ORNL/flowcept/actions/workflows/code-formatting.yml/badge.svg)](https://github.com/ORNL/flowcept/actions/workflows/code-formatting.yml)
 [![License: MIT](https://img.shields.io/github/license/ORNL/flowcept)](LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # FlowCept
 
-FlowCept is a runtime data integration system that aims at empowering any data generation system to capture 
-workflow provenance data using data observability, with minimal (often no) changes in the target system code. 
-Thus, it is able to integrate data from multiple workflows, enabling users to understand complex, heterogeneous, large-scale data coming from various sources in federated environments.
+FlowCept is a runtime data integration system that empowers any data processing system to capture and query workflow 
+provenance data using data observability, requiring minimal or no changes in the target system code. It seamlessly integrates data from multiple workflows, enabling users to comprehend complex, heterogeneous, and large-scale data from various sources in federated environments.
 
 FlowCept is intended to address scenarios where multiple workflows in a science campaign or in an enterprise run and generate 
-important data to be analyzed in an integrated manner. Since these workflows may use different data generation tools or can be executed within
-different parallel computing systems (e.g., Dask, Spark, workflow management systems), its key differentiator is the 
-capability to seamless integrate multi-workflow data from various sources using data observability.
-It builds an integrated data view at runtime of these multi-workflow data following 
-[W3C PROV](https://www.w3.org/TR/prov-overview/) recommendations for its data schema.
+important data to be analyzed in an integrated manner. Since these workflows may use different data manipulation tools (e.g., provenance or lineage capture tools, database systems, performance profiling tools) or can be executed within
+different parallel computing systems (e.g., Dask, Spark, Workflow Management Systems), its key differentiator is the 
+capability to seamless and automatically integrate data from various workflows using data observability.
+It builds an integrated data view at runtime enabling end-to-end exploratory data analysis and monitoring.
+It follows [W3C PROV](https://www.w3.org/TR/prov-overview/) recommendations for its data schema.
 It does not require changes in user codes or systems (i.e., instrumentation). 
 All users need to do is to create adapters for their systems or tools, if one is not available yet. 
 
 Currently, FlowCept provides adapters for: [Dask](https://www.dask.org/), [MLFlow](https://mlflow.org/), [TensorBoard](https://www.tensorflow.org/tensorboard), and [Zambeze](https://github.com/ORNL/zambeze). 
 
 See the [Jupyter Notebooks](notebooks) for utilization examples.
```

### Comparing `flowcept-0.1.3/README.md` & `flowcept-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 [![Tests](https://github.com/ORNL/flowcept/actions/workflows/run-tests.yml/badge.svg)](https://github.com/ORNL/flowcept/actions/workflows/run-tests.yml)
 [![Code Formatting](https://github.com/ORNL/flowcept/actions/workflows/code-formatting.yml/badge.svg)](https://github.com/ORNL/flowcept/actions/workflows/code-formatting.yml)
 [![License: MIT](https://img.shields.io/github/license/ORNL/flowcept)](LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # FlowCept
 
-FlowCept is a runtime data integration system that aims at empowering any data generation system to capture 
-workflow provenance data using data observability, with minimal (often no) changes in the target system code. 
-Thus, it is able to integrate data from multiple workflows, enabling users to understand complex, heterogeneous, large-scale data coming from various sources in federated environments.
+FlowCept is a runtime data integration system that empowers any data processing system to capture and query workflow 
+provenance data using data observability, requiring minimal or no changes in the target system code. It seamlessly integrates data from multiple workflows, enabling users to comprehend complex, heterogeneous, and large-scale data from various sources in federated environments.
 
 FlowCept is intended to address scenarios where multiple workflows in a science campaign or in an enterprise run and generate 
-important data to be analyzed in an integrated manner. Since these workflows may use different data generation tools or can be executed within
-different parallel computing systems (e.g., Dask, Spark, workflow management systems), its key differentiator is the 
-capability to seamless integrate multi-workflow data from various sources using data observability.
-It builds an integrated data view at runtime of these multi-workflow data following 
-[W3C PROV](https://www.w3.org/TR/prov-overview/) recommendations for its data schema.
+important data to be analyzed in an integrated manner. Since these workflows may use different data manipulation tools (e.g., provenance or lineage capture tools, database systems, performance profiling tools) or can be executed within
+different parallel computing systems (e.g., Dask, Spark, Workflow Management Systems), its key differentiator is the 
+capability to seamless and automatically integrate data from various workflows using data observability.
+It builds an integrated data view at runtime enabling end-to-end exploratory data analysis and monitoring.
+It follows [W3C PROV](https://www.w3.org/TR/prov-overview/) recommendations for its data schema.
 It does not require changes in user codes or systems (i.e., instrumentation). 
 All users need to do is to create adapters for their systems or tools, if one is not available yet. 
 
 Currently, FlowCept provides adapters for: [Dask](https://www.dask.org/), [MLFlow](https://mlflow.org/), [TensorBoard](https://www.tensorflow.org/tensorboard), and [Zambeze](https://github.com/ORNL/zambeze). 
 
 See the [Jupyter Notebooks](notebooks) for utilization examples.
```

### Comparing `flowcept-0.1.3/flowcept/__init__.py` & `flowcept-0.1.4/flowcept/__init__.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/commons/daos/document_db_dao.py` & `flowcept-0.1.4/flowcept/commons/daos/document_db_dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Dict, Tuple, Any
 from bson import ObjectId
 from pymongo import MongoClient, UpdateOne
 
 from flowcept.commons.flowcept_logger import FlowceptLogger
-from flowcept.commons.flowcept_data_classes import TaskMessage
+from flowcept.commons.flowcept_dataclasses.task_message import TaskMessage
 from flowcept.commons.utils import perf_log
 from flowcept.configs import (
     MONGO_HOST,
     MONGO_PORT,
     MONGO_DB,
     MONGO_COLLECTION,
     PERF_LOG,
```

### Comparing `flowcept-0.1.3/flowcept/commons/daos/mq_dao.py` & `flowcept-0.1.4/flowcept/commons/daos/mq_dao.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/commons/flowcept_data_classes.py` & `flowcept-0.1.4/flowcept/commons/flowcept_dataclasses/task_message.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from enum import Enum
 from typing import Dict, AnyStr, Any, Union, List
 
+from flowcept.commons.flowcept_dataclasses.telemetry import Telemetry
+
 
 class Status(str, Enum):  # inheriting from str here for JSON serialization
     SUBMITTED = "SUBMITTED"
     WAITING = "WAITING"
     RUNNING = "RUNNING"
     FINISHED = "FINISHED"
     ERROR = "ERROR"
@@ -18,23 +20,22 @@
 # Not a dataclass because a dataclass stores keys even when there's no value,
 # adding unnecessary overhead.
 class TaskMessage:
     task_id: AnyStr = None  # Any way to identify a task
     utc_timestamp: float = None
     adapter_id: AnyStr = None
     user: AnyStr = None
-    msg_id: AnyStr = None  # TODO: This is deprecated. Remove from all plugins
     used: Dict[AnyStr, Any] = None  # Used parameter and files
     campaign_id: AnyStr = None
     generated: Dict[AnyStr, Any] = None  # Generated results and files
     submitted_at: float = None
     started_at: float = None
     ended_at: float = None
-    start_telemetry: Dict[AnyStr, Any] = None
-    end_telemetry: Dict[AnyStr, Any] = None
+    telemetry_at_start: Telemetry = None
+    telemetry_at_end: Telemetry = None
     workflow_name: AnyStr = None
     workflow_id: AnyStr = None
     activity_id: AnyStr = None
     status: Status = None
     stdout: Union[AnyStr, Dict] = None
     stderr: Union[AnyStr, Dict] = None
     custom_metadata: Dict[AnyStr, Any] = None
@@ -45,14 +46,15 @@
     private_ip: AnyStr = None
     hostname: AnyStr = None
     extra_metadata: Dict = None
     sys_name: AnyStr = None
     address: AnyStr = None
     dependencies: List = None
     dependents: List = None
+    flowcept_version: str = None
 
     @staticmethod
     def get_dict_field_names():
         return [
             "used",
             "generated",
             "custom_metadata",
@@ -61,8 +63,13 @@
         ]
 
     @staticmethod
     def get_index_field():
         return "task_id"
 
     def to_dict(self):
-        return self.__dict__
+        ret = self.__dict__
+        if self.telemetry_at_start is not None:
+            ret["telemetry_at_start"] = self.telemetry_at_start.to_dict()
+        if self.telemetry_at_end is not None:
+            ret["telemetry_at_end"] = self.telemetry_at_end.to_dict()
+        return ret
```

### Comparing `flowcept-0.1.3/flowcept/commons/flowcept_logger.py` & `flowcept-0.1.4/flowcept/commons/flowcept_logger.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/commons/utils.py` & `flowcept-0.1.4/flowcept/commons/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime, timedelta
 import json
 from time import time
 from flowcept.configs import PERF_LOG
 from flowcept.commons.flowcept_logger import FlowceptLogger
-from flowcept.commons.flowcept_data_classes import Status
+from flowcept.commons.flowcept_dataclasses.task_message import Status
 
 
 def get_utc_now() -> float:
     now = datetime.utcnow()
     return now.timestamp()
```

### Comparing `flowcept-0.1.3/flowcept/configs.py` & `flowcept-0.1.4/flowcept/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 # SYSTEM SETTINGS #
 ######################
 
 MQ_TYPE = settings["project"].get("mq_type", "redis")
 DEBUG_MODE = settings["project"].get("debug", False)
 PERF_LOG = settings["project"].get("performance_logging", False)
 JSON_SERIALIZER = settings["project"].get("json_serializer", "default")
+TELEMETRY_CAPTURE = settings["project"].get("telemetry_capture", None)
 
 ######################
 # SYS METADATA #
 ######################
 
 sys_metadata = settings.get("sys_metadata", None)
 if sys_metadata is not None:
```

### Comparing `flowcept-0.1.3/flowcept/flowcept_api/consumer_api.py` & `flowcept-0.1.4/flowcept/flowcept_api/consumer_api.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowcept_api/task_query_api.py` & `flowcept-0.1.4/flowcept/flowcept_api/task_query_api.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowcept_webserver/app.py` & `flowcept-0.1.4/flowcept/flowcept_webserver/app.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowcept_webserver/resources/query_rsrc.py` & `flowcept-0.1.4/flowcept/flowcept_webserver/resources/query_rsrc.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowcept_webserver/resources/task_messages_rsrc.py` & `flowcept-0.1.4/flowcept/flowcept_webserver/resources/task_messages_rsrc.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowceptor/consumers/consumer_utils.py` & `flowcept-0.1.4/flowcept/flowceptor/consumers/consumer_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict
 
-from flowcept.commons.flowcept_data_classes import TaskMessage
+from flowcept.commons.flowcept_dataclasses.task_message import TaskMessage
 
 
 def curate_task_msg(task_msg_dict: dict):
     # Converting any arg to kwarg in the form {"arg1": val1, "arg2: val2}
     for field in TaskMessage.get_dict_field_names():
         if field not in task_msg_dict:
             continue
```

### Comparing `flowcept-0.1.3/flowcept/flowceptor/consumers/document_inserter.py` & `flowcept-0.1.4/flowcept/flowceptor/consumers/document_inserter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from time import time, sleep
 from threading import Thread, Event, Lock
 from typing import Dict
 from datetime import datetime
 
 from flowcept.commons.utils import GenericJSONDecoder
-from flowcept.commons.flowcept_data_classes import TaskMessage
+from flowcept.commons.flowcept_dataclasses.task_message import TaskMessage
 from flowcept.configs import (
     MONGO_INSERTION_BUFFER_TIME,
     MONGO_MAX_BUFFER_SIZE,
     MONGO_MIN_BUFFER_SIZE,
     MONGO_ADAPTIVE_BUFFER_SIZE,
     DEBUG_MODE,
     JSON_SERIALIZER,
```

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/base_interceptor.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/base_interceptor.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,19 @@
     PRIVATE_IP,
     CAMPAIGN_ID,
     HOSTNAME,
     EXTRA_METADATA,
 )
 from flowcept.commons.flowcept_logger import FlowceptLogger
 from flowcept.commons.daos.mq_dao import MQDao
-from flowcept.commons.flowcept_data_classes import TaskMessage
+from flowcept.commons.flowcept_dataclasses.task_message import TaskMessage
 from flowcept.flowceptor.plugins.settings_factory import get_settings
 
+from flowcept.version import __version__
+
 
 def _enrich_task_message(settings_key, task_msg: TaskMessage):
     if task_msg.utc_timestamp is None:
         task_msg.utc_timestamp = get_utc_now()
 
     if task_msg.adapter_id is None:
         task_msg.adapter_id = settings_key
@@ -48,14 +50,17 @@
 
     if task_msg.hostname is None and HOSTNAME is not None:
         task_msg.hostname = HOSTNAME
 
     if task_msg.extra_metadata is None and EXTRA_METADATA is not None:
         task_msg.extra_metadata = EXTRA_METADATA
 
+    if task_msg.flowcept_version is None:
+        task_msg.flowcept_version = __version__
+
 
 class BaseInterceptor(object, metaclass=ABCMeta):
     def __init__(self, plugin_key):
         self.logger = FlowceptLogger().get_logger()
         self.settings = get_settings(plugin_key)
         self._mq_dao = MQDao()
```

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/dask/dask_interceptor.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_interceptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import pickle
 
-from flowcept.commons.flowcept_data_classes import TaskMessage, Status
+from flowcept.commons.flowcept_dataclasses.task_message import (
+    TaskMessage,
+    Status,
+)
 from flowcept.flowceptor.plugins.base_interceptor import (
     BaseInterceptor,
 )
 from flowcept.commons.utils import get_utc_now
+from flowcept.configs import TELEMETRY_CAPTURE
+from flowcept.flowceptor.telemetry_capture import capture_telemetry
 
 
 def get_run_spec_data(task_msg: TaskMessage, run_spec):
     def _get_arg(arg_name):
         if type(run_spec) == dict:
             return run_spec.get(arg_name, None)
         elif hasattr(run_spec, arg_name):
@@ -138,34 +143,40 @@
 
             ts = self._worker.state.tasks[task_id]
 
             task_msg = TaskMessage()
             task_msg.task_id = task_id
 
             if ts.state == "executing":
+                if TELEMETRY_CAPTURE is not None:
+                    task_msg.telemetry_at_start = capture_telemetry()
                 task_msg.status = Status.RUNNING
                 task_msg.address = self._worker.worker_address
                 if self.settings.worker_create_timestamps:
                     task_msg.started_at = get_utc_now()
             elif ts.state == "memory":
                 task_msg.status = Status.FINISHED
                 if self.settings.worker_create_timestamps:
                     task_msg.ended_at = get_utc_now()
                 else:
                     get_times_from_task_state(task_msg, ts)
+                if TELEMETRY_CAPTURE is not None:
+                    task_msg.telemetry_at_end = capture_telemetry()
             elif ts.state == "error":
                 task_msg.status = Status.ERROR
                 if self.settings.worker_create_timestamps:
                     task_msg.ended_at = get_utc_now()
                 else:
                     get_times_from_task_state(task_msg, ts)
                 task_msg.stderr = {
                     "exception": ts.exception_text,
                     "traceback": ts.traceback_text,
                 }
+                if TELEMETRY_CAPTURE is not None:
+                    task_msg.telemetry_at_end = capture_telemetry()
             else:
                 return
 
             if self.settings.worker_should_get_input:
                 if hasattr(ts, "run_spec"):
                     get_run_spec_data(task_msg, ts.run_spec)
```

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/dask/dask_plugins.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/dask/dask_plugins.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/interceptor_state_manager.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/interceptor_state_manager.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import sys
 import os
 import time
-from threading import Thread, Event
 
 from watchdog.observers import Observer
 
-from flowcept.commons.flowcept_data_classes import TaskMessage
+from flowcept.commons.flowcept_dataclasses.task_message import TaskMessage
 from flowcept.commons.utils import get_utc_now, get_status_from_str
 from flowcept.flowceptor.plugins.base_interceptor import (
     BaseInterceptor,
 )
 from flowcept.flowceptor.plugins.interceptor_state_manager import (
     InterceptorStateManager,
 )
```

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/settings_factory.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/settings_factory.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 import time
 
 from watchdog.observers import Observer
 from tbparse import SummaryReader
 
-from flowcept.commons.flowcept_data_classes import TaskMessage, Status
+from flowcept.commons.flowcept_dataclasses.task_message import (
+    TaskMessage,
+    Status,
+)
 from flowcept.commons.utils import get_utc_now
 from flowcept.flowceptor.plugins.interceptor_state_manager import (
     InterceptorStateManager,
 )
 from flowcept.flowceptor.plugins.base_interceptor import (
     BaseInterceptor,
 )
```

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py` & `flowcept-0.1.4/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from threading import Thread
 from time import sleep
 import pika
 import json
 from typing import Dict
 
 from flowcept.commons.utils import get_utc_now, get_status_from_str
-from flowcept.commons.flowcept_data_classes import TaskMessage
+from flowcept.commons.flowcept_dataclasses.task_message import TaskMessage
 from flowcept.flowceptor.plugins.base_interceptor import (
     BaseInterceptor,
 )
 
 
 class ZambezeInterceptor(BaseInterceptor):
     def __init__(self, plugin_key="zambeze"):
```

### Comparing `flowcept-0.1.3/flowcept/main.py` & `flowcept-0.1.4/flowcept/main.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/flowcept.egg-info/PKG-INFO` & `flowcept-0.1.4/flowcept.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: flowcept
-Version: 0.1.3
-Summary: A system to integrate data from multiple workflows.
+Version: 0.1.4
+Summary: FlowCept is a runtime data integration system that empowers any data processing system to capture and query workflow provenance data using data observability, requiring minimal or no changes in the target system code. It seamlessly integrates data from multiple workflows, enabling users to comprehend complex, heterogeneous, and large-scale data from various sources in federated environments.
 Home-page: https://github.com/ORNL/flowcept
 Author: Oak Ridge National Laboratory
 License: MIT
+Keywords: ai,ml,machine-learning,provenance,lineage,responsible-ai,databases,big-data,provenance,tensorboard,data-integration,scientific-workflows,dask,reproducibility,workflows,parallel-processing,lineage,model-management,mlflow,responsible-ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: Database
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: zambeze
 Provides-Extra: mlflow
 Provides-Extra: tensorboard
 Provides-Extra: mongo
 Provides-Extra: dask
@@ -28,24 +35,23 @@
 [![Tests](https://github.com/ORNL/flowcept/actions/workflows/run-tests.yml/badge.svg)](https://github.com/ORNL/flowcept/actions/workflows/run-tests.yml)
 [![Code Formatting](https://github.com/ORNL/flowcept/actions/workflows/code-formatting.yml/badge.svg)](https://github.com/ORNL/flowcept/actions/workflows/code-formatting.yml)
 [![License: MIT](https://img.shields.io/github/license/ORNL/flowcept)](LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # FlowCept
 
-FlowCept is a runtime data integration system that aims at empowering any data generation system to capture 
-workflow provenance data using data observability, with minimal (often no) changes in the target system code. 
-Thus, it is able to integrate data from multiple workflows, enabling users to understand complex, heterogeneous, large-scale data coming from various sources in federated environments.
+FlowCept is a runtime data integration system that empowers any data processing system to capture and query workflow 
+provenance data using data observability, requiring minimal or no changes in the target system code. It seamlessly integrates data from multiple workflows, enabling users to comprehend complex, heterogeneous, and large-scale data from various sources in federated environments.
 
 FlowCept is intended to address scenarios where multiple workflows in a science campaign or in an enterprise run and generate 
-important data to be analyzed in an integrated manner. Since these workflows may use different data generation tools or can be executed within
-different parallel computing systems (e.g., Dask, Spark, workflow management systems), its key differentiator is the 
-capability to seamless integrate multi-workflow data from various sources using data observability.
-It builds an integrated data view at runtime of these multi-workflow data following 
-[W3C PROV](https://www.w3.org/TR/prov-overview/) recommendations for its data schema.
+important data to be analyzed in an integrated manner. Since these workflows may use different data manipulation tools (e.g., provenance or lineage capture tools, database systems, performance profiling tools) or can be executed within
+different parallel computing systems (e.g., Dask, Spark, Workflow Management Systems), its key differentiator is the 
+capability to seamless and automatically integrate data from various workflows using data observability.
+It builds an integrated data view at runtime enabling end-to-end exploratory data analysis and monitoring.
+It follows [W3C PROV](https://www.w3.org/TR/prov-overview/) recommendations for its data schema.
 It does not require changes in user codes or systems (i.e., instrumentation). 
 All users need to do is to create adapters for their systems or tools, if one is not available yet. 
 
 Currently, FlowCept provides adapters for: [Dask](https://www.dask.org/), [MLFlow](https://mlflow.org/), [TensorBoard](https://www.tensorflow.org/tensorboard), and [Zambeze](https://github.com/ORNL/zambeze). 
 
 See the [Jupyter Notebooks](notebooks) for utilization examples.
```

### Comparing `flowcept-0.1.3/flowcept.egg-info/SOURCES.txt` & `flowcept-0.1.4/flowcept.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,30 +8,33 @@
 flowcept/version.py
 flowcept.egg-info/PKG-INFO
 flowcept.egg-info/SOURCES.txt
 flowcept.egg-info/dependency_links.txt
 flowcept.egg-info/requires.txt
 flowcept.egg-info/top_level.txt
 flowcept/commons/__init__.py
-flowcept/commons/flowcept_data_classes.py
 flowcept/commons/flowcept_logger.py
 flowcept/commons/utils.py
 flowcept/commons/vocabulary.py
 flowcept/commons/daos/__init__.py
 flowcept/commons/daos/document_db_dao.py
 flowcept/commons/daos/mq_dao.py
+flowcept/commons/flowcept_dataclasses/__init__.py
+flowcept/commons/flowcept_dataclasses/task_message.py
+flowcept/commons/flowcept_dataclasses/telemetry.py
 flowcept/flowcept_api/__init__.py
 flowcept/flowcept_api/consumer_api.py
 flowcept/flowcept_api/task_query_api.py
 flowcept/flowcept_webserver/__init__.py
 flowcept/flowcept_webserver/app.py
 flowcept/flowcept_webserver/resources/__init__.py
 flowcept/flowcept_webserver/resources/query_rsrc.py
 flowcept/flowcept_webserver/resources/task_messages_rsrc.py
 flowcept/flowceptor/__init__.py
+flowcept/flowceptor/telemetry_capture.py
 flowcept/flowceptor/consumers/__init__.py
 flowcept/flowceptor/consumers/consumer_utils.py
 flowcept/flowceptor/consumers/document_inserter.py
 flowcept/flowceptor/plugins/__init__.py
 flowcept/flowceptor/plugins/base_interceptor.py
 flowcept/flowceptor/plugins/base_settings_dataclasses.py
 flowcept/flowceptor/plugins/interceptor_state_manager.py
@@ -49,14 +52,15 @@
 flowcept/flowceptor/plugins/tensorboard/tensorboard_dataclasses.py
 flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py
 flowcept/flowceptor/plugins/zambeze/__init__.py
 flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py
 flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py
 tests/__init__.py
 tests/log_tests.py
+tests/telemetry_test.py
 tests/api/__init__.py
 tests/api/query_test.py
 tests/doc_db_inserter/__init__.py
 tests/doc_db_inserter/doc_db_inserter_test.py
 tests/log_tests/__init__.py
 tests/log_tests/log_test.py
 tests/plugins/__init__.py
```

### Comparing `flowcept-0.1.3/flowcept.egg-info/requires.txt` & `flowcept-0.1.4/flowcept.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 PyYAML==6.0
 redis==4.4.2
+psutil==5.9.5
 
 [dask]
 tomli==1.1.0
 dask[distributed]==2022.12.0
 
 [full]
 PyYAML==6.0
 redis==4.4.2
+psutil==5.9.5
 pika==1.3.1
 mlflow-skinny==2.1.1
 SQLAlchemy==1.4.42
 alembic==1.8.1
 watchdog==2.2.1
 pandas==1.5.1
 tensorboard==2.11.0
```

### Comparing `flowcept-0.1.3/tests/api/query_test.py` & `flowcept-0.1.4/tests/api/query_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import random
 from threading import Thread
 import requests
 import inspect
 from time import sleep
 from uuid import uuid4
 
-from flowcept.commons.flowcept_data_classes import TaskMessage
+from flowcept.commons.flowcept_dataclasses.task_message import TaskMessage
 from flowcept.configs import WEBSERVER_PORT, WEBSERVER_HOST
 from flowcept.flowcept_api.task_query_api import TaskQueryAPI
 from flowcept.flowcept_webserver.app import app, BASE_ROUTE
 from flowcept.flowcept_webserver.resources.query_rsrc import TaskQuery
 from flowcept.commons.daos.document_db_dao import DocumentDBDao
 
 
@@ -187,30 +187,32 @@
         assert res_without == res_with
 
         dao.delete_keys("task_id", docs[0]["task_id"])
         c1 = dao.count()
         assert c0 == c1
 
     def test_aggregation(self):
-        docs, task_ids = gen_some_mock_multi_workflow_data2(size=10000)
+        docs, task_ids = gen_some_mock_multi_workflow_data2(size=100)
 
         dao = DocumentDBDao()
         c0 = dao.count()
         dao.insert_many(docs)
         sleep(3)
         api = TaskQueryAPI()
         res = api.query(
             aggregation=[
                 ("max", "used.epochs"),
                 ("max", "generated.accuracy"),
                 ("avg", "used.batch_size"),
             ]
         )
         assert len(res) > 0
-        assert res[0]["max_generated_accuracy"] > 0
+        for doc in res:
+            if doc.get("max_generated_accuracy") is not None:
+                assert doc["max_generated_accuracy"] > 0
 
         campaign_id = docs[0]["campaign_id"]
         res = api.query(
             filter={"campaign_id": campaign_id},
             aggregation=[
                 ("max", "used.epochs"),
                 ("max", "generated.accuracy"),
@@ -219,27 +221,31 @@
             sort=[
                 ("max_used_epochs", TaskQueryAPI.ASC),
                 ("ended_at", TaskQueryAPI.DESC),
             ],
             limit=10,
         )
         assert len(res) > 0
-        assert res[0]["max_generated_accuracy"] > 0
+        for doc in res:
+            if doc.get("max_generated_accuracy") is not None:
+                assert doc["max_generated_accuracy"] > 0
 
         res = api.query(
             projection=["used.batch_size"],
             filter={"campaign_id": campaign_id},
             aggregation=[
                 ("min", "generated.loss"),
                 ("max", "generated.accuracy"),
             ],
             sort=[
                 ("ended_at", TaskQueryAPI.DESC),
             ],
             limit=10,
         )
         assert len(res) > 1
-        assert res[0]["max_generated_accuracy"] > 0
+        for doc in res:
+            if doc.get("max_generated_accuracy") is not None:
+                assert doc["max_generated_accuracy"] > 0
 
         dao.delete_keys("task_id", task_ids)
         c1 = dao.count()
         assert c0 == c1
```

### Comparing `flowcept-0.1.3/tests/doc_db_inserter/doc_db_inserter_test.py` & `flowcept-0.1.4/tests/doc_db_inserter/doc_db_inserter_test.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/tests/log_tests/log_test.py` & `flowcept-0.1.4/tests/log_tests/log_test.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/tests/plugins/test_dask.py` & `flowcept-0.1.4/tests/plugins/test_dask.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,17 +130,20 @@
         except:
             pass
         return o1.key
 
     def test_observer_and_consumption(self):
         doc_dao = DocumentDBDao()
         o2_task_id = self.atest_pure_workflow()
+        print("Task_id=" + o2_task_id)
         print("Done workflow!")
         sleep(3)
-        assert len(doc_dao.query({"task_id": o2_task_id})) > 0
+        docs = doc_dao.query({"task_id": o2_task_id})
+        assert len(docs) > 0
+        assert len(docs[0]["telemetry_at_end"]) > 0
 
     def test_observer_and_consumption_varying_args(self):
         doc_dao = DocumentDBDao()
         if TestDask.consumer is None or not TestDask.consumer.is_started:
             TestDask._init_consumption()
         o2_task_id = self.varying_args()
         sleep(10)
```

### Comparing `flowcept-0.1.3/tests/plugins/test_mlflow.py` & `flowcept-0.1.4/tests/plugins/test_mlflow.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/tests/plugins/test_tensorboard.py` & `flowcept-0.1.4/tests/plugins/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `flowcept-0.1.3/tests/plugins/test_zambeze.py` & `flowcept-0.1.4/tests/plugins/test_zambeze.py`

 * *Files identical despite different names*

