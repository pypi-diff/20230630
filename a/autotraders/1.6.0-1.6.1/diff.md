# Comparing `tmp/autotraders-1.6.0.tar.gz` & `tmp/autotraders-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.6.0.tar", last modified: Thu Jun 29 22:40:49 2023, max compression
+gzip compressed data, was "autotraders-1.6.1.tar", last modified: Fri Jun 30 00:48:36 2023, max compression
```

## Comparing `autotraders-1.6.0.tar` & `autotraders-1.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.242345 autotraders-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 22:40:34.000000 autotraders-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-29 22:40:49.242345 autotraders-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-29 22:40:34.000000 autotraders-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.234345 autotraders-1.6.0/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.234345 autotraders-1.6.0/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.238345 autotraders-1.6.0/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.238345 autotraders-1.6.0/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.238345 autotraders-1.6.0/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/ship_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.238345 autotraders-1.6.0/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.234345 autotraders-1.6.0/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-29 22:40:34.000000 autotraders-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:40:49.242345 autotraders-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.242345 autotraders-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.788461 autotraders-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 00:48:21.000000 autotraders-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-30 00:48:36.784461 autotraders-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-30 00:48:21.000000 autotraders-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.780461 autotraders-1.6.1/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.780461 autotraders-1.6.1/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.780461 autotraders-1.6.1/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.784461 autotraders-1.6.1/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.784461 autotraders-1.6.1/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/ship_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.784461 autotraders-1.6.1/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.780461 autotraders-1.6.1/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-30 00:48:21.000000 autotraders-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 00:48:36.788461 autotraders-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.784461 autotraders-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_util.py
```

### Comparing `autotraders-1.6.0/LICENSE` & `autotraders-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/PKG-INFO` & `autotraders-1.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.6.0
+Version: 1.6.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.6.0/README.md` & `autotraders-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/agent.py` & `autotraders-1.6.1/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/faction/__init__.py` & `autotraders-1.6.1/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/faction/contract.py` & `autotraders-1.6.1/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/map/system.py` & `autotraders-1.6.1/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/map/waypoint.py` & `autotraders-1.6.1/autotraders/map/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.6.1/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.6.1/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.6.1/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.6.1/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/paginated_list.py` & `autotraders-1.6.1/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/session.py` & `autotraders-1.6.1/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/shared_models/map_symbol.py` & `autotraders-1.6.1/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/shared_models/transaction.py` & `autotraders-1.6.1/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/ship/__init__.py` & `autotraders-1.6.1/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/ship/cargo.py` & `autotraders-1.6.1/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/ship/nav.py` & `autotraders-1.6.1/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/ship/ship_components.py` & `autotraders-1.6.1/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/space_traders_entity.py` & `autotraders-1.6.1/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/status.py` & `autotraders-1.6.1/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders/util.py` & `autotraders-1.6.1/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/autotraders.egg-info/PKG-INFO` & `autotraders-1.6.1/autotraders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.6.0
+Version: 1.6.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.6.0/autotraders.egg-info/SOURCES.txt` & `autotraders-1.6.1/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/pyproject.toml` & `autotraders-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.6.0"
+version = "1.6.1"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.6.0/tests/test_init.py` & `autotraders-1.6.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/tests/test_map.py` & `autotraders-1.6.1/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/tests/test_ship.py` & `autotraders-1.6.1/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.0/tests/test_util.py` & `autotraders-1.6.1/tests/test_util.py`

 * *Files identical despite different names*

