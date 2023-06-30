# Comparing `tmp/specklia-1.1.8.tar.gz` & `tmp/specklia-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.1.8.tar", last modified: Fri Jun 30 10:44:43 2023, max compression
+gzip compressed data, was "specklia-1.1.9.tar", last modified: Fri Jun 30 12:56:33 2023, max compression
```

## Comparing `specklia-1.1.8.tar` & `specklia-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 10:44:43.617897 specklia-1.1.8/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-30 10:44:40.000000 specklia-1.1.8/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 10:44:43.617897 specklia-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-30 10:44:40.000000 specklia-1.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-30 10:44:43.617897 specklia-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-30 10:44:40.000000 specklia-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 10:44:43.617897 specklia-1.1.8/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-30 10:44:40.000000 specklia-1.1.8/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-30 10:44:40.000000 specklia-1.1.8/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    24587 2023-06-30 10:44:40.000000 specklia-1.1.8/specklia/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 10:44:43.617897 specklia-1.1.8/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 10:44:43.000000 specklia-1.1.8/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-30 10:44:43.000000 specklia-1.1.8/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 10:44:43.000000 specklia-1.1.8/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-30 10:44:43.000000 specklia-1.1.8/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-30 10:44:43.000000 specklia-1.1.8/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 10:44:43.617897 specklia-1.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)    10184 2023-06-30 10:44:40.000000 specklia-1.1.8/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6632 2023-06-30 10:44:40.000000 specklia-1.1.8/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:56:33.536222 specklia-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-30 12:56:30.000000 specklia-1.1.9/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 12:56:33.536222 specklia-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-30 12:56:30.000000 specklia-1.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-30 12:56:33.536222 specklia-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-30 12:56:30.000000 specklia-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:56:33.536222 specklia-1.1.9/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-30 12:56:30.000000 specklia-1.1.9/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-30 12:56:30.000000 specklia-1.1.9/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    35334 2023-06-30 12:56:30.000000 specklia-1.1.9/specklia/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:56:33.536222 specklia-1.1.9/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-30 12:56:33.000000 specklia-1.1.9/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:56:33.536222 specklia-1.1.9/tests/
+-rw-r--r--   0 root         (0) root         (0)    10184 2023-06-30 12:56:30.000000 specklia-1.1.9/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6632 2023-06-30 12:56:30.000000 specklia-1.1.9/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.1.8/LICENCE` & `specklia-1.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.1.8/PKG-INFO` & `specklia-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.1.8/README.md` & `specklia-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.1.8/setup.py` & `specklia-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.8/specklia/_websocket_helpers.py` & `specklia-1.1.9/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.8/specklia/client.py` & `specklia-1.1.9/specklia/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,14 +39,28 @@
         Parameters
         ----------
         auth_token : str
             The authentication token to use to authorise calls to Specklia.
             Obtained via the official specklia website, which is currently https://specklia.earthwave.co.uk.
         url : Optional[str]
             The url where Specklia is running, by default the URL of the Specklia server.
+
+        Examples
+        --------
+        To start using Specklia, we first need to navigate to https://specklia.earthwave.co.uk and follow the
+        instructions to generate a Specklia API key.
+
+        The key should then be kept somewhere safe where only we can access it, and needs to be passed each time we
+        instantiate our Specklia client.
+
+        If we save our key to a file, we can then utilise it as such::
+
+            >>> with open("our_auth_token.jwt") as fh:
+            ...     user_auth_token = fh.read()
+            >>> client = Specklia(auth_token=user_auth_token)
         """
         self.server_url = url
         self.auth_token = auth_token
         self._data_streaming_timeout_s = 3600
         _log.info('New Specklia client created.')
 
     @property
@@ -81,14 +95,33 @@
         group_id : str
             The UUID of the group for which to list users.
 
         Returns
         -------
         pd.DataFrame
             A dataframe describing users within a group.
+
+        Examples
+        --------
+        To use this endpoint, we need to be an ADMIN of a group and know its ID.
+
+        By default, we are the ADMIN of our own personal group, the name of which is the same as our user_id, as well
+        as of any group that we create. Other users may also give us ADMIN privileges in their groups through
+        client.add_user_to_group() and client.update_user_privileges().
+
+        If we know the name of the group but not its ID, we can determine this by calling client.list_groups() and
+        filtering results.
+
+        We can then run::
+
+            >>> users = client.list_users(group_id=GROUP_ID)
+
+        The result will contain the ID and privileges level of each user that is within our group. We can then utilise
+        client.delete_user_from_group(), client.add_user_to_group(), and client.update_user_privileges to make any
+        desired changes.
         """
         response = requests.get(
             self.server_url + "/users",
             headers={"Authorization": "Bearer " + self.auth_token},
             params={'group_id': group_id})
         _check_response_ok(response)
         _log.info('listed users within group_id %s.', group_id)
@@ -118,30 +151,65 @@
             The minimum datetime for the query. Only points occurring after this datetime will be returned.
         max_datetime : datetime
             The maximum datetime for the query. Only points occurring before this datetime will be returned.
         columns_to_return : List[str]
             A list of dataset columns to return. If empty, all columns are returned.
         additional_filters: List[Dict[str, Union[float, str]]]
             Additional filters to apply to the data. These operate on additional rows in the data.
-            A list of dicts of the form {'column': str, 'operator': str, 'threshold': Union[float, str]} where:
-                'column' is the name of a column that occurs within the dataset
-                'operator' is a comparison operator, one of '>', '<', '=', '!=', '>=', '<='
-                'threshold' is the value the column will be compared against.
+            A list of dicts of the form : {'column': str, 'operator': str, 'threshold': Union[float, str]}, where:
+
+            * 'column' is the name of a column that occurs within the dataset
+            * 'operator' is a comparison operator, one of '>', '<', '=', '!=', '>=', '<='
+            * 'threshold' is the value the column will be compared against.
+
             These conditions are applied to the data using logical AND.
 
         Raises
         ------
         RuntimeError
             If the query failed for some reason.
 
         Returns
         -------
         Tuple[gpd.GeoDataFrame, Dict]
             The data resulting from the query
             Metadata for the query, including a list of sources for the data
+
+        Examples
+        --------
+        We can utilise client.list_datasets() to determine which dataset we wish to query and narrow down our
+        query parameters. The output from the call will include all the necessary details of a dataset, such as its
+        spatio-temporal coverage and available columns.
+
+        For example, let's say we have found a dataset which has data in our area of interest in December 2022 and we
+        are specifically interested in its 'air_quality' column. We can query this as such::
+
+            >>> from shapely import Polygon
+            >>> from datetime import datetime
+
+            >>> query_start_time = datetime(2022, 12, 15)
+            >>> query_end_time = datetime(2022, 12, 20)
+            >>> query_polygon = Polygon(((-1, -1), (-1, 2), (2, 2), (2, -1), (-1, -1)))
+
+            >>> all_points_in_dataset = client.query_dataset(dataset_id=dataset_id,
+            ...                                              epsg4326_polygon=query_polygonm
+            ...                                              min_datetime=query_start_time,
+            ...                                              max_datetime=query_end_time,
+            ...                                              columns_to_return=['air_quality'],
+            ...                                              additional_filters=[])
+
+        We should always pick our query polygon and time window carefully, based on our use-case.
+
+        Where possible, we should also utilise the additional_filters parameter to filter data down further
+        before retrieval. For example, if our dataset has a column 'bird_type' and we know we are only interested in
+        swallows, we should pass::
+
+            additional_filters=[{'column': 'bird_type', 'operator': '=', 'threshold': 'swallow'}].
+
+        This will ensure fast querying and minimise the amount of data streamed back to our device.
         """
         # note the use of json.loads() here, so effectively converting the geojson
         # back into a dictionary of JSON-compatible types to avoid "double-JSONing" it.
         ws = simple_websocket.Client(
             self.server_url.replace("http://", "ws://") + "/query",
             headers={"Authorization": "Bearer " + self.auth_token})
         _websocket_helpers.send_object_to_websocket(ws, {
@@ -285,14 +353,24 @@
         group_name : str
             The new group's name. Must contain alphanumeric characters, spaces, underscores and hyphens only.
 
         Returns
         -------
         str
             The unique ID of the newly created group
+
+        Examples
+        --------
+        To create a new group, we run::
+
+            >>> client.create_group(group_name='important_group')
+            group_id
+
+        The endpoint will return the new group's unique ID, auto-generated by Specklia. We can pass this ID to other
+        Specklia endpoints to modify the group, its members, and datasets.
         """
         response = requests.post(self.server_url + "/groups", json={'group_name': group_name},
                                  headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
         _log.info('created new group with name %s.', group_name)
         return response.text.strip('\n"')
 
@@ -309,14 +387,22 @@
         new_group_name : str
             Desired new name of group. Must contain alphanumeric characters, spaces, underscores and hyphens only.
 
         Returns
         -------
         str
             Response from server
+
+        Examples
+        --------
+        To change the name of any group of which we are an ADMIN, we run::
+
+            >>> client.update_group_name(group_id=GROUP_ID, new_group_name='much_better_name')
+
+        The group's unique ID, users, and datasets will remain unchanged.
         """
         response = requests.put(
             self.server_url + "/groups",
             json={'group_id': group_id, 'new_group_name': new_group_name},
             headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
         _log.info('updated name of group ID %s to %s.', group_id, new_group_name)
@@ -333,14 +419,23 @@
         group_id : str
             The UUID of group to delete
 
         Returns
         -------
         str
             The response from the server.
+
+        Examples
+        --------
+        To delete an existing group of which we are an admin, we run::
+
+            >>> client.delete_group(group_id=GROUP_ID)
+
+        The above will additionally delete any datasets owned by the group at the time of the deletion. Users within the
+        group will be removed from it, but left unchanged otherwise.
         """
         response = requests.delete(
             self.server_url + "/groups", headers={"Authorization": "Bearer " + self.auth_token},
             json={'group_id': group_id})
         _check_response_ok(response)
         _log.info('deleted group ID %s', group_id)
         return response.text.strip('\n"')
@@ -349,41 +444,73 @@
         """
         List all of the groups that you are part of.
 
         Returns
         -------
         pd.DataFrame
             A dataframe describing the groups the user is part of.
+
+        Examples
+        --------
+        Running client.list_groups() returns a dataframe with all the groups we are a member of. Each group
+        in the result is described by a group_name and a group_id.
+
+        By default, each user is a member of their personal group, with group_name equal to their user_id, as well the
+        special all_users group.
+
+        If we know a group's name but not its ID, we can call client.list_groups() and filter down the results::
+
+            >>> groups_i_belong_to_df = client.list_groups()
+            >>> name_of_group_to_find = "university_of_edinburgh"
+            >>> desired_group_id = groups_i_belong_to_df[
+            ... groups_i_belong_to_df['group_name'] == name_of_group_to_find]['group_id'].iloc[0]
+
+        We can now pass this ID to other Specklia endpoints to modify the group, its members, and datasets.
         """
         response = requests.get(
             self.server_url + "/groupmembership", headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
         _log.info('listed groups that user is part of.')
         return pd.DataFrame(response.json()).convert_dtypes()
 
     def add_user_to_group(self: Specklia, group_id: str, user_to_add_id: str) -> str:
         """
         Add a user to an existing group.
 
         You must have ADMIN permissions within the group in order to do this.
-        The user will initially be granted READ_ONLY permissions within the group.
-        Use Specklia.update_user_privileges() to change this after you have moved them into the group.
+
+        The user will initially be granted READ_ONLY permissions within the group. Use
+        Specklia.update_user_privileges() to change this after you have moved them into the group.
 
         Parameters
         ----------
-        group_id: str
+        group_id : str
             The group's UUID
-
         user_to_add_id : str
             UUID of user to add to group
 
         Returns
         -------
         str
             The response from the server
+
+        Examples
+        --------
+        As an ADMIN of a group, we might wish to add other users to it so they are able to access the group's datasets.
+
+        We have to ask a user for their ID before we can add them to our group. If they wish to be added, they can
+        determine their ID through other_users_client.user_id and share the result with us.
+
+        Once we have this information, we can run::
+
+            >>> client.add_user_to_group(group_id=GROUP_ID, user_to_add_id=USER_ID)
+
+        By default, the newly added user will have READ_ONLY permissions within our group. If we wish for them to be
+        able to write to the group's datasets or manage users within the group, we can update their privileges via
+        client.update_user_privileges().
         """
         response = requests.post(self.server_url + "/groupmembership",
                                  json={'group_id': group_id, "user_to_add_id": user_to_add_id},
                                  headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
         _log.info('added user ID %s to group ID %s', user_to_add_id, group_id)
         return response.text.strip('\n"')
@@ -391,35 +518,58 @@
     def update_user_privileges(self: Specklia, group_id: str, user_to_update_id: str, new_privileges: str) -> str:
         """
         Update a user's privileges within a particular group.
 
         You must have ADMIN permissions within the group in order to do this.
 
         These privileges determine what a user can do with the datasets and users in the group:
-        - READ_ONLY means that the user can read the datasets, but cannot write to them,
-          or change properties of the group.
-        - READ_WRITE means that the user can write to existing datasets as well as read from them,
-          but cannot change the properties of the group. Users with READ_WRITE permissions cannot create or destroy
-          whole datasets within a group.
-        - ADMIN means that the user can add and remove other users from the group, can change their privileges,
-          and can add and remove datasets from the group.
+
+        * READ_ONLY means that the user can read the datasets, but cannot write to them, or change properties of the
+          group.
+        * READ_WRITE means that the user can write to existing datasets as well as read from them, but cannot change the
+          properties of the group. Users with READ_WRITE permissions cannot create or destroy whole datasets within a
+          group.
+        * ADMIN means that the user can add and remove other users from the group, can change their privileges, and can
+          add and remove datasets from the group.
 
         Parameters
         ----------
         group_id : str
             The group's UUID
         user_to_update_id : str
             UUID of user to update privileges for
         new_privileges : str
             New privileges of the users. Must be 'READ_ONLY', 'READ_WRITE' or 'ADMIN'.
 
         Returns
         -------
         str
             Response from server
+
+        Examples
+        --------
+        When we use client.add_user_to_group() to add a user to a group of which we are an ADMIN, they
+        are automatically given READ_ONLY privileges. This means they can read the group's datasets, but not modify
+        them.
+
+        If we wish for the user to be able to add, delete, and modify points in the group's datasets, but not delete
+        the datasets themselves, we can give them READ_WRITE privileges::
+
+            >>> client.update_user_privileges(group_id=GROUP_ID,
+            ...                               user_to_update_id=USER_ID,
+            ...                               new_privileges='READ_WRITE')
+
+        If we wish for the user to additionally be able to modify users and datasets within the group, or even delete
+        the group itself, we can give them ADMIN privileges::
+
+            >>> client.update_user_privileges(group_id=GROUP_ID,
+            ...                               user_to_update_id=USER_ID,
+            ...                               new_privileges='ADMIN')
+
+        We should always aim to grant users the lowest privileges necessary.
         """
         response = requests.put(
             self.server_url + "/groupmembership",
             json={'group_id': group_id,
                   "user_to_update_id": user_to_update_id,
                   'new_privileges': new_privileges},
             headers={"Authorization": "Bearer " + self.auth_token})
@@ -441,14 +591,29 @@
         user_to_delete_id : str
             UUID of user to delete from group
 
         Returns
         -------
         str
             The response from the server.
+
+        Examples
+        --------
+        To utilise this function, we need to know the ID of the group as well as the ID of the user we would like to
+        remove from it.
+
+        To determine the group ID, we can use the client.list_groups() endpoint and filter the results.
+
+        Once we have the group ID, we can call client.list_users(group_id=DETERMINED_GROUP_ID), which lists
+        IDs and privileges of all users within a group, to determine the desired user ID.
+
+        Once we determine who to remove, we run::
+
+            >>> client.delete_user_group_group(group_id=DETERMINED_GROUP_ID, user_to_delete_id=DETERMINED_USER_ID)
+
         """
         response = requests.delete(
             self.server_url + "/groupmembership", headers={"Authorization": "Bearer " + self.auth_token},
             json={'group_id': group_id, "user_to_delete_id": user_to_delete_id})
         _check_response_ok(response)
         _log.info('Deleted user ID %s from group ID %s.', user_to_delete_id, group_id)
         return response.text.strip('\n"')
@@ -475,46 +640,70 @@
             self: Specklia, dataset_name: str, description: str,
             columns: Optional(List[Dict[str, str]]) = None) -> str:
         """
         Create a dataset.
 
         Specklia datasets contain point cloud data.
         When you create the dataset, you must specify the fields within the data.
-        After you have created the dataset, you'll probably want to add data to it
-        using Specklia.add_points_to_dataset()
+
+        After you have created the dataset, you'll probably want to add data to it using
+        Specklia.add_points_to_dataset().
 
         When a dataset is first created, it will be owned by a group with its group_name matching your user ID.
         You have ADMIN permissions within this group. In order for other people to access this dataset, you must
-        either move it into another group using Specklia.update_dataset_ownership(), or add a user to your personal
-        group using Specklia.add_user_to_group().
+        either move it into another group using Specklia.update_dataset_ownership(), or add a user to your
+        personal group using Specklia.add_user_to_group().
 
         Parameters
         ---------
         dataset_name : str
             The name the user provides for the dataset.
             Must contain alphanumeric characters, spaces, underscores and hyphens only.
         description : str
             A description of the dataset.
             Must contain alphanumeric characters, spaces, underscores and hyphens only.
         columns : Optional(List[Dict[str, str]])),
             A list where each item is an additional column the user wishes to add to the dataset,
             beyond the mandatory columns of 'lat', 'lon' and 'timestamp',
             which are EPSG4326 latitude, longitude and POSIX timestamp as an integer respectively.
-            A list of columns should follow the format: [
-                {'name': 'elevation', 'type': 'float', 'description': 'elevation', 'unit': 'metres'},
+            A list of columns should follow the format::
+
+                [{'name': 'elevation', 'type': 'float', 'description': 'elevation', 'unit': 'metres'},
                 {'name': 'remarks', 'type': 'str', 'description': 'per-row remarks', 'unit': 'NA'}]
+
             Where valid values for 'type' are 'string', 'float' and 'int' and the other three fields are strings,
             which must contain alphanumeric characters, spaces, underscores and hyphens only.
             Please do not create explicit EPSG:4326 columns (e.g. 'lat', 'lon') or POSIX timestamp columns
             as these are unnecessary repetitions of Specklia default columns.
 
         Returns
         -------
         str
             The unique ID of the newly created dataset.
+
+        Examples
+        --------
+        To create a dataset, we must choose a name, and then provide a description and a list of all of its columns
+        beyond 'lat', 'lon', and 'time'. For example::
+
+            >>> client.create_dataset(
+            ...     dataset_name='my_air_dataset',
+            ...     description='Dataset containing air quality measurements gathered for Stop Pollution project',
+            ...     columns=[
+            ...         {'name': 'air_quality', 'type': 'int', 'description': 'Air Quality Index value', 'unit': 'AQI'},
+            ...         {'name': 'air_temperature', 'type': 'float', 'description': 'Air temperature', 'unit': 'C'},
+            ...         {'name': 'remarks', 'type': 'str', 'description': 'per-row remarks', 'unit': 'NA'}])
+            dataset_id
+
+        The above has created a new dataset, by default owned by our personal group - the group whose name matches our
+        user ID.  We can use the returned dataset_id to write data to the dataset with client.add_points_to_dataset()
+        or move it to another group through client.update_dataset_ownership().
+
+        If nothing is passed to the optional parameter 'columns', the created dataset will only have three columns: lat,
+        long, and time.
         """
         if columns and any(x in ['lat', 'lon', 'long', 'latitude', 'longitude', 'timestamp', 'posix']
                            for x in [col['name'].lower() for col in columns]):
             message = ("Please refrain from creating explicit EPSG:4326 or POSIX timestamp columns "
                        "as these are repetitious of Specklia's default columns.")
             _log.warning(message)
             warnings.warn(message, stacklevel=1)
@@ -545,14 +734,36 @@
         new_owning_group_id : str
             The group UUID the user wishes to change the dataset ownership tot
 
         Returns
         -------
         str
             The response from the server
+
+        Examples
+        --------
+        By default, each dataset we create belongs to our personal group - the group whose name is the same as our user
+        ID. To give another user access to our dataset, we can either add them to our personal group through
+        client.add_user_to_group(), or change the dataset's ownership, moving it to a different group of which
+        they are a member.
+
+        Let's say our friend Bob has given us his ID, BOBS_ID, and we wish to give him access to our important dataset.
+        We can do this as follows::
+
+            >>> important_dataset_id = client.create_dataset(
+                                                    dataset_name='important_dataset',
+            ...                                     description='Dataset containing greatest secrets of the world')
+            >>> important_group_id = client.create_group(group_name='important_group')
+
+            >>> client.add_user_to_group(group_id=important_group_id,
+            ...                          user_to_add_id=BOBS_ID))
+
+            >>> client.update_dataset_ownership(dataset_id=important_dataset_id,
+            ...                                 group_id=important_group_id)
+
         """
         response = requests.put(
             self.server_url + "/metadata",
             json={'dataset_id': dataset_id,
                   'new_owning_group_id': new_owning_group_id},
             headers={"Authorization": "Bearer " + self.auth_token}
         )
@@ -571,14 +782,24 @@
         dataset_id : str
             The UUID of the dataset the user wishes to delete
 
         Returns
         -------
         str
             The response from the server
+
+        Examples
+        --------
+        To determine the ID of the dataset we wish to delete, we can call client.list_datasets() and filter the results.
+        We are then ready to run::
+
+            >>> client.delete_dataset(dataset_id=DETERMINED_DATASET_ID)
+
+        Specklia will respond with a success message as long as the dataset exists and we are an ADMIN within the
+        group that owns it.
         """
         response = requests.delete(
             self.server_url + "/metadata",
             json={'dataset_id': dataset_id},
             headers={"Authorization": "Bearer " + self.auth_token}
         )
         _check_response_ok(response)
```

### Comparing `specklia-1.1.8/specklia.egg-info/PKG-INFO` & `specklia-1.1.9/specklia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.1.8/tests/test_client.py` & `specklia-1.1.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.8/tests/test_websocket_helpers.py` & `specklia-1.1.9/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

