# Comparing `tmp/squarelet_auth-0.1.2.tar.gz` & `tmp/squarelet_auth-0.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squarelet_auth-0.1.2.tar", last modified: Fri Jun 30 17:24:47 2023, max compression
+gzip compressed data, was "squarelet_auth-0.1.2.dev0.tar", last modified: Fri Jun 30 14:42:53 2023, max compression
```

## Comparing `squarelet_auth-0.1.2.tar` & `squarelet_auth-0.1.2.dev0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 17:24:47.295717 squarelet_auth-0.1.2/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1464 2020-04-21 18:13:31.000000 squarelet_auth-0.1.2/LICENSE
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      606 2023-06-30 17:24:47.295717 squarelet_auth-0.1.2/PKG-INFO
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      102 2020-04-21 18:11:12.000000 squarelet_auth-0.1.2/README.md
--rw-rw-r--   0 mitch     (1000) mitch     (1000)       38 2023-06-30 17:24:47.295717 squarelet_auth-0.1.2/setup.cfg
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      860 2023-06-30 17:24:36.000000 squarelet_auth-0.1.2/setup.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 17:24:47.287717 squarelet_auth-0.1.2/squarelet_auth/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)        0 2020-04-21 12:41:38.000000 squarelet_auth-0.1.2/squarelet_auth/__init__.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      439 2020-05-27 21:10:29.000000 squarelet_auth-0.1.2/squarelet_auth/apps.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      629 2020-04-21 12:49:39.000000 squarelet_auth-0.1.2/squarelet_auth/backends.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      874 2020-04-21 14:01:16.000000 squarelet_auth-0.1.2/squarelet_auth/fields.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 17:24:47.291717 squarelet_auth-0.1.2/squarelet_auth/migrations/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)        0 2020-04-21 12:41:38.000000 squarelet_auth-0.1.2/squarelet_auth/migrations/__init__.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1740 2020-04-21 17:59:27.000000 squarelet_auth-0.1.2/squarelet_auth/mixins.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 17:24:47.291717 squarelet_auth-0.1.2/squarelet_auth/organizations/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      733 2020-04-22 20:50:14.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/__init__.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2338 2020-05-28 16:00:23.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/admin.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      261 2020-04-22 20:04:25.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/apps.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 17:24:47.291717 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2411 2020-04-23 14:07:31.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0001_initial.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2592 2020-04-23 14:08:54.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0002_auto_20200423_1008.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      471 2020-05-26 12:52:40.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0003_plan_resources.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1223 2020-05-27 13:20:21.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0004_auto_20200527_0920.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      863 2020-05-27 20:35:30.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0005_auto_20200527_0921.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      297 2020-05-28 12:33:05.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0006_auto_20200527_1646.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      314 2020-05-28 12:49:00.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0007_delete_plan.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      407 2023-06-30 14:12:56.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0008_alter_entitlement_resources.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)        0 2020-04-23 12:28:05.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/__init__.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     7288 2023-06-30 13:09:23.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/models.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      284 2020-04-25 15:47:22.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/urls.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1866 2020-05-28 13:43:46.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/utils.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1255 2020-04-25 15:47:23.000000 squarelet_auth-0.1.2/squarelet_auth/organizations/views.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1519 2022-04-01 19:28:59.000000 squarelet_auth-0.1.2/squarelet_auth/pipeline.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1271 2020-05-27 13:20:18.000000 squarelet_auth-0.1.2/squarelet_auth/settings.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1743 2020-05-29 11:50:01.000000 squarelet_auth-0.1.2/squarelet_auth/tasks.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      441 2020-04-25 12:39:08.000000 squarelet_auth-0.1.2/squarelet_auth/urls.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 17:24:47.291717 squarelet_auth-0.1.2/squarelet_auth/users/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)        0 2020-04-21 13:31:04.000000 squarelet_auth-0.1.2/squarelet_auth/users/__init__.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2134 2023-06-30 14:42:11.000000 squarelet_auth-0.1.2/squarelet_auth/users/admin.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     4856 2023-06-30 14:40:49.000000 squarelet_auth-0.1.2/squarelet_auth/users/models.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     4159 2023-01-24 18:03:05.000000 squarelet_auth-0.1.2/squarelet_auth/users/utils.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2177 2023-06-30 14:39:07.000000 squarelet_auth-0.1.2/squarelet_auth/utils.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2288 2020-04-25 13:54:38.000000 squarelet_auth-0.1.2/squarelet_auth/views.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 17:24:47.291717 squarelet_auth-0.1.2/squarelet_auth.egg-info/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      606 2023-06-30 17:24:47.000000 squarelet_auth-0.1.2/squarelet_auth.egg-info/PKG-INFO
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1496 2023-06-30 17:24:47.000000 squarelet_auth-0.1.2/squarelet_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)        1 2023-06-30 17:24:47.000000 squarelet_auth-0.1.2/squarelet_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)       55 2023-06-30 17:24:47.000000 squarelet_auth-0.1.2/squarelet_auth.egg-info/requires.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)       15 2023-06-30 17:24:47.000000 squarelet_auth-0.1.2/squarelet_auth.egg-info/top_level.txt
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 14:42:53.478689 squarelet_auth-0.1.2.dev0/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1464 2020-04-21 18:13:31.000000 squarelet_auth-0.1.2.dev0/LICENSE
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      611 2023-06-30 14:42:53.478689 squarelet_auth-0.1.2.dev0/PKG-INFO
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      102 2020-04-21 18:11:12.000000 squarelet_auth-0.1.2.dev0/README.md
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)       38 2023-06-30 14:42:53.478689 squarelet_auth-0.1.2.dev0/setup.cfg
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      864 2023-06-30 14:42:32.000000 squarelet_auth-0.1.2.dev0/setup.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 14:42:53.474689 squarelet_auth-0.1.2.dev0/squarelet_auth/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)        0 2020-04-21 12:41:38.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/__init__.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      439 2020-05-27 21:10:29.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/apps.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      629 2020-04-21 12:49:39.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/backends.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      874 2020-04-21 14:01:16.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/fields.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 14:42:53.474689 squarelet_auth-0.1.2.dev0/squarelet_auth/migrations/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)        0 2020-04-21 12:41:38.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/migrations/__init__.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1740 2020-04-21 17:59:27.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/mixins.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 14:42:53.478689 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      733 2020-04-22 20:50:14.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/__init__.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2338 2020-05-28 16:00:23.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/admin.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      261 2020-04-22 20:04:25.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/apps.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 14:42:53.478689 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2411 2020-04-23 14:07:31.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0001_initial.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2592 2020-04-23 14:08:54.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0002_auto_20200423_1008.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      471 2020-05-26 12:52:40.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0003_plan_resources.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1223 2020-05-27 13:20:21.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0004_auto_20200527_0920.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      863 2020-05-27 20:35:30.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0005_auto_20200527_0921.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      297 2020-05-28 12:33:05.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0006_auto_20200527_1646.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      314 2020-05-28 12:49:00.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0007_delete_plan.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      407 2023-06-30 14:12:56.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0008_alter_entitlement_resources.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)        0 2020-04-23 12:28:05.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/__init__.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     7288 2023-06-30 13:09:23.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/models.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      284 2020-04-25 15:47:22.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/urls.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1866 2020-05-28 13:43:46.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/utils.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1255 2020-04-25 15:47:23.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/views.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1519 2022-04-01 19:28:59.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/pipeline.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1271 2020-05-27 13:20:18.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/settings.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1743 2020-05-29 11:50:01.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/tasks.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      441 2020-04-25 12:39:08.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/urls.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 14:42:53.478689 squarelet_auth-0.1.2.dev0/squarelet_auth/users/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)        0 2020-04-21 13:31:04.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/users/__init__.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2134 2023-06-30 14:42:11.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/users/admin.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     4856 2023-06-30 14:40:49.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/users/models.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     4159 2023-01-24 18:03:05.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/users/utils.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2177 2023-06-30 14:39:07.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/utils.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2288 2020-04-25 13:54:38.000000 squarelet_auth-0.1.2.dev0/squarelet_auth/views.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-06-30 14:42:53.474689 squarelet_auth-0.1.2.dev0/squarelet_auth.egg-info/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      611 2023-06-30 14:42:53.000000 squarelet_auth-0.1.2.dev0/squarelet_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1496 2023-06-30 14:42:53.000000 squarelet_auth-0.1.2.dev0/squarelet_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)        1 2023-06-30 14:42:53.000000 squarelet_auth-0.1.2.dev0/squarelet_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)       55 2023-06-30 14:42:53.000000 squarelet_auth-0.1.2.dev0/squarelet_auth.egg-info/requires.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)       15 2023-06-30 14:42:53.000000 squarelet_auth-0.1.2.dev0/squarelet_auth.egg-info/top_level.txt
```

### Comparing `squarelet_auth-0.1.2/LICENSE` & `squarelet_auth-0.1.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/PKG-INFO` & `squarelet_auth-0.1.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squarelet_auth
-Version: 0.1.2
+Version: 0.1.2.dev0
 Summary: Django authentication against the MuckRock user service
 Home-page: https://github.com/muckrock/squarelet-auth/
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `squarelet_auth-0.1.2/setup.py` & `squarelet_auth-0.1.2.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="squarelet_auth",  # Replace with your own username
-    version="0.1.2",
+    version="0.1.2dev0",
     author="Mitchell Kotler",
     author_email="mitch@muckrock.com",
     description="Django authentication against the MuckRock user service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/muckrock/squarelet-auth/",
     packages=setuptools.find_packages(),
```

### Comparing `squarelet_auth-0.1.2/squarelet_auth/backends.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/backends.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/fields.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/fields.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/mixins.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/__init__.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/admin.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/admin.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0001_initial.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0002_auto_20200423_1008.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0002_auto_20200423_1008.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0004_auto_20200527_0920.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0004_auto_20200527_0920.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/migrations/0005_auto_20200527_0921.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/migrations/0005_auto_20200527_0921.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/models.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/models.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/utils.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/utils.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/organizations/views.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/organizations/views.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/pipeline.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/pipeline.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/settings.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/settings.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/tasks.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/tasks.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/users/admin.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/users/admin.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/users/models.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/users/models.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/users/utils.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/users/utils.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/utils.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/utils.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth/views.py` & `squarelet_auth-0.1.2.dev0/squarelet_auth/views.py`

 * *Files identical despite different names*

### Comparing `squarelet_auth-0.1.2/squarelet_auth.egg-info/PKG-INFO` & `squarelet_auth-0.1.2.dev0/squarelet_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squarelet-auth
-Version: 0.1.2
+Version: 0.1.2.dev0
 Summary: Django authentication against the MuckRock user service
 Home-page: https://github.com/muckrock/squarelet-auth/
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `squarelet_auth-0.1.2/squarelet_auth.egg-info/SOURCES.txt` & `squarelet_auth-0.1.2.dev0/squarelet_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

