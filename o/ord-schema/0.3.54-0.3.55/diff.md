# Comparing `tmp/ord-schema-0.3.54.tar.gz` & `tmp/ord-schema-0.3.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.54.tar", last modified: Mon Jun  5 16:43:06 2023, max compression
+gzip compressed data, was "ord-schema-0.3.55.tar", last modified: Fri Jun 30 18:44:21 2023, max compression
```

## Comparing `ord-schema-0.3.54.tar` & `ord-schema-0.3.55.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:06.731537 ord-schema-0.3.54/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-05 16:42:40.000000 ord-schema-0.3.54/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 16:42:40.000000 ord-schema-0.3.54/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 16:42:40.000000 ord-schema-0.3.54/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-05 16:43:06.731537 ord-schema-0.3.54/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-05 16:42:40.000000 ord-schema-0.3.54/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:06.715536 ord-schema-0.3.54/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:06.719537 ord-schema-0.3.54/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    35657 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:06.723537 ord-schema-0.3.54/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/add_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/add_datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:06.723537 ord-schema-0.3.54/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    77919 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:06.727537 ord-schema-0.3.54/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45197 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-05 16:42:40.000000 ord-schema-0.3.54/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:06.715536 ord-schema-0.3.54/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-05 16:43:06.000000 ord-schema-0.3.54/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-05 16:43:06.000000 ord-schema-0.3.54/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:43:06.000000 ord-schema-0.3.54/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-05 16:43:06.000000 ord-schema-0.3.54/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 16:43:06.000000 ord-schema-0.3.54/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:43:06.731537 ord-schema-0.3.54/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-05 16:42:40.000000 ord-schema-0.3.54/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (123)    46054 2023-06-05 16:42:40.000000 ord-schema-0.3.54/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-05 16:42:40.000000 ord-schema-0.3.54/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-05 16:42:40.000000 ord-schema-0.3.54/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:43:06.731537 ord-schema-0.3.54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-05 16:42:45.000000 ord-schema-0.3.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.086528 ord-schema-0.3.55/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-30 18:44:00.000000 ord-schema-0.3.55/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 18:44:00.000000 ord-schema-0.3.55/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 18:44:00.000000 ord-schema-0.3.55/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 18:44:21.086528 ord-schema-0.3.55/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-30 18:44:00.000000 ord-schema-0.3.55/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.078528 ord-schema-0.3.55/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.078528 ord-schema-0.3.55/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35657 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.082528 ord-schema-0.3.55/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/add_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/add_datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.082528 ord-schema-0.3.55/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.082528 ord-schema-0.3.55/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45197 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.078528 ord-schema-0.3.55/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.086528 ord-schema-0.3.55/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-30 18:44:00.000000 ord-schema-0.3.55/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    46054 2023-06-30 18:44:00.000000 ord-schema-0.3.55/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-30 18:44:00.000000 ord-schema-0.3.55/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-30 18:44:00.000000 ord-schema-0.3.55/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:44:21.086528 ord-schema-0.3.55/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-30 18:44:03.000000 ord-schema-0.3.55/setup.py
```

### Comparing `ord-schema-0.3.54/LICENSE` & `ord-schema-0.3.55/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/PKG-INFO` & `ord-schema-0.3.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.54
+Version: 0.3.55
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.54/README.md` & `ord-schema-0.3.55/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/__init__.py` & `ord-schema-0.3.55/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/frozen_message.py` & `ord-schema-0.3.55/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/frozen_message_test.py` & `ord-schema-0.3.55/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/logging.py` & `ord-schema-0.3.55/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/macros/__init__.py` & `ord-schema-0.3.55/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/macros/solutions.py` & `ord-schema-0.3.55/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.55/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/macros/workups.py` & `ord-schema-0.3.55/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/message_helpers.py` & `ord-schema-0.3.55/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/message_helpers_test.py` & `ord-schema-0.3.55/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/orm/__init__.py` & `ord-schema-0.3.55/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/orm/add_datasets.py` & `ord-schema-0.3.55/ord_schema/orm/add_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,30 +38,30 @@
 from docopt import docopt
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session
 
 from ord_schema.logging import get_logger
 from ord_schema.message_helpers import load_message
 from ord_schema.orm.database import add_dataset, add_rdkit, delete_dataset, get_connection_string
-from ord_schema.proto.dataset_pb2 import Dataset
+from ord_schema.proto import dataset_pb2
 
 logger = get_logger(__name__)
 
 
 def _add_dataset(filename: str, url: str, overwrite: bool) -> None:
     """Adds a single dataset to the database.
 
     Args:
         filename: Dataset filename.
         url: Database connection string.
         overwrite: If True, overwrite an existing dataset.
     """
     logger.info(f"Loading {filename}")
     start = time.time()
-    dataset = load_message(filename, Dataset)
+    dataset = load_message(filename, dataset_pb2.Dataset)
     logger.info(f"load_message() took {time.time() - start}s")
     engine = create_engine(url, future=True)
     with Session(engine) as session:
         if overwrite:
             delete_dataset(dataset.dataset_id, session)
         add_dataset(dataset, session)
         start = time.time()
```

### Comparing `ord-schema-0.3.54/ord_schema/orm/add_datasets_test.py` & `ord-schema-0.3.55/ord_schema/orm/add_datasets_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/orm/conftest.py` & `ord-schema-0.3.55/ord_schema/orm/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 import pytest
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session
 from testing.postgresql import Postgresql
 
 from ord_schema.message_helpers import load_message
 from ord_schema.orm.database import add_dataset, add_rdkit, prepare_database
-from ord_schema.proto.dataset_pb2 import Dataset
+from ord_schema.proto import dataset_pb2
 
 
 @pytest.fixture
 def test_session() -> Iterator[Session]:
-    dataset = load_message(os.path.join(os.path.dirname(__file__), "testdata", "ord-nielsen-example.pbtxt"), Dataset)
+    dataset = load_message(
+        os.path.join(os.path.dirname(__file__), "testdata", "ord-nielsen-example.pbtxt"), dataset_pb2.Dataset
+    )
     with Postgresql() as postgres:
         engine = create_engine(postgres.url(), future=True, echo=True)
         rdkit_cartridge = prepare_database(engine)
         with Session(engine) as session:
             add_dataset(dataset, session)
             session.flush()
             if rdkit_cartridge:
```

### Comparing `ord-schema-0.3.54/ord_schema/orm/database.py` & `ord-schema-0.3.55/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/orm/database_test.py` & `ord-schema-0.3.55/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/orm/mappers.py` & `ord-schema-0.3.55/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.55/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.55/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.55/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/proto/__init__.py` & `ord-schema-0.3.55/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.55/ord_schema/proto/dataset_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,48 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ord-schema/proto/dataset.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ord_schema.proto import reaction_pb2 as ord__schema_dot_proto_dot_reaction__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eord-schema/proto/dataset.proto\x12\x03ord\x1a\x1ford-schema/proto/reaction.proto\"x\n\x07\x44\x61taset\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12 \n\treactions\x18\x03 \x03(\x0b\x32\r.ord.Reaction\x12\x14\n\x0creaction_ids\x18\x04 \x03(\t\x12\x12\n\ndataset_id\x18\x05 \x01(\t\"i\n\x0e\x44\x61tasetExample\x12\x12\n\ndataset_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12!\n\x07\x63reated\x18\x04 \x01(\x0b\x32\x10.ord.RecordEventb\x06proto3')
 
-
-
-_DATASET = DESCRIPTOR.message_types_by_name['Dataset']
-_DATASETEXAMPLE = DESCRIPTOR.message_types_by_name['DatasetExample']
-Dataset = _reflection.GeneratedProtocolMessageType('Dataset', (_message.Message,), {
-  'DESCRIPTOR' : _DATASET,
-  '__module__' : 'ord_schema.proto.dataset_pb2'
-  # @@protoc_insertion_point(class_scope:ord.Dataset)
-  })
-_sym_db.RegisterMessage(Dataset)
-
-DatasetExample = _reflection.GeneratedProtocolMessageType('DatasetExample', (_message.Message,), {
-  'DESCRIPTOR' : _DATASETEXAMPLE,
-  '__module__' : 'ord_schema.proto.dataset_pb2'
-  # @@protoc_insertion_point(class_scope:ord.DatasetExample)
-  })
-_sym_db.RegisterMessage(DatasetExample)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ord_schema.proto.dataset_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _DATASET._serialized_start=72
-  _DATASET._serialized_end=192
-  _DATASETEXAMPLE._serialized_start=194
-  _DATASETEXAMPLE._serialized_end=299
+  _globals['_DATASET']._serialized_start=72
+  _globals['_DATASET']._serialized_end=192
+  _globals['_DATASETEXAMPLE']._serialized_start=194
+  _globals['_DATASETEXAMPLE']._serialized_end=299
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ord-schema-0.3.54/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.55/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.55/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/resolvers.py` & `ord-schema-0.3.55/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/resolvers_test.py` & `ord-schema-0.3.55/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/__init__.py` & `ord-schema-0.3.55/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.55/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.55/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.55/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.55/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.55/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.55/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.55/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.55/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.55/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.55/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.55/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/templating.py` & `ord-schema-0.3.55/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/templating_test.py` & `ord-schema-0.3.55/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/units.py` & `ord-schema-0.3.55/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/units_test.py` & `ord-schema-0.3.55/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/updates.py` & `ord-schema-0.3.55/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/updates_test.py` & `ord-schema-0.3.55/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/validations.py` & `ord-schema-0.3.55/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema/validations_test.py` & `ord-schema-0.3.55/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.55/ord_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.54
+Version: 0.3.55
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.54/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.55/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.55/ord_schema.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 flask>=1.1.2
 inflection>=0.5.1
 jinja2>=2.0.0
 joblib>=1.0.0
 numpy>=1.18.1
 openpyxl>=3.0.5
 pandas>=1.0.4
-protobuf<3.20,>=3.13.0
+protobuf==4.22.3
 psycopg2>=2.8.5
 pygithub>=1.51
 python-dateutil>=1.10.0
 rdkit>=2021.9.5
 sqlalchemy>=1.4.39
 
 [docs]
```

### Comparing `ord-schema-0.3.54/proto/dataset.proto` & `ord-schema-0.3.55/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/proto/reaction.proto` & `ord-schema-0.3.55/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/proto/test.proto` & `ord-schema-0.3.55/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.54/setup.py` & `ord-schema-0.3.55/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.54",
+    version="0.3.55",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
@@ -38,15 +38,15 @@
         "flask>=1.1.2",
         "inflection>=0.5.1",
         "jinja2>=2.0.0",
         "joblib>=1.0.0",
         "numpy>=1.18.1",
         "openpyxl>=3.0.5",
         "pandas>=1.0.4",
-        "protobuf<3.20,>=3.13.0",
+        "protobuf==4.22.3",
         "psycopg2>=2.8.5",
         "pygithub>=1.51",
         "python-dateutil>=1.10.0",
         "rdkit>=2021.9.5",
         "sqlalchemy>=1.4.39",
     ],
     extras_require={
```

