# Comparing `tmp/cypherdataframe-0.3.1.tar.gz` & `tmp/cypherdataframe-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypherdataframe-0.3.1.tar", last modified: Fri Jun 30 15:53:56 2023, max compression
+gzip compressed data, was "cypherdataframe-0.3.2.tar", last modified: Fri Jun 30 16:09:02 2023, max compression
```

## Comparing `cypherdataframe-0.3.1.tar` & `cypherdataframe-0.3.2.tar`

### file list

```diff
@@ -1,49 +1,67 @@
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.932713 cypherdataframe-0.3.1/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-06-30 15:53:56.932409 cypherdataframe-0.3.1/PKG-INFO
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.916341 cypherdataframe-0.3.1/cypherdataframe/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.3.1/cypherdataframe/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.3.1/cypherdataframe/branch_maker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.3.1/cypherdataframe/config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     9142 2023-06-29 21:29:55.000000 cypherdataframe-0.3.1/cypherdataframe/cypher.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.919020 cypherdataframe-0.3.1/cypherdataframe/garner_domain/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1340 2023-06-29 20:43:49.000000 cypherdataframe-0.3.1/cypherdataframe/garner_domain/BranchMaker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.3.1/cypherdataframe/garner_domain/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.3.1/cypherdataframe/garner_domain/properties_defaults.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.921851 cypherdataframe-0.3.1/cypherdataframe/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2213 2023-06-15 17:59:52.000000 cypherdataframe-0.3.1/cypherdataframe/model/Branch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.3.1/cypherdataframe/model/Config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      829 2023-05-05 22:58:23.000000 cypherdataframe-0.3.1/cypherdataframe/model/LabelNode.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.3.1/cypherdataframe/model/Property.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.3.1/cypherdataframe/model/Query.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.3.1/cypherdataframe/model/QueryAccumulation.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.3.1/cypherdataframe/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.3.1/cypherdataframe/testfunctions.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.918092 cypherdataframe-0.3.1/cypherdataframe.egg-info/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-06-30 15:53:56.000000 cypherdataframe-0.3.1/cypherdataframe.egg-info/PKG-INFO
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1221 2023-06-30 15:53:56.000000 cypherdataframe-0.3.1/cypherdataframe.egg-info/SOURCES.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-06-30 15:53:56.000000 cypherdataframe-0.3.1/cypherdataframe.egg-info/dependency_links.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-06-30 15:53:56.000000 cypherdataframe-0.3.1/cypherdataframe.egg-info/requires.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-06-30 15:53:56.000000 cypherdataframe-0.3.1/cypherdataframe.egg-info/top_level.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-06-30 15:53:56.932807 cypherdataframe-0.3.1/setup.cfg
--rw-r--r--   0 avanderploeg   (501) staff       (20)      444 2023-06-30 15:50:10.000000 cypherdataframe-0.3.1/setup.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.926542 cypherdataframe-0.3.1/tests/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.3.1/tests/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.3.1/tests/branch_maker_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.3.1/tests/conftest.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.3.1/tests/cypher_integration_test.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.927212 cypherdataframe-0.3.1/tests/fixtures/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.1/tests/fixtures/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.929993 cypherdataframe-0.3.1/tests/fixtures/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.3.1/tests/fixtures/model/Branch_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.3.1/tests/fixtures/model/Node_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.3.1/tests/fixtures/model/Property_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.3.1/tests/fixtures/model/Query_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.1/tests/fixtures/model/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 15:53:56.932035 cypherdataframe-0.3.1/tests/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.3.1/tests/model/Branch_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.3.1/tests/model/Node_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.3.1/tests/model/Query_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.1/tests/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.3.1/tests/test_config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.3.1/tests/test_testfunctions.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.3.1/tests/tsest_ignorefunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.714344 cypherdataframe-0.3.2/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-06-30 16:09:02.714052 cypherdataframe-0.3.2/PKG-INFO
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.698204 cypherdataframe-0.3.2/cypherdataframe/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.3.2/cypherdataframe/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.3.2/cypherdataframe/branch_maker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.3.2/cypherdataframe/config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     9142 2023-06-29 21:29:55.000000 cypherdataframe-0.3.2/cypherdataframe/cypher.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.701229 cypherdataframe-0.3.2/cypherdataframe/garner_domain/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1340 2023-06-29 20:43:49.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/BranchMaker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.702085 cypherdataframe-0.3.2/cypherdataframe/garner_domain/logistics/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:02:39.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/logistics/TransferBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/logistics/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.702734 cypherdataframe-0.3.2/cypherdataframe/garner_domain/measure/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      634 2023-06-09 21:00:14.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/measure/MeasureBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/measure/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/properties_defaults.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.703465 cypherdataframe-0.3.2/cypherdataframe/garner_domain/queries/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      919 2023-06-29 20:44:47.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/queries/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.704130 cypherdataframe-0.3.2/cypherdataframe/garner_domain/reference/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      613 2023-06-29 21:20:43.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/reference/ReferenceBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/reference/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.705899 cypherdataframe-0.3.2/cypherdataframe/garner_domain/status/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:17:38.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-06-29 21:18:56.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/status/AttainedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      658 2023-06-29 21:17:38.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      615 2023-06-29 21:18:10.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/status/ForecastedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.2/cypherdataframe/garner_domain/status/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.708359 cypherdataframe-0.3.2/cypherdataframe/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2213 2023-06-15 17:59:52.000000 cypherdataframe-0.3.2/cypherdataframe/model/Branch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.3.2/cypherdataframe/model/Config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      829 2023-05-05 22:58:23.000000 cypherdataframe-0.3.2/cypherdataframe/model/LabelNode.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.3.2/cypherdataframe/model/Property.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.3.2/cypherdataframe/model/Query.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.3.2/cypherdataframe/model/QueryAccumulation.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.3.2/cypherdataframe/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.3.2/cypherdataframe/testfunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.700095 cypherdataframe-0.3.2/cypherdataframe.egg-info/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-06-30 16:09:02.000000 cypherdataframe-0.3.2/cypherdataframe.egg-info/PKG-INFO
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-06-30 16:09:02.000000 cypherdataframe-0.3.2/cypherdataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-06-30 16:09:02.000000 cypherdataframe-0.3.2/cypherdataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-06-30 16:09:02.000000 cypherdataframe-0.3.2/cypherdataframe.egg-info/requires.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-06-30 16:09:02.000000 cypherdataframe-0.3.2/cypherdataframe.egg-info/top_level.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-06-30 16:09:02.714450 cypherdataframe-0.3.2/setup.cfg
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-06-30 16:08:15.000000 cypherdataframe-0.3.2/setup.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.710596 cypherdataframe-0.3.2/tests/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.3.2/tests/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.3.2/tests/branch_maker_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.3.2/tests/conftest.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.3.2/tests/cypher_integration_test.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.710914 cypherdataframe-0.3.2/tests/fixtures/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.2/tests/fixtures/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.712440 cypherdataframe-0.3.2/tests/fixtures/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.3.2/tests/fixtures/model/Branch_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.3.2/tests/fixtures/model/Node_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.3.2/tests/fixtures/model/Property_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.3.2/tests/fixtures/model/Query_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.2/tests/fixtures/model/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-06-30 16:09:02.713705 cypherdataframe-0.3.2/tests/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.3.2/tests/model/Branch_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.3.2/tests/model/Node_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.3.2/tests/model/Query_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.2/tests/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.3.2/tests/test_config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.3.2/tests/test_testfunctions.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.3.2/tests/tsest_ignorefunctions.py
```

### Comparing `cypherdataframe-0.3.1/cypherdataframe/branch_maker.py` & `cypherdataframe-0.3.2/cypherdataframe/branch_maker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/cypherdataframe/cypher.py` & `cypherdataframe-0.3.2/cypherdataframe/cypher.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/cypherdataframe/garner_domain/BranchMaker.py` & `cypherdataframe-0.3.2/cypherdataframe/garner_domain/BranchMaker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/cypherdataframe/garner_domain/properties_defaults.py` & `cypherdataframe-0.3.2/cypherdataframe/garner_domain/properties_defaults.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/cypherdataframe/model/Branch.py` & `cypherdataframe-0.3.2/cypherdataframe/model/Branch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/cypherdataframe/model/LabelNode.py` & `cypherdataframe-0.3.2/cypherdataframe/model/LabelNode.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/cypherdataframe/model/Query.py` & `cypherdataframe-0.3.2/cypherdataframe/model/Query.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/cypherdataframe/model/QueryAccumulation.py` & `cypherdataframe-0.3.2/cypherdataframe/model/QueryAccumulation.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/tests/branch_maker_test.py` & `cypherdataframe-0.3.2/tests/branch_maker_test.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/tests/fixtures/model/Property_fixture.py` & `cypherdataframe-0.3.2/tests/fixtures/model/Property_fixture.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.1/tests/tsest_ignorefunctions.py` & `cypherdataframe-0.3.2/tests/tsest_ignorefunctions.py`

 * *Files identical despite different names*

