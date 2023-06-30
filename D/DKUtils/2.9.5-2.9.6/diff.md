# Comparing `tmp/DKUtils-2.9.5.tar.gz` & `tmp/DKUtils-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DKUtils-2.9.5.tar", last modified: Tue Aug 23 21:26:58 2022, max compression
+gzip compressed data, was "DKUtils-2.9.6.tar", last modified: Tue Aug 23 21:42:50 2022, max compression
```

## Comparing `DKUtils-2.9.5.tar` & `DKUtils-2.9.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.434568 DKUtils-2.9.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.430567 DKUtils-2.9.5/DKUtils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3963 2022-08-23 21:26:58.000000 DKUtils-2.9.5/DKUtils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1190 2022-08-23 21:26:58.000000 DKUtils-2.9.5/DKUtils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-23 21:26:58.000000 DKUtils-2.9.5/DKUtils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      249 2022-08-23 21:26:58.000000 DKUtils-2.9.5/DKUtils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-08-23 21:26:58.000000 DKUtils-2.9.5/DKUtils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3963 2022-08-23 21:26:58.434568 DKUtils-2.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2962 2022-08-23 21:26:25.000000 DKUtils-2.9.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.430567 DKUtils-2.9.5/dkutils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.430567 DKUtils-2.9.5/dkutils/alteryx_api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/alteryx_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12416 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/alteryx_api/gallery_client.py
--rw-r--r--   0 root         (0) root         (0)     1329 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.430567 DKUtils-2.9.5/dkutils/datakitchen_api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/datakitchen_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63394 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/datakitchen_api/datakitchen_client.py
--rw-r--r--   0 root         (0) root         (0)      593 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/datakitchen_api/datetime_utils.py
--rw-r--r--   0 root         (0) root         (0)    17427 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/datakitchen_api/kitchen.py
--rw-r--r--   0 root         (0) root         (0)    14474 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/datakitchen_api/order_run_monitor.py
--rw-r--r--   0 root         (0) root         (0)     8199 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/datakitchen_api/recipe.py
--rw-r--r--   0 root         (0) root         (0)    10546 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/datakitchen_api/tests_utils.py
--rw-r--r--   0 root         (0) root         (0)     5696 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/datakitchen_api/vault.py
--rw-r--r--   0 root         (0) root         (0)     1442 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/decorators.py
--rw-r--r--   0 root         (0) root         (0)     4398 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/dictionary_comparator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.430567 DKUtils-2.9.5/dkutils/gmail_api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/gmail_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11373 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/gmail_api/gmail_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.434568 DKUtils-2.9.5/dkutils/jira_api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/jira_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6678 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/jira_api/jira_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.434568 DKUtils-2.9.5/dkutils/reporting/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/reporting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5764 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/reporting/dataframe_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.434568 DKUtils-2.9.5/dkutils/smtp_api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/smtp_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3470 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/smtp_api/sender.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.434568 DKUtils-2.9.5/dkutils/ssh/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7503 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/ssh/remote_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.434568 DKUtils-2.9.5/dkutils/streamsets_api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/streamsets_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7948 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/streamsets_api/datacollector_client.py
--rw-r--r--   0 root         (0) root         (0)      918 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/util.py
--rw-r--r--   0 root         (0) root         (0)     5058 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:26:58.434568 DKUtils-2.9.5/dkutils/veeva_network_api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/veeva_network_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22826 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/veeva_network_api/veeva_network_client.py
--rw-r--r--   0 root         (0) root         (0)     1092 2022-08-23 21:26:25.000000 DKUtils-2.9.5/dkutils/wait_loop.py
--rw-r--r--   0 root         (0) root         (0)     1608 2022-08-23 21:26:58.434568 DKUtils-2.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1399 2022-08-23 21:26:25.000000 DKUtils-2.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.135306 DKUtils-2.9.6/DKUtils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3963 2022-08-23 21:42:50.000000 DKUtils-2.9.6/DKUtils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1190 2022-08-23 21:42:50.000000 DKUtils-2.9.6/DKUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-23 21:42:50.000000 DKUtils-2.9.6/DKUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      249 2022-08-23 21:42:50.000000 DKUtils-2.9.6/DKUtils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-23 21:42:50.000000 DKUtils-2.9.6/DKUtils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3963 2022-08-23 21:42:50.139305 DKUtils-2.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2962 2022-08-23 21:42:15.000000 DKUtils-2.9.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.135306 DKUtils-2.9.6/dkutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.135306 DKUtils-2.9.6/dkutils/alteryx_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/alteryx_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12416 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/alteryx_api/gallery_client.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/dkutils/datakitchen_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/datakitchen_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63394 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/datakitchen_api/datakitchen_client.py
+-rw-r--r--   0 root         (0) root         (0)      593 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/datakitchen_api/datetime_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17427 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/datakitchen_api/kitchen.py
+-rw-r--r--   0 root         (0) root         (0)    14687 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/datakitchen_api/order_run_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     8199 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/datakitchen_api/recipe.py
+-rw-r--r--   0 root         (0) root         (0)    10546 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/datakitchen_api/tests_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/datakitchen_api/vault.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/dictionary_comparator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/dkutils/gmail_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/gmail_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11373 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/gmail_api/gmail_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/dkutils/jira_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/jira_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6678 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/jira_api/jira_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/dkutils/reporting/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/reporting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/reporting/dataframe_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/dkutils/smtp_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/smtp_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3470 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/smtp_api/sender.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/dkutils/ssh/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7503 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/ssh/remote_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/dkutils/streamsets_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/streamsets_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7948 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/streamsets_api/datacollector_client.py
+-rw-r--r--   0 root         (0) root         (0)      918 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/util.py
+-rw-r--r--   0 root         (0) root         (0)     5058 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 21:42:50.139305 DKUtils-2.9.6/dkutils/veeva_network_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/veeva_network_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22826 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/veeva_network_api/veeva_network_client.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2022-08-23 21:42:15.000000 DKUtils-2.9.6/dkutils/wait_loop.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2022-08-23 21:42:50.139305 DKUtils-2.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1399 2022-08-23 21:42:15.000000 DKUtils-2.9.6/setup.py
```

### Comparing `DKUtils-2.9.5/DKUtils.egg-info/PKG-INFO` & `DKUtils-2.9.6/DKUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DKUtils
-Version: 2.9.5
+Version: 2.9.6
 Summary: DataKitchen Utils Library
 Home-page: https://github.com/DataKitchen/DKUtils
 Author: DataKitchen
 Author-email: info@datakitchen.io
 License: UNKNOWN
 Project-URL: Documentation, https://datakitchen.github.io/DKUtils
 Project-URL: Source Code, https://github.com/DataKitchen/DKUtils
```

### Comparing `DKUtils-2.9.5/DKUtils.egg-info/SOURCES.txt` & `DKUtils-2.9.6/DKUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/PKG-INFO` & `DKUtils-2.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DKUtils
-Version: 2.9.5
+Version: 2.9.6
 Summary: DataKitchen Utils Library
 Home-page: https://github.com/DataKitchen/DKUtils
 Author: DataKitchen
 Author-email: info@datakitchen.io
 License: UNKNOWN
 Project-URL: Documentation, https://datakitchen.github.io/DKUtils
 Project-URL: Source Code, https://github.com/DataKitchen/DKUtils
```

### Comparing `DKUtils-2.9.5/README.md` & `DKUtils-2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/alteryx_api/gallery_client.py` & `DKUtils-2.9.6/dkutils/alteryx_api/gallery_client.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/constants.py` & `DKUtils-2.9.6/dkutils/constants.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/datakitchen_api/datakitchen_client.py` & `DKUtils-2.9.6/dkutils/datakitchen_api/datakitchen_client.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/datakitchen_api/datetime_utils.py` & `DKUtils-2.9.6/dkutils/datakitchen_api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/datakitchen_api/kitchen.py` & `DKUtils-2.9.6/dkutils/datakitchen_api/kitchen.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/datakitchen_api/order_run_monitor.py` & `DKUtils-2.9.6/dkutils/datakitchen_api/order_run_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,25 +73,29 @@
     info: dict
 
     @property
     def status(self) -> str:
         return self.info['status']
 
     @status.setter
-    def status(self, status):
+    def status(self, status) -> None:
         self.info['status'] = status
 
     @property
     def start_time(self) -> int:
         if self.info['start_time'] is None or self.info['start_time'] == 0:
             # Due to a race condition, the start_time is occasionally 0 (i.e. 01/01/1970)
             # Due to a platform bug, the start_time is occasionally None
-            self.info['start_time'] = get_utc_timestamp()
+            self.start_time = get_utc_timestamp()
         return self.info['start_time']
 
+    @start_time.setter
+    def start_time(self, start_time) -> None:
+        self.info['start_time'] = start_time
+
     @property
     def running(self) -> bool:
         return self.status == NODE_RUNNING
 
     @property
     def succeeded(self) -> bool:
         return self.status == NODE_SUCCESSFULL
@@ -106,16 +110,18 @@
 
     def init(self):
         self._handle_event()
         return self
 
     def update(self, nodes_info: dict) -> None:
         new_status = nodes_info[self.name]['status']
+        start_time = nodes_info[self.name]['start_time']
         if self.status != new_status:
             self.status = new_status
+            self.start_time = start_time
             self._handle_event()
 
     def _handle_event(self) -> None:
         if self.running:
             self._publish_task_status_event(TaskStatus.STARTED)
         elif self.succeeded or self.stopped:
             self._publish_task_status_event(TaskStatus.COMPLETED)
```

### Comparing `DKUtils-2.9.5/dkutils/datakitchen_api/recipe.py` & `DKUtils-2.9.6/dkutils/datakitchen_api/recipe.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/datakitchen_api/tests_utils.py` & `DKUtils-2.9.6/dkutils/datakitchen_api/tests_utils.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/datakitchen_api/vault.py` & `DKUtils-2.9.6/dkutils/datakitchen_api/vault.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/decorators.py` & `DKUtils-2.9.6/dkutils/decorators.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/dictionary_comparator.py` & `DKUtils-2.9.6/dkutils/dictionary_comparator.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/gmail_api/gmail_client.py` & `DKUtils-2.9.6/dkutils/gmail_api/gmail_client.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/jira_api/jira_client.py` & `DKUtils-2.9.6/dkutils/jira_api/jira_client.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/reporting/dataframe_wrapper.py` & `DKUtils-2.9.6/dkutils/reporting/dataframe_wrapper.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/smtp_api/sender.py` & `DKUtils-2.9.6/dkutils/smtp_api/sender.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/ssh/remote_client.py` & `DKUtils-2.9.6/dkutils/ssh/remote_client.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/streamsets_api/datacollector_client.py` & `DKUtils-2.9.6/dkutils/streamsets_api/datacollector_client.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/util.py` & `DKUtils-2.9.6/dkutils/util.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/validation.py` & `DKUtils-2.9.6/dkutils/validation.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/veeva_network_api/veeva_network_client.py` & `DKUtils-2.9.6/dkutils/veeva_network_api/veeva_network_client.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/dkutils/wait_loop.py` & `DKUtils-2.9.6/dkutils/wait_loop.py`

 * *Files identical despite different names*

### Comparing `DKUtils-2.9.5/setup.cfg` & `DKUtils-2.9.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.9.5
+current_version = 2.9.6
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `DKUtils-2.9.5/setup.py` & `DKUtils-2.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DKUtils",
-    version="2.9.5",
+    version="2.9.6",
     author="DataKitchen",
     author_email="info@datakitchen.io",
     description="DataKitchen Utils Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DataKitchen/DKUtils",
     project_urls={
```

