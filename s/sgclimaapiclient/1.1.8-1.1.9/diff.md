# Comparing `tmp/sgclimaapiclient-1.1.8.tar.gz` & `tmp/sgclimaapiclient-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgclimaapiclient-1.1.8.tar", last modified: Tue Oct 26 14:58:20 2021, max compression
+gzip compressed data, was "sgclimaapiclient-1.1.9.tar", last modified: Tue Oct 26 15:02:47 2021, max compression
```

## Comparing `sgclimaapiclient-1.1.8.tar` & `sgclimaapiclient-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-26 14:58:20.925003 sgclimaapiclient-1.1.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1068 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      227 2021-10-26 14:58:20.921003 sgclimaapiclient-1.1.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      148 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      103 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2021-10-26 14:58:20.925003 sgclimaapiclient-1.1.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      740 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-26 14:58:20.921003 sgclimaapiclient-1.1.8/sgclimaapiclient/
--rw-r--r--   0 vsts      (1001) docker     (121)       76 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/sgclimaapiclient/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1587 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/sgclimaapiclient/baseapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12660 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/sgclimaapiclient/dataapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1096 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/sgclimaapiclient/modelsapi.py
--rw-r--r--   0 vsts      (1001) docker     (121)       21 2021-10-26 14:58:07.000000 sgclimaapiclient-1.1.8/sgclimaapiclient/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-26 14:58:20.921003 sgclimaapiclient-1.1.8/sgclimaapiclient.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)      227 2021-10-26 14:58:20.000000 sgclimaapiclient-1.1.8/sgclimaapiclient.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      422 2021-10-26 14:58:20.000000 sgclimaapiclient-1.1.8/sgclimaapiclient.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-10-26 14:58:20.000000 sgclimaapiclient-1.1.8/sgclimaapiclient.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-10-26 14:58:20.000000 sgclimaapiclient-1.1.8/sgclimaapiclient.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       64 2021-10-26 14:58:20.000000 sgclimaapiclient-1.1.8/sgclimaapiclient.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       17 2021-10-26 14:58:20.000000 sgclimaapiclient-1.1.8/sgclimaapiclient.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-26 15:02:47.037754 sgclimaapiclient-1.1.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1068 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      227 2021-10-26 15:02:47.037754 sgclimaapiclient-1.1.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      148 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)      103 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)       38 2021-10-26 15:02:47.037754 sgclimaapiclient-1.1.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      740 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-26 15:02:47.037754 sgclimaapiclient-1.1.9/sgclimaapiclient/
+-rw-r--r--   0 vsts      (1001) docker     (121)       76 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/sgclimaapiclient/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1587 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/sgclimaapiclient/baseapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12699 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/sgclimaapiclient/dataapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1096 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/sgclimaapiclient/modelsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       21 2021-10-26 15:02:33.000000 sgclimaapiclient-1.1.9/sgclimaapiclient/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-26 15:02:47.037754 sgclimaapiclient-1.1.9/sgclimaapiclient.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)      227 2021-10-26 15:02:47.000000 sgclimaapiclient-1.1.9/sgclimaapiclient.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      422 2021-10-26 15:02:47.000000 sgclimaapiclient-1.1.9/sgclimaapiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-10-26 15:02:47.000000 sgclimaapiclient-1.1.9/sgclimaapiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-10-26 15:02:46.000000 sgclimaapiclient-1.1.9/sgclimaapiclient.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       64 2021-10-26 15:02:47.000000 sgclimaapiclient-1.1.9/sgclimaapiclient.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       17 2021-10-26 15:02:47.000000 sgclimaapiclient-1.1.9/sgclimaapiclient.egg-info/top_level.txt
```

### Comparing `sgclimaapiclient-1.1.8/LICENSE` & `sgclimaapiclient-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sgclimaapiclient-1.1.8/setup.py` & `sgclimaapiclient-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `sgclimaapiclient-1.1.8/sgclimaapiclient/baseapi.py` & `sgclimaapiclient-1.1.9/sgclimaapiclient/baseapi.py`

 * *Files identical despite different names*

### Comparing `sgclimaapiclient-1.1.8/sgclimaapiclient/dataapi.py` & `sgclimaapiclient-1.1.9/sgclimaapiclient/dataapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,24 +71,24 @@
 
     def get_site_zones(self, site_id: int) -> dict:
         """
         Get all zones of a given site.
         \f
         :param site_id: Site id
         """
-        return self._call_json("/sites/{id}".format(id=site_id))
+        return self._call_json("/sites/{id}/zones".format(id=site_id))
 
     def get_site_equipments(self, site_id: int, equipment_type: str = None) -> dict:
         """
         Get all equipments of a given site.
         \f
         :param site_id: Site id
         """
         params = self._build_params(equipment_type=equipment_type)
-        return self._call_json("/sites/{id}".format(id=site_id), params=params)
+        return self._call_json("/sites/{id}/equipments".format(id=site_id), params=params)
 
     def download_site_data(self, site_id: int, start: Union[datetime, date, str],
                            end: Union[datetime, date, str]) -> pd.DataFrame:
         """
         Get the Site data for each Parameter given a date/timestamp range.
         Things to consider about the data:
 
@@ -183,15 +183,15 @@
     def get_zone_equipments(self, zone_id: int, equipment_type: str = None) -> dict:
         """
         Get all equipments of a given zone.
         \f
         :param zone_id: Zone id
         """
         params = self._build_params(equipment_type=equipment_type)
-        return self._call_json("/zones/{id}".format(id=zone_id), params=params)
+        return self._call_json("/zones/{id}/equipments".format(id=zone_id), params=params)
 
     def download_zone_data(self, zone_id: int, start: Union[datetime, date, str],
                            end: Union[datetime, date, str]) -> pd.DataFrame:
         """
         Get the Zone data for each Parameter given a date/timestamp range.
         Things to consider about the data:
 
@@ -253,15 +253,15 @@
 
     def get_gateway_parameters(self, gateway_id: int) -> dict:
         """
         Get all parameters of a given gateway.
         \f
         :param gateway_id: Gateway id
         """
-        return self._call_json("/gateways/{id}".format(id=gateway_id))
+        return self._call_json("/gateways/{id}/parameters".format(id=gateway_id))
 
     def list_parameters(self, site_id: int = None, gateway_id: int = None) -> dict:
         """
         List all the parameters.
         \f
         :param site_id: Filter by site based on its identifier
         :param gateway_id: Filter by gateway based on its identifier
```

### Comparing `sgclimaapiclient-1.1.8/sgclimaapiclient/modelsapi.py` & `sgclimaapiclient-1.1.9/sgclimaapiclient/modelsapi.py`

 * *Files identical despite different names*

