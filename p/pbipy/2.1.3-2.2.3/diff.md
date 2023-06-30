# Comparing `tmp/pbipy-2.1.3.tar.gz` & `tmp/pbipy-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbipy-2.1.3.tar", last modified: Mon Jun 19 05:49:13 2023, max compression
+gzip compressed data, was "pbipy-2.2.3.tar", last modified: Fri Jun 30 01:38:05 2023, max compression
```

## Comparing `pbipy-2.1.3.tar` & `pbipy-2.2.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 05:49:13.549757 pbipy-2.1.3/
--rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.1.3/LICENSE
--rw-rw-rw-   0        0        0    10195 2023-06-19 05:49:13.548762 pbipy-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     9411 2023-06-19 05:21:11.000000 pbipy-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 05:49:13.536758 pbipy-2.1.3/pbipy/
--rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.1.3/pbipy/__init__.py
--rw-rw-rw-   0        0        0      335 2023-06-19 05:22:36.000000 pbipy-2.1.3/pbipy/__version__.py
--rw-rw-rw-   0        0        0     7848 2023-06-19 04:55:25.000000 pbipy-2.1.3/pbipy/powerbi.py
--rw-rw-rw-   0        0        0    26494 2023-06-19 05:06:21.000000 pbipy-2.1.3/pbipy/resources.py
--rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.1.3/pbipy/settings.py
--rw-rw-rw-   0        0        0    10236 2023-06-19 04:16:26.000000 pbipy-2.1.3/pbipy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:49:13.546756 pbipy-2.1.3/pbipy.egg-info/
--rw-rw-rw-   0        0        0    10195 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 05:49:13.000000 pbipy-2.1.3/pbipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 05:49:13.549757 pbipy-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:38:05.231437 pbipy-2.2.3/
+-rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0    10239 2023-06-30 01:38:05.230438 pbipy-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9455 2023-06-30 01:32:50.000000 pbipy-2.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 01:38:05.215436 pbipy-2.2.3/pbipy/
+-rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.2.3/pbipy/__init__.py
+-rw-rw-rw-   0        0        0      335 2023-06-30 01:35:59.000000 pbipy-2.2.3/pbipy/__version__.py
+-rw-rw-rw-   0        0        0    19984 2023-06-20 20:08:48.000000 pbipy-2.2.3/pbipy/datasets.py
+-rw-rw-rw-   0        0        0     5861 2023-06-20 20:12:45.000000 pbipy-2.2.3/pbipy/groups.py
+-rw-rw-rw-   0        0        0    11659 2023-06-25 19:35:31.000000 pbipy-2.2.3/pbipy/powerbi.py
+-rw-rw-rw-   0        0        0    12743 2023-06-30 01:26:29.000000 pbipy-2.2.3/pbipy/reports.py
+-rw-rw-rw-   0        0        0     1312 2023-06-19 20:24:41.000000 pbipy-2.2.3/pbipy/resources.py
+-rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.2.3/pbipy/settings.py
+-rw-rw-rw-   0        0        0    11125 2023-06-29 21:51:58.000000 pbipy-2.2.3/pbipy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:38:05.227439 pbipy-2.2.3/pbipy.egg-info/
+-rw-rw-rw-   0        0        0    10239 2023-06-30 01:38:05.000000 pbipy-2.2.3/pbipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-06-30 01:38:05.000000 pbipy-2.2.3/pbipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 01:38:05.000000 pbipy-2.2.3/pbipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-30 01:38:05.000000 pbipy-2.2.3/pbipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 01:38:05.000000 pbipy-2.2.3/pbipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 01:38:05.231437 pbipy-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.2.3/setup.py
```

### Comparing `pbipy-2.1.3/LICENSE` & `pbipy-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pbipy-2.1.3/PKG-INFO` & `pbipy-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.1.3
+Version: 2.2.3
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -21,15 +21,17 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-*\* Quick note:* `pbipy` is currently in active development and not all API functionality is supported yet. See [development progress](#development-progress) below for what's been implemented and what's coming.
+`pbipy` supports operations for Reports, Datasets, and Groups (Workspaces), allowing users to perform actions on their PowerBI instance using Python.
+
+See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
 ```
 
@@ -261,16 +263,16 @@
 
 `pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
-| Reports             	| Doing     |       	|
-| Apps                	| Todo     	|       	|
+| Reports             	| Done      |       	|
+| Apps                	| Doing   	|       	|
 | Dataflows           	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.1.3/README.md` & `pbipy-2.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-*\* Quick note:* `pbipy` is currently in active development and not all API functionality is supported yet. See [development progress](#development-progress) below for what's been implemented and what's coming.
+`pbipy` supports operations for Reports, Datasets, and Groups (Workspaces), allowing users to perform actions on their PowerBI instance using Python.
+
+See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
 ```
 
@@ -241,16 +243,16 @@
 
 `pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
-| Reports             	| Doing     |       	|
-| Apps                	| Todo     	|       	|
+| Reports             	| Done      |       	|
+| Apps                	| Doing   	|       	|
 | Dataflows           	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.1.3/pbipy/powerbi.py` & `pbipy-2.2.3/pbipy/powerbi.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 https://learn.microsoft.com/en-us/rest/api/power-bi/
 """
 
 import requests
 from requests.exceptions import HTTPError
 
 from pbipy import settings
-from pbipy.resources import Dataset, Group
+from pbipy.groups import Group
+from pbipy.datasets import Dataset
+from pbipy.reports import Report
 from pbipy.utils import RequestsMixin, remove_no_values
 
 
 class PowerBI(RequestsMixin):
     """
     User Interface into Power BI Rest Api.
 
@@ -33,14 +35,15 @@
 
     https://learn.microsoft.com/en-us/rest/api/power-bi/
 
     Parameters
     ----------
     `bearer_token` : `str`
         Bearer token used to authenticate with your Power BI service.
+
     """
 
     BASE_URL = settings.BASE_URL
 
     def __init__(
         self,
         bearer_token: str,
@@ -70,14 +73,15 @@
         `group` : `str`, optional
             Group Id where the dataset resides., by default None
 
         Returns
         -------
         `Dataset`
             The specified dataset.
+
         """
 
         if isinstance(dataset, Dataset):
             return dataset
 
         dataset = Dataset(dataset, self.session, group_id=group)
         dataset.load()
@@ -97,14 +101,15 @@
             Group Id where the datasets reside. If not supplied, then datasets
             will be retrieved from MyWorkspace.
 
         Returns
         -------
         `list[Dataset]`
             List of datasets for MyWorkspace or the specified group.
+
         """
 
         if group:
             path = f"/groups/{group}/datasets"
         else:
             path = "/datasets"
 
@@ -139,15 +144,17 @@
         `group` : `str`, optional
             Group Id where the dataset resides., by default None
 
         Raises
         ------
         `HTTPError`
             If the api response status code is not equal to 200.
+
         """
+        # FIXME: Doesn't use the group from the Dataset.
 
         if isinstance(dataset, Dataset):
             dataset_id = dataset.id
         else:
             dataset_id = dataset
 
         if group:
@@ -179,14 +186,15 @@
         `Group`
             The specified group.
 
         Raises
         ------
         `ValueError`
             If the Group was not found by the api.
+
         """
 
         id_filter = f"id eq '{group_id}'"
 
         groups = self.groups(filter=id_filter)
 
         if groups == []:
@@ -214,14 +222,20 @@
             Returns only the first n results.
 
         Returns
         -------
         `list[Group]`
             List of `Group` objects the user has access to, and/or
             that matched the specified filters.
+        
+        Notes
+        -----
+        See below for more details on filter syntax:
+        https://learn.microsoft.com/en-us/power-bi/collaborate-share/service-url-filters
+
         """
 
         params = {
             "$filter": filter,
             "$skip": skip,
             "$top": top,
         }
@@ -257,14 +271,15 @@
         `workspace_v2` : `bool`, optional
             (Preview feature) Whether to create a workspace. The only supported value is `true`.
 
         Returns
         -------
         `Group`
             The newly created workspace (group).
+
         """
 
         payload = {"name": name}
 
         if workspace_v2 is not None:
             resource = self.BASE_URL + f"/groups?workspaceV2={workspace_v2}"
         else:
@@ -283,17 +298,145 @@
         """
         Delete the specified workgroup.
 
         Parameters
         ----------
         `group` : `str | Group`
             Group Id or `Group` object to delete.
+
         """
 
         if isinstance(group, Group):
             group_id = group.id
         else:
             group_id = group
 
         resource = self.BASE_URL + f"/groups/{group_id}"
 
         self.delete(resource, self.session)
+
+    def report(
+        self,
+        report: str | Report,
+        group: str | Group = None,
+    ) -> Report:
+        """
+        Return the specified report from MyWorkspace or the specified group.
+
+        Parameters
+        ----------
+        report : `str | Report`
+            Report Id to retrieve.
+        group : `str | Group`, optional
+            Group Id or `Group` object where the report resides.
+
+        Returns
+        -------
+        `Report`
+            The specified `Report` object.
+
+        """
+
+        if isinstance(report, Report):
+            return report
+
+        if isinstance(group, Group):
+            group_id = group.id
+        else:
+            group_id = group
+
+        report = Report(report, self.session, group_id=group_id)
+        report.load()
+
+        return report
+
+    def reports(
+        self,
+        group: str | Group = None,
+    ) -> list[dict]:
+        """
+        Return a list of reports for MyWorkspace or the specified
+        group (workspace).
+
+        Parameters
+        ----------
+        `group` : `str | Group`, optional
+            Group Id or `Group` object where the reports reside., by default None
+
+        Returns
+        -------
+        `list[dict]`
+            List of `Report` objects for MyWorkspace or the specified
+            group (workspace).
+
+        """
+
+        if isinstance(group, Group):
+            group_id = group.id
+        else:
+            group_id = group
+
+        if group_id:
+            path = f"/groups/{group_id}/reports"
+        else:
+            path = "/reports"
+
+        resource = self.BASE_URL + path
+        raw = self.get_raw(resource, self.session)
+
+        reports = [
+            Report(
+                report_js.get("id"),
+                self.session,
+                group_id=group_id,
+                raw=report_js,
+            )
+            for report_js in raw
+        ]
+
+        return reports
+
+    def delete_report(
+        self,
+        report: str | Report,
+        group: str | Group = None,
+    ) -> None:
+        """
+        Delete the specified report. 
+        
+        If a `Report` type is provided as `report`, then it's `group_id` 
+        will be taken as the `group` value.
+
+        Parameters
+        ----------
+        `report` : `str | Report`
+            Report Id or `Report` object to delete.
+        `group` : `str | Group`, optional
+            The Group Id or `Group` object where the report resides. If
+            a `Report` object is provided then the `group_id` of that report
+            will override the provided group value.
+
+            If no group value is provided, it is assumed the report resides
+            in the current user's workspace.
+        
+        """
+
+        if isinstance(report, Report):
+            report_id = report.id
+        else:
+            report_id = report
+        
+        # If we got report, use its group_id and ignore provided
+        if isinstance(report, Report):
+            group_id = report.group_id
+        else:
+            if isinstance(group, Group):
+                group_id = group.id
+            else:
+                group_id = group
+        
+        if group_id:
+            resource = self.BASE_URL + f"/groups/{group_id}/reports/{report_id}"
+        else:
+            resource = self.BASE_URL + f"/reports/{report_id}"
+        
+        self.delete(resource, self.session)
```

### Comparing `pbipy-2.1.3/pbipy/resources.py` & `pbipy-2.2.3/pbipy/datasets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,12 @@
-from requests import Session
-
-from pbipy import settings
-from pbipy.utils import RequestsMixin, remove_no_values, to_snake_case
-
-
-class Resource(RequestsMixin):
-    BASE_URL = settings.BASE_URL
-
-    def __init__(
-        self,
-        id: str,
-        session: Session,
-        **kwargs,
-    ) -> None:
-        self.id = id
-        self.session = session
-        self.raw = None
-
-    def __repr__(
-        self,
-    ) -> str:
-        """
-        Provide a readable representation of the class. Looks to the class'
-        `self._REPR` to determine what to show.
-
-        Returns
-        -------
-        `str`
-            Formatted, readable representation of the class.
-        """
-
-        name = self.__class__.__name__
-
-        attrs = []
-        for attr in self._REPR:
-            if attr in self.__dict__.keys():
-                attr_str = "{}={!r}".format(attr, self.__dict__.get(attr))
-                attrs.append(attr_str)
-
-        return f"<{name} {', '.join(attrs)}>"
-
-    def _load_from_raw(self, raw):
-        self.raw = raw
+from pbipy.resources import Resource
+from pbipy.utils import remove_no_values
 
-        for k, v in raw.items():
-            attr = to_snake_case(k)
-            setattr(self, attr, v)
 
-        return self
-
-    def load(self):
-        raw = self.get_raw(self.base_path, self.session)
-        self._load_from_raw(raw)
+from requests import Session
 
 
 class Dataset(Resource):
     _REPR = [
         "id",
         "name",
         "group_id",
@@ -92,26 +43,27 @@
         self,
         identifier: str,
         principal_type: str,
         access_right: str,
     ) -> None:
         """
         Grants the specified user's permissions to the specified dataset.
-
+        
         Parameters
         ----------
         `identifier` : `str`
             For principal type `User`, provide the UPN. Otherwise provide
             the object ID of the principal.
         `principal_type` : `str`
             The principal type, e.g., "App", "Group", "None", or "User".
         `access_right` : `str`
             The Dataset User Access Right to grant to the user for the
             dataset, e.g.,"Read", "ReadExplore", "ReadReshare", or
             "ReadReshareExplore".
+        
         """
 
         resource = self.base_path + "/users"
         dataset_user_access = {
             "identifier": identifier,
             "principalType": principal_type,
             "datasetUserAccessRight": access_right,
@@ -125,23 +77,24 @@
         datasource_object_ids: list = None,
     ) -> None:
         """
         Binds the specified dataset from MyWorkspace or group to the specified
         gateway, optionally with a given set of data source IDs. If you
         don't supply a specific data source ID, the dataset will be bound
         to the first matching data source in the gateway.
-
+        
         Parameters
         ----------
         `gateway_object_id` : `str`
             The gateway ID. When using a gateway cluster, the gateway ID
             refers to the primary (first) gateway in the cluster and is
             similar to the gateway cluster ID.
         `datasource_object_ids` : `list`, optional
             The unique identifiers for the data sources in the gateway.
+        
         """
 
         bind_to_gateway_request = {
             "gatewayObjectId": gateway_object_id,
             "datasourceObjectIds": datasource_object_ids,
         }
 
@@ -155,103 +108,103 @@
     def cancel_refresh(
         self,
         refresh_id: str,
     ) -> None:
         """
         Cancels the specified refresh operation for the specified dataset
         from MyWorkspace or group.
-
+        
         Parameters
         ----------
         `refresh_id` : `str`
             Refresh Id to cancel.
+        
         """
 
         resource = self.base_path + f"/refreshes/{refresh_id}"
         self.delete(resource, self.session)
 
     def datasources(
         self,
     ) -> list[dict]:
         """
         Returns a list of datasources for the dataset.
-
+        
         Returns
         -------
         `list[dict]`
             List of PowerBI datasources for the dataset.
+        
         """
 
         resource = self.base_path + "/datasources"
         return self.get_raw(resource, self.session)
 
     def discover_gateways(
         self,
     ) -> list:
         """
-        Returns a list of gateways that the specified dataset from My workspace
-        can be bound to.
-
+        Returns a list of gateways that the dataset can be bound to.
+        
         This API call is only relevant to datasets that have at least one
         on-premises connection. For datasets with cloud-only connections,
         this API call returns an empty list.
-
+        
         Returns
         -------
         `list`
             List of PowerBI Gateways that can be bound to.
+        
         """
 
         resource = self.base_path + "/Default.DiscoverGateways"
         return self.get_raw(resource, self.session)
 
     def execute_queries(
         self,
         queries: str | list[str],
         impersonated_user_name: str = None,
         include_nulls: bool = None,
     ) -> dict:
         """
         Executes Data Analysis Expressions (DAX) queries against the provided
         dataset.
-
+        
         DAX query errors will result in:
-
             A response error, such as DAX query failure.
             A failure HTTP status code (400).
-
+        
         A query that requests more than one table, or more than the allowed
         number of table rows, will result in:
-
             Limited data being returned.
             A response error, such as More than one result table in a query
             or More than {allowed number} rows in a query result.
-
             A successful HTTP status code (200).
-
+        
         Columns that are fully qualified in the query will be returned with
         a fully qualified name, for example, MyTable[MyColumn]. Columns
         that are renamed or created in the query will be returned within
         square bracket, for example, `[MyNewColumn]`.
-
+        
         Parameters
         ----------
         `queries` : `str | list[str]`
             Query or list of queries to execute against the dataset.
         `impersonated_user_name` : `str`, optional
             The UPN of a user to be impersonated. If the model is not RLS
             enabled, this will be ignored.
         `include_nulls` : `bool`, optional
             Whether null (blank) values should be included in the result
             set. If unspecified, the default value is `false`.
-
+        
         Returns
         -------
         `dict`
             Dict containing the results of the execution.
+        
         """
 
         if isinstance(queries, str):
             qs = [{"query": queries}]
         else:
             qs = [{"query": query} for query in queries]
 
@@ -275,19 +228,20 @@
         return raw
 
     def parameters(
         self,
     ) -> list[dict]:
         """
         Return a list of parameters for the dataset.
-
+        
         Returns
         -------
         `list[dict]`
             Parameter list.
+        
         """
 
         resource = self.base_path + "/parameters"
         return self.get_raw(resource, self.session)
 
     def refresh(
         self,
@@ -299,15 +253,15 @@
         objects: list[dict] = None,
         retry_count: int = None,
         type: str = None,
     ) -> None:
         """
         Trigger a refresh of the dataset. An enhanced refresh is triggered
         only if a request option other than `notify_option` is set.
-
+        
         Parameters
         ----------
         `notify_option` : `str`
             Mail notification options, e.g., "MailOnCompletion", "MailOnFailure",
             or "NoNotification".
         `apply_refresh_policy` : bool, optional
             Determine if the policy is applied or not.
@@ -318,35 +272,33 @@
             If an incremental refresh policy is applied, the `effective_date`
             parameter overrides the current date.
         `max_parallelism` : `int`, optional
             The maximum number of threads on which to run parallel processing
             commands.
         `objects` : `list[dict]`, optional
             A list of objects to be processed, e.g.,
-
             ```
             [
                 {
                 "table": "Customer",
                 "partition": "Robert"
                 }
             ]
             ```
-
         `retry_count` : `int`, optional
             Number of times the operation will retry before failing.
         `type` : `str`, optional
            The type of processing to perform, e.g., "Automatic", "Calculate",
            "ClearValues", "DataOnly", "Defragment", or "Full".
-
+        
         Notes
         -----
         See here for request options in greater detail:
-
         https://learn.microsoft.com/en-us/rest/api/power-bi/datasets/refresh-dataset#definitions
+        
         """
 
         refresh_request = {
             "applyRefreshPolicy": apply_refresh_policy,
             "commitMode": commit_mode,
             "effectiveDate": effective_date,
             "maxParallelism": max_parallelism,
@@ -364,51 +316,53 @@
     def refresh_details(
         self,
         refresh_id: str,
     ) -> dict:
         """
         Returns execution details of an enhanced refresh operation for
         the dataset.
-
+        
         Parameters
         ----------
         `refresh_id` : `str`
             Refresh Id to get the execution details for.
-
+        
         Returns
         -------
         `dict`
             Refresh execution details.
+        
         """
 
         resource = self.base_path + f"/refreshes/{refresh_id}"
         return self.get_raw(resource, self.session)
 
     def refresh_history(
         self,
         top: int = None,
     ) -> list[dict]:
         """
         Returns the refresh history for the dataset.
-
+        
         Parameters
         ----------
         `top` : `int`, optional
             The requested number of entries in the refresh history. If
             not provided, the default is the last available 500 entries.
-
+        
         Returns
         -------
         `list[dict]`
             List of refresh history entries.
-
+        
         Raises
         ------
         `HTTPError`
             If the api response status code is not equal to 200.
+        
         """
         # TODO: implement Refresh object
 
         resource = self.base_path + "/refreshes"
         params = {"$top": top}
 
         raw = self.get_raw(resource, self.session, params)
@@ -418,24 +372,25 @@
     def refresh_schedule(
         self,
         direct_query: bool = False,
     ) -> dict:
         """
         Return the Refresh Schedule or Direct Query Refresh Schedule for
         the dataset.
-
+        
         Parameters
         ----------
         `direct_query` : `bool`, optional
             Return the Direct Query Refresh Schedule instead of the Refresh Schedule.
-
+        
         Returns
         -------
         `dict`
             Refresh schedule or Direct Query Refresh Schedule.
+        
         """
 
         if direct_query:
             resource = self.base_path + "/directQueryRefreshSchedule"
         else:
             resource = self.base_path + "/refreshSchedule"
 
@@ -444,21 +399,22 @@
         return raw
 
     def take_over(
         self,
     ) -> None:
         """
         Transfer ownership of the dataset to the current authorized user.
-
+        
         Raises
         ------
         `TypeError`
             If the dataset does not have a group_id. In other words, can't
             take over dataset in MyWorkspace, the authorized user already
             owns these.
+        
         """
 
         if not self.group_id:
             raise TypeError(
                 "Dataset does not have a group_id. Taking over a dataset can only be performed on a Dataset in a Group."
             )
 
@@ -467,41 +423,42 @@
 
     def update(
         self,
         target_storage_mode: str,
     ) -> None:
         """
         Update the properties of the dataset.
-
+        
         Parameters
         ----------
         `target_storage_mode` : `str`
             The dataset storage mode, .e.g, "PremiumFiles", or "Abf".
+        
         """
         update_dataset_request = {"targetStorageMode": target_storage_mode}
 
         self.patch(self.base_path, self.session, update_dataset_request)
 
     def update_datasources(
         self,
         update_details: dict | list[dict],
     ) -> None:
         """
         Update the data sources of the dataset.
-
+        
         Parameters
         ----------
         `update_details` : `dict | list[dict]`
             A dict, or list of dicts, representing the updates.
-
+        
         Notes
         -----
         See here for how to construct the update details:
-
         https://learn.microsoft.com/en-us/rest/api/power-bi/datasets/update-datasources#examples
+        
         """
 
         if isinstance(update_details, dict):
             update_details_prepared = [update_details]
         else:
             update_details_prepared = update_details
 
@@ -512,33 +469,32 @@
 
     def update_parameters(
         self,
         update_details: dict | list[dict],
     ) -> None:
         """
         Updates the parameters values for the dataset.
-
+        
         Parameters
         ----------
         update_details : `dict | list[dict]`
             Dict, or list of dicts, of the parameters to update.
-
             Parameter updates take the form:
-
             ```
             {
                 "name": "parameter_name",
                 "newValue": "new_value"
             }
             ```
+        
         Notes
         -----
         See more here:
-
         https://learn.microsoft.com/en-us/rest/api/power-bi/datasets/update-parameters#example
+        
         """
 
         if isinstance(update_details, dict):
             update_details_prepared = [update_details]
         else:
             update_details_prepared = update_details
 
@@ -558,18 +514,18 @@
         frequency: int = None,
         local_time_zone_id: str = None,
         times: list[str] = None,
     ) -> None:
         """
         Update the Refresh Schedule or Direct Query Refresh Schedule of the
         dataset.
-
+        
         Providing `direct_query=True` targets the Direct Query
         Refresh Schedule.
-
+        
         Parameters
         ----------
         `notify_option` : `str`
             Mail notification options, e.g., "MailOnCompletion", "MailOnFailure",
             or "NoNotification".
         `direct_query` : bool, optional
             Target the Direct Query Refresh Schedule (if there is one) of the
@@ -579,27 +535,27 @@
             "Tuesday", "Wednesday", etc.
         `enabled` : bool, optional
             Whether the refresh is enabled.
         `frequency` : int, optional
             Applies to Direct Query Refresh Schedule only. The interval in minutes
             between successive refreshes. Supported values are 15, 30, 60, 120,
             and 180.
-
             If `frequency` is supplied and `direct_query` is `false`, then `frequency`
             will be ignored.
         `local_time_zone_id` : `str`, optional
             _The ID of the time zone to use, e.g, "UTC".
         `times` : list[str], optional
             The times of day to execute the refresh expressed as hh:mm, e.g.,
             "07:00", "16:00", etc.
-
+        
         Raises
         ------
         `ValueError`
             If no values are provided for the request.
+        
         """
 
         # Prepare the request details
         refresh_schedule_request = {
             "value": {
                 "notifyOption": notify_option,
                 "days": days,
@@ -634,25 +590,26 @@
         identifier: str,
         principal_type: str,
         access_right: str,
     ) -> None:
         """
         Updates the existing permissions for a user of the dataset to the
         specified permissions.
-
+        
         Parameters
         ----------
         `identifier` : `str`
             For principal type User, provide the UPN. Otherwise provide
             the object ID of the principal.
         `principal_type` : `str`
             The principal type, e.g., "App", "Group", "None", or "User".
         `access_right` : `str`
             The Dataset User Access Right to grant to the user, e.g.,"Read",
             "ReadExplore", "ReadReshare", or "ReadReshareExplore".
+        
         """
 
         resource = self.base_path + "/users"
         dataset_user_access = {
             "identifier": identifier,
             "principalType": principal_type,
             "datasetUserAccessRight": access_right,
@@ -661,203 +618,18 @@
         self.put(resource, self.session, dataset_user_access)
 
     def users(
         self,
     ) -> list[dict]:
         """
         Returns a list of principals that have access to the dataset.
-
+        
         Returns
         -------
         `list[dict]`
             List of principals, e.g., Users, Groups, with access to the
             dataset.
+        
         """
 
         resource = self.base_path + "/users"
-        return self.get_raw(resource, self.session)
-
-
-class Group(Resource):
-    _REPR = [
-        "id",
-        "name",
-    ]
-
-    def __init__(
-        self,
-        id: str,
-        session: Session,
-        raw=None,
-        **kwargs,
-    ) -> None:
-        super().__init__(id, session, **kwargs)
-
-        self.base_path = f"{self.BASE_URL}/groups/{self.id}"
-
-        if raw:
-            self._load_from_raw(raw)
-
-    def add_user(
-        self,
-        identifier: str,
-        principal_type: str,
-        access_right: str,
-        display_name: str = None,
-        email_address: str = None,
-        graph_id: str = None,
-        profile: dict = None,
-        user_type: str = None,
-    ) -> None:
-        """
-        Grants the specified user the specified permissions to the workspace.
-
-        Parameters
-        ----------
-        `identifier` : `str`
-            Identifier of the principal.
-        `principal_type` : `str`
-            The principal type, e.g., "App", "Group", "None", or "User".
-        `access_right` : `str`
-            The access right (permission level) that a user has on the
-            workspace, e.g., "Admin", "Contributor", "Member", "None",
-            or "Viewer".
-        `display_name` : `str`, optional
-            Display name of the principal.
-        `email_address` : `str`, optional
-            Email address of the user.
-        `graph_id` : `str`, optional
-            Identifier of the principal in Microsoft Graph. Only available
-            for admin APIs.
-        `profile` : `dict`, optional
-            A Power BI service principal profile. Only relevant for Power
-            BI Embedded multi-tenancy solution.
-        `user_type` : `str`, optional
-            Type of the user.
-        """
-
-        payload = {
-            "identifier": identifier,
-            "groupUserAccessRight": access_right,
-            "principalType": principal_type,
-            "displayName": display_name,
-            "emailAddress": email_address,
-            "graphId": graph_id,
-            "profile": profile,
-            "userType": user_type,
-        }
-
-        prepared_payload = remove_no_values(payload)
-        resource = self.base_path + "/users"
-
-        self.post(resource, self.session, prepared_payload)
-
-    def delete_user(
-        self,
-        user: str,
-        profile: str = None,
-    ) -> None:
-        """
-        Deletes the specified user permissions from the specified workspace.
-
-        Parameters
-        ----------
-        `user` : `str`
-            The email address of the user or object ID of the service principal
-            to delete.
-        `profile` : `str`, optional
-            The service principal profile ID to delete.
-        """
-
-        if profile:
-            resource = self.base_path + f"/users/{user}?profileId={profile}"
-        else:
-            resource = self.base_path + f"/users/{user}"
-
-        self.delete(resource, self.session)
-
-    def update_user(
-        self,
-        identifier: str,
-        principal_type: str,
-        access_right: str,
-        display_name: str = None,
-        email_address: str = None,
-        graph_id: str = None,
-        profile: dict = None,
-        user_type: str = None,
-    ) -> None:
-        """
-        Updates the specified user permissions on the workspace.
-
-        Parameters
-        ----------
-        `identifier` : `str`
-            Identifier of the principal.
-        `principal_type` : `str`
-            The principal type, e.g., "App", "Group", "None", or "User".
-        `access_right` : `str`
-            The access right (permission level) that a user has on the
-            workspace, e.g., "Admin", "Contributor", "Member", "None",
-            or "Viewer".
-        `display_name` : `str`, optional
-            Display name of the principal.
-        `email_address` : `str`, optional
-            Email address of the user.
-        `graph_id` : `str`, optional
-            Identifier of the principal in Microsoft Graph. Only available
-            for admin APIs.
-        `profile` : `dict`, optional
-            A Power BI service principal profile. Only relevant for Power
-            BI Embedded multi-tenancy solution.
-        `user_type` : `str`, optional
-            Type of the user.
-        """
-
-        payload = {
-            "identifier": identifier,
-            "groupUserAccessRight": access_right,
-            "principalType": principal_type,
-            "displayName": display_name,
-            "emailAddress": email_address,
-            "graphId": graph_id,
-            "profile": profile,
-            "userType": user_type,
-        }
-
-        prepared_payload = remove_no_values(payload)
-        resource = self.base_path + "/users"
-
-        self.put(resource, self.session, prepared_payload)
-
-    def users(
-        self,
-        skip: int = None,
-        top: int = None,
-    ) -> list[dict]:
-        """
-        Returns a list of users that have access to the workspace.
-
-        Parameters
-        ----------
-        `skip` : `int`, optional
-            Skips the first n results.
-        `top` : `int`, optional
-            Returns onl the first n results.
-
-        Returns
-        -------
-        `list[dict]`
-            List of users that have access to the workspace.
-        """
-
-        params = {
-            "$skip": skip,
-            "$top": top,
-        }
-
-        prepared_params = remove_no_values(params)
-        resource = self.base_path + "/users"
-
-        raw = self.get_raw(resource, self.session, params=prepared_params)
-
-        return raw
+        return self.get_raw(resource, self.session)
```

### Comparing `pbipy-2.1.3/pbipy/utils.py` & `pbipy-2.2.3/pbipy/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Utility functions and classes used internally by pybi."""
 
 import json
+from pathlib import Path
 import re
 
 from requests import Response, Session
 from requests.exceptions import HTTPError
 
 
 def to_snake_case(s):
@@ -48,14 +49,54 @@
             v = remove_no_values(v)
         if not v in (None, {}):
             new_d[k] = v
 
     return new_d
 
 
+def file_path_from_components(
+    file_name: str,
+    extension: str,
+    directory: str | Path = None,
+):
+    """
+    Create a file path from file path components.
+
+    Parameters
+    ----------
+    `file_name` : `str`
+        Name of the file (without extension).
+    `extension` : `str`
+        The file extension.
+    `directory` : `str | Path`, optional
+        Directory of the file.
+
+    Returns
+    -------
+    `Path`
+        File path to the file.
+
+    """
+
+    if isinstance(directory, str):
+        f_dir = Path(directory)
+    elif directory is None:
+        f_dir = Path()  # cwd
+    else:
+        f_dir = directory
+    
+    # Be a bit more flexible and accept .ext
+    if extension[0] == ".":
+        f_ext = extension[1:]
+    else:
+        f_ext = extension
+
+    return f_dir / f"{file_name}.{f_ext}"
+
+
 class RequestsMixin:
     """
     Mixin class for http requests and response handling.
 
     Lets the PowerBI client and Resources use the same functionality for
     making requests and handling the response.
 
@@ -139,15 +180,15 @@
         return response
 
     def post(
         self,
         resource: str,
         session: Session,
         payload: dict = None,
-        success_codes: list[int] = [200, 201],
+        success_codes: list[int] = [200, 201, 202],
     ) -> Response:
         """
         Post data to an api endpoint.
 
         Parameters
         ----------
         `resource` : `str`
```

### Comparing `pbipy-2.1.3/pbipy.egg-info/PKG-INFO` & `pbipy-2.2.3/pbipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.1.3
+Version: 2.2.3
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -21,15 +21,17 @@
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
-*\* Quick note:* `pbipy` is currently in active development and not all API functionality is supported yet. See [development progress](#development-progress) below for what's been implemented and what's coming.
+`pbipy` supports operations for Reports, Datasets, and Groups (Workspaces), allowing users to perform actions on their PowerBI instance using Python.
+
+See [development progress](#development-progress) below for what's been implemented and what's coming.
 
 ## Installation
 
 ```console
 pip install pbipy
 ```
 
@@ -261,16 +263,16 @@
 
 `pbipy` is in the early stages of development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
 
 | PowerBI Component   	| Progress 	| Notes 	|
 |---------------------	|----------	|-------	|
 | Datasets            	| Done     	|       	|
 | Groups (Workspaces) 	| Done    	|       	|
-| Reports             	| Doing     |       	|
-| Apps                	| Todo     	|       	|
+| Reports             	| Done      |       	|
+| Apps                	| Doing   	|       	|
 | Dataflows           	| Todo     	|       	|
 | Dashboards          	| Todo     	|       	|
 | Everything else     	| Backlog  	|       	|
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
```

### Comparing `pbipy-2.1.3/setup.py` & `pbipy-2.2.3/setup.py`

 * *Files identical despite different names*

