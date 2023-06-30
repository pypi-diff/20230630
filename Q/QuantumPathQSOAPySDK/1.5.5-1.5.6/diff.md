# Comparing `tmp/QuantumPathQSOAPySDK-1.5.5.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.5.5.tar", last modified: Tue Jun 27 11:54:45 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.5.6.tar", last modified: Fri Jun 30 07:20:53 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.5.5.tar` & `QuantumPathQSOAPySDK-1.5.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.060810 QuantumPathQSOAPySDK-1.5.5/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0      928 2023-06-27 11:54:45.059813 QuantumPathQSOAPySDK-1.5.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.921137 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0    42866 2023-06-27 06:40:09.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.958208 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/
--rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.966019 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/
--rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
--rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
--rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/components.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.971007 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/flow/
--rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
--rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.989012 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/gates/
--rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
--rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/gates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.009902 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
--rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/SolutionItem.py
--rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.019872 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/
--rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/__init__.py
--rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
--rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
--rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.028848 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/
--rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/Context.py
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/Exception.py
--rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/apiConnection.py
--rw-rw-rw-   0        0        0     3216 2023-06-22 11:57:59.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/checker.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.956044 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      928 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 11:54:45.060810 QuantumPathQSOAPySDK-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-06-27 11:54:12.000000 QuantumPathQSOAPySDK-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.032887 QuantumPathQSOAPySDK-1.5.5/test/
--rw-rw-rw-   0        0        0       83 2023-06-27 11:27:42.000000 QuantumPathQSOAPySDK-1.5.5/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.043856 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_ContextMethods.py
--rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_DynamicMethods.py
--rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_QSOAPlatform.py
--rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_SecurityMethods.py
--rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_StaticMethods.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.058122 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/__init__.py
--rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitFlow.py
--rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates.py
--rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates_gates1.py
--rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates_gates2.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:53.022478 QuantumPathQSOAPySDK-1.5.6/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      928 2023-06-30 07:20:53.021549 QuantumPathQSOAPySDK-1.5.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.848099 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0    43170 2023-06-29 15:26:36.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.881494 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/
+-rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.889477 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/
+-rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
+-rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/components.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.892707 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/flow/
+-rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
+-rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.898451 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/gates/
+-rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
+-rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/gates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.921396 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/FlowItem.py
+-rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/SolutionItem.py
+-rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.932364 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/
+-rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/__init__.py
+-rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
+-rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
+-rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.945837 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/
+-rw-rw-rw-   0        0        0     3303 2023-06-30 07:13:23.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/Context.py
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/Exception.py
+-rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/apiConnection.py
+-rw-rw-rw-   0        0        0     3216 2023-06-22 11:57:59.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/checker.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.880199 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-30 07:20:52.000000 QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 07:20:53.023125 QuantumPathQSOAPySDK-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-06-30 07:20:27.000000 QuantumPathQSOAPySDK-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.957292 QuantumPathQSOAPySDK-1.5.6/test/
+-rw-rw-rw-   0        0        0       83 2023-06-30 07:16:32.000000 QuantumPathQSOAPySDK-1.5.6/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:52.974529 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/__init__.py
+-rw-rw-rw-   0        0        0     4070 2023-06-30 07:20:02.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_ContextMethods.py
+-rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_DynamicMethods.py
+-rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_QSOAPlatform.py
+-rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_SecurityMethods.py
+-rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_StaticMethods.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:20:53.017207 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/__init__.py
+-rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates.py
+-rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates_gates1.py
+-rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates_gates2.py
```

### Comparing `QuantumPathQSOAPySDK-1.5.5/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.5
+Version: 1.5.6
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,36 +131,42 @@
         Output
         ----------
         tuple
         """
         return self.__context.getActiveEnvironment()
 
     # SET ACTIVE ENVIRONMENT
-    def setActiveEnvironment(self, environmentName: str) -> tuple:
+    def setActiveEnvironment(self, environmentName: str, qSOATargetURL: str = None) -> tuple:
         """
         Set active QuantumPath environment.
 
         Prerequisites
         ----------
         Existing QuantumPath environment.
 
         Parameters
         ----------
         environmentName : str
             QuantumPath environment name to set as active.
+        qSOATargetURL : str
+            Optional argument. New qSOA target URL to add to existing environments and set as active.
 
         Output
         ----------
         tuple
         """
         checkInputTypes(
             ('environmentName', environmentName, (str,))
         )
+        if qSOATargetURL:
+            checkInputTypes(
+                ('qSOATargetURL', qSOATargetURL, (str,))
+            )
 
-        return self.__context.setActiveEnvironment(environmentName)
+        return self.__context.setActiveEnvironment(environmentName, qSOATargetURL)
 
 
     ##################_____SECURITY METHODS_____##################
 
     # ENCODE PASSWORD
     def encodePassword(self, password: str):
         """
```

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/components.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/annealing/components.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Application.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Asset.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/DeviceItem.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Execution.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/__init__.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/connectionPoints.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/connectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/Context.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/Context.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,64 +4,46 @@
 from configparser import ConfigParser
 
 
 class Context:
 
     # CONSTRUCTOR
     def __init__(self, username: str = None, password: str = None, url: str = None):
-        self.__environments = {
-            'default-environments': {
-                'pro': 'https://qsoa.quantumpath.app:8443/api/'
-            },
-            'custom-environments': {}
-        }
+        customEnvironments = []
 
         qpathFile = ConfigParser(allow_no_value=True)
         qpathFileExists = qpathFile.read(str(Path.home()) + '\.qpath')
+
         if qpathFileExists:
             self.__activeEnvironment = eval(qpathFile.options('active-environment')[0])
+            for key in qpathFile['custom-environments']:
+                customEnvironments.append((key, qpathFile['custom-environments'][key]))
         else:
             self.__activeEnvironment = ('default-environments', 'pro')
 
+        self.__environments = {
+            'default-environments': {
+                'pro': 'https://qsoa.quantumpath.app:8443/api/'
+            },
+            'custom-environments': dict(customEnvironments)
+        }
+
         self.__credentials = {
             "Username": username,
             "Password": password
         } if username else None
 
         self.__authToken = apiConnection(url, self.__credentials, 'string', 'data') if username else None
 
         self.__header = {
             "Authorization": 'Bearer ' + str(self.__authToken)
         } if username else None
 
-    # PRIVATE METHODS
-    def __updateEnviroments(self):
-        customEnvironments = list()
-
-        qpathFile = ConfigParser(allow_no_value=True)
-        qpathFileExists = qpathFile.read(str(Path.home()) + '\.qpath')
-
-        if qpathFileExists:
-            for key in qpathFile['custom-environments']:
-                customEnvironments.append((key, qpathFile['custom-environments'][key]))
-                
-        self.__environments = {
-            'default-environments': {
-                'pro': 'https://qsoa.quantumpath.app:8443/api/'
-            },
-            'custom-environments': dict(customEnvironments)
-        }
 
     # GETTERS
-    def getEnvironments(self) -> dict:
-        return self.__environments
-
-    def getActiveEnvironment(self) -> dict:
-        return self.__activeEnvironment
-
     def getCredentials(self) -> dict:
         return self.__credentials
 
     def getAuthToken(self) -> str:
         return self.__authToken
     
     def getHeader(self) -> dict:
@@ -81,29 +63,27 @@
 
         self.__header = {
             "Authorization": 'Bearer ' + str(self.__authToken)
         }
 
     # GET ENVIRONMENTS
     def getEnvironments(self) -> dict:
-        qpathFile = ConfigParser(allow_no_value=True)
-        qpathFileExists = qpathFile.read(str(Path.home()) + '\.qpath')
-
-        if qpathFileExists:
-            self.__updateEnviroments()
-
         return self.__environments
 
     # GET ACTIVE ENVIRONMENT
     def getActiveEnvironment(self) -> tuple:
         return self.__activeEnvironment
 
     # SET ACTIVE ENVIRONMENT
-    def setActiveEnvironment(self, environmentName: str) -> tuple:
-        self.__updateEnviroments()
+    def setActiveEnvironment(self, environmentName: str, qSOATargetURL: str = None) -> tuple:
+        if qSOATargetURL:
+            if environmentName in self.__environments['default-environments']:
+                raise ValueError(f'Environment not valid, default-environments cannot be changed. Active environment is still {self.__activeEnvironment}')
+
+            self.__environments['custom-environments'][environmentName] = qSOATargetURL
 
         if environmentName in self.__environments['default-environments']:
             newActiveEnvironment = ('default-environments', environmentName)
         
         elif environmentName in self.__environments['custom-environments']:
             newActiveEnvironment = ('custom-environments', environmentName)
```

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/Exception.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/apiConnection.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/apiConnection.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/checker.py` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK/utils/checker.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.5
+Version: 1.5.6
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.5.6/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/setup.py` & `QuantumPathQSOAPySDK-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.5.5',
+  version='1.5.6',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_DynamicMethods.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_DynamicMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_SecurityMethods.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_SecurityMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_StaticMethods.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_QSOAPlatform/test_StaticMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates_gates1.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates_gates1.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates_gates2.py` & `QuantumPathQSOAPySDK-1.5.6/test/test_circuit/test_CircuitGates_gates2.py`

 * *Files identical despite different names*

