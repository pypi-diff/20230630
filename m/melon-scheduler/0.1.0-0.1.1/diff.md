# Comparing `tmp/melon_scheduler-0.1.0.tar.gz` & `tmp/melon_scheduler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_scheduler-0.1.0.tar", max compression
+gzip compressed data, was "melon_scheduler-0.1.1.tar", max compression
```

## Comparing `melon_scheduler-0.1.0.tar` & `melon_scheduler-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2108 2023-06-27 22:02:19.451664 melon_scheduler-0.1.0/README.md
--rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.0/melon/__init__.py
--rw-r--r--   0        0        0     4366 2023-06-30 13:07:13.877474 melon_scheduler-0.1.0/melon/calendar.py
--rw-r--r--   0        0        0      280 2023-06-22 13:28:19.950601 melon_scheduler-0.1.0/melon/config.py
--rw-r--r--   0        0        0      401 2023-06-26 13:37:58.951726 melon_scheduler-0.1.0/melon/libscheduler.rs
--rw-r--r--   0        0        0     7310 2023-06-30 13:04:39.283709 melon_scheduler-0.1.0/melon/melon.py
--rw-r--r--   0        0        0     6262 2023-06-30 12:22:34.016082 melon_scheduler-0.1.0/melon/scheduler.py
--rw-r--r--   0        0        0     6489 2023-06-30 12:44:19.705982 melon_scheduler-0.1.0/melon/todo.py
--rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.0/melongui/__init__.py
--rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.0/melongui/assets/complete.png
--rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.0/melongui/assets/complete.svg
--rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.0/melongui/calendarlist.py
--rw-r--r--   0        0        0     4882 2023-06-29 19:52:23.397332 melon_scheduler-0.1.0/melongui/mainwindow.py
--rw-r--r--   0        0        0     5980 2023-06-27 19:31:46.233422 melon_scheduler-0.1.0/melongui/taskitemdelegate.py
--rw-r--r--   0        0        0     5417 2023-06-26 15:51:18.939957 melon_scheduler-0.1.0/melongui/tasklist.py
--rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.0/melongui/taskwidgets.py
--rw-r--r--   0        0        0     1014 2023-06-30 13:44:21.672414 melon_scheduler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 melon_scheduler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2108 2023-06-27 22:02:19.451664 melon_scheduler-0.1.1/README.md
+-rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.1/melon/__init__.py
+-rw-r--r--   0        0        0     4366 2023-06-30 13:07:13.877474 melon_scheduler-0.1.1/melon/calendar.py
+-rw-r--r--   0        0        0      280 2023-06-22 13:28:19.950601 melon_scheduler-0.1.1/melon/config.py
+-rw-r--r--   0        0        0      401 2023-06-26 13:37:58.951726 melon_scheduler-0.1.1/melon/libscheduler.rs
+-rw-r--r--   0        0        0     7310 2023-06-30 13:04:39.283709 melon_scheduler-0.1.1/melon/melon.py
+-rw-r--r--   0        0        0     6262 2023-06-30 12:22:34.016082 melon_scheduler-0.1.1/melon/scheduler.py
+-rw-r--r--   0        0        0     6489 2023-06-30 12:44:19.705982 melon_scheduler-0.1.1/melon/todo.py
+-rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.1/melongui/__init__.py
+-rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.1/melongui/assets/complete.png
+-rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.1/melongui/assets/complete.svg
+-rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.1/melongui/calendarlist.py
+-rw-r--r--   0        0        0     4882 2023-06-29 19:52:23.397332 melon_scheduler-0.1.1/melongui/mainwindow.py
+-rw-r--r--   0        0        0     5980 2023-06-27 19:31:46.233422 melon_scheduler-0.1.1/melongui/taskitemdelegate.py
+-rw-r--r--   0        0        0     5417 2023-06-26 15:51:18.939957 melon_scheduler-0.1.1/melongui/tasklist.py
+-rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.1/melongui/taskwidgets.py
+-rw-r--r--   0        0        0     1057 2023-06-30 14:08:02.286025 melon_scheduler-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 melon_scheduler-0.1.1/PKG-INFO
```

### Comparing `melon_scheduler-0.1.0/README.md` & `melon_scheduler-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melon/calendar.py` & `melon_scheduler-0.1.1/melon/calendar.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melon/melon.py` & `melon_scheduler-0.1.1/melon/melon.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melon/scheduler.py` & `melon_scheduler-0.1.1/melon/scheduler.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melon/todo.py` & `melon_scheduler-0.1.1/melon/todo.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melongui/assets/complete.png` & `melon_scheduler-0.1.1/melongui/assets/complete.png`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melongui/assets/complete.svg` & `melon_scheduler-0.1.1/melongui/assets/complete.svg`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melongui/calendarlist.py` & `melon_scheduler-0.1.1/melongui/calendarlist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melongui/mainwindow.py` & `melon_scheduler-0.1.1/melongui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melongui/taskitemdelegate.py` & `melon_scheduler-0.1.1/melongui/taskitemdelegate.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melongui/tasklist.py` & `melon_scheduler-0.1.1/melongui/tasklist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/melongui/taskwidgets.py` & `melon_scheduler-0.1.1/melongui/taskwidgets.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.0/pyproject.toml` & `melon_scheduler-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "melon-scheduler"
-version = "0.1.0"
+version = "0.1.1"
 description = "Schedules Todos into your Calendar"
 authors = ["MrP01 <peter@waldert.at>"]
 readme = "README.md"
 packages = [
-  {include="melon"},
-  {include="melongui"},
+  { include = "melon" },
+  { include = "melongui" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10, <3.12"
 caldav = "^1.2.1"
 dateparser = "^1.1.8"
 tqdm = "^4.65.0"
-# numba = "^0.57.1"
-pyside6 = {version="<6.5", optional=true}
+tomli = { version = "^2.0.1", python = "<3.11" }
+pyside6 = { version = "<6.5", optional = true }
 
 [tool.poetry.extras]
 gui = ["pyside6"]
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.14.0"
 dill = "^0.3.6"
```

### Comparing `melon_scheduler-0.1.0/PKG-INFO` & `melon_scheduler-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: melon-scheduler
-Version: 0.1.0
+Version: 0.1.1
 Summary: Schedules Todos into your Calendar
 Author: MrP01
 Author-email: peter@waldert.at
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
 Requires-Dist: caldav (>=1.2.1,<2.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: pyside6 (<6.5) ; extra == "gui"
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Melon UI
 
 A CalDav Task Application written in Qt6.
```

