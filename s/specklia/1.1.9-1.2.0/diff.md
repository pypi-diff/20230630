# Comparing `tmp/specklia-1.1.9.tar.gz` & `tmp/specklia-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.1.9.tar", last modified: Fri Jun 30 12:56:33 2023, max compression
+gzip compressed data, was "specklia-1.2.0.tar", last modified: Fri Jun 30 15:16:51 2023, max compression
```

## Comparing `specklia-1.1.9.tar` & `specklia-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:56:33.536222 specklia-1.1.9/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-30 12:56:30.000000 specklia-1.1.9/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 12:56:33.536222 specklia-1.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-30 12:56:30.000000 specklia-1.1.9/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-30 12:56:33.536222 specklia-1.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-30 12:56:30.000000 specklia-1.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:56:33.536222 specklia-1.1.9/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-30 12:56:30.000000 specklia-1.1.9/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-30 12:56:30.000000 specklia-1.1.9/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    35334 2023-06-30 12:56:30.000000 specklia-1.1.9/specklia/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:56:33.536222 specklia-1.1.9/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:56:33.536222 specklia-1.1.9/tests/
--rw-r--r--   0 root         (0) root         (0)    10184 2023-06-30 12:56:30.000000 specklia-1.1.9/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6632 2023-06-30 12:56:30.000000 specklia-1.1.9/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:16:51.493293 specklia-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-30 13:03:23.000000 specklia-1.2.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 15:16:51.493293 specklia-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-30 13:03:23.000000 specklia-1.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-30 15:16:51.493293 specklia-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-30 13:03:23.000000 specklia-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:16:51.493293 specklia-1.2.0/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-30 13:03:23.000000 specklia-1.2.0/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-30 13:03:23.000000 specklia-1.2.0/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    35189 2023-06-30 13:03:23.000000 specklia-1.2.0/specklia/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:16:51.493293 specklia-1.2.0/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-30 15:16:51.000000 specklia-1.2.0/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:16:51.493293 specklia-1.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)    10184 2023-06-30 13:03:23.000000 specklia-1.2.0/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6632 2023-06-30 13:03:23.000000 specklia-1.2.0/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.1.9/LICENCE` & `specklia-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.1.9/PKG-INFO` & `specklia-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.9
+Version: 1.2.0
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.1.9/README.md` & `specklia-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.1.9/setup.py` & `specklia-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.9/specklia/_websocket_helpers.py` & `specklia-1.2.0/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.9/specklia/client.py` & `specklia-1.2.0/specklia/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,32 +20,32 @@
 
 
 class Specklia:
     """
     Client for the Specklia webservice.
 
     Specklia is a geospatial point cloud database designed for Academic use.
-    Further details are available at https://specklia.earthwave.co.uk.
+    Further details are available at https://specklia.earthwave.co.uk/static/docs/index.html.
     """
 
     def __init__(
             self: Specklia,
             auth_token: str,
-            url: Optional[str] = 'https://specklia.earthwave.co.uk') -> None:
+            url: str = 'https://specklia.earthwave.co.uk') -> None:
         """
         Create a new Specklia client object.
 
         This object is a Python client for connecting to Specklia's API.
 
         Parameters
         ----------
         auth_token : str
             The authentication token to use to authorise calls to Specklia.
-            Obtained via the official specklia website, which is currently https://specklia.earthwave.co.uk.
-        url : Optional[str]
+            Obtained via https://specklia.earthwave.co.uk.
+        url : str
             The url where Specklia is running, by default the URL of the Specklia server.
 
         Examples
         --------
         To start using Specklia, we first need to navigate to https://specklia.earthwave.co.uk and follow the
         instructions to generate a Specklia API key.
 
@@ -174,15 +174,15 @@
             The data resulting from the query
             Metadata for the query, including a list of sources for the data
 
         Examples
         --------
         We can utilise client.list_datasets() to determine which dataset we wish to query and narrow down our
         query parameters. The output from the call will include all the necessary details of a dataset, such as its
-        spatio-temporal coverage and available columns.
+        space-time coverage and available columns.
 
         For example, let's say we have found a dataset which has data in our area of interest in December 2022 and we
         are specifically interested in its 'air_quality' column. We can query this as such::
 
             >>> from shapely import Polygon
             >>> from datetime import datetime
 
@@ -574,15 +574,15 @@
                   'new_privileges': new_privileges},
             headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
         _log.info('Updated user ID %s privileges to %s within group ID %s.',
                   user_to_update_id, new_privileges, group_id)
         return response.text.strip('\n"')
 
-    def delete_user_from_group(self: Specklia, group_id: str, user_to_delete_id: str,) -> str:
+    def delete_user_from_group(self: Specklia, group_id: str, user_to_delete_id: str) -> str:
         """
         Remove a user from an existing group.
 
         You must have ADMIN permissions within the group in order to do this.
 
         Parameters
         ----------
@@ -659,24 +659,23 @@
             The name the user provides for the dataset.
             Must contain alphanumeric characters, spaces, underscores and hyphens only.
         description : str
             A description of the dataset.
             Must contain alphanumeric characters, spaces, underscores and hyphens only.
         columns : Optional(List[Dict[str, str]])),
             A list where each item is an additional column the user wishes to add to the dataset,
-            beyond the mandatory columns of 'lat', 'lon' and 'timestamp',
-            which are EPSG4326 latitude, longitude and POSIX timestamp as an integer respectively.
+            beyond the mandatory EPSG4326 latitude, longitude and POSIX timestamp.
             A list of columns should follow the format::
 
                 [{'name': 'elevation', 'type': 'float', 'description': 'elevation', 'unit': 'metres'},
                 {'name': 'remarks', 'type': 'str', 'description': 'per-row remarks', 'unit': 'NA'}]
 
             Where valid values for 'type' are 'string', 'float' and 'int' and the other three fields are strings,
             which must contain alphanumeric characters, spaces, underscores and hyphens only.
-            Please do not create explicit EPSG:4326 columns (e.g. 'lat', 'lon') or POSIX timestamp columns
+            Please do not create explicit EPSG4326 columns (e.g. 'lat', 'lon') or POSIX timestamp columns
             as these are unnecessary repetitions of Specklia default columns.
 
         Returns
         -------
         str
             The unique ID of the newly created dataset.
 
@@ -699,15 +698,15 @@
         or move it to another group through client.update_dataset_ownership().
 
         If nothing is passed to the optional parameter 'columns', the created dataset will only have three columns: lat,
         long, and time.
         """
         if columns and any(x in ['lat', 'lon', 'long', 'latitude', 'longitude', 'timestamp', 'posix']
                            for x in [col['name'].lower() for col in columns]):
-            message = ("Please refrain from creating explicit EPSG:4326 or POSIX timestamp columns "
+            message = ("Please refrain from creating explicit EPSG4326 or POSIX timestamp columns "
                        "as these are repetitious of Specklia's default columns.")
             _log.warning(message)
             warnings.warn(message, stacklevel=1)
 
         response = requests.post(
             self.server_url + "/metadata",
             json={'dataset_name': dataset_name,
```

### Comparing `specklia-1.1.9/specklia.egg-info/PKG-INFO` & `specklia-1.2.0/specklia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.9
+Version: 1.2.0
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.1.9/tests/test_client.py` & `specklia-1.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.9/tests/test_websocket_helpers.py` & `specklia-1.2.0/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

