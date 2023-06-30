# Comparing `tmp/PyExpansion-0.0.1a20230628.tar.gz` & `tmp/PyExpansion-0.0.1a20230630.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyExpansion-0.0.1a20230628.tar", last modified: Wed Jun 28 14:16:13 2023, max compression
+gzip compressed data, was "PyExpansion-0.0.1a20230630.tar", last modified: Fri Jun 30 11:07:27 2023, max compression
```

## Comparing `PyExpansion-0.0.1a20230628.tar` & `PyExpansion-0.0.1a20230630.tar`

### file list

```diff
@@ -1,84 +1,112 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.325316 PyExpansion-0.0.1a20230628/
--rw-rw-rw-   0        0        0     1081 2023-06-17 07:28:57.000000 PyExpansion-0.0.1a20230628/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-06-17 09:17:44.000000 PyExpansion-0.0.1a20230628/MANIFEST.in
--rw-rw-rw-   0        0        0     1727 2023-06-28 14:16:13.309659 PyExpansion-0.0.1a20230628/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.094617 PyExpansion-0.0.1a20230628/PyExpansion/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:29:27.000000 PyExpansion-0.0.1a20230628/PyExpansion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.122188 PyExpansion-0.0.1a20230628/PyExpansion/application/
--rw-rw-rw-   0        0        0        0 2023-06-17 09:22:08.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.122188 PyExpansion-0.0.1a20230628/PyExpansion/application/datetime/
--rw-rw-rw-   0        0        0        0 2023-06-26 12:46:25.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/datetime/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.137860 PyExpansion-0.0.1a20230628/PyExpansion/application/finance/
--rw-rw-rw-   0        0        0        0 2023-06-26 08:09:50.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/finance/__init__.py
--rw-rw-rw-   0        0        0     2387 2023-06-26 13:44:48.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/finance/calculator.py
--rw-rw-rw-   0        0        0     1075 2023-06-26 09:41:55.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/finance/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.137860 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.153441 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/
--rw-rw-rw-   0        0        0        0 2023-06-17 03:59:05.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.169067 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/country/
--rw-rw-rw-   0        0        0     8543 2023-06-24 15:35:29.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/country/Malaysia.py
--rw-rw-rw-   0        0        0     2913 2023-06-24 10:35:35.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/country/Singapore.py
--rw-rw-rw-   0        0        0        0 2023-06-17 06:05:34.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/country/__init__.py
--rw-rw-rw-   0        0        0      215 2023-06-24 15:35:22.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/country/base.py
--rw-rw-rw-   0        0        0     1090 2023-06-24 09:43:29.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/main.py
--rw-rw-rw-   0        0        0      509 2023-06-24 15:34:57.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/status_code_list.py
--rw-rw-rw-   0        0        0     1827 2023-06-24 09:46:15.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/tests.py
--rw-rw-rw-   0        0        0        0 2023-06-22 15:31:40.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.184724 PyExpansion-0.0.1a20230628/PyExpansion/application/maths/
--rw-rw-rw-   0        0        0        0 2023-06-25 09:40:34.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/maths/__init__.py
--rw-rw-rw-   0        0        0     2037 2023-06-26 10:00:13.000000 PyExpansion-0.0.1a20230628/PyExpansion/application/maths/table.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.200310 PyExpansion-0.0.1a20230628/PyExpansion/common/
--rw-rw-rw-   0        0        0        0 2023-06-17 09:35:58.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/__init__.py
--rw-rw-rw-   0        0        0      144 2023-06-18 10:34:10.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/basic_function.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.215983 PyExpansion-0.0.1a20230628/PyExpansion/common/constants/
--rw-rw-rw-   0        0        0        0 2023-06-24 09:11:08.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/constants/__init__.py
--rw-rw-rw-   0        0        0      158 2023-06-24 09:13:45.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/constants/common.py
--rw-rw-rw-   0        0        0      118 2023-06-25 04:45:04.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/constants/datetime.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.215983 PyExpansion-0.0.1a20230628/PyExpansion/common/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-18 07:42:28.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/data_type/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.231599 PyExpansion-0.0.1a20230628/PyExpansion/common/data_type/lists/
--rw-rw-rw-   0        0        0        0 2023-06-18 08:46:51.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/data_type/lists/__init__.py
--rw-rw-rw-   0        0        0      464 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/data_type/lists/main.py
--rw-rw-rw-   0        0        0      327 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/data_type/lists/status_code_list.py
--rw-rw-rw-   0        0        0      395 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/data_type/lists/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.247173 PyExpansion-0.0.1a20230628/PyExpansion/common/date_time/
--rw-rw-rw-   0        0        0        0 2023-06-25 04:20:38.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/date_time/__init__.py
--rw-rw-rw-   0        0        0      765 2023-06-28 13:47:45.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/date_time/reality.py
--rw-rw-rw-   0        0        0      588 2023-06-26 13:12:55.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/date_time/utils.py
--rw-rw-rw-   0        0        0      989 2023-06-24 10:06:05.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/message.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.262842 PyExpansion-0.0.1a20230628/PyExpansion/common/status_code/
--rw-rw-rw-   0        0        0        0 2023-06-24 07:45:47.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/status_code/__init__.py
--rw-rw-rw-   0        0        0     9071 2023-06-25 01:23:17.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/status_code/http_code.py
--rw-rw-rw-   0        0        0      283 2023-06-25 02:14:18.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/status_code/utils.py
--rw-rw-rw-   0        0        0      618 2023-06-26 13:45:15.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/table.py
--rw-rw-rw-   0        0        0     2978 2023-06-24 15:34:07.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/utils.py
--rw-rw-rw-   0        0        0     2718 2023-06-24 08:09:05.000000 PyExpansion-0.0.1a20230628/PyExpansion/common/version_history.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.262842 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.278416 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyBrainFuck/
--rw-rw-rw-   0        0        0        0 2023-06-23 11:30:05.000000 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyBrainFuck/__init__.py
--rw-rw-rw-   0        0        0     4954 2023-06-26 09:06:49.000000 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyBrainFuck/main.py
--rw-rw-rw-   0        0        0      347 2023-06-26 09:06:49.000000 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyBrainFuck/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.278416 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyMorseCode/
--rw-rw-rw-   0        0        0        0 2023-06-26 03:12:56.000000 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyMorseCode/__init__.py
--rw-rw-rw-   0        0        0     1729 2023-06-26 07:44:02.000000 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyMorseCode/main.py
--rw-rw-rw-   0        0        0      211 2023-06-26 07:50:09.000000 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyMorseCode/tests.py
--rw-rw-rw-   0        0        0        0 2023-06-23 11:29:40.000000 PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/__init__.py
--rw-rw-rw-   0        0        0     1264 2023-06-28 14:15:08.000000 PyExpansion-0.0.1a20230628/PyExpansion/version.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.122188 PyExpansion-0.0.1a20230628/PyExpansion.egg-info/
--rw-rw-rw-   0        0        0     1727 2023-06-28 14:16:10.000000 PyExpansion-0.0.1a20230628/PyExpansion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2364 2023-06-28 14:16:10.000000 PyExpansion-0.0.1a20230628/PyExpansion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 14:16:10.000000 PyExpansion-0.0.1a20230628/PyExpansion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-28 14:16:10.000000 PyExpansion-0.0.1a20230628/PyExpansion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1566 2023-06-26 08:09:31.000000 PyExpansion-0.0.1a20230628/README.md
--rw-rw-rw-   0        0        0       42 2023-06-28 14:16:13.325316 PyExpansion-0.0.1a20230628/setup.cfg
--rw-rw-rw-   0        0        0      540 2023-06-28 14:10:39.000000 PyExpansion-0.0.1a20230628/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.294084 PyExpansion-0.0.1a20230628/undone/
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.309659 PyExpansion-0.0.1a20230628/undone/PyCalendar/
--rw-rw-rw-   0        0        0        0 2023-06-26 12:47:01.000000 PyExpansion-0.0.1a20230628/undone/PyCalendar/__init__.py
--rw-rw-rw-   0        0        0      379 2023-06-26 17:24:22.000000 PyExpansion-0.0.1a20230628/undone/PyCalendar/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:16:13.309659 PyExpansion-0.0.1a20230628/undone/PyCalendar/holiday/
--rw-rw-rw-   0        0        0        0 2023-06-26 17:25:02.000000 PyExpansion-0.0.1a20230628/undone/PyCalendar/holiday/__init__.py
--rw-rw-rw-   0        0        0       10 2023-06-26 17:26:43.000000 PyExpansion-0.0.1a20230628/undone/PyCalendar/holiday/common.py
--rw-rw-rw-   0        0        0      199 2023-06-27 00:36:32.000000 PyExpansion-0.0.1a20230628/undone/PyCalendar/main.py
--rw-rw-rw-   0        0        0        0 2023-06-26 17:36:00.000000 PyExpansion-0.0.1a20230628/undone/PyCalendar/utils.py
--rw-rw-rw-   0        0        0        0 2023-06-28 13:48:17.000000 PyExpansion-0.0.1a20230628/undone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.488536 PyExpansion-0.0.1a20230630/
+-rw-rw-rw-   0        0        0     1081 2023-06-17 07:28:57.000000 PyExpansion-0.0.1a20230630/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:17:44.000000 PyExpansion-0.0.1a20230630/MANIFEST.in
+-rw-rw-rw-   0        0        0     1727 2023-06-30 11:07:27.488536 PyExpansion-0.0.1a20230630/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.050809 PyExpansion-0.0.1a20230630/PyExpansion/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:29:27.000000 PyExpansion-0.0.1a20230630/PyExpansion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.081997 PyExpansion-0.0.1a20230630/PyExpansion/application/
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:22:08.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.081997 PyExpansion-0.0.1a20230630/PyExpansion/application/datetime/
+-rw-rw-rw-   0        0        0        0 2023-06-26 12:46:25.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/datetime/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.113242 PyExpansion-0.0.1a20230630/PyExpansion/application/finance/
+-rw-rw-rw-   0        0        0        0 2023-06-26 08:09:50.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/finance/__init__.py
+-rw-rw-rw-   0        0        0     2387 2023-06-26 13:44:48.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/finance/calculator.py
+-rw-rw-rw-   0        0        0     1075 2023-06-26 09:41:55.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/finance/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.113242 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.128866 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/
+-rw-rw-rw-   0        0        0        0 2023-06-17 03:59:05.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.175724 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/country/
+-rw-rw-rw-   0        0        0     8543 2023-06-24 15:35:29.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/country/Malaysia.py
+-rw-rw-rw-   0        0        0     2913 2023-06-24 10:35:35.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/country/Singapore.py
+-rw-rw-rw-   0        0        0        0 2023-06-17 06:05:34.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/country/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-06-24 15:35:22.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/country/base.py
+-rw-rw-rw-   0        0        0     1090 2023-06-24 09:43:29.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/main.py
+-rw-rw-rw-   0        0        0      509 2023-06-24 15:34:57.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/status_code_list.py
+-rw-rw-rw-   0        0        0     1827 2023-06-24 09:46:15.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/tests.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 15:31:40.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.191346 PyExpansion-0.0.1a20230630/PyExpansion/application/maths/
+-rw-rw-rw-   0        0        0        0 2023-06-25 09:40:34.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/maths/__init__.py
+-rw-rw-rw-   0        0        0     2037 2023-06-26 10:00:13.000000 PyExpansion-0.0.1a20230630/PyExpansion/application/maths/table.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.206977 PyExpansion-0.0.1a20230630/PyExpansion/common/
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:35:58.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-06-18 10:34:10.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/basic_function.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.222633 PyExpansion-0.0.1a20230630/PyExpansion/common/constants/
+-rw-rw-rw-   0        0        0        0 2023-06-24 09:11:08.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/constants/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-06-24 09:13:45.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/constants/common.py
+-rw-rw-rw-   0        0        0      118 2023-06-25 04:45:04.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/constants/datetime.py
+-rw-rw-rw-   0        0        0       59 2023-06-30 04:02:44.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/constants/file_extension.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.238211 PyExpansion-0.0.1a20230630/PyExpansion/common/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-18 07:42:28.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/data_type/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.253831 PyExpansion-0.0.1a20230630/PyExpansion/common/data_type/lists/
+-rw-rw-rw-   0        0        0        0 2023-06-18 08:46:51.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/data_type/lists/__init__.py
+-rw-rw-rw-   0        0        0      464 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/data_type/lists/main.py
+-rw-rw-rw-   0        0        0      327 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/data_type/lists/status_code_list.py
+-rw-rw-rw-   0        0        0      395 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/data_type/lists/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.285486 PyExpansion-0.0.1a20230630/PyExpansion/common/date_time/
+-rw-rw-rw-   0        0        0        0 2023-06-25 04:20:38.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/date_time/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-06-28 13:47:45.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/date_time/reality.py
+-rw-rw-rw-   0        0        0      588 2023-06-26 13:12:55.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/date_time/utils.py
+-rw-rw-rw-   0        0        0      989 2023-06-24 10:06:05.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/message.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.316727 PyExpansion-0.0.1a20230630/PyExpansion/common/status_code/
+-rw-rw-rw-   0        0        0        0 2023-06-24 07:45:47.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/status_code/__init__.py
+-rw-rw-rw-   0        0        0     9071 2023-06-25 01:23:17.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/status_code/http_code.py
+-rw-rw-rw-   0        0        0      283 2023-06-25 02:14:18.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/status_code/utils.py
+-rw-rw-rw-   0        0        0      618 2023-06-26 13:45:15.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/table.py
+-rw-rw-rw-   0        0        0     2978 2023-06-24 15:34:07.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/utils.py
+-rw-rw-rw-   0        0        0     2718 2023-06-24 08:09:05.000000 PyExpansion-0.0.1a20230630/PyExpansion/common/version_history.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.316727 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.347559 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyBrainFuck/
+-rw-rw-rw-   0        0        0        0 2023-06-23 11:30:05.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyBrainFuck/__init__.py
+-rw-rw-rw-   0        0        0     4954 2023-06-26 09:06:49.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyBrainFuck/main.py
+-rw-rw-rw-   0        0        0      347 2023-06-26 09:06:49.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyBrainFuck/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.347559 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyDeadFish/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:12:52.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyDeadFish/__init__.py
+-rw-rw-rw-   0        0        0     3227 2023-06-30 11:04:52.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyDeadFish/main.py
+-rw-rw-rw-   0        0        0      530 2023-06-30 11:05:16.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyDeadFish/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.363182 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyMorseCode/
+-rw-rw-rw-   0        0        0        0 2023-06-26 03:12:56.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyMorseCode/__init__.py
+-rw-rw-rw-   0        0        0     1729 2023-06-26 07:44:02.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyMorseCode/main.py
+-rw-rw-rw-   0        0        0      211 2023-06-26 07:50:09.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyMorseCode/tests.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 11:29:40.000000 PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/__init__.py
+-rw-rw-rw-   0        0        0     1421 2023-06-30 08:17:15.000000 PyExpansion-0.0.1a20230630/PyExpansion/version.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.066375 PyExpansion-0.0.1a20230630/PyExpansion.egg-info/
+-rw-rw-rw-   0        0        0     1727 2023-06-30 11:07:26.000000 PyExpansion-0.0.1a20230630/PyExpansion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3023 2023-06-30 11:07:26.000000 PyExpansion-0.0.1a20230630/PyExpansion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:07:26.000000 PyExpansion-0.0.1a20230630/PyExpansion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 11:07:26.000000 PyExpansion-0.0.1a20230630/PyExpansion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1566 2023-06-26 08:09:31.000000 PyExpansion-0.0.1a20230630/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 11:07:27.488536 PyExpansion-0.0.1a20230630/setup.cfg
+-rw-rw-rw-   0        0        0      540 2023-06-28 14:10:39.000000 PyExpansion-0.0.1a20230630/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.035134 PyExpansion-0.0.1a20230630/undone/
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.378802 PyExpansion-0.0.1a20230630/undone/OSstuff/
+-rw-rw-rw-   0        0        0        0 2023-06-04 11:15:03.000000 PyExpansion-0.0.1a20230630/undone/OSstuff/__init__.py
+-rw-rw-rw-   0        0        0     1839 2023-06-04 09:05:15.000000 PyExpansion-0.0.1a20230630/undone/OSstuff/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.394424 PyExpansion-0.0.1a20230630/undone/PyCalendar/
+-rw-rw-rw-   0        0        0        0 2023-06-26 12:47:01.000000 PyExpansion-0.0.1a20230630/undone/PyCalendar/__init__.py
+-rw-rw-rw-   0        0        0      379 2023-06-26 17:24:22.000000 PyExpansion-0.0.1a20230630/undone/PyCalendar/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.394424 PyExpansion-0.0.1a20230630/undone/PyCalendar/holiday/
+-rw-rw-rw-   0        0        0        0 2023-06-26 17:25:02.000000 PyExpansion-0.0.1a20230630/undone/PyCalendar/holiday/__init__.py
+-rw-rw-rw-   0        0        0       10 2023-06-26 17:26:43.000000 PyExpansion-0.0.1a20230630/undone/PyCalendar/holiday/common.py
+-rw-rw-rw-   0        0        0      199 2023-06-27 00:36:32.000000 PyExpansion-0.0.1a20230630/undone/PyCalendar/main.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 17:36:00.000000 PyExpansion-0.0.1a20230630/undone/PyCalendar/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.425665 PyExpansion-0.0.1a20230630/undone/PyCarPlate/
+-rw-rw-rw-   0        0        0        0 2023-06-18 05:49:46.000000 PyExpansion-0.0.1a20230630/undone/PyCarPlate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.441338 PyExpansion-0.0.1a20230630/undone/PyCarPlate/country/
+-rw-rw-rw-   0        0        0        0 2023-06-18 05:50:12.000000 PyExpansion-0.0.1a20230630/undone/PyCarPlate/country/__init__.py
+-rw-rw-rw-   0        0        0     1233 2023-06-18 15:37:34.000000 PyExpansion-0.0.1a20230630/undone/PyCarPlate/country/base.py
+-rw-rw-rw-   0        0        0      349 2023-06-18 15:26:14.000000 PyExpansion-0.0.1a20230630/undone/PyCarPlate/country/malaysia.py
+-rw-rw-rw-   0        0        0      942 2023-06-18 15:26:14.000000 PyExpansion-0.0.1a20230630/undone/PyCarPlate/main.py
+-rw-rw-rw-   0        0        0      574 2023-06-18 15:19:31.000000 PyExpansion-0.0.1a20230630/undone/PyCarPlate/status_code_list.py
+-rw-rw-rw-   0        0        0      615 2023-06-18 15:19:31.000000 PyExpansion-0.0.1a20230630/undone/PyCarPlate/tests.py
+-rw-rw-rw-   0        0        0      485 2023-06-18 15:15:05.000000 PyExpansion-0.0.1a20230630/undone/PyCarPlate/version.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.456960 PyExpansion-0.0.1a20230630/undone/common/
+-rw-rw-rw-   0        0        0        0 2023-06-05 13:35:50.000000 PyExpansion-0.0.1a20230630/undone/common/__init__.py
+-rw-rw-rw-   0        0        0     3824 2023-06-08 15:16:30.000000 PyExpansion-0.0.1a20230630/undone/common/extend.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.472582 PyExpansion-0.0.1a20230630/undone/math/
+-rw-rw-rw-   0        0        0        0 2023-06-04 07:19:20.000000 PyExpansion-0.0.1a20230630/undone/math/__init__.py
+-rw-rw-rw-   0        0        0      318 2023-06-04 09:59:26.000000 PyExpansion-0.0.1a20230630/undone/math/prime.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.472582 PyExpansion-0.0.1a20230630/undone/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 08:02:14.000000 PyExpansion-0.0.1a20230630/undone/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:07:27.472582 PyExpansion-0.0.1a20230630/undone/utils/pypi/
+-rw-rw-rw-   0        0        0        0 2023-06-04 08:06:48.000000 PyExpansion-0.0.1a20230630/undone/utils/pypi/__init__.py
+-rw-rw-rw-   0        0        0     1413 2023-06-04 11:15:11.000000 PyExpansion-0.0.1a20230630/undone/utils/pypi/create_pypi.py
```

### Comparing `PyExpansion-0.0.1a20230628/LICENSE.txt` & `PyExpansion-0.0.1a20230630/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PKG-INFO` & `PyExpansion-0.0.1a20230630/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyExpansion
-Version: 0.0.1a20230628
+Version: 0.0.1a20230630
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Overviews
 
 ![PyPI](https://img.shields.io/pypi/v/pyexpansion) &nbsp;
```

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/application/finance/calculator.py` & `PyExpansion-0.0.1a20230630/PyExpansion/application/finance/calculator.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/application/finance/utils.py` & `PyExpansion-0.0.1a20230630/PyExpansion/application/finance/utils.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/country/Malaysia.py` & `PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/country/Malaysia.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/country/Singapore.py` & `PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/country/Singapore.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/main.py` & `PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/main.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/application/human_resource/PyIC/tests.py` & `PyExpansion-0.0.1a20230630/PyExpansion/application/human_resource/PyIC/tests.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/application/maths/table.py` & `PyExpansion-0.0.1a20230630/PyExpansion/application/maths/table.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/common/date_time/reality.py` & `PyExpansion-0.0.1a20230630/PyExpansion/common/date_time/reality.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/common/date_time/utils.py` & `PyExpansion-0.0.1a20230630/PyExpansion/common/date_time/utils.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/common/message.py` & `PyExpansion-0.0.1a20230630/PyExpansion/common/message.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/common/status_code/http_code.py` & `PyExpansion-0.0.1a20230630/PyExpansion/common/status_code/http_code.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/common/table.py` & `PyExpansion-0.0.1a20230630/PyExpansion/common/table.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/common/utils.py` & `PyExpansion-0.0.1a20230630/PyExpansion/common/utils.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/common/version_history.py` & `PyExpansion-0.0.1a20230630/PyExpansion/common/version_history.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyBrainFuck/main.py` & `PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyBrainFuck/main.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/just_for_fun/PyMorseCode/main.py` & `PyExpansion-0.0.1a20230630/PyExpansion/just_for_fun/PyMorseCode/main.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion/version.py` & `PyExpansion-0.0.1a20230630/PyExpansion/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 
     def version_5(self):
         return self.default_setup(
             application_name="common",
             version="0.0.1a20230628"
         )
 
+    def version_6(self):
+        return self.default_setup(
+            application_name="PyDeadFish",
+            version="0.0.1a20230630"
+        )
+
 
 c = PyICVersionHistory()
 test = False
 if test:
     print("How many version:", c.total_version())
     print("Version list:", c.get_version_list())
     print("Latest version: ", c.get_latest_version())
```

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion.egg-info/PKG-INFO` & `PyExpansion-0.0.1a20230630/PyExpansion.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyExpansion
-Version: 0.0.1a20230628
+Version: 0.0.1a20230630
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Overviews
 
 ![PyPI](https://img.shields.io/pypi/v/pyexpansion) &nbsp;
```

### Comparing `PyExpansion-0.0.1a20230628/PyExpansion.egg-info/SOURCES.txt` & `PyExpansion-0.0.1a20230630/PyExpansion.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 PyExpansion/common/message.py
 PyExpansion/common/table.py
 PyExpansion/common/utils.py
 PyExpansion/common/version_history.py
 PyExpansion/common/constants/__init__.py
 PyExpansion/common/constants/common.py
 PyExpansion/common/constants/datetime.py
+PyExpansion/common/constants/file_extension.py
 PyExpansion/common/data_type/__init__.py
 PyExpansion/common/data_type/lists/__init__.py
 PyExpansion/common/data_type/lists/main.py
 PyExpansion/common/data_type/lists/status_code_list.py
 PyExpansion/common/data_type/lists/tests.py
 PyExpansion/common/date_time/__init__.py
 PyExpansion/common/date_time/reality.py
@@ -44,17 +45,36 @@
 PyExpansion/common/status_code/__init__.py
 PyExpansion/common/status_code/http_code.py
 PyExpansion/common/status_code/utils.py
 PyExpansion/just_for_fun/__init__.py
 PyExpansion/just_for_fun/PyBrainFuck/__init__.py
 PyExpansion/just_for_fun/PyBrainFuck/main.py
 PyExpansion/just_for_fun/PyBrainFuck/tests.py
+PyExpansion/just_for_fun/PyDeadFish/__init__.py
+PyExpansion/just_for_fun/PyDeadFish/main.py
+PyExpansion/just_for_fun/PyDeadFish/tests.py
 PyExpansion/just_for_fun/PyMorseCode/__init__.py
 PyExpansion/just_for_fun/PyMorseCode/main.py
 PyExpansion/just_for_fun/PyMorseCode/tests.py
-undone/__init__.py
+undone/OSstuff/__init__.py
+undone/OSstuff/utils.py
 undone/PyCalendar/__init__.py
 undone/PyCalendar/constants.py
 undone/PyCalendar/main.py
 undone/PyCalendar/utils.py
 undone/PyCalendar/holiday/__init__.py
-undone/PyCalendar/holiday/common.py
+undone/PyCalendar/holiday/common.py
+undone/PyCarPlate/__init__.py
+undone/PyCarPlate/main.py
+undone/PyCarPlate/status_code_list.py
+undone/PyCarPlate/tests.py
+undone/PyCarPlate/version.py
+undone/PyCarPlate/country/__init__.py
+undone/PyCarPlate/country/base.py
+undone/PyCarPlate/country/malaysia.py
+undone/common/__init__.py
+undone/common/extend.py
+undone/math/__init__.py
+undone/math/prime.py
+undone/utils/__init__.py
+undone/utils/pypi/__init__.py
+undone/utils/pypi/create_pypi.py
```

### Comparing `PyExpansion-0.0.1a20230628/README.md` & `PyExpansion-0.0.1a20230630/README.md`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230628/setup.py` & `PyExpansion-0.0.1a20230630/setup.py`

 * *Files identical despite different names*

