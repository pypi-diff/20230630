# Comparing `tmp/armonik-3.9.1.dev577.tar.gz` & `tmp/armonik-3.9.1.dev597.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armonik-3.9.1.dev577.tar", last modified: Wed Jun 28 06:47:43 2023, max compression
+gzip compressed data, was "armonik-3.9.1.dev597.tar", last modified: Fri Jun 30 08:10:17 2023, max compression
```

## Comparing `armonik-3.9.1.dev577.tar` & `armonik-3.9.1.dev597.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.801825 armonik-3.9.1.dev577/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-28 06:47:43.801825 armonik-3.9.1.dev577/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 06:47:43.801825 armonik-3.9.1.dev577/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.789825 armonik-3.9.1.dev577/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.793825 armonik-3.9.1.dev577/src/armonik/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.793825 armonik-3.9.1.dev577/src/armonik/client/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/client/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/client/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.793825 armonik-3.9.1.dev577/src/armonik/common/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/common/enumwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.793825 armonik-3.9.1.dev577/src/armonik/protogen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.797825 armonik-3.9.1.dev577/src/armonik/protogen/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/applications_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/applications_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/applications_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/auth_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/auth_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/auth_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/events_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/events_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/events_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/partitions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/partitions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/partitions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/results_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/results_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/results_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/sessions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/sessions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/sessions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/submitter_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/submitter_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/submitter_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/tasks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/tasks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/tasks_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/versions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/versions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/client/versions_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.801825 armonik-3.9.1.dev577/src/armonik/protogen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/agent_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/agent_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/agent_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/applications_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/applications_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/applications_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/auth_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/auth_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/auth_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/events_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/events_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/events_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/objects_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/objects_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/objects_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/partitions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/partitions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/partitions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/result_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/result_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/result_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/results_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/results_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/results_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/session_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/session_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/session_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/sessions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/sessions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/sessions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/sort_direction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/sort_direction_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/sort_direction_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/submitter_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/submitter_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/submitter_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/task_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/task_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/task_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/tasks_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/tasks_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/tasks_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/versions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/versions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/versions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/worker_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/worker_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/common/worker_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.801825 armonik-3.9.1.dev577/src/armonik/protogen/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/worker/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/worker/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/worker/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/worker/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/worker/worker_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-28 06:47:37.000000 armonik-3.9.1.dev577/src/armonik/protogen/worker/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.801825 armonik-3.9.1.dev577/src/armonik/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/worker/seqlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/worker/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-28 06:47:27.000000 armonik-3.9.1.dev577/src/armonik/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:47:43.793825 armonik-3.9.1.dev577/src/armonik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-28 06:47:43.000000 armonik-3.9.1.dev577/src/armonik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-28 06:47:43.000000 armonik-3.9.1.dev577/src/armonik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 06:47:43.000000 armonik-3.9.1.dev577/src/armonik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-28 06:47:43.000000 armonik-3.9.1.dev577/src/armonik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-28 06:47:43.000000 armonik-3.9.1.dev577/src/armonik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.477346 armonik-3.9.1.dev597/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-30 08:10:17.477346 armonik-3.9.1.dev597/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:10:17.477346 armonik-3.9.1.dev597/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.461344 armonik-3.9.1.dev597/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.461344 armonik-3.9.1.dev597/src/armonik/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.465345 armonik-3.9.1.dev597/src/armonik/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/client/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/client/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.465345 armonik-3.9.1.dev597/src/armonik/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/common/enumwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.461344 armonik-3.9.1.dev597/src/armonik/protogen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.469345 armonik-3.9.1.dev597/src/armonik/protogen/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/applications_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/applications_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/applications_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/auth_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/auth_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/auth_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/events_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/events_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/events_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/partitions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/partitions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/partitions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/results_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/results_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/results_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/sessions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/sessions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/sessions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/submitter_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/submitter_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/submitter_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/tasks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/tasks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/tasks_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/versions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/versions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/client/versions_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.473345 armonik-3.9.1.dev597/src/armonik/protogen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/agent_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/agent_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/agent_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/applications_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/applications_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/applications_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/auth_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/auth_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/auth_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/events_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/events_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/events_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/objects_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/objects_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/objects_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/partitions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/partitions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/partitions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/result_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/result_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/result_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/results_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/results_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/results_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/session_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/session_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/session_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/sessions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/sessions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/sessions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/sort_direction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/sort_direction_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/sort_direction_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/submitter_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/submitter_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/submitter_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/task_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/task_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/task_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/tasks_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/tasks_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/tasks_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/versions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/versions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/versions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/worker_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/worker_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/common/worker_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.477346 armonik-3.9.1.dev597/src/armonik/protogen/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/worker/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/worker/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/worker/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/worker/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/worker/worker_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-30 08:10:08.000000 armonik-3.9.1.dev597/src/armonik/protogen/worker/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.477346 armonik-3.9.1.dev597/src/armonik/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/worker/seqlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/worker/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-30 08:09:52.000000 armonik-3.9.1.dev597/src/armonik/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:10:17.465345 armonik-3.9.1.dev597/src/armonik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-30 08:10:17.000000 armonik-3.9.1.dev597/src/armonik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-30 08:10:17.000000 armonik-3.9.1.dev597/src/armonik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:10:17.000000 armonik-3.9.1.dev597/src/armonik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 08:10:17.000000 armonik-3.9.1.dev597/src/armonik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 08:10:17.000000 armonik-3.9.1.dev597/src/armonik.egg-info/top_level.txt
```

### Comparing `armonik-3.9.1.dev577/PKG-INFO` & `armonik-3.9.1.dev597/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.9.1.dev577
+Version: 3.9.1.dev597
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.9.1.dev577/README.md` & `armonik-3.9.1.dev597/README.md`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/pyproject.toml` & `armonik-3.9.1.dev597/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/client/results.py` & `armonik-3.9.1.dev597/src/armonik/client/results.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/client/submitter.py` & `armonik-3.9.1.dev597/src/armonik/client/submitter.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/client/tasks.py` & `armonik-3.9.1.dev597/src/armonik/client/tasks.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/common/enumwrapper.py` & `armonik-3.9.1.dev597/src/armonik/common/enumwrapper.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/common/helpers.py` & `armonik-3.9.1.dev597/src/armonik/common/helpers.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/common/objects.py` & `armonik-3.9.1.dev597/src/armonik/common/objects.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/applications_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/applications_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/applications_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/applications_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/auth_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/auth_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/events_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/events_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/events_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/partitions_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/partitions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/partitions_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/partitions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/results_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/results_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/results_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/results_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/sessions_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/sessions_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/sessions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/submitter_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/submitter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/submitter_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/submitter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/tasks_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/tasks_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/tasks_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/tasks_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/versions_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/versions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/client/versions_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/client/versions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/agent_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/agent_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/agent_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/agent_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/applications_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/applications_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/applications_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/applications_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/auth_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/auth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/auth_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/auth_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/events_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/events_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/events_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/events_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/objects_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/objects_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/objects_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/objects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/partitions_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/partitions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/partitions_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/partitions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/result_status_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/result_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/result_status_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/result_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/results_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/results_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/results_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/results_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/session_status_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/session_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/session_status_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/session_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/sessions_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/sessions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/sessions_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/sessions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/sort_direction_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/sort_direction_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/sort_direction_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/sort_direction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/submitter_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/submitter_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/submitter_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/submitter_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/task_status_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/task_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/task_status_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/task_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/tasks_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/tasks_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/tasks_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/tasks_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/versions_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/versions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/versions_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/versions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/worker_common_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/common/worker_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/common/worker_common_pb2.pyi` & `armonik-3.9.1.dev597/src/armonik/protogen/common/worker_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/worker/agent_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/worker/agent_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/worker/agent_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/worker/agent_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/worker/worker_service_pb2.py` & `armonik-3.9.1.dev597/src/armonik/protogen/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/protogen/worker/worker_service_pb2_grpc.py` & `armonik-3.9.1.dev597/src/armonik/protogen/worker/worker_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/worker/seqlogger.py` & `armonik-3.9.1.dev597/src/armonik/worker/seqlogger.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/worker/taskhandler.py` & `armonik-3.9.1.dev597/src/armonik/worker/taskhandler.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik/worker/worker.py` & `armonik-3.9.1.dev597/src/armonik/worker/worker.py`

 * *Files identical despite different names*

### Comparing `armonik-3.9.1.dev577/src/armonik.egg-info/PKG-INFO` & `armonik-3.9.1.dev597/src/armonik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.9.1.dev577
+Version: 3.9.1.dev597
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.9.1.dev577/src/armonik.egg-info/SOURCES.txt` & `armonik-3.9.1.dev597/src/armonik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

