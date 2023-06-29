# Comparing `tmp/ecoengine-0.0.8.tar.gz` & `tmp/ecoengine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-0.0.8.tar", last modified: Tue Jun 20 19:21:49 2023, max compression
+gzip compressed data, was "ecoengine-0.0.9.tar", last modified: Tue Jun 20 20:17:31 2023, max compression
```

## Comparing `ecoengine-0.0.8.tar` & `ecoengine-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.400133 ecoengine-0.0.8/
--rw-rw-rw-   0        0        0       45 2023-04-13 18:49:37.000000 ecoengine-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3815 2023-06-20 19:21:49.270751 ecoengine-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3175 2023-04-11 19:29:37.000000 ecoengine-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-03-28 18:57:57.000000 ecoengine-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      767 2023-06-20 19:21:49.324869 ecoengine-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-04-11 19:29:37.000000 ecoengine-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.436133 ecoengine-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.568133 ecoengine-0.0.8/src/ecoengine/
--rw-rw-rw-   0        0        0      915 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.496133 ecoengine-0.0.8/src/ecoengine/constants/
--rw-rw-rw-   0        0        0      572 2023-06-19 21:37:33.000000 ecoengine-0.0.8/src/ecoengine/constants/Constants.py
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.516133 ecoengine-0.0.8/src/ecoengine/data/
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.544133 ecoengine-0.0.8/src/ecoengine/data/load_shapes/
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/apartment.json
--rw-rw-rw-   0        0        0      971 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/elementary_school.json
--rw-rw-rw-   0        0        0     1127 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/food_service_a.json
--rw-rw-rw-   0        0        0     1272 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/food_service_b.json
--rw-rw-rw-   0        0        0     1240 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/junior_high.json
--rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/motel.json
--rw-rw-rw-   0        0        0   259798 2023-05-26 20:26:21.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/multi_family.json
--rw-rw-rw-   0        0        0     1273 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/nursing_home.json
--rw-rw-rw-   0        0        0     1058 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/office_building.json
--rw-rw-rw-   0        0        0     1120 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/senior_high.json
--rw-rw-rw-   0        0        0     1219 2023-04-11 19:29:37.000000 ecoengine-0.0.8/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.568133 ecoengine-0.0.8/src/ecoengine/engine/
--rw-rw-rw-   0        0        0     8720 2023-06-13 16:15:20.000000 ecoengine-0.0.8/src/ecoengine/engine/BuildingCreator.py
--rw-rw-rw-   0        0        0    10779 2023-06-20 18:37:08.000000 ecoengine-0.0.8/src/ecoengine/engine/EcosizerEngine.py
--rw-rw-rw-   0        0        0     4047 2023-06-19 17:36:14.000000 ecoengine-0.0.8/src/ecoengine/engine/Simulator.py
--rw-rw-rw-   0        0        0     4540 2023-06-15 17:18:04.000000 ecoengine-0.0.8/src/ecoengine/engine/SystemCreator.py
--rw-rw-rw-   0        0        0      894 2023-04-11 19:29:38.000000 ecoengine-0.0.8/src/ecoengine/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.596133 ecoengine-0.0.8/src/ecoengine/objects/
--rw-rw-rw-   0        0        0    10098 2023-06-20 18:36:29.000000 ecoengine-0.0.8/src/ecoengine/objects/Building.py
--rw-rw-rw-   0        0        0     4957 2023-06-20 18:12:14.000000 ecoengine-0.0.8/src/ecoengine/objects/PrefMapTracker.py
--rw-rw-rw-   0        0        0    12246 2023-06-19 17:44:26.000000 ecoengine-0.0.8/src/ecoengine/objects/SimulationRun.py
--rw-rw-rw-   0        0        0    38112 2023-06-20 18:41:57.000000 ecoengine-0.0.8/src/ecoengine/objects/SystemConfig.py
--rw-rw-rw-   0        0        0      940 2023-04-11 19:29:38.000000 ecoengine-0.0.8/src/ecoengine/objects/__init__.py
--rw-rw-rw-   0        0        0     3481 2023-05-30 20:59:48.000000 ecoengine-0.0.8/src/ecoengine/objects/systemConfigUtils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.620133 ecoengine-0.0.8/src/ecoengine/objects/systems/
--rw-rw-rw-   0        0        0     4530 2023-06-15 17:19:45.000000 ecoengine-0.0.8/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-rw-rw-   0        0        0    22591 2023-06-20 19:20:20.000000 ecoengine-0.0.8/src/ecoengine/objects/systems/SwingTank.py
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:38.000000 ecoengine-0.0.8/src/ecoengine/objects/systems/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:21:44.464133 ecoengine-0.0.8/src/ecoengine.egg-info/
--rw-rw-rw-   0        0        0     3815 2023-06-20 19:21:43.000000 ecoengine-0.0.8/src/ecoengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1543 2023-06-20 19:21:44.000000 ecoengine-0.0.8/src/ecoengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 19:21:43.000000 ecoengine-0.0.8/src/ecoengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-20 19:21:43.000000 ecoengine-0.0.8/src/ecoengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 19:21:43.000000 ecoengine-0.0.8/src/ecoengine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.353368 ecoengine-0.0.9/
+-rw-rw-rw-   0        0        0      143 2023-06-20 20:16:44.000000 ecoengine-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3815 2023-06-20 20:17:31.794678 ecoengine-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3175 2023-04-11 19:29:37.000000 ecoengine-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-28 18:57:57.000000 ecoengine-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      767 2023-06-20 20:17:31.842526 ecoengine-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-04-11 19:29:37.000000 ecoengine-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.405368 ecoengine-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.589368 ecoengine-0.0.9/src/ecoengine/
+-rw-rw-rw-   0        0        0      915 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.457368 ecoengine-0.0.9/src/ecoengine/constants/
+-rw-rw-rw-   0        0        0      572 2023-06-19 21:37:33.000000 ecoengine-0.0.9/src/ecoengine/constants/Constants.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.537368 ecoengine-0.0.9/src/ecoengine/data/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.513368 ecoengine-0.0.9/src/ecoengine/data/climate_data/
+-rw-rw-rw-   0        0        0   778857 2023-06-15 00:33:46.000000 ecoengine-0.0.9/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
+-rw-rw-rw-   0        0        0     1356 2023-05-22 22:02:40.000000 ecoengine-0.0.9/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
+-rw-rw-rw-   0        0        0    25488 2023-05-26 19:54:11.000000 ecoengine-0.0.9/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
+-rw-rw-rw-   0        0        0  1676166 2023-06-19 17:23:29.000000 ecoengine-0.0.9/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.537368 ecoengine-0.0.9/src/ecoengine/data/load_shapes/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/apartment.json
+-rw-rw-rw-   0        0        0      971 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-rw-rw-   0        0        0     1127 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-rw-rw-   0        0        0     1272 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-rw-rw-   0        0        0     1240 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/junior_high.json
+-rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/motel.json
+-rw-rw-rw-   0        0        0   259798 2023-05-26 20:26:21.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/multi_family.json
+-rw-rw-rw-   0        0        0     1273 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-rw-rw-   0        0        0     1058 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/office_building.json
+-rw-rw-rw-   0        0        0     1120 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/senior_high.json
+-rw-rw-rw-   0        0        0     1219 2023-04-11 19:29:37.000000 ecoengine-0.0.9/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.561368 ecoengine-0.0.9/src/ecoengine/data/preformanceMaps/
+-rw-rw-rw-   0        0        0     3554 2023-06-13 19:52:21.000000 ecoengine-0.0.9/src/ecoengine/data/preformanceMaps/maps.json
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.589368 ecoengine-0.0.9/src/ecoengine/engine/
+-rw-rw-rw-   0        0        0     8720 2023-06-13 16:15:20.000000 ecoengine-0.0.9/src/ecoengine/engine/BuildingCreator.py
+-rw-rw-rw-   0        0        0    10779 2023-06-20 18:37:08.000000 ecoengine-0.0.9/src/ecoengine/engine/EcosizerEngine.py
+-rw-rw-rw-   0        0        0     4047 2023-06-19 17:36:14.000000 ecoengine-0.0.9/src/ecoengine/engine/Simulator.py
+-rw-rw-rw-   0        0        0     4540 2023-06-15 17:18:04.000000 ecoengine-0.0.9/src/ecoengine/engine/SystemCreator.py
+-rw-rw-rw-   0        0        0      894 2023-04-11 19:29:38.000000 ecoengine-0.0.9/src/ecoengine/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.625368 ecoengine-0.0.9/src/ecoengine/objects/
+-rw-rw-rw-   0        0        0    10098 2023-06-20 18:36:29.000000 ecoengine-0.0.9/src/ecoengine/objects/Building.py
+-rw-rw-rw-   0        0        0     4957 2023-06-20 18:12:14.000000 ecoengine-0.0.9/src/ecoengine/objects/PrefMapTracker.py
+-rw-rw-rw-   0        0        0    12246 2023-06-19 17:44:26.000000 ecoengine-0.0.9/src/ecoengine/objects/SimulationRun.py
+-rw-rw-rw-   0        0        0    38112 2023-06-20 18:41:57.000000 ecoengine-0.0.9/src/ecoengine/objects/SystemConfig.py
+-rw-rw-rw-   0        0        0      940 2023-04-11 19:29:38.000000 ecoengine-0.0.9/src/ecoengine/objects/__init__.py
+-rw-rw-rw-   0        0        0     3481 2023-05-30 20:59:48.000000 ecoengine-0.0.9/src/ecoengine/objects/systemConfigUtils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.657369 ecoengine-0.0.9/src/ecoengine/objects/systems/
+-rw-rw-rw-   0        0        0     4530 2023-06-15 17:19:45.000000 ecoengine-0.0.9/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-rw-rw-   0        0        0    22591 2023-06-20 19:20:20.000000 ecoengine-0.0.9/src/ecoengine/objects/systems/SwingTank.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:38.000000 ecoengine-0.0.9/src/ecoengine/objects/systems/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:17:24.437368 ecoengine-0.0.9/src/ecoengine.egg-info/
+-rw-rw-rw-   0        0        0     3815 2023-06-20 20:17:23.000000 ecoengine-0.0.9/src/ecoengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1853 2023-06-20 20:17:24.000000 ecoengine-0.0.9/src/ecoengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 20:17:23.000000 ecoengine-0.0.9/src/ecoengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-20 20:17:23.000000 ecoengine-0.0.9/src/ecoengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 20:17:23.000000 ecoengine-0.0.9/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-0.0.8/PKG-INFO` & `ecoengine-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.8
+Version: 0.0.9
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-0.0.8/README.md` & `ecoengine-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/setup.cfg` & `ecoengine-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 656e 6769 6e65 0d0a 7665   = ecoengine..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 380d 0a61  rsion = 0.0.8..a
+00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
 00000030: 7574 686f 7220 3d20 4e6f 6c61 6e0d 0a61  uthor = Nolan..a
 00000040: 7574 686f 725f 656d 6169 6c20 3d20 6e6f  uthor_email = no
 00000050: 6c61 6e40 6563 6f74 6f70 652e 636f 6d0d  lan@ecotope.com.
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000070: 2073 6f66 7477 6172 6520 666f 7220 7369   software for si
 00000080: 7a69 6e67 2048 6561 7420 5075 6d70 2057  zing Heat Pump W
 00000090: 6174 6572 2048 6561 7465 7273 2066 6f72  ater Heaters for
```

### Comparing `ecoengine-0.0.8/src/ecoengine/__init__.py` & `ecoengine-0.0.9/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/constants/Constants.py` & `ecoengine-0.0.9/src/ecoengine/constants/Constants.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/multi_family.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/multi_family.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-0.0.9/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-0.0.9/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-0.0.9/src/ecoengine/engine/EcosizerEngine.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/engine/Simulator.py` & `ecoengine-0.0.9/src/ecoengine/engine/Simulator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/engine/SystemCreator.py` & `ecoengine-0.0.9/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/engine/__init__.py` & `ecoengine-0.0.9/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/objects/Building.py` & `ecoengine-0.0.9/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/objects/PrefMapTracker.py` & `ecoengine-0.0.9/src/ecoengine/objects/PrefMapTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/objects/SimulationRun.py` & `ecoengine-0.0.9/src/ecoengine/objects/SimulationRun.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/objects/SystemConfig.py` & `ecoengine-0.0.9/src/ecoengine/objects/SystemConfig.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/objects/__init__.py` & `ecoengine-0.0.9/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-0.0.9/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-0.0.9/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-0.0.9/src/ecoengine/objects/systems/SwingTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.8/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-0.0.9/src/ecoengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.8
+Version: 0.0.9
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-0.0.8/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-0.0.9/src/ecoengine.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,27 +8,32 @@
 src/ecoengine.egg-info/SOURCES.txt
 src/ecoengine.egg-info/dependency_links.txt
 src/ecoengine.egg-info/requires.txt
 src/ecoengine.egg-info/top_level.txt
 src/ecoengine/constants/Constants.py
 src/ecoengine/constants/__init__.py
 src/ecoengine/data/__init__.py
+src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
+src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
+src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
+src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
 src/ecoengine/data/load_shapes/__init__.py
 src/ecoengine/data/load_shapes/apartment.json
 src/ecoengine/data/load_shapes/elementary_school.json
 src/ecoengine/data/load_shapes/food_service_a.json
 src/ecoengine/data/load_shapes/food_service_b.json
 src/ecoengine/data/load_shapes/junior_high.json
 src/ecoengine/data/load_shapes/mens_dorm.json
 src/ecoengine/data/load_shapes/motel.json
 src/ecoengine/data/load_shapes/multi_family.json
 src/ecoengine/data/load_shapes/nursing_home.json
 src/ecoengine/data/load_shapes/office_building.json
 src/ecoengine/data/load_shapes/senior_high.json
 src/ecoengine/data/load_shapes/womens_dorm.json
+src/ecoengine/data/preformanceMaps/maps.json
 src/ecoengine/engine/BuildingCreator.py
 src/ecoengine/engine/EcosizerEngine.py
 src/ecoengine/engine/Simulator.py
 src/ecoengine/engine/SystemCreator.py
 src/ecoengine/engine/__init__.py
 src/ecoengine/objects/Building.py
 src/ecoengine/objects/PrefMapTracker.py
```

