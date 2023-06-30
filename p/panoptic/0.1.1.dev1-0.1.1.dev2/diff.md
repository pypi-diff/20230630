# Comparing `tmp/panoptic-0.1.1.dev1.tar.gz` & `tmp/panoptic-0.1.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptic-0.1.1.dev1.tar", last modified: Thu Jun 29 09:07:10 2023, max compression
+gzip compressed data, was "panoptic-0.1.1.dev2.tar", last modified: Fri Jun 30 12:29:49 2023, max compression
```

## Comparing `panoptic-0.1.1.dev1.tar` & `panoptic-0.1.1.dev2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.920733 panoptic-0.1.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-29 09:07:10.920733 panoptic-0.1.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/build_commans.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/description.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.912733 panoptic-0.1.1.dev1/panoptic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.912733 panoptic-0.1.1.dev1/panoptic/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/compute/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/compute/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/compute/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.912733 panoptic-0.1.1.dev1/panoptic/compute/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/compute/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/compute/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.916733 panoptic-0.1.1.dev1/panoptic/core/
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/core/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/core/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/core/image_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/core/process_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.916733 panoptic-0.1.1.dev1/panoptic/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.916733 panoptic-0.1.1.dev1/panoptic/html/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/html/assets/bootstrap-icons-966620f9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/html/assets/bootstrap-icons-c6569d46.woff
--rw-r--r--   0 runner    (1001) docker     (123)   354076 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/html/assets/index-44ffb943.js
--rw-r--r--   0 runner    (1001) docker     (123)   432216 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/html/assets/index-7cd47128.css
--rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/html/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.916733 panoptic-0.1.1.dev1/panoptic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/models/payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.920733 panoptic-0.1.1.dev1/panoptic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/scripts/create_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/scripts/create_faiss_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/scripts/populate_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/scripts/to_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/panoptic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:07:10.912733 panoptic-0.1.1.dev1/panoptic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-29 09:07:10.000000 panoptic-0.1.1.dev1/panoptic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-29 09:07:10.000000 panoptic-0.1.1.dev1/panoptic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:07:10.000000 panoptic-0.1.1.dev1/panoptic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 09:07:10.000000 panoptic-0.1.1.dev1/panoptic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 09:07:10.000000 panoptic-0.1.1.dev1/panoptic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 09:07:10.000000 panoptic-0.1.1.dev1/panoptic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:07:10.920733 panoptic-0.1.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-29 09:06:25.000000 panoptic-0.1.1.dev1/thunder-collection_Panoptic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/build_commans.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.230583 panoptic-0.1.1.dev2/panoptic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/compute/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/image_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/process_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/html/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/assets/bootstrap-icons-966620f9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/assets/bootstrap-icons-c6569d46.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   354076 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/assets/index-44ffb943.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432216 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/assets/index-7cd47128.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/panoptic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/models/payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/panoptic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/create_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/create_faiss_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/populate_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/to_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.230583 panoptic-0.1.1.dev2/panoptic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/thunder-collection_Panoptic.json
```

### Comparing `panoptic-0.1.1.dev1/PKG-INFO` & `panoptic-0.1.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.1.1.dev1
+Version: 0.1.1.dev2
 License: MPL-2.0 license
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.1.1.dev1/description.md` & `panoptic-0.1.1.dev2/description.md`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/api.py` & `panoptic-0.1.1.dev2/panoptic/api.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/compute/ocr.py` & `panoptic-0.1.1.dev2/panoptic/compute/ocr.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/compute/similarity.py` & `panoptic-0.1.1.dev2/panoptic/compute/similarity.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/compute/transform.py` & `panoptic-0.1.1.dev2/panoptic/compute/transform.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/compute/transformers/__init__.py` & `panoptic-0.1.1.dev2/panoptic/compute/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/compute/utils.py` & `panoptic-0.1.1.dev2/panoptic/compute/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/core/__init__.py` & `panoptic-0.1.1.dev2/panoptic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/core/db.py` & `panoptic-0.1.1.dev2/panoptic/core/db.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/core/db_utils.py` & `panoptic-0.1.1.dev2/panoptic/core/db_utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/core/image_importer.py` & `panoptic-0.1.1.dev2/panoptic/core/image_importer.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/core/process_queue.py` & `panoptic-0.1.1.dev2/panoptic/core/process_queue.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/html/assets/bootstrap-icons-966620f9.woff2` & `panoptic-0.1.1.dev2/panoptic/html/assets/bootstrap-icons-966620f9.woff2`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/html/assets/bootstrap-icons-c6569d46.woff` & `panoptic-0.1.1.dev2/panoptic/html/assets/bootstrap-icons-c6569d46.woff`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/html/assets/index-44ffb943.js` & `panoptic-0.1.1.dev2/panoptic/html/assets/index-44ffb943.js`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/html/assets/index-7cd47128.css` & `panoptic-0.1.1.dev2/panoptic/html/assets/index-7cd47128.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/html/favicon.ico` & `panoptic-0.1.1.dev2/panoptic/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/main.py` & `panoptic-0.1.1.dev2/panoptic/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 import os
+import pathlib
+import sys
 import tkinter as tk
 import webbrowser
 import socket
 import argparse
 from threading import Thread
 from time import sleep
 from tkinter import filedialog, ttk
@@ -221,19 +223,48 @@
 
 
 def on_fastapi_start():
     ui.server_status.set('fastapi init...')
     t1 = Thread(target=ui.init_folders)
     t1.start()
 
+def init_folders_server():
+    os.makedirs(os.path.dirname(PROJECT_PATH), exist_ok=True)
+
+    # Vérifier si le fichier JSON existe
+    if os.path.exists(PROJECT_PATH):
+        # Lire le fichier JSON
+        with open(PROJECT_PATH) as json_file:
+            projects = json.load(json_file)
+    else:
+        projects = {'projects': [], 'last_opened': None}
+        # Créer un fichier JSON avec une liste vide
+        with open(PROJECT_PATH, 'w') as json_file:
+            json.dump(projects, json_file)
+    if len(projects['projects']) == 0:
+        with open(PROJECT_PATH, 'w') as f:
+            new_project = {'name': "panoptic", 'path': (pathlib.Path.home() / 'panoptic').as_posix()}
+            projects['projects'].append(new_project)
+            json.dump(projects, f)
+    os.environ['PANOPTIC_DATA'] = projects['projects'][0]['path']
+    path = os.path.join(os.environ['PANOPTIC_DATA'], 'mini')
+    if not os.path.exists(path):
+        os.makedirs(path)
+    # requests.post(api("project"), json={"project": projects['projects'][0]['path']})
+    requests.post(api('folders'), headers={"Content-type": "application/json"}, json={"path": FOLDER}).json()
+
+def on_fastapi_start_server():
+    t1 = Thread(target=init_folders_server)
+    t1.start()
 
 def launch_uvicorn():
     from panoptic.api import app
-    app.add_event_handler('startup', on_fastapi_start)
-    app.add_event_handler('shutdown', lambda: ui.server_status.set('stopped'))
+    app.add_event_handler('startup', on_fastapi_start if not SERVER else on_fastapi_start_server)
+    if not SERVER:
+        app.add_event_handler('shutdown', lambda: ui.server_status.set('stopped'))
     if HOST:
         uvicorn.run(app, host="0.0.0.0", port=PORT)
     else:
         uvicorn.run(app)
 
 
 def start_thread():
@@ -243,25 +274,41 @@
     THREAD.start()
 
 
 def start():
     parser = argparse.ArgumentParser(
         description="Start Panoptic, use --host to share your panoptic across local network")
     parser.add_argument('--host', action="store_true")
+    parser.add_argument('--server', action="store_true")
+    parser.add_argument('--folder', type=str)
+
     args = parser.parse_args()
     global HOST
+    global SERVER
+    global FOLDER
     HOST = args.host
-    root = tk.Tk()
-    try:
-        root.iconbitmap(os.path.join(os.path.dirname(__file__), "html/favicon.ico"))
-    except:
-        pass
+    SERVER = args.server
+    FOLDER = args.folder
+
+    if not SERVER:
+        root = tk.Tk()
+        try:
+            root.iconbitmap(os.path.join(os.path.dirname(__file__), "html/favicon.ico"))
+        except:
+            pass
+
+        global ui
+        ui = MiniUI(root)
+
+        root.mainloop()
+    else:
+        if not FOLDER:
+            print("folder parameter need to be fullfilled in server mode")
+            sys.exit(0)
+        launch_uvicorn()
 
-    global ui
-    ui = MiniUI(root)
 
-    root.mainloop()
 
 
 if __name__ == '__main__':
     start()
```

### Comparing `panoptic-0.1.1.dev1/panoptic/models/models.py` & `panoptic-0.1.1.dev2/panoptic/models/models.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/models/payloads.py` & `panoptic-0.1.1.dev2/panoptic/models/payloads.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/scripts/create_db.sql` & `panoptic-0.1.1.dev2/panoptic/scripts/create_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/scripts/create_faiss_index.py` & `panoptic-0.1.1.dev2/panoptic/scripts/create_faiss_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,13 +14,14 @@
     all_images: list[ComputedValue] = await db.get_sha1_computed_values()
     create_similarity_tree_faiss(all_images)
     logger.info('Success')
 
 async def start():
     os.environ['PANOPTIC_DATA'] = "D:\\Alie\\Documents\\panoptic_GJ"
     await db_utils.init()
+    await compute_faiss_index()
 
 if __name__ == '__main__':
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(start())
```

### Comparing `panoptic-0.1.1.dev1/panoptic/scripts/populate_db.sql` & `panoptic-0.1.1.dev2/panoptic/scripts/populate_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/scripts/to_pca.py` & `panoptic-0.1.1.dev2/panoptic/scripts/to_pca.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic/utils.py` & `panoptic-0.1.1.dev2/panoptic/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/panoptic.egg-info/PKG-INFO` & `panoptic-0.1.1.dev2/panoptic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.1.1.dev1
+Version: 0.1.1.dev2
 License: MPL-2.0 license
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.1.1.dev1/panoptic.egg-info/SOURCES.txt` & `panoptic-0.1.1.dev2/panoptic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev1/setup.py` & `panoptic-0.1.1.dev2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def parse_requirements(req_file):
     with open(req_file) as fp:
         _requires = fp.read()
     return _requires
 
 
 NAME = "panoptic"
-VERSION = "0.1.1.dev1"
+VERSION = "0.1.1.dev2"
 # Get dependencies from requirement files
 SETUP_REQUIRES = ['setuptools', 'setuptools-git', 'wheel']
 INSTALL_REQUIRES = parse_requirements('requirements.txt')
 LONG_DESCRIPTION = ""
 
 with open(os.path.join(os.path.dirname(__file__), 'description.md'), 'r') as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `panoptic-0.1.1.dev1/thunder-collection_Panoptic.json` & `panoptic-0.1.1.dev2/thunder-collection_Panoptic.json`

 * *Files identical despite different names*

