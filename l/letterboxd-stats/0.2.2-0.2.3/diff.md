# Comparing `tmp/letterboxd_stats-0.2.2.tar.gz` & `tmp/letterboxd_stats-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.2.2.tar", last modified: Mon Jun 19 14:33:36 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.2.3.tar", last modified: Fri Jun 30 11:15:17 2023, max compression
```

## Comparing `letterboxd_stats-0.2.2.tar` & `letterboxd_stats-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.2/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.2/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1745 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.2/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5222 2023-06-13 14:00:37.000000 letterboxd_stats-0.2.2/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.2/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.2/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-05-08 18:03:39.000000 letterboxd_stats-0.2.2/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     6353 2023-06-19 14:31:28.000000 letterboxd_stats-0.2.2/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-06-19 14:33:09.000000 letterboxd_stats-0.2.2/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.3/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.3/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1745 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.3/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5331 2023-06-30 11:14:04.000000 letterboxd_stats-0.2.3/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-26 09:44:09.000000 letterboxd_stats-0.2.3/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.3/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-05-08 18:03:39.000000 letterboxd_stats-0.2.3/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     6353 2023-06-21 19:07:47.000000 letterboxd_stats-0.2.3/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-06-30 11:14:42.000000 letterboxd_stats-0.2.3/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/setup.cfg
```

### Comparing `letterboxd_stats-0.2.2/LICENCE` & `letterboxd_stats-0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.2/PKG-INFO` & `letterboxd_stats-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd_stats
-Version: 0.2.2
+Version: 0.2.3
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.2/README.md` & `letterboxd_stats-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.2/letterboxd_stats/__init__.py` & `letterboxd_stats-0.2.3/letterboxd_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.2/letterboxd_stats/cli.py` & `letterboxd_stats-0.2.3/letterboxd_stats/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,15 +123,18 @@
         validate=lambda n: (2 * float(n)).is_integer(),
         invalid_message="Wrong value. Either an integer or a .5 float",
         replace_mode=True,
         filter=lambda n: int(2 * float(n)),
     ).execute()
     liked = inquirer.confirm(message="Did you like the movie?").execute()  # type: ignore
     review = inquirer.text(  # type: ignore
-        message="Write a review. Press Enter for multiline.", multiline=True
+        message="Write a review. "
+        + "Use HTML tags for formatting (<b>, <i>, <a href='[URL]'>, <blockquote<>). "
+        + "Press Enter for multiline.",
+        multiline=True,
     ).execute()
     contains_spoilers = False
     if len(review) > 0:
         contains_spoilers = inquirer.confirm(message="The review contains spoilers?").execute()  # type: ignore
     rewatch = inquirer.confirm(message="Have you seen this film before?").execute()  # type: ignore
     payload = {
         "specifiedDate": specify_date,
```

### Comparing `letterboxd_stats-0.2.2/letterboxd_stats/data.py` & `letterboxd_stats-0.2.3/letterboxd_stats/data.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.2/letterboxd_stats/main.py` & `letterboxd_stats-0.2.3/letterboxd_stats/main.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.2/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.2.3/letterboxd_stats/tmdb.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.2/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.2.3/letterboxd_stats/web_scraper.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.2/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.2.3/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd-stats
-Version: 0.2.2
+Version: 0.2.3
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.2/pyproject.toml` & `letterboxd_stats-0.2.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.2.2"
+version = "0.2.3"
 authors = [{ name = "mBaratta96" }]
 description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
```

