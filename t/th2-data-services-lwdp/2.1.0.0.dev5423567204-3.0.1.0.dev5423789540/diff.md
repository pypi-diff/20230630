# Comparing `tmp/th2_data_services_lwdp-2.1.0.0.dev5423567204.tar.gz` & `tmp/th2_data_services_lwdp-3.0.1.0.dev5423789540.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5423567204.tar", last modified: Fri Jun 30 13:44:28 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-3.0.1.0.dev5423789540.tar", last modified: Fri Jun 30 14:09:44 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204.tar` & `th2_data_services_lwdp-3.0.1.0.dev5423789540.tar`

### file list

```diff
@@ -1,60 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-30 13:44:16.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    61099 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    14512 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4508 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-30 13:43:00.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-30 13:44:28.000000 th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7683 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-30 14:09:28.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60895 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14524 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4354 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-30 14:08:38.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9661 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-30 14:09:44.000000 th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/PKG-INFO` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.1.0.0.dev5423567204
+Version: 3.0.1.0.dev5423789540
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
@@ -16,16 +16,16 @@
         <!-- start get_started_example.py -->
         ```python
         from typing import List
         
         from th2_data_services.event_tree import EventTreeCollection
         
         from th2_data_services.data_source.lwdp.commands import http as commands
-        from th2_data_services.data_source.lwdp.data_source import HTTPDataSource
-        from th2_data_services.data_source.lwdp.event_tree import HttpETCDriver
+        from th2_data_services.data_source.lwdp.data_source import DataSource
+        from th2_data_services.data_source.lwdp.event_tree import ETCDriver
         from th2_data_services.data_source.lwdp.streams import Streams, Stream
         from th2_data_services.data import Data
         from datetime import datetime
         from th2_data_services.data_source.lwdp.utils import Page
         
         # About this example
         #   The following document shows common features of the library.
@@ -69,15 +69,15 @@
         
         # Date has to be in utc timezone.
         START_TIME = datetime(year=2023, month=1, day=5, hour=13, minute=57, second=5, microsecond=0)
         END_TIME = datetime(year=2023, month=1, day=5, hour=13, minute=57, second=6, microsecond=0)
         
         # [1] Create data source object to connect to lightweight data provider.
         provider_url_link = f"http://10.100.66.105:32681"
-        data_source = HTTPDataSource(provider_url_link)
+        data_source = DataSource(provider_url_link)
         
         # [2] Getting books, pages, scopes, groups and aliases.
         
         # [2.1] Get books.
         #   On database data is segregated with books, such as they never intersect.
         #   To get the names of the books we have a command GetBooks which takes no argument.
         books: List[str] = data_source.command(commands.GetBooks())
@@ -194,15 +194,15 @@
         )
         
         # [4] ETCDriver
         #   To work with EventTreeCollection and its children we need to use special driver.
         #   This driver contains lwdp-related methods that ETC required.
         
         # [4.1] Init driver
-        etc_driver = HttpETCDriver(data_source=data_source, use_stub=False)
+        etc_driver = ETCDriver(data_source=data_source, use_stub=False)
         # [4.2] Init ETC object
         etc = EventTreeCollection(etc_driver)
         
         # [4.3] Build Event Trees inside ETC and recover unknown events if it has them.
         etc.build(events)
         etc.recover_unknown_events()
         # See more info about how to use ETC in th2-data-services lib documentation.
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/README.md` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 <!-- start get_started_example.py -->
 ```python
 from typing import List
 
 from th2_data_services.event_tree import EventTreeCollection
 
 from th2_data_services.data_source.lwdp.commands import http as commands
-from th2_data_services.data_source.lwdp.data_source import HTTPDataSource
-from th2_data_services.data_source.lwdp.event_tree import HttpETCDriver
+from th2_data_services.data_source.lwdp.data_source import DataSource
+from th2_data_services.data_source.lwdp.event_tree import ETCDriver
 from th2_data_services.data_source.lwdp.streams import Streams, Stream
 from th2_data_services.data import Data
 from datetime import datetime
 from th2_data_services.data_source.lwdp.utils import Page
 
 # About this example
 #   The following document shows common features of the library.
@@ -61,15 +61,15 @@
 
 # Date has to be in utc timezone.
 START_TIME = datetime(year=2023, month=1, day=5, hour=13, minute=57, second=5, microsecond=0)
 END_TIME = datetime(year=2023, month=1, day=5, hour=13, minute=57, second=6, microsecond=0)
 
 # [1] Create data source object to connect to lightweight data provider.
 provider_url_link = f"http://10.100.66.105:32681"
-data_source = HTTPDataSource(provider_url_link)
+data_source = DataSource(provider_url_link)
 
 # [2] Getting books, pages, scopes, groups and aliases.
 
 # [2.1] Get books.
 #   On database data is segregated with books, such as they never intersect.
 #   To get the names of the books we have a command GetBooks which takes no argument.
 books: List[str] = data_source.command(commands.GetBooks())
@@ -186,15 +186,15 @@
 )
 
 # [4] ETCDriver
 #   To work with EventTreeCollection and its children we need to use special driver.
 #   This driver contains lwdp-related methods that ETC required.
 
 # [4.1] Init driver
-etc_driver = HttpETCDriver(data_source=data_source, use_stub=False)
+etc_driver = ETCDriver(data_source=data_source, use_stub=False)
 # [4.2] Init ETC object
 etc = EventTreeCollection(etc_driver)
 
 # [4.3] Build Event Trees inside ETC and recover unknown events if it has them.
 etc.build(events)
 etc.recover_unknown_events()
 # See more info about how to use ETC in th2-data-services lib documentation.
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/setup.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .message_response_format import ResponseFormat
 from .streams import Stream, Streams
 from .page import Page
 
 from th2_data_services.config import options as _o
 
 from th2_data_services.data_source.lwdp.resolver import (
-    LwdpEventFieldsResolver,
-    LwdpMessageFieldsResolver,
-    SubMessageFieldResolver
+    EventFieldResolver,
+    MessageFieldResolver,
+    SubMessageFieldResolver,
 )
 
-_o.EVENT_FIELDS_RESOLVER = LwdpEventFieldsResolver()
-_o.MESSAGE_FIELDS_RESOLVER = LwdpMessageFieldsResolver()
+_o.EVENT_FIELDS_RESOLVER = EventFieldResolver()
+_o.MESSAGE_FIELDS_RESOLVER = MessageFieldResolver()
 _o.SUB_MESSAGE_FIELDS_RESOLVER = SubMessageFieldResolver()
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,11 +8,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# from .basic_adapters import GRPCObjectToDictAdapter
-from .event_adapters import DeleteEventWrappersAdapter
-from .message_adapters import DeleteMessageWrappersAdapter
-from .adapter_sse import SSEAdapter
+from abc import ABC
+
+
+class IFilter(ABC):
+    pass
+
+
+ILwDPFilter = IFilter
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
 from th2_data_services.data import Data
 from th2_data_services.exceptions import EventNotFound, MessageNotFound
 from th2_data_services.utils.converters import DatetimeConverter, ProtobufTimestampConverter
 
 from th2_data_services.data_source.lwdp import Page
 from th2_data_services.data_source.lwdp.interfaces.command import IHTTPCommand
-from th2_data_services.data_source.lwdp.data_source.http import HTTPDataSource
-from th2_data_services.data_source.lwdp.source_api.http import HTTPAPI
+from th2_data_services.data_source.lwdp.data_source.http import DataSource
+from th2_data_services.data_source.lwdp.source_api.http import API
 from th2_data_services.data_source.lwdp.streams import Streams, Stream
 from th2_data_services.utils.sse_client import SSEClient
 from th2_data_services.data_source.lwdp.adapters.adapter_sse import (
     SSEAdapter,
     DEFAULT_BUFFER_LIMIT,
 )
 from th2_data_services.utils.decode_error_handler import UNICODE_REPLACE_HANDLER
-from th2_data_services.data_source.lwdp.filters.event_filters import LwDPEventFilter
+from th2_data_services.data_source.lwdp.filters.event_filters import EventFilter
 from th2_data_services.data_source.lwdp.utils import (
     _check_datetime,
     _check_list_or_tuple,
     _check_response_formats,
 )
 from th2_data_services.data_source.lwdp.utils._misc import (
     get_utc_datetime_now,
@@ -99,60 +99,60 @@
         Returns:
             Data
         """
         self._current_handle_function = self._data_object
         return self
 
     def _sse_bytes_stream(
-        self, data_source: HTTPDataSource
+        self, data_source: DataSource
     ) -> Generator[bytes, None, None]:  # noqa
-        api: HTTPAPI = data_source.source_api
+        api: API = data_source.source_api
         urls: List[str] = self._get_urls(data_source)
         for url in urls:
             # LOG             logger.info(url)
             yield from api.execute_sse_request(url)
 
-    def _sse_events_stream(self, data_source: HTTPDataSource) -> Generator[Event, Any, None]:
+    def _sse_events_stream(self, data_source: DataSource) -> Generator[Event, Any, None]:
         """Turns SSEByte Stream Into SSEEvent Stream.
 
         Args:
-            data_source: HTTPDataSource
+            data_source: DataSource
 
         Returns:
              Generator[Event, Any, None]
         """
         sse_bytes_stream = partial(self._sse_bytes_stream, data_source)
 
         client = SSEClient(
             sse_bytes_stream(),
             char_enc=self._char_enc,
             decode_errors_handler=self._decode_error_handler,
         )
         yield from client.events()
 
-    def _data_object(self, data_source: HTTPDataSource) -> Data:
+    def _data_object(self, data_source: DataSource) -> Data:
         """Parses SSEEvents Into Data Object.
 
         Args:
-            data_source: HTTPDataSource
+            data_source: DataSource
 
         Returns:
              Data
         """
         sse_events_stream = partial(self._sse_events_stream, data_source)
         data = Data(sse_events_stream).map_stream(self._sse_handler.handle).use_cache(self._cache)
         data.metadata["urls"] = self._get_urls(data_source)
         return data
 
     @abstractmethod
-    def _get_urls(self, data_source: HTTPDataSource) -> List[str]:
+    def _get_urls(self, data_source: DataSource) -> List[str]:
         pass
 
     def handle(
-        self, data_source: HTTPDataSource
+        self, data_source: DataSource
     ) -> Union[Generator[bytes, None, None], Generator[Event, None, None], Data]:
         """Handles Stream By Handle Function, Defaults To `Data`.
 
         Args:
             data_source: data_source
 
         Returns:
@@ -206,28 +206,28 @@
             _check_datetime(start_timestamp)
             _check_datetime(end_timestamp)
             self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
             self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
             self._all_results = False
         self._book_id = book_id
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         if self._all_results:
             return [api.get_url_get_scopes(book_id=self._book_id)]
         else:
             return [
                 api.get_url_get_scopes(self._book_id, self._start_timestamp, self._end_timestamp)
             ]
 
-    def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
+    def _data_object(self, data_source: DataSource) -> Data[Page]:
         """Parses SSEEvents Into Data Object.
 
         Args:
-            data_source: HTTPDataSource
+            data_source: DataSource
 
         Returns:
              Data
         """
         sse_events_stream = partial(self._sse_events_stream, data_source)
         data = Data(sse_events_stream).map_stream(self._sse_handler).use_cache(self._cache)
         data.metadata["urls"] = self._get_urls(data_source)
@@ -279,30 +279,30 @@
             _check_datetime(start_timestamp)
             _check_datetime(end_timestamp)
             self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
             self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
             self._all_results = False
         self._book_id = book_id
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         if self._all_results:
             return [api.get_url_get_message_aliases(book_id=self._book_id)]
         else:
             return [
                 api.get_url_get_message_aliases(
                     self._book_id, self._start_timestamp, self._end_timestamp
                 )
             ]
 
-    def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
+    def _data_object(self, data_source: DataSource) -> Data[Page]:
         """Parses SSEEvents Into Data Object.
 
         Args:
-            data_source: HTTPDataSource
+            data_source: DataSource
 
         Returns:
              Data
         """
         sse_events_stream = partial(self._sse_events_stream, data_source)
         data = Data(sse_events_stream).map_stream(self._sse_handler).use_cache(self._cache)
         data.metadata["urls"] = self._get_urls(data_source)
@@ -354,30 +354,30 @@
             _check_datetime(start_timestamp)
             _check_datetime(end_timestamp)
             self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
             self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
             self._all_results = False
         self._book_id = book_id
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         if self._all_results:
             return [api.get_url_get_message_groups(book_id=self._book_id)]
         else:
             return [
                 api.get_url_get_message_groups(
                     self._book_id, self._start_timestamp, self._end_timestamp
                 )
             ]
 
-    def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
+    def _data_object(self, data_source: DataSource) -> Data[Page]:
         """Parses SSEEvents Into Data Object.
 
         Args:
-            data_source: HTTPDataSource
+            data_source: DataSource
 
         Returns:
              Data
         """
         sse_events_stream = partial(self._sse_events_stream, data_source)
         data = Data(sse_events_stream).map_stream(self._sse_handler).use_cache(self._cache)
         data.metadata["urls"] = self._get_urls(data_source)
@@ -393,16 +393,16 @@
         dict: List[str].
     """
 
     def __init__(self):
         """GetBooks constructor."""
         super().__init__()
 
-    def handle(self, data_source: HTTPDataSource) -> List[str]:  # noqa: D102
-        api: HTTPAPI = data_source.source_api
+    def handle(self, data_source: DataSource) -> List[str]:  # noqa: D102
+        api: API = data_source.source_api
         url = api.get_url_get_books()
 
         # LOG         logger.info(url)
 
         return api.execute_request(url).json()
 
 
@@ -425,15 +425,15 @@
             book_id: Book to search inside.
             page_name: Page name to search for.
         """
         super().__init__()
         self._book_id = book_id
         self._page_name = page_name
 
-    def handle(self, data_source: HTTPDataSource) -> Page:  # noqa: D102
+    def handle(self, data_source: DataSource) -> Page:  # noqa: D102
         pages = data_source.command(GetPages(self._book_id)).filter(
             lambda page: page.name == self._page_name
         )
         for page in pages:
             return page
         else:
             raise PageNotFound(self._page_name, self._book_id)
@@ -479,34 +479,34 @@
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
         self._book_id = book_id
         self._result_limit = result_limit
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         if self._all_results:
             return [api.get_url_get_pages_info_all(self._book_id)]
         else:
             return [
                 api.get_url_get_pages_info(
                     self._book_id, self._start_timestamp, self._end_timestamp, self._result_limit
                 )
             ]
 
     def to_pages(self, stream):  # noqa
         for event_data in stream:
             yield Page(event_data)
 
-    def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
+    def _data_object(self, data_source: DataSource) -> Data[Page]:
         """Parses SSEEvents Into Data Object.
 
         Args:
-            data_source: HTTPDataSource
+            data_source: DataSource
 
         Returns:
              Data
         """
         sse_events_stream = partial(self._sse_events_stream, data_source)
         data = (
             Data(sse_events_stream)
@@ -538,16 +538,16 @@
             use_stub: If True the command returns stub instead of exception.
 
         """
         super().__init__()
         self._id = id
         self._stub_status = use_stub
 
-    def handle(self, data_source: HTTPDataSource) -> dict:  # noqa: D102
-        api: HTTPAPI = data_source.source_api
+    def handle(self, data_source: DataSource) -> dict:  # noqa: D102
+        api: API = data_source.source_api
         url = api.get_url_find_event_by_id(self._id)
 
         # LOG         logger.info(url)
 
         response = api.execute_request(url)
         # +TODO - perhaps we have to move it to api.execute_request
         if response.status_code == 404 and self._stub_status:
@@ -582,15 +582,15 @@
             use_stub: If True the command returns stub instead of exception.
 
         """
         super().__init__()
         self._ids: ids = ids
         self._stub_status = use_stub
 
-    def handle(self, data_source: HTTPDataSource) -> List[dict]:  # noqa: D102
+    def handle(self, data_source: DataSource) -> List[dict]:  # noqa: D102
         result = []
         for event_id in self._ids:
             event = GetEventById(event_id, use_stub=self._stub_status).handle(data_source)
             result.append(event)
 
         return result
 
@@ -607,15 +607,15 @@
     def __init__(
         self,
         page: Union[Page, str],
         book_id: str = None,
         parent_event: str = None,
         search_direction: str = "next",
         result_count_limit: int = None,
-        filters: Union[LwDPEventFilter, List[LwDPEventFilter]] = None,
+        filters: Union[EventFilter, List[EventFilter]] = None,
         cache: bool = False,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         buffer_limit=DEFAULT_BUFFER_LIMIT,
     ):
         """GetEventsByPage Constructor.
 
@@ -639,15 +639,15 @@
         self._book_id = book_id
         self._parent_event = parent_event
         self._result_count_limit = result_count_limit
         self._search_direction = search_direction
         self._filters = filters
         self._cache = cache
 
-    def handle(self, data_source: HTTPDataSource):
+    def handle(self, data_source: DataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         self._start_timestamp = ProtobufTimestampConverter.to_datetime(page.start_timestamp)
         self._end_timestamp = (
             get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_datetime(page.end_timestamp)
         )
@@ -692,15 +692,15 @@
         start_timestamp: datetime,
         book_id: str,
         scopes: List[str],
         end_timestamp: Optional[datetime] = None,
         parent_event: str = None,
         search_direction: str = "next",
         result_count_limit: int = None,
-        filters: Union[LwDPEventFilter, List[LwDPEventFilter]] = None,
+        filters: Union[EventFilter, List[EventFilter]] = None,
         # Non-data source args.
         # +TODO - add `max_url_length: int = 2048,`
         #   It'll be required when you implement `__split_requests` in source_api/http.py
         cache: bool = False,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
@@ -741,22 +741,22 @@
         )
         self._parent_event = parent_event
         self._search_direction = search_direction
         self._result_count_limit = result_count_limit
         self._filters = filters
         self._book_id = book_id
         self._scopes = scopes
-        if isinstance(filters, LwDPEventFilter):
+        if isinstance(filters, EventFilter):
             self._filters = filters.url()
         elif isinstance(filters, (tuple, list)):
             self._filters = "".join([filter_.url() for filter_ in filters])
 
         _check_list_or_tuple(self._scopes, var_name="scopes")
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         return [
             api.get_url_search_sse_events(
                 start_timestamp=self._start_timestamp,
                 end_timestamp=self._end_timestamp,
                 parent_event=self._parent_event,
                 search_direction=self._search_direction,
@@ -782,15 +782,15 @@
         self,
         page: Union[Page, str],
         scopes: List[str],
         book_id: str = None,
         parent_event: str = None,
         search_direction: str = "next",
         result_count_limit: int = None,
-        filters: Union[LwDPEventFilter, List[LwDPEventFilter]] = None,
+        filters: Union[EventFilter, List[EventFilter]] = None,
         # Non-data source args.
         # +TODO - add `max_url_length: int = 2048,`
         #   It'll be required when you implement `__split_requests` in source_api/http.py
         cache: bool = False,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         buffer_limit=DEFAULT_BUFFER_LIMIT,
@@ -824,22 +824,22 @@
         self._page = page
         self._book_id = book_id
         self._parent_event = parent_event
         self._search_direction = search_direction
         self._result_count_limit = result_count_limit
         self._filters = filters
         self._scopes = scopes
-        if isinstance(filters, LwDPEventFilter):
+        if isinstance(filters, EventFilter):
             self._filters = filters.url()
         elif isinstance(filters, (tuple, list)):
             self._filters = "".join([filter_.url() for filter_ in filters])
 
         _check_list_or_tuple(self._scopes, var_name="scopes")
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
         self._end_timestamp = (
             get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
         )
@@ -882,16 +882,16 @@
 
         """
         super().__init__()
         self._id = id
         self._stub_status = use_stub
         self._response_formats = response_formats
 
-    def handle(self, data_source: HTTPDataSource) -> dict:  # noqa: D102
-        api: HTTPAPI = data_source.source_api
+    def handle(self, data_source: DataSource) -> dict:  # noqa: D102
+        api: API = data_source.source_api
         if self._response_formats in [["JSON_PARSED", "BASE_64"], ["BASE_64", "JSON_PARSED"], None]:
             only_raw = False
         elif self._response_formats == ["BASE_64"]:
             only_raw = True
         else:
             raise Exception(
                 "response_formats should be either ['BASE_64'] or ['JSON_PARSED','BASE_64']"
@@ -936,15 +936,15 @@
 
         """
         super().__init__()
         self._ids: ids = ids
         self._stub_status = use_stub
         self._response_formats = response_formats
 
-    def handle(self, data_source: HTTPDataSource) -> List[dict]:  # noqa: D102
+    def handle(self, data_source: DataSource) -> List[dict]:  # noqa: D102
         result = []
         for message_id in self._ids:
             message = GetMessageById(
                 message_id,
                 use_stub=self._stub_status,
                 response_formats=self._response_formats,
             ).handle(data_source)
@@ -1047,15 +1047,15 @@
                     self._streams.append(stream)
         else:
             raise TypeError(
                 f"streams argument has to be list, tuple or Streams type. "
                 f"Got {type(self._streams)}"
             )
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         return api.get_url_search_sse_messages(
             start_timestamp=self._start_timestamp,
             message_ids=self._message_ids,
             stream=self._streams,
             search_direction=self._search_direction,
             result_count_limit=self._result_count_limit,
@@ -1107,15 +1107,15 @@
         self._page = page
         self._book_id = book_id
         self._sort = sort
         self._response_formats = response_formats
         self._keep_open = keep_open
         self._max_url_length = max_url_length
 
-    def handle(self, data_source: HTTPDataSource):
+    def handle(self, data_source: DataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         start_timestamp = ProtobufTimestampConverter.to_datetime(page.start_timestamp)
         end_timestamp = (
             get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_datetime(page.end_timestamp)
         )
@@ -1187,15 +1187,15 @@
         self._sort = sort
         self._response_formats = response_formats
         self._keep_open = keep_open
         self._max_url_length = max_url_length
 
         _check_list_or_tuple(self._groups, var_name="groups")
 
-    def handle(self, data_source: HTTPDataSource):
+    def handle(self, data_source: DataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
         self._end_timestamp = (
             get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
         )
@@ -1277,15 +1277,15 @@
         self._response_formats = response_formats
         self._keep_open = keep_open
         self._book_id = book_id
         self._max_url_length = max_url_length
 
         _check_list_or_tuple(self._groups, var_name="groups")
 
-    def handle(self, data_source: HTTPDataSource):
+    def handle(self, data_source: DataSource):
         api = data_source.source_api
         urls = api.get_download_messages(
             start_timestamp=self._start_timestamp,
             end_timestamp=self._end_timestamp,
             book_id=self._book_id,
             groups=self._groups,
             sort=self._sort,
@@ -1370,15 +1370,15 @@
         self._response_formats = response_formats
         self._keep_open = keep_open
         self._book_id = book_id
         self._max_url_length = max_url_length
 
         _check_list_or_tuple(self._groups, var_name="groups")
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         return api.get_url_search_messages_by_groups(
             start_timestamp=self._start_timestamp,
             end_timestamp=self._end_timestamp,
             groups=self._groups,
             response_formats=self._response_formats,
             keep_open=self._keep_open,
@@ -1434,15 +1434,15 @@
         self._book_id = book_id
         self._sort = sort
         self._response_formats = response_formats
         self._keep_open = keep_open
         self._max_url_length = max_url_length
         self._cache = cache
 
-    def handle(self, data_source: HTTPDataSource):
+    def handle(self, data_source: DataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         start_timestamp = ProtobufTimestampConverter.to_datetime(page.start_timestamp)
         end_timestamp = (
             get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_datetime(page.end_timestamp)
         )
@@ -1526,15 +1526,15 @@
         self._search_direction = search_direction
         self._response_formats = response_formats
         self._message_ids = message_ids
         self._keep_open = keep_open
         self._max_url_length = max_url_length
         self._stream = stream
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
         self._end_timestamp = (
             get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
         )
@@ -1611,15 +1611,15 @@
         self._sort = sort
         self._response_formats = response_formats
         self._keep_open = keep_open
         self._max_url_length = max_url_length
 
         _check_list_or_tuple(self._groups, var_name="groups")
 
-    def _get_urls(self, data_source: HTTPDataSource):
+    def _get_urls(self, data_source: DataSource):
         page = _get_page_object(self._book_id, self._page, data_source)
         self._start_timestamp = ProtobufTimestampConverter.to_nanoseconds(page.start_timestamp)
         self._end_timestamp = (
             get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
         )
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-# from .grpc import GRPCDataSource
-from .http import HTTPDataSource
+
+from .http import API, HTTPAPI
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,95 +8,100 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from __future__ import annotations
-from typing import Any
 
-from grpc._channel import _InactiveRpcError
+# LOG import logging
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
 from th2_data_services.exceptions import CommandError
-from th2_data_services.interfaces import IEventStruct, IMessageStruct
+from th2_data_services.interfaces import IEventStruct, IMessageStruct, IEventStub, IMessageStub
 
-if TYPE_CHECKING:
-    from th2_data_services.data_source.lwdp.interfaces.command import IGRPCCommand
-
-from th2_data_services.data_source.lwdp.interfaces.data_source import IGRPCDataSource
 
-import logging
+if TYPE_CHECKING:
+    from th2_data_services.data_source.lwdp.interfaces.command import IHTTPCommand
 
-from th2_data_services.data_source.lwdp.stub_builder import IEventStub, IMessageStub
-from th2_data_services.data_source.lwdp.source_api import GRPCAPI
 from th2_data_services.data_source.lwdp.struct import (
-    grpc_message_struct,
-    grpc_event_struct,
+    event_struct,
+    message_struct,
+    EventStruct,
+    MessageStruct,
 )
 from th2_data_services.data_source.lwdp.stub_builder import (
-    grpc_event_stub_builder,
-    grpc_message_stub_builder,
+    event_stub_builder,
+    message_stub_builder,
+    EventStubBuilder,
+    MessageStubBuilder,
 )
+from th2_data_services.data_source.lwdp.source_api.http import API
+from th2_data_services.data_source.lwdp.interfaces.data_source import IHTTPDataSource
 
-logger = logging.getLogger(__name__)
+# LOG logger = logging.getLogger(__name__)
 
 
-class GRPCDataSource(IGRPCDataSource):
-    """DataSource class which provide work with lw-data-provider.
-
-    Protocol: GRPC
-    """
+class DataSource(
+    IHTTPDataSource[EventStruct, MessageStruct, EventStubBuilder, MessageStubBuilder]
+):
+    """DataSource class which provide work with http LwDP."""
 
     def __init__(
         self,
         url: str,
-        event_struct: IEventStruct = grpc_event_struct,
-        message_struct: IMessageStruct = grpc_message_struct,
-        event_stub_builder: IEventStub = grpc_event_stub_builder,
-        message_stub_builder: IMessageStub = grpc_message_stub_builder,
+        chunk_length: int = 65536,
+        event_struct: IEventStruct = event_struct,
+        message_struct: IMessageStruct = message_struct,
+        event_stub_builder: IEventStub = event_stub_builder,
+        message_stub_builder: IMessageStub = message_stub_builder,
+        check_connect_timeout: Union[int, float] = 5,
     ):
-        """GRPCDataSource constructor.
+        """DataSource constructor.
 
         Args:
-            url: Url of lw-data-provider.
-            event_struct: Event structure that is supplied by lw-data-provider.
-            message_struct: Message structure that is supplied by lw-data-provider.
-            event_stub_builder: Stub builder for broken events.
-            message_stub_builder: Stub builder for broken messages.
+            url: HTTP data source url.
+            check_connect_timeout: How many seconds to wait for the server to send data before giving up.
+            chunk_length: How much of the content to read in one chunk.
+            decode_error_handler: Registered decode error handler.
+            event_struct: Struct of event from rpt-data-provider.
+            message_struct: Struct of message from rpt-data-provider.
+            event_stub_builder: Stub for event.
+            message_stub_builder: Stub for message.
         """
         super().__init__(
-            url=url,
-            event_struct=event_struct,
-            message_struct=message_struct,
-            event_stub_builder=event_stub_builder,
-            message_stub_builder=message_stub_builder,
+            url, event_struct, message_struct, event_stub_builder, message_stub_builder
         )
 
-        self.__provider_api = GRPCAPI(url)
+        self.__chunk_length = chunk_length
+        self.check_connect(check_connect_timeout)
+        self._provider_api = API(url, chunk_length)
 
-        logger.info(url)
+    # LOG         logger.info(url)
 
-    def command(self, cmd: IGRPCCommand) -> Any:
-        """Execute the transmitted GRPC command.
+    def command(self, cmd: IHTTPCommand):
+        """HTTP  command processor.
 
         Args:
-            cmd: GRPC Command.
+            cmd: The command of data source to execute.
 
         Returns:
-            Any: Command response.
+            Data source command result.
 
         Raises:
             CommandError: If the command was broken.
         """
         try:
             return cmd.handle(data_source=self)
-        except _InactiveRpcError as info:
+        except Exception as e:
             raise CommandError(
-                f"The command '{cmd.__class__.__name__}' was broken. Details of error:\n{info.details()}"
+                f"The command '{cmd.__class__.__name__}' was broken. Details of error:\n{e}"
             )
 
     @property
-    def source_api(self) -> GRPCAPI:
-        """Returns Provider API."""
-        return self.__provider_api
+    def source_api(self) -> API:
+        """HTTP  API."""
+        return self._provider_api
+
+
+HTTPDataSource = DataSource
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-
-from .http_etc_driver import HttpETCDriver
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 #  limitations under the License.
 
 from typing import Sequence, Optional
 from th2_data_services.event_tree import IETCDriver
 from th2_data_services.event_tree.etc_driver import Th2EventType
 from th2_data_services.event_tree.exceptions import FieldIsNotExist
 from th2_data_services.data_source.lwdp.commands.http import GetEventsById
-from th2_data_services.data_source.lwdp.interfaces.data_source import ILwDPDataSource
-from th2_data_services.data_source.lwdp.struct import EventStruct, http_event_struct
-from th2_data_services.data_source.lwdp.stub_builder import http_event_stub_builder
+from th2_data_services.data_source.lwdp.interfaces.data_source import IHTTPDataSource
+from th2_data_services.data_source.lwdp.struct import EventStruct, event_struct
+from th2_data_services.data_source.lwdp.stub_builder import event_stub_builder
 
 
-class HttpETCDriver(IETCDriver):
+class ETCDriver(IETCDriver):
     def __init__(
         self,
-        data_source: ILwDPDataSource = None,
-        event_struct: EventStruct = http_event_struct,
+        data_source: IHTTPDataSource = None,
+        event_struct: EventStruct = event_struct,
         use_stub: bool = False,
     ):
         """The driver for EventsTreeCollection (HTTP).
 
         Args:
             event_struct: Structure of the event.
-            data_source: LwDPDataSource object.
+            data_source: DataSource.
             use_stub: Build stubs or not.
         """
         super().__init__(data_source=data_source, event_struct=event_struct, use_stub=use_stub)
 
     def get_events_by_id_from_source(self, ids: Sequence) -> list:
         """Downloads the list of events from the provided data_source.
 
@@ -91,11 +91,14 @@
 
         Args:
             id_: Event Id.
 
         Returns:
             Stub event.
         """
-        return http_event_stub_builder.build({self.event_struct.EVENT_ID: id_})
+        return event_stub_builder.build({self.event_struct.EVENT_ID: id_})
 
     def stub_event_name(self):
-        return http_event_stub_builder.template[self.event_struct.NAME]
+        return event_stub_builder.template[self.event_struct.NAME]
+
+
+HttpETCDriver = ETCDriver
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from th2_data_services.data_source.lwdp.filters.filter import LwDPEventFilter
+from th2_data_services.data_source.lwdp.filters.filter import EventFilter
 
 
-class TypeFilter(LwDPEventFilter):
+class TypeFilter(EventFilter):
     """Will match the events which type contains one of the given substrings."""
 
     FILTER_NAME = "type"
 
 
-class NameFilter(LwDPEventFilter):
+class NameFilter(EventFilter):
     """Will match the events which name contains one of the given substrings."""
 
     FILTER_NAME = "name"
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,24 +8,18 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from th2_data_services.data_source.lwdp.interfaces.filter import ILwDPFilter
+from th2_data_services.data_source.lwdp.interfaces.filter import IFilter
 from typing import Sequence, Any, Union
 
-# from th2_grpc_lw_data_provider.lw_data_provider_pb2 import (
-#     Filter as grpc_Filter,
-#     FilterName as grpc_FilterName,
-# )
-
-
-class LwDPFilter(ILwDPFilter):
+class Filter(IFilter):
     """General interface for Filters of Provider v6."""
 
     def __init__(
         self,
         name: str,
         values: Union[str, int, float, Sequence[Union[str, int, float]]],
         negative: bool = False,
@@ -73,26 +67,21 @@
         return (
             f"&filters={self.name}"
             + "".join([f"&{self.name}-values={val}" for val in self.values])
             + f"&{self.name}-negative={self.negative}"
             + f"&{self.name}-conjunct={self.conjunct}"
         )
 
-    # def grpc(self) -> grpc_Filter:
-    #     """Generates the grpc object of the GRPC protocol API."""
-    #     return grpc_Filter(
-    #         name=grpc_FilterName(name=self.name),
-    #         negative=google.protobuf.wrappers_pb2.BoolValue(value=self.negative),
-    #         value=self.values,
-    #         conjunct=google.protobuf.wrappers_pb2.BoolValue(value=self.conjunct),
-    #     )
 
-
-class _LwDPFilterBase(LwDPFilter):
+class _FilterBase(Filter):
     FILTER_NAME = "FILTER_NAME"
 
     def __init__(self, values: Sequence[Any], negative: bool = False, conjunct: bool = False):
         super().__init__(self.FILTER_NAME, values, negative, conjunct)
 
 
-class LwDPEventFilter(_LwDPFilterBase):
+class EventFilter(_FilterBase):
     """Base class for Event Filters of LwDP."""
+
+LwDPFilter = Filter
+_LwDPFilterBase = _FilterBase
+LwDPEventFilter = EventFilter
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+
+from .http_etc_driver import ETCDriver, HttpETCDriver
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from abc import abstractmethod
 from th2_data_services.data_source.lwdp.interfaces.data_source import (
     ILwDPDataSource,
-    IGRPCDataSource,
     IHTTPDataSource,
 )
 from th2_data_services.interfaces import ICommand
 
 
 class ILwDPCommand(ICommand):
     """Interface of command for lwdp-data-provider."""
@@ -32,18 +31,7 @@
 class IHTTPCommand(ILwDPCommand):
     """Interface of command for rpt-data-provider which works via HTTP."""
 
     @abstractmethod
     def handle(self, data_source: IHTTPDataSource):
         pass
 
-
-class IGRPCCommand(ILwDPCommand):
-    """Interface of command for lwdp-data-provider.
-
-    Lwdp-data-provider version: 1.1.x
-    Protocol: GRPC
-    """
-
-    @abstractmethod
-    def handle(self, data_source: IGRPCDataSource):
-        pass
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,43 +9,38 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from abc import abstractmethod
-from typing import TYPE_CHECKING, TypeVar, Generic
+from typing import TYPE_CHECKING, TypeVar, Generic, Tuple
 
 import requests
 import urllib3
 
 if TYPE_CHECKING:
-    from th2_data_services.data_source.lwdp.interfaces.command import IGRPCCommand, ILwDPCommand
+    from th2_data_services.interfaces import ILwDPCommand
 
-from th2_data_services.interfaces import IDataSource
-from th2_data_services.data_source.lwdp.interfaces.source_api import (
-    IGRPCSourceAPI,
-    ILwDPSourceAPI,
-    IHTTPSourceAPI,
-)
+from th2_data_services.interfaces.data_source import IDataSource
+from th2_data_services.data_source.lwdp.interfaces.source_api import IHTTPSourceAPI 
 from th2_data_services.data_source.lwdp.struct import IEventStruct, IMessageStruct
 from th2_data_services.data_source.lwdp.stub_builder import IEventStub, IMessageStub
 
 CommandT = TypeVar("CommandT", bound="ILwDPCommand")
 EventStructT = TypeVar("EventStructT", bound="IEventStruct")
 MessageStructT = TypeVar("MessageStructT", bound="IMessageStruct")
 EventStubBuilderT = TypeVar("EventStubBuilderT", bound="IEventStub")
 MessageStubBuilderT = TypeVar("MessageStubBuilderT", bound="IMessageStub")
 
 
 # LOG import logging
 
 # LOG logger = logging.getLogger(__name__)
 
-
 class ILwDPDataSource(
     IDataSource, Generic[EventStructT, MessageStructT, EventStubBuilderT, MessageStubBuilderT]
 ):
     def __init__(
         self,
         url: str,
         event_struct: IEventStruct,
@@ -97,43 +92,28 @@
 
     @abstractmethod
     def command(self, cmd: CommandT):
         """Execute the transmitted command."""
 
     @property
     @abstractmethod
-    def source_api(self) -> ILwDPSourceAPI:
+    def source_api(self) -> IHTTPSourceAPI:
         """Returns Provider API."""
 
-
-class IGRPCDataSource(
-    ILwDPDataSource, Generic[EventStructT, MessageStructT, EventStubBuilderT, MessageStubBuilderT]
-):
-    """Interface of DataSource that provides work with lwdp-data-provider via GRPC."""
-
-    @abstractmethod
-    def command(self, cmd: "IGRPCCommand"):
-        """Execute the transmitted GRPC command."""
-
-    @property
-    @abstractmethod
-    def source_api(self) -> IGRPCSourceAPI:
-        """Returns GRPC Provider API."""
-
-
+ 
 class IHTTPDataSource(
     ILwDPDataSource, Generic[EventStructT, MessageStructT, EventStubBuilderT, MessageStubBuilderT]
 ):
     """Interface of DataSource that provides work with lwdp-data-provider via HTTP."""
 
     @abstractmethod
     def command(self, cmd):
         """Execute the transmitted HTTP command."""
 
-    def check_connect(self, timeout: (int, float), certification: bool = True) -> None:
+    def check_connect(self, timeout: Tuple[int, float], certification: bool = True) -> None:
         """Checks whether url is working.
 
         Args:
             timeout: How many seconds to wait for the server to send data before giving up.
             certification: Checking SSL certification.
 
         Raises:
@@ -145,8 +125,8 @@
             raise urllib3.exceptions.HTTPError(
                 f"Unable to connect to host '{self.url}'\nReason: {error}"
             )
 
     @property
     @abstractmethod
     def source_api(self) -> IHTTPSourceAPI:
-        """Returns HTTP Provider API."""
+        """Returns HTTP Provider API."""
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,12 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from abc import ABC
-
-
-class ILwDPFilter(ABC):
-    pass
+from .adapter_sse import SSEAdapter
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,9 @@
 
 from th2_data_services.interfaces import ISourceAPI
 
 
 class ILwDPSourceAPI(ISourceAPI):
     """Interface for Source API of lwdp-data-provider."""
 
-
-class IGRPCSourceAPI(ILwDPSourceAPI):
-    """Interface for Source API of lwdp-data-provider which works via GRPC."""
-
-
 class IHTTPSourceAPI(ILwDPSourceAPI):
     """Interface for Source API of lwdp-data-provider which works via HTTP."""
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/resolver.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,115 +8,122 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from th2_data_services.interfaces.utils.resolver import EventFieldsResolver, MessageFieldsResolver, SubMessageFieldResolver
-from th2_data_services.data_source.lwdp.struct import http_event_struct, http_message_struct
+from th2_data_services.interfaces.utils import resolver as resolver_core
+from th2_data_services.data_source.lwdp.struct import event_struct, message_struct
 
 
-class LwdpEventFieldsResolver(EventFieldsResolver):
+class EventFieldResolver(resolver_core.EventFieldResolver):
     @staticmethod
     def get_id(event):
-        return event[http_event_struct.EVENT_ID]
+        return event[event_struct.EVENT_ID]
 
     @staticmethod
     def get_parent_id(event):
-        return event[http_event_struct.PARENT_EVENT_ID]
+        return event[event_struct.PARENT_EVENT_ID]
 
     @staticmethod
     def get_status(event):
-        return event[http_event_struct.STATUS]
+        return event[event_struct.STATUS]
 
     @staticmethod
     def get_name(event):
-        return event[http_event_struct.NAME]
+        return event[event_struct.NAME]
 
     @staticmethod
     def get_batch_id(event):
-        return event[http_event_struct.BATCH_ID]
+        return event[event_struct.BATCH_ID]
 
     @staticmethod
     def get_is_batched(event):
-        return event[http_event_struct.IS_BATCHED]
+        return event[event_struct.IS_BATCHED]
 
     @staticmethod
     def get_type(event):
-        return event[http_event_struct.EVENT_TYPE]
+        return event[event_struct.EVENT_TYPE]
 
     @staticmethod
     def get_start_timestamp(event):
-        return event[http_event_struct.START_TIMESTAMP]
+        return event[event_struct.START_TIMESTAMP]
 
     @staticmethod
     def get_end_timestamp(event):
-        return event[http_event_struct.END_TIMESTAMP]
+        return event[event_struct.END_TIMESTAMP]
 
     @staticmethod
     def get_attached_messages_ids(event):
-        return event[http_event_struct.ATTACHED_MESSAGES_IDS]
+        return event[event_struct.ATTACHED_MESSAGES_IDS]
 
     @staticmethod
     def get_body(event):
-        return event[http_event_struct.BODY]
+        return event[event_struct.BODY]
 
 
-class LwdpMessageFieldsResolver(MessageFieldsResolver):
+class MessageFieldResolver(resolver_core.MessageFieldResolver):
     @staticmethod
     def get_direction(message):
-        return message[http_message_struct.DIRECTION]
+        return message[message_struct.DIRECTION]
 
     @staticmethod
     def get_session_id(message):
-        return message[http_message_struct.SESSION_ID]
+        return message[message_struct.SESSION_ID]
 
     @staticmethod
     def get_type(message):
         raise NotImplementedError
 
     @staticmethod
-    def get_sequence(message): # <book>:<alias>:<direction>:<timestamp>:<sequence>.<\d>.<\d>
-        return message[http_message_struct.MESSAGE_ID].split(':')[4].split('.')[0]
+    def get_sequence(message):  # <book>:<alias>:<direction>:<timestamp>:<sequence>.<\d>.<\d>
+        return message[message_struct.MESSAGE_ID].split(":")[4].split(".")[0]
 
     @staticmethod
     def get_timestamp(message):
-        return message[http_message_struct.TIMESTAMP]
+        return message[message_struct.TIMESTAMP]
 
     @staticmethod
     def get_body(message):
-        return message[http_message_struct.BODY]
+        return message[message_struct.BODY]
 
     @staticmethod
     def get_body_base64(message):
-        return message[http_message_struct.BODY_BASE64]
+        return message[message_struct.BODY_BASE64]
 
     @staticmethod
     def get_id(message):
-        return message[http_message_struct.MESSAGE_ID]
+        return message[message_struct.MESSAGE_ID]
 
     @staticmethod
     def get_attached_event_ids(message):
-        return message[http_message_struct.ATTACHED_EVENT_IDS]
+        return message[message_struct.ATTACHED_EVENT_IDS]
 
 
-class SubMessageFieldResolver(SubMessageFieldResolver):
+class SubMessageFieldResolver(resolver_core.SubMessageFieldResolver):
     @staticmethod
     def get_metadata(sub_message):
         return sub_message["metadata"]
 
     @staticmethod
     def get_subsequence(sub_message):
-        return SubMessageFieldResolver.get_metadata(sub_message).get(http_message_struct.SUBSEQUENCE, [1])
+        return SubMessageFieldResolver.get_metadata(sub_message).get(
+            message_struct.SUBSEQUENCE, [1]
+        )
 
     @staticmethod
     def get_type(sub_message):
-        return SubMessageFieldResolver.get_metadata(sub_message)[http_message_struct.MESSAGE_TYPE]
+        return SubMessageFieldResolver.get_metadata(sub_message)[message_struct.MESSAGE_TYPE]
 
     @staticmethod
     def get_protocol(sub_message):
-        return SubMessageFieldResolver.get_metadata(sub_message).get(http_message_struct.PROTOCOL)
+        return SubMessageFieldResolver.get_metadata(sub_message).get(message_struct.PROTOCOL)
 
     @staticmethod
     def get_fields(sub_message):
         return sub_message["fields"]
+
+
+# TODO - for backward compatibility. Should be removed some time.
+LwdpEventFieldsResolver = EventFieldResolver
+LwdpMessageFieldsResolver = MessageFieldResolver
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,10 +7,8 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-
-# from .grpc import GRPCAPI
-from .http import HTTPAPI
+from .http import DataSource, HTTPDataSource
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,422 +8,394 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import logging
-from collections import namedtuple
-from typing import Iterable, List, Optional, Union
-
-from google.protobuf.timestamp_pb2 import Timestamp
-from google.protobuf.wrappers_pb2 import BoolValue, Int32Value
-from th2_grpc_common.common_pb2 import MessageID, EventID, ConnectionID, Direction
-from th2_grpc_lw_data_provider.lw_data_provider_pb2_grpc import DataProviderStub
-from th2_grpc_lw_data_provider.lw_data_provider_pb2 import (
-    EventScope,
-    BookId,
-    BooksResponse,
-    BooksRequest,
-    EventResponse,
-    MessageGroupResponse,
-    MessageGroupsSearchRequest,
-    MessageStreamsResponse,
-    MessageStreamsRequest,
-    MessageSearchResponse,
-    EventSearchResponse,
-    EventSearchRequest,
-    MessageSearchRequest,
-    TimeRelation,
-    MessageStream,
-    MessageStreamPointer,
-)
-from grpc import Channel, insecure_channel
-from th2_data_services.data_source.lwdp.interfaces.source_api import IGRPCSourceAPI
-from th2_data_services.data_source.lwdp.streams import Streams
-from th2_data_services.data_source.lwdp.filters.event_filters import LwDPEventFilter
-
-logger = logging.getLogger(__name__)
-
-BasicRequest = namedtuple(
-    "BasicRequest",
-    [
-        "start_timestamp",
-        "end_timestamp",
-        "result_count_limit",
-        "search_direction",
-        "keep_open",
-        "filters",
-    ],
-)
-
-
-class GRPCAPI(IGRPCSourceAPI):
-    def __init__(self, url: str):
-        """GRPC API.
+# LOG import logging
+from http import HTTPStatus
+from typing import List, Generator, Optional, Union
+
+import requests
+from requests import Response
+from urllib3 import PoolManager, exceptions
+from urllib.parse import quote
+
+from th2_data_services.data_source.lwdp.interfaces.source_api import IHTTPSourceAPI 
+
+
+# LOG logger = logging.getLogger("th2_data_services")
+# LOG logger.setLevel(logging.DEBUG)
 
-        Args:
-            url: GRPC data source url.
-        """
-        self._create_connection(url)
 
-    def _create_connection(self, url: str) -> None:
-        """Creates gRPC channel to gRPC-server.
+class API(IHTTPSourceAPI):
+    def __init__(self, url: str, chunk_length: int = 65536):
+        """HTTP API.
 
         Args:
-            url: Url of gRPC-server.
+            url: HTTP data source url.
+            chunk_length: How much of the content to read in one chunk.
         """
-        channel: Channel = insecure_channel(url)
-        self.__stub: DataProviderStub = DataProviderStub(channel)
+        self._url = self.__normalize_url(url)
+        self._chunk_length = chunk_length
 
-    def get_message_streams(self, book_id: str = None) -> MessageStreamsResponse:
-        """GRPC-API `GetMessageStreams` call returns a list of message stream names."""
-        book_id = BookId(name=book_id)
-        message_streams_request = MessageStreamsRequest(book_id=book_id)
-        return self.__stub.GetMessageStreams(message_streams_request)
+    def __normalize_url(self, url):
+        if url is None:
+            return url
 
-    def search_message_groups(
+        pos = len(url) - 1
+        while url[pos] == "/" and pos >= 0:
+            pos -= 1
+
+        return url[: pos + 1]
+
+    def __encode_url(self, url: str) -> str:
+        return quote(url.encode(), "/:&?=")
+
+    def get_url_get_books(self) -> str:
+        """REST-API `books` call returns a list of books in cradleAPI."""
+        return self.__encode_url(f"{self._url}/books")
+
+    def get_url_get_scopes(
         self,
+        book_id: str,
         start_timestamp: int = None,
         end_timestamp: int = None,
-        book_id: str = None,
-        message_groups: List[str] = None,
-        sort: bool = None,
-        raw_only: bool = None,
-        keep_open: bool = None,
-    ) -> MessageSearchResponse:
-        """GRPC-API `SearchMessageGroups` call returns a list of message groups in specified time range.
+        chunked_size: int = None,
+    ) -> str:
+        """REST-API `book/{bookID}/event/scopes/sse` call creates an sse channel of event scopes in book named bookID."""
+        url = f"{self._url}/book/{book_id}/event/scopes/sse?"
+
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "chunkedSize": chunked_size,
+        }
 
-        Args:
-            start_timestamp: Sets the search starting point. Expected in nanoseconds. One of the 'start_timestamp'
-                or 'resume_from_id' must not absent.
-            end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'.
-                Expected in nanoseconds.
-            book_id: book ID for requested groups
-            message_groups: Set of books to request
-            sort: Enables message sorting in the request
-            raw_only: If true, only raw message will be returned in the response
-            keep_open: If true, keeps pulling for new message until don't have one outside the requested range
+        url += "&".join(f"{k}={v}" for k, v in kwargs.items() if v is not None)
+        return self.__encode_url(url)
 
-        Returns:
-            Iterable object which return messages as parts of streaming response or message stream pointers.
-        """
-        self.__search_basic_checks(start_timestamp=start_timestamp, end_timestamp=end_timestamp)
-        basic_request = self.__build_basic_request_object(
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-        )
-        book_id = BookId(name=book_id)
-        message_groups = [MessageGroupsSearchRequest.Group(name=x) for x in message_groups]
-        sort = BoolValue(sort)
-        message_group_search_request = MessageGroupsSearchRequest(
-            start_timestamp=basic_request.start_timestamp,
-            end_timestamp=basic_request.end_timestamp,
-            book_id=book_id,
-            message_group=message_groups,
-            sort=sort,
-            raw_only=raw_only,
-            keep_open=keep_open,
-        )
-        return self.__stub.SearchMessageGroups(message_group_search_request)
-
-    def get_books(self) -> BooksResponse:
-        """GRPC-API `GetBooks` call returns a list of book names."""
-        return self.__stub.GetBooks(BooksRequest())
+    def get_url_get_message_aliases(
+        self,
+        book_id: str,
+        start_timestamp: int = None,
+        end_timestamp: int = None,
+        chunked_size: int = None,
+    ) -> str:
+        """REST-API `book/{bookID}/message/aliases/sse` call creates an sse channel of message aliases in book named bookID."""
+        url = f"{self._url}/book/{book_id}/message/aliases/sse?"
+
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "chunkedSize": chunked_size,
+        }
+
+        url += "&".join(f"{k}={v}" for k, v in kwargs.items() if v is not None)
+        return self.__encode_url(url)
 
-    def search_events(
+    def get_url_get_message_groups(
         self,
-        start_timestamp: int,
-        end_timestamp: int,
-        parent_event: str = None,
-        search_direction: str = "NEXT",
-        result_count_limit: int = None,
-        filter: List[LwDPEventFilter] = None,
-        book_id: str = None,
-        scope: str = None,
-    ) -> Iterable[EventSearchResponse]:
-        """GRPC-API `searchEvents` call creates an event or an event metadata stream that matches the filter.
+        book_id: str,
+        start_timestamp: int = None,
+        end_timestamp: int = None,
+        chunked_size: int = None,
+    ) -> str:
+        """REST-API `book/{bookID}/message/groups/sse` call creates an sse channel of message groups in book named bookID."""
+        url = f"{self._url}/book/{book_id}/message/groups/sse?"
+
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "chunkedSize": chunked_size,
+        }
+
+        url += "&".join(f"{k}={v}" for k, v in kwargs.items() if v is not None)
+        return self.__encode_url(url)
+
+    def get_url_find_event_by_id(self, event_id: str) -> str:
+        """REST-API `event` call returns a single event with the specified id."""
+        return self.__encode_url(f"{self._url}/event/{event_id}")
+
+    def get_url_find_message_by_id(self, message_id: str, only_raw: bool = False) -> str:
+        """REST-API `message` call returns a single      message with the specified id."""
+        return self.__encode_url(f"{self._url}/message/{message_id}?onlyRaw={only_raw}")
+
+    def get_url_get_pages_info_all(self, book_id: str):
+        """REST-API `search/see/page-infos/{$BOOK_ID}/all` call returns page information with the specified timeframe."""
+        url = f"{self._url}/search/sse/page-infos/{book_id}/all"
+        return self.__encode_url(url)
 
-        Args:
-            start_timestamp: Sets the search starting point. Expected in nanoseconds. One of the 'start_timestamp'
-                or 'resume_from_id' must not absent.
-            end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'.
-                Expected in nanoseconds.
-            parent_event: Match events to the specified parent.
-            search_direction: Sets the lookup direction. Can be 'NEXT' or 'PREVIOUS'.
-            result_count_limit: Sets the maximum amount of events to return.
-            limit_for_parent: How many children events for each parent do we want to request.
-            filters: Which filters to apply in a search.
-            book_id: book ID for events
-            scope: scope for events
+    def get_url_get_pages_info(
+        self, book_id: str, start_timestamp: int, end_timestamp: int, limit=None
+    ):
+        """REST-API `search/see/page-infos` call returns page information with the specified timeframe."""
+        url = f"{self._url}/search/sse/page-infos?"
+        params = {
+            "bookId": book_id,
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+        }
+        if limit:
+            params["resultCountLimit"] = limit
+        url += "&".join(f"{k}={v}" for k, v in params.items())
+        return self.__encode_url(url)
 
-        Returns:
-            Iterable object which return events as parts of streaming response.
+    def get_url_search_sse_events(
+        self,
+        start_timestamp: int,
+        book_id: str,
+        scope: str,
+        end_timestamp: Optional[int] = None,
+        parent_event: Optional[str] = None,
+        search_direction: Optional[str] = "next",
+        result_count_limit: Union[int, float] = None,
+        filters: Optional[str] = None,
+    ) -> str:
+        """REST-API `search/sse/events` call create a sse channel of event metadata that matches the filter.
+
+        https://github.com/th2-net/th2-rpt-data-provider#sse-requests-api
         """
-        self.__search_basic_checks(
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-            result_count_limit=result_count_limit,
-            search_direction=search_direction,
-        )
-
-        basic_request = self.__build_basic_request_object(
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-            search_direction=search_direction,
-            result_count_limit=result_count_limit,
-            filters=filter,
-        )
-        parent_event = EventID(id=parent_event) if parent_event else None
-        book_id = BookId(name=book_id)
-        scope = EventScope(name=scope)
-
-        event_search_request = EventSearchRequest(
-            start_timestamp=basic_request.start_timestamp,
-            end_timestamp=basic_request.end_timestamp,
-            parent_event=parent_event,
-            search_direction=basic_request.search_direction,
-            result_count_limit=basic_request.result_count_limit,
-            filter=basic_request.filters,
-            book_id=book_id,
-            scope=scope,
-        )
-        return self.__stub.SearchEvents(event_search_request)
+        # +TODO - add __split_requests here like in get_url_search_sse_messages
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "parentEvent": parent_event,
+            "searchDirection": search_direction,
+            "resultCountLimit": result_count_limit,
+            "bookId": book_id,
+            "scope": scope,
+        }
+
+        query = ""
+        url = f"{self._url}/search/sse/events?"
+        for k, v in kwargs.items():
+            if v is None:
+                continue
+            else:
+                query += f"&{k}={v}"
+        url = f"{url}{query[1:]}"
+        if filters is not None:
+            url += filters
+        return self.__encode_url(url)
 
-    def search_messages(
+    def get_url_search_sse_messages(
         self,
         start_timestamp: int,
-        end_timestamp: int = None,
-        search_direction: str = "NEXT",
-        result_count_limit: int = None,
+        book_id: str,
+        message_ids: List[str] = None,
         stream: List[str] = None,
+        search_direction: Optional[str] = "next",
+        result_count_limit: Union[int, float] = None,
+        end_timestamp: Optional[int] = None,
+        response_formats: List[str] = None,
         keep_open: bool = False,
-        stream_pointer: List[MessageStreamPointer] = None,
+        max_url_length=2048,
+    ) -> List[str]:
+        """REST-API `search/sse/messages` call create a sse channel of messages that matches the filter.
+
+        https://github.com/th2-net/th2-rpt-data-provider#sse-requests-api
+        """
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "messageId": message_ids,
+            "stream": stream,
+            "searchDirection": search_direction,
+            "resultCountLimit": result_count_limit,
+            "endTimestamp": end_timestamp,
+            "responseFormat": response_formats,
+            "keepOpen": keep_open,
+            "bookId": book_id,
+        }
+        if stream:
+            kwargs["stream"] = None
+            optional = [f"&stream={x}" for x in stream]
+        else:
+            kwargs["messageId"] = None
+            optional = [f"&messageId={x}" for x in message_ids]
+
+        query = ""
+        url = f"{self._url}/search/sse/messages?"
+        for k, v in kwargs.items():
+            if v is None:
+                continue
+            if k in ["stream", "responseFormat", "messageId"]:
+                for item in v:
+                    query += f"&{k}={item}"
+            else:
+                query += f"&{k}={v}"
+        url = f"{url}{query[1:]}"
+        urls = self.__split_requests(url, optional, max_url_length)
+        return [self.__encode_url(url) for url in urls]
+
+    def get_url_search_messages_by_groups(
+        self,
+        start_timestamp: int,
+        end_timestamp: int,
+        book_id: str,
+        groups: List[str],
+        sort: bool = None,
         response_formats: List[str] = None,
-        book_id: str = None,
-    ) -> Iterable[MessageSearchResponse]:
-        """GRPC-API `searchMessages` call creates a message stream that matches the filter.
+        keep_open: bool = None,
+        max_url_length=2048,
+    ) -> List[str]:
+        """REST-API `search/sse/messages/group` call creates a sse channel of messages groups in specified time range.
 
         Args:
             start_timestamp: Sets the search starting point. Expected in nanoseconds. One of the 'start_timestamp'
                 or 'resume_from_id' must not absent.
             end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'.
                 Expected in nanoseconds.
-            search_direction: Sets the lookup direction. Can be 'NEXT' or 'PREVIOUS'.
-            result_count_limit: Sets the maximum amount of messages to return.
-            stream: Sets the stream ids to search in.
+            book_id: book ID for requested groups.
+            groups: List of groups to search messages by
+            sort: Enables message sorting in the request
+            response_formats: Response format
             keep_open: If true, keeps pulling for new message until don't have one outside the requested range
-            stream_pointer: List of stream pointers to restore the search from.
-                start_timestamp will be ignored if this parameter is specified. This parameter is only received
-                from the provider.
-            response_formats: List of possible response formats (e.g. PARSED or BASE_64)
-            book_id: book ID for messages
+            max_url_length: API request url max length.
 
         Returns:
             Iterable object which return messages as parts of streaming response or message stream pointers.
         """
-        self.__search_basic_checks(
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-            search_direction=search_direction,
-            result_count_limit=result_count_limit,
-        )
-
-        basic_request = self.__build_basic_request_object(
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-            result_count_limit=result_count_limit,
-            search_direction=search_direction,
-            keep_open=keep_open,
-        )
-
-        stream = self.__transform_streams(stream)
-        book_id = BookId(book_id)
-        message_search_request = MessageSearchRequest(
-            start_timestamp=basic_request.start_timestamp,
-            end_timestamp=basic_request.end_timestamp,
-            search_direction=basic_request.search_direction,
-            result_count_limit=basic_request.result_count_limit,
-            keep_open=basic_request.keep_open,
-            stream_pointer=stream_pointer,
-            stream=stream,
-            response_formats=response_formats,
-            book_id=book_id,
-        )
-
-        return self.__stub.SearchMessages(message_search_request)
-
-    @staticmethod
-    def __search_basic_checks(
-        start_timestamp: Optional[int],
-        end_timestamp: Optional[int],
-        search_direction: Optional[str],
-        result_count_limit: Optional[int],
-    ):
-        if start_timestamp is None:
-            raise ValueError("One of the 'startTimestamp' or 'resumeFromId(s)' must not be None.")
-
-        if end_timestamp is None and result_count_limit is None:
-            raise ValueError("One of the 'end_timestamp' or 'result_count_limit' must not be None.")
-
-        if (
-            start_timestamp is not None
-            and len(str(start_timestamp)) != 19
-            or end_timestamp is not None
-            and len(str(end_timestamp)) != 19
-        ):
-            raise ValueError(
-                "Arguments 'start_timestamp' and 'end_timestamp' are expected in nanoseconds."
-            )
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "bookId": book_id,
+            "sort": sort,
+            "responseFormat": response_formats,
+            "keepOpen": keep_open,
+        }
+        groups = [f"&group={x}" for x in groups]  # "&group=".join(groups)  #
+        options = []
+        url = f"{self._url}/search/sse/messages/group?"
+
+        for k, v in kwargs.items():
+            if v is None:
+                continue
+            if k in ["responseFormat"]:
+                for item in v:
+                    options.append(self._option(k, item))
+            else:
+                options.append(self._option(k, v))
 
-        if search_direction is not None:
-            search_direction = search_direction.upper()
-            if search_direction not in ("NEXT", "PREVIOUS"):
-                raise ValueError("Argument 'search_direction' must be 'NEXT' or 'PREVIOUS'.")
-        else:
-            raise ValueError("Argument 'search_direction' must be 'NEXT' or 'PREVIOUS'.")
+        options_url = "&".join(options)
+        url = f"{url}{options_url}"
+        urls = self.__split_requests(url, groups, max_url_length)
+        return [self.__encode_url(url) for url in urls]
 
-    def __transform_streams(self, streams: List[str]) -> List[MessageStream]:
-        """Transforms streams to MessagesStream of 'protobuf' entity.
+    def get_download_messages(
+        self,
+        start_timestamp: int,
+        end_timestamp: int,
+        book_id: str,
+        groups: List[str],
+        sort: bool = None,
+        response_formats: List[str] = None,
+        keep_open: bool = None,
+        max_url_length=2048,
+    ) -> List[str]:
+        """REST-API `download/messages` call downloads messages in specified time range in json format.
 
         Args:
-            streams: Streams.
+            start_timestamp: Sets the search starting point. Expected in nanoseconds. One of the 'start_timestamp'
+                or 'resume_from_id' must not absent.
+            end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'.
+                Expected in nanoseconds.
+            book_id: book ID for requested groups.
+            groups: List of groups to search messages by
+            sort: Enables message sorting in the request
+            response_formats: Response format
+            keep_open: If true, keeps pulling for new message until don't have one outside the requested range
+            max_url_length: API request url max length.
 
         Returns:
-            List of MessageStream.
+            URL for downloading messages.
         """
-        new_streams = []
-        for raw_stream in streams:
-            if isinstance(raw_stream, Streams):
-                msg_stream = raw_stream.grpc()
-            else:
-                msg_stream = self.__build_message_stream(raw_stream)
-            if isinstance(msg_stream, list):
-                new_streams.extend(msg_stream)
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "bookId": book_id,
+            "sort": sort,
+            "responseFormat": response_formats,
+            "keepOpen": keep_open,
+        }
+        groups = [f"&group={x}" for x in groups]  # "&group=".join(groups)  #
+        options = []
+        url = f"{self._url}/download/messages?"
+
+        for k, v in kwargs.items():
+            if v is None:
+                continue
+            if k in ["responseFormat"]:
+                for item in v:
+                    options.append(self._option(k, item))
             else:
-                new_streams.append(msg_stream)
-        return new_streams
+                options.append(self._option(k, v))
 
-    @staticmethod
-    def __build_message_stream(raw_stream: str) -> Union[MessageStream, List[MessageStream]]:
-        """Builds MessageStream of 'protobuf' entity.
+        options_url = "&".join(options)
+        url = f"{url}{options_url}"
+        urls = self.__split_requests(url, groups, max_url_length)
+        return [self.__encode_url(url) for url in urls]
 
-        Note that if raw_stream doesn't have direction, the function returns both directions.
+    def execute_sse_request(self, url: str) -> Generator[bytes, None, None]:
+        """Create stream connection.
 
         Args:
-            raw_stream: Stream string as 'alias:direction'
+            url: Url.
 
-        Returns:
-            MessageStream.
+        Yields:
+             str: Response stream data.
         """
-        splitted_stream = raw_stream.split(":")
-        name = splitted_stream[0]
-        if len(splitted_stream) > 1:
-            name, search_direction = ":".join(splitted_stream[0:-1]), splitted_stream[-1].upper()
-            if search_direction in ("FIRST", "SECOND"):
-                return MessageStream(name=name, direction=Direction.Value(search_direction))
-            else:
-                name = ":".join(splitted_stream)
-        return [
-            MessageStream(name=name, direction=Direction.Value("FIRST")),
-            MessageStream(name=name, direction=Direction.Value("SECOND")),
-        ]
+        headers = {"Accept": "text/event-stream"}
+        http = PoolManager()
+        response = http.request(method="GET", url=url, headers=headers, preload_content=False)
+
+        if response.status != HTTPStatus.OK:
+            for s in HTTPStatus:
+                if s == response.status:
+                    raise exceptions.HTTPError(
+                        f"{s.value} {s.phrase} ({s.description}). {response.data}"
+                    )
+            raise exceptions.HTTPError(f"Http returned bad status: {response.status}")
 
-    def __build_basic_request_object(
-        self,
-        start_timestamp: int = None,
-        end_timestamp: int = None,
-        result_count_limit: int = None,
-        keep_open: bool = False,
-        search_direction: str = "NEXT",
-        filters: List[LwDPEventFilter] = None,
-    ) -> BasicRequest:
-        """Builds a BasicRequest wrapper-object.
+        yield from response.stream(self._chunk_length)
+
+        response.release_conn()
+
+    def execute_request(self, url: str, headers: dict = None, stream=False) -> Response:
+        """Sends a GET request to provider.
 
         Args:
-            start_timestamp: Start Timestamp for request.
-            end_timestamp: End Timestamp for request.
-            result_count_limit: Data count limit.
-            keep_open: Option for stream-request.
-            search_direction: Searching direction.
-            filters: Which filters to apply in a request.
+            url: Url for a get request to rpt-data-provider.
+            headers: Dictionary of headers for request.
+            stream: Gets response as a stream if True.
 
         Returns:
-            BasicRequest wrapper-object.
+            requests.Response: Response data.
         """
-        if filters is None:
-            filters = []
+        return requests.get(url, headers=headers, stream=stream)
 
-        start_timestamp = (
-            self.__build_timestamp_object(start_timestamp) if start_timestamp else None
-        )
-        end_timestamp = self.__build_timestamp_object(end_timestamp) if end_timestamp else None
-        search_direction = TimeRelation.Value(search_direction)  # getting a value from enum
-        result_count_limit = Int32Value(value=result_count_limit) if result_count_limit else None
-        keep_open = BoolValue(value=keep_open)
-
-        basic_request = BasicRequest(
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-            search_direction=search_direction,
-            result_count_limit=result_count_limit,
-            keep_open=keep_open,
-            filters=filters,
-        )
-        return basic_request
-
-    @staticmethod
-    def __build_timestamp_object(timestamp: int) -> Timestamp:
-        """Builds a Timestamp of 'protobuf' entity.
+    def __split_requests(self, fixed_url: str, optional: List[str], max_url_len: int):
+        if len(fixed_url) >= max_url_len:
+            raise Exception(
+                f"Fixed url part ({len(fixed_url)}) >= than max url len ({max_url_len})"
+            )
 
-        Args:
-            timestamp: Timestamp in nanoseconds.
+        result_urls = []
+        url = fixed_url
 
-        Returns:
-            Timestamp object.
-        """
-        nanos = timestamp % 10**9
-        seconds = timestamp // 10**9
-        timestamp = Timestamp(seconds=seconds, nanos=nanos)
-        return timestamp
-
-    @staticmethod
-    def __build_message_id_object(message_id: str) -> MessageID:
-        """Builds a MessageID of 'protobuf' entity.
+        for s in optional:
+            if len(url) + len(s) >= max_url_len:
+                result_urls.append(url)
+                url = fixed_url + s
+                continue
+            url += s
+        if url:
+            result_urls.append(url)
 
-        Args:
-            message_id: Message id.
+        return result_urls
+
+    def _option(self, opt_name, value):
+        return f"{opt_name}={value}"
 
-        Returns:
-            MessageID object.
-        """
-        split_id = message_id.split(":")
-        split_id.reverse()  # Parse the message id from the end.
 
-        sequence, direction, alias = split_id[0], split_id[1].upper(), split_id[2:]
-        split_sequence = sequence.split(".")
-        sequence, subsequence = int(split_sequence[0]), split_sequence[1:]
-        subsequence = map(int, subsequence) if subsequence else subsequence
-        alias.reverse()
-        alias = ":".join(alias)
-
-        connection_id = ConnectionID(session_alias=alias)
-        direction = Direction.Value(direction)  # Get a value from enum.
-
-        message_id = MessageID(
-            connection_id=connection_id,
-            direction=direction,
-            sequence=sequence,
-            subsequence=subsequence,
-        )
-        return message_id
-
-    def get_event(self, event_id: str) -> EventResponse:
-        """GRPC-API `GetEvent` call returns a single event with the specified id."""
-        event_id = EventID(id=event_id)
-        return self.__stub.GetEvent(event_id)
-
-    def get_message(self, message_id: str) -> MessageGroupResponse:
-        """GRPC-API `GetMessage` call returns a single message with the specified id."""
-        message_id = self.__build_message_id_object(message_id)
-        return self.__stub.GetMessage(message_id)
+HTTPAPI = API
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/struct.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,57 +46,29 @@
     TIMESTAMP: str
     BODY: str
     BODY_BASE64: str
     MESSAGE_ID: str
     ATTACHED_EVENT_IDS: str
 
 
-http_event_struct = EventStruct(
+http_event_struct = event_struct = EventStruct(
     EVENT_ID="eventId",
     PARENT_EVENT_ID="parentEventId",
     STATUS="successful",
     NAME="eventName",
     BATCH_ID="batchId",
     IS_BATCHED="isBatched",
     EVENT_TYPE="eventType",
     END_TIMESTAMP="endTimestamp",
     START_TIMESTAMP="startTimestamp",
     ATTACHED_MESSAGES_IDS="attachedMessageIds",
     BODY="body",
 )
 
-grpc_event_struct = EventStruct(
-    EVENT_ID="eventId",
-    PARENT_EVENT_ID="parentEventId",
-    STATUS="successful",
-    NAME="eventName",
-    BATCH_ID="batchId",
-    IS_BATCHED="isBatched",
-    EVENT_TYPE="eventType",
-    END_TIMESTAMP="endTimestamp",
-    START_TIMESTAMP="startTimestamp",
-    ATTACHED_MESSAGES_IDS="attachedMessageIds",
-    BODY="body",
-)
-
-# +TODO - unknown fields. Perhaps we have them in GRPC
-http_message_struct = MessageStruct(
-    DIRECTION="direction",
-    SESSION_ID="sessionId",
-    MESSAGE_TYPE="messageType",
-    SUBSEQUENCE="subsequence",
-    PROTOCOL="protocol",
-    TIMESTAMP="timestamp",
-    BODY="body",
-    BODY_BASE64="bodyBase64",
-    MESSAGE_ID="messageId",
-    ATTACHED_EVENT_IDS="attachedEventIds",
-)
-
-grpc_message_struct = MessageStruct(
+http_message_struct = message_struct = MessageStruct(
     DIRECTION="direction",
     SESSION_ID="sessionId",
     MESSAGE_TYPE="messageType",
     SUBSEQUENCE="subsequence",
     PROTOCOL="protocol",
     TIMESTAMP="timestamp",
     BODY="body",
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from th2_data_services.interfaces import IEventStub, IMessageStub
 from th2_data_services.data_source.lwdp.struct import (
-    grpc_event_struct,
-    grpc_message_struct,
-    http_event_struct,
-    http_message_struct,
+    event_struct,
+    message_struct,
     EventStruct,
     MessageStruct,
 )
 
 
 class _Singleton(type):
     _instances = {}
@@ -115,18 +113,16 @@
             self.message_fields.BODY: [],
             self.message_fields.BODY_BASE64: [],
             self.message_fields.MESSAGE_ID: self.REQUIRED_FIELD,
             self.message_fields.ATTACHED_EVENT_IDS: [],
         }
 
 
-http_event_stub_builder = EventStubBuilder(http_event_struct)
-http_message_stub_builder = MessageStubBuilder(http_message_struct)
-grpc_event_stub_builder = EventStubBuilder(grpc_event_struct)
-grpc_message_stub_builder = MessageStubBuilder(grpc_message_struct)
+http_event_stub_builder = event_stub_builder = EventStubBuilder(event_struct)
+http_message_stub_builder = message_stub_builder = MessageStubBuilder(message_struct)
 
 
 if __name__ == "__main__":
     # Tests
     # TODO - move to unit-tests (tech debt)
     be1 = BrokenEvent()
     be2 = BrokenEvent()
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/_misc.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.1.0.0.dev5423567204
+Version: 3.0.1.0.dev5423789540
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
@@ -16,16 +16,16 @@
         <!-- start get_started_example.py -->
         ```python
         from typing import List
         
         from th2_data_services.event_tree import EventTreeCollection
         
         from th2_data_services.data_source.lwdp.commands import http as commands
-        from th2_data_services.data_source.lwdp.data_source import HTTPDataSource
-        from th2_data_services.data_source.lwdp.event_tree import HttpETCDriver
+        from th2_data_services.data_source.lwdp.data_source import DataSource
+        from th2_data_services.data_source.lwdp.event_tree import ETCDriver
         from th2_data_services.data_source.lwdp.streams import Streams, Stream
         from th2_data_services.data import Data
         from datetime import datetime
         from th2_data_services.data_source.lwdp.utils import Page
         
         # About this example
         #   The following document shows common features of the library.
@@ -69,15 +69,15 @@
         
         # Date has to be in utc timezone.
         START_TIME = datetime(year=2023, month=1, day=5, hour=13, minute=57, second=5, microsecond=0)
         END_TIME = datetime(year=2023, month=1, day=5, hour=13, minute=57, second=6, microsecond=0)
         
         # [1] Create data source object to connect to lightweight data provider.
         provider_url_link = f"http://10.100.66.105:32681"
-        data_source = HTTPDataSource(provider_url_link)
+        data_source = DataSource(provider_url_link)
         
         # [2] Getting books, pages, scopes, groups and aliases.
         
         # [2.1] Get books.
         #   On database data is segregated with books, such as they never intersect.
         #   To get the names of the books we have a command GetBooks which takes no argument.
         books: List[str] = data_source.command(commands.GetBooks())
@@ -194,15 +194,15 @@
         )
         
         # [4] ETCDriver
         #   To work with EventTreeCollection and its children we need to use special driver.
         #   This driver contains lwdp-related methods that ETC required.
         
         # [4.1] Init driver
-        etc_driver = HttpETCDriver(data_source=data_source, use_stub=False)
+        etc_driver = ETCDriver(data_source=data_source, use_stub=False)
         # [4.2] Init ETC object
         etc = EventTreeCollection(etc_driver)
         
         # [4.3] Build Event Trees inside ETC and recover unknown events if it has them.
         etc.build(events)
         etc.recover_unknown_events()
         # See more info about how to use ETC in th2-data-services lib documentation.
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5423567204/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-3.0.1.0.dev5423789540/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,35 +8,29 @@
 th2_data_services/data_source/lwdp/page.py
 th2_data_services/data_source/lwdp/resolver.py
 th2_data_services/data_source/lwdp/streams.py
 th2_data_services/data_source/lwdp/struct.py
 th2_data_services/data_source/lwdp/stub_builder.py
 th2_data_services/data_source/lwdp/adapters/__init__.py
 th2_data_services/data_source/lwdp/adapters/adapter_sse.py
-th2_data_services/data_source/lwdp/adapters/basic_adapters.py
-th2_data_services/data_source/lwdp/adapters/event_adapters.py
-th2_data_services/data_source/lwdp/adapters/message_adapters.py
 th2_data_services/data_source/lwdp/commands/__init__.py
-th2_data_services/data_source/lwdp/commands/grpc.py
 th2_data_services/data_source/lwdp/commands/http.py
 th2_data_services/data_source/lwdp/data_source/__init__.py
-th2_data_services/data_source/lwdp/data_source/grpc.py
 th2_data_services/data_source/lwdp/data_source/http.py
 th2_data_services/data_source/lwdp/event_tree/__init__.py
 th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
 th2_data_services/data_source/lwdp/filters/__init__.py
 th2_data_services/data_source/lwdp/filters/event_filters.py
 th2_data_services/data_source/lwdp/filters/filter.py
 th2_data_services/data_source/lwdp/interfaces/__init__.py
 th2_data_services/data_source/lwdp/interfaces/command.py
 th2_data_services/data_source/lwdp/interfaces/data_source.py
 th2_data_services/data_source/lwdp/interfaces/filter.py
 th2_data_services/data_source/lwdp/interfaces/source_api.py
 th2_data_services/data_source/lwdp/source_api/__init__.py
-th2_data_services/data_source/lwdp/source_api/grpc.py
 th2_data_services/data_source/lwdp/source_api/http.py
 th2_data_services/data_source/lwdp/utils/__init__.py
 th2_data_services/data_source/lwdp/utils/_misc.py
 th2_data_services/data_source/lwdp/utils/_response_formats.py
 th2_data_services/data_source/lwdp/utils/json.py
 th2_data_services_lwdp.egg-info/PKG-INFO
 th2_data_services_lwdp.egg-info/SOURCES.txt
```

