# Comparing `tmp/simple_dwd_weatherforecast-2.0.1.tar.gz` & `tmp/simple_dwd_weatherforecast-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_dwd_weatherforecast-2.0.1.tar", last modified: Fri Jun 30 08:56:21 2023, max compression
+gzip compressed data, was "simple_dwd_weatherforecast-2.0.2.tar", last modified: Fri Jun 30 12:41:36 2023, max compression
```

## Comparing `simple_dwd_weatherforecast-2.0.1.tar` & `simple_dwd_weatherforecast-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:56:21.140142 simple_dwd_weatherforecast-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 08:56:09.000000 simple_dwd_weatherforecast-2.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 08:56:21.140142 simple_dwd_weatherforecast-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 08:56:09.000000 simple_dwd_weatherforecast-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:56:21.144142 simple_dwd_weatherforecast-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 08:56:09.000000 simple_dwd_weatherforecast-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:56:21.140142 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:56:09.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29857 2023-06-30 08:56:09.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast/dwdforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 08:56:09.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast/dwdmap.py
--rw-r--r--   0 runner    (1001) docker     (123)   386545 2023-06-30 08:56:09.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast/stations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:56:21.140142 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 08:56:21.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 08:56:21.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:56:21.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 08:56:21.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 08:56:21.000000 simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:41:36.303895 simple_dwd_weatherforecast-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 12:41:36.303895 simple_dwd_weatherforecast-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:41:36.307895 simple_dwd_weatherforecast-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:41:36.303895 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/dwdforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/dwdmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   386545 2023-06-30 12:41:25.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/stations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:41:36.303895 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 12:41:36.000000 simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/top_level.txt
```

### Comparing `simple_dwd_weatherforecast-2.0.1/LICENCE` & `simple_dwd_weatherforecast-2.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.1/PKG-INFO` & `simple_dwd_weatherforecast-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_dwd_weatherforecast
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `simple_dwd_weatherforecast-2.0.1/README.md` & `simple_dwd_weatherforecast-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.1/setup.py` & `simple_dwd_weatherforecast-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_dwd_weatherforecast",
-    version="2.0.1",
+    version="2.0.2",
     author="Max Fermor",
     description="A simple tool to retrieve a weather forecast from DWD OpenData",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FL550/simple_dwd_weatherforecast.git",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast/dwdforecast.py` & `simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/dwdforecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 import csv
 
 # from .stations import stations
 with open("stations.json", encoding="utf-8") as f:
     stations = json.load(f)
 
 
-def is_valid_station_id(station_id: str):
-    return station_id in stations
+def load_station_id(station_id: str):
+    if station_id in stations:
+        return stations[station_id]
+    return None
 
 
 def get_nearest_station_id(lat: float, lon: float):
     return get_stations_sorted_by_distance(lat, lon)[0][0]
 
 
 def get_stations_sorted_by_distance(lat: float, lon: float):
@@ -189,23 +191,23 @@
         "SL": "dwoi",
         "BB": "dwpg",
         "BE": "dwpg",
         "MV": "dwph",
     }
 
     def __init__(self, station_id):
-        if is_valid_station_id(station_id):
+        station = load_station_id(station_id)
+        if station:
             self.station_id = station_id
+            self.station_name = station["name"]
             self.region = get_region(station_id)
         else:
             raise ValueError("Not a valid station_id")
 
-    def get_station_name(self, shouldUpdate=False):
-        if self.station_name == "" or shouldUpdate:
-            self.update()
+    def get_station_name(self):
         return self.station_name
 
     def is_in_timerange(self, timestamp: datetime):
         return (
             list(self.forecast_data.keys())[0]
             <= self.strip_to_hour_str(timestamp)
             <= list(self.forecast_data.keys())[-1]
@@ -213,15 +215,15 @@
 
     def is_valid_timeframe(_, timeframe: int) -> bool:
         if 24 < timeframe or timeframe <= 0:
             return False
         return 24 % timeframe == 0
 
     def has_report(self, station_id):
-        if is_valid_station_id(station_id):
+        if load_station_id(station_id):
             return stations[station_id]["report_available"] == 1
         return False
 
     def get_forecast_data(
         self, weatherDataType: WeatherDataType, timestamp: datetime, shouldUpdate=True
     ):
         if shouldUpdate:
@@ -589,17 +591,17 @@
         # print(f"timesteps: {timesteps}")
 
         for placemark in tree.findall("//kml:Placemark", namespaces=self.namespaces):
             item = placemark.find("./kml:name", namespaces=self.namespaces)
             if item.text == self.station_id:
                 tree = placemark
                 break
-        self.station_name = tree.xpath("./kml:description", namespaces=self.namespaces)[
-            0
-        ].text
+        self.loaded_station_name = tree.xpath(
+            "./kml:description", namespaces=self.namespaces
+        )[0].text
 
         result = tree.xpath(
             './kml:ExtendedData/dwd:Forecast[@dwd:elementName="ww"]/dwd:value',
             namespaces=self.namespaces,
         )[0].text
         conditions = []
         for elem in result.split():
```

### Comparing `simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast/dwdmap.py` & `simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/dwdmap.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast/stations.py` & `simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast/stations.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.1/simple_dwd_weatherforecast.egg-info/PKG-INFO` & `simple_dwd_weatherforecast-2.0.2/simple_dwd_weatherforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-dwd-weatherforecast
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

