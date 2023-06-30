# Comparing `tmp/letterboxd_stats-0.2.3.tar.gz` & `tmp/letterboxd_stats-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.2.3.tar", last modified: Fri Jun 30 11:15:17 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.2.4.tar", last modified: Fri Jun 30 20:18:09 2023, max compression
```

## Comparing `letterboxd_stats-0.2.3.tar` & `letterboxd_stats-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.3/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.3/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1745 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.3/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5331 2023-06-30 11:14:04.000000 letterboxd_stats-0.2.3/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-26 09:44:09.000000 letterboxd_stats-0.2.3/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.3/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-05-08 18:03:39.000000 letterboxd_stats-0.2.3/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     6353 2023-06-21 19:07:47.000000 letterboxd_stats-0.2.3/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-06-30 11:15:17.000000 letterboxd_stats-0.2.3/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-06-30 11:14:42.000000 letterboxd_stats-0.2.3/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-06-30 11:15:17.434806 letterboxd_stats-0.2.3/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.4/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.4/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1472 2023-06-30 20:01:47.000000 letterboxd_stats-0.2.4/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5331 2023-06-30 11:32:08.000000 letterboxd_stats-0.2.4/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-26 09:44:09.000000 letterboxd_stats-0.2.4/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.4/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-06-30 15:36:50.000000 letterboxd_stats-0.2.4/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     6306 2023-06-30 20:08:17.000000 letterboxd_stats-0.2.4/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      142 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      886 2023-06-30 20:14:27.000000 letterboxd_stats-0.2.4/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/setup.cfg
```

### Comparing `letterboxd_stats-0.2.3/LICENCE` & `letterboxd_stats-0.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.3/PKG-INFO` & `letterboxd_stats-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd_stats
-Version: 0.2.3
+Version: 0.2.4
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.3/README.md` & `letterboxd_stats-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.3/letterboxd_stats/__init__.py` & `letterboxd_stats-0.2.4/letterboxd_stats/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,13 +32,7 @@
 if not os.path.exists(path):
     raise FileNotFoundError(
         f"Found no configuration file in {path}. "
         + "Please, add a config.toml in that folder or specify a custom one with the -c command."
     )
 with open(path, "rb") as f:
     config = tomli.load(f)
-
-cache_path = os.path.expanduser(os.path.join(config["root_folder"], "static", "cache.csv"))
-if not os.path.exists(cache_path):
-    with open(cache_path, "w") as csvfile:
-        writer = csv.writer(csvfile, delimiter=",")
-        writer.writerow(["Letterboxd URI", "Id"])
```

### Comparing `letterboxd_stats-0.2.3/letterboxd_stats/cli.py` & `letterboxd_stats-0.2.4/letterboxd_stats/cli.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.3/letterboxd_stats/data.py` & `letterboxd_stats-0.2.4/letterboxd_stats/data.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.3/letterboxd_stats/main.py` & `letterboxd_stats-0.2.4/letterboxd_stats/main.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.3/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.2.4/letterboxd_stats/tmdb.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.3/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.2.4/letterboxd_stats/web_scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from zipfile import ZipFile
 from letterboxd_stats import config
 from letterboxd_stats import cli
 import requests
 from lxml import html
-import pandas as pd
+import pickledb
 
 URL = "https://letterboxd.com"
 LOGIN_PAGE = URL + "/user/login.do"
 DATA_PAGE = URL + "/data/export"
 ADD_DIARY_URL = URL + "/s/save-diary-entry"
 MOVIE_OPERATIONS = {
     "Add to diary": "add_film_diary",
@@ -19,16 +19,16 @@
     "search": lambda s: f"/search/films/{s}/?adult",
     "diary": lambda s: f"/csi/film/{s}/sidebar-user-actions/?esiAllowUser=true",
     "add_watchlist": lambda s: f"/film/{s}/add-to-watchlist/",
     "remove_watchlist": lambda s: f"/film/{s}/remove-from-watchlist/",
     "film_page": lambda s: f"/film/{s}",
 }
 
-cache_path = os.path.expanduser(os.path.join(config["root_folder"], "static", "cache.csv"))
-tmdb_id_df = pd.read_csv(cache_path, header=0, index_col=0)
+cache_path = os.path.expanduser(os.path.join(config["root_folder"], "static", "cache.db"))
+tmdb_id_cache = pickledb.load(cache_path, auto_dump=True)
 
 
 class Downloader:
     def __init__(self):
         self.session = requests.Session()
         self.session.get(URL)
 
@@ -92,31 +92,30 @@
 
 
 def create_movie_url(title: str, operation: str):
     return URL + OPERATIONS_URLS[operation](title)
 
 
 def get_tmdb_id(link: str, is_diary: bool):
-    if link in tmdb_id_df.index:
-        return int(tmdb_id_df.loc[link]["Id"])
+    if tmdb_id_cache.exists(link):
+        return tmdb_id_cache.get(link)
     res = requests.get(link)
     movie_page = html.fromstring(res.text)
     if is_diary:
         title_link = movie_page.xpath("//span[@class='film-title-wrapper']/a")
         if len(title_link) == 0:
             return None
         movie_link = title_link[0]
         movie_url = URL + movie_link.get("href")
         movie_page = html.fromstring(requests.get(movie_url).text)
     tmdb_link = movie_page.xpath("//a[@data-track-action='TMDb']")
     if len(tmdb_link) == 0:
         return None
     id = tmdb_link[0].get("href").split("/")[-2]
-    tmdb_id_df.loc[link] = [id]
-    tmdb_id_df.to_csv(cache_path)
+    tmdb_id_cache.set(link, id)
     return int(id)
 
 
 def select_optional_operation():
     return cli.select_value(["Exit"] + list(MOVIE_OPERATIONS.keys()), "Select operation:")
```

### Comparing `letterboxd_stats-0.2.3/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.2.4/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd-stats
-Version: 0.2.3
+Version: 0.2.4
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.3/pyproject.toml` & `letterboxd_stats-0.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.2.3"
+version = "0.2.4"
 authors = [{ name = "mBaratta96" }]
 description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -16,14 +16,15 @@
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "ascii_magic~=2.3.0",
   "inquirerpy~=0.3.4",
   "lxml~=4.9.0",
   "pandas~=1.5.1",
+  "pickleDB~=0.9.2",
   "platformdirs~=3.0.0",
   "rich~=13.3.5",
   "tmdbv3api~=1.7.7",
   "tomli~=2.0.1",
 ]
 
 [project.urls]
```

