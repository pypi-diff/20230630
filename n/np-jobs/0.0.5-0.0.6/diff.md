# Comparing `tmp/np_jobs-0.0.5.tar.gz` & `tmp/np_jobs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_jobs-0.0.5.tar", last modified: Fri Jun 30 06:08:50 2023, max compression
+gzip compressed data, was "np_jobs-0.0.6.tar", last modified: Fri Jun 30 06:20:18 2023, max compression
```

## Comparing `np_jobs-0.0.5.tar` & `np_jobs-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      110 2023-05-10 01:20:18.221900 np_jobs-0.0.5/README.md
--rw-r--r--   0        0        0     2358 2023-06-30 06:08:50.209942 np_jobs-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      243 2023-05-10 05:18:07.654589 np_jobs-0.0.5/src/np_jobs/__init__.py
--rw-r--r--   0        0        0       75 2023-05-10 01:25:17.321180 np_jobs-0.0.5/src/np_jobs/jobs/__init__.py
--rw-r--r--   0        0        0     1112 2023-05-10 01:37:07.453140 np_jobs-0.0.5/src/np_jobs/jobs/base.py
--rw-r--r--   0        0        0      150 2023-05-10 01:25:17.320182 np_jobs-0.0.5/src/np_jobs/jobs/pipeline_sorting.py
--rw-r--r--   0        0        0       42 2023-05-10 00:44:55.816888 np_jobs-0.0.5/src/np_jobs/queues/__init__.py
--rw-r--r--   0        0        0      443 2023-05-10 06:12:46.620875 np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/__init__.py
--rw-r--r--   0        0        0    11562 2023-06-30 06:08:26.659686 np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/base.py
--rw-r--r--   0        0        0      161 2023-05-10 01:06:56.845630 np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/codeocean_upload_queue.py
--rw-r--r--   0        0        0      161 2023-05-10 01:06:39.090798 np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/datajoint_upload_queue.py
--rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      161 2023-05-10 00:57:38.731220 np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/pipeline_npexp_upload_queue.py
--rw-r--r--   0        0        0      142 2023-05-10 00:57:35.004534 np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/pipeline_qc_queue.py
--rw-r--r--   0        0        0      348 2023-05-10 00:54:41.870192 np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/pipeline_sorting_queue.py
--rw-r--r--   0        0        0     4938 2023-05-10 01:08:07.498322 np_jobs-0.0.5/src/np_jobs/types.py
--rw-r--r--   0        0        0     2772 2023-05-11 23:27:56.478961 np_jobs-0.0.5/src/np_jobs/utils.py
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 np_jobs-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-05-10 01:20:18.221900 np_jobs-0.0.6/README.md
+-rw-r--r--   0        0        0     2358 2023-06-30 06:20:18.175863 np_jobs-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-05-10 05:18:07.654589 np_jobs-0.0.6/src/np_jobs/__init__.py
+-rw-r--r--   0        0        0       75 2023-05-10 01:25:17.321180 np_jobs-0.0.6/src/np_jobs/jobs/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-10 01:37:07.453140 np_jobs-0.0.6/src/np_jobs/jobs/base.py
+-rw-r--r--   0        0        0      150 2023-05-10 01:25:17.320182 np_jobs-0.0.6/src/np_jobs/jobs/pipeline_sorting.py
+-rw-r--r--   0        0        0       42 2023-05-10 00:44:55.816888 np_jobs-0.0.6/src/np_jobs/queues/__init__.py
+-rw-r--r--   0        0        0      443 2023-05-10 06:12:46.620875 np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/__init__.py
+-rw-r--r--   0        0        0    11544 2023-06-30 06:18:45.923277 np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/base.py
+-rw-r--r--   0        0        0      161 2023-05-10 01:06:56.845630 np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/codeocean_upload_queue.py
+-rw-r--r--   0        0        0      161 2023-05-10 01:06:39.090798 np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/datajoint_upload_queue.py
+-rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      161 2023-05-10 00:57:38.731220 np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/pipeline_npexp_upload_queue.py
+-rw-r--r--   0        0        0      142 2023-05-10 00:57:35.004534 np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/pipeline_qc_queue.py
+-rw-r--r--   0        0        0      348 2023-05-10 00:54:41.870192 np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/pipeline_sorting_queue.py
+-rw-r--r--   0        0        0     4938 2023-05-10 01:08:07.498322 np_jobs-0.0.6/src/np_jobs/types.py
+-rw-r--r--   0        0        0     2772 2023-05-11 23:27:56.478961 np_jobs-0.0.6/src/np_jobs/utils.py
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 np_jobs-0.0.6/PKG-INFO
```

### Comparing `np_jobs-0.0.5/pyproject.toml` & `np_jobs-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_jobs"
-version = "0.0.5"
+version = "0.0.6"
 description = "Interfaces for job queues used to coordinate distributed tasks for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np-config>=0.4.17",
     "np-logging>=0.5.1",
```

### Comparing `np_jobs-0.0.5/src/np_jobs/jobs/base.py` & `np_jobs-0.0.6/src/np_jobs/jobs/base.py`

 * *Files identical despite different names*

### Comparing `np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/base.py` & `np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         self.update(session_or_job, started=None, hostname=None, finished=None, errored=None)
     
     def set_errored(self, session_or_job: SessionArgs | Job, error: str | Exception) -> None:
         self.update(session_or_job, error=str(error))
     
     def is_started(self, session_or_job: SessionArgs | Job) -> bool:
         """Whether the job has started processing, but not yet finished."""
-        job = get_job(session_or_job, self.job_type)
+        job = self[session_or_job]
         return (
             bool(job.started)
             and not job.finished
             and not job.error
         )
```

### Comparing `np_jobs-0.0.5/src/np_jobs/queues/sqlite_isilon/dynamicrouting_behavior_session_mtrain_upload.py` & `np_jobs-0.0.6/src/np_jobs/queues/sqlite_isilon/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_jobs-0.0.5/src/np_jobs/types.py` & `np_jobs-0.0.6/src/np_jobs/types.py`

 * *Files identical despite different names*

### Comparing `np_jobs-0.0.5/src/np_jobs/utils.py` & `np_jobs-0.0.6/src/np_jobs/utils.py`

 * *Files identical despite different names*

### Comparing `np_jobs-0.0.5/PKG-INFO` & `np_jobs-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np_jobs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Interfaces for job queues used to coordinate distributed tasks for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

