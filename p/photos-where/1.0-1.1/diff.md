# Comparing `tmp/photos-where-1.0.tar.gz` & `tmp/photos-where-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photos-where-1.0.tar", last modified: Fri Jun 30 19:00:17 2023, max compression
+gzip compressed data, was "photos-where-1.1.tar", last modified: Fri Jun 30 19:03:03 2023, max compression
```

## Comparing `photos-where-1.0.tar` & `photos-where-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:00:17.436272 photos-where-1.0/
--rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos-where-1.0/LICENSE
--rw-r--r--   0 visgean    (501) staff       (20)       52 2023-06-30 18:32:54.000000 photos-where-1.0/MANIFEST.in
--rw-r--r--   0 visgean    (501) staff       (20)      474 2023-06-30 19:00:17.436114 photos-where-1.0/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)       32 2022-09-28 18:42:28.000000 photos-where-1.0/README.md
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:00:17.435203 photos-where-1.0/photos_where.egg-info/
--rw-r--r--   0 visgean    (501) staff       (20)      474 2023-06-30 19:00:17.000000 photos-where-1.0/photos_where.egg-info/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)      297 2023-06-30 19:00:17.000000 photos-where-1.0/photos_where.egg-info/SOURCES.txt
--rw-r--r--   0 visgean    (501) staff       (20)        1 2023-06-30 19:00:17.000000 photos-where-1.0/photos_where.egg-info/dependency_links.txt
--rw-r--r--   0 visgean    (501) staff       (20)       46 2023-06-30 19:00:17.000000 photos-where-1.0/photos_where.egg-info/entry_points.txt
--rw-r--r--   0 visgean    (501) staff       (20)       30 2023-06-30 19:00:17.000000 photos-where-1.0/photos_where.egg-info/requires.txt
--rw-r--r--   0 visgean    (501) staff       (20)        4 2023-06-30 19:00:17.000000 photos-where-1.0/photos_where.egg-info/top_level.txt
--rw-r--r--   0 visgean    (501) staff       (20)       38 2023-06-30 19:00:17.436317 photos-where-1.0/setup.cfg
--rw-r--r--   0 visgean    (501) staff       (20)      944 2023-06-30 19:00:16.000000 photos-where-1.0/setup.py
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:00:17.435769 photos-where-1.0/src/
--rw-r--r--   0 visgean    (501) staff       (20)       24 2023-06-30 17:41:46.000000 photos-where-1.0/src/__init__.py
--rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos-where-1.0/src/main.py
--rw-r--r--   0 visgean    (501) staff       (20)     5094 2023-06-30 18:35:06.000000 photos-where-1.0/src/where.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:03:03.290268 photos-where-1.1/
+-rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos-where-1.1/LICENSE
+-rw-r--r--   0 visgean    (501) staff       (20)       52 2023-06-30 18:32:54.000000 photos-where-1.1/MANIFEST.in
+-rw-r--r--   0 visgean    (501) staff       (20)      896 2023-06-30 19:03:03.290115 photos-where-1.1/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)      318 2023-06-30 19:02:35.000000 photos-where-1.1/README.md
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:03:03.288830 photos-where-1.1/photos_where.egg-info/
+-rw-r--r--   0 visgean    (501) staff       (20)      896 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)      297 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/SOURCES.txt
+-rw-r--r--   0 visgean    (501) staff       (20)        1 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/dependency_links.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       46 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/entry_points.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       30 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/requires.txt
+-rw-r--r--   0 visgean    (501) staff       (20)        4 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/top_level.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       38 2023-06-30 19:03:03.290336 photos-where-1.1/setup.cfg
+-rw-r--r--   0 visgean    (501) staff       (20)      944 2023-06-30 19:00:50.000000 photos-where-1.1/setup.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:03:03.289491 photos-where-1.1/src/
+-rw-r--r--   0 visgean    (501) staff       (20)       24 2023-06-30 17:41:46.000000 photos-where-1.1/src/__init__.py
+-rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos-where-1.1/src/main.py
+-rw-r--r--   0 visgean    (501) staff       (20)     5094 2023-06-30 18:35:06.000000 photos-where-1.1/src/where.py
```

### Comparing `photos-where-1.0/LICENSE` & `photos-where-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `photos-where-1.0/setup.py` & `photos-where-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="photos-where",
-    version="1.0",
+    version="1.1",
     description="Analyze exif data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Visgean",
     author_email="visgean@gmail.com",
     url="https://github.com/visgean/where",
     packages=[
```

### Comparing `photos-where-1.0/src/main.py` & `photos-where-1.1/src/main.py`

 * *Files identical despite different names*

### Comparing `photos-where-1.0/src/where.py` & `photos-where-1.1/src/where.py`

 * *Files identical despite different names*

