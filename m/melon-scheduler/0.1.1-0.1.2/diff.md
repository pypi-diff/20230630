# Comparing `tmp/melon_scheduler-0.1.1.tar.gz` & `tmp/melon_scheduler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_scheduler-0.1.1.tar", max compression
+gzip compressed data, was "melon_scheduler-0.1.2.tar", max compression
```

## Comparing `melon_scheduler-0.1.1.tar` & `melon_scheduler-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2108 2023-06-27 22:02:19.451664 melon_scheduler-0.1.1/README.md
--rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.1/melon/__init__.py
--rw-r--r--   0        0        0     4366 2023-06-30 13:07:13.877474 melon_scheduler-0.1.1/melon/calendar.py
--rw-r--r--   0        0        0      280 2023-06-22 13:28:19.950601 melon_scheduler-0.1.1/melon/config.py
--rw-r--r--   0        0        0      401 2023-06-26 13:37:58.951726 melon_scheduler-0.1.1/melon/libscheduler.rs
--rw-r--r--   0        0        0     7310 2023-06-30 13:04:39.283709 melon_scheduler-0.1.1/melon/melon.py
--rw-r--r--   0        0        0     6262 2023-06-30 12:22:34.016082 melon_scheduler-0.1.1/melon/scheduler.py
--rw-r--r--   0        0        0     6489 2023-06-30 12:44:19.705982 melon_scheduler-0.1.1/melon/todo.py
--rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.1/melongui/__init__.py
--rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.1/melongui/assets/complete.png
--rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.1/melongui/assets/complete.svg
--rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.1/melongui/calendarlist.py
--rw-r--r--   0        0        0     4882 2023-06-29 19:52:23.397332 melon_scheduler-0.1.1/melongui/mainwindow.py
--rw-r--r--   0        0        0     5980 2023-06-27 19:31:46.233422 melon_scheduler-0.1.1/melongui/taskitemdelegate.py
--rw-r--r--   0        0        0     5417 2023-06-26 15:51:18.939957 melon_scheduler-0.1.1/melongui/tasklist.py
--rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.1/melongui/taskwidgets.py
--rw-r--r--   0        0        0     1057 2023-06-30 14:08:02.286025 melon_scheduler-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 melon_scheduler-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2108 2023-06-27 22:02:19.451664 melon_scheduler-0.1.2/README.md
+-rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.2/melon/__init__.py
+-rw-r--r--   0        0        0     4366 2023-06-30 13:07:13.877474 melon_scheduler-0.1.2/melon/calendar.py
+-rw-r--r--   0        0        0      337 2023-06-30 14:09:58.520159 melon_scheduler-0.1.2/melon/config.py
+-rw-r--r--   0        0        0      401 2023-06-26 13:37:58.951726 melon_scheduler-0.1.2/melon/libscheduler.rs
+-rw-r--r--   0        0        0     7310 2023-06-30 13:04:39.283709 melon_scheduler-0.1.2/melon/melon.py
+-rw-r--r--   0        0        0     6262 2023-06-30 12:22:34.016082 melon_scheduler-0.1.2/melon/scheduler.py
+-rw-r--r--   0        0        0     6489 2023-06-30 12:44:19.705982 melon_scheduler-0.1.2/melon/todo.py
+-rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.2/melongui/__init__.py
+-rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.2/melongui/assets/complete.png
+-rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.2/melongui/assets/complete.svg
+-rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.2/melongui/calendarlist.py
+-rw-r--r--   0        0        0     4882 2023-06-29 19:52:23.397332 melon_scheduler-0.1.2/melongui/mainwindow.py
+-rw-r--r--   0        0        0     5980 2023-06-27 19:31:46.233422 melon_scheduler-0.1.2/melongui/taskitemdelegate.py
+-rw-r--r--   0        0        0     5417 2023-06-26 15:51:18.939957 melon_scheduler-0.1.2/melongui/tasklist.py
+-rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.2/melongui/taskwidgets.py
+-rw-r--r--   0        0        0     1057 2023-06-30 14:10:42.091424 melon_scheduler-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 melon_scheduler-0.1.2/PKG-INFO
```

### Comparing `melon_scheduler-0.1.1/README.md` & `melon_scheduler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melon/calendar.py` & `melon_scheduler-0.1.2/melon/calendar.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melon/melon.py` & `melon_scheduler-0.1.2/melon/melon.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melon/scheduler.py` & `melon_scheduler-0.1.2/melon/scheduler.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melon/todo.py` & `melon_scheduler-0.1.2/melon/todo.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melongui/assets/complete.png` & `melon_scheduler-0.1.2/melongui/assets/complete.png`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melongui/assets/complete.svg` & `melon_scheduler-0.1.2/melongui/assets/complete.svg`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melongui/calendarlist.py` & `melon_scheduler-0.1.2/melongui/calendarlist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melongui/mainwindow.py` & `melon_scheduler-0.1.2/melongui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melongui/taskitemdelegate.py` & `melon_scheduler-0.1.2/melongui/taskitemdelegate.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melongui/tasklist.py` & `melon_scheduler-0.1.2/melongui/tasklist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/melongui/taskwidgets.py` & `melon_scheduler-0.1.2/melongui/taskwidgets.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.1/pyproject.toml` & `melon_scheduler-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "melon-scheduler"
-version = "0.1.1"
+version = "0.1.2"
 description = "Schedules Todos into your Calendar"
 authors = ["MrP01 <peter@waldert.at>"]
 readme = "README.md"
 packages = [
   { include = "melon" },
   { include = "melongui" },
 ]
```

### Comparing `melon_scheduler-0.1.1/PKG-INFO` & `melon_scheduler-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melon-scheduler
-Version: 0.1.1
+Version: 0.1.2
 Summary: Schedules Todos into your Calendar
 Author: MrP01
 Author-email: peter@waldert.at
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

