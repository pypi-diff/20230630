# Comparing `tmp/th2_data_services_lwdp-2.1.0.0.dev5400437624.tar.gz` & `tmp/th2_data_services_lwdp-2.1.0.0.dev5423567204.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5400437624.tar", last modified: Wed Jun 28 11:17:31 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5423567204.tar", last modified: Fri Jun 30 13:44:28 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624.tar` & `th2_data_services_lwdp-2.1.0.0.dev5423567204.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-28 11:17:12.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    61099 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    14512 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-28 11:15:56.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-28 11:17:30.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-06-28 11:17:31.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-28 11:17:30.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-28 11:17:30.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-28 11:17:30.000000 th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-30 13:44:16.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61099 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14512 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4508 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.1.0.0.dev5400437624
+Version: 2.1.0.0.dev5423567204
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/README.md` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/setup.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,11 +18,13 @@
 from .page import Page
 
 from th2_data_services.config import options as _o
 
 from th2_data_services.data_source.lwdp.resolver import (
     LwdpEventFieldsResolver,
     LwdpMessageFieldsResolver,
+    SubMessageFieldResolver
 )
 
 _o.EVENT_FIELDS_RESOLVER = LwdpEventFieldsResolver()
 _o.MESSAGE_FIELDS_RESOLVER = LwdpMessageFieldsResolver()
+_o.SUB_MESSAGE_FIELDS_RESOLVER = SubMessageFieldResolver()
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from th2_data_services.interfaces.utils.resolver import EventFieldsResolver, MessageFieldsResolver
+from th2_data_services.interfaces.utils.resolver import EventFieldsResolver, MessageFieldsResolver, SubMessageFieldResolver
 from th2_data_services.data_source.lwdp.struct import http_event_struct, http_message_struct
 
 
 class LwdpEventFieldsResolver(EventFieldsResolver):
     @staticmethod
     def get_id(event):
         return event[http_event_struct.EVENT_ID]
@@ -60,44 +60,28 @@
     @staticmethod
     def get_body(event):
         return event[http_event_struct.BODY]
 
 
 class LwdpMessageFieldsResolver(MessageFieldsResolver):
     @staticmethod
-    def get_subsequence(message):
-        raise NotImplementedError
-
-    @staticmethod
     def get_direction(message):
         return message[http_message_struct.DIRECTION]
 
     @staticmethod
     def get_session_id(message):
         return message[http_message_struct.SESSION_ID]
 
     @staticmethod
     def get_type(message):
-        return message[http_message_struct.MESSAGE_TYPE]
-
-    @staticmethod
-    def get_connection_id(message):
-        return message[http_message_struct.BODY]["metadata"]["id"][
-            http_message_struct.CONNECTION_ID
-        ]
-
-    @staticmethod
-    def get_session_alias(message):
-        return message[http_message_struct.BODY]["metadata"]["id"][
-            http_message_struct.CONNECTION_ID
-        ][http_message_struct.SESSION_ALIAS]
+        raise NotImplementedError
 
     @staticmethod
-    def get_sequence(message):
-        return message[http_message_struct.BODY]["metadata"]["id"][http_message_struct.SEQUENCE]
+    def get_sequence(message): # <book>:<alias>:<direction>:<timestamp>:<sequence>.<\d>.<\d>
+        return message[http_message_struct.MESSAGE_ID].split(':')[4].split('.')[0]
 
     @staticmethod
     def get_timestamp(message):
         return message[http_message_struct.TIMESTAMP]
 
     @staticmethod
     def get_body(message):
@@ -111,10 +95,28 @@
     def get_id(message):
         return message[http_message_struct.MESSAGE_ID]
 
     @staticmethod
     def get_attached_event_ids(message):
         return message[http_message_struct.ATTACHED_EVENT_IDS]
 
+
+class SubMessageFieldResolver(SubMessageFieldResolver):
+    @staticmethod
+    def get_metadata(sub_message):
+        return sub_message["metadata"]
+
+    @staticmethod
+    def get_subsequence(sub_message):
+        return SubMessageFieldResolver.get_metadata(sub_message).get(http_message_struct.SUBSEQUENCE, [1])
+
+    @staticmethod
+    def get_type(sub_message):
+        return SubMessageFieldResolver.get_metadata(sub_message)[http_message_struct.MESSAGE_TYPE]
+
+    @staticmethod
+    def get_protocol(sub_message):
+        return SubMessageFieldResolver.get_metadata(sub_message).get(http_message_struct.PROTOCOL)
+
     @staticmethod
-    def get_fields(message):
-        return message[http_message_struct.BODY]["fields"]
+    def get_fields(sub_message):
+        return sub_message["fields"]
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/struct.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,18 +37,16 @@
 @dataclass
 class MessageStruct(IMessageStruct):
     """Interface for Message of data-provider v5."""
 
     DIRECTION: str
     SESSION_ID: str
     MESSAGE_TYPE: str
-    CONNECTION_ID: str
-    SESSION_ALIAS: str
     SUBSEQUENCE: str
-    SEQUENCE: str
+    PROTOCOL: str
     TIMESTAMP: str
     BODY: str
     BODY_BASE64: str
     MESSAGE_ID: str
     ATTACHED_EVENT_IDS: str
 
 
@@ -81,32 +79,28 @@
 )
 
 # +TODO - unknown fields. Perhaps we have them in GRPC
 http_message_struct = MessageStruct(
     DIRECTION="direction",
     SESSION_ID="sessionId",
     MESSAGE_TYPE="messageType",
-    CONNECTION_ID="connectionId",  # ??
-    SESSION_ALIAS="sessionAlias",  # ??
-    SUBSEQUENCE="subsequence",  # ??
-    SEQUENCE="sequence",  # ??
+    SUBSEQUENCE="subsequence",
+    PROTOCOL="protocol",
     TIMESTAMP="timestamp",
     BODY="body",
     BODY_BASE64="bodyBase64",
     MESSAGE_ID="messageId",
     ATTACHED_EVENT_IDS="attachedEventIds",
 )
 
 grpc_message_struct = MessageStruct(
     DIRECTION="direction",
     SESSION_ID="sessionId",
     MESSAGE_TYPE="messageType",
-    CONNECTION_ID="connectionId",
-    SESSION_ALIAS="sessionAlias",
     SUBSEQUENCE="subsequence",
-    SEQUENCE="sequence",
+    PROTOCOL="protocol",
     TIMESTAMP="timestamp",
     BODY="body",
     BODY_BASE64="bodyBase64",
     MESSAGE_ID="messageId",
     ATTACHED_EVENT_IDS="attachedEventIds",
 )
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
 
         Returns:
             (dict) Message stub template.
         """
         return {
             self.message_fields.DIRECTION: None,
             self.message_fields.SESSION_ID: BrokenMessage(),
-            self.message_fields.MESSAGE_TYPE: BrokenMessage(),
             self.message_fields.TIMESTAMP: {"nano": 0, "epochSecond": 0},
             self.message_fields.BODY: [],
             self.message_fields.BODY_BASE64: [],
             self.message_fields.MESSAGE_ID: self.REQUIRED_FIELD,
             self.message_fields.ATTACHED_EVENT_IDS: [],
         }
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/_misc.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.1.0.0.dev5400437624
+Version: 2.1.0.0.dev5423567204
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5400437624/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

