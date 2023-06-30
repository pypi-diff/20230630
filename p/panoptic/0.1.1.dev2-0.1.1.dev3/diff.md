# Comparing `tmp/panoptic-0.1.1.dev2.tar.gz` & `tmp/panoptic-0.1.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptic-0.1.1.dev2.tar", last modified: Fri Jun 30 12:29:49 2023, max compression
+gzip compressed data, was "panoptic-0.1.1.dev3.tar", last modified: Fri Jun 30 13:18:48 2023, max compression
```

## Comparing `panoptic-0.1.1.dev2.tar` & `panoptic-0.1.1.dev3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/build_commans.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/description.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.230583 panoptic-0.1.1.dev2/panoptic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/compute/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/compute/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/core/
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/image_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/core/process_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.234583 panoptic-0.1.1.dev2/panoptic/html/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/assets/bootstrap-icons-966620f9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/assets/bootstrap-icons-c6569d46.woff
--rw-r--r--   0 runner    (1001) docker     (123)   354076 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/assets/index-44ffb943.js
--rw-r--r--   0 runner    (1001) docker     (123)   432216 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/assets/index-7cd47128.css
--rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/panoptic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/models/payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/panoptic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/create_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/create_faiss_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/populate_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/scripts/to_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/panoptic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:29:49.230583 panoptic-0.1.1.dev2/panoptic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 12:29:49.000000 panoptic-0.1.1.dev2/panoptic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:29:49.238583 panoptic-0.1.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-30 12:29:31.000000 panoptic-0.1.1.dev2/thunder-collection_Panoptic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.634533 panoptic-0.1.1.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-30 13:18:48.634533 panoptic-0.1.1.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/build_commans.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.626533 panoptic-0.1.1.dev3/panoptic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.630533 panoptic-0.1.1.dev3/panoptic/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/compute/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/compute/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/compute/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.630533 panoptic-0.1.1.dev3/panoptic/compute/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/compute/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.630533 panoptic-0.1.1.dev3/panoptic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/core/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/core/image_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/core/process_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.630533 panoptic-0.1.1.dev3/panoptic/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.630533 panoptic-0.1.1.dev3/panoptic/html/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/html/assets/bootstrap-icons-966620f9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/html/assets/bootstrap-icons-c6569d46.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   354076 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/html/assets/index-44ffb943.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432216 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/html/assets/index-7cd47128.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/html/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.634533 panoptic-0.1.1.dev3/panoptic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/models/payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.634533 panoptic-0.1.1.dev3/panoptic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/scripts/create_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/scripts/create_faiss_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/scripts/populate_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/scripts/to_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/panoptic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:48.626533 panoptic-0.1.1.dev3/panoptic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-30 13:18:48.000000 panoptic-0.1.1.dev3/panoptic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-30 13:18:48.000000 panoptic-0.1.1.dev3/panoptic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:18:48.000000 panoptic-0.1.1.dev3/panoptic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 13:18:48.000000 panoptic-0.1.1.dev3/panoptic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 13:18:48.000000 panoptic-0.1.1.dev3/panoptic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 13:18:48.000000 panoptic-0.1.1.dev3/panoptic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:18:48.634533 panoptic-0.1.1.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-30 13:18:33.000000 panoptic-0.1.1.dev3/thunder-collection_Panoptic.json
```

### Comparing `panoptic-0.1.1.dev2/PKG-INFO` & `panoptic-0.1.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.1.1.dev2
+Version: 0.1.1.dev3
 License: MPL-2.0 license
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.1.1.dev2/description.md` & `panoptic-0.1.1.dev3/description.md`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/api.py` & `panoptic-0.1.1.dev3/panoptic/api.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/compute/ocr.py` & `panoptic-0.1.1.dev3/panoptic/compute/ocr.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/compute/similarity.py` & `panoptic-0.1.1.dev3/panoptic/compute/similarity.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/compute/transform.py` & `panoptic-0.1.1.dev3/panoptic/compute/transform.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/compute/transformers/__init__.py` & `panoptic-0.1.1.dev3/panoptic/compute/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/compute/utils.py` & `panoptic-0.1.1.dev3/panoptic/compute/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/core/__init__.py` & `panoptic-0.1.1.dev3/panoptic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/core/db.py` & `panoptic-0.1.1.dev3/panoptic/core/db.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/core/db_utils.py` & `panoptic-0.1.1.dev3/panoptic/core/db_utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/core/image_importer.py` & `panoptic-0.1.1.dev3/panoptic/core/image_importer.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/core/process_queue.py` & `panoptic-0.1.1.dev3/panoptic/core/process_queue.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/html/assets/bootstrap-icons-966620f9.woff2` & `panoptic-0.1.1.dev3/panoptic/html/assets/bootstrap-icons-966620f9.woff2`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/html/assets/bootstrap-icons-c6569d46.woff` & `panoptic-0.1.1.dev3/panoptic/html/assets/bootstrap-icons-c6569d46.woff`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/html/assets/index-44ffb943.js` & `panoptic-0.1.1.dev3/panoptic/html/assets/index-44ffb943.js`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/html/assets/index-7cd47128.css` & `panoptic-0.1.1.dev3/panoptic/html/assets/index-7cd47128.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/html/favicon.ico` & `panoptic-0.1.1.dev3/panoptic/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/main.py` & `panoptic-0.1.1.dev3/panoptic/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from tkinter.filedialog import askdirectory
 
 import uvicorn
 import requests
 
 from panoptic.utils import get_datadir
 
-PORT = 8000
+PORT = 8123
 HOST = False
 THREAD = None
 
 
 def api(path):
     return 'http://localhost:' + str(PORT) + '/' + path
 
@@ -224,32 +224,15 @@
 
 def on_fastapi_start():
     ui.server_status.set('fastapi init...')
     t1 = Thread(target=ui.init_folders)
     t1.start()
 
 def init_folders_server():
-    os.makedirs(os.path.dirname(PROJECT_PATH), exist_ok=True)
-
-    # Vérifier si le fichier JSON existe
-    if os.path.exists(PROJECT_PATH):
-        # Lire le fichier JSON
-        with open(PROJECT_PATH) as json_file:
-            projects = json.load(json_file)
-    else:
-        projects = {'projects': [], 'last_opened': None}
-        # Créer un fichier JSON avec une liste vide
-        with open(PROJECT_PATH, 'w') as json_file:
-            json.dump(projects, json_file)
-    if len(projects['projects']) == 0:
-        with open(PROJECT_PATH, 'w') as f:
-            new_project = {'name': "panoptic", 'path': (pathlib.Path.home() / 'panoptic').as_posix()}
-            projects['projects'].append(new_project)
-            json.dump(projects, f)
-    os.environ['PANOPTIC_DATA'] = projects['projects'][0]['path']
+    os.environ['PANOPTIC_DATA'] = os.getenv('PANOPTIC_DATA', (pathlib.Path.home() / 'panoptic').as_posix())
     path = os.path.join(os.environ['PANOPTIC_DATA'], 'mini')
     if not os.path.exists(path):
         os.makedirs(path)
     # requests.post(api("project"), json={"project": projects['projects'][0]['path']})
     requests.post(api('folders'), headers={"Content-type": "application/json"}, json={"path": FOLDER}).json()
 
 def on_fastapi_start_server():
```

### Comparing `panoptic-0.1.1.dev2/panoptic/models/models.py` & `panoptic-0.1.1.dev3/panoptic/models/models.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/models/payloads.py` & `panoptic-0.1.1.dev3/panoptic/models/payloads.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/scripts/create_db.sql` & `panoptic-0.1.1.dev3/panoptic/scripts/create_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/scripts/create_faiss_index.py` & `panoptic-0.1.1.dev3/panoptic/scripts/create_faiss_index.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/scripts/populate_db.sql` & `panoptic-0.1.1.dev3/panoptic/scripts/populate_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/scripts/to_pca.py` & `panoptic-0.1.1.dev3/panoptic/scripts/to_pca.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic/utils.py` & `panoptic-0.1.1.dev3/panoptic/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/panoptic.egg-info/PKG-INFO` & `panoptic-0.1.1.dev3/panoptic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.1.1.dev2
+Version: 0.1.1.dev3
 License: MPL-2.0 license
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.1.1.dev2/panoptic.egg-info/SOURCES.txt` & `panoptic-0.1.1.dev3/panoptic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panoptic-0.1.1.dev2/setup.py` & `panoptic-0.1.1.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def parse_requirements(req_file):
     with open(req_file) as fp:
         _requires = fp.read()
     return _requires
 
 
 NAME = "panoptic"
-VERSION = "0.1.1.dev2"
+VERSION = "0.1.1.dev3"
 # Get dependencies from requirement files
 SETUP_REQUIRES = ['setuptools', 'setuptools-git', 'wheel']
 INSTALL_REQUIRES = parse_requirements('requirements.txt')
 LONG_DESCRIPTION = ""
 
 with open(os.path.join(os.path.dirname(__file__), 'description.md'), 'r') as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `panoptic-0.1.1.dev2/thunder-collection_Panoptic.json` & `panoptic-0.1.1.dev3/thunder-collection_Panoptic.json`

 * *Files identical despite different names*

