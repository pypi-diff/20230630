# Comparing `tmp/Aruna-Python-API-1.1.0rc6.tar.gz` & `tmp/Aruna-Python-API-1.1.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aruna-Python-API-1.1.0rc6.tar", last modified: Tue Jun 27 06:58:53 2023, max compression
+gzip compressed data, was "Aruna-Python-API-1.1.0rc7.tar", last modified: Fri Jun 30 12:19:08 2023, max compression
```

## Comparing `Aruna-Python-API-1.1.0rc6.tar` & `Aruna-Python-API-1.1.0rc7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.157492 Aruna-Python-API-1.1.0rc6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.145492 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-27 06:58:53.157492 Aruna-Python-API-1.1.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.145492 Aruna-Python-API-1.1.0rc6/aruna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.145492 Aruna-Python-API-1.1.0rc6/aruna/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.145492 Aruna-Python-API-1.1.0rc6/aruna/api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/notification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21174 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.157492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25264 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 06:58:53.157492 Aruna-Python-API-1.1.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.603444 Aruna-Python-API-1.1.0rc7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.591443 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-30 12:19:08.603444 Aruna-Python-API-1.1.0rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.591443 Aruna-Python-API-1.1.0rc7/aruna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.591443 Aruna-Python-API-1.1.0rc7/aruna/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.591443 Aruna-Python-API-1.1.0rc7/aruna/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21174 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.599444 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25264 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 12:19:08.603444 Aruna-Python-API-1.1.0rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/setup.py
```

### Comparing `Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/PKG-INFO` & `Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc6
+Version: 1.1.0rc7
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/SOURCES.txt` & `Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/LICENSE` & `Aruna-Python-API-1.1.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/PKG-INFO` & `Aruna-Python-API-1.1.0rc7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc6
+Version: 1.1.0rc7
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc6/README.md` & `Aruna-Python-API-1.1.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 
 from aruna.api.storage.models.v1 import auth_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_auth__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.6*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.7*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.project_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.6*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
+  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.7*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
   _PROJECTSERVICE.methods_by_name['CreateProject']._options = None
   _PROJECTSERVICE.methods_by_name['CreateProject']._serialized_options = b'\202\323\344\223\002\020:\001*\"\013/v1/project'
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._options = None
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._serialized_options = b'\202\323\344\223\002&:\001*\"!/v1/project/{project_id}/add_user'
   _PROJECTSERVICE.methods_by_name['GetProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetProject']._serialized_options = b'\202\323\344\223\002\032\022\030/v1/project/{project_id}'
   _PROJECTSERVICE.methods_by_name['GetProjects']._options = None
```

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,81 +8,78 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from aruna.api.storage.models.v1 import auth_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_auth__pb2
-from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;aruna/api/storage/services/v1/service_account_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1bgoogle/api/visibility.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x99\x01\n\x1b\x43reateServiceAccountRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\"\xb2\x01\n\x0eServiceAccount\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12G\n\npermission\x18\x04 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\"v\n\x1c\x43reateServiceAccountResponse\x12V\n\x0fservice_account\x18\x01 \x01(\x0b\x32-.aruna.api.storage.services.v1.ServiceAccountR\x0eserviceAccount\"\x85\x02\n CreateServiceAccountTokenRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x39\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12G\n\npermission\x18\x05 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\"\x80\x01\n!CreateServiceAccountTokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\x12!\n\x0ctoken_secret\x18\x02 \x01(\tR\x0btokenSecret\"\x9b\x01\n#EditServiceAccountPermissionRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12N\n\x0enew_permission\x18\x02 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\rnewPermission\"~\n$EditServiceAccountPermissionResponse\x12V\n\x0fservice_account\x18\x01 \x01(\x0b\x32-.aruna.api.storage.services.v1.ServiceAccountR\x0eserviceAccount\"`\n\x1dGetServiceAccountTokenRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12\x19\n\x08token_id\x18\x02 \x01(\tR\x07tokenId\"Z\n\x1eGetServiceAccountTokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\"F\n\x1eGetServiceAccountTokensRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\"[\n\x1fGetServiceAccountTokensResponse\x12\x38\n\x05token\x18\x01 \x03(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\"C\n\"GetServiceAccountsByProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"w\n#GetServiceAccountsByProjectResponse\x12P\n\x0csvc_accounts\x18\x01 \x03(\x0b\x32-.aruna.api.storage.services.v1.ServiceAccountR\x0bsvcAccounts\"c\n DeleteServiceAccountTokenRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12\x19\n\x08token_id\x18\x02 \x01(\tR\x07tokenId\"#\n!DeleteServiceAccountTokenResponse\"I\n!DeleteServiceAccountTokensRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\"$\n\"DeleteServiceAccountTokensResponse\"C\n\x1b\x44\x65leteServiceAccountRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\"\x1e\n\x1c\x44\x65leteServiceAccountResponse2\x95\x0f\n\x15ServiceAccountService\x12\xaf\x01\n\x14\x43reateServiceAccount\x12:.aruna.api.storage.services.v1.CreateServiceAccountRequest\x1a;.aruna.api.storage.services.v1.CreateServiceAccountResponse\"\x1e\x82\xd3\xe4\x93\x02\x18:\x01*\"\x13/v1/service_account\x12\xd5\x01\n\x19\x43reateServiceAccountToken\x12?.aruna.api.storage.services.v1.CreateServiceAccountTokenRequest\x1a@.aruna.api.storage.services.v1.CreateServiceAccountTokenResponse\"5\x82\xd3\xe4\x93\x02/:\x01*\"*/v1/service_account/{svc_account_id}/token\x12\xe4\x01\n\x1c\x45\x64itServiceAccountPermission\x12\x42.aruna.api.storage.services.v1.EditServiceAccountPermissionRequest\x1a\x43.aruna.api.storage.services.v1.EditServiceAccountPermissionResponse\";\x82\xd3\xe4\x93\x02\x35:\x01*\x1a\x30/v1/service_account/{svc_account_id}/permissions\x12\xd4\x01\n\x16GetServiceAccountToken\x12<.aruna.api.storage.services.v1.GetServiceAccountTokenRequest\x1a=.aruna.api.storage.services.v1.GetServiceAccountTokenResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v1/service_account/{svc_account_id}/token/{token_id}\x12\xcd\x01\n\x17GetServiceAccountTokens\x12=.aruna.api.storage.services.v1.GetServiceAccountTokensRequest\x1a>.aruna.api.storage.services.v1.GetServiceAccountTokensResponse\"3\x82\xd3\xe4\x93\x02-\x12+/v1/service_account/{svc_account_id}/tokens\x12\xd6\x01\n\x1bGetServiceAccountsByProject\x12\x41.aruna.api.storage.services.v1.GetServiceAccountsByProjectRequest\x1a\x42.aruna.api.storage.services.v1.GetServiceAccountsByProjectResponse\"0\x82\xd3\xe4\x93\x02*\x12(/v1/service_account/project/{project_id}\x12\xdd\x01\n\x19\x44\x65leteServiceAccountToken\x12?.aruna.api.storage.services.v1.DeleteServiceAccountTokenRequest\x1a@.aruna.api.storage.services.v1.DeleteServiceAccountTokenResponse\"=\x82\xd3\xe4\x93\x02\x37*5/v1/service_account/{svc_account_id}/token/{token_id}\x12\xd6\x01\n\x1a\x44\x65leteServiceAccountTokens\x12@.aruna.api.storage.services.v1.DeleteServiceAccountTokensRequest\x1a\x41.aruna.api.storage.services.v1.DeleteServiceAccountTokensResponse\"3\x82\xd3\xe4\x93\x02-*+/v1/service_account/{svc_account_id}/tokens\x12\xbd\x01\n\x14\x44\x65leteServiceAccount\x12:.aruna.api.storage.services.v1.DeleteServiceAccountRequest\x1a;.aruna.api.storage.services.v1.DeleteServiceAccountResponse\",\x82\xd3\xe4\x93\x02&*$/v1/service_account/{svc_account_id}\x1a\x12\xfa\xd2\xe4\x93\x02\x0c\x12\nUNFINISHEDB\x97\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x15ServiceAccountServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;aruna/api/storage/services/v1/service_account_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x99\x01\n\x1b\x43reateServiceAccountRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\"\xb2\x01\n\x0eServiceAccount\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12G\n\npermission\x18\x04 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\"v\n\x1c\x43reateServiceAccountResponse\x12V\n\x0fservice_account\x18\x01 \x01(\x0b\x32-.aruna.api.storage.services.v1.ServiceAccountR\x0eserviceAccount\"\xa4\x02\n CreateServiceAccountTokenRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12\x39\n\nexpires_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12G\n\npermission\x18\x06 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\"\xc8\x01\n!CreateServiceAccountTokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\x12!\n\x0ctoken_secret\x18\x02 \x01(\tR\x0btokenSecret\x12\"\n\rs3_access_key\x18\x03 \x01(\tR\x0bs3AccessKey\x12\"\n\rs3_secret_key\x18\x04 \x01(\tR\x0bs3SecretKey\"\x9a\x01\n\"SetServiceAccountPermissionRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12N\n\x0enew_permission\x18\x02 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\rnewPermission\"}\n#SetServiceAccountPermissionResponse\x12V\n\x0fservice_account\x18\x01 \x01(\x0b\x32-.aruna.api.storage.services.v1.ServiceAccountR\x0eserviceAccount\"`\n\x1dGetServiceAccountTokenRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12\x19\n\x08token_id\x18\x02 \x01(\tR\x07tokenId\"Z\n\x1eGetServiceAccountTokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\"F\n\x1eGetServiceAccountTokensRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\"[\n\x1fGetServiceAccountTokensResponse\x12\x38\n\x05token\x18\x01 \x03(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\"C\n\"GetServiceAccountsByProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"w\n#GetServiceAccountsByProjectResponse\x12P\n\x0csvc_accounts\x18\x01 \x03(\x0b\x32-.aruna.api.storage.services.v1.ServiceAccountR\x0bsvcAccounts\"c\n DeleteServiceAccountTokenRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\x12\x19\n\x08token_id\x18\x02 \x01(\tR\x07tokenId\"#\n!DeleteServiceAccountTokenResponse\"I\n!DeleteServiceAccountTokensRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\"$\n\"DeleteServiceAccountTokensResponse\"C\n\x1b\x44\x65leteServiceAccountRequest\x12$\n\x0esvc_account_id\x18\x01 \x01(\tR\x0csvcAccountId\"\x1e\n\x1c\x44\x65leteServiceAccountResponse2\xfe\x0e\n\x15ServiceAccountService\x12\xaf\x01\n\x14\x43reateServiceAccount\x12:.aruna.api.storage.services.v1.CreateServiceAccountRequest\x1a;.aruna.api.storage.services.v1.CreateServiceAccountResponse\"\x1e\x82\xd3\xe4\x93\x02\x18:\x01*\"\x13/v1/service_account\x12\xd5\x01\n\x19\x43reateServiceAccountToken\x12?.aruna.api.storage.services.v1.CreateServiceAccountTokenRequest\x1a@.aruna.api.storage.services.v1.CreateServiceAccountTokenResponse\"5\x82\xd3\xe4\x93\x02/:\x01*\"*/v1/service_account/{svc_account_id}/token\x12\xe1\x01\n\x1bSetServiceAccountPermission\x12\x41.aruna.api.storage.services.v1.SetServiceAccountPermissionRequest\x1a\x42.aruna.api.storage.services.v1.SetServiceAccountPermissionResponse\";\x82\xd3\xe4\x93\x02\x35:\x01*\x1a\x30/v1/service_account/{svc_account_id}/permissions\x12\xd4\x01\n\x16GetServiceAccountToken\x12<.aruna.api.storage.services.v1.GetServiceAccountTokenRequest\x1a=.aruna.api.storage.services.v1.GetServiceAccountTokenResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v1/service_account/{svc_account_id}/token/{token_id}\x12\xcd\x01\n\x17GetServiceAccountTokens\x12=.aruna.api.storage.services.v1.GetServiceAccountTokensRequest\x1a>.aruna.api.storage.services.v1.GetServiceAccountTokensResponse\"3\x82\xd3\xe4\x93\x02-\x12+/v1/service_account/{svc_account_id}/tokens\x12\xd6\x01\n\x1bGetServiceAccountsByProject\x12\x41.aruna.api.storage.services.v1.GetServiceAccountsByProjectRequest\x1a\x42.aruna.api.storage.services.v1.GetServiceAccountsByProjectResponse\"0\x82\xd3\xe4\x93\x02*\x12(/v1/service_account/project/{project_id}\x12\xdd\x01\n\x19\x44\x65leteServiceAccountToken\x12?.aruna.api.storage.services.v1.DeleteServiceAccountTokenRequest\x1a@.aruna.api.storage.services.v1.DeleteServiceAccountTokenResponse\"=\x82\xd3\xe4\x93\x02\x37*5/v1/service_account/{svc_account_id}/token/{token_id}\x12\xd6\x01\n\x1a\x44\x65leteServiceAccountTokens\x12@.aruna.api.storage.services.v1.DeleteServiceAccountTokensRequest\x1a\x41.aruna.api.storage.services.v1.DeleteServiceAccountTokensResponse\"3\x82\xd3\xe4\x93\x02-*+/v1/service_account/{svc_account_id}/tokens\x12\xbd\x01\n\x14\x44\x65leteServiceAccount\x12:.aruna.api.storage.services.v1.DeleteServiceAccountRequest\x1a;.aruna.api.storage.services.v1.DeleteServiceAccountResponse\",\x82\xd3\xe4\x93\x02&*$/v1/service_account/{svc_account_id}B\x97\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x15ServiceAccountServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.service_account_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\025ServiceAccountServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1'
-  _SERVICEACCOUNTSERVICE._options = None
-  _SERVICEACCOUNTSERVICE._serialized_options = b'\372\322\344\223\002\014\022\nUNFINISHED'
   _SERVICEACCOUNTSERVICE.methods_by_name['CreateServiceAccount']._options = None
   _SERVICEACCOUNTSERVICE.methods_by_name['CreateServiceAccount']._serialized_options = b'\202\323\344\223\002\030:\001*\"\023/v1/service_account'
   _SERVICEACCOUNTSERVICE.methods_by_name['CreateServiceAccountToken']._options = None
   _SERVICEACCOUNTSERVICE.methods_by_name['CreateServiceAccountToken']._serialized_options = b'\202\323\344\223\002/:\001*\"*/v1/service_account/{svc_account_id}/token'
-  _SERVICEACCOUNTSERVICE.methods_by_name['EditServiceAccountPermission']._options = None
-  _SERVICEACCOUNTSERVICE.methods_by_name['EditServiceAccountPermission']._serialized_options = b'\202\323\344\223\0025:\001*\0320/v1/service_account/{svc_account_id}/permissions'
+  _SERVICEACCOUNTSERVICE.methods_by_name['SetServiceAccountPermission']._options = None
+  _SERVICEACCOUNTSERVICE.methods_by_name['SetServiceAccountPermission']._serialized_options = b'\202\323\344\223\0025:\001*\0320/v1/service_account/{svc_account_id}/permissions'
   _SERVICEACCOUNTSERVICE.methods_by_name['GetServiceAccountToken']._options = None
   _SERVICEACCOUNTSERVICE.methods_by_name['GetServiceAccountToken']._serialized_options = b'\202\323\344\223\0027\0225/v1/service_account/{svc_account_id}/token/{token_id}'
   _SERVICEACCOUNTSERVICE.methods_by_name['GetServiceAccountTokens']._options = None
   _SERVICEACCOUNTSERVICE.methods_by_name['GetServiceAccountTokens']._serialized_options = b'\202\323\344\223\002-\022+/v1/service_account/{svc_account_id}/tokens'
   _SERVICEACCOUNTSERVICE.methods_by_name['GetServiceAccountsByProject']._options = None
   _SERVICEACCOUNTSERVICE.methods_by_name['GetServiceAccountsByProject']._serialized_options = b'\202\323\344\223\002*\022(/v1/service_account/project/{project_id}'
   _SERVICEACCOUNTSERVICE.methods_by_name['DeleteServiceAccountToken']._options = None
   _SERVICEACCOUNTSERVICE.methods_by_name['DeleteServiceAccountToken']._serialized_options = b'\202\323\344\223\0027*5/v1/service_account/{svc_account_id}/token/{token_id}'
   _SERVICEACCOUNTSERVICE.methods_by_name['DeleteServiceAccountTokens']._options = None
   _SERVICEACCOUNTSERVICE.methods_by_name['DeleteServiceAccountTokens']._serialized_options = b'\202\323\344\223\002-*+/v1/service_account/{svc_account_id}/tokens'
   _SERVICEACCOUNTSERVICE.methods_by_name['DeleteServiceAccount']._options = None
   _SERVICEACCOUNTSERVICE.methods_by_name['DeleteServiceAccount']._serialized_options = b'\202\323\344\223\002&*$/v1/service_account/{svc_account_id}'
-  _CREATESERVICEACCOUNTREQUEST._serialized_start=227
-  _CREATESERVICEACCOUNTREQUEST._serialized_end=380
-  _SERVICEACCOUNT._serialized_start=383
-  _SERVICEACCOUNT._serialized_end=561
-  _CREATESERVICEACCOUNTRESPONSE._serialized_start=563
-  _CREATESERVICEACCOUNTRESPONSE._serialized_end=681
-  _CREATESERVICEACCOUNTTOKENREQUEST._serialized_start=684
-  _CREATESERVICEACCOUNTTOKENREQUEST._serialized_end=945
-  _CREATESERVICEACCOUNTTOKENRESPONSE._serialized_start=948
-  _CREATESERVICEACCOUNTTOKENRESPONSE._serialized_end=1076
-  _EDITSERVICEACCOUNTPERMISSIONREQUEST._serialized_start=1079
-  _EDITSERVICEACCOUNTPERMISSIONREQUEST._serialized_end=1234
-  _EDITSERVICEACCOUNTPERMISSIONRESPONSE._serialized_start=1236
-  _EDITSERVICEACCOUNTPERMISSIONRESPONSE._serialized_end=1362
-  _GETSERVICEACCOUNTTOKENREQUEST._serialized_start=1364
-  _GETSERVICEACCOUNTTOKENREQUEST._serialized_end=1460
-  _GETSERVICEACCOUNTTOKENRESPONSE._serialized_start=1462
-  _GETSERVICEACCOUNTTOKENRESPONSE._serialized_end=1552
-  _GETSERVICEACCOUNTTOKENSREQUEST._serialized_start=1554
-  _GETSERVICEACCOUNTTOKENSREQUEST._serialized_end=1624
-  _GETSERVICEACCOUNTTOKENSRESPONSE._serialized_start=1626
-  _GETSERVICEACCOUNTTOKENSRESPONSE._serialized_end=1717
-  _GETSERVICEACCOUNTSBYPROJECTREQUEST._serialized_start=1719
-  _GETSERVICEACCOUNTSBYPROJECTREQUEST._serialized_end=1786
-  _GETSERVICEACCOUNTSBYPROJECTRESPONSE._serialized_start=1788
-  _GETSERVICEACCOUNTSBYPROJECTRESPONSE._serialized_end=1907
-  _DELETESERVICEACCOUNTTOKENREQUEST._serialized_start=1909
-  _DELETESERVICEACCOUNTTOKENREQUEST._serialized_end=2008
-  _DELETESERVICEACCOUNTTOKENRESPONSE._serialized_start=2010
-  _DELETESERVICEACCOUNTTOKENRESPONSE._serialized_end=2045
-  _DELETESERVICEACCOUNTTOKENSREQUEST._serialized_start=2047
-  _DELETESERVICEACCOUNTTOKENSREQUEST._serialized_end=2120
-  _DELETESERVICEACCOUNTTOKENSRESPONSE._serialized_start=2122
-  _DELETESERVICEACCOUNTTOKENSRESPONSE._serialized_end=2158
-  _DELETESERVICEACCOUNTREQUEST._serialized_start=2160
-  _DELETESERVICEACCOUNTREQUEST._serialized_end=2227
-  _DELETESERVICEACCOUNTRESPONSE._serialized_start=2229
-  _DELETESERVICEACCOUNTRESPONSE._serialized_end=2259
-  _SERVICEACCOUNTSERVICE._serialized_start=2262
-  _SERVICEACCOUNTSERVICE._serialized_end=4203
+  _CREATESERVICEACCOUNTREQUEST._serialized_start=198
+  _CREATESERVICEACCOUNTREQUEST._serialized_end=351
+  _SERVICEACCOUNT._serialized_start=354
+  _SERVICEACCOUNT._serialized_end=532
+  _CREATESERVICEACCOUNTRESPONSE._serialized_start=534
+  _CREATESERVICEACCOUNTRESPONSE._serialized_end=652
+  _CREATESERVICEACCOUNTTOKENREQUEST._serialized_start=655
+  _CREATESERVICEACCOUNTTOKENREQUEST._serialized_end=947
+  _CREATESERVICEACCOUNTTOKENRESPONSE._serialized_start=950
+  _CREATESERVICEACCOUNTTOKENRESPONSE._serialized_end=1150
+  _SETSERVICEACCOUNTPERMISSIONREQUEST._serialized_start=1153
+  _SETSERVICEACCOUNTPERMISSIONREQUEST._serialized_end=1307
+  _SETSERVICEACCOUNTPERMISSIONRESPONSE._serialized_start=1309
+  _SETSERVICEACCOUNTPERMISSIONRESPONSE._serialized_end=1434
+  _GETSERVICEACCOUNTTOKENREQUEST._serialized_start=1436
+  _GETSERVICEACCOUNTTOKENREQUEST._serialized_end=1532
+  _GETSERVICEACCOUNTTOKENRESPONSE._serialized_start=1534
+  _GETSERVICEACCOUNTTOKENRESPONSE._serialized_end=1624
+  _GETSERVICEACCOUNTTOKENSREQUEST._serialized_start=1626
+  _GETSERVICEACCOUNTTOKENSREQUEST._serialized_end=1696
+  _GETSERVICEACCOUNTTOKENSRESPONSE._serialized_start=1698
+  _GETSERVICEACCOUNTTOKENSRESPONSE._serialized_end=1789
+  _GETSERVICEACCOUNTSBYPROJECTREQUEST._serialized_start=1791
+  _GETSERVICEACCOUNTSBYPROJECTREQUEST._serialized_end=1858
+  _GETSERVICEACCOUNTSBYPROJECTRESPONSE._serialized_start=1860
+  _GETSERVICEACCOUNTSBYPROJECTRESPONSE._serialized_end=1979
+  _DELETESERVICEACCOUNTTOKENREQUEST._serialized_start=1981
+  _DELETESERVICEACCOUNTTOKENREQUEST._serialized_end=2080
+  _DELETESERVICEACCOUNTTOKENRESPONSE._serialized_start=2082
+  _DELETESERVICEACCOUNTTOKENRESPONSE._serialized_end=2117
+  _DELETESERVICEACCOUNTTOKENSREQUEST._serialized_start=2119
+  _DELETESERVICEACCOUNTTOKENSREQUEST._serialized_end=2192
+  _DELETESERVICEACCOUNTTOKENSRESPONSE._serialized_start=2194
+  _DELETESERVICEACCOUNTTOKENSRESPONSE._serialized_end=2230
+  _DELETESERVICEACCOUNTREQUEST._serialized_start=2232
+  _DELETESERVICEACCOUNTREQUEST._serialized_end=2299
+  _DELETESERVICEACCOUNTRESPONSE._serialized_start=2301
+  _DELETESERVICEACCOUNTRESPONSE._serialized_end=2331
+  _SERVICEACCOUNTSERVICE._serialized_start=2334
+  _SERVICEACCOUNTSERVICE._serialized_end=4252
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from aruna.api.storage.models.v1 import auth_pb2 as _auth_pb2
-from google.api import visibility_pb2 as _visibility_pb2
 from google.api import annotations_pb2 as _annotations_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
@@ -22,34 +21,40 @@
 class CreateServiceAccountResponse(_message.Message):
     __slots__ = ["service_account"]
     SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
     service_account: ServiceAccount
     def __init__(self, service_account: _Optional[_Union[ServiceAccount, _Mapping]] = ...) -> None: ...
 
 class CreateServiceAccountTokenRequest(_message.Message):
-    __slots__ = ["collection_id", "expires_at", "name", "permission", "svc_account_id"]
+    __slots__ = ["collection_id", "expires_at", "name", "permission", "project_id", "svc_account_id"]
     COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PERMISSION_FIELD_NUMBER: _ClassVar[int]
+    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     SVC_ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
     collection_id: str
     expires_at: _timestamp_pb2.Timestamp
     name: str
     permission: _auth_pb2.Permission
+    project_id: str
     svc_account_id: str
-    def __init__(self, svc_account_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., name: _Optional[str] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., permission: _Optional[_Union[_auth_pb2.Permission, str]] = ...) -> None: ...
+    def __init__(self, svc_account_id: _Optional[str] = ..., project_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., name: _Optional[str] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., permission: _Optional[_Union[_auth_pb2.Permission, str]] = ...) -> None: ...
 
 class CreateServiceAccountTokenResponse(_message.Message):
-    __slots__ = ["token", "token_secret"]
+    __slots__ = ["s3_access_key", "s3_secret_key", "token", "token_secret"]
+    S3_ACCESS_KEY_FIELD_NUMBER: _ClassVar[int]
+    S3_SECRET_KEY_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     TOKEN_SECRET_FIELD_NUMBER: _ClassVar[int]
+    s3_access_key: str
+    s3_secret_key: str
     token: _auth_pb2.Token
     token_secret: str
-    def __init__(self, token: _Optional[_Union[_auth_pb2.Token, _Mapping]] = ..., token_secret: _Optional[str] = ...) -> None: ...
+    def __init__(self, token: _Optional[_Union[_auth_pb2.Token, _Mapping]] = ..., token_secret: _Optional[str] = ..., s3_access_key: _Optional[str] = ..., s3_secret_key: _Optional[str] = ...) -> None: ...
 
 class DeleteServiceAccountRequest(_message.Message):
     __slots__ = ["svc_account_id"]
     SVC_ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
     svc_account_id: str
     def __init__(self, svc_account_id: _Optional[str] = ...) -> None: ...
 
@@ -75,28 +80,14 @@
     svc_account_id: str
     def __init__(self, svc_account_id: _Optional[str] = ...) -> None: ...
 
 class DeleteServiceAccountTokensResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class EditServiceAccountPermissionRequest(_message.Message):
-    __slots__ = ["new_permission", "svc_account_id"]
-    NEW_PERMISSION_FIELD_NUMBER: _ClassVar[int]
-    SVC_ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
-    new_permission: _auth_pb2.Permission
-    svc_account_id: str
-    def __init__(self, svc_account_id: _Optional[str] = ..., new_permission: _Optional[_Union[_auth_pb2.Permission, str]] = ...) -> None: ...
-
-class EditServiceAccountPermissionResponse(_message.Message):
-    __slots__ = ["service_account"]
-    SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
-    service_account: ServiceAccount
-    def __init__(self, service_account: _Optional[_Union[ServiceAccount, _Mapping]] = ...) -> None: ...
-
 class GetServiceAccountTokenRequest(_message.Message):
     __slots__ = ["svc_account_id", "token_id"]
     SVC_ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
     TOKEN_ID_FIELD_NUMBER: _ClassVar[int]
     svc_account_id: str
     token_id: str
     def __init__(self, svc_account_id: _Optional[str] = ..., token_id: _Optional[str] = ...) -> None: ...
@@ -138,7 +129,21 @@
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     SVC_ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
     name: str
     permission: _auth_pb2.Permission
     project_id: str
     svc_account_id: str
     def __init__(self, svc_account_id: _Optional[str] = ..., project_id: _Optional[str] = ..., name: _Optional[str] = ..., permission: _Optional[_Union[_auth_pb2.Permission, str]] = ...) -> None: ...
+
+class SetServiceAccountPermissionRequest(_message.Message):
+    __slots__ = ["new_permission", "svc_account_id"]
+    NEW_PERMISSION_FIELD_NUMBER: _ClassVar[int]
+    SVC_ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
+    new_permission: _auth_pb2.Permission
+    svc_account_id: str
+    def __init__(self, svc_account_id: _Optional[str] = ..., new_permission: _Optional[_Union[_auth_pb2.Permission, str]] = ...) -> None: ...
+
+class SetServiceAccountPermissionResponse(_message.Message):
+    __slots__ = ["service_account"]
+    SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
+    service_account: ServiceAccount
+    def __init__(self, service_account: _Optional[_Union[ServiceAccount, _Mapping]] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.CreateServiceAccountResponse.FromString,
                 )
         self.CreateServiceAccountToken = channel.unary_unary(
                 '/aruna.api.storage.services.v1.ServiceAccountService/CreateServiceAccountToken',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.CreateServiceAccountTokenRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.CreateServiceAccountTokenResponse.FromString,
                 )
-        self.EditServiceAccountPermission = channel.unary_unary(
-                '/aruna.api.storage.services.v1.ServiceAccountService/EditServiceAccountPermission',
-                request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.EditServiceAccountPermissionRequest.SerializeToString,
-                response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.EditServiceAccountPermissionResponse.FromString,
+        self.SetServiceAccountPermission = channel.unary_unary(
+                '/aruna.api.storage.services.v1.ServiceAccountService/SetServiceAccountPermission',
+                request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.SetServiceAccountPermissionRequest.SerializeToString,
+                response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.SetServiceAccountPermissionResponse.FromString,
                 )
         self.GetServiceAccountToken = channel.unary_unary(
                 '/aruna.api.storage.services.v1.ServiceAccountService/GetServiceAccountToken',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.GetServiceAccountTokenRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.GetServiceAccountTokenResponse.FromString,
                 )
         self.GetServiceAccountTokens = channel.unary_unary(
@@ -92,16 +92,16 @@
         Each service account can only have one permission -> The token will have the same permission as the
         service account
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def EditServiceAccountPermission(self, request, context):
-        """EditServiceAccountPermission
+    def SetServiceAccountPermission(self, request, context):
+        """SetServiceAccountPermission
 
         Overwrites the project specific permissions for a service account
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -171,18 +171,18 @@
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.CreateServiceAccountResponse.SerializeToString,
             ),
             'CreateServiceAccountToken': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateServiceAccountToken,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.CreateServiceAccountTokenRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.CreateServiceAccountTokenResponse.SerializeToString,
             ),
-            'EditServiceAccountPermission': grpc.unary_unary_rpc_method_handler(
-                    servicer.EditServiceAccountPermission,
-                    request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.EditServiceAccountPermissionRequest.FromString,
-                    response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.EditServiceAccountPermissionResponse.SerializeToString,
+            'SetServiceAccountPermission': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetServiceAccountPermission,
+                    request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.SetServiceAccountPermissionRequest.FromString,
+                    response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.SetServiceAccountPermissionResponse.SerializeToString,
             ),
             'GetServiceAccountToken': grpc.unary_unary_rpc_method_handler(
                     servicer.GetServiceAccountToken,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.GetServiceAccountTokenRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.GetServiceAccountTokenResponse.SerializeToString,
             ),
             'GetServiceAccountTokens': grpc.unary_unary_rpc_method_handler(
@@ -256,27 +256,27 @@
         return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.ServiceAccountService/CreateServiceAccountToken',
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.CreateServiceAccountTokenRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.CreateServiceAccountTokenResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def EditServiceAccountPermission(request,
+    def SetServiceAccountPermission(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.ServiceAccountService/EditServiceAccountPermission',
-            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.EditServiceAccountPermissionRequest.SerializeToString,
-            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.EditServiceAccountPermissionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.ServiceAccountService/SetServiceAccountPermission',
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.SetServiceAccountPermissionRequest.SerializeToString,
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_service__account__service__pb2.SetServiceAccountPermissionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetServiceAccountToken(request,
             target,
             options=(),
```

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc6/setup.py` & `Aruna-Python-API-1.1.0rc7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='Aruna-Python-API',
-    version="1.1.0-rc.6",
+    version="1.1.0-rc.7",
     description='Aruna Object Storage Python API builds',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ArunaStorage/python-api',
     license='Apache 2.0',
     author='Marius Dieckmann, Jannis Hochmuth',
     author_email='marius.dieckmann@computational.bio.uni-giessen.de, '
```

