# Comparing `tmp/restsuite-0.1.7.1.tar.gz` & `tmp/restsuite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restsuite-0.1.7.1.tar", last modified: Mon Apr 17 21:14:03 2023, max compression
+gzip compressed data, was "restsuite-1.0.0.tar", last modified: Fri Jun 30 01:33:37 2023, max compression
```

## Comparing `restsuite-0.1.7.1.tar` & `restsuite-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-04-17 21:14:03.067467 restsuite-0.1.7.1/
--rw-r--r--   0 peterwilliams   (501) staff       (20)     1070 2023-01-10 22:48:18.000000 restsuite-0.1.7.1/LICENSE
--rw-r--r--   0 peterwilliams   (501) staff       (20)     9437 2023-04-17 21:14:03.067279 restsuite-0.1.7.1/PKG-INFO
--rw-r--r--   0 peterwilliams   (501) staff       (20)     7583 2023-01-18 21:17:16.000000 restsuite-0.1.7.1/README.md
--rw-r--r--   0 peterwilliams   (501) staff       (20)      803 2023-04-17 21:13:56.000000 restsuite-0.1.7.1/pyproject.toml
-drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-04-17 21:14:03.066306 restsuite-0.1.7.1/restsuite/
--rw-r--r--   0 peterwilliams   (501) staff       (20)       86 2023-01-10 17:43:57.000000 restsuite-0.1.7.1/restsuite/__init__.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)    13271 2023-02-02 14:13:32.000000 restsuite-0.1.7.1/restsuite/auth.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)     7978 2023-01-18 21:38:29.000000 restsuite-0.1.7.1/restsuite/base_rest.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)     2527 2023-01-10 21:32:14.000000 restsuite-0.1.7.1/restsuite/rest.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)     6626 2023-01-13 20:33:33.000000 restsuite-0.1.7.1/restsuite/restlet.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)     4455 2023-04-17 21:12:25.000000 restsuite-0.1.7.1/restsuite/suiteql.py
-drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-04-17 21:14:03.067104 restsuite-0.1.7.1/restsuite.egg-info/
--rw-r--r--   0 peterwilliams   (501) staff       (20)     9437 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/PKG-INFO
--rw-r--r--   0 peterwilliams   (501) staff       (20)      319 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/SOURCES.txt
--rw-r--r--   0 peterwilliams   (501) staff       (20)        1 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/dependency_links.txt
--rw-r--r--   0 peterwilliams   (501) staff       (20)        9 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/requires.txt
--rw-r--r--   0 peterwilliams   (501) staff       (20)       10 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/top_level.txt
--rw-r--r--   0 peterwilliams   (501) staff       (20)       38 2023-04-17 21:14:03.067516 restsuite-0.1.7.1/setup.cfg
+drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-06-30 01:33:37.994824 restsuite-1.0.0/
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     1070 2023-01-10 22:48:18.000000 restsuite-1.0.0/LICENSE
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     9469 2023-06-30 01:33:37.994511 restsuite-1.0.0/PKG-INFO
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     7617 2023-06-30 01:19:20.000000 restsuite-1.0.0/README.md
+-rw-r--r--   0 peterwilliams   (501) staff       (20)      826 2023-06-30 01:20:32.000000 restsuite-1.0.0/pyproject.toml
+drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-06-30 01:33:37.993411 restsuite-1.0.0/restsuite/
+-rw-r--r--   0 peterwilliams   (501) staff       (20)       66 2023-06-30 01:23:01.000000 restsuite-1.0.0/restsuite/__init__.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     2702 2023-06-30 01:21:10.000000 restsuite-1.0.0/restsuite/base_rest.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)      382 2023-06-30 01:21:10.000000 restsuite-1.0.0/restsuite/rest.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     6626 2023-01-13 20:33:33.000000 restsuite-1.0.0/restsuite/restlet.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     4733 2023-06-30 01:21:10.000000 restsuite-1.0.0/restsuite/suiteql.py
+drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-06-30 01:33:37.994328 restsuite-1.0.0/restsuite.egg-info/
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     9469 2023-06-30 01:33:37.000000 restsuite-1.0.0/restsuite.egg-info/PKG-INFO
+-rw-r--r--   0 peterwilliams   (501) staff       (20)      301 2023-06-30 01:33:37.000000 restsuite-1.0.0/restsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 peterwilliams   (501) staff       (20)        1 2023-06-30 01:33:37.000000 restsuite-1.0.0/restsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 peterwilliams   (501) staff       (20)       27 2023-06-30 01:33:37.000000 restsuite-1.0.0/restsuite.egg-info/requires.txt
+-rw-r--r--   0 peterwilliams   (501) staff       (20)       10 2023-06-30 01:33:37.000000 restsuite-1.0.0/restsuite.egg-info/top_level.txt
+-rw-r--r--   0 peterwilliams   (501) staff       (20)       38 2023-06-30 01:33:37.994878 restsuite-1.0.0/setup.cfg
```

### Comparing `restsuite-0.1.7.1/LICENSE` & `restsuite-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `restsuite-0.1.7.1/PKG-INFO` & `restsuite-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restsuite
-Version: 0.1.7.1
+Version: 1.0.0
 Summary: Easily work with Netsuite's REST API
 Author: Peter Williams, Richard Demke, Andy Gannaway
 Author-email: Peter Williams <petercw94@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Williams
         
@@ -37,40 +37,37 @@
 License-File: LICENSE
 
 # restsuite
 
 restsuite is a python package developed to help developers interact with the Netsuite REST API. restsuite offers a number of classes that can be utilized to interact with Netsuite's Suite-Talk, RESTlet, or SuiteQL services. restsuite currently utilizes Netsuite's token authentication methods, however, current development is under way for supporting Netsuite's Oauth2 authentication methods. 
 
 
-### Disclaimer:  
-
-*restsuite is still in developement stages and is currently being tested through usage in our company. Although open to the public for use, understand that this is not a stable version of the restsuite package. Integrating restsuite into production applications at this stage is not advised.*
 
 ## Installation
 
 restsuite is part of the Python Package Index (PyPI) and can thus be installed with pip:
 
 ```
 pip install restsuite
 ```
 
-restsuite requires a python version of 3.8 or higher and depends only on the [requests python package](https://requests.readthedocs.io/en/latest/) 
+restsuite requires a python version of 3.8 or higher and depends on the [requests python package](https://requests.readthedocs.io/en/latest/) and the [requests_oauthlib python package](https://pypi.org/project/requests-oauthlib/)
 
 
 ## Getting Started
 
 As restsuite is an abstraction of the Netsuite API, it will be helpful to become familiar with, or at least reference, the Netsuite API documentation:
 
 - [Suite-Talk Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1540391670.html)
 - [RESTlet Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2970701.html)
 - [SuiteQL Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156257770590.html)
 
 ### Authentication
 
-Each of the provided classes (NetSuiteRest, NetSuiteRESTlet, NetSuiteQL) handle authentication for the developer. All that is required is basic account information that can be generated in the user's account integration settings (see [REST Web Services Prerequisites and Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544787084.html) for a guide on setting up your Netsuite application to utilize REST capabilities)
+Each of the provided classes (NetSuiteRest, NetSuiteRESTlet, NetSuiteQL) utilize the [requests_oauthlib](https://pypi.org/project/requests-oauthlib/) package to handle authentication for the developer. All that is required is basic account information that can be generated in the user's account integration settings (see [REST Web Services Prerequisites and Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544787084.html) for a guide on setting up your Netsuite application to utilize REST capabilities)
 
 Each class requires that you pass the following attributes upon object instantiation:
 - Netsuite Account ID : This can be found the Netsuite url path (e.g: *https://{{ account_id }}.app.netsuite.com)*)
 - Consumer Key : Consumer Key and Secret are provided upon integration record creation [Integration Record Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4389727047.html).
 - Consumer Secret : Consumer Secret is provided upon integation record creation [Integration Record Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4389727047.html)
 - Token Key : Tokens can be generated a number of ways. We are currently developing a Class for generating tokens with the [issuetoken endpoint](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157017286140.html). For the time being, you can [generate a token with the Netsuite UI](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4254081947.html).
 - Token Secret : See Token Key
@@ -97,58 +94,58 @@
 )
 ```
 
 #### Getting a Record (GET):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job".format(NS_ACCOUNT_ID)
 
-response = netsuite.get(url)
+response = netsuite.request("GET", url)
 
-if response.status_code <= 300:
+if response.status_code < 300:
     data = response.json()
 ```
-*[Getting docs]()*
+*[Getting docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545141500.html#Getting-a-Record-Instance)*
 
 *It is important to note here that all classes will require the full URL to be passed to each request method.*
 
 #### Creating a Record object (POST):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"entityid": "New Customer", "companyname": "My Company", "subsidiary": {"id": "1"}}
 
-response = netsuite.post(url=url, body=body)
+response = netsuite.request("POST", url=url, body=body)
 ```
 *[Creating docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545141395.html)*
 
 #### Updating a Record object (PATCH):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"entityid": "Updated Customer"}
 
-response = netsuite.patch(url=url, body=body)
+response = netsuite.request("PATCH", url=url, body=body)
 ```
 *[Updating docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545142173.html)*
 
 #### Upserting a Record object (PUT):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"firstName": "John", "lastName": "Smith"}
 
-response = netsuite.put(url=url, body=body)
+response = netsuite.request("PUT", url=url, body=body)
 ```
 *[Upsert docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156335203191.html)*
 
 #### Deleting a Record object (DELETE)
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
-response = netsuite.delete(url=url)
+response = netsuite.request("DELETE", url=url)
 ```
 
 ## RESTlet
 
 "A restlet is a SuiteScript that executes when called by an external application or by another SuiteScript. Depending on how the RESTlet is written and called, it may also return data to the calling application."
 
 The *restsuite.NetSuiteRESTlet* class acts as an external application that allows you to activate RESTlets based on a handful of HTTP verbs:
@@ -174,15 +171,15 @@
     consumer_secret = CONSUMER_SECRET,
     token_key = TOKEN_KEY,
     token_secret = TOKEN_SECRET
 )
 
 url = "https://{}.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script={}&deploy={}".format(NS_ACCOUNT_ID, SCRIPT_ID, DEPLOYMENT_ID)
 
-response = netsuite.get(url)
+response = netsuite.request("GET", url)
 ```
 
 ## SuiteQL
 
 NetSuite allows for users to query their records their version of SQL, SuiteQL. In order to utilize SuiteQL, query strings are sent to a suiteql endpoint. SuiteQL queries can be sent to Netsuite using the NetSuiteQL class:
 
 ```python
```

### Comparing `restsuite-0.1.7.1/README.md` & `restsuite-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 # restsuite
 
 restsuite is a python package developed to help developers interact with the Netsuite REST API. restsuite offers a number of classes that can be utilized to interact with Netsuite's Suite-Talk, RESTlet, or SuiteQL services. restsuite currently utilizes Netsuite's token authentication methods, however, current development is under way for supporting Netsuite's Oauth2 authentication methods. 
 
 
-### Disclaimer:  
-
-*restsuite is still in developement stages and is currently being tested through usage in our company. Although open to the public for use, understand that this is not a stable version of the restsuite package. Integrating restsuite into production applications at this stage is not advised.*
 
 ## Installation
 
 restsuite is part of the Python Package Index (PyPI) and can thus be installed with pip:
 
 ```
 pip install restsuite
 ```
 
-restsuite requires a python version of 3.8 or higher and depends only on the [requests python package](https://requests.readthedocs.io/en/latest/) 
+restsuite requires a python version of 3.8 or higher and depends on the [requests python package](https://requests.readthedocs.io/en/latest/) and the [requests_oauthlib python package](https://pypi.org/project/requests-oauthlib/)
 
 
 ## Getting Started
 
 As restsuite is an abstraction of the Netsuite API, it will be helpful to become familiar with, or at least reference, the Netsuite API documentation:
 
 - [Suite-Talk Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1540391670.html)
 - [RESTlet Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2970701.html)
 - [SuiteQL Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156257770590.html)
 
 ### Authentication
 
-Each of the provided classes (NetSuiteRest, NetSuiteRESTlet, NetSuiteQL) handle authentication for the developer. All that is required is basic account information that can be generated in the user's account integration settings (see [REST Web Services Prerequisites and Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544787084.html) for a guide on setting up your Netsuite application to utilize REST capabilities)
+Each of the provided classes (NetSuiteRest, NetSuiteRESTlet, NetSuiteQL) utilize the [requests_oauthlib](https://pypi.org/project/requests-oauthlib/) package to handle authentication for the developer. All that is required is basic account information that can be generated in the user's account integration settings (see [REST Web Services Prerequisites and Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544787084.html) for a guide on setting up your Netsuite application to utilize REST capabilities)
 
 Each class requires that you pass the following attributes upon object instantiation:
 - Netsuite Account ID : This can be found the Netsuite url path (e.g: *https://{{ account_id }}.app.netsuite.com)*)
 - Consumer Key : Consumer Key and Secret are provided upon integration record creation [Integration Record Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4389727047.html).
 - Consumer Secret : Consumer Secret is provided upon integation record creation [Integration Record Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4389727047.html)
 - Token Key : Tokens can be generated a number of ways. We are currently developing a Class for generating tokens with the [issuetoken endpoint](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157017286140.html). For the time being, you can [generate a token with the Netsuite UI](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4254081947.html).
 - Token Secret : See Token Key
@@ -59,58 +56,58 @@
 )
 ```
 
 #### Getting a Record (GET):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job".format(NS_ACCOUNT_ID)
 
-response = netsuite.get(url)
+response = netsuite.request("GET", url)
 
-if response.status_code <= 300:
+if response.status_code < 300:
     data = response.json()
 ```
-*[Getting docs]()*
+*[Getting docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545141500.html#Getting-a-Record-Instance)*
 
 *It is important to note here that all classes will require the full URL to be passed to each request method.*
 
 #### Creating a Record object (POST):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"entityid": "New Customer", "companyname": "My Company", "subsidiary": {"id": "1"}}
 
-response = netsuite.post(url=url, body=body)
+response = netsuite.request("POST", url=url, body=body)
 ```
 *[Creating docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545141395.html)*
 
 #### Updating a Record object (PATCH):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"entityid": "Updated Customer"}
 
-response = netsuite.patch(url=url, body=body)
+response = netsuite.request("PATCH", url=url, body=body)
 ```
 *[Updating docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545142173.html)*
 
 #### Upserting a Record object (PUT):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"firstName": "John", "lastName": "Smith"}
 
-response = netsuite.put(url=url, body=body)
+response = netsuite.request("PUT", url=url, body=body)
 ```
 *[Upsert docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156335203191.html)*
 
 #### Deleting a Record object (DELETE)
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
-response = netsuite.delete(url=url)
+response = netsuite.request("DELETE", url=url)
 ```
 
 ## RESTlet
 
 "A restlet is a SuiteScript that executes when called by an external application or by another SuiteScript. Depending on how the RESTlet is written and called, it may also return data to the calling application."
 
 The *restsuite.NetSuiteRESTlet* class acts as an external application that allows you to activate RESTlets based on a handful of HTTP verbs:
@@ -136,15 +133,15 @@
     consumer_secret = CONSUMER_SECRET,
     token_key = TOKEN_KEY,
     token_secret = TOKEN_SECRET
 )
 
 url = "https://{}.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script={}&deploy={}".format(NS_ACCOUNT_ID, SCRIPT_ID, DEPLOYMENT_ID)
 
-response = netsuite.get(url)
+response = netsuite.request("GET", url)
 ```
 
 ## SuiteQL
 
 NetSuite allows for users to query their records their version of SQL, SuiteQL. In order to utilize SuiteQL, query strings are sent to a suiteql endpoint. SuiteQL queries can be sent to Netsuite using the NetSuiteQL class:
 
 ```python
```

### Comparing `restsuite-0.1.7.1/pyproject.toml` & `restsuite-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "restsuite"
-version = "0.1.7.1"
+version = "1.0.0"
 description = "Easily work with Netsuite's REST API"
 readme = "README.md"
 authors = [
     {name="Peter Williams", email="petercw94@gmail.com"},
     {name="Peter Williams"},
     {name="Richard Demke"},
     {name="Andy Gannaway"}
@@ -20,15 +20,16 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers"
 ]
 keywords = ["netsuite", "oauth", "rest"]
 dependencies = [
-    "requests"
+    "requests",
+    "requests-oauthlib"
 ]
 requires-python = ">=3.8"
 
 
 [project.urls]
 Homepage = "https://github.com/Petercw94/restsuite"
```

### Comparing `restsuite-0.1.7.1/restsuite/rest.py` & `restsuite-1.0.0/restsuite/base_rest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 """
-Module for handling all REST related requests in the Netsuite API.
+Base Class for SuiteTalk and RESTlet.
 """
 
-
-import json
 import requests
+import json
 
-from .base_rest import Rest
-
+from requests_oauthlib import OAuth1
 
-class NetSuiteRest(Rest):
-    """
-    """
 
+class Rest:
     def __init__(self, account_id, consumer_key, consumer_secret, token_key=None, token_secret=None) -> None:
-        super().__init__(account_id, consumer_key, consumer_secret, token_key, token_secret)
+        self.auth = OAuth1(
+            realm=account_id,
+            client_key=consumer_key,
+            client_secret=consumer_secret,
+            resource_owner_key=token_key,
+            resource_owner_secret=token_secret,
+            signature_method="HMAC-SHA256"
+        )
 
-    def patch(self, url: str, body: dict, headers=None):
+    def request(self, method: str, url: str, **kwargs):
         """
-        Update a record in Netsuite.
-
-        Wrapper function for all endpoints in the Netsuite API that accept the 
-        PATCH http method.
+        NEW for version 1.
 
-        NOTE: To delete a value from a record, simply pass null as the value.
+        Main request method inherited by each NetSuite interface. 
+        Key-word arguments can be passed dependent upon the http 
+        method desired. This allows for a single method to be called
+        for every method desired. 
 
         Args:
-        -----
-        - url (str) -> The url from which to get data (actual url, not base string. see Examples section for example)
-        - body (dict) -> The PATCH body containing fields to update and their new values as key-value pairs.
-        - headers (dict) -> Optional dictionary of headers to override the defaults. (See README or NetsuiteOAuth.generate_headers for defaults)
-
-        Returns:
-        --------
-        - response (obj) -> requests.response object from PATCH request. 
-
-        Examples:
-        ---------
-        URL: https://{{ NETSUITE ACCOUNT ID }}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345
-
-        BODY: {"entityid": "Updated Customer"} <- update customer 12345's entity id to "Updated Customer"
-
-        HEADERS: {"Prefer": "respond-async", "limit": 100, "offset": 2}
-            NOTE: The get method would take the above headers parameter and add the Authorization 
-            header to it, in order to properly sign the request. All other default headers will be dropped.
+            method (str) : HTTP method for request
+            url (str) : url to send request to
+
+        Kwargs:
+            headers (dict) : desired request headers for the request
+            body (dict) : body data for POST, PATCH, PUT type requests
+            params (dict) : query parameters for request NOTE: query params 
+                            can also be passed directly into the url.
+
+        Returns 
+            response (obj) : requests.Response instance object
+
         """
+        headers = kwargs.get('headers')
+        body = kwargs.get('body')
+        params = kwargs.get('params')
 
         # type checking
         if headers and not isinstance(headers, dict):
             raise TypeError(
-                "Expected dictionary for headers parameter. Received: {}".format(type(headers)))
+                "Expected type dict for headers | received type: {}".format(
+                    type(headers))
+            )
 
-        if not isinstance(body, dict):
+        if body and not isinstance(body, dict):
             raise TypeError(
-                "Expected dictionary for headers parameter. Received: {}".format(type(body)))
-
-        # generate default auth headers:
-        default_headers = self.auth.generate_auth_header("PATCH", url)
-
-        # override headers if necessary
-        if headers:
-            headers["Authorization"] = default_headers["Authorization"]
+                "Expected type dict for body | received type: {}".format(
+                    type(headers))
+            )
+        # if no headers are provided, default to the following
+        if not headers:
+            headers = {
+                "Prefer": "transient",
+                "Content-Type": "application/json",
+                "cache-control": "no-cache"
+            }
+
+        # request library raises ValueError if GET or HEAD requests contain a body
+        if method.upper() in ("GET", "HEAD"):
+            res = requests.request(method.upper(), url,
+                                   headers=headers, auth=self.auth, params=params)
+        # all other requests can have the body passed
         else:
-            headers = default_headers
-
-        response = requests.patch(
-            url, headers=headers, data=json.dumps(body, default=str))
+            res = requests.request(method.upper(), url,
+                                   headers=headers, auth=self.auth, params=params, data=json.dumps(body, default=str))
 
-        return response
+        return res
```

### Comparing `restsuite-0.1.7.1/restsuite/restlet.py` & `restsuite-1.0.0/restsuite/restlet.py`

 * *Files identical despite different names*

### Comparing `restsuite-0.1.7.1/restsuite/suiteql.py` & `restsuite-1.0.0/restsuite/suiteql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 """
 Module for making SuiteQL queries
 """
 
 import json
 
-from .auth import NetsuiteOAuth
+from requests_oauthlib import OAuth1
 import requests
 
 
 class NetSuiteQL:
     """
     """
 
     def __init__(self, account_id, consumer_key, consumer_secret, token_key=None, token_secret=None) -> None:
-        self.auth = NetsuiteOAuth(
-            account_id, consumer_key, consumer_secret, token_key, token_secret)
+        self.auth = OAuth1(
+            realm=account_id,
+            client_key=consumer_key,
+            client_secret=consumer_secret,
+            resource_owner_key=token_key,
+            resource_owner_secret=token_secret,
+            signature_method="HMAC-SHA256"
+        )
         self.url = "https://{}.suitetalk.api.netsuite.com/services/rest/query/v1/suiteql".format(
             account_id)
         self.items = []
         self.response_body = []
 
     def query(self, url, query_string: str):
         """
@@ -38,17 +44,21 @@
         -------
         - response (obj) -> requests.response object from POST request.
 
         """
 
         body = json.dumps({"q": query_string})
 
-        headers = self.auth.generate_auth_header("POST", url)
+        headers = {
+            "Prefer": "transient",
+            "Content-Type": "application/json",
+            "cache-control": "no-cache"
+        }
 
-        response = requests.post(url, headers=headers, data=body, cookies={
+        response = requests.post(url, headers=headers, auth=self.auth, data=body, cookies={
                                  'NS_ROUTING_VERSION': 'LAGGING'})
 
         return response
 
     def suiteql(self, query_string: str):
         """
         Returns all results for a SuiteQL query.
```

### Comparing `restsuite-0.1.7.1/restsuite.egg-info/PKG-INFO` & `restsuite-1.0.0/restsuite.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restsuite
-Version: 0.1.7.1
+Version: 1.0.0
 Summary: Easily work with Netsuite's REST API
 Author: Peter Williams, Richard Demke, Andy Gannaway
 Author-email: Peter Williams <petercw94@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Williams
         
@@ -37,40 +37,37 @@
 License-File: LICENSE
 
 # restsuite
 
 restsuite is a python package developed to help developers interact with the Netsuite REST API. restsuite offers a number of classes that can be utilized to interact with Netsuite's Suite-Talk, RESTlet, or SuiteQL services. restsuite currently utilizes Netsuite's token authentication methods, however, current development is under way for supporting Netsuite's Oauth2 authentication methods. 
 
 
-### Disclaimer:  
-
-*restsuite is still in developement stages and is currently being tested through usage in our company. Although open to the public for use, understand that this is not a stable version of the restsuite package. Integrating restsuite into production applications at this stage is not advised.*
 
 ## Installation
 
 restsuite is part of the Python Package Index (PyPI) and can thus be installed with pip:
 
 ```
 pip install restsuite
 ```
 
-restsuite requires a python version of 3.8 or higher and depends only on the [requests python package](https://requests.readthedocs.io/en/latest/) 
+restsuite requires a python version of 3.8 or higher and depends on the [requests python package](https://requests.readthedocs.io/en/latest/) and the [requests_oauthlib python package](https://pypi.org/project/requests-oauthlib/)
 
 
 ## Getting Started
 
 As restsuite is an abstraction of the Netsuite API, it will be helpful to become familiar with, or at least reference, the Netsuite API documentation:
 
 - [Suite-Talk Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1540391670.html)
 - [RESTlet Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2970701.html)
 - [SuiteQL Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156257770590.html)
 
 ### Authentication
 
-Each of the provided classes (NetSuiteRest, NetSuiteRESTlet, NetSuiteQL) handle authentication for the developer. All that is required is basic account information that can be generated in the user's account integration settings (see [REST Web Services Prerequisites and Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544787084.html) for a guide on setting up your Netsuite application to utilize REST capabilities)
+Each of the provided classes (NetSuiteRest, NetSuiteRESTlet, NetSuiteQL) utilize the [requests_oauthlib](https://pypi.org/project/requests-oauthlib/) package to handle authentication for the developer. All that is required is basic account information that can be generated in the user's account integration settings (see [REST Web Services Prerequisites and Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544787084.html) for a guide on setting up your Netsuite application to utilize REST capabilities)
 
 Each class requires that you pass the following attributes upon object instantiation:
 - Netsuite Account ID : This can be found the Netsuite url path (e.g: *https://{{ account_id }}.app.netsuite.com)*)
 - Consumer Key : Consumer Key and Secret are provided upon integration record creation [Integration Record Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4389727047.html).
 - Consumer Secret : Consumer Secret is provided upon integation record creation [Integration Record Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4389727047.html)
 - Token Key : Tokens can be generated a number of ways. We are currently developing a Class for generating tokens with the [issuetoken endpoint](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157017286140.html). For the time being, you can [generate a token with the Netsuite UI](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4254081947.html).
 - Token Secret : See Token Key
@@ -97,58 +94,58 @@
 )
 ```
 
 #### Getting a Record (GET):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job".format(NS_ACCOUNT_ID)
 
-response = netsuite.get(url)
+response = netsuite.request("GET", url)
 
-if response.status_code <= 300:
+if response.status_code < 300:
     data = response.json()
 ```
-*[Getting docs]()*
+*[Getting docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545141500.html#Getting-a-Record-Instance)*
 
 *It is important to note here that all classes will require the full URL to be passed to each request method.*
 
 #### Creating a Record object (POST):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"entityid": "New Customer", "companyname": "My Company", "subsidiary": {"id": "1"}}
 
-response = netsuite.post(url=url, body=body)
+response = netsuite.request("POST", url=url, body=body)
 ```
 *[Creating docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545141395.html)*
 
 #### Updating a Record object (PATCH):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"entityid": "Updated Customer"}
 
-response = netsuite.patch(url=url, body=body)
+response = netsuite.request("PATCH", url=url, body=body)
 ```
 *[Updating docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545142173.html)*
 
 #### Upserting a Record object (PUT):
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
 body = {"firstName": "John", "lastName": "Smith"}
 
-response = netsuite.put(url=url, body=body)
+response = netsuite.request("PUT", url=url, body=body)
 ```
 *[Upsert docs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156335203191.html)*
 
 #### Deleting a Record object (DELETE)
 ```python
 url = "https://{}.suitetalk.api.netsuite.com/services/rest/record/v1/job/12345".format(NS_ACCOUNT_ID)
 
-response = netsuite.delete(url=url)
+response = netsuite.request("DELETE", url=url)
 ```
 
 ## RESTlet
 
 "A restlet is a SuiteScript that executes when called by an external application or by another SuiteScript. Depending on how the RESTlet is written and called, it may also return data to the calling application."
 
 The *restsuite.NetSuiteRESTlet* class acts as an external application that allows you to activate RESTlets based on a handful of HTTP verbs:
@@ -174,15 +171,15 @@
     consumer_secret = CONSUMER_SECRET,
     token_key = TOKEN_KEY,
     token_secret = TOKEN_SECRET
 )
 
 url = "https://{}.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script={}&deploy={}".format(NS_ACCOUNT_ID, SCRIPT_ID, DEPLOYMENT_ID)
 
-response = netsuite.get(url)
+response = netsuite.request("GET", url)
 ```
 
 ## SuiteQL
 
 NetSuite allows for users to query their records their version of SQL, SuiteQL. In order to utilize SuiteQL, query strings are sent to a suiteql endpoint. SuiteQL queries can be sent to Netsuite using the NetSuiteQL class:
 
 ```python
```

