# Comparing `tmp/specklia-1.1.6.tar.gz` & `tmp/specklia-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.1.6.tar", last modified: Thu Jun 29 16:44:20 2023, max compression
+gzip compressed data, was "specklia-1.1.7.tar", last modified: Fri Jun 30 09:15:23 2023, max compression
```

## Comparing `specklia-1.1.6.tar` & `specklia-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 16:44:20.130450 specklia-1.1.6/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-29 16:14:30.000000 specklia-1.1.6/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-29 16:44:20.130450 specklia-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-29 16:14:30.000000 specklia-1.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 16:44:20.130450 specklia-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2391 2023-06-29 16:43:09.000000 specklia-1.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 16:44:20.130450 specklia-1.1.6/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-29 16:14:30.000000 specklia-1.1.6/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-29 16:14:30.000000 specklia-1.1.6/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    24497 2023-06-29 16:43:09.000000 specklia-1.1.6/specklia/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 16:44:20.130450 specklia-1.1.6/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-29 16:44:20.000000 specklia-1.1.6/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-29 16:44:20.000000 specklia-1.1.6/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 16:44:20.000000 specklia-1.1.6/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-29 16:44:20.000000 specklia-1.1.6/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 16:44:20.000000 specklia-1.1.6/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 16:44:20.130450 specklia-1.1.6/tests/
--rw-r--r--   0 root         (0) root         (0)    10184 2023-06-29 16:14:30.000000 specklia-1.1.6/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6632 2023-06-29 16:14:30.000000 specklia-1.1.6/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:15:22.995435 specklia-1.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-30 09:15:13.000000 specklia-1.1.7/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 09:15:22.995435 specklia-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-30 09:15:13.000000 specklia-1.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-30 09:15:22.995435 specklia-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-06-30 09:15:13.000000 specklia-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:15:22.995435 specklia-1.1.7/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-30 09:15:13.000000 specklia-1.1.7/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-30 09:15:13.000000 specklia-1.1.7/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    24497 2023-06-30 09:15:13.000000 specklia-1.1.7/specklia/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:15:22.995435 specklia-1.1.7/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 09:15:22.000000 specklia-1.1.7/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-30 09:15:22.000000 specklia-1.1.7/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 09:15:22.000000 specklia-1.1.7/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-30 09:15:22.000000 specklia-1.1.7/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-30 09:15:22.000000 specklia-1.1.7/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:15:22.995435 specklia-1.1.7/tests/
+-rw-r--r--   0 root         (0) root         (0)    10184 2023-06-30 09:15:13.000000 specklia-1.1.7/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6632 2023-06-30 09:15:13.000000 specklia-1.1.7/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.1.6/LICENCE` & `specklia-1.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.1.6/PKG-INFO` & `specklia-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.1.6/README.md` & `specklia-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.1.6/setup.py` & `specklia-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.6/specklia/_websocket_helpers.py` & `specklia-1.1.7/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.6/specklia/client.py` & `specklia-1.1.7/specklia/client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.6/specklia.egg-info/PKG-INFO` & `specklia-1.1.7/specklia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.1.6/tests/test_client.py` & `specklia-1.1.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.6/tests/test_websocket_helpers.py` & `specklia-1.1.7/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

