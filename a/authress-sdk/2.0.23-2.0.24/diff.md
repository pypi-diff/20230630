# Comparing `tmp/authress-sdk-2.0.23.tar.gz` & `tmp/authress-sdk-2.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/authress-sdk.py/authress-sdk.py/dist/.tmp-sxtohfwx/authress-sdk-2.0.23.tar", last modified: Fri Jun 30 07:18:46 2023, max compression
+gzip compressed data, was "/home/runner/work/authress-sdk.py/authress-sdk.py/dist/.tmp-gmv272m9/authress-sdk-2.0.24.tar", last modified: Fri Jun 30 07:27:24 2023, max compression
```

## Comparing `authress-sdk-2.0.23.tar` & `authress-sdk-2.0.24.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:18:46.496527 authress-sdk-2.0.23/
--rw-r--r--   0 runner    (1001) docker     (122)     6844 2023-06-30 07:18:46.496527 authress-sdk-2.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6212 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:18:46.480526 authress-sdk-2.0.23/authress_sdk/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-30 07:18:28.000000 authress-sdk-2.0.23/authress_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:18:46.484526 authress-sdk-2.0.23/authress_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22074 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/api/access_records_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    13228 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/api/accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    11402 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/api/resource_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/api/service_client_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    25091 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/api/service_clients_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3127 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/api/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (122)    14971 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/api/user_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/authress_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    22061 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:18:46.496527 authress-sdk-2.0.23/authress_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/access_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/access_record_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/access_record_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/access_record_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/access_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (122)     3504 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/access_record_statement.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/access_record_user.py
--rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/account_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/claim_request.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/claim_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3966 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/client_access_key.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/client_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/client_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/identity_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/permission_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/resource_permission.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/resource_permission_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/resource_permission_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1868 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/user_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/models/user_resources.py
--rw-r--r--   0 runner    (1001) docker     (122)    11644 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/authress_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:18:46.484526 authress-sdk-2.0.23/authress_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6844 2023-06-30 07:18:46.000000 authress-sdk-2.0.23/authress_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-30 07:18:46.000000 authress-sdk-2.0.23/authress_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 07:18:46.000000 authress-sdk-2.0.23/authress_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-30 07:18:46.000000 authress-sdk-2.0.23/authress_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-30 07:18:46.000000 authress-sdk-2.0.23/authress_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 07:18:46.496527 authress-sdk-2.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:18:46.496527 authress-sdk-2.0.23/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3917 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/test/test_service_client_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-30 07:18:20.000000 authress-sdk-2.0.23/test/test_token_verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:27:24.946988 authress-sdk-2.0.24/
+-rw-r--r--   0 runner    (1001) docker     (122)     6844 2023-06-30 07:27:24.946988 authress-sdk-2.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6212 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:27:24.938988 authress-sdk-2.0.24/authress_sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-30 07:27:07.000000 authress-sdk-2.0.24/authress_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:27:24.942988 authress-sdk-2.0.24/authress_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22320 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/api/access_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13228 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/api/accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11402 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/api/resource_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/api/service_client_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25091 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/api/service_clients_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3127 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/api/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14971 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/api/user_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/authress_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22061 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:27:24.946988 authress-sdk-2.0.24/authress_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/access_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/access_record_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/access_record_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/access_record_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/access_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3504 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/access_record_statement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/access_record_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/account_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/claim_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/claim_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3966 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/client_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/client_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/client_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/identity_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/permission_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/resource_permission.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/resource_permission_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/resource_permission_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1868 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/user_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/models/user_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11644 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/authress_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:27:24.942988 authress-sdk-2.0.24/authress_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6844 2023-06-30 07:27:24.000000 authress-sdk-2.0.24/authress_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-30 07:27:24.000000 authress-sdk-2.0.24/authress_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 07:27:24.000000 authress-sdk-2.0.24/authress_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-30 07:27:24.000000 authress-sdk-2.0.24/authress_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-30 07:27:24.000000 authress-sdk-2.0.24/authress_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 07:27:24.946988 authress-sdk-2.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 07:27:24.946988 authress-sdk-2.0.24/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3917 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/test/test_service_client_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-30 07:26:59.000000 authress-sdk-2.0.24/test/test_token_verifier.py
```

### Comparing `authress-sdk-2.0.23/PKG-INFO` & `authress-sdk-2.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authress-sdk
-Version: 2.0.23
+Version: 2.0.24
 Summary: Authress SDK for authorization as a service and interact with the Authress API.
 Home-page: https://github.com/Authress/authress-sdk.py.git
 Author: Rhosys Developers
 Author-email: developers@authress.io
 License: Apache-2.0
 Keywords: Authorization as a service,Security,authorization,authorization as a service,authentication,user authentication,Authress,Authress client,access management,access management as a service,user security,oso,polar,open source policy engine,embedded authorization,batteries included authorization
 Description-Content-Type: text/markdown
```

### Comparing `authress-sdk-2.0.23/README.md` & `authress-sdk-2.0.24/README.md`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/__init__.py` & `authress-sdk-2.0.24/authress_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/api/access_records_api.py` & `authress-sdk-2.0.24/authress_sdk/api/access_records_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from __future__ import absolute_import
 
 import re
 
 # python 2 and python 3 compatibility library
 import six
 
+from authress_sdk.models.access_record_collection import AccessRecordCollection
+from authress_sdk.models.access_record import AccessRecord
+
 
 class AccessRecordsApi(object):
     def __init__(self, api_client):
       self.api_client = api_client
 
     def create_claim(self, body, **kwargs):
         """Claim a resource by an allowed user
@@ -106,15 +109,15 @@
             response_type='ClaimResponse',
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_records(self, limit=20, cursor=None, filter=None, **kwargs):
+    def get_records(self, limit: int = 20, cursor: str = None, filter: str = None, **kwargs) -> AccessRecordCollection:
         """Get all account records.
 
         <i class=\"far fa-money-bill-alt text-primary\"></i> <span class=\"text-primary\">Billable</span> Returns a paginated records list for the account. Only records the user has access to are returned.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_records(async_req=True)
         >>> result = thread.get()
@@ -201,15 +204,15 @@
             response_type='AccessRecordCollection',
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_record(self, body, **kwargs):
+    def create_record(self, body: AccessRecord, **kwargs):
         """Create a new access record
 
         Specify user roles for specific resources.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_record(body, async_req=True)
         >>> result = thread.get()
@@ -298,15 +301,15 @@
             response_type='AccessRecord',
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete_record(self, record_id, **kwargs):
+    def delete_record(self, record_id: str, **kwargs):
         """Deletes an access record.
 
         Remove an access record, removing associated permissions from all users in record. If a user has a permission from another record, that permission will not be removed.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_record(record_id, async_req=True)
         >>> result = thread.get()
@@ -387,15 +390,15 @@
             response_type=None,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_record(self, record_id, **kwargs):
+    def get_record(self, record_id: str, **kwargs) -> AccessRecord:
         """Get an access record for the account.
 
         Access records contain information assigning permissions to users for resources.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_record(record_id, async_req=True)
         >>> result = thread.get()
@@ -480,15 +483,15 @@
             response_type='AccessRecord',
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_record(self, body, record_id, **kwargs):
+    def update_record(self, body: AccessRecord, record_id: str, **kwargs):
         """Update an access record.
 
         Updates an access record adding or removing user permissions to resources.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_record(body, record_id, async_req=True)
         >>> result = thread.get()
```

### Comparing `authress-sdk-2.0.23/authress_sdk/api/accounts_api.py` & `authress-sdk-2.0.24/authress_sdk/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/api/resource_permissions_api.py` & `authress-sdk-2.0.24/authress_sdk/api/resource_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/api/service_client_token_provider.py` & `authress-sdk-2.0.24/authress_sdk/api/service_client_token_provider.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/api/service_clients_api.py` & `authress-sdk-2.0.24/authress_sdk/api/service_clients_api.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/api/token_verifier.py` & `authress-sdk-2.0.24/authress_sdk/api/token_verifier.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/api/user_permissions_api.py` & `authress-sdk-2.0.24/authress_sdk/api/user_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/authress_client.py` & `authress-sdk-2.0.24/authress_sdk/authress_client.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/http_client.py` & `authress-sdk-2.0.24/authress_sdk/http_client.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/__init__.py` & `authress-sdk-2.0.24/authress_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/access_record.py` & `authress-sdk-2.0.24/authress_sdk/models/access_record.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/access_record_account.py` & `authress-sdk-2.0.24/authress_sdk/models/access_record_account.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/access_record_collection.py` & `authress-sdk-2.0.24/authress_sdk/models/access_record_collection.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/access_record_group.py` & `authress-sdk-2.0.24/authress_sdk/models/access_record_group.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/access_record_resource.py` & `authress-sdk-2.0.24/authress_sdk/models/access_record_resource.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/access_record_statement.py` & `authress-sdk-2.0.24/authress_sdk/models/access_record_statement.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/access_record_user.py` & `authress-sdk-2.0.24/authress_sdk/models/access_record_user.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/account.py` & `authress-sdk-2.0.24/authress_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/account_collection.py` & `authress-sdk-2.0.24/authress_sdk/models/account_collection.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/claim_request.py` & `authress-sdk-2.0.24/authress_sdk/models/claim_request.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/client.py` & `authress-sdk-2.0.24/authress_sdk/models/client.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/client_access_key.py` & `authress-sdk-2.0.24/authress_sdk/models/client_access_key.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/client_collection.py` & `authress-sdk-2.0.24/authress_sdk/models/client_collection.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/client_options.py` & `authress-sdk-2.0.24/authress_sdk/models/client_options.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/identity.py` & `authress-sdk-2.0.24/authress_sdk/models/identity.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/identity_collection.py` & `authress-sdk-2.0.24/authress_sdk/models/identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/identity_request.py` & `authress-sdk-2.0.24/authress_sdk/models/identity_request.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/permission_object.py` & `authress-sdk-2.0.24/authress_sdk/models/permission_object.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/resource_permission.py` & `authress-sdk-2.0.24/authress_sdk/models/resource_permission.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/resource_permission_collection.py` & `authress-sdk-2.0.24/authress_sdk/models/resource_permission_collection.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/resource_permission_object.py` & `authress-sdk-2.0.24/authress_sdk/models/resource_permission_object.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/user_permissions.py` & `authress-sdk-2.0.24/authress_sdk/models/user_permissions.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/models/user_resources.py` & `authress-sdk-2.0.24/authress_sdk/models/user_resources.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk/rest.py` & `authress-sdk-2.0.24/authress_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/authress_sdk.egg-info/PKG-INFO` & `authress-sdk-2.0.24/authress_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authress-sdk
-Version: 2.0.23
+Version: 2.0.24
 Summary: Authress SDK for authorization as a service and interact with the Authress API.
 Home-page: https://github.com/Authress/authress-sdk.py.git
 Author: Rhosys Developers
 Author-email: developers@authress.io
 License: Apache-2.0
 Keywords: Authorization as a service,Security,authorization,authorization as a service,authentication,user authentication,Authress,Authress client,access management,access management as a service,user security,oso,polar,open source policy engine,embedded authorization,batteries included authorization
 Description-Content-Type: text/markdown
```

### Comparing `authress-sdk-2.0.23/authress_sdk.egg-info/SOURCES.txt` & `authress-sdk-2.0.24/authress_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/setup.py` & `authress-sdk-2.0.24/setup.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/test/test_service_client_token_provider.py` & `authress-sdk-2.0.24/test/test_service_client_token_provider.py`

 * *Files identical despite different names*

### Comparing `authress-sdk-2.0.23/test/test_token_verifier.py` & `authress-sdk-2.0.24/test/test_token_verifier.py`

 * *Files identical despite different names*

