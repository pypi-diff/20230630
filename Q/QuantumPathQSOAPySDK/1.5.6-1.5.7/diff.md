# Comparing `tmp/QuantumPathQSOAPySDK-1.5.6.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.5.6.tar", last modified: Fri Jun 30 07:20:53 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.5.7.tar", last modified: Fri Jun 30 08:01:30 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.5.6.tar` & `QuantumPathQSOAPySDK-1.5.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:53.022478 QuantumPathQSOAPySDK-1.5.6/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0      928 2023-06-30 07:20:53.021549 QuantumPathQSOAPySDK-1.5.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.848099 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0    43170 2023-06-29 15:26:36.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.881494 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/
--rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.889477 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/
--rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
--rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
--rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/components.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.892707 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/flow/
--rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
--rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.898451 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/gates/
--rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
--rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/gates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.921396 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
--rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/SolutionItem.py
--rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.932364 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/
--rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/__init__.py
--rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
--rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
--rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.945837 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/
--rw-rw-rw-   0        0        0     3303 2023-06-30 07:13:23.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/Context.py
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/Exception.py
--rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/apiConnection.py
--rw-rw-rw-   0        0        0     3216 2023-06-22 11:57:59.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/checker.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.880199 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      928 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 07:20:53.023125 QuantumPathQSOAPySDK-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-06-30 07:20:27.000000 QuantumPathQSOAPySDK-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.957292 QuantumPathQSOAPySDK-1.5.6/test/
--rw-rw-rw-   0        0        0       83 2023-06-30 07:16:32.000000 QuantumPathQSOAPySDK-1.5.6/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.974529 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/__init__.py
--rw-rw-rw-   0        0        0     4070 2023-06-30 07:20:02.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_ContextMethods.py
--rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_DynamicMethods.py
--rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_QSOAPlatform.py
--rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_SecurityMethods.py
--rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_StaticMethods.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:20:53.017207 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/__init__.py
--rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitFlow.py
--rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates.py
--rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates_gates1.py
--rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates_gates2.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.529219 QuantumPathQSOAPySDK-1.5.7/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      928 2023-06-30 08:01:30.528226 QuantumPathQSOAPySDK-1.5.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.167704 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0    43170 2023-06-29 15:26:36.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.220423 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/
+-rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.234349 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/
+-rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
+-rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/components.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.315819 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/flow/
+-rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
+-rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.349640 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/gates/
+-rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
+-rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/gates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.415099 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/FlowItem.py
+-rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/SolutionItem.py
+-rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.436709 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/
+-rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/__init__.py
+-rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
+-rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
+-rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.460589 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/
+-rw-rw-rw-   0        0        0     3542 2023-06-30 07:54:28.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/Context.py
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/Exception.py
+-rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/apiConnection.py
+-rw-rw-rw-   0        0        0     3216 2023-06-22 11:57:59.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/checker.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.215449 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-06-30 08:01:29.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-06-30 08:01:30.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 08:01:29.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-30 08:01:29.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-30 08:01:29.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 08:01:30.530215 QuantumPathQSOAPySDK-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-06-30 08:01:23.000000 QuantumPathQSOAPySDK-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.465557 QuantumPathQSOAPySDK-1.5.7/test/
+-rw-rw-rw-   0        0        0       83 2023-06-30 08:00:25.000000 QuantumPathQSOAPySDK-1.5.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.495398 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/__init__.py
+-rw-rw-rw-   0        0        0     4601 2023-06-30 07:59:05.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_ContextMethods.py
+-rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_DynamicMethods.py
+-rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_QSOAPlatform.py
+-rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_SecurityMethods.py
+-rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_StaticMethods.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.523248 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/__init__.py
+-rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates.py
+-rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates_gates1.py
+-rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates_gates2.py
```

### Comparing `QuantumPathQSOAPySDK-1.5.6/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.6
+Version: 1.5.7
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/components.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/components.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Application.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Asset.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/DeviceItem.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Execution.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/__init__.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/connectionPoints.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/connectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/Context.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/Context.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 
         qpathFile = ConfigParser(allow_no_value=True)
         qpathFileExists = qpathFile.read(str(Path.home()) + '\.qpath')
 
         if qpathFileExists:
             self.__activeEnvironment = eval(qpathFile.options('active-environment')[0])
             for key in qpathFile['custom-environments']:
-                customEnvironments.append((key, qpathFile['custom-environments'][key]))
+                value = qpathFile['custom-environments'][key]
+
+                if value[len(value)-1] != '/':
+                    value = value + '/'
+
+                customEnvironments.append((key, value))
         else:
             self.__activeEnvironment = ('default-environments', 'pro')
 
         self.__environments = {
             'default-environments': {
                 'pro': 'https://qsoa.quantumpath.app:8443/api/'
             },
@@ -75,14 +80,17 @@
 
     # SET ACTIVE ENVIRONMENT
     def setActiveEnvironment(self, environmentName: str, qSOATargetURL: str = None) -> tuple:
         if qSOATargetURL:
             if environmentName in self.__environments['default-environments']:
                 raise ValueError(f'Environment not valid, default-environments cannot be changed. Active environment is still {self.__activeEnvironment}')
 
+            if qSOATargetURL[len(qSOATargetURL)-1] != '/':
+                qSOATargetURL = qSOATargetURL + '/'
+
             self.__environments['custom-environments'][environmentName] = qSOATargetURL
 
         if environmentName in self.__environments['default-environments']:
             newActiveEnvironment = ('default-environments', environmentName)
         
         elif environmentName in self.__environments['custom-environments']:
             newActiveEnvironment = ('custom-environments', environmentName)
```

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/Exception.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/apiConnection.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/apiConnection.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/checker.py` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/checker.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.6
+Version: 1.5.7
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/setup.py` & `QuantumPathQSOAPySDK-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.5.6',
+  version='1.5.7',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_ContextMethods.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_ContextMethods.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,36 +52,48 @@
         qsoa = QSOAPlatform()
 
         setActiveEnvironment = qsoa.setActiveEnvironment('pro')
 
         self.assertIsInstance(setActiveEnvironment, tuple)
         self.assertEqual(setActiveEnvironment, ('default-environments', 'pro'))
     
-    # SET ACTIVE ENVIRONMENT qSOATargetURL
-    def test_setActiveEnvironment_qSOATargetURL(self):
+    # SET ACTIVE ENVIRONMENT qSOATargetURL SLASH
+    def test_setActiveEnvironment_qSOATargetURL_slash(self):
+        qsoa = QSOAPlatform()
+
+        setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url/')
+
+        customEnvironments = qsoa.getEnvironments()['custom-environments']
+
+        self.assertEqual(customEnvironments, {'custom': 'url/'})
+        self.assertIsInstance(setActiveEnvironment, tuple)
+        self.assertEqual(setActiveEnvironment, ('custom-environments', 'custom'))
+
+    # SET ACTIVE ENVIRONMENT qSOATargetURL NO SLASH
+    def test_setActiveEnvironment_qSOATargetURL_noSlash(self):
         qsoa = QSOAPlatform()
 
         setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url')
 
         customEnvironments = qsoa.getEnvironments()['custom-environments']
 
-        self.assertEqual(customEnvironments, {'custom': 'url'})
+        self.assertEqual(customEnvironments, {'custom': 'url/'})
         self.assertIsInstance(setActiveEnvironment, tuple)
         self.assertEqual(setActiveEnvironment, ('custom-environments', 'custom'))
 
     # SET ACTIVE ENVIRONMENT qSOATargetURL OVERRIDE
     def test_setActiveEnvironment_qSOATargetURL_override(self):
         qsoa = QSOAPlatform()
         qsoa.setActiveEnvironment('custom', 'url')
 
         setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url2')
 
         customEnvironments = qsoa.getEnvironments()['custom-environments']
 
-        self.assertEqual(customEnvironments, {'custom': 'url2'})
+        self.assertEqual(customEnvironments, {'custom': 'url2/'})
         self.assertIsInstance(setActiveEnvironment, tuple)
         self.assertEqual(setActiveEnvironment, ('custom-environments', 'custom'))
 
     # BAD ARGUMENT environmentName
     def test_setActiveEnvironment_badArgument_environmentName(self):
         qsoa = QSOAPlatform()
```

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_DynamicMethods.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_DynamicMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_SecurityMethods.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_SecurityMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_StaticMethods.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_StaticMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates_gates1.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates_gates1.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates_gates2.py` & `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates_gates2.py`

 * *Files identical despite different names*

