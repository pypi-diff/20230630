# Comparing `tmp/preheat_open-1.38.tar.gz` & `tmp/preheat_open-1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preheat_open-1.38.tar", last modified: Tue Mar 14 12:28:25 2023, max compression
+gzip compressed data, was "preheat_open-1.39.tar", last modified: Fri Jun 30 13:00:40 2023, max compression
```

## Comparing `preheat_open-1.38.tar` & `preheat_open-1.39.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 pvf       (1000) pvf       (1000)        0 2023-03-14 12:28:25.375611 preheat_open-1.38/
--rw-rw-r--   0 pvf       (1000) pvf       (1000)    11357 2023-02-28 21:11:41.000000 preheat_open-1.38/LICENSE
--rw-rw-r--   0 pvf       (1000) pvf       (1000)       55 2023-02-28 21:11:41.000000 preheat_open-1.38/MANIFEST.in
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2999 2023-03-14 12:28:25.375611 preheat_open-1.38/PKG-INFO
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2343 2023-02-28 21:11:41.000000 preheat_open-1.38/README.md
-drwxrwxr-x   0 pvf       (1000) pvf       (1000)        0 2023-03-14 12:28:25.359611 preheat_open-1.38/docs/
--rw-rw-r--   0 pvf       (1000) pvf       (1000)       69 2023-02-28 21:11:41.000000 preheat_open-1.38/docs/requirements.txt
-drwxrwxr-x   0 pvf       (1000) pvf       (1000)        0 2023-03-14 12:28:25.375611 preheat_open-1.38/preheat_open/
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1073 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/__init__.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      496 2023-03-14 12:28:25.375611 preheat_open-1.38/preheat_open/_version.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)    14939 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/api.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2243 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/backwards_compatibility.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)    19368 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/building.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)    12131 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/building_unit.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     3859 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/cache.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1292 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/comfort_profiles.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      913 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/component.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2220 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/control_unit.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     9276 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/data.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2098 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/device.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      625 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/exceptions.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     5021 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/helpers.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     6701 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/logging.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)    12894 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/price.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2014 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/setpoints.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      239 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/singleton.py
-drwxrwxr-x   0 pvf       (1000) pvf       (1000)        0 2023-03-14 12:28:25.375611 preheat_open-1.38/preheat_open/test/
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1866 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/__init__.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1947 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/test/conftest.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      674 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_anonymisation.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     3380 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_api.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1215 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_backwards_compatibility.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     4308 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_building.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2266 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_building_unit.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1138 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/test/test_cache.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     5192 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_control_unit.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     5233 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_data.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2105 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_device.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      829 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_helpers.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1596 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_import.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1038 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_price.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1621 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_unit.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2010 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/test/test_weather.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     3299 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/test/test_zone.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      109 2023-02-28 21:11:41.000000 preheat_open-1.38/preheat_open/types.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     9853 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/unit.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     4616 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/unit_graph.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     3690 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/weather.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     8149 2023-02-28 21:28:25.000000 preheat_open-1.38/preheat_open/zone.py
-drwxrwxr-x   0 pvf       (1000) pvf       (1000)        0 2023-03-14 12:28:25.371611 preheat_open-1.38/preheat_open.egg-info/
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     2999 2023-03-14 12:28:25.000000 preheat_open-1.38/preheat_open.egg-info/PKG-INFO
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1463 2023-03-14 12:28:25.000000 preheat_open-1.38/preheat_open.egg-info/SOURCES.txt
--rw-rw-r--   0 pvf       (1000) pvf       (1000)        1 2023-03-14 12:28:25.000000 preheat_open-1.38/preheat_open.egg-info/dependency_links.txt
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      255 2023-03-14 12:28:25.000000 preheat_open-1.38/preheat_open.egg-info/requires.txt
--rw-rw-r--   0 pvf       (1000) pvf       (1000)       13 2023-03-14 12:28:25.000000 preheat_open-1.38/preheat_open.egg-info/top_level.txt
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      244 2023-02-28 21:11:41.000000 preheat_open-1.38/pyproject.toml
--rw-rw-r--   0 pvf       (1000) pvf       (1000)       48 2023-02-28 21:11:41.000000 preheat_open-1.38/requirements.txt
--rw-rw-r--   0 pvf       (1000) pvf       (1000)      345 2023-03-14 12:28:25.375611 preheat_open-1.38/setup.cfg
--rw-rw-r--   0 pvf       (1000) pvf       (1000)     1450 2023-02-28 21:11:41.000000 preheat_open-1.38/setup.py
--rw-rw-r--   0 pvf       (1000) pvf       (1000)    78325 2023-02-28 21:11:41.000000 preheat_open-1.38/versioneer.py
+drwxrwxr-x   0 ala       (1000) ala       (1000)        0 2023-06-30 13:00:40.478613 preheat_open-1.39/
+-rw-rw-r--   0 ala       (1000) ala       (1000)    11357 2023-05-23 12:48:53.000000 preheat_open-1.39/LICENSE
+-rw-rw-r--   0 ala       (1000) ala       (1000)       55 2023-05-23 12:48:53.000000 preheat_open-1.39/MANIFEST.in
+-rw-rw-r--   0 ala       (1000) ala       (1000)     3117 2023-06-30 13:00:40.478613 preheat_open-1.39/PKG-INFO
+-rw-rw-r--   0 ala       (1000) ala       (1000)     2399 2023-06-30 12:56:40.000000 preheat_open-1.39/README.md
+drwxrwxr-x   0 ala       (1000) ala       (1000)        0 2023-06-30 13:00:40.474613 preheat_open-1.39/docs/
+-rw-rw-r--   0 ala       (1000) ala       (1000)       80 2023-06-30 12:56:40.000000 preheat_open-1.39/docs/requirements.txt
+drwxrwxr-x   0 ala       (1000) ala       (1000)        0 2023-06-30 13:00:40.478613 preheat_open-1.39/preheat_open/
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1420 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/__init__.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)      496 2023-06-30 13:00:40.478613 preheat_open-1.39/preheat_open/_version.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)    16557 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/api.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1662 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/backwards_compatibility.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)    19898 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/building.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)    12313 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/building_unit.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     4099 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/cache.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1383 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/comfort_profiles.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1250 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/component.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     2986 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/control_unit.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)    10375 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/data.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     4300 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/device.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)      668 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/exceptions.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     7156 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/helpers.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     6496 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/logging.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)    12944 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/price.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1947 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/setpoints.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)      239 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/singleton.py
+drwxrwxr-x   0 ala       (1000) ala       (1000)        0 2023-06-30 13:00:40.478613 preheat_open-1.39/preheat_open/test/
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1866 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/__init__.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1854 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/conftest.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)      674 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_anonymisation.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     3380 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_api.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1215 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_backwards_compatibility.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     4489 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/test/test_building.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     2266 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_building_unit.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1097 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_cache.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     5192 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_control_unit.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     5233 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_data.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     2105 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_device.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)      829 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_helpers.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1596 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_import.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1038 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_price.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1621 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_unit.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1958 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/test/test_weather.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     3379 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/test/test_zone.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)      109 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/types.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)    13916 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/unit.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     4474 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/unit_graph.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     4070 2023-06-30 12:56:40.000000 preheat_open-1.39/preheat_open/weather.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)     7916 2023-05-23 12:48:53.000000 preheat_open-1.39/preheat_open/zone.py
+drwxrwxr-x   0 ala       (1000) ala       (1000)        0 2023-06-30 13:00:40.478613 preheat_open-1.39/preheat_open.egg-info/
+-rw-rw-r--   0 ala       (1000) ala       (1000)     3117 2023-06-30 13:00:40.000000 preheat_open-1.39/preheat_open.egg-info/PKG-INFO
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1463 2023-06-30 13:00:40.000000 preheat_open-1.39/preheat_open.egg-info/SOURCES.txt
+-rw-rw-r--   0 ala       (1000) ala       (1000)        1 2023-06-30 13:00:40.000000 preheat_open-1.39/preheat_open.egg-info/dependency_links.txt
+-rw-rw-r--   0 ala       (1000) ala       (1000)      274 2023-06-30 13:00:40.000000 preheat_open-1.39/preheat_open.egg-info/requires.txt
+-rw-rw-r--   0 ala       (1000) ala       (1000)       13 2023-06-30 13:00:40.000000 preheat_open-1.39/preheat_open.egg-info/top_level.txt
+-rw-rw-r--   0 ala       (1000) ala       (1000)      244 2023-05-23 12:48:53.000000 preheat_open-1.39/pyproject.toml
+-rw-rw-r--   0 ala       (1000) ala       (1000)       60 2023-06-30 12:56:40.000000 preheat_open-1.39/requirements.txt
+-rw-rw-r--   0 ala       (1000) ala       (1000)      345 2023-06-30 13:00:40.478613 preheat_open-1.39/setup.cfg
+-rw-rw-r--   0 ala       (1000) ala       (1000)     1612 2023-06-30 12:56:40.000000 preheat_open-1.39/setup.py
+-rw-rw-r--   0 ala       (1000) ala       (1000)    78325 2023-05-23 12:48:53.000000 preheat_open-1.39/versioneer.py
```

### Comparing `preheat_open-1.38/LICENSE` & `preheat_open-1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/PKG-INFO` & `preheat_open-1.39/preheat_open.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
-Name: preheat_open
-Version: 1.38
+Name: preheat-open
+Version: 1.39
 Summary: Python wrapper for Neogrid Technologies' REST API
 Home-page: https://gitlab.com/neogrid-technologies-public/preheat-open-python
 Author: Neogrid and contributors
 Author-email: analytics@neogrid.dk
 Project-URL: Bug Tracker, https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/issues
 Project-URL: Documentation, https://preheat-open.readthedocs.io/en/latest/
 Project-URL: Source Code, https://gitlab.com/neogrid-technologies-public/preheat-open-python
+Project-URL: Changelog, https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/RELEASE_NOTES.md
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # PreHEAT Open Python Package
 
 This is the open Python package to consume Neogrids REST API.
 
-For a quick introduction to how to use it on real-world data, see the [**quick start guide**](https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/docs/source/tutorials/demo.ipynb).
+For a quick introduction to how to use it on real-world data, see the [quick start guide](https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/docs/source/tutorials/demo.ipynb).
 
 ## Installation and configuration
 
 ### Simple installation:
 Install the package directly from [PyPi](https://pypi.org/project/preheat-open/) using:
 
     pip install preheat_open
```

### Comparing `preheat_open-1.38/README.md` & `preheat_open-1.39/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# PreHEAT Open Python Package
-
-This is the open Python package to consume Neogrids REST API.
-
-For a quick introduction to how to use it on real-world data, see the [**quick start guide**](https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/docs/source/tutorials/demo.ipynb).
-
-## Installation and configuration
-
-### Simple installation:
-Install the package directly from [PyPi](https://pypi.org/project/preheat-open/) using:
-
-    pip install preheat_open
-
-
-
-### Configuring the toolbox
-First, make sure that you have created an API key for your user. This can be done on your [user profile page](https://app.neogrid.dk/icebear/#!/app/user/profile) in the PreHEAT App.
-
-Now, you can store the API key in a configuration file. This user configuration file should be created in the following places:
-
-| OS      | User level (recommended)                  | Machine level                  |  
-|---------|-------------------------------------------|--------------------------------|
-| Windows | C:/Users/[your user]/.preheat/config.json | (unsupported)                  |
-| Linux   | ~/.preheat/config.json                    | /etc[/opt]/preheat/config.json |
-
-The configuration files are read in the following priority order (using the first available):
-
-1- User level
-
-2- Machine level (Linux only): */etc/opt/preheat/config.json*
-
-3- Machine level (Linux only): */etc/preheat/config.json*
-
-And then add the following content in this file (adjusting with your API key):
-
-
-```
-{
-  "PREHEAT_API_KEY": "YOUR_API_KEY_HERE"
-}
-```
-
-Alternatively, you can also just import it explicitly in your code using the following command in your code 
-(this is however not recommended, as you risk compromising your API key when sharing your code with others) :
-
-```
-from preheat_open import set_api_key
-
-set_api_key("YOUR_API_KEY_HERE")
-```
-
-## Additional Information
-You can find additional information about the [PreHeat API here](https://neogrid-technologies.gitlab.io/neogrid-api/).
-
-## Contributions
-
-We encourage pull requests if you have developed new interesting features.
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+# PreHEAT Open Python Package
+
+This is the open Python package to consume Neogrids REST API.
+
+For a quick introduction to how to use it on real-world data, see the [quick start guide](https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/docs/source/tutorials/demo.ipynb).
+
+## Installation and configuration
+
+### Simple installation:
+Install the package directly from [PyPi](https://pypi.org/project/preheat-open/) using:
+
+    pip install preheat_open
+
+
+
+### Configuring the toolbox
+First, make sure that you have created an API key for your user. This can be done on your [user profile page](https://app.neogrid.dk/icebear/#!/app/user/profile) in the PreHEAT App.
+
+Now, you can store the API key in a configuration file. This user configuration file should be created in the following places:
+
+| OS      | User level (recommended)                  | Machine level                  |  
+|---------|-------------------------------------------|--------------------------------|
+| Windows | C:/Users/[your user]/.preheat/config.json | (unsupported)                  |
+| Linux   | ~/.preheat/config.json                    | /etc[/opt]/preheat/config.json |
+
+The configuration files are read in the following priority order (using the first available):
+
+1- User level
+
+2- Machine level (Linux only): */etc/opt/preheat/config.json*
+
+3- Machine level (Linux only): */etc/preheat/config.json*
+
+And then add the following content in this file (adjusting with your API key):
+
+
+```
+{
+  "PREHEAT_API_KEY": "YOUR_API_KEY_HERE"
+}
+```
+
+Alternatively, you can also just import it explicitly in your code using the following command in your code 
+(this is however not recommended, as you risk compromising your API key when sharing your code with others) :
+
+```
+from preheat_open import set_api_key
+
+set_api_key("YOUR_API_KEY_HERE")
+```
+
+## Additional Information
+You can find additional information about the [PreHeat API here](https://neogrid-technologies.gitlab.io/neogrid-api/).
+
+## Contributions
+
+We encourage pull requests if you have developed new interesting features.
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
```

### Comparing `preheat_open-1.38/preheat_open/__init__.py` & `preheat_open-1.39/preheat_open/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,55 @@
-# Imports for backwards compatibility of dependent code
-# noinspection PyUnresolvedReferences
-import os
-import re
-import sys
-
-from . import _version
-from .api import (
-    BASE_URL,
-    MAX_CIDS_PER_REQ,
-    MAX_POINTS_PER_REQ,
-    TIMEZONE,
-    AccessDeniedError,
-    APIDataExtractError,
-    APIKeyMissingError,
-    load_configuration,
-    set_api_key,
-)
-
-# noinspection PyUnresolvedReferences
-from .building import Building, available_buildings
-
-# noinspection PyUnresolvedReferences
-from .logging import set_logging_level
-
-# noinspection PyUnresolvedReferences
-from .unit import Unit
-
-__version__ = _version.get_versions()["version"]
-
-
-config = load_configuration()
-
-
-def running_in_test_mode() -> bool:
-    # A function to detect whether or not the system is running with Pytest
-    if "PYTEST_CURRENT_TEST" in os.environ:
-        return True
-    elif any(re.findall(r"pytest|py.test", sys.argv[0])):
-        return True
-    else:
-        return False
-
-
-# list of environment variables for tricks
-ENV_VAR_TRACK_MISSING_DATA_FIELD = "PREHEAT_OPEN_TRACK_MISSING_FIELDS"
+"""
+The preheat_open package provides methods to load building data from `Neogrids <https://www.neogrid.dk/>`_ platform
+"""
+
+# Imports for backwards compatibility of dependent code
+# noinspection PyUnresolvedReferences
+import os
+import re
+import sys
+
+from . import _version
+from .api import (
+    BASE_URL,
+    MAX_CIDS_PER_REQ,
+    MAX_POINTS_PER_REQ,
+    TIMEZONE,
+    AccessDeniedError,
+    APIDataExtractError,
+    APIKeyMissingError,
+    load_configuration,
+    set_api_key,
+)
+
+# noinspection PyUnresolvedReferences
+from .building import Building, available_buildings
+
+# noinspection PyUnresolvedReferences
+from .logging import set_logging_level
+
+# noinspection PyUnresolvedReferences
+from .unit import Unit
+
+__version__ = _version.get_versions()["version"]
+
+
+config = load_configuration()
+
+
+def running_in_test_mode() -> bool:
+    """
+    Method to evaluate whether the code is running in test mode. Test mode is activated when using Pytest
+
+    :return: True if running in test mode, False otherwise
+    """
+    # Pytest is detailed via argv or an environment variable
+    if "PYTEST_CURRENT_TEST" in os.environ:
+        return True
+    elif any(re.findall(r"pytest|py.test", sys.argv[0])):
+        return True
+    else:
+        return False
+
+
+# list of environment variables for tricks
+ENV_VAR_TRACK_MISSING_DATA_FIELD = "PREHEAT_OPEN_TRACK_MISSING_FIELDS"
```

### Comparing `preheat_open-1.38/preheat_open/api.py` & `preheat_open-1.39/preheat_open/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,76 +13,78 @@
 from requests import Session
 from requests.adapters import HTTPAdapter
 from requests.models import Response
 from urllib3.util.retry import Retry
 
 import preheat_open
 
+from .backwards_compatibility import warn_deprecation_pending
 from .exceptions import (  # For backwards compatibility
     AccessDeniedError,
     APIDataExtractError,
     APIKeyMissingError,
     MissingConfigurationFile,
     MissingConfigurationFileError,
 )
 from .logging import Logging, write_log_to_profiling_file
 from .singleton import Singleton
 
+# Settings of the API
 BASE_URL: str = "https://api.neogrid.dk/public/api/v1"
 MAX_CIDS_PER_REQ: int = 3
 MAX_POINTS_PER_REQ: int = 90000
 MAX_IDS_AND_CIDS_PER_REQUEST: int = 100
-
 GET_TIMEOUT_SECONDS: int = 60
 PUT_TIMEOUT_SECONDS: int = 10
 
 # Perhaps we can steal this from the OS?
 TIMEZONE = gettz("Europe/Copenhagen")
 DATETIME_FORMAT: str = "%Y-%m-%dT%H:%M:%S.%fZ"
 
+# Addresses of the configuration file (if changing this, make sure to update the documentation in the README file
 USER_LEVEL_CONFIGURATION_FILE: str = os.path.expanduser("~/.preheat/config.json")
 MACHINE_LEVEL_CONFIGURATION_FILE: str = os.path.expanduser("/etc/preheat/config.json")
 MACHINE_LEVEL_CONFIGURATION_FILE_OPT: str = os.path.expanduser(
     "/etc/opt/preheat/config.json"
 )
 
 
 def configuration_file_path() -> str:
     """
-    Determines the path of the configuration file to be used
+    Determines the path of the configuration file to be used.
 
+    :raise: preheat_open.exceptions.MissingConfigurationFileError if no cofiguration file is available
     :return: full path of the configuration file
     """
-    if os.path.exists(USER_LEVEL_CONFIGURATION_FILE):
-        out = USER_LEVEL_CONFIGURATION_FILE
-    elif os.path.exists(MACHINE_LEVEL_CONFIGURATION_FILE_OPT):
-        out = MACHINE_LEVEL_CONFIGURATION_FILE_OPT
-    elif os.path.exists(MACHINE_LEVEL_CONFIGURATION_FILE):
-        out = MACHINE_LEVEL_CONFIGURATION_FILE
-    else:
-        raise MissingConfigurationFileError()
-    return out
+    for i in [
+        USER_LEVEL_CONFIGURATION_FILE,
+        MACHINE_LEVEL_CONFIGURATION_FILE_OPT,
+        MACHINE_LEVEL_CONFIGURATION_FILE,
+    ]:
+        if os.path.exists(i):
+            return i
+    raise MissingConfigurationFileError()
 
 
 def api_string_to_datetime(t: str) -> datetime:
     """
     Converts a datetime string from the API to a python datetime
 
     :param t: datetime in string format
-    :return: python datetime
+    :return: datetime corresponding to the input
     """
     return datetime.strptime(t, "%Y-%m-%dT%H:%M:%S.%f%z")
 
 
 def datetime_to_api_string(t: datetime) -> str:
     """
     Converts a python datetime to a string ready for use in the API I/O
 
-    :param t: python datetime
-    :return:
+    :param t: datetime to convert to string
+    :return: a string with a format compatible with the API
     """
     return t.isoformat()
 
 
 def ids_list_to_string(list2use: list, separator: str = ",") -> str:
     """
     Helper function to turn list into string, e.g. comma separated (default).
@@ -179,39 +181,37 @@
         headers = {"Authorization": "Apikey " + str(api_key)}
         self.session.headers.update(headers)
 
     def set_api_url(self, api_url=None):
         """
         DEPRECATED (only kept for backwards-compatibility)
         """
-        Logging().warning(
-            DeprecationWarning(f"Manual update of the API url is deprecated")
-        )
+        warn_deprecation_pending(f"Manual update of the API url is deprecated")
 
     def __log_api_io(self, msg: str) -> None:
         Logging().debug(msg)
         write_log_to_profiling_file("API-I/O: " + msg)
 
     def api_get(
         self,
         endpoint: str,
         out: str = "json",
         payload: Optional[dict[str, Any]] = None,
         headers: Optional[dict[str, Any]] = None,
         bare_url: bool = False,
     ):
         """
-        Carries out a get request on the API
+        Method to send a GET request to the API
 
-        :param endpoint: endpoint to call on the API
-        :param out: format for the output (json or csv)
-        :param payload:
-        :param headers:
-        :param bare_url:
-        :return:
+        :param endpoint: URL of the endpoint
+        :param out: output type (json or csv)
+        :param payload: payload for the request
+        :param headers: headers to use for the request
+        :param bare_url: if True, uses the endpoint as full URL (and skips base URL additions)
+        :return: API response in request.Response format
         """
         payload = payload if payload is not None else {}
         headers = headers if headers is not None else {}
         self.__log_api_io(f"GET /{endpoint} [{self.addr()}]")
 
         if bare_url:
             path = endpoint
@@ -255,19 +255,22 @@
         endpoint: str,
         out: str = "json",
         json_payload: Optional[dict[str, Any]] = None,
         headers: Optional[dict[str, Any]] = None,
         bare_url: bool = False,
     ) -> Response:
         """
+        Method to send a PUT request to the API
 
-        :param endpoint:
-        :param json_payload:
-        :param bare_url:
-        :return:
+        :param endpoint: URL of the endpoint
+        :param out: output type (json or csv)
+        :param json_payload: payload for the request
+        :param headers: headers to use for the request
+        :param bare_url: if True, uses the endpoint as full URL (and skips base URL additions)
+        :return: API response in request.Response format
         """
         json_payload = json_payload if json_payload is not None else {}
         self.__log_api_io(f"PUT /{endpoint} [{self.addr()}]")
 
         if bare_url:
             path = endpoint
         else:
@@ -290,19 +293,21 @@
         self,
         endpoint: str,
         out: str = "json",
         json_payload: Optional[dict[str, Any]] = None,
         bare_url: bool = False,
     ) -> Response:
         """
+        Method to send a POST request to the API
 
-        :param endpoint:
-        :param json_payload:
-        :param bare_url:
-        :return:
+        :param endpoint: URL of the endpoint
+        :param out: output type (json or csv)
+        :param json_payload: payload for the request
+        :param bare_url: if True, uses the endpoint as full URL (and skips base URL additions)
+        :return: API response in request.Response format
         """
         json_payload = json_payload if json_payload is not None else {}
         self.__log_api_io(f"POST /{endpoint} [{self.addr()}]")
 
         if bare_url:
             path = endpoint
         else:
@@ -413,20 +418,22 @@
     endpoint: str,
     out: str = "json",
     payload: Optional[dict[str, Any]] = None,
     headers: Optional[dict[str, Any]] = None,
     bare_url: bool = False,
 ) -> Response:
     """
+    Method to send a GET request to the API
 
-    :param endpoint:
-    :param out:
-    :param payload:
-    :param headers:
-    :return:
+    :param endpoint: URL of the endpoint
+    :param out: output type (json or csv)
+    :param payload: payload for the request
+    :param headers: headers to use for the request
+    :param bare_url: if True, uses the endpoint as full URL (and skips base URL additions)
+    :return: API response in request.Response format
     """
     return ApiSession().api_get(
         endpoint,
         out=out,
         payload=payload,
         headers=headers,
         bare_url=bare_url,
@@ -436,50 +443,53 @@
 def api_post(
     endpoint: str,
     out: str = "json",
     json_payload: Optional[dict[str, Any]] = None,
     bare_url: bool = False,
 ) -> Response:
     """
+    Method to send a POST request to the API
 
-    :param endpoint:
-    :param out:
-    :param json_payload:
-    :param headers:
-    :return:
+    :param endpoint: URL of the endpoint
+    :param out: output type (json or csv)
+    :param json_payload: payload for the request
+    :param bare_url: if True, uses the endpoint as full URL (and skips base URL addition)
+    :return: API response in request.Response format
     """
     return ApiSession().api_post(
         endpoint,
         out=out,
         json_payload=json_payload,
         bare_url=bare_url,
     )
 
 
 def api_put(
     endpoint: str, json_payload: Optional[dict[str, Any]] = None, bare_url: bool = False
 ) -> Response:
     """
+    Method to send a PUT request to the API
 
-    :param endpoint:
-    :param json_payload:
-    :return:
+    :param endpoint: URL of the endpoint
+    :param json_payload: payload for the request
+    :param bare_url: if True, uses the endpoint as full URL (and skips base URL addition)
+    :return: API response in request.Response format
     """
     return ApiSession().api_put(
         endpoint,
         out="json",
         json_payload=json_payload,
         bare_url=bare_url,
     )
 
 
 # For backwards compatibility (deprecated methods and classes)
 def set_api_url(api_url: str) -> None:
     """
     Only kept for backwards compatibility
     """
-    Logging().warning(DeprecationWarning(f"Manual update of the API url is deprecated"))
+    warn_deprecation_pending(f"Manual update of the API url is deprecated")
     ApiSession().set_api_url(api_url)
 
 
 def __enforce_imports():
     f = [APIKeyMissingError(), AccessDeniedError(), MissingConfigurationFile()]
```

### Comparing `preheat_open-1.38/preheat_open/building.py` & `preheat_open-1.39/preheat_open/building.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
-This module defines the Building class, which represents buildings containing different units and their data
+Module defining the Building class, which represents buildings containing different units and their data
 """
 import re
 from enum import Enum
 from typing import Any, Optional, Union
 
+import networkx as nx
 import pandas as pd
 
 from . import unit_graph
 from .api import AccessDeniedError, api_get
-from .backwards_compatibility import load_parameter_old_naming
+from .backwards_compatibility import load_parameter_old_naming, warn_deprecation_pending
 from .building_unit import (
     BaseBuildingUnit,
     exclude_shared_units_from_list,
     populate_units,
 )
 from .comfort_profiles import fetch_comfort_profiles
 from .data import load_model_data
@@ -27,15 +28,17 @@
 )
 from .price import SupplyPoint
 from .types import TYPE_DATETIME_INPUT
 from .unit import Unit
 from .weather import Weather
 from .zone import Zone, populate_zones, zone_matches
 
-_TOP_LEVEL_UNIT_TYPES = [  # Order is important due to cross-dependency
+# When adding new unit hierarchies, these need to be added explicitly in the list
+# WARNING: Order is important due to cross-dependency
+_TOP_LEVEL_UNIT_TYPES = [
     "main",
     "coldWater",
     "heating",
     "hotWater",
     "cooling",
     "electricity",
     "ventilation",
@@ -71,32 +74,55 @@
         # Supply points (for pricing)
         self.__supply_points = []
 
         # Load from API
         self.__populate()
 
         # Construct graph
-        self.G = unit_graph.generate_unit_graph(self)
+        self.__unit_graph = unit_graph.generate_unit_graph(self)
 
         # Traverse and map sub-unit references
-        for node, data in self.G.nodes.data():
+        for u in self.iterate_units():
             # Add sub-units as new nodes
-            if hasattr(data["unit"], "_related_sub_units_refs"):
-                for ref in data["unit"]._related_sub_units_refs:
-                    data["unit"].add_sub_unit(self.G.nodes[ref]["unit"])
-            if hasattr(data["unit"], "_related_meters_refs"):
-                for ref in data["unit"]._related_meters_refs:
-                    data["unit"]._meters.append(self.G.nodes[ref]["unit"])
+            if hasattr(u, "_related_sub_units_refs"):
+                for ref in u._related_sub_units_refs:
+                    u.add_sub_unit(self.unit_graph.nodes[ref]["unit"])
+            if hasattr(u, "_related_meters_refs"):
+                for ref in u._related_meters_refs:
+                    u._meters.append(self.unit_graph.nodes[ref]["unit"])
 
         # Devices
         self.__devices: Optional[list[Device]] = None
 
         # Comfort profiles
         self.__comfort_profile_data = None
 
+    def iterate_units(self) -> list[BaseBuildingUnit]:
+        out = [data["unit"] for node, data in self.unit_graph.nodes.data()]
+        return out
+
+    @property
+    def unit_graph(self) -> nx.MultiDiGraph:
+        return self.__unit_graph
+
+    @property
+    def G(self) -> nx.MultiDiGraph:
+        """DEPRECATED: use the 'unit_graph' attribute instead"""
+        warn_deprecation_pending(
+            "The 'G' attribute is deprecated - use the 'unit_graph' attribute instead"
+        )
+        return self.unit_graph
+
+    def get_unit_graph(self) -> nx.MultiDiGraph:
+        """DEPRECATED: use the 'unit_graph' attribute instead"""
+        warn_deprecation_pending(
+            "The 'get_unit_graph' method is deprecated - use the 'unit_graph' attribute instead"
+        )
+        return self.unit_graph
+
     def load_comfort_profile_data(
         self, start: TYPE_DATETIME_INPUT, end: TYPE_DATETIME_INPUT
     ) -> None:
         """
         Loads the comfort profile data in the building object
 
         :param start: start of the period
@@ -116,30 +142,29 @@
         self.__comfort_profile_data = None
 
     @property
     def comfort_profile_data(self) -> pd.DataFrame:
         """
         Convenience accessor to the comfort profile data for the building, if only one is defined.
 
-        Raises NoComfortProfileError if no data is loaded/available or if there are too many comfort profiles
+        :raise: NoComfortProfileError if no data is loaded/available or if there are too many comfort profiles
             for the building
         """
         return self.get_comfort_profile_data(None)
 
     def get_comfort_profile_data(
         self, comfort_profile_id: Optional[int] = None
     ) -> pd.DataFrame:
         """
         Accessor to the comfort profile data for a given comfort_profile_id.
         This requires prior loading via the *load_comfort_profile_data* method.
 
-        Raises NoComfortProfileError if no data is loaded or available
-
         :param comfort_profile_id: ID of the comfort profile, if None tries to access the only comfort profile in
             the building (for convenience in small buildings without zones) and fails if too many available
+        :raise: NoComfortProfileError if no data is loaded or available
         :return: dictionary of comfort profiles (key=comfort profile ID, value=dataframe[setpoint, min, max, value])
         """
         if self.__comfort_profile_data is None:
             raise NoComfortProfileError("No comfort profile loaded/available")
         elif comfort_profile_id is None:
             if len(self.__comfort_profile_data) == 1:
                 out = list(self.__comfort_profile_data.values())[0]
@@ -152,21 +177,14 @@
             if out is None:
                 raise NoComfortProfileError(
                     "No comfort profile available for the comfort_profile_id"
                 )
 
         return out
 
-    def get_unit_graph(self):
-        """
-
-        :return:
-        """
-        return self.G
-
     def load_data(
         self,
         start: TYPE_DATETIME_INPUT,
         end: TYPE_DATETIME_INPUT,
         resolution: Union[str, Enum] = "hour",
         components: Optional[dict[str, list[str]]] = None,
         **kwargs,
@@ -208,15 +226,15 @@
                 else:
                     [
                         u_i.load_data(start, end, resolution, components=c_i)
                         for u_i in self.query_units(unit_type=i)
                     ]
 
     def list_all_units(self) -> list[Unit]:
-        out = [self.weather] + [i[1]["unit"] for i in self.G.nodes.data()]
+        out = [self.weather] + self.iterate_units()
         return out
 
     def load_dataset(
         self,
         component_map,
         start: TYPE_DATETIME_INPUT,
         end: TYPE_DATETIME_INPUT,
@@ -246,35 +264,35 @@
     def clear_data(self) -> None:
         """
         Clears all data in the units of the object
 
         :return: /
         """
         self.weather.clear_data()
-        [data["unit"].clear_data() for node, data in self.G.nodes.data()]
+        [u.clear_data() for u in self.iterate_units()]
 
     def get_all_component_ids(self) -> dict:
         """
 
         :return:
         """
         return {
             k: v
-            for node, data in self.G.nodes.data()
-            for k, v in data["unit"].get_all_component_ids(True).items()
+            for u in self.iterate_units()
+            for k, v in u.get_all_component_ids(True).items()
         }
 
-    def get_all_component_details(self):
+    def get_all_component_details(self) -> list[dict[str, Union[str, float, None]]]:
         """
 
         :return:
         """
         all_comps = []
-        for node, data in self.G.nodes.data():
-            all_comps += data["unit"].get_all_component_details(prefix=True)
+        for u in self.iterate_units():
+            all_comps += u.get_all_component_details(prefix=True)
 
         return all_comps
 
     def query_units(
         self,
         unit_type: str = None,
         name: str = None,
@@ -287,16 +305,16 @@
         :param name:
         :param unit_id:
         :param exclude_shared: if True, excludes shared units
         :return: a list of the relevant units
         """
         # If we pass a unit ID, find specific unit
         if unit_id:
-            if unit_id in self.G.nodes.keys():
-                out = [self.G.nodes[unit_id]["unit"]]
+            if unit_id in self.unit_graph.nodes.keys():
+                out = [self.unit_graph.nodes[unit_id]["unit"]]
             else:
                 out = []
 
         else:
             # If we pass a unit_type, check if we do regex search or strict search
             if unit_type:
                 if unit_type[0] == "?":
@@ -315,32 +333,25 @@
                 else:
                     name_match = lambda n: n == name
 
             try:
                 # If we pass unit_type and name
                 if unit_type and name:
                     result = [
-                        data["unit"]
-                        for node, data in self.G.nodes.data()
-                        if name_match(data["unit"].name)
-                        and type_match(data["unit"].unit_type)
+                        u
+                        for u in self.iterate_units()
+                        if name_match(u.name) and type_match(u.unit_type)
                     ]
 
                 elif name:
-                    result = [
-                        data["unit"]
-                        for node, data in self.G.nodes.data()
-                        if name_match(data["unit"].name)
-                    ]
+                    result = [u for u in self.iterate_units() if name_match(u.name)]
 
                 elif unit_type:
                     result = [
-                        data["unit"]
-                        for node, data in self.G.nodes.data()
-                        if type_match(data["unit"].unit_type)
+                        u for u in self.iterate_units() if type_match(u.unit_type)
                     ]
 
                 out = result
 
             except Exception:
                 out = []
```

### Comparing `preheat_open-1.38/preheat_open/building_unit.py` & `preheat_open-1.39/preheat_open/building_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Module defining building units and their auxiliary methods
+"""
 from __future__ import annotations
 
 import re
 from enum import Enum
 from typing import Optional, Union
 
 from .backwards_compatibility import load_parameter_old_naming
@@ -18,31 +21,34 @@
 
 def populate_units(unit_type, units_data, building_ref):
     # Loop over units; create and populate Unit instances
     units = [BuildingUnit(unit_type, unit_i, building_ref) for unit_i in units_data]
     return units
 
 
-def add_unique_units(units, new_units, ids):
+def add_unique_units(units, new_units, ids) -> None:
     for item in new_units:
         if item.id not in ids:
             units.append(item)
             ids.append(item.id)
-    return
 
 
 def exclude_shared_units_from_list(x: list[BaseBuildingUnit]) -> list[BaseBuildingUnit]:
     return [u for u in x if not u.is_shared()]
 
 
 class BaseBuildingUnit(Unit):
     """Building Unit; an extension of Unit to handle zones and parent units"""
 
     def __init__(
-        self, unit_type: str, unit_data: dict, building_ref, load_data_by: str = "id"
+        self,
+        unit_type: str,
+        unit_data: dict[str, Union[str, float, bool, None]],
+        building_ref,
+        load_data_by: str = "id",
     ):
         super().__init__(unit_type, unit_data, load_data_by=load_data_by)
 
         # Building reference
         self.building = building_ref
 
         # Zones covered (Attempt to first extract 'zoneIds', then ['zoneId']), and couple zones
@@ -62,16 +68,16 @@
 
     def __add_zone(self, zone_id):
         self.zone_ids.append(zone_id)
         self.__zones += self.building.get_zones([zone_id])
 
     def parents(self) -> list[BaseBuildingUnit]:
         return [
-            self.building.G.nodes[item[0]]["unit"]
-            for item in self.building.G.pred[self.id].items()
+            self.building.unit_graph.nodes[item[0]]["unit"]
+            for item in self.building.unit_graph.pred[self.id].items()
         ]
 
     @property
     def weather(self) -> Weather:
         return self.building.weather
 
     # Taken from open API: building_unit.py
@@ -140,15 +146,15 @@
     def qpu(self, *args, **kwargs) -> Union[BaseBuildingUnit, list[BaseBuildingUnit]]:
         result = self.query_parent_units(*args, **kwargs)
         return convenience_result_list_shortener(result)
 
     def get_zones(self):
         return self.__zones
 
-    def query_units(self, **kwargs) -> list[BaseBuildingUnit]:
+    def query_units(self, *args, **kwargs) -> list[BaseBuildingUnit]:
         return []
 
     def qu(self, *args, **kwargs) -> Union[BaseBuildingUnit, list[BaseBuildingUnit]]:
         result = self.query_units(*args, **kwargs)
         return convenience_result_list_shortener(result)
 
     # Experimental functions below, use with care
@@ -253,16 +259,16 @@
     def clear_data(self, clear_children: bool = False) -> None:
         super().clear_data()
         if clear_children:
             [u_i.clear_data(clear_children=True) for u_i in self.children()]
 
     def children(self) -> list[BaseBuildingUnit]:
         return [
-            self.building.G.nodes[item[0]]["unit"]
-            for item in self.building.G.succ[self.id].items()
+            self.building.unit_graph.nodes[item[0]]["unit"]
+            for item in self.building.unit_graph.succ[self.id].items()
         ]
 
     def query_units(
         self,
         unit_type: Optional[str] = None,
         name: Optional[str] = None,
         exclude_shared: bool = False,
```

### Comparing `preheat_open-1.38/preheat_open/cache.py` & `preheat_open-1.39/preheat_open/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,30 +58,35 @@
     filename = __cache_filename(id, path)
     Logging().debug(f"Caching data to {filename}")
     with open(filename, "wb") as file_id:
         try:
             pickle.dump(data, file=file_id)
         except Exception as e:
             Logging().warning(
-                "Failed to cache to {} (exception: {})".format(filename, e)
+                RuntimeWarning(f"Failed to cache to {filename} (exception: {e})")
             )
 
 
 def load_from_cache(
     id: str,
     expiry_s: Optional[int] = None,
     path: str = ".cache/",
 ) -> tuple[Any, bool]:
     """
-    Loads data from the on-disk cache
+    Loads data from the on-disk cache.
+
+    WARNING: this method loads data from a file using pickle, which may execute code at the time of loading.
+        Make sure to load only files that you generated yourself or trust in order to avoid execution of malicious code.
 
     :param id: cache identifier
     :param expiry_s: acceptable lifetime of the cache (in s)
     :param path: path in which to cache the data
-    :return: tuple of data loaded from cache (or None if inexistent) and indicator of whether or not data was loaded
+    :return: tuple of:
+        data loaded from cache (or None if non-existent) and
+        indicator of whether data was loaded
     """
     filename = __cache_filename(id, path)
     if os.path.exists(filename) is False:
         data_should_be_loaded = False
     else:
         if expiry_s is None:
             data_should_be_loaded = True
@@ -98,21 +103,21 @@
 
     data = None
     data_was_loaded = False
 
     if data_should_be_loaded is True:
         with open(filename, "rb") as file_id:
             try:
-                Logging().debug("Loading data from cache in {}".format(filename))
+                Logging().debug(f"Loading data from cache in {filename}")
                 data = pickle.load(file=file_id)
                 data_was_loaded = True
             except Exception as e:
                 Logging().warning(
-                    "Failed to load from cache in {} (exception: {})".format(
-                        filename, str(e)
+                    RuntimeWarning(
+                        f"Failed to load from cache in {filename} (exception: {e})"
                     )
                 )
 
     return data, data_was_loaded
 
 
 def delete_from_cache(id: str, path: str = ".cache/") -> None:
@@ -122,9 +127,9 @@
     :param id: cache identifier
     :param path: path in which to cache the data
     :return: /
     """
 
     filename = __cache_filename(id, path)
     if os.path.exists(filename) is True:
-        Logging().debug("Deleting cache from {}".format(filename))
+        Logging().debug(f"Deleting cache from {filename}")
         os.remove(filename)
```

### Comparing `preheat_open-1.38/preheat_open/comfort_profiles.py` & `preheat_open-1.39/preheat_open/comfort_profiles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-"""
-Module to manage the comfort profiles
-"""
-import pandas as pd
-
-from .api import api_get, datetime_to_api_string
-from .exceptions import NoComfortProfileError
-from .helpers import sanitise_datetime_input
-from .types import TYPE_DATETIME_INPUT
-
-
-def fetch_comfort_profiles(
-    location_id: int,
-    start: TYPE_DATETIME_INPUT,
-    end: TYPE_DATETIME_INPUT,
-) -> dict[int, pd.DataFrame]:
-    """
-    Get target temperature using API call
-    """
-    start = sanitise_datetime_input(start)
-    end = sanitise_datetime_input(end)
-    package = api_get(
-        f"locations/{location_id}/comfortprofile/setpoints",
-        payload={
-            "start_time": datetime_to_api_string(start),
-            "end_time": datetime_to_api_string(end),
-        },
-        out="json",
-    )["comfortProfiles"]
-    if not package:
-        raise NoComfortProfileError(
-            "No comfort profile available for location in period"
-        )
-
-    data = {}
-    for comfort_profile in package:
-        zdf = pd.DataFrame(comfort_profile["setpoints"]).set_index("time")
-        zdf.index = pd.DatetimeIndex(zdf.index)
-        comfort_profile_id = comfort_profile["id"]
-
-        # Fixing API issue by cropping the data to the focus period
-        data[comfort_profile_id] = zdf[start:end]
-
-    return data
+"""
+Module to manage the comfort profiles
+"""
+import pandas as pd
+
+from .api import api_get, datetime_to_api_string
+from .exceptions import NoComfortProfileError
+from .helpers import sanitise_datetime_input
+from .types import TYPE_DATETIME_INPUT
+
+
+def fetch_comfort_profiles(
+    location_id: int,
+    start: TYPE_DATETIME_INPUT,
+    end: TYPE_DATETIME_INPUT,
+) -> dict[int, pd.DataFrame]:
+    """
+    Get target temperature using API call
+    """
+    start = sanitise_datetime_input(start)
+    end = sanitise_datetime_input(end)
+    package = api_get(
+        f"locations/{location_id}/comfortprofile/setpoints",
+        payload={
+            "start_time": datetime_to_api_string(start),
+            "end_time": datetime_to_api_string(end),
+        },
+        out="json",
+    )["comfortProfiles"]
+    if not package:
+        raise NoComfortProfileError(
+            "No comfort profile available for location in period"
+        )
+
+    data = {}
+    for comfort_profile in package:
+        zdf = pd.DataFrame(comfort_profile["setpoints"]).set_index("time")
+        zdf.index = pd.DatetimeIndex(zdf.index)
+        zdf["name"] = comfort_profile["name"]
+        comfort_profile_id = comfort_profile["id"]
+
+        # Fixing API issue by cropping the data to the focus period
+        data[comfort_profile_id] = zdf[start:end]
+
+    return data
```

### Comparing `preheat_open-1.38/preheat_open/control_unit.py` & `preheat_open-1.39/preheat_open/setpoints.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,67 @@
-"""
-Management control units and scheduling
-"""
-from typing import Any
-
-import numpy as np
 import pandas as pd
+from requests import HTTPError
 from requests.models import Response
 
-from .building_unit import BaseBuildingUnit
-from .helpers import check_no_remaining_fields
-from .logging import Logging
-from .setpoints import (
-    InvalidScheduleError,
-    get_setpoint_schedule,
-    send_setpoint_schedule,
-)
+from .api import TIMEZONE, api_get, api_put
+from .exceptions import InvalidSchedule  # For backwards compatibility
+from .exceptions import InvalidScheduleError
+from .helpers import sanitise_datetime_input
 from .types import TYPE_DATETIME_INPUT
 
 
-def validate_schedule(schedule_df: pd.DataFrame) -> None:
-    if schedule_df["value"].isnull().any():
-        raise InvalidScheduleError("requested schedule has missing values")
-    if np.isinf(schedule_df["value"]).any():
-        raise InvalidScheduleError("requested schedule has infinite values")
-    if schedule_df.empty or (len(schedule_df) == 0):
-        raise InvalidScheduleError(
-            "An empty schedule_df was requested (the API does not accept this)"
-        )
-
+def send_setpoint_schedule(controlunit_id: int, schedule_df: pd.DataFrame) -> Response:
+    path = f"controlunit/{controlunit_id}/setpoint"
 
-class ControlUnit(BaseBuildingUnit):
-    """Control Unit; an extension of Unit to handle controls"""
+    # Build payload from DataFrame
+    payload = {"schedule": []}
+    if "operation" not in schedule_df.keys():
+        schedule_df["operation"] = len(schedule_df) * ["NORMAL"]
+
+    [
+        payload["schedule"].append(
+            {
+                "startTime": index.isoformat(),
+                "value": row["value"],
+                "operation": row["operation"],
+            }
+        )
+        for index, row in schedule_df.iterrows()
+    ]
 
-    def __init__(self, unit_data: dict[str, Any], building_ref=None):
-        super().__init__("control", unit_data, building_ref)
-        if "active" in unit_data.keys():
-            self.active = unit_data.pop("active")
-        else:
-            self.active = False
-
-        check_no_remaining_fields(unit_data, debug_helper="control_unit_data")
-
-    def request_schedule(self, schedule_df: pd.DataFrame) -> Response:
-        if self.active is False:
-            Logging().warning(
-                RuntimeWarning(
-                    """Warning: you are trying to control an unit that is not activated 
-                    (id={} / details: [unit: {} / building: [{}] {}])""".format(
-                        self.id,
-                        self.name,
-                        self.building.location["locationId"],
-                        self.building.location["address"],
-                    )
-                )
-            )
-        validate_schedule(schedule_df)
-        return send_setpoint_schedule(self.id, schedule_df)
-
-    def get_schedule(
-        self, start_date: TYPE_DATETIME_INPUT, end_date: TYPE_DATETIME_INPUT
-    ) -> pd.DataFrame:
-        return get_setpoint_schedule(self.id, start_date, end_date)
+    try:
+        # PUT request
+        return api_put(path, json_payload=payload)
+    except HTTPError as e:
+        extra_info = f"""HTTP error when writing the schedule: 
+            {str(payload["schedule"])}
+            
+            Details: {e}"""
+        raise InvalidScheduleError(extra_info) from e
+
+
+def get_setpoint_schedule(
+    controlunit_id: int, start_date: TYPE_DATETIME_INPUT, end_date: TYPE_DATETIME_INPUT
+) -> pd.DataFrame:
+    start_date = sanitise_datetime_input(start_date)
+    end_date = sanitise_datetime_input(end_date)
+
+    path = f"controlunit/{controlunit_id}/setpoint"
+
+    payload = {
+        "start_time": start_date.isoformat(),
+        "end_time": end_date.isoformat(),
+    }
+
+    raw = api_get(path, out="json", payload=payload)
+    df = pd.DataFrame(raw)
+
+    if df.empty:
+        return df
+
+    df["startTime"] = pd.to_datetime(df["startTime"], utc=True)
+    return df.set_index("startTime")
+
+
+# For backwards compatibility
+def __enforce_imports():
+    d = [InvalidSchedule(), TIMEZONE]
```

### Comparing `preheat_open-1.38/preheat_open/data.py` & `preheat_open-1.39/preheat_open/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 To manage timeseries data loading
 """
 import math
 from datetime import datetime, timedelta
 from functools import reduce
-from typing import Optional
+from typing import Any, Optional
 
 import numpy as np
 import pandas as pd
 
 from .api import (
     DATETIME_FORMAT,
     MAX_IDS_AND_CIDS_PER_REQUEST,
@@ -20,21 +20,28 @@
 from .helpers import list_to_string, sanitise_datetime_input
 from .types import TYPE_DATETIME_INPUT
 
 __DEFAULT_DATAFRAME_INDEX = pd.DatetimeIndex([], tz="UTC")
 
 
 def load_box_data(
-    component_map,
+    component_map: dict[str, Any],
     start: TYPE_DATETIME_INPUT,
     end: TYPE_DATETIME_INPUT,
     resolution="minute",
 ) -> pd.DataFrame:
-    # Parse strings to datetime object
+    """
+    Loads box data from the API
 
+    :param component_map: mapping of the components to load data for
+    :param start: start of the period
+    :param end: end of the period
+    :param resolution: resolution to load data with (raw, minute/5min, hour , day, week, month, year)
+    :return: data in Dataframe format
+    """
     start = sanitise_datetime_input(start)
     end = sanitise_datetime_input(end)
     __check_start_end_date(start, end)
 
     path = "measurements"
     cid_key = "cids"
     cids = list(component_map.keys())
@@ -44,20 +51,28 @@
 
     resp = __perform_requests(path, cid_key, cids, start, end, resolution, "csv")
 
     return __extract_data(resp, "cid", component_map, "csv").astype(float)
 
 
 def load_model_data(
-    component_map,
+    component_map: dict[str, Any],
     start: TYPE_DATETIME_INPUT,
     end: TYPE_DATETIME_INPUT,
     resolution="raw",
 ) -> pd.DataFrame:
-    # Parse strings to datetime object
+    """
+    Loads data using a building model representation
+
+    :param component_map: mapping of the components
+    :param start: start of the period
+    :param end: end of the period
+    :param resolution: resolution of the data (raw, minute/5min, hour, day, week, month, year)
+    :return: data loaded in dataFrame format
+    """
     start = sanitise_datetime_input(start)
     end = sanitise_datetime_input(end)
     __check_start_end_date(start, end)
 
     path = "units/measurements"
     id_key = "ids"
     ids = list(component_map.keys())
@@ -72,21 +87,33 @@
         # Do single request
         resp = __make_request(path, {id_key: ids}, start, end, resolution, "csv")
 
     return __extract_data(resp, "id", component_map, "csv").astype(float)
 
 
 def load_weather_data(
-    location_id,
-    component_map,
+    location_id: int,
+    component_map: dict[str, Any],
     start: TYPE_DATETIME_INPUT,
     end: TYPE_DATETIME_INPUT,
     resolution: str = "hour",
-    components=None,
+    **kwargs,
 ) -> pd.DataFrame:
+    """
+    Loads weather data from the API
+
+    :param location_id: location ID
+    :param component_map: mapping of the components
+    :param start: start of the period
+    :param end: end of the period
+    :param resolution: resolution of the data (raw, minute/5min, hour, day, week, month, year)
+        Note: raw, minute/5min are overwritten to hour
+    :param kwargs: /
+    :return: loaded data in DataFrame format
+    """
     # Parse strings to datetime object
     start = sanitise_datetime_input(start)
     end = sanitise_datetime_input(end)
     __check_start_end_date(start, end)
 
     path = f"weather/{location_id}"
     cid_key = "type_ids"
@@ -198,15 +225,15 @@
         resolution = "minute"
 
     payload["time_resolution"] = resolution
 
     return api_get(path, payload=payload, out=format)
 
 
-def extract_data(resp, id_key, component_map, format="csv"):
+def extract_data(resp, id_key, component_map, format: str = "csv"):
     return __extract_data(resp, id_key, component_map, format)
 
 
 def __reformat_dataframe(
     resp: pd.DataFrame,
     component_map: dict[str, str],
     id_key: Optional[str] = None,
```

### Comparing `preheat_open-1.38/preheat_open/exceptions.py` & `preheat_open-1.39/preheat_open/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 
 class InvalidSchedule(Exception):
     pass
 
 
 # / backwards compatibility
+class NotFoundError(Exception):
+    pass
 
 
 class APIKeyMissingError(Exception):
     pass
 
 
 class AccessDeniedError(Exception):
```

### Comparing `preheat_open-1.38/preheat_open/price.py` & `preheat_open-1.39/preheat_open/price.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,25 +163,27 @@
                                 )
                             )
                             df_i["price"] = row_ij["price"][0]
 
                         if df_price_raw_i is None:
                             df_price_raw_i = df_i.ffill()
                         else:
-                            df_price_raw_i = df_price_raw_i.append(df_i.ffill())
+                            df_price_raw_i = pd.concat(
+                                [df_price_raw_i, df_i.ffill()], axis=0
+                            )
 
                 df_price_i = df_price_raw_i[["price"]]
 
             elif (pc_ki["timeSeriesData"] is not None) and (
                 len(pc_ki["timeSeriesData"]) > 0
             ):
                 df_price_i = pd.DataFrame(pc_ki["timeSeriesData"])
                 if len(df_price_i) > 0:
                     df_price_i.set_index(
-                        pd.to_datetime(df_price_i["time"], infer_datetime_format=True),
+                        pd.to_datetime(df_price_i["time"]),
                         inplace=True,
                     )
                     df_price_i.drop(columns=["time"], inplace=True)
                 else:
                     df_price_i = None
 
             else:
```

### Comparing `preheat_open-1.38/preheat_open/test/__init__.py` & `preheat_open-1.39/preheat_open/test/__init__.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/conftest.py` & `preheat_open-1.39/preheat_open/test/conftest.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from copy import deepcopy
-
-import pytest
-
-import preheat_open
-from preheat_open.test import (
-    API_KEY,
-    MEDIUM_TEST_PERIOD,
-    SHORT_TEST_PERIOD,
-    TEST_LOCATION_ID,
-    mark_pytest_package_test,
-)
-
-# Defining fixture scope
-FIXTURE_SCOPE = "session"
-
-
-# Fixing API key once and for all
-@pytest.fixture(autouse=True)
-def mark_as_pytest_run():
-    mark_pytest_package_test()
-
-
-@pytest.fixture(autouse=True)
-def set_api_key():
-    preheat_open.api.set_api_key(API_KEY)
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def medium_period():
-    return MEDIUM_TEST_PERIOD
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def short_period():
-    return SHORT_TEST_PERIOD
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def building():
-    return preheat_open.Building(TEST_LOCATION_ID)
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def building_with_devices(building):
-    b = deepcopy(building)
-    b.load_devices()
-    return b
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def building_with_data(building, medium_period):
-    building_new = deepcopy(building)
-    building_new.load_data(*medium_period)
-    return building_new
-
-
-# Legacy fixtures
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def building_id():
-    return TEST_LOCATION_ID
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def unit_id():
-    return 15312
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def control_unit_id():
-    return 15357
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def unit(building, unit_id):
-    return building.query_units(unit_id=unit_id)[0]
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def unit_with_data(unit, medium_period):
-    unit_new = deepcopy(unit)
-    unit_new.load_data(*medium_period)
-    return unit_new
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def control_unit(building):
-    return building.qu("control", "control_unit_custom_1")
-
-
-@pytest.fixture(scope=FIXTURE_SCOPE)
-def weather_unit(building):
-    return building.weather
+from copy import deepcopy
+
+import pytest
+
+import preheat_open
+from preheat_open.test import (
+    API_KEY,
+    MEDIUM_TEST_PERIOD,
+    SHORT_TEST_PERIOD,
+    TEST_LOCATION_ID,
+    mark_pytest_package_test,
+)
+
+# Defining fixture scope
+FIXTURE_SCOPE = "session"
+
+
+# Fixing API key once and for all
+@pytest.fixture(autouse=True)
+def mark_as_pytest_run():
+    mark_pytest_package_test()
+
+
+@pytest.fixture(autouse=True)
+def set_api_key():
+    preheat_open.api.set_api_key(API_KEY)
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def medium_period():
+    return MEDIUM_TEST_PERIOD
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def short_period():
+    return SHORT_TEST_PERIOD
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def building():
+    return preheat_open.Building(TEST_LOCATION_ID)
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def building_with_devices(building):
+    b = deepcopy(building)
+    b.load_devices()
+    return b
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def building_with_data(building, medium_period):
+    building_new = deepcopy(building)
+    building_new.load_data(*medium_period)
+    return building_new
+
+
+# Legacy fixtures
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def building_id():
+    return TEST_LOCATION_ID
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def unit_id():
+    return 15312
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def control_unit_id():
+    return 15357
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def unit(building, unit_id):
+    return building.query_units(unit_id=unit_id)[0]
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def unit_with_data(unit, medium_period):
+    unit_new = deepcopy(unit)
+    unit_new.load_data(*medium_period)
+    return unit_new
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def control_unit(building):
+    return building.qu("control", "control_unit_custom_1")
+
+
+@pytest.fixture(scope=FIXTURE_SCOPE)
+def weather_unit(building):
+    return building.weather
```

### Comparing `preheat_open-1.38/preheat_open/test/test_anonymisation.py` & `preheat_open-1.39/preheat_open/test/test_anonymisation.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_api.py` & `preheat_open-1.39/preheat_open/test/test_api.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_backwards_compatibility.py` & `preheat_open-1.39/preheat_open/test/test_backwards_compatibility.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_building.py` & `preheat_open-1.39/preheat_open/test/test_building.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,106 +1,109 @@
-from copy import deepcopy
-
-import pandas as pd
-
-from preheat_open import test
-from preheat_open.weather import Weather
-
-
-class TestBuilding(test.PreheatTest):
-    def test_building(self, building):
-        assert building is not None
-        assert building.weather is not None
-        assert isinstance(building.weather, Weather)
-        assert building.units is not None
-        assert len(building.units) > 0
-        assert building.units["heating"] is not None
-
-    def test_query_units(self, building, unit_id):
-        assert building.query_units(unit_id=unit_id) is not None
-        assert building.query_units("heating") is not None
-        assert building.query_units("heating", exclude_shared=True) is not None
-        assert building.query_units("?h") is not None
-        assert building.query_units("?ting") is not None
-        assert building.qu(name="heating_primary") is not None
-
-        assert building.query_units("definitely not there") is not None
-        assert len(building.query_units("definitely not there")) == 0
-        assert building.qu(name="definitely not there") is None
-        assert building.qu(unit_id="definitely not there") is None
-
-    def test_get_unit_graph(self, building):
-        assert building.get_unit_graph() is not None
-
-    def test_clear_data(self, building_with_data):
-        from copy import deepcopy
-
-        building_new = deepcopy(building_with_data)
-        building_new.clear_data()
-        assert building_new.weather is not None
-        assert building_new.weather.data is not None
-        assert building_new.weather.data.empty
-
-    def test_load_data(self, building_with_data, short_period):
-        # Testing standard data loading
-        assert building_with_data is not None
-        assert building_with_data.weather is not None
-        assert building_with_data.weather.data is not None
-        assert not building_with_data.weather.data.empty
-
-        # Testing selective data loading
-        new_building_with_data = deepcopy(building_with_data)
-        new_building_with_data.clear_data()
-        comps = {
-            "weather": ["Temperature", "Humidity"],
-            "main": None,
-            "secondaries": ["supplyT"],
-        }
-        new_building_with_data.load_data(*short_period, components=comps)
-
-        df_weather = new_building_with_data.weather.data
-        df_main = new_building_with_data.query_units("main")[0].data
-        df_secondary = new_building_with_data.query_units("secondaries")[0].data
-
-        assert df_weather.empty is False
-        assert "Temperature" in df_weather
-        assert "Humidity" in df_weather
-        assert "WindSpeed" not in df_weather
-
-        assert df_main.empty is False
-
-        assert df_secondary.empty is False
-        assert "supplyT" in df_secondary
-        assert "returnT" not in df_secondary
-
-        assert new_building_with_data.query_units("indoorClimate")[0].data.empty is True
-        assert new_building_with_data.query_units("heating")[0].data.empty is True
-
-    def test_get_sub_zones(self, building_with_data):
-        assert building_with_data.get_zones([]) == []
-        assert len(building_with_data.get_zones([1])) == 0
-        assert len(building_with_data.get_zones([4830])) == 1
-        assert len(building_with_data.get_zones([4830, 4834])) == 2
-        assert len(building_with_data.query_zones(zone_id=0)) == 0
-        assert len(building_with_data.query_zones(zone_id=4830)) == 1
-        assert len(building_with_data.query_zones(zone_type="apartment")) >= 1
-        assert (
-            len(building_with_data.query_zones(zone_id=4830, zone_type="apartment"))
-            == 1
-        )
-        assert (
-            len(building_with_data.query_zones(zone_id=4830, zone_type="doesnt exist"))
-            == 0
-        )
-        assert len(building_with_data.query_zones(zone_type="doesnt exist")) == 0
-
-    def test_describe(self, building_with_devices):
-        assert isinstance(building_with_devices.describe(display=False), str)
-        assert isinstance(building_with_devices.describe_devices(display=False), str)
-
-
-def test_available_buildings():
-    from preheat_open.building import available_buildings
-
-    df = available_buildings()
-    assert isinstance(df, pd.DataFrame)
-    assert len(df) == 1, "The API key has access to too many buildings"
+from copy import deepcopy
+
+import networkx as nx
+import pandas as pd
+
+from preheat_open import test
+from preheat_open.weather import Weather
+
+
+class TestBuilding(test.PreheatTest):
+    def test_building(self, building):
+        assert building is not None
+        assert building.weather is not None
+        assert isinstance(building.weather, Weather)
+        assert building.units is not None
+        assert len(building.units) > 0
+        assert building.units["heating"] is not None
+
+    def test_query_units(self, building, unit_id):
+        assert building.query_units(unit_id=unit_id) is not None
+        assert building.query_units("heating") is not None
+        assert building.query_units("heating", exclude_shared=True) is not None
+        assert building.query_units("?h") is not None
+        assert building.query_units("?ting") is not None
+        assert building.qu(name="heating_primary") is not None
+
+        assert building.query_units("definitely not there") is not None
+        assert len(building.query_units("definitely not there")) == 0
+        assert building.qu(name="definitely not there") is None
+        assert building.qu(unit_id="definitely not there") is None
+
+    def test_unit_graph(self, building):
+        g = building.unit_graph
+        assert g is not None
+        assert isinstance(g, nx.MultiDiGraph)
+
+    def test_clear_data(self, building_with_data):
+        from copy import deepcopy
+
+        building_new = deepcopy(building_with_data)
+        building_new.clear_data()
+        assert building_new.weather is not None
+        assert building_new.weather.data is not None
+        assert building_new.weather.data.empty
+
+    def test_load_data(self, building_with_data, short_period):
+        # Testing standard data loading
+        assert building_with_data is not None
+        assert building_with_data.weather is not None
+        assert building_with_data.weather.data is not None
+        assert not building_with_data.weather.data.empty
+
+        # Testing selective data loading
+        new_building_with_data = deepcopy(building_with_data)
+        new_building_with_data.clear_data()
+        comps = {
+            "weather": ["Temperature", "Humidity"],
+            "main": None,
+            "secondaries": ["supplyT"],
+        }
+        new_building_with_data.load_data(*short_period, components=comps)
+
+        df_weather = new_building_with_data.weather.data
+        df_main = new_building_with_data.query_units("main")[0].data
+        df_secondary = new_building_with_data.query_units("secondaries")[0].data
+
+        assert df_weather.empty is False
+        assert "Temperature" in df_weather
+        assert "Humidity" in df_weather
+        assert "WindSpeed" not in df_weather
+
+        assert df_main.empty is False
+
+        assert df_secondary.empty is False
+        assert "supplyT" in df_secondary
+        assert "returnT" not in df_secondary
+
+        assert new_building_with_data.query_units("indoorClimate")[0].data.empty is True
+        assert new_building_with_data.query_units("heating")[0].data.empty is True
+
+    def test_get_sub_zones(self, building_with_data):
+        assert building_with_data.get_zones([]) == []
+        assert len(building_with_data.get_zones([1])) == 0
+        assert len(building_with_data.get_zones([4830])) == 1
+        assert len(building_with_data.get_zones([4830, 4834])) == 2
+        assert len(building_with_data.query_zones(zone_id=0)) == 0
+        assert len(building_with_data.query_zones(zone_id=4830)) == 1
+        assert len(building_with_data.query_zones(zone_type="apartment")) >= 1
+        assert (
+            len(building_with_data.query_zones(zone_id=4830, zone_type="apartment"))
+            == 1
+        )
+        assert (
+            len(building_with_data.query_zones(zone_id=4830, zone_type="doesnt exist"))
+            == 0
+        )
+        assert len(building_with_data.query_zones(zone_type="doesnt exist")) == 0
+
+    def test_describe(self, building_with_devices):
+        assert isinstance(building_with_devices.describe(display=False), str)
+        assert isinstance(building_with_devices.describe_devices(display=False), str)
+
+
+def test_available_buildings():
+    from preheat_open.building import available_buildings
+
+    df = available_buildings()
+    assert isinstance(df, pd.DataFrame)
+    assert len(df) == 1, "The API key has access to too many buildings"
```

### Comparing `preheat_open-1.38/preheat_open/test/test_building_unit.py` & `preheat_open-1.39/preheat_open/test/test_building_unit.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_cache.py` & `preheat_open-1.39/preheat_open/test/test_cache.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import os
-import uuid
-
-from preheat_open.cache import delete_from_cache, load_from_cache, save_to_cache
-from preheat_open.logging import Logging
-
-
-def test_caching():
-    try:
-        os.chdir("/tmp")
-    except Exception as e:
-        Logging().warning(
-            "Failed to change dir to /tmp (maybe you are on Windows) // Error: "
-            + str(e)
-        )
-
-    a = "This is a test cache content"
-    id = "test_cache"
-    path_out = ".preheat_test_cache_" + str(uuid.uuid4())
-
-    delete_from_cache(id, path=path_out)
-    __, nok = load_from_cache(id)
-    assert nok is False
-
-    save_to_cache(a, id, path=path_out)
-    a_cached, ok = load_from_cache(id, path=path_out)
-    assert ok is True
-    assert a_cached == a
-
-    delete_from_cache(id, path=path_out)
-    no_data, nok = load_from_cache(id, path=path_out)
-    assert nok is False
-
-    delete_from_cache(id, path=path_out)
-    save_to_cache(a, id, path=path_out)
-    a_cached, ok = load_from_cache(id, path=path_out)
-    assert ok is True
-    assert a_cached == a
-    delete_from_cache(id, path=path_out)
-
-    os.rmdir(path_out)
+import os
+import uuid
+
+from preheat_open.cache import delete_from_cache, load_from_cache, save_to_cache
+from preheat_open.logging import Logging
+
+
+def test_caching():
+    try:
+        os.chdir("/tmp")
+    except Exception as e:
+        Logging().warning(
+            "Failed to change dir to /tmp (maybe you are on Windows) // Error: "
+            + str(e)
+        )
+
+    a = "This is a test cache content"
+    id = "test_cache"
+    path_out = ".preheat_test_cache_" + str(uuid.uuid4())
+
+    delete_from_cache(id, path=path_out)
+    __, nok = load_from_cache(id)
+    assert nok is False
+
+    save_to_cache(a, id, path=path_out)
+    a_cached, ok = load_from_cache(id, path=path_out)
+    assert ok is True
+    assert a_cached == a
+
+    delete_from_cache(id, path=path_out)
+    no_data, nok = load_from_cache(id, path=path_out)
+    assert nok is False
+
+    delete_from_cache(id, path=path_out)
+    save_to_cache(a, id, path=path_out)
+    a_cached, ok = load_from_cache(id, path=path_out)
+    assert ok is True
+    assert a_cached == a
+    delete_from_cache(id, path=path_out)
+
+    os.rmdir(path_out)
```

### Comparing `preheat_open-1.38/preheat_open/test/test_control_unit.py` & `preheat_open-1.39/preheat_open/test/test_control_unit.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_data.py` & `preheat_open-1.39/preheat_open/test/test_data.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_device.py` & `preheat_open-1.39/preheat_open/test/test_device.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_helpers.py` & `preheat_open-1.39/preheat_open/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_import.py` & `preheat_open-1.39/preheat_open/test/test_import.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_price.py` & `preheat_open-1.39/preheat_open/test/test_price.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_unit.py` & `preheat_open-1.39/preheat_open/test/test_unit.py`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/preheat_open/test/test_weather.py` & `preheat_open-1.39/preheat_open/test/test_weather.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from copy import deepcopy
-
-import pandas as pd
-import pytest
-
-from preheat_open import test
-
-
-class TestBuilding(test.PreheatTest):
-    def test_load_data(self, weather_unit, short_period):
-        weather_unit.load_data(*short_period)
-        assert weather_unit is not None
-        assert weather_unit.data is not None
-        assert not weather_unit.data.empty
-        assert weather_unit.has_data()
-        print(weather_unit.data)
-        assert weather_unit.has_data("Temperature")
-        with pytest.warns(Warning):
-            weather_unit.load_data(*short_period)
-            assert not weather_unit.data.empty
-
-    def test_clear_data(self, weather_unit, short_period):
-        weather_unit2 = deepcopy(weather_unit)
-        weather_unit2.load_data(*short_period)
-        weather_unit2.clear_data()
-        assert weather_unit2.data is not None
-        assert weather_unit2.data.empty
-
-    def test_selected_data_loading(self, weather_unit, unit, short_period):
-        weather_unit.load_data(*short_period, components=["Temperature", "LowClouds"])
-        assert weather_unit.data is not None
-        assert not weather_unit.data.empty
-        assert "Temperature" in weather_unit.data.keys()
-        assert "LowClouds" in weather_unit.data.keys()
-        assert "Humidity" not in weather_unit.data.keys()
-        assert "Fog" not in weather_unit.data.keys()
-
-    def test_get_state(self, weather_unit):
-        sw1 = weather_unit.get_state(
-            update=True, estimate="last", seconds_back=12 * 3600
-        )
-        sw2 = weather_unit.get_state(update=False, estimate="median")
-        sw3 = weather_unit.get_state(update=False, estimate="mean")
-        assert isinstance(sw1, pd.Series)
-        assert isinstance(sw2, pd.Series)
-        assert isinstance(sw3, pd.Series)
-
-        # The location does not get new data
-        assert len(sw1) > 0
-        assert len(sw2) > 0
-        assert len(sw3) > 0
-        weather_unit.clear_state()
+from copy import deepcopy
+
+import pandas as pd
+import pytest
+
+from preheat_open import test
+
+
+class TestBuilding(test.PreheatTest):
+    def test_load_data(self, weather_unit, short_period):
+        weather_unit.load_data(*short_period)
+        assert weather_unit is not None
+        assert weather_unit.data is not None
+        assert not weather_unit.data.empty
+        assert weather_unit.has_data()
+        print(weather_unit.data)
+        assert weather_unit.has_data("Temperature")
+        with pytest.warns(Warning):
+            weather_unit.load_data(*short_period)
+            assert not weather_unit.data.empty
+
+    def test_clear_data(self, weather_unit, short_period):
+        weather_unit2 = deepcopy(weather_unit)
+        weather_unit2.load_data(*short_period)
+        weather_unit2.clear_data()
+        assert weather_unit2.data is not None
+        assert weather_unit2.data.empty
+
+    def test_selected_data_loading(self, weather_unit, unit, short_period):
+        weather_unit.load_data(*short_period, components=["Temperature", "LowClouds"])
+        assert weather_unit.data is not None
+        assert not weather_unit.data.empty
+        assert "Temperature" in weather_unit.data.keys()
+        assert "LowClouds" in weather_unit.data.keys()
+        assert "Humidity" not in weather_unit.data.keys()
+        assert "Fog" not in weather_unit.data.keys()
+
+    def test_get_state(self, weather_unit):
+        sw1 = weather_unit.get_state(
+            update=True, estimate="last", seconds_back=12 * 3600
+        )
+        sw2 = weather_unit.get_state(update=False, estimate="median")
+        sw3 = weather_unit.get_state(update=False, estimate="mean")
+        assert isinstance(sw1, pd.Series)
+        assert isinstance(sw2, pd.Series)
+        assert isinstance(sw3, pd.Series)
+
+        # The location does not get new data
+        assert len(sw1) > 0
+        assert len(sw2) > 0
+        assert len(sw3) > 0
+        weather_unit.clear_state()
```

### Comparing `preheat_open-1.38/preheat_open/test/test_zone.py` & `preheat_open-1.39/preheat_open/test/test_zone.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import pandas as pd
-import pytest
-from pandas.util.testing import assert_frame_equal
-
-from preheat_open import test
-from preheat_open.exceptions import NoComfortProfileError
-
-
-class TestBuilding(test.PreheatTest):
-    def test_zone_type(self, building):
-        apt_zone = building.get_zones(zone_ids=[4832])[0]
-        wet_zone = building.get_zones(zone_ids=[4833])[0]
-        dry_zone = building.get_zones(zone_ids=[4835])[0]
-
-        type_1, wet_or_dry_1 = apt_zone.get_type()
-        assert type_1 == "apartment"
-        assert wet_or_dry_1 == "?"
-
-        type_a, wet_or_dry_a = wet_zone.get_type()
-        assert type_a == "bathroom"
-        assert wet_or_dry_a == "wet"
-
-        type_b, wet_or_dry_b = dry_zone.get_type()
-        assert type_b == "corridor"
-        assert wet_or_dry_b == "dry"
-
-    def query_zones(self, building):
-        z = building.query_zones(zone_id=4832, zone_type="apartment")[0]
-        assert len(z.query_zones(zone_id=4833)) == 1
-        assert len(z.query_zones(zone_type="bathroom")) == 1
-        assert len(z.query_zones(zone_id=4833, zone_type="bathroom")) == 1
-
-        assert len(z.query_zones(zone_id=4833, zone_type="apartment")) == 0
-        assert len(z.query_zones(zone_type="doesnt exist")) == 0
-        assert len(z.query_zones(zone_id=0)) == 0
-
-    def test_get_units(self, building_with_data):
-        # Zone A1 -- connected to unit named 'indoor_climate_1'
-        zone_A1 = building_with_data.get_zones(zone_ids=[4830])[0]
-        units_A1 = zone_A1.get_units("indoorClimate")
-        assert units_A1[0] == building_with_data.qu(name="indoor_climate_1")
-        zone_A1b = building_with_data.get_zone(id=4830)
-        assert zone_A1 == zone_A1b
-
-        # Zone A2 -- not connected to any units
-        zone_A2 = building_with_data.get_zones(zone_ids=[4831])[0]
-        units_A2 = zone_A2.get_units("indoorClimate")
-        assert not units_A2
-
-        zone_A = zone_A1b.get_parent_zone()
-        assert zone_A.get_parent_zone() is None
-        assert len(zone_A.get_units("indoorClimate")) > 0
-
-    def test_comfort_profiles(self, building):
-        # Zone A1 -- connected to unit named 'indoor_climate_1'
-        zone_A1 = building.get_zones(zone_ids=[4830])[0]
-
-        start_cp = "2023-01-05"
-        end_cp = "2023-01-06"
-        zone_A1.load_comfort_profile_data(start_cp, end_cp)
-
-        df_cp = zone_A1.comfort_profile_data
-        assert isinstance(df_cp, pd.DataFrame)
-        assert 23 <= len(df_cp) <= 25
-
-        df_cp2 = zone_A1.sub_zones[0].comfort_profile_data
-        assert isinstance(df_cp2, pd.DataFrame)
-        assert_frame_equal(df_cp, df_cp2)
-
-        with pytest.raises(NoComfortProfileError):
-            zone_A1.get_parent_zone().comfort_profile_data
-
-    def test_get_unit_types(self, building_with_data):
-        # Zone A1 -- connected to unit named 'indoor_climate_1'
-        zone_A1 = building_with_data.get_zones(zone_ids=[4830])[0]
-        types_A1 = zone_A1.get_unit_types()
-        assert isinstance(types_A1, list)
-        for t in types_A1:
-            assert isinstance(t, str)
-
-        # Zone A2 -- not connected to any units
-        zone_A2 = building_with_data.get_zones(zone_ids=[4831])[0]
-        types_A2 = zone_A2.get_unit_types()
-        assert isinstance(types_A2, list)
-        assert not types_A2
+import pandas as pd
+import pytest
+from pandas.testing import assert_frame_equal
+
+from preheat_open import test
+from preheat_open.exceptions import NoComfortProfileError
+
+
+class TestBuilding(test.PreheatTest):
+    def test_zone_type(self, building):
+        apt_zone = building.get_zones(zone_ids=[4832])[0]
+        wet_zone = building.get_zones(zone_ids=[4833])[0]
+        dry_zone = building.get_zones(zone_ids=[4835])[0]
+
+        type_1, wet_or_dry_1 = apt_zone.get_type()
+        assert type_1 == "apartment"
+        assert wet_or_dry_1 == "?"
+
+        type_a, wet_or_dry_a = wet_zone.get_type()
+        assert type_a == "bathroom"
+        assert wet_or_dry_a == "wet"
+
+        type_b, wet_or_dry_b = dry_zone.get_type()
+        assert type_b == "corridor"
+        assert wet_or_dry_b == "dry"
+
+    def query_zones(self, building):
+        z = building.query_zones(zone_id=4832, zone_type="apartment")[0]
+        assert len(z.query_zones(zone_id=4833)) == 1
+        assert len(z.query_zones(zone_type="bathroom")) == 1
+        assert len(z.query_zones(zone_id=4833, zone_type="bathroom")) == 1
+
+        assert len(z.query_zones(zone_id=4833, zone_type="apartment")) == 0
+        assert len(z.query_zones(zone_type="doesnt exist")) == 0
+        assert len(z.query_zones(zone_id=0)) == 0
+
+    def test_get_units(self, building_with_data):
+        # Zone A1 -- connected to unit named 'indoor_climate_1'
+        zone_A1 = building_with_data.get_zones(zone_ids=[4830])[0]
+        units_A1 = zone_A1.get_units("indoorClimate")
+        assert units_A1[0] == building_with_data.qu(name="indoor_climate_1")
+        zone_A1b = building_with_data.get_zone(id=4830)
+        assert zone_A1 == zone_A1b
+
+        # Zone A2 -- not connected to any units
+        zone_A2 = building_with_data.get_zones(zone_ids=[4831])[0]
+        units_A2 = zone_A2.get_units("indoorClimate")
+        assert not units_A2
+
+        zone_A = zone_A1b.get_parent_zone()
+        assert zone_A.get_parent_zone() is None
+        assert len(zone_A.get_units("indoorClimate")) > 0
+
+    def test_comfort_profiles(self, building):
+        # Zone A1 -- connected to unit named 'indoor_climate_1'
+        zone_A1 = building.get_zones(zone_ids=[4830])[0]
+
+        start_cp = "2023-01-05"
+        end_cp = "2023-01-06"
+        zone_A1.load_comfort_profile_data(start_cp, end_cp)
+
+        df_cp = zone_A1.comfort_profile_data
+        assert isinstance(df_cp, pd.DataFrame)
+        assert 23 <= len(df_cp) <= 25
+
+        df_cp2 = zone_A1.sub_zones[0].comfort_profile_data
+        assert isinstance(df_cp2, pd.DataFrame)
+        assert_frame_equal(df_cp, df_cp2)
+
+        with pytest.raises(NoComfortProfileError):
+            zone_A1.get_parent_zone().comfort_profile_data
+
+    def test_get_unit_types(self, building_with_data):
+        # Zone A1 -- connected to unit named 'indoor_climate_1'
+        zone_A1 = building_with_data.get_zones(zone_ids=[4830])[0]
+        types_A1 = zone_A1.get_unit_types()
+        assert isinstance(types_A1, list)
+        for t in types_A1:
+            assert isinstance(t, str)
+
+        # Zone A2 -- not connected to any units
+        zone_A2 = building_with_data.get_zones(zone_ids=[4831])[0]
+        types_A2 = zone_A2.get_unit_types()
+        assert isinstance(types_A2, list)
+        assert not types_A2
```

### Comparing `preheat_open-1.38/preheat_open/unit_graph.py` & `preheat_open-1.39/preheat_open/unit_graph.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import networkx as nx
-
-from .unit import Unit
-
-
-def generate_unit_graph(building):
-    """
-    Function to build unit graph from a Building object.
-    Iterates through units (nodes) and builds graph based on relations (sub-units).
-    Returns a networkx directed multigraph.
-    """
-
-    # Empty graph
-    G = nx.MultiDiGraph()
-    # Number of nodes, initially
-    pre = 0
-
-    # First run (top-level units)
-    [
-        G.add_nodes_from(
-            [(unit.id, {"unit": unit, "name": unit.name}) for unit in units]
-        )
-        for unit_type, units in building.units.items()
-    ]
-
-    # Note: discovery of sub-units is not optimized (but robust)
-
-    # While new units are discovered
-    while pre < G.number_of_nodes():
-        # Update number of nodes
-        pre = G.number_of_nodes()
-
-        # For each old node (copy of graph)
-        for node, data in nx.create_empty_copy(G).nodes.data():
-            if hasattr(data["unit"], "sub_units"):
-                # Add sub-units as new nodes
-                new_nodes = [
-                    (unit.id, {"unit": unit, "name": unit.name})
-                    for unit in data["unit"].sub_units
-                ]
-                G.add_nodes_from(new_nodes)
-
-                # Make corresponding edges between nodes
-                new_edges = [
-                    (node, unit.id, {"weight": 0})
-                    for unit in data["unit"].sub_units
-                    if not G.has_edge(node, unit.id)
-                ]
-                G.add_edges_from(new_edges)
-
-    if building.units["main"]:
-        # Add edges to Main (heating and hot water)
-        G.add_edges_from(
-            [
-                (building.units["main"][0].id, node, {"weight": 0})
-                for node, data in G.nodes.data()
-                if data["unit"].unit_type == "heating"
-                or data["unit"].unit_type == "hotWater"
-            ]
-        )
-
-        heating_primary = Unit("supplyPoint", {"id": 0, "name": "Heat"})
-        G.add_node(heating_primary.id, name=heating_primary.name, unit=heating_primary)
-        G.add_edge(heating_primary.id, building.units["main"][0].id, weight=0)
-
-    # Manually add edges to Main (electricity)
-    main_electricity = [
-        node
-        for node, data in G.nodes.data()
-        if data["unit"].name == "Main" and data["unit"].unit_type == "electricity"
-    ]
-
-    if main_electricity:
-        # Add other meters (not main) to main
-        G.add_edges_from(
-            [
-                (main_electricity[0], node, {"weight": 0})
-                for node, data in G.nodes.data()
-                if data["unit"].unit_type == "electricity"
-                and node != main_electricity[0]
-            ]
-        )
-
-        electricity_primary = Unit("supplyPoint", {"id": 1, "name": "Electricity"})
-        G.add_node(
-            electricity_primary.id,
-            name=electricity_primary.name,
-            unit=electricity_primary,
-        )
-        G.add_edge(electricity_primary.id, main_electricity[0], weight=0)
-
-    return G
-
-
-def obtain_loop(graph, id):
-    """
-    Function which first finds a tree, based on id of origin unit/node.
-    The end nodes of the tree are then connected back to the origin, to
-    form a loop/circuit -- for circuit analysis.
-    """
-
-    # First traverse and find tree based on starting point
-    tree = nx.dfs_tree(graph, id)
-
-    # Find end nodes
-    end_nodes = [n for n in tree.nodes() if tree.out_degree(n) == 0]
-
-    # Subgraph (copy, because we want to manipulate with it)
-    Gi = graph.subgraph(tree)
-    Gi = Gi.copy()
-
-    # Close loop to initial node to form circuit
-    Gi.add_edges_from([(n, id, {"weight": 0}) for n in end_nodes])
-
-    # Return tree and graph
-    return tree, Gi
-
-
-def load_data_graph(graph, start, end, resolution):
-    """
-    Loads data for a graph. Loops through nodes (units) and loads
-    data on the units with the given start, end and resolution.
-    Does not return anything -- data is held in the Unit objects.
-    """
-    [
-        data["unit"].load_data(start, end, resolution)
-        for node, data in graph.nodes.data()
-    ]
-
-
-def draw_graph(graph):
-    """
-    Draws graph using networkx built in draw function.
-    This is not pretty, but will help to see if graph is constructed correctly.
-    """
-    nx.draw(
-        graph,
-        pos=nx.shell_layout(graph),
-        node_size=20,
-        labels={node: data["unit"].name for node, data in graph.nodes.data()},
-        font_size=8,
-    )
+import networkx as nx
+
+from .unit import Unit
+
+
+def generate_unit_graph(building):
+    """
+    Function to build unit graph from a Building object.
+    Iterates through units (nodes) and builds graph based on relations (sub-units).
+    Returns a networkx directed multigraph.
+    """
+
+    # Empty graph
+    G = nx.MultiDiGraph()
+    # Number of nodes, initially
+    pre = 0
+
+    # First run (top-level units)
+    [
+        G.add_nodes_from(
+            [(unit.id, {"unit": unit, "name": unit.name}) for unit in units]
+        )
+        for unit_type, units in building.units.items()
+    ]
+
+    # Note: discovery of sub-units is not optimized (but robust)
+
+    # While new units are discovered
+    while pre < G.number_of_nodes():
+        # Update number of nodes
+        pre = G.number_of_nodes()
+
+        # For each old node (copy of graph)
+        for node, data in nx.create_empty_copy(G).nodes.data():
+            if hasattr(data["unit"], "sub_units"):
+                # Add sub-units as new nodes
+                new_nodes = [
+                    (unit.id, {"unit": unit, "name": unit.name})
+                    for unit in data["unit"].sub_units
+                ]
+                G.add_nodes_from(new_nodes)
+
+                # Make corresponding edges between nodes
+                new_edges = [
+                    (node, unit.id, {"weight": 0})
+                    for unit in data["unit"].sub_units
+                    if not G.has_edge(node, unit.id)
+                ]
+                G.add_edges_from(new_edges)
+
+    if building.units["main"]:
+        # Add edges to Main (heating and hot water)
+        G.add_edges_from(
+            [
+                (building.units["main"][0].id, node, {"weight": 0})
+                for node, data in G.nodes.data()
+                if data["unit"].unit_type == "heating"
+                or data["unit"].unit_type == "hotWater"
+            ]
+        )
+
+        heating_primary = Unit("supplyPoint", {"id": 0, "name": "Heat"})
+        G.add_node(heating_primary.id, name=heating_primary.name, unit=heating_primary)
+        G.add_edge(heating_primary.id, building.units["main"][0].id, weight=0)
+
+    # Manually add edges to Main (electricity)
+    main_electricity = [
+        node
+        for node, data in G.nodes.data()
+        if data["unit"].name == "Main" and data["unit"].unit_type == "electricity"
+    ]
+
+    if main_electricity:
+        # Add other meters (not main) to main
+        G.add_edges_from(
+            [
+                (main_electricity[0], node, {"weight": 0})
+                for node, data in G.nodes.data()
+                if data["unit"].unit_type == "electricity"
+                and node != main_electricity[0]
+            ]
+        )
+
+        electricity_primary = Unit("supplyPoint", {"id": 1, "name": "Electricity"})
+        G.add_node(
+            electricity_primary.id,
+            name=electricity_primary.name,
+            unit=electricity_primary,
+        )
+        G.add_edge(electricity_primary.id, main_electricity[0], weight=0)
+
+    return G
+
+
+def obtain_loop(graph, id):
+    """
+    Function which first finds a tree, based on id of origin unit/node.
+    The end nodes of the tree are then connected back to the origin, to
+    form a loop/circuit -- for circuit analysis.
+    """
+
+    # First traverse and find tree based on starting point
+    tree = nx.dfs_tree(graph, id)
+
+    # Find end nodes
+    end_nodes = [n for n in tree.nodes() if tree.out_degree(n) == 0]
+
+    # Subgraph (copy, because we want to manipulate with it)
+    Gi = graph.subgraph(tree)
+    Gi = Gi.copy()
+
+    # Close loop to initial node to form circuit
+    Gi.add_edges_from([(n, id, {"weight": 0}) for n in end_nodes])
+
+    # Return tree and graph
+    return tree, Gi
+
+
+def load_data_graph(graph, start, end, resolution):
+    """
+    Loads data for a graph. Loops through nodes (units) and loads
+    data on the units with the given start, end and resolution.
+    Does not return anything -- data is held in the Unit objects.
+    """
+    [
+        data["unit"].load_data(start, end, resolution)
+        for node, data in graph.nodes.data()
+    ]
+
+
+def draw_graph(graph):
+    """
+    Draws graph using networkx built in draw function.
+    This is not pretty, but will help to see if graph is constructed correctly.
+    """
+    nx.draw(
+        graph,
+        pos=nx.shell_layout(graph),
+        node_size=20,
+        labels={node: data["unit"].name for node, data in graph.nodes.data()},
+        font_size=8,
+    )
```

### Comparing `preheat_open-1.38/preheat_open/weather.py` & `preheat_open-1.39/preheat_open/weather.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from typing import Optional
+
 import pandas as pd
-from pandas import DataFrame
 
 from .backwards_compatibility import load_parameter_old_naming
 from .component import Component
 from .data import load_weather_data
 from .helpers import check_no_remaining_fields, now, sanitise_datetime_input, timedelta
 from .types import TYPE_DATETIME_INPUT
 from .unit import Unit
@@ -86,29 +87,44 @@
                 end,
                 resolution,
             )
 
         self.data: pd.DataFrame = res
         self._ensure_continuity_of_data(resolution)
 
-    def load_state(self, seconds_back: int = 3600, t_now=None) -> None:
+    def load_state(
+        self,
+        seconds_back: int = 3600,
+        t_now=None,
+        resolution_overwrite: Optional[str] = None,
+    ) -> None:
         t_now = now() if t_now is None else sanitise_datetime_input(t_now)
 
+        if resolution_overwrite is None:
+            resolution = "hour"
+        else:
+            resolution = resolution_overwrite
+
         components_to_load = self.get_all_component_ids()
         self._state = load_weather_data(
             self.location_id,
             components_to_load,
             t_now - timedelta(seconds=seconds_back),
             t_now,
-            "hour",
+            resolution,
         )
 
     def get_state(
         self,
         update: bool = False,
         estimate: str = "last",
         seconds_back: int = 3600,
+        resolution_overwrite: Optional[str] = None,
         **kwargs
     ) -> pd.Series:
         return super().get_state(
-            update=update, estimate=estimate, seconds_back=seconds_back, **kwargs
+            update=update,
+            estimate=estimate,
+            seconds_back=seconds_back,
+            resolution_overwrite=resolution_overwrite,
+            **kwargs
         )
```

### Comparing `preheat_open-1.38/preheat_open/zone.py` & `preheat_open-1.39/preheat_open/zone.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-from __future__ import annotations
-
-from typing import Optional
-
-import pandas as pd
-
-from .building_unit import BaseBuildingUnit
-from .exceptions import NoComfortProfileError
-from .helpers import check_no_remaining_fields
-from .types import TYPE_DATETIME_INPUT
-
-
-def populate_zones(zones_data, parent_zone=None, building=None):
-    # Loop over zones; create and populate Zone instances
-    zones = [
-        Zone(zone_i, parent_zone=parent_zone, building=building)
-        for zone_i in zones_data
-    ]
-    return zones
-
-
-class Zone(object):
-    """Defines a building zone in the PreHEAT sense"""
-
-    def __init__(self, zone_data, parent_zone=None, building=None):
-        self.building = building
-
-        # Identifier of the zone
-        self.id = zone_data.pop("id")
-        # Name of the zone
-        self.name = zone_data.pop("name", str(self.id))
-        self.__external_identifier = zone_data.pop("externalIdentifier", "")
-
-        # Floor area of the zone
-        self.area = zone_data.pop("zoneArea", None)
-        # Whether zone has an external wall (boolean)
-        self.has_external_wall = zone_data.pop("hasExternalWall", None)
-        # Sub-zones of the zone (list of PreHEAT_API.Zones)
-        self.sub_zones = populate_zones(
-            zone_data.pop("subZones", []), parent_zone=self, building=self.building
-        )
-        # Adjacency
-        self.adjacent_zones = [
-            z["zoneId"] for z in zone_data.pop("adjacentZones", None)
-        ]
-        # Type of the zone
-        self._type = zone_data.pop("type")
-
-        # Parent zone
-        self.__parent = parent_zone
-
-        # Adding coupled units
-        self.__coupled_units = dict()
-
-        # Adding comfort profile
-        self.__comfort_profile_id = zone_data.pop("comfortProfileId", None)
-
-        # Add ventilation context
-        self.__ventilation_settings = {
-            "supply": zone_data.pop("ventilationSupply", False),
-            "exhaust": zone_data.pop("ventilationExhaust", False),
-        }
-
-        check_no_remaining_fields(zone_data, debug_helper="zone_data")
-
-    def load_comfort_profile_data(
-        self, start: TYPE_DATETIME_INPUT, end: TYPE_DATETIME_INPUT
-    ) -> None:
-        """
-        Loads the comfort profile data in the building object
-
-        :param start: start of the period
-        :param end: end of the period
-        """
-        self.building.load_comfort_profile_data(start, end)
-
-    def clear_comfort_profile_data(self) -> None:
-        """
-        Clears the comfort profile data loaded in the building object (therefore also the zone)
-        """
-        self.building.clear_comfort_profile_data()
-
-    @property
-    def comfort_profile_data(self) -> pd.DataFrame:
-        """
-        Accessor to the comfort profile data of the given zone (or its parents).
-        This requires prior loading via the *load_comfort_profile_data* method.
-
-        If no comfort profile is defined in the zone and the building only has one,
-        then it falls back to the comfort profile at building level.
-
-        Raises NoComfortProfileError if no data is loaded or available
-
-        :return: comfort profile in format: dataframe[setpoint, min, max, value]
-        """
-        if self.__comfort_profile_id is None:
-            if self.__parent is None:
-                try:
-                    # By default, return comfort profile for building if there is only one
-                    out = self.building.comfort_profile_data
-                except ValueError as e:
-                    raise NoComfortProfileError(
-                        "No comfort profile available for zone, and no parent available"
-                    ) from e
-            else:
-                out = self.__parent.comfort_profile_data
-        else:
-            out = self.building.get_comfort_profile_data(self.__comfort_profile_id)
-
-        return out
-
-    def get_sub_zones(self, zone_ids=None) -> list[Zone]:
-        if zone_ids is None:
-            res = self.sub_zones
-        else:
-            res = []
-            for z_i in self.sub_zones:
-                if z_i.id in zone_ids:
-                    res.append(z_i)
-                res += z_i.get_sub_zones(zone_ids=zone_ids)
-        return res
-
-    def get_parent_zone(self) -> Zone:
-        return self.__parent
-
-    def get_type(self) -> tuple[Optional[str], str]:
-        """
-        Returns the type of the zone ('room', 'stairway', 'corridor', 'bathroom', 'kitchen')
-        and its 'dryness' ('dry', 'wet', '?')
-
-        :return: zone_type, wet_or_dry
-        """
-        if self._type is None:
-            return None, "?"
-        zone_type = self._type.lower()
-        if zone_type in ["room", "stairway", "corridor"]:
-            wet_or_dry = "dry"
-        elif zone_type in ["bathroom", "kitchen"]:
-            wet_or_dry = "wet"
-        else:
-            wet_or_dry = "?"
-        return zone_type, wet_or_dry
-
-    def __repr__(self):
-        return "{0}({1})".format(type(self).__name__, self.name)
-
-    def add_coupled_unit(self, unit) -> None:
-        unit_type = unit.unit_type
-        if unit_type in self.__coupled_units.keys():
-            if unit.id in [u_i.id for u_i in self.__coupled_units[unit_type]]:
-                pass  # Skip addition of already existing units
-            else:
-                self.__coupled_units[unit_type].append(unit)
-        else:
-            self.__coupled_units[unit_type] = [unit]
-
-    def get_units(self, unit_type, sub_zones=True) -> list[BaseBuildingUnit]:
-        """
-        Returns the coupled units of a given type
-
-        :param unit_type: str
-        :param sub_zones: bool (True)
-        :return: list(BuildingUnit) or None
-        """
-        us = self.__coupled_units.get(unit_type)
-        if us is None:
-            us = []
-        if sub_zones is True:
-            for z_i in self.sub_zones:
-                us_i = z_i.get_units(unit_type, sub_zones=True)
-                if len(us_i) > 0:
-                    us += us_i
-        return us
-
-    def get_unit_types(self, sub_zones=True) -> list[str]:
-        """
-        Return as list of the coupled unit types
-        """
-        us = list(self.__coupled_units.keys())
-        if sub_zones is True:
-            for z_i in self.sub_zones:
-                us_i = z_i.get_unit_types(sub_zones=True)
-                if us_i is not None:
-                    if us is None:
-                        us = us_i
-                    else:
-                        us += us_i
-        out = []
-        [out.append(k) for k in us if k not in out]
-        return out
-
-    def describe(
-        self, children: bool = True, prefix: str = "", display: bool = True
-    ) -> str:
-        z_type, __ = self.get_type()
-        type_prefix = "[{}] ".format(z_type) if z_type is not None else ""
-        out = prefix + type_prefix + self.name + " [id={}]".format(self.id)
-        if children:
-            for z in self.sub_zones:
-                out += "\n" + z.describe(
-                    prefix=prefix.replace("-", "") + "\t- ", display=False
-                )
-        if display:
-            print(out)
-        return out
-
-    def query_zones(
-        self, zone_id: Optional[int] = None, zone_type: Optional[str] = None
-    ) -> list[Zone]:
-        out = []
-        for z in self.sub_zones:
-            if zone_matches(z, zone_id=zone_id, zone_type=zone_type):
-                out += [z]
-            out += z.query_zones(zone_id=zone_id, zone_type=zone_type)
-        return out
-
-
-def zone_matches(
-    z: Zone, zone_id: Optional[int] = None, zone_type: Optional[str] = None
-) -> bool:
-    by_zone_id = zone_id is not None
-    by_zone_type = zone_type is not None
-    z_zone_type, __ = z.get_type()
-
-    if by_zone_id and by_zone_type:
-        out = (zone_id == z.id) and (zone_type == z_zone_type)
-    elif by_zone_id:
-        out = zone_id == z.id
-    elif by_zone_type:
-        out = zone_type == z_zone_type
-    else:
-        out = False
-    return out
+from __future__ import annotations
+
+from typing import Optional
+
+import pandas as pd
+
+from .building_unit import BaseBuildingUnit
+from .exceptions import NoComfortProfileError
+from .helpers import check_no_remaining_fields
+from .types import TYPE_DATETIME_INPUT
+
+
+def populate_zones(zones_data, parent_zone=None, building=None):
+    # Loop over zones; create and populate Zone instances
+    zones = [
+        Zone(zone_i, parent_zone=parent_zone, building=building)
+        for zone_i in zones_data
+    ]
+    return zones
+
+
+class Zone(object):
+    """Defines a building zone in the PreHEAT sense"""
+
+    def __init__(self, zone_data, parent_zone=None, building=None):
+        self.building = building
+
+        # Identifier of the zone
+        self.id = zone_data.pop("id")
+        # Name of the zone
+        self.name = zone_data.pop("name", str(self.id))
+        self.__external_identifier = zone_data.pop("externalIdentifier", "")
+
+        # Floor area of the zone
+        self.area = zone_data.pop("zoneArea", None)
+        # Whether zone has an external wall (boolean)
+        self.has_external_wall = zone_data.pop("hasExternalWall", None)
+        # Sub-zones of the zone (list of PreHEAT_API.Zones)
+        self.sub_zones = populate_zones(
+            zone_data.pop("subZones", []), parent_zone=self, building=self.building
+        )
+        # Adjacency
+        self.adjacent_zones = [
+            z["zoneId"] for z in zone_data.pop("adjacentZones", None)
+        ]
+        # Type of the zone
+        self._type = zone_data.pop("type")
+
+        # Parent zone
+        self.__parent = parent_zone
+
+        # Adding coupled units
+        self.__coupled_units = dict()
+
+        # Adding comfort profile
+        self.__comfort_profile_id = zone_data.pop("comfortProfileId", None)
+
+        # Add ventilation context
+        self.__ventilation_settings = {
+            "supply": zone_data.pop("ventilationSupply", False),
+            "exhaust": zone_data.pop("ventilationExhaust", False),
+        }
+
+        check_no_remaining_fields(zone_data, debug_helper="zone_data")
+
+    def load_comfort_profile_data(
+        self, start: TYPE_DATETIME_INPUT, end: TYPE_DATETIME_INPUT
+    ) -> None:
+        """
+        Loads the comfort profile data in the building object
+
+        :param start: start of the period
+        :param end: end of the period
+        """
+        self.building.load_comfort_profile_data(start, end)
+
+    def clear_comfort_profile_data(self) -> None:
+        """
+        Clears the comfort profile data loaded in the building object (therefore also the zone)
+        """
+        self.building.clear_comfort_profile_data()
+
+    @property
+    def comfort_profile_data(self) -> pd.DataFrame:
+        """
+        Accessor to the comfort profile data of the given zone (or its parents).
+        This requires prior loading via the *load_comfort_profile_data* method.
+
+        If no comfort profile is defined in the zone and the building only has one,
+        then it falls back to the comfort profile at building level.
+
+        Raises NoComfortProfileError if no data is loaded or available
+
+        :return: comfort profile in format: dataframe[setpoint, min, max, value]
+        """
+        if self.__comfort_profile_id is None:
+            if self.__parent is None:
+                try:
+                    # By default, return comfort profile for building if there is only one
+                    out = self.building.comfort_profile_data
+                except ValueError as e:
+                    raise NoComfortProfileError(
+                        "No comfort profile available for zone, and no parent available"
+                    ) from e
+            else:
+                out = self.__parent.comfort_profile_data
+        else:
+            out = self.building.get_comfort_profile_data(self.__comfort_profile_id)
+
+        return out
+
+    def get_sub_zones(self, zone_ids=None) -> list[Zone]:
+        if zone_ids is None:
+            res = self.sub_zones
+        else:
+            res = []
+            for z_i in self.sub_zones:
+                if z_i.id in zone_ids:
+                    res.append(z_i)
+                res += z_i.get_sub_zones(zone_ids=zone_ids)
+        return res
+
+    def get_parent_zone(self) -> Zone:
+        return self.__parent
+
+    def get_type(self) -> tuple[Optional[str], str]:
+        """
+        Returns the type of the zone ('room', 'stairway', 'corridor', 'bathroom', 'kitchen')
+        and its 'dryness' ('dry', 'wet', '?')
+
+        :return: zone_type, wet_or_dry
+        """
+        if self._type is None:
+            return None, "?"
+        zone_type = self._type.lower()
+        if zone_type in ["room", "stairway", "corridor"]:
+            wet_or_dry = "dry"
+        elif zone_type in ["bathroom", "kitchen"]:
+            wet_or_dry = "wet"
+        else:
+            wet_or_dry = "?"
+        return zone_type, wet_or_dry
+
+    def __repr__(self):
+        return "{0}({1})".format(type(self).__name__, self.name)
+
+    def add_coupled_unit(self, unit) -> None:
+        unit_type = unit.unit_type
+        if unit_type in self.__coupled_units.keys():
+            if unit.id in [u_i.id for u_i in self.__coupled_units[unit_type]]:
+                pass  # Skip addition of already existing units
+            else:
+                self.__coupled_units[unit_type].append(unit)
+        else:
+            self.__coupled_units[unit_type] = [unit]
+
+    def get_units(self, unit_type, sub_zones=True) -> list[BaseBuildingUnit]:
+        """
+        Returns the coupled units of a given type
+
+        :param unit_type: str
+        :param sub_zones: bool (True)
+        :return: list(BuildingUnit) or None
+        """
+        us = self.__coupled_units.get(unit_type)
+        if us is None:
+            us = []
+        if sub_zones is True:
+            for z_i in self.sub_zones:
+                us_i = z_i.get_units(unit_type, sub_zones=True)
+                if len(us_i) > 0:
+                    us += us_i
+        return us
+
+    def get_unit_types(self, sub_zones=True) -> list[str]:
+        """
+        Return as list of the coupled unit types
+        """
+        us = list(self.__coupled_units.keys())
+        if sub_zones is True:
+            for z_i in self.sub_zones:
+                us_i = z_i.get_unit_types(sub_zones=True)
+                if us_i is not None:
+                    if us is None:
+                        us = us_i
+                    else:
+                        us += us_i
+        out = []
+        [out.append(k) for k in us if k not in out]
+        return out
+
+    def describe(
+        self, children: bool = True, prefix: str = "", display: bool = True
+    ) -> str:
+        z_type, __ = self.get_type()
+        type_prefix = "[{}] ".format(z_type) if z_type is not None else ""
+        out = prefix + type_prefix + self.name + " [id={}]".format(self.id)
+        if children:
+            for z in self.sub_zones:
+                out += "\n" + z.describe(
+                    prefix=prefix.replace("-", "") + "\t- ", display=False
+                )
+        if display:
+            print(out)
+        return out
+
+    def query_zones(
+        self, zone_id: Optional[int] = None, zone_type: Optional[str] = None
+    ) -> list[Zone]:
+        out = []
+        for z in self.sub_zones:
+            if zone_matches(z, zone_id=zone_id, zone_type=zone_type):
+                out += [z]
+            out += z.query_zones(zone_id=zone_id, zone_type=zone_type)
+        return out
+
+
+def zone_matches(
+    z: Zone, zone_id: Optional[int] = None, zone_type: Optional[str] = None
+) -> bool:
+    by_zone_id = zone_id is not None
+    by_zone_type = zone_type is not None
+    z_zone_type, __ = z.get_type()
+
+    if by_zone_id and by_zone_type:
+        out = (zone_id == z.id) and (zone_type == z_zone_type)
+    elif by_zone_id:
+        out = zone_id == z.id
+    elif by_zone_type:
+        out = zone_type == z_zone_type
+    else:
+        out = False
+    return out
```

### Comparing `preheat_open-1.38/preheat_open.egg-info/PKG-INFO` & `preheat_open-1.39/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
-Name: preheat-open
-Version: 1.38
+Name: preheat_open
+Version: 1.39
 Summary: Python wrapper for Neogrid Technologies' REST API
 Home-page: https://gitlab.com/neogrid-technologies-public/preheat-open-python
 Author: Neogrid and contributors
 Author-email: analytics@neogrid.dk
 Project-URL: Bug Tracker, https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/issues
 Project-URL: Documentation, https://preheat-open.readthedocs.io/en/latest/
 Project-URL: Source Code, https://gitlab.com/neogrid-technologies-public/preheat-open-python
+Project-URL: Changelog, https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/RELEASE_NOTES.md
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # PreHEAT Open Python Package
 
 This is the open Python package to consume Neogrids REST API.
 
-For a quick introduction to how to use it on real-world data, see the [**quick start guide**](https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/docs/source/tutorials/demo.ipynb).
+For a quick introduction to how to use it on real-world data, see the [quick start guide](https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/docs/source/tutorials/demo.ipynb).
 
 ## Installation and configuration
 
 ### Simple installation:
 Install the package directly from [PyPi](https://pypi.org/project/preheat-open/) using:
 
     pip install preheat_open
```

### Comparing `preheat_open-1.38/preheat_open.egg-info/SOURCES.txt` & `preheat_open-1.39/preheat_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preheat_open-1.38/setup.py` & `preheat_open-1.39/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-import setuptools
-
-import versioneer
-
-package_requirements_file = "requirements.txt"
-docs_requirements_file = "docs/requirements.txt"
-documentation_requirements = open(docs_requirements_file).read().split("\n")
-
-setuptools.setup(
-    name="preheat_open",
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
-    author="Neogrid and contributors",
-    author_email="analytics@neogrid.dk",
-    description="Python wrapper for Neogrid Technologies' REST API",
-    long_description=open("README.md").read(),
-    long_description_content_type="text/markdown",
-    url="https://gitlab.com/neogrid-technologies-public/preheat-open-python",
-    project_urls={
-        "Bug Tracker": "https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/issues",
-        "Documentation": "https://preheat-open.readthedocs.io/en/latest/",
-        "Source Code": "https://gitlab.com/neogrid-technologies-public/preheat-open-python",
-    },
-    packages=setuptools.find_packages(),
-    data_files=[("requirements", [package_requirements_file, docs_requirements_file])],
-    python_requires=">=3.9",
-    install_requires=open(package_requirements_file).read().split("\n"),
-    extras_require={
-        "doc": documentation_requirements,
-        "dev": [
-            "setuptools>=42",
-            "wheel",
-            "pytest",
-            "pytest-cov",
-            "pytest-xdist",
-        ]
-        + documentation_requirements,
-    },
-)
+import setuptools
+
+import versioneer
+
+package_requirements_file = "requirements.txt"
+docs_requirements_file = "docs/requirements.txt"
+documentation_requirements = open(docs_requirements_file).read().split("\n")
+
+setuptools.setup(
+    name="preheat_open",
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
+    author="Neogrid and contributors",
+    author_email="analytics@neogrid.dk",
+    description="Python wrapper for Neogrid Technologies' REST API",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    url="https://gitlab.com/neogrid-technologies-public/preheat-open-python",
+    project_urls={
+        "Bug Tracker": "https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/issues",
+        "Documentation": "https://preheat-open.readthedocs.io/en/latest/",
+        "Source Code": "https://gitlab.com/neogrid-technologies-public/preheat-open-python",
+        "Changelog": "https://gitlab.com/neogrid-technologies-public/preheat-open-python/-/blob/master/RELEASE_NOTES.md",
+    },
+    packages=setuptools.find_packages(),
+    data_files=[("requirements", [package_requirements_file, docs_requirements_file])],
+    python_requires=">=3.9",
+    install_requires=open(package_requirements_file).read().split("\n"),
+    extras_require={
+        "doc": documentation_requirements,
+        "dev": [
+            "setuptools>=42",
+            "wheel",
+            "pytest",
+            "pytest-cov",
+            "pytest-xdist",
+        ]
+        + documentation_requirements,
+    },
+)
```

### Comparing `preheat_open-1.38/versioneer.py` & `preheat_open-1.39/versioneer.py`

 * *Files identical despite different names*

