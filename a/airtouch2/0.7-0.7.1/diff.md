# Comparing `tmp/airtouch2-0.7.tar.gz` & `tmp/airtouch2-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch2-0.7.tar", last modified: Sun Jun 25 08:50:15 2023, max compression
+gzip compressed data, was "airtouch2-0.7.1.tar", last modified: Fri Jun 30 10:34:18 2023, max compression
```

## Comparing `airtouch2-0.7.tar` & `airtouch2-0.7.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.368157 airtouch2-0.7/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7/LICENSE
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2279 2023-06-25 08:50:15.368157 airtouch2-0.7/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)      271 2023-01-10 07:31:33.000000 airtouch2-0.7/README.md
--rw-r--r--   0 nathan    (1000) nathan    (1000)      850 2023-06-25 08:46:07.000000 airtouch2-0.7/pyproject.toml
--rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-06-25 08:50:15.368157 airtouch2-0.7/setup.cfg
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      236 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     5462 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2/At2Aircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3653 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2/At2Client.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3301 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2/At2Group.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2777 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2plus/At2PlusAircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     8229 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2plus/At2PlusClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/at2plus/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/common/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2227 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/common/Buffer.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4349 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/common/NetClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/common/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      428 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/common/interfaces.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/helpers/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/helpers/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/helpers/diff_bytes.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/protocol/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7/src/airtouch2/protocol/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/protocol/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2584 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2773 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      647 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/lookups.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      307 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2/protocol/at2/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/RequestState.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     5046 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/ResponseMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      339 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2861 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/ac_commands.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2/messages/group_commands.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.368157 airtouch2-0.7/src/airtouch2/protocol/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/control_status_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/crc16_modbus.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/extended_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3941 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.368157 airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcControl.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcStatus.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:50:15.364157 airtouch2-0.7/src/airtouch2.egg-info/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2279 2023-06-25 08:50:15.000000 airtouch2-0.7/src/airtouch2.egg-info/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1675 2023-06-25 08:50:15.000000 airtouch2-0.7/src/airtouch2.egg-info/SOURCES.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-06-25 08:50:15.000000 airtouch2-0.7/src/airtouch2.egg-info/dependency_links.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-06-25 08:50:15.000000 airtouch2-0.7/src/airtouch2.egg-info/top_level.txt
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.433845 airtouch2-0.7.1/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.1/LICENSE
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-06-30 10:34:18.433845 airtouch2-0.7.1/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      271 2023-01-10 07:31:33.000000 airtouch2-0.7.1/README.md
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-06-30 10:33:39.000000 airtouch2-0.7.1/pyproject.toml
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-06-30 10:34:18.433845 airtouch2-0.7.1/setup.cfg
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.425845 airtouch2-0.7.1/src/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.429845 airtouch2-0.7.1/src/airtouch2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      236 2023-06-25 11:43:58.000000 airtouch2-0.7.1/src/airtouch2/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.429845 airtouch2-0.7.1/src/airtouch2/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     5511 2023-06-28 10:35:59.000000 airtouch2-0.7.1/src/airtouch2/at2/At2Aircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3653 2023-06-25 11:44:39.000000 airtouch2-0.7.1/src/airtouch2/at2/At2Client.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3301 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/at2/At2Group.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/at2/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.429845 airtouch2-0.7.1/src/airtouch2/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-06-28 10:35:27.000000 airtouch2-0.7.1/src/airtouch2/at2plus/At2PlusAircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     8229 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/at2plus/At2PlusClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/at2plus/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.429845 airtouch2-0.7.1/src/airtouch2/common/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2227 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/common/Buffer.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4729 2023-06-30 10:19:45.000000 airtouch2-0.7.1/src/airtouch2/common/NetClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/common/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1127 2023-06-28 10:43:48.000000 airtouch2-0.7.1/src/airtouch2/common/interfaces.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.429845 airtouch2-0.7.1/src/airtouch2/helpers/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/helpers/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/helpers/diff_bytes.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.429845 airtouch2-0.7.1/src/airtouch2/protocol/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.1/src/airtouch2/protocol/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.433845 airtouch2-0.7.1/src/airtouch2/protocol/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2584 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2773 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      647 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/lookups.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      307 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.433845 airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/RequestState.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     5046 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/ResponseMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      339 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2861 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/ac_commands.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/group_commands.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.433845 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/control_status_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/crc16_modbus.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/extended_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3941 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.433845 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/messages/AcControl.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.1/src/airtouch2/protocol/at2plus/messages/AcStatus.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-30 10:34:18.429845 airtouch2-0.7.1/src/airtouch2.egg-info/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-06-30 10:34:18.000000 airtouch2-0.7.1/src/airtouch2.egg-info/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1675 2023-06-30 10:34:18.000000 airtouch2-0.7.1/src/airtouch2.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-06-30 10:34:18.000000 airtouch2-0.7.1/src/airtouch2.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-06-30 10:34:18.000000 airtouch2-0.7.1/src/airtouch2.egg-info/top_level.txt
```

### Comparing `airtouch2-0.7/LICENSE` & `airtouch2-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/PKG-INFO` & `airtouch2-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7
+Version: 0.7.1
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtouch2-0.7/pyproject.toml` & `airtouch2-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtouch2"
 description = "API for the monitoring and control of a Polyaire Airtouch 2 system over the local network"
-version = "0.7"
+version = "0.7.1"
 authors = [{ name = "Nathan Van der Hoek", email = "nathan.vanderhoek@student.adelaide.edu.au" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `airtouch2-0.7/src/airtouch2/at2/At2Aircon.py` & `airtouch2-0.7.1/src/airtouch2/at2/At2Aircon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 import asyncio
 import logging
 from itertools import compress
 from typing import TYPE_CHECKING, Callable
+from airtouch2.common.interfaces import Callback
 from airtouch2.protocol.at2.conversions import brand_from_gateway_id, fan_speed_from_val, supported_fan_speeds, val_from_fan_speed
 if TYPE_CHECKING:
     from airtouch2.at2.At2Client import At2Client
 from airtouch2.protocol.at2.enums import ACFanSpeedReference, ACBrand, ACMode
 from airtouch2.protocol.at2.messages import ChangeSetTemperature, ResponseMessage, SetFanSpeed, SetMode, ToggleAc
 from airtouch2.protocol.at2.lookups import GATEWAYID_BRAND_LOOKUP
 
@@ -79,15 +80,15 @@
             _LOGGER.warning(f"AC{self.number} appears disconnected from airtouch")
 
         self.name = response_message.ac_name[self.number]
 
         for callback in self._callbacks:
             callback()
 
-    def add_callback(self, func: Callable) -> Callable:
+    def add_callback(self, func: Callback) -> Callback:
         self._callbacks.append(func)
 
         def remove_callback() -> None:
             if func in self._callbacks:
                 self._callbacks.remove(func)
 
         return remove_callback
```

### Comparing `airtouch2-0.7/src/airtouch2/at2/At2Client.py` & `airtouch2-0.7.1/src/airtouch2/at2/At2Client.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/at2/At2Group.py` & `airtouch2-0.7.1/src/airtouch2/at2/At2Group.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/at2plus/At2PlusAircon.py` & `airtouch2-0.7.1/src/airtouch2/at2plus/At2PlusAircon.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     async def set_setpoint(self, setpoint: float):
         settings = AcSettings(self.status.id, AcSetPower.UNCHANGED, AcSetMode.UNCHANGED, AcFanSpeed.UNCHANGED, setpoint)
         await self._client.send(AcControlMessage([settings]))
 
     async def wait_until_ready(self) -> None:
         await self._ready.wait()
 
-    def add_callback(self, callback: Callback):
+    def add_callback(self, callback: Callback) -> Callback:
         self._callbacks.append(callback)
 
         def remove_callback() -> None:
             if callback in self._callbacks:
                 self._callbacks.remove(callback)
 
         return remove_callback
```

### Comparing `airtouch2-0.7/src/airtouch2/at2plus/At2PlusClient.py` & `airtouch2-0.7.1/src/airtouch2/at2plus/At2PlusClient.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/common/Buffer.py` & `airtouch2-0.7.1/src/airtouch2/common/Buffer.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/common/NetClient.py` & `airtouch2-0.7.1/src/airtouch2/common/NetClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,29 +68,39 @@
         """Send the serializable 'message'"""
         if self._writer is None:
             raise RuntimeError("Client is not connected - call connect() first")
         else:
             bytes_to_write = message.to_bytes()
             _LOGGER.debug(f"Sending {message.__class__.__name__} with data: {bytes_to_write.hex(':')}")
             self._writer.write(bytes_to_write)
-            await self._writer.drain()
+            drained: bool = False
+            while not drained:
+                try:
+                    await self._writer.drain()
+                    drained = True
+                except (ConnectionResetError, asyncio.IncompleteReadError) as e:
+                    await self._try_reconnect()
 
     async def read_bytes(self, size: int) -> bytes | None:
         """
         Read exactly 'size' bytes, return None if could not read enough bytes or on disconnection and reconnection.
         This coroutine handles reconnection.
         """
         if self._reader is None:
             raise RuntimeError("Client is not connected - call connect() first")
         try:
             data = await self._reader.readexactly(size)
         except asyncio.IncompleteReadError as e:
             _LOGGER.debug(f"IncompleteReadError - partial bytes: {e.partial.hex(':')}")
             data = None
-        if not data:
+        except ConnectionResetError as e:
+            _LOGGER.debug(f"ConnectionResetError")
+            data = None
+
+        if data is None:
             _LOGGER.warning("Connection lost, reconnecting")
             await self._try_reconnect()
             return None
         _LOGGER.debug(f"Read payload of size {size}: {data.hex(':')}")
         return data
 
     async def _main(self) -> None:
```

### Comparing `airtouch2-0.7/src/airtouch2/helpers/diff_bytes.py` & `airtouch2-0.7.1/src/airtouch2/helpers/diff_bytes.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2/constants.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2/constants.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2/conversions.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2/enums.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2/lookups.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2/lookups.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2/messages/RequestState.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/RequestState.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2/messages/ResponseMessage.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/ResponseMessage.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2/messages/ac_commands.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/ac_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2/messages/group_commands.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2/messages/group_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/control_status_common.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/control_status_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/conversions.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/crc16_modbus.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/enums.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/extended_common.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/extended_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/message_common.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/message_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcControl.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/messages/AcControl.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2/protocol/at2plus/messages/AcStatus.py` & `airtouch2-0.7.1/src/airtouch2/protocol/at2plus/messages/AcStatus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7/src/airtouch2.egg-info/PKG-INFO` & `airtouch2-0.7.1/src/airtouch2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7
+Version: 0.7.1
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtouch2-0.7/src/airtouch2.egg-info/SOURCES.txt` & `airtouch2-0.7.1/src/airtouch2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

