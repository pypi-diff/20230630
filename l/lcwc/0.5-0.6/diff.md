# Comparing `tmp/lcwc-0.5.tar.gz` & `tmp/lcwc-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcwc-0.5.tar", last modified: Sat Jun 24 15:02:46 2023, max compression
+gzip compressed data, was "lcwc-0.6.tar", last modified: Fri Jun 30 18:48:35 2023, max compression
```

## Comparing `lcwc-0.5.tar` & `lcwc-0.6.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.139338 lcwc-0.5/
--rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.5/LICENSE
--rw-rw-rw-   0        0        0     2325 2023-06-24 15:02:46.137840 lcwc-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.5/README.md
--rw-rw-rw-   0        0        0      789 2023-06-24 15:01:35.000000 lcwc-0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 15:02:46.139338 lcwc-0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.101343 lcwc-0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.114838 lcwc-0.5/src/lcwc/
--rw-rw-rw-   0        0        0       20 2023-06-24 15:01:21.000000 lcwc-0.5/src/lcwc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.124839 lcwc-0.5/src/lcwc/arcgis/
--rw-rw-rw-   0        0        0       60 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/arcgis/__init__.py
--rw-rw-rw-   0        0        0     6050 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/arcgis/client.py
--rw-rw-rw-   0        0        0     1592 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/arcgis/incident.py
--rw-rw-rw-   0        0        0      326 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/category.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.129839 lcwc-0.5/src/lcwc/feed/
--rw-rw-rw-   0        0        0       64 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/feed/__init__.py
--rw-rw-rw-   0        0        0     4201 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/feed/client.py
--rw-rw-rw-   0        0        0      889 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/feed/incident.py
--rw-rw-rw-   0        0        0     2344 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/incident.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.133339 lcwc-0.5/src/lcwc/utils/
--rw-rw-rw-   0        0        0     2925 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/utils/__init__.py
--rw-rw-rw-   0        0        0     4162 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/utils/restadapter.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.136839 lcwc-0.5/src/lcwc/web/
--rw-rw-rw-   0        0        0       27 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/web/__init__.py
--rw-rw-rw-   0        0        0     3681 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/web/client.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.120844 lcwc-0.5/src/lcwc.egg-info/
--rw-rw-rw-   0        0        0     2325 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.420009 lcwc-0.6/
+-rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.6/LICENSE
+-rw-rw-rw-   0        0        0     2325 2023-06-30 18:48:35.419510 lcwc-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.6/README.md
+-rw-rw-rw-   0        0        0      802 2023-06-30 18:44:05.000000 lcwc-0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 18:48:35.420009 lcwc-0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.381510 lcwc-0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.398009 lcwc-0.6/src/lcwc/
+-rw-rw-rw-   0        0        0      120 2023-06-30 18:41:06.000000 lcwc-0.6/src/lcwc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.407009 lcwc-0.6/src/lcwc/arcgis/
+-rw-rw-rw-   0        0        0       72 2023-06-30 18:00:38.000000 lcwc-0.6/src/lcwc/arcgis/__init__.py
+-rw-rw-rw-   0        0        0     6273 2023-06-30 18:39:48.000000 lcwc-0.6/src/lcwc/arcgis/client.py
+-rw-rw-rw-   0        0        0     1631 2023-06-30 18:39:07.000000 lcwc-0.6/src/lcwc/arcgis/incident.py
+-rw-rw-rw-   0        0        0      326 2023-06-24 14:32:45.000000 lcwc-0.6/src/lcwc/category.py
+-rw-rw-rw-   0        0        0      318 2023-06-30 18:02:43.000000 lcwc-0.6/src/lcwc/client.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.411011 lcwc-0.6/src/lcwc/feed/
+-rw-rw-rw-   0        0        0       68 2023-06-30 17:57:06.000000 lcwc-0.6/src/lcwc/feed/__init__.py
+-rw-rw-rw-   0        0        0     4468 2023-06-30 18:37:18.000000 lcwc-0.6/src/lcwc/feed/client.py
+-rw-rw-rw-   0        0        0      926 2023-06-30 18:37:26.000000 lcwc-0.6/src/lcwc/feed/incident.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.412009 lcwc-0.6/src/lcwc/feed/utils/
+-rw-rw-rw-   0        0        0     2373 2023-06-30 18:38:10.000000 lcwc-0.6/src/lcwc/feed/utils/__init__.py
+-rw-rw-rw-   0        0        0     1486 2023-06-30 18:36:44.000000 lcwc-0.6/src/lcwc/incident.py
+-rw-rw-rw-   0        0        0      512 2023-06-30 18:35:11.000000 lcwc-0.6/src/lcwc/unit.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.414511 lcwc-0.6/src/lcwc/utils/
+-rw-rw-rw-   0        0        0      610 2023-06-30 17:20:03.000000 lcwc-0.6/src/lcwc/utils/__init__.py
+-rw-rw-rw-   0        0        0     4162 2023-06-24 14:32:45.000000 lcwc-0.6/src/lcwc/utils/restadapter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.418010 lcwc-0.6/src/lcwc/web/
+-rw-rw-rw-   0        0        0       64 2023-06-30 17:55:06.000000 lcwc-0.6/src/lcwc/web/__init__.py
+-rw-rw-rw-   0        0        0     3972 2023-06-30 18:34:22.000000 lcwc-0.6/src/lcwc/web/client.py
+-rw-rw-rw-   0        0        0     2459 2023-06-30 18:31:01.000000 lcwc-0.6/src/lcwc/web/incident.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.403510 lcwc-0.6/src/lcwc.egg-info/
+-rw-rw-rw-   0        0        0     2325 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/top_level.txt
```

### Comparing `lcwc-0.5/LICENSE` & `lcwc-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lcwc-0.5/PKG-INFO` & `lcwc-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.5
+Version: 0.6
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.5/README.md` & `lcwc-0.6/README.md`

 * *Files identical despite different names*

### Comparing `lcwc-0.5/pyproject.toml` & `lcwc-0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lcwc"
-version = "0.5"
+version = "0.6"
 authors = [
   { name="Nate Shoffner", email="nate.shoffner@gmail.com" },
 ]
 description = "Python library for fetching the Lancaster County-Wide Communications live incident list."
 keywords = ["lcwc", "lancaster", "police", "fire", "ems", "dispatch", "911", "incident"]
 readme = "README.md"
 requires-python = ">=3.9"
@@ -13,15 +13,16 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "bs4", 
     "aiohttp", 
-    "feedparser"
+    "feedparser",
+    "pytz"
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project.urls]
 "Homepage" = "https://github.com/NateShoffner/python-lcwc"
```

### Comparing `lcwc-0.5/src/lcwc/arcgis/client.py` & `lcwc-0.6/src/lcwc/arcgis/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import aiohttp
 import datetime
 import json
 import re
+from lcwc import Client
 from lcwc.arcgis.incident import ArcGISIncident, Coordinates
 from lcwc.category import IncidentCategory
+from lcwc.unit import Unit
 from lcwc.utils.restadapter import RestAdapter, RestException
 
 
-class Client:
+class ArcGISClient(Client):
     """Client for the ArcGIS REST API"""
 
+    @property
+    def name(self) -> str:
+        return "ArcGISClient"
+
     async def get_incidents(
         self, session: aiohttp.ClientSession, timeout: int = 10
     ) -> list[ArcGISIncident]:
         """Fetches the page and parses the contents and returns a list of incidents"""
 
         layer_mapping = {
             IncidentCategory.FIRE: 0,
@@ -138,23 +144,24 @@
     def __parse_incident(
         self, category: IncidentCategory, incident: dict
     ) -> ArcGISIncident:
         attributes = incident["attributes"]
         geometry = incident["geometry"]
 
         date = datetime.datetime.fromtimestamp(attributes["IncidentOrigination"] / 1000)
-        township = attributes["IncidentMunicipality"]
+        municipality = attributes["IncidentMunicipality"]
 
         intersection = re.sub(
             " +", " ", attributes["PublicLocation"]
         )  # collapse multiple spaces
 
         # unit names are condensed, lacking spaces and delimiters (ex: MED8611)
         if "CurrentUnits" in attributes and attributes["CurrentUnits"] is not None:
-            units = attributes["CurrentUnits"].split(",")
+            unit_names = attributes["CurrentUnits"].split(",")
+            units = [Unit(unit_name) for unit_name in unit_names]
         else:
             units = []
 
         number = int(attributes["IncidentNumber"])
 
         if "Priority" in attributes:
             priority = int(attributes["Priority"])
@@ -166,15 +173,15 @@
 
         coords = Coordinates(geometry["x"], geometry["y"])
 
         incident = ArcGISIncident(
             category,
             date,
             description,
-            township,
+            municipality,
             intersection,
             number,
             priority,
             agency,
             public,
             coords,
             units,
```

### Comparing `lcwc-0.5/src/lcwc/arcgis/incident.py` & `lcwc-0.6/src/lcwc/arcgis/incident.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import datetime
 from lcwc.incident import Incident
 from lcwc.category import IncidentCategory
 from collections import namedtuple
 
+from lcwc.unit import Unit
+
 Coordinates = namedtuple("Coordinates", ["longitude", "latitude"])
 
 
 class ArcGISIncident(Incident):
     """Represents an incident from the live ArcGIS REST API"""
 
     def __init__(
         self,
         category: IncidentCategory,
         date: datetime,
         description: str,
-        township: str,
+        municipality: str,
         intersection: str,
         number: int,
         priority: int,
         agency: str,
         public: bool,
         coordinates: Coordinates,
-        units: list[str] = [],
+        units: list[Unit] = [],
     ) -> None:
-        super().__init__(category, date, description, township, intersection, units)
+        super().__init__(category, date, description, municipality, intersection, units)
         self._incident_number = number
         self._priority = priority
         self._agency = agency
         self._public = public
         self._coordinates = coordinates
 
     @property
```

### Comparing `lcwc-0.5/src/lcwc/feed/client.py` & `lcwc-0.6/src/lcwc/feed/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import aiohttp
 import datetime
 import feedparser
 import pytz
-from lcwc.feed.incident import FeedIncident
-from lcwc.utils import (
+
+from lcwc import Client
+from lcwc.unit import Unit
+from .utils import (
     FIRE_UNIT_NAMES,
     LOCATION_NAMES,
     MEDICAL_UNIT_NAMES,
     determine_category,
 )
+from lcwc.feed.incident import FeedIncident
 
 """
 Example entry:
 
 <item>
     <title>MEDICAL EMERGENCY</title>
     <link>http://www.lcwc911.us/lcwc/lcwc/publiccad.asp</link>
     <description>MARTIC TOWNSHIP; BRIDGE VALLEY RD & LAKE ALDRED TER; MEDIC 56-1; </description>
     <pubDate>Wed, 25 Jan 2023 15:22:54 GMT</pubDate>
     <guid isPermaLink="false">792d7e14-34ef-4907-bb50-86c43cd3d570</guid>
 </item>
 """
 
 
-class Client:
+class FeedClient(Client):
     """Client for the incident RSS feed"""
 
     URL = "https://webcad.lcwc911.us/Pages/Public/LiveIncidentsFeed.aspx"
     """ The URL of the live incident feed """
 
+    @property
+    def name(self) -> str:
+        """Returns the name of the client"""
+        return "FeedClient"
+
     async def get_incidents(
         self, session: aiohttp.ClientSession, timeout: int = 10
     ) -> list[FeedIncident]:
         """Gets the live incident feed and returns a list of incidents
 
         :param session: The aiohttp session to use
         :param timeout: The timeout for the request
@@ -73,41 +81,41 @@
             gmt_date = datetime.datetime.strptime(
                 entry.published, "%a, %d %b %Y %H:%M:%S %Z"
             )
             date = gmt_date.replace(tzinfo=datetime.timezone.utc).astimezone(pytz.utc)
             description = entry.title
 
             # Possible formats:
-            # [township];[intersection];[units assigned]
-            # [township];[intersection]
-            # [township];[units assigned]
-            # [township]
+            # [municipality];[intersection];[units assigned]
+            # [municipality];[intersection]
+            # [municipality];[units assigned]
+            # [municipality]
             details_split = entry["description"].strip().split(";", maxsplit=3)
 
-            # first item is always the township
-            township = details_split[0].strip()
+            # first item is always the municipality
+            municipality = details_split[0].strip()
 
             intersection = None
             units = []
 
-            # skip if only township is present
+            # skip if only municipality is present
             if len(details_split) >= 2:
                 if has_unit_names(details_split[1]):
                     units = self.__extract_units(details_split[1])
                 else:
                     if has_intersection(details_split[1]):
                         intersection = details_split[1].strip()
                     if len(details_split) > 2 and has_unit_names(details_split[2]):
                         units = self.__extract_units(details_split[2])
 
             category = determine_category(description, units)
 
             incidents.append(
                 FeedIncident(
-                    category, date, description, township, intersection, units, guid
+                    category, date, description, municipality, intersection, units, guid
                 )
             )
 
         return incidents
 
     def __extract_units(self, units_data: str) -> list[str]:
         """Extracts the units from the data string
@@ -115,8 +123,9 @@
         :param units_data: The data string containing the units
         :return: A list of units
         :rtype: list[str]
         """
         units_data = units_data.strip()
         if units_data == "":
             return []
-        return [u.strip() for u in units_data.strip().split("<br />")]
+        unit_names = [u.strip() for u in units_data.strip().split("<br />")]
+        return [Unit(u) for u in unit_names]
```

### Comparing `lcwc-0.5/src/lcwc/feed/incident.py` & `lcwc-0.6/src/lcwc/feed/incident.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # custom class to handle the guid attribute
 # a bit usless on its own but might be useful for statically identifying incidents
 # since apparently every detail is subject to change except maybe the timestamp
 import datetime
 from lcwc.category import IncidentCategory
 from lcwc.incident import Incident
+from lcwc.unit import Unit
 
 
 class FeedIncident(Incident):
     """Represents an incident from the live incident feed"""
 
     def __init__(
         self,
         category: IncidentCategory,
         date: datetime,
         description: str,
-        township: str,
+        municipality: str,
         intersection: str,
-        units: list[str] = [],
+        units: list[Unit] = [],
         guid: str = None,
     ) -> None:
-        super().__init__(category, date, description, township, intersection, units)
+        super().__init__(category, date, description, municipality, intersection, units)
         self._guid = guid
 
     @property
     def guid(self) -> str:
         """Returns the guid of the incident"""
         return self._guid
```

### Comparing `lcwc-0.5/src/lcwc/incident.py` & `lcwc-0.6/src/lcwc/incident.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,30 @@
+from abc import ABC
 import datetime
+
 from lcwc.category import IncidentCategory
+from lcwc.unit import Unit
 
 
-class Incident:
+class Incident(ABC):
     """Represents an incident"""
 
     def __init__(
         self,
         category: IncidentCategory,
         date: datetime,
         description: str,
-        township: str,
+        municipality: str,
         intersection: str,
-        units: list[str] = [],
+        units: list[Unit] = [],
     ) -> None:
-        """Constructor.
-
-        :param IncidentCategory category: The category of the incident
-
-        :param datetime date: The date and time of the incident in local time (EST)
-
-        :param str description: The description of the incident
-
-        :param str township: The location of the incident location
-
-        :param str intersection: The intersection of the incident location
-
-        :param list[str] units: A list of units responding to the incident
-        """
-
         self._category = category
         self._date = date
         self._description = description
-        self._township = township
+        self._municipality = municipality
         self._intersection = intersection
         self._units = units
 
     @property
     def category(self) -> IncidentCategory:
         """Returns the category of the incident"""
         return self._category
@@ -48,33 +36,20 @@
 
     @property
     def description(self) -> str:
         """Returns the incident description"""
         return self._description
 
     @property
-    def township(self) -> str:
-        """Returns the township of the incident location"""
-        return self._township
+    def municipality(self) -> str:
+        """Returns the municipality of the incident location"""
+        return self._municipality
 
     @property
     def intersection(self) -> str:
         """Returns the intersection of the incident location"""
         return self._intersection
 
     @property
-    def location(self) -> str:
-        """Returns the full location of the incident"""
-        if self._intersection is None:
-            return self._township
-        else:
-            return "\n".join([self._intersection, self._township])
-
-    @property
-    def units(self) -> list[str]:
+    def units(self) -> list[Unit]:
         """Returns a list of units responding to the incident"""
         return self._units
-
-    @property
-    def units_pending(self) -> bool:
-        """Returns true if the incident has units pending"""
-        return any([unit == "PENDING" for unit in self._units])
```

### Comparing `lcwc-0.5/src/lcwc/utils/__init__.py` & `lcwc-0.6/src/lcwc/feed/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import datetime
 from lcwc.category import IncidentCategory
-from lcwc.incident import Incident
+from lcwc.unit import Unit
 
 """ A list of keywords that indicate a location name"""
 FIRE_UNIT_NAMES = [
     "ATV",
     "BATTALION",
     "BOAT",
     "BRUSH",
@@ -47,28 +46,28 @@
 """ A list of keywords that indicate a fire incident """
 FIRE_DESCRIPTION_KEYWORDS = ["FIRE"]
 
 """ A list of keywords that indicate a traffic incident """
 TRAFFIC_DESCRIPTION_KEYWORDS = ["TRAFFIC", "VEHICLE"]
 
 
-def determine_category(description: str, units: list[str]) -> IncidentCategory:
+def determine_category(description: str, units: list[Unit]) -> IncidentCategory:
     """Determines the category of an incident based on the description and units assigned
 
     :param description: The description of the incident
     :param units: The units assigned to the incident
     :return: The category of the incident
     :rtype: IncidentCategory
     """
 
     # check for unit matches
     for unit in units:
-        if any(k in unit for k in FIRE_UNIT_NAMES):
+        if any(k in unit.name for k in FIRE_UNIT_NAMES):
             return IncidentCategory.FIRE
-        elif any(k in unit for k in MEDICAL_UNIT_NAMES):
+        elif any(k in unit.name for k in MEDICAL_UNIT_NAMES):
             return IncidentCategory.MEDICAL
 
     # extra note regarding traffic incidents: they tend to not have units assigned
     # unless there is an accompanying fire or medical incident for the same call
     # this needs to be checked before the description check for other categories
     if len(units) == 0 and any(k in description for k in TRAFFIC_DESCRIPTION_KEYWORDS):
         return IncidentCategory.TRAFFIC
@@ -76,22 +75,7 @@
     # perform a basic description check
     if any(k in description for k in MEDICAL_DESCRIPTION_KEYWORDS):
         return IncidentCategory.MEDICAL
     if any(k in description for k in FIRE_DESCRIPTION_KEYWORDS):
         return IncidentCategory.FIRE
 
     return IncidentCategory.UNKNOWN
-
-
-def is_related_incident(a: Incident, b: Incident, delta: datetime.timedelta) -> bool:
-    """Determines if two incidents are related based on the intersection and time delta
-
-    :param a: The first incident
-    :param b: The second incident
-    :param delta: The time delta
-    :return: True if the incidents are related, False otherwise
-    :rtype: bool
-    """
-
-    if a.intersection is None or b.intersection is None:
-        return False
-    return a.intersection == b.intersection and abs(a.date - b.date) <= delta
```

### Comparing `lcwc-0.5/src/lcwc/utils/restadapter.py` & `lcwc-0.6/src/lcwc/utils/restadapter.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.5/src/lcwc/web/client.py` & `lcwc-0.6/src/lcwc/web/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import datetime
 import aiohttp
 import pytz
 from bs4 import BeautifulSoup
+from lcwc import Client
 from lcwc.category import IncidentCategory
-from lcwc.incident import Incident
+from lcwc.unit import Unit
+from lcwc.web.incident import WebIncident as Incident
 
 DATE_FORMAT = "%a, %b %d, %Y %H:%M"
 """ The date format used on the LCWC website """
 
 
-class Client:
+class WebClient(Client):
     """Client for scraping the live incident page"""
 
     URL = "https://www.lcwc911.us/live-incident-list"
     """ The URL of the live incident page """
 
+    @property
+    def name(self) -> str:
+        """Returns the name of the client"""
+        return "WebClient"
+
     async def get_incidents(
         self, session: aiohttp.ClientSession, timeout: int = 10
     ) -> list[Incident]:
         """Fetches the live incident page and returns a list of incidents
 
         :param session: The aiohttp session to use
         :param timeout: The timeout in seconds
@@ -76,29 +83,31 @@
                     date_row.text.strip(), DATE_FORMAT
                 )
                 local_dt = local_tz.localize(raw_date, is_dst=None)
                 date = local_dt.astimezone(pytz.utc)
 
                 description = incident_row.text.strip().strip()
 
-                # split location by street(s) and township (if applicable)
+                # split location by street(s) and municipality (if applicable)
                 location = [l.strip() for l in location_row.text.strip().split("\n")]
 
                 if len(location) == 1:
                     intersection = None
-                    township = location[0]
+                    municipality = location[0]
                 else:
                     intersection = location[0]
-                    township = location[1]
+                    municipality = location[1]
 
                 # we have to decode manually because of internal <br/> tags
-                units = [
+                unit_names = [
                     u.strip()
                     for u in units_row.decode_contents().strip().split("<br/>")
                 ]
 
+                units = [Unit(u) for u in unit_names if u != ""]
+
                 incident = Incident(
-                    category, date, description, township, intersection, units
+                    category, date, description, municipality, intersection, units
                 )
                 incidents.append(incident)
 
         return incidents
```

### Comparing `lcwc-0.5/src/lcwc.egg-info/PKG-INFO` & `lcwc-0.6/src/lcwc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.5
+Version: 0.6
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.5/src/lcwc.egg-info/SOURCES.txt` & `lcwc-0.6/src/lcwc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 src/lcwc/__init__.py
 src/lcwc/category.py
+src/lcwc/client.py
 src/lcwc/incident.py
+src/lcwc/unit.py
 src/lcwc.egg-info/PKG-INFO
 src/lcwc.egg-info/SOURCES.txt
 src/lcwc.egg-info/dependency_links.txt
 src/lcwc.egg-info/requires.txt
 src/lcwc.egg-info/top_level.txt
 src/lcwc/arcgis/__init__.py
 src/lcwc/arcgis/client.py
 src/lcwc/arcgis/incident.py
 src/lcwc/feed/__init__.py
 src/lcwc/feed/client.py
 src/lcwc/feed/incident.py
+src/lcwc/feed/utils/__init__.py
 src/lcwc/utils/__init__.py
 src/lcwc/utils/restadapter.py
 src/lcwc/web/__init__.py
-src/lcwc/web/client.py
+src/lcwc/web/client.py
+src/lcwc/web/incident.py
```

