# Comparing `tmp/ord-schema-0.3.55.tar.gz` & `tmp/ord-schema-0.3.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.55.tar", last modified: Fri Jun 30 18:44:21 2023, max compression
+gzip compressed data, was "ord-schema-0.3.56.tar", last modified: Fri Jun 30 19:04:03 2023, max compression
```

## Comparing `ord-schema-0.3.55.tar` & `ord-schema-0.3.56.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.086528 ord-schema-0.3.55/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-30 18:44:00.000000 ord-schema-0.3.55/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 18:44:00.000000 ord-schema-0.3.55/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 18:44:00.000000 ord-schema-0.3.55/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 18:44:21.086528 ord-schema-0.3.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-30 18:44:00.000000 ord-schema-0.3.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.078528 ord-schema-0.3.55/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.078528 ord-schema-0.3.55/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    35657 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.082528 ord-schema-0.3.55/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/add_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/add_datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.082528 ord-schema-0.3.55/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.082528 ord-schema-0.3.55/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45197 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-30 18:44:00.000000 ord-schema-0.3.55/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.078528 ord-schema-0.3.55/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 18:44:21.000000 ord-schema-0.3.55/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:44:21.086528 ord-schema-0.3.55/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-30 18:44:00.000000 ord-schema-0.3.55/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (123)    46054 2023-06-30 18:44:00.000000 ord-schema-0.3.55/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-30 18:44:00.000000 ord-schema-0.3.55/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-30 18:44:00.000000 ord-schema-0.3.55/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:44:21.086528 ord-schema-0.3.55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-30 18:44:03.000000 ord-schema-0.3.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.182771 ord-schema-0.3.56/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-30 19:03:38.000000 ord-schema-0.3.56/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 19:03:38.000000 ord-schema-0.3.56/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 19:03:38.000000 ord-schema-0.3.56/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 19:04:03.182771 ord-schema-0.3.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-30 19:03:38.000000 ord-schema-0.3.56/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/add_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/add_datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.182771 ord-schema-0.3.56/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45197 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.182771 ord-schema-0.3.56/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-30 19:03:38.000000 ord-schema-0.3.56/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    46054 2023-06-30 19:03:38.000000 ord-schema-0.3.56/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-30 19:03:38.000000 ord-schema-0.3.56/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-30 19:03:38.000000 ord-schema-0.3.56/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:04:03.182771 ord-schema-0.3.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-30 19:03:42.000000 ord-schema-0.3.56/setup.py
```

### Comparing `ord-schema-0.3.55/LICENSE` & `ord-schema-0.3.56/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/PKG-INFO` & `ord-schema-0.3.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.55
+Version: 0.3.56
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.55/README.md` & `ord-schema-0.3.56/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/__init__.py` & `ord-schema-0.3.56/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/frozen_message.py` & `ord-schema-0.3.56/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/frozen_message_test.py` & `ord-schema-0.3.56/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/logging.py` & `ord-schema-0.3.56/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/macros/__init__.py` & `ord-schema-0.3.56/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/macros/solutions.py` & `ord-schema-0.3.56/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.56/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/macros/workups.py` & `ord-schema-0.3.56/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/message_helpers.py` & `ord-schema-0.3.56/ord_schema/message_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """Helper functions for constructing Protocol Buffer messages."""
 
 import enum
 import functools
 import gzip
 import os
 import re
+import urllib.parse
 import warnings
 from collections.abc import Iterable, Mapping, Sequence
 from typing import Optional, Type, TypeVar, Union
 
 import pandas as pd
 import requests
 from google import protobuf  # pytype: disable=import-error
@@ -38,14 +39,15 @@
 
 _COMPOUND_IDENTIFIER_LOADERS = {
     reaction_pb2.CompoundIdentifier.SMILES: Chem.MolFromSmiles,
     reaction_pb2.CompoundIdentifier.INCHI: Chem.MolFromInchi,
     reaction_pb2.CompoundIdentifier.MOLBLOCK: Chem.MolFromMolBlock,
 }
 MessageType = TypeVar("MessageType")  # Generic for setting return types; pylint: disable=invalid-name.
+ORD_DATA_URL = "https://github.com/Open-Reaction-Database/ord-data/raw/main/"
 
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-locals
 
 
 def build_compound(
@@ -715,19 +717,27 @@
 
     Args:
         dataset_id: Dataset ID.
         timeout: Number of seconds to wait before timing out the request.
 
     Returns:
         Dataset message.
+
+    Raises:
+        RuntimeError: If the request fails.
+        ValueError: If the dataset ID is invalid.
     """
-    url = os.path.join(
-        "https://github.com/open-reaction-database/ord-data/raw/main", id_filename(f"{dataset_id}.pb.gz")
-    )
+    from ord_schema import validations  # Avoid circular import; pylint: disable=import-outside-toplevel.
+
+    if not validations.is_valid_dataset_id(dataset_id):
+        raise ValueError(f"Invalid dataset ID: {dataset_id}")
+    url = urllib.parse.urljoin(ORD_DATA_URL, id_filename(f"{dataset_id}.pb.gz"))
     response = requests.get(url, timeout=timeout)
+    if response.status_code != 200:
+        raise RuntimeError(f"Request {url} failed with status {response.status_code}")
     return dataset_pb2.Dataset.FromString(gzip.decompress(response.content))
 
 
 # pylint: disable=inconsistent-return-statements
 def load_message(filename: str, message_type: Type[MessageType]) -> MessageType:
     """Loads a protocol buffer message from a file.
```

### Comparing `ord-schema-0.3.55/ord_schema/message_helpers_test.py` & `ord-schema-0.3.56/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/__init__.py` & `ord-schema-0.3.56/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/add_datasets.py` & `ord-schema-0.3.56/ord_schema/orm/add_datasets.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/add_datasets_test.py` & `ord-schema-0.3.56/ord_schema/orm/add_datasets_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/conftest.py` & `ord-schema-0.3.56/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/database.py` & `ord-schema-0.3.56/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/database_test.py` & `ord-schema-0.3.56/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/mappers.py` & `ord-schema-0.3.56/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.56/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.56/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.56/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/proto/__init__.py` & `ord-schema-0.3.56/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.56/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.56/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.56/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.56/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.56/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/resolvers.py` & `ord-schema-0.3.56/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/resolvers_test.py` & `ord-schema-0.3.56/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/__init__.py` & `ord-schema-0.3.56/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.56/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.56/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.56/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.56/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.56/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.56/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.56/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.56/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.56/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.56/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.56/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/templating.py` & `ord-schema-0.3.56/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/templating_test.py` & `ord-schema-0.3.56/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/units.py` & `ord-schema-0.3.56/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/units_test.py` & `ord-schema-0.3.56/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/updates.py` & `ord-schema-0.3.56/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/updates_test.py` & `ord-schema-0.3.56/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/validations.py` & `ord-schema-0.3.56/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema/validations_test.py` & `ord-schema-0.3.56/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.56/ord_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.55
+Version: 0.3.56
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.55/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.56/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.56/ord_schema.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,14 @@
 tensorflow>=2.4.1
 tqdm>=4.61.2
 wget>=3.2
 
 [tests]
 black[jupyter]>=22.3.0
 coverage>=5.2.1
-pylint>=2.13.9
+pylint~=2.17.4
 pytest>=7.1.1
 pytest-cov>=3.0.0
 pytest-xdist>=3.0.2
-pytype>=2022.5.19
+pytype==2023.6.16
 testing-postgresql>=1.3.0
 treon>=0.1.3
```

### Comparing `ord-schema-0.3.55/proto/dataset.proto` & `ord-schema-0.3.56/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/proto/reaction.proto` & `ord-schema-0.3.56/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/proto/test.proto` & `ord-schema-0.3.56/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.55/setup.py` & `ord-schema-0.3.56/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.55",
+    version="0.3.56",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
@@ -64,17 +64,17 @@
             "tensorflow>=2.4.1",
             "tqdm>=4.61.2",
             "wget>=3.2",
         ],
         "tests": [
             "black[jupyter]>=22.3.0",
             "coverage>=5.2.1",
-            "pylint>=2.13.9",
+            "pylint~=2.17.4",
             "pytest>=7.1.1",
             "pytest-cov>=3.0.0",
             "pytest-xdist>=3.0.2",
-            "pytype>=2022.5.19",
+            "pytype==2023.6.16",
             "testing-postgresql>=1.3.0",
             "treon>=0.1.3",
         ],
     },
 )
```

