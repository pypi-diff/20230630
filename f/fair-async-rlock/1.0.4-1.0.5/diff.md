# Comparing `tmp/fair_async_rlock-1.0.4.tar.gz` & `tmp/fair_async_rlock-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_async_rlock-1.0.4.tar", last modified: Thu Jun 29 11:55:48 2023, max compression
+gzip compressed data, was "fair_async_rlock-1.0.5.tar", last modified: Fri Jun 30 09:30:25 2023, max compression
```

## Comparing `fair_async_rlock-1.0.4.tar` & `fair_async_rlock-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.4/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     4457 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.4/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-29 11:55:48.186770 fair_async_rlock-1.0.4/fair_async_rlock/
--rw-rw-r--   0 albert    (1000) albert    (1000)       48 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.4/fair_async_rlock/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2364 2023-06-29 11:49:51.000000 fair_async_rlock-1.0.4/fair_async_rlock/fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/fair_async_rlock/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.4/fair_async_rlock/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    17446 2023-06-29 11:43:58.000000 fair_async_rlock-1.0.4/fair_async_rlock/tests/test_fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-29 11:55:48.000000 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-29 11:55:48.000000 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-29 11:55:48.000000 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-29 11:55:48.000000 fair_async_rlock-1.0.4/fair_async_rlock.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.4/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-29 11:55:48.190770 fair_async_rlock-1.0.4/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-29 11:50:29.000000 fair_async_rlock-1.0.4/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 09:30:25.965637 fair_async_rlock-1.0.5/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.5/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-30 09:30:25.965637 fair_async_rlock-1.0.5/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4457 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.5/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 09:30:25.965637 fair_async_rlock-1.0.5/fair_async_rlock/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       48 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.5/fair_async_rlock/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2364 2023-06-29 11:56:29.000000 fair_async_rlock-1.0.5/fair_async_rlock/fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 09:30:25.965637 fair_async_rlock-1.0.5/fair_async_rlock/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.5/fair_async_rlock/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17584 2023-06-30 09:29:44.000000 fair_async_rlock-1.0.5/fair_async_rlock/tests/test_fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 09:30:25.965637 fair_async_rlock-1.0.5/fair_async_rlock.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-30 09:30:25.000000 fair_async_rlock-1.0.5/fair_async_rlock.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-30 09:30:25.000000 fair_async_rlock-1.0.5/fair_async_rlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-30 09:30:25.000000 fair_async_rlock-1.0.5/fair_async_rlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-30 09:30:25.000000 fair_async_rlock-1.0.5/fair_async_rlock.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.5/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-30 09:30:25.965637 fair_async_rlock-1.0.5/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-30 09:27:40.000000 fair_async_rlock-1.0.5/setup.py
```

### Comparing `fair_async_rlock-1.0.4/LICENSE` & `fair_async_rlock-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.4/PKG-INFO` & `fair_async_rlock-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_async_rlock
-Version: 1.0.4
+Version: 1.0.5
 Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
 Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fair_async_rlock-1.0.4/README.md` & `fair_async_rlock-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.4/fair_async_rlock/fair_async_rlock.py` & `fair_async_rlock-1.0.5/fair_async_rlock/fair_async_rlock.py`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.4/fair_async_rlock/tests/test_fair_async_rlock.py` & `fair_async_rlock-1.0.5/fair_async_rlock/tests/test_fair_async_rlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,15 +448,15 @@
 
     assert lock._owner is None  # lock should not be owned by any task
 
 
 @pytest.mark.asyncio
 async def test_stochastic_cancellation():
     lock = FairAsyncRLock()
-    num_tasks = 10  # number of tasks to create
+    num_tasks = 100  # number of tasks to create
     tasks = []
     cancellation_occurred = asyncio.Event()
 
     async def task_func(task_id):
         """Function to be run in tasks. Tries to acquire and release the lock."""
         try:
             await asyncio.sleep(random.random())  # simulate work with random duration
@@ -466,16 +466,21 @@
         except asyncio.CancelledError:
             print(f"Task {task_id} was cancelled")
             cancellation_occurred.set()
 
     async def monitor_func():
         """Function to be run in monitor task. Randomly cancels one of the tasks."""
         await asyncio.sleep(random.random())  # wait random duration before cancelling a task
-        task_to_cancel = random.choice(tasks)
-        task_to_cancel.cancel()
+        order = list(range(len(tasks)))
+        random.shuffle(order)
+        for i in order:
+            task_to_cancel = tasks[i]
+            if not task_to_cancel.done():
+                task_to_cancel.cancel()
+
 
     # Create tasks
     for i in range(num_tasks):
         tasks.append(asyncio.create_task(task_func(i)))
 
     await asyncio.sleep(0)
     # Create monitor task
```

### Comparing `fair_async_rlock-1.0.4/fair_async_rlock.egg-info/PKG-INFO` & `fair_async_rlock-1.0.5/fair_async_rlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-async-rlock
-Version: 1.0.4
+Version: 1.0.5
 Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
 Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fair_async_rlock-1.0.4/setup.py` & `fair_async_rlock-1.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='fair_async_rlock',
-      version='1.0.4',
+      version='1.0.5',
       description='A well-tested implementation of a fair asynchronous RLock for concurrent programming.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/Joshuaalbert/FairAsyncRLock",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=[],
```

