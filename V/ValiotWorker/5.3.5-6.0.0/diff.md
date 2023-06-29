# Comparing `tmp/ValiotWorker-5.3.5.tar.gz` & `tmp/ValiotWorker-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ValiotWorker-5.3.5.tar", last modified: Thu Jun 15 14:28:52 2023, max compression
+gzip compressed data, was "ValiotWorker-6.0.0.tar", last modified: Thu Jun 29 22:45:13 2023, max compression
```

## Comparing `ValiotWorker-5.3.5.tar` & `ValiotWorker-6.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.398371 ValiotWorker-5.3.5/
--rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-5.3.5/LICENCE
--rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-5.3.5/MANIFEST.in
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-06-15 14:28:52.398170 ValiotWorker-5.3.5/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-5.3.5/README.md
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.394583 ValiotWorker-5.3.5/ValiotWorker/
--rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-04-19 23:58:36.000000 ValiotWorker-5.3.5/ValiotWorker/Logging.py
--rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-5.3.5/ValiotWorker/Notifications.py
--rw-r--r--   0 baruc      (501) staff       (20)      294 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/__main__.py
--rw-r--r--   0 baruc      (501) staff       (20)       22 2023-06-15 04:32:45.000000 ValiotWorker-5.3.5/ValiotWorker/__version__.py
--rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-5.3.5/ValiotWorker/croniterHelpers.py
--rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-5.3.5/ValiotWorker/dateHelpers.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.396978 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/
--rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/__main__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.397475 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/modules/
--rw-r--r--   0 baruc      (501) staff       (20)        0 2023-06-15 04:43:52.000000 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/modules/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/modules/http_server.py
--rw-r--r--   0 baruc      (501) staff       (20)     7019 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/mutations.py
--rw-r--r--   0 baruc      (501) staff       (20)     4394 2023-03-07 23:36:56.000000 ValiotWorker-5.3.5/ValiotWorker/queries.py
--rw-r--r--   0 baruc      (501) staff       (20)     5885 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/redis.py
--rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/subscriptions.py
--rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-5.3.5/ValiotWorker/uploaders.py
--rw-r--r--   0 baruc      (501) staff       (20)    69826 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/worker.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.396473 ValiotWorker-5.3.5/ValiotWorker.egg-info/
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)      841 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/SOURCES.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/dependency_links.txt
--rw-r--r--   0 baruc      (501) staff       (20)       60 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/entry_points.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/not-zip-safe
--rw-r--r--   0 baruc      (501) staff       (20)      233 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/requires.txt
--rw-r--r--   0 baruc      (501) staff       (20)       13 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/top_level.txt
--rw-r--r--   0 baruc      (501) staff       (20)       38 2023-06-15 14:28:52.398425 ValiotWorker-5.3.5/setup.cfg
--rw-r--r--   0 baruc      (501) staff       (20)     2607 2023-06-15 04:31:00.000000 ValiotWorker-5.3.5/setup.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.397805 ValiotWorker-5.3.5/tests/
--rw-r--r--   0 baruc      (501) staff       (20)      106 2023-06-15 03:50:01.000000 ValiotWorker-5.3.5/tests/test_dummy.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.611581 ValiotWorker-6.0.0/
+-rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-6.0.0/LICENCE
+-rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-6.0.0/MANIFEST.in
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-06-29 22:45:13.611381 ValiotWorker-6.0.0/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-6.0.0/README.md
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.607956 ValiotWorker-6.0.0/ValiotWorker/
+-rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-04-19 23:58:36.000000 ValiotWorker-6.0.0/ValiotWorker/Logging.py
+-rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-6.0.0/ValiotWorker/Notifications.py
+-rw-r--r--   0 baruc      (501) staff       (20)      294 2023-06-15 04:30:39.000000 ValiotWorker-6.0.0/ValiotWorker/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-06-29 18:09:35.000000 ValiotWorker-6.0.0/ValiotWorker/__main__.py
+-rw-r--r--   0 baruc      (501) staff       (20)       22 2023-06-29 22:42:29.000000 ValiotWorker-6.0.0/ValiotWorker/__version__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-6.0.0/ValiotWorker/croniterHelpers.py
+-rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-6.0.0/ValiotWorker/dateHelpers.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.609938 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/
+-rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/__main__.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.610646 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/modules/
+-rw-r--r--   0 baruc      (501) staff       (20)        0 2023-06-16 19:03:59.000000 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/modules/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/modules/http_server.py
+-rw-r--r--   0 baruc      (501) staff       (20)     7019 2023-06-15 04:30:39.000000 ValiotWorker-6.0.0/ValiotWorker/mutations.py
+-rw-r--r--   0 baruc      (501) staff       (20)     4393 2023-06-29 22:42:29.000000 ValiotWorker-6.0.0/ValiotWorker/queries.py
+-rw-r--r--   0 baruc      (501) staff       (20)     5885 2023-06-15 04:30:39.000000 ValiotWorker-6.0.0/ValiotWorker/redis.py
+-rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-06-15 04:30:39.000000 ValiotWorker-6.0.0/ValiotWorker/subscriptions.py
+-rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-6.0.0/ValiotWorker/uploaders.py
+-rw-r--r--   0 baruc      (501) staff       (20)    70027 2023-06-29 22:42:29.000000 ValiotWorker-6.0.0/ValiotWorker/worker.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.609433 ValiotWorker-6.0.0/ValiotWorker.egg-info/
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)      841 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/SOURCES.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/dependency_links.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       60 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/entry_points.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/not-zip-safe
+-rw-r--r--   0 baruc      (501) staff       (20)      233 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/requires.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       13 2023-06-29 22:45:13.000000 ValiotWorker-6.0.0/ValiotWorker.egg-info/top_level.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       38 2023-06-29 22:45:13.611650 ValiotWorker-6.0.0/setup.cfg
+-rw-r--r--   0 baruc      (501) staff       (20)     2607 2023-06-16 19:03:59.000000 ValiotWorker-6.0.0/setup.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-29 22:45:13.611007 ValiotWorker-6.0.0/tests/
+-rw-r--r--   0 baruc      (501) staff       (20)      106 2023-06-29 18:09:35.000000 ValiotWorker-6.0.0/tests/test_dummy.py
```

### Comparing `ValiotWorker-5.3.5/LICENCE` & `ValiotWorker-6.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/PKG-INFO` & `ValiotWorker-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 5.3.5
+Version: 6.0.0
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-5.3.5/README.md` & `ValiotWorker-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/Logging.py` & `ValiotWorker-6.0.0/ValiotWorker/Logging.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/Notifications.py` & `ValiotWorker-6.0.0/ValiotWorker/Notifications.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/__main__.py` & `ValiotWorker-6.0.0/ValiotWorker/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/__main__.py` & `ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/modules/http_server.py` & `ValiotWorker-6.0.0/ValiotWorker/healthCheckProbe/modules/http_server.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/mutations.py` & `ValiotWorker-6.0.0/ValiotWorker/mutations.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/queries.py` & `ValiotWorker-6.0.0/ValiotWorker/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   }
 }
 '''
 
 paginate_stale_jobs = '''
   query WorkerWaitingJobsPaginate(
     $worker: String!
-    $cursor: Int = 0
+    $cursor: String
     $limit: Int = 10
   ){
     jobsPaginate(
       cursor: $cursor
       filter: {
         workerCode: $worker
         jobStatus: WAITING
```

### Comparing `ValiotWorker-5.3.5/ValiotWorker/redis.py` & `ValiotWorker-6.0.0/ValiotWorker/redis.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/subscriptions.py` & `ValiotWorker-6.0.0/ValiotWorker/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/ValiotWorker/worker.py` & `ValiotWorker-6.0.0/ValiotWorker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -843,39 +843,44 @@
 
     def abortStaleJobs(self):
         """This function aborts all stale jobs.
         """
         # * pagination configuration
         workerRegex = f'^{self.worker["code"]}$'  # worker exact match
         limit = 100  # how many jobs to delete in one batch
-        cursor = 0  # starting point for each page
+        cursor = None  # starting point for each page
         hasNextPage = True
         abortedCount = 0
         pages = 0
         while hasNextPage:
             # * Get staled jobs page
             data, errors = self.gql.query(
                 queries.paginate_stale_jobs,
                 variables={'worker': workerRegex,
                            'cursor': cursor, 'limit': limit}
             )
+            if errors:
+                self.log(LogLevel.ERROR, 'Errors deleting stale jobs:')
+                self.log(LogLevel.ERROR, str(errors))
+                break
             jobs = __.get(data, 'jobs', [])
             cursor = __.get(data, 'pageInfo.endCursor')
             hasNextPage = __.get(data, 'pageInfo.hasNextPage')
             # ! delete 'em jobs
             # * get batch mutation
             BATCH_STALE_DELETE_MUT = mutations.build_batch_stale_mutation(jobs)
             if not BATCH_STALE_DELETE_MUT:
                 continue
             # * run mutation
             self.log(LogLevel.WARNING, f'Deleting {len(jobs)} stale jobs...')
             data, errors = self.gql.mutate(BATCH_STALE_DELETE_MUT)
             if errors:
                 self.log(LogLevel.ERROR, 'Errors deleting stale jobs:')
-                self.log(LogLevel.ERROR, errors)
+                self.log(LogLevel.ERROR, str(errors))
+                break
             self.log(LogLevel.ERROR, f'Deleted {len(jobs)} stale jobs')
             abortedCount += len(jobs)
             pages += 1
         if abortedCount and pages >= 2:
             self.log(LogLevel.ERROR,
                      f'Deleted a total of {abortedCount} stale jobs')
         elif not abortedCount:
```

### Comparing `ValiotWorker-5.3.5/ValiotWorker.egg-info/PKG-INFO` & `ValiotWorker-6.0.0/ValiotWorker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 5.3.5
+Version: 6.0.0
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-5.3.5/ValiotWorker.egg-info/SOURCES.txt` & `ValiotWorker-6.0.0/ValiotWorker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.5/setup.py` & `ValiotWorker-6.0.0/setup.py`

 * *Files identical despite different names*

