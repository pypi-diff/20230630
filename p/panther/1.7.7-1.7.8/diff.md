# Comparing `tmp/panther-1.7.7.tar.gz` & `tmp/panther-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-1.7.7.tar", last modified: Thu Jun 29 14:20:19 2023, max compression
+gzip compressed data, was "panther-1.7.8.tar", last modified: Fri Jun 30 10:50:52 2023, max compression
```

## Comparing `panther-1.7.7.tar` & `panther-1.7.8.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.780356 panther-1.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-29 14:19:56.000000 panther-1.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-29 14:20:19.780356 panther-1.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-29 14:19:56.000000 panther-1.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.772356 panther-1.7.7/panther/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 14:19:56.000000 panther-1.7.7/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-29 14:19:56.000000 panther-1.7.7/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-29 14:19:56.000000 panther-1.7.7/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-29 14:19:56.000000 panther-1.7.7/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-29 14:19:56.000000 panther-1.7.7/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.776356 panther-1.7.7/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-29 14:19:56.000000 panther-1.7.7/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.776356 panther-1.7.7/panther/db/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.776356 panther-1.7.7/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-29 14:19:56.000000 panther-1.7.7/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-29 14:19:56.000000 panther-1.7.7/panther/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-06-29 14:19:56.000000 panther-1.7.7/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.780356 panther-1.7.7/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.780356 panther-1.7.7/panther/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-29 14:19:56.000000 panther-1.7.7/panther/panel/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 14:19:56.000000 panther-1.7.7/panther/panel/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 14:19:56.000000 panther-1.7.7/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-29 14:19:56.000000 panther-1.7.7/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-29 14:19:56.000000 panther-1.7.7/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-29 14:19:56.000000 panther-1.7.7/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-29 14:19:56.000000 panther-1.7.7/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-29 14:19:56.000000 panther-1.7.7/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-29 14:19:56.000000 panther-1.7.7/panther/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.776356 panther-1.7.7/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-29 14:19:56.000000 panther-1.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:20:19.780356 panther-1.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-29 14:19:56.000000 panther-1.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.585147 panther-1.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-30 10:50:35.000000 panther-1.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-30 10:50:52.585147 panther-1.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-30 10:50:35.000000 panther-1.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 10:50:35.000000 panther-1.7.8/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-30 10:50:35.000000 panther-1.7.8/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-30 10:50:35.000000 panther-1.7.8/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-30 10:50:35.000000 panther-1.7.8/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-30 10:50:35.000000 panther-1.7.8/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-30 10:50:35.000000 panther-1.7.8/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 10:50:35.000000 panther-1.7.8/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-30 10:50:35.000000 panther-1.7.8/panther/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-30 10:50:35.000000 panther-1.7.8/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.585147 panther-1.7.8/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.585147 panther-1.7.8/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:35.000000 panther-1.7.8/panther/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-30 10:50:35.000000 panther-1.7.8/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-30 10:50:35.000000 panther-1.7.8/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-30 10:50:35.000000 panther-1.7.8/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-30 10:50:35.000000 panther-1.7.8/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-30 10:50:35.000000 panther-1.7.8/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-30 10:50:35.000000 panther-1.7.8/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-30 10:50:35.000000 panther-1.7.8/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 10:50:35.000000 panther-1.7.8/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-30 10:50:35.000000 panther-1.7.8/panther/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-30 10:50:35.000000 panther-1.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:50:52.585147 panther-1.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-30 10:50:35.000000 panther-1.7.8/setup.py
```

### Comparing `panther-1.7.7/LICENSE` & `panther-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/PKG-INFO` & `panther-1.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.7
+Version: 1.7.8
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panther-1.7.7/README.md` & `panther-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/_utils.py` & `panther-1.7.8/panther/_utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/app.py` & `panther-1.7.8/panther/app.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/authentications.py` & `panther-1.7.8/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/caching.py` & `panther-1.7.8/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/cli/create_command.py` & `panther-1.7.8/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/cli/main.py` & `panther-1.7.8/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/cli/monitor_command.py` & `panther-1.7.8/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/cli/run_command.py` & `panther-1.7.8/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/cli/template.py` & `panther-1.7.8/panther/cli/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,18 @@
 env = load_env(BASE_DIR / '.env')
 
 DB_NAME = env['DB_NAME']
 SECRET_KEY = env['SECRET_KEY']
 
 # # # More Info: Https://PantherPy.GitHub.io/middlewares/
 MIDDLEWARES = [
-    ('panther.middlewares.db.Middleware', {'url': f'pantherdb://{BASE_DIR}/{DB_NAME}.pantherdb'}),
+    ('panther.middlewares.db.Middleware', {'url': f'pantherdb://{BASE_DIR}/{DB_NAME}.pdb'}),
 ]
 
-# More Info: https://pantherpy.github.io/configs/#user_model
+# More Info: https://PantherPy.GitHub.io/configs/#user_model
 USER_MODEL = 'panther.db.models.BaseUser'
 
 # More Info: https://PantherPy.GitHub.io/authentications/
 AUTHENTICATION = 'panther.authentications.JWTAuthentication'
 
 # More Info: https://PantherPy.GitHub.io/monitoring/
 MONITORING = True
@@ -111,15 +111,15 @@
 
 git_ignore = """__pycache__/
 .venv/
 .idea/
 logs/
 
 .env
-*.pantherdb
+*.pdb
 """
 
 requirements = """panther==%s
 """ % version()
 
 Template = {
     'app': {
```

### Comparing `panther-1.7.7/panther/cli/utils.py` & `panther-1.7.8/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/configs.py` & `panther-1.7.8/panther/configs.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/db/connection.py` & `panther-1.7.8/panther/db/connection.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/db/models.py` & `panther-1.7.8/panther/db/models.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/db/queries/mongodb_queries.py` & `panther-1.7.8/panther/db/queries/mongodb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/db/queries/pantherdb_queries.py` & `panther-1.7.8/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/db/queries/queries.py` & `panther-1.7.8/panther/db/queries/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Self
+from typing import Self, NoReturn
 
 from pydantic import ValidationError
 
 from panther.configs import config
 from panther.db.utils import log_query
 from panther.db.queries.mongodb_queries import BaseMongoDBQuery
 from panther.db.queries.pantherdb_queries import BasePantherDBQuery
@@ -17,15 +17,15 @@
     'Query',
 )
 
 
 class Query(BaseQuery):
 
     @classmethod
-    def validate_data(cls, data: dict, is_updating: bool = False) -> Self | None:
+    def validate_data(cls, data: dict, is_updating: bool = False) -> NoReturn:
         """
         *. Validate the input of user with its class
         *. If is_updating is True & exception happens but the message was empty
         """
         try:
             cls(**data)
         except ValidationError as validation_error:
```

### Comparing `panther-1.7.7/panther/db/utils.py` & `panther-1.7.8/panther/db/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/exceptions.py` & `panther-1.7.8/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/logger.py` & `panther-1.7.8/panther/logger.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/main.py` & `panther-1.7.8/panther/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,25 +127,27 @@
                         for n in node.body:
                             # Find classes in each element of files' body
                             if type(n) is ast.ClassDef and n.bases:
                                 class_path = file_path\
                                     .removesuffix('/models.py')\
                                     .removeprefix(f'{config["base_dir"]}/')\
                                     .replace('/', '.')
-                                # Import the class to check his father and brother
-                                klass = import_class(f'{class_path}.models.{n.name}')
-                                for parent in klass.__mro__:
-                                    if parent is Model:
-                                        # The class was one our database models so collect it
-                                        config['models'].append({
-                                            'name': n.name,
-                                            'path':  file_path,
-                                            'class': klass,
-                                            'app': class_path.split('.'),
-                                        })
+                                # We don't need to import the package classes
+                                if class_path.find('site-packages') == -1:
+                                    # Import the class to check his father and brother
+                                    klass = import_class(f'{class_path}.models.{n.name}')
+                                    for parent in klass.__mro__:
+                                        if parent is Model:
+                                            # The class was one our database models so collect it
+                                            config['models'].append({
+                                                'name': n.name,
+                                                'path':  file_path,
+                                                'class': klass,
+                                                'app': class_path.split('.'),
+                                            })
 
     async def __call__(self, scope, receive, send) -> None:
         """
         We Used Python3.11 For asyncio.TaskGroup()
         1.
             async with asyncio.TaskGroup() as tg:
                 tg.create_task(self.run(scope, receive, send))
```

### Comparing `panther-1.7.7/panther/middlewares/monitoring.py` & `panther-1.7.8/panther/middlewares/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/middlewares/redis.py` & `panther-1.7.8/panther/middlewares/redis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/panel/apis.py` & `panther-1.7.8/panther/panel/apis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/request.py` & `panther-1.7.8/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/response.py` & `panther-1.7.8/panther/response.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/routings.py` & `panther-1.7.8/panther/routings.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,8 +132,8 @@
 def finalize_urls(urls: dict) -> dict:
     urls_list = list()
     for url, endpoint in urls.items():
         path = dict()
         for single_path in url.split('/')[:-1][::-1]:
             path = {single_path: path or endpoint}
         urls_list.append(path)
-    return merge(*urls_list)
+    return merge(*urls_list) if urls_list else {}
```

### Comparing `panther-1.7.7/panther/status.py` & `panther-1.7.8/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.7/panther/utils.py` & `panther-1.7.8/panther/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     if env_file is None or not os.path.isfile(env_file):
         logger.critical(f'"{env_file}" is not valid file for load_env()')
         return variables
 
     with open(env_file) as file:
         for line in file.readlines():
             line = line.strip()
-            if '=' in line and not line.startswith('#'):
+            if not line.startswith('#') and '=' in line:
                 key, value = line.split('=', 1)
                 key = key.strip()
                 value = value.strip().strip('"\'')
                 variables[key] = value
     return variables
```

### Comparing `panther-1.7.7/panther.egg-info/PKG-INFO` & `panther-1.7.8/panther.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.7
+Version: 1.7.8
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panther-1.7.7/panther.egg-info/SOURCES.txt` & `panther-1.7.8/panther.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -40,9 +40,10 @@
 panther/db/queries/pantherdb_queries.py
 panther/db/queries/queries.py
 panther/middlewares/__init__.py
 panther/middlewares/base.py
 panther/middlewares/db.py
 panther/middlewares/monitoring.py
 panther/middlewares/redis.py
+panther/panel/__init__.py
 panther/panel/apis.py
 panther/panel/urls.py
```

### Comparing `panther-1.7.7/setup.py` & `panther-1.7.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     package_data={
         'panther': ['cli/*'],
     },
     install_requires=[
         'bpython>=0.24',
         'bson>=0.5.10',
         'httptools>=0.5.0',
-        'pantherdb>=1.2.2',
+        'pantherdb>=1.2.3',
         'pydantic>=1.10.7',
         'redis>=4.5.3',
         'rich>=13.3.2',
         'uvicorn>=0.21.1',
         'uvloop>=0.17.0',
         'watchfiles>=0.18.1',
         'python-jose==3.3.0',
```

