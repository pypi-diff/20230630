# Comparing `tmp/autotraders-1.5.5.tar.gz` & `tmp/autotraders-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.5.5.tar", last modified: Sun Jun 18 22:53:06 2023, max compression
+gzip compressed data, was "autotraders-1.6.0.tar", last modified: Thu Jun 29 22:40:49 2023, max compression
```

## Comparing `autotraders-1.5.5.tar` & `autotraders-1.6.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.395029 autotraders-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-18 22:52:54.000000 autotraders-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 22:53:06.395029 autotraders-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-18 22:52:54.000000 autotraders-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-18 22:52:54.000000 autotraders-1.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 22:53:06.395029 autotraders-1.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.242345 autotraders-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 22:40:34.000000 autotraders-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-29 22:40:49.242345 autotraders-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-29 22:40:34.000000 autotraders-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.234345 autotraders-1.6.0/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.234345 autotraders-1.6.0/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.238345 autotraders-1.6.0/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.238345 autotraders-1.6.0/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.238345 autotraders-1.6.0/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/ship_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.238345 autotraders-1.6.0/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-29 22:40:34.000000 autotraders-1.6.0/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.234345 autotraders-1.6.0/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 22:40:49.000000 autotraders-1.6.0/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-29 22:40:34.000000 autotraders-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:40:49.242345 autotraders-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:40:49.242345 autotraders-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-29 22:40:34.000000 autotraders-1.6.0/tests/test_util.py
```

### Comparing `autotraders-1.5.5/LICENSE` & `autotraders-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/PKG-INFO` & `autotraders-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.5
+Version: 1.6.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.5/README.md` & `autotraders-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/agent.py` & `autotraders-1.6.0/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/faction/__init__.py` & `autotraders-1.6.0/autotraders/faction/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from autotraders.error import SpaceTradersException
 from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.shared_models.trait import Trait
 
 
@@ -29,29 +30,22 @@
         self.is_recruiting = data["isRecruiting"]
 
     @staticmethod
     def all(session, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
-                + "my/contracts?limit="
-                + str(num_per_page)
-                + "&page="
-                + str(p)
-            )
-            r = session.get(
-                session.base_url
                 + "factions?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise IOError(j["error"]["message"])
+                raise SpaceTradersException(j["error"]["message"], r.status_code)
             factions = []
             for f in j["data"]:
                 faction = Faction(f["symbol"], session, f)
                 factions.append(faction)
             return factions, r.json()["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.5.5/autotraders/faction/contract.py` & `autotraders-1.6.0/autotraders/faction/contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
 
+from autotraders.error import SpaceTradersException
 from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.time import parse_time
 
 
@@ -52,19 +53,20 @@
             "deliver",
             data={"shipSymbol": symbol, "tradeSymbol": cargo_symbol, "units": amount},
         )
         self.update(j["data"]["contract"])
 
     @staticmethod
     def negotiate(ship_symbol, session):
-        j = session.post(
+        r = session.post(
             session.base_url + "my/ships/" + ship_symbol + "/negotiate/contract"
-        ).json()
+        )
+        j = r.json()
         if "error" in j:
-            raise IOError(j["error"]["message"])
+            raise SpaceTradersException(j["error"]["message"], r.status_code)
         c = Contract(j["data"]["contract"]["id"], session, j["data"]["contract"])
         return c
 
     def fulfill(self):
         j = self.post("fulfill")
         self.update(j["data"]["contract"])
 
@@ -76,15 +78,15 @@
                 + "my/contracts?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise IOError(j["error"]["message"])
+                raise SpaceTradersException(j["error"]["message"], r.status_code)
             contracts = []
             for contract in j["data"]:
                 c = Contract(contract["id"], session, contract)
                 contracts.append(c)
             return contracts, r.json()["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.5.5/autotraders/map/system.py` & `autotraders-1.6.0/autotraders/map/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Union
 
+from autotraders.error import SpaceTradersException
 from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.map.waypoint import Waypoint
 from autotraders.shared_models.map_symbol import MapSymbol
 
 
@@ -21,15 +22,17 @@
     ):
         self.symbol: MapSymbol = MapSymbol(symbol)
         super().__init__(session, "systems/" + str(self.symbol) + "/", data)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
-        self.waypoints = [Waypoint(w["symbol"], self.session, w) for w in data["waypoints"]]
+        self.waypoints = [
+            Waypoint(w["symbol"], self.session, w) for w in data["waypoints"]
+        ]
         self.x = data["x"]
         self.y = data["y"]
         self.factions = data["factions"]
         self.star_type = data["type"]
 
     @staticmethod
     def all(session, page: int = 1) -> PaginatedList:
@@ -39,15 +42,15 @@
                 + "systems?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise IOError(j["error"]["message"])
+                raise SpaceTradersException(j["error"]["message"], r.status_code)
             systems = []
             for system in j["data"]:
                 s = System(system["symbol"], session, system)
                 systems.append(s)
             return systems, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.5.5/autotraders/map/waypoint.py` & `autotraders-1.6.0/autotraders/map/waypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Union
 
+from autotraders.error import SpaceTradersException
 from autotraders.paginated_list import PaginatedList
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.trait import Trait
 
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.space_traders_entity import SpaceTradersEntity
 
@@ -41,15 +42,16 @@
         self.traits = None
         if "traits" in data:
             self.traits = []
             for trait in data["traits"]:
                 self.traits.append(Trait(trait))
         if self.traits is not None:
             self.marketplace = (
-                len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+                len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"])
+                > 0
             )
             self.shipyard = (
                 len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
             )
         else:
             self.marketplace = None
             self.shipyard = None
@@ -64,15 +66,15 @@
                 + "/waypoints?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise IOError(j["error"]["message"])
+                raise SpaceTradersException(j["error"]["message"], r.status_code)
             waypoints = []
             for w in j["data"]:
                 waypoint = Waypoint(w["symbol"], session, w)
                 waypoints.append(waypoint)
             return waypoints, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.5.5/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.6.0/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.6.0/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.6.0/autotraders/map/waypoint_types/marketplace.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,15 @@
     trade_goods: list[TradeGood]
 
     def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
         super().__init__(waypoint, "market", session, data)
 
     def update(self, data: dict = None):
         if data is None:
-            data = self.session.get(
-                self.session.base_url
-                + "systems/"
-                + self.location.system
-                + "/waypoints/"
-                + self.location.waypoint
-                + "/market"
-            ).json()["data"]
+            data = self.get()["data"]
         self.imports = []
         for i in data["imports"]:
             self.imports.append(i["symbol"])
         self.exports = []
         for i in data["exports"]:
             self.exports.append(i["symbol"])
         self.exchange = []
```

### Comparing `autotraders-1.5.5/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.6.0/autotraders/map/waypoint_types/shipyard.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,10 +37,10 @@
                 self.ships.append(ShipyardShip(ship))
 
     def purchase(self, ship_type: str):
         j = self.session.post(
             self.session.base_url + "my/ships",
             data={"shipType": ship_type, "waypointSymbol": self.location},
         ).json()
-        return Ship(j["data"]["ship"]["symbol"], self.session, j["data"]["ship"]), ShipyardTransaction(
-            j["data"]["transaction"]
-        )
+        return Ship(
+            j["data"]["ship"]["symbol"], self.session, j["data"]["ship"]
+        ), ShipyardTransaction(j["data"]["transaction"])
```

### Comparing `autotraders-1.5.5/autotraders/paginated_list.py` & `autotraders-1.6.0/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/session.py` & `autotraders-1.6.0/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/shared_models/map_symbol.py` & `autotraders-1.6.0/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/shared_models/transaction.py` & `autotraders-1.6.0/autotraders/shared_models/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from autotraders.shared_models.item import Item
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.time import parse_time
 
 
 class ShipyardTransaction:
     def __init__(self, data):
-        self.credits: int = data["price"]
+        if "price" in data:
+            self.credits: int = data["price"]
+        else:
+            self.credits: int = data["totalPrice"]
         self.waypoint_symbol: MapSymbol = MapSymbol(data["waypointSymbol"])
         self.ship_symbol: str = data["shipSymbol"]
-        self.agent_symbol: str = data["agentSymbol"]
+        if "agentSymbol" in data:
+            self.agent_symbol: str = data["agentSymbol"]
         self.timestamp = parse_time(data["timestamp"])
 
 
 class MarketTransaction:
     def __init__(self, data):
         self.waypoint_symbol: MapSymbol = MapSymbol(data["waypointSymbol"])
         self.ship_symbol: str = data["shipSymbol"]
```

### Comparing `autotraders-1.5.5/autotraders/ship/__init__.py` & `autotraders-1.6.0/autotraders/ship/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import json
 from typing import Union, Optional
 
 import requests
 
+from autotraders.error import SpaceTradersException
 from autotraders.paginated_list import PaginatedList
 from autotraders.shared_models.item import Item
 from autotraders.shared_models.transaction import MarketTransaction, ShipyardTransaction
 from autotraders.ship.cargo import Cargo
 from autotraders.ship.nav import Nav
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.map.system import System
@@ -46,14 +47,15 @@
 
 class Capabilities:
     """
     :ivar warp: can the ship warp
     :ivar jump: can the ship jump without a jump gate
     :ivar mine: can the ship mine (experimental)
     """
+
     def __init__(self, modules, mounts):
         warp_drives = [module for module in modules if "warp" in module.symbol.lower()]
         jump_drives = [module for module in modules if "jump" in module.symbol.lower()]
         mine = [mount for mount in mounts if "mine" in mount.symbol.lower()]
         self.warp = len(warp_drives) > 0
         self.jump = len(jump_drives) > 0
         self.mine = len(mine) > 0
@@ -140,41 +142,46 @@
             },
         )
         self.update(j["data"])
 
     def patch_navigation(self, new_flight_mode):
         r = self.session.patch(
             self.session.base_url + "my/ships/" + self.symbol + "/nav",
-            data=json.dumps({"flightMode": new_flight_mode})  # Requests is so dumb I spent 30 minutes debugging this
+            data=json.dumps(
+                {"flightMode": new_flight_mode}
+            )  # Requests is so dumb I spent 30 minutes debugging this
             # just to find that its requests fault for sending a body of "flightMode=DRIFT".
         )
         j = r.json()
         if "error" in j:
-            raise IOError(j["error"]["message"])
+            raise SpaceTradersException(j["error"]["message"], r.status_code)
         self.update({"nav": j["data"]})
 
     def dock(self):
         j = self.post("dock")
         self.update(j["data"])
 
     def orbit(self):
         j = self.post("orbit")
         self.update(j["data"])
 
     def extract(self, survey: Survey = None):
         if survey is None:
             j = self.post("extract")
         else:
-            j = self.post("extract", data={
-                "signature": survey.signature,
-                "symbol": survey.symbol,
-                "deposits": survey.deposits,
-                "expiration": survey.expiration.isoformat(),
-                "size": survey.size
-            })
+            j = self.post(
+                "extract",
+                data={
+                    "signature": survey.signature,
+                    "symbol": survey.symbol,
+                    "deposits": survey.deposits,
+                    "expiration": survey.expiration.isoformat(),
+                    "size": survey.size,
+                },
+            )
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return Item(
             j["data"]["extraction"]["yield"]["symbol"],
             j["data"]["extraction"]["yield"]["units"],
             None,
         )
@@ -265,15 +272,15 @@
         for ship in j["data"]["ships"]:
             s = Ship(ship["symbol"], self.session, ship)
             ships.append(s)
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return ships
 
     def update_ship_cooldown(self):
-        try: # TODO: get more elegant solution
+        try:  # TODO: get more elegant solution
             j = self.get("cooldown")
             self.reactor.cooldown = parse_time(j["data"]["expiration"])
         except requests.exceptions.JSONDecodeError:
             self.reactor.cooldown = None
 
     def install_mount(self, mount_symbol: str):
         j = self.post("mounts/install", data={"symbol": mount_symbol})
@@ -294,15 +301,15 @@
                 + "my/ships?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise IOError(j["error"]["message"])
+                raise SpaceTradersException(j["error"]["message"], r.status_code)
             ships = []
             for ship in j["data"]:
                 s = Ship(ship["symbol"], session, ship)
                 ships.append(s)
             return ships, r.json()["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.5.5/autotraders/ship/cargo.py` & `autotraders-1.6.0/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/ship/nav.py` & `autotraders-1.6.0/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/ship/ship_components.py` & `autotraders-1.6.0/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders/space_traders_entity.py` & `autotraders-1.6.0/autotraders/space_traders_entity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 
 from autotraders import AutoTradersSession
+from autotraders.error import SpaceTradersException
 
 
 class SpaceTradersEntity:
     def __init__(self, session: AutoTradersSession, action_url, data=None):
         self.session: AutoTradersSession = session
         self.action_url = session.base_url + action_url
         if self.action_url[-1] != "/":
@@ -18,29 +19,29 @@
             )
         else:
             r = self.session.get(
                 self.action_url + action,
             )
         j = r.json()
         if "error" in j:
-            raise IOError(j["error"]["message"])
+            raise SpaceTradersException(j["error"], r.status_code)
         return j
 
     def post(self, action: str, data=None) -> dict:
         self.session.headers["Content-Type"] = "application/json"
         if data is not None:
             r = self.session.post(
                 self.action_url + action,
                 data=json.dumps(data),
             )
         else:
             r = self.session.post(self.action_url + action)
         j = r.json()
         if "error" in j:
-            raise IOError(j["error"]["message"])
+            raise SpaceTradersException(j["error"]["message"], r.status_code)
         return j
 
     def update(self, data: dict = None):
         """
         :param data: If you have data from an api requests, you can provide it here. If not provided, an API request
         will be sent.
         :raise IOException: If the server fails
```

### Comparing `autotraders-1.5.5/autotraders/status.py` & `autotraders-1.6.0/autotraders/status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 
 import requests
 
+from autotraders.error import SpaceTradersException
 from autotraders.time import parse_time
 
 
 class LeaderboardPlayer:
     symbol: str
     value: int
 
@@ -63,15 +64,15 @@
     """returns the API status, with reset dates, see the Status class for more info."""
     if session is None:
         r = requests.get("https://api.spacetraders.io/v2/")
     else:
         r = session.get("https://api.spacetraders.io/v2/")
     j = r.json()
     if "error" in j:
-        raise IOError(j["error"]["message"])
+        raise SpaceTradersException(j["error"]["message"], r.status_code)
     s = Status()
     s.status = j["status"]
     s.version = j["version"]
     s.reset_date = parse_time(j["resetDate"])
     s.description = j["description"]
     s.stats = j["stats"]
     s.next_reset = parse_time(j["serverResets"]["next"])
```

### Comparing `autotraders-1.5.5/autotraders/util.py` & `autotraders-1.6.0/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/autotraders.egg-info/PKG-INFO` & `autotraders-1.6.0/autotraders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.5
+Version: 1.6.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.5/autotraders.egg-info/SOURCES.txt` & `autotraders-1.6.0/autotraders.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 autotraders/__init__.py
 autotraders/agent.py
+autotraders/error.py
 autotraders/paginated_list.py
 autotraders/session.py
 autotraders/space_traders_entity.py
 autotraders/status.py
 autotraders/time.py
 autotraders/util.py
 autotraders.egg-info/PKG-INFO
@@ -21,14 +22,15 @@
 autotraders/map/waypoint.py
 autotraders/map/waypoint_types/__init__.py
 autotraders/map/waypoint_types/jumpgate.py
 autotraders/map/waypoint_types/marketplace.py
 autotraders/map/waypoint_types/shipyard.py
 autotraders/shared_models/item.py
 autotraders/shared_models/map_symbol.py
+autotraders/shared_models/ship_symbol.py
 autotraders/shared_models/symbol.py
 autotraders/shared_models/trait.py
 autotraders/shared_models/transaction.py
 autotraders/ship/__init__.py
 autotraders/ship/cargo.py
 autotraders/ship/nav.py
 autotraders/ship/ship_components.py
```

### Comparing `autotraders-1.5.5/pyproject.toml` & `autotraders-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.5.5"
+version = "1.6.0"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.5.5/tests/test_init.py` & `autotraders-1.6.0/tests/test_init.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # import time
 
 import pytest
 
 from autotraders import get_status
 from autotraders.agent import Agent
+from autotraders.error import SpaceTradersException
 from autotraders.faction import Faction
 from autotraders.session import get_session
 
 
 @pytest.fixture
 def session():
     s = get_session("TEST")
@@ -18,15 +19,15 @@
 
 def test_invalid_api_key():
     s = get_session("INVALID TOKEN")
     try:
         Agent(s)
         assert False  # shouldn't complete successfully
     except Exception as e:
-        assert type(e) is IOError
+        assert type(e) is SpaceTradersException
 
 
 def test_get_status():
     status = get_status()
     assert status.version == "v2"
```

### Comparing `autotraders-1.5.5/tests/test_map.py` & `autotraders-1.6.0/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/tests/test_ship.py` & `autotraders-1.6.0/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.5/tests/test_util.py` & `autotraders-1.6.0/tests/test_util.py`

 * *Files identical despite different names*

