# Comparing `tmp/ckanext-googleanalyticsbasic-0.2.0.tar.gz` & `tmp/ckanext-googleanalyticsbasic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-googleanalyticsbasic-0.2.0.tar", last modified: Wed Sep 14 17:03:41 2022, max compression
+gzip compressed data, was "ckanext-googleanalyticsbasic-0.2.1.tar", last modified: Fri Jun 30 14:47:35 2023, max compression
```

## Comparing `ckanext-googleanalyticsbasic-0.2.0.tar` & `ckanext-googleanalyticsbasic-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 17:03:41.170709 ckanext-googleanalyticsbasic-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-09-14 17:03:41.170709 ckanext-googleanalyticsbasic-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2294 2022-09-14 17:03:40.000000 ckanext-googleanalyticsbasic-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 17:03:41.170709 ckanext-googleanalyticsbasic-0.2.0/ckanext/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-14 17:03:40.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 17:03:41.170709 ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-14 17:03:40.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-09-14 17:03:40.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 17:03:41.170709 ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 17:03:40.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-09-14 17:03:40.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-09-14 17:03:40.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/tests/test_scripts_present.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 17:03:41.170709 ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-09-14 17:03:41.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-09-14 17:03:41.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 17:03:41.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-09-14 17:03:41.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-14 17:03:41.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 17:03:41.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-14 17:03:41.000000 ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-14 17:03:41.170709 ckanext-googleanalyticsbasic-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-09-14 17:03:40.000000 ckanext-googleanalyticsbasic-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:47:35.027731 ckanext-googleanalyticsbasic-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-30 14:47:35.027731 ckanext-googleanalyticsbasic-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-30 14:47:34.000000 ckanext-googleanalyticsbasic-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:47:35.023731 ckanext-googleanalyticsbasic-0.2.1/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 14:47:34.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:47:35.027731 ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 14:47:34.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-30 14:47:34.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:47:35.027731 ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:47:34.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-30 14:47:34.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-30 14:47:34.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/tests/test_scripts_present.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:47:35.027731 ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-30 14:47:35.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 14:47:35.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:47:35.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 14:47:35.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 14:47:35.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:47:35.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 14:47:35.000000 ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-30 14:47:35.027731 ckanext-googleanalyticsbasic-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-30 14:47:34.000000 ckanext-googleanalyticsbasic-0.2.1/setup.py
```

### Comparing `ckanext-googleanalyticsbasic-0.2.0/PKG-INFO` & `ckanext-googleanalyticsbasic-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,97 @@
 Metadata-Version: 2.1
 Name: ckanext-googleanalyticsbasic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Basic extension to add google analytics tracking code in page header
 Home-page: https://github.com/GSA/ckanext-googleanalyticsbasic
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: UNKNOWN
-Description: [![Github Actions](https://github.com/GSA/ckanext-googleanalyticsbasic/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-googleanalyticsbasic/actions)
-        [![PyPI version](https://badge.fury.io/py/ckanext-googleanalyticsbasic.svg)](https://badge.fury.io/py/ckanext-googleanalyticsbasic)
-        
-        
-        ckanext-googleanalyticsbasic
-        ============================
-        
-        Puts the Google Analytics asynchronous tracking code into your page headers for basic Google Analytics page tracking.
-        
-        Installation
-        -------------
-        1. Install the extension as usual, e.g. (from an activated virtualenv)
-        		::
-        		
-        		$ pip install -e  git+https://github.com/GSA/ckanext-googleanalyticsbasic#egg=ckanext-googleanalyticsbasic
-        
-        2. Edit your development.ini (or similar) to provide space separated list of google ids
-        		::
-          	
-        		googleanalytics.ids = UA-1010101-1 UA-1010101-2
-        
-        3. Edit again your configuration ini file to activate the plugin with:
-        		::
-          	
-        		ckan.plugins = googleanalyticsbasic
-        
-        ### Compatibility
-        
-        This extension is compatible with these versions of CKAN.
-        
-        CKAN version | Compatibility
-        ------------ | -------------
-        <=2.8        | no
-        2.9          | yes
-        
-        ## Tests
-        
-        All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder.
-        
-        ## Using the Docker Dev Environment
-        
-        ### Build Environment
-        
-        To start environment, run:
-        ```docker-compose build```
-        ```docker-compose up```
-        
-        CKAN will start at localhost:5000
-        
-        To shut down environment, run:
-        
-        ```docker-compose down```
-        
-        To docker exec into the CKAN image, run:
-        
-        ```docker-compose exec app /bin/bash```
-        
-        ### Testing
-        
-        They follow the guidelines for [testing CKAN
-        extensions](https://docs.ckan.org/en/2.9/extensions/testing-extensions.html#testing-extensions).
-        
-        To run the extension tests, start the containers with `make up`, then:
-        
-            $ make test
-        
-        Lint the code.
-        
-            $ make lint
-        
-        ### Matrix builds
-        
-        The development environment drops as many dependencies as possible. It is
-        not meant to have feature parity with
-        [GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
-        mock external dependencies where possible.
-        
-        In order to support multiple versions of CKAN, or even upgrade to new versions
-        of CKAN, we support development and testing through the `CKAN_VERSION`
-        environment variable.
-        
-            $ make CKAN_VERSION=2.9 test
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+[![Github Actions](https://github.com/GSA/ckanext-googleanalyticsbasic/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-googleanalyticsbasic/actions)
+[![PyPI version](https://badge.fury.io/py/ckanext-googleanalyticsbasic.svg)](https://badge.fury.io/py/ckanext-googleanalyticsbasic)
+
+
+ckanext-googleanalyticsbasic
+============================
+
+Puts the Google Analytics asynchronous tracking code into your page headers for basic Google Analytics page tracking.
+
+Installation
+-------------
+1. Install the extension as usual, e.g. (from an activated virtualenv)
+		::
+		
+		$ pip install -e  git+https://github.com/GSA/ckanext-googleanalyticsbasic#egg=ckanext-googleanalyticsbasic
+
+2. Edit your development.ini (or similar) to provide space separated list of google ids
+		::
+  	
+		googleanalytics.ids = UA-1010101-1 UA-1010101-2
+
+3. Edit again your configuration ini file to activate the plugin with:
+		::
+  	
+		ckan.plugins = googleanalyticsbasic
+
+### Compatibility
+
+This extension is compatible with these versions of CKAN.
+
+CKAN version  | Compatibility
+------------- | -------------
+<=2.8         | no
+2.9           | yes
+2.10          | yes
+
+## Tests
+
+All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder.
+
+## Using the Docker Dev Environment
+
+### Build Environment
+
+To start environment, run:
+```docker-compose build```
+```docker-compose up```
+
+CKAN will start at localhost:5000
+
+To shut down environment, run:
+
+```docker-compose down```
+
+To docker exec into the CKAN image, run:
+
+```docker-compose exec app /bin/bash```
+
+### Testing
+
+They follow the guidelines for [testing CKAN
+extensions](https://docs.ckan.org/en/2.10/extensions/testing-extensions.html#testing-extensions).
+
+To run the extension tests, start the containers with `make up`, then:
+
+    $ make test
+
+Lint the code.
+
+    $ make lint
+
+### Matrix builds
+
+The development environment drops as many dependencies as possible. It is
+not meant to have feature parity with
+[GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
+mock external dependencies where possible.
+
+In order to support multiple versions of CKAN, or even upgrade to new versions
+of CKAN, we support development and testing through the `CKAN_VERSION`
+environment variable.
+
+    $ make CKAN_VERSION=2.10 test
+
+
```

### Comparing `ckanext-googleanalyticsbasic-0.2.0/README.md` & `ckanext-googleanalyticsbasic-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,19 @@
   	
 		ckan.plugins = googleanalyticsbasic
 
 ### Compatibility
 
 This extension is compatible with these versions of CKAN.
 
-CKAN version | Compatibility
------------- | -------------
-<=2.8        | no
-2.9          | yes
+CKAN version  | Compatibility
+------------- | -------------
+<=2.8         | no
+2.9           | yes
+2.10          | yes
 
 ## Tests
 
 All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder.
 
 ## Using the Docker Dev Environment
 
@@ -54,15 +55,15 @@
 To docker exec into the CKAN image, run:
 
 ```docker-compose exec app /bin/bash```
 
 ### Testing
 
 They follow the guidelines for [testing CKAN
-extensions](https://docs.ckan.org/en/2.9/extensions/testing-extensions.html#testing-extensions).
+extensions](https://docs.ckan.org/en/2.10/extensions/testing-extensions.html#testing-extensions).
 
 To run the extension tests, start the containers with `make up`, then:
 
     $ make test
 
 Lint the code.
 
@@ -75,8 +76,8 @@
 [GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
 mock external dependencies where possible.
 
 In order to support multiple versions of CKAN, or even upgrade to new versions
 of CKAN, we support development and testing through the `CKAN_VERSION`
 environment variable.
 
-    $ make CKAN_VERSION=2.9 test
+    $ make CKAN_VERSION=2.10 test
```

### Comparing `ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/plugin.py` & `ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 class GoogleAnalyticsBasicException(Exception):
     pass
 
 
 class GoogleAnalyticsBasicPlugin(p.SingletonPlugin):
     p.implements(p.IConfigurable, inherit=True)
-    p.implements(p.IRoutes, inherit=True)
     p.implements(p.IConfigurer, inherit=True)
     p.implements(p.ITemplateHelpers)
 
     def configure(self, config):
         '''Load config settings for this extension from config file.
 
         See IConfigurable.
```

### Comparing `ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/tests/test_plugin.py` & `ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalyticsbasic-0.2.0/ckanext/googleanalyticsbasic/tests/test_scripts_present.py` & `ckanext-googleanalyticsbasic-0.2.1/ckanext/googleanalyticsbasic/tests/test_scripts_present.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/PKG-INFO` & `ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,97 @@
 Metadata-Version: 2.1
 Name: ckanext-googleanalyticsbasic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Basic extension to add google analytics tracking code in page header
 Home-page: https://github.com/GSA/ckanext-googleanalyticsbasic
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: UNKNOWN
-Description: [![Github Actions](https://github.com/GSA/ckanext-googleanalyticsbasic/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-googleanalyticsbasic/actions)
-        [![PyPI version](https://badge.fury.io/py/ckanext-googleanalyticsbasic.svg)](https://badge.fury.io/py/ckanext-googleanalyticsbasic)
-        
-        
-        ckanext-googleanalyticsbasic
-        ============================
-        
-        Puts the Google Analytics asynchronous tracking code into your page headers for basic Google Analytics page tracking.
-        
-        Installation
-        -------------
-        1. Install the extension as usual, e.g. (from an activated virtualenv)
-        		::
-        		
-        		$ pip install -e  git+https://github.com/GSA/ckanext-googleanalyticsbasic#egg=ckanext-googleanalyticsbasic
-        
-        2. Edit your development.ini (or similar) to provide space separated list of google ids
-        		::
-          	
-        		googleanalytics.ids = UA-1010101-1 UA-1010101-2
-        
-        3. Edit again your configuration ini file to activate the plugin with:
-        		::
-          	
-        		ckan.plugins = googleanalyticsbasic
-        
-        ### Compatibility
-        
-        This extension is compatible with these versions of CKAN.
-        
-        CKAN version | Compatibility
-        ------------ | -------------
-        <=2.8        | no
-        2.9          | yes
-        
-        ## Tests
-        
-        All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder.
-        
-        ## Using the Docker Dev Environment
-        
-        ### Build Environment
-        
-        To start environment, run:
-        ```docker-compose build```
-        ```docker-compose up```
-        
-        CKAN will start at localhost:5000
-        
-        To shut down environment, run:
-        
-        ```docker-compose down```
-        
-        To docker exec into the CKAN image, run:
-        
-        ```docker-compose exec app /bin/bash```
-        
-        ### Testing
-        
-        They follow the guidelines for [testing CKAN
-        extensions](https://docs.ckan.org/en/2.9/extensions/testing-extensions.html#testing-extensions).
-        
-        To run the extension tests, start the containers with `make up`, then:
-        
-            $ make test
-        
-        Lint the code.
-        
-            $ make lint
-        
-        ### Matrix builds
-        
-        The development environment drops as many dependencies as possible. It is
-        not meant to have feature parity with
-        [GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
-        mock external dependencies where possible.
-        
-        In order to support multiple versions of CKAN, or even upgrade to new versions
-        of CKAN, we support development and testing through the `CKAN_VERSION`
-        environment variable.
-        
-            $ make CKAN_VERSION=2.9 test
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+[![Github Actions](https://github.com/GSA/ckanext-googleanalyticsbasic/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-googleanalyticsbasic/actions)
+[![PyPI version](https://badge.fury.io/py/ckanext-googleanalyticsbasic.svg)](https://badge.fury.io/py/ckanext-googleanalyticsbasic)
+
+
+ckanext-googleanalyticsbasic
+============================
+
+Puts the Google Analytics asynchronous tracking code into your page headers for basic Google Analytics page tracking.
+
+Installation
+-------------
+1. Install the extension as usual, e.g. (from an activated virtualenv)
+		::
+		
+		$ pip install -e  git+https://github.com/GSA/ckanext-googleanalyticsbasic#egg=ckanext-googleanalyticsbasic
+
+2. Edit your development.ini (or similar) to provide space separated list of google ids
+		::
+  	
+		googleanalytics.ids = UA-1010101-1 UA-1010101-2
+
+3. Edit again your configuration ini file to activate the plugin with:
+		::
+  	
+		ckan.plugins = googleanalyticsbasic
+
+### Compatibility
+
+This extension is compatible with these versions of CKAN.
+
+CKAN version  | Compatibility
+------------- | -------------
+<=2.8         | no
+2.9           | yes
+2.10          | yes
+
+## Tests
+
+All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder.
+
+## Using the Docker Dev Environment
+
+### Build Environment
+
+To start environment, run:
+```docker-compose build```
+```docker-compose up```
+
+CKAN will start at localhost:5000
+
+To shut down environment, run:
+
+```docker-compose down```
+
+To docker exec into the CKAN image, run:
+
+```docker-compose exec app /bin/bash```
+
+### Testing
+
+They follow the guidelines for [testing CKAN
+extensions](https://docs.ckan.org/en/2.10/extensions/testing-extensions.html#testing-extensions).
+
+To run the extension tests, start the containers with `make up`, then:
+
+    $ make test
+
+Lint the code.
+
+    $ make lint
+
+### Matrix builds
+
+The development environment drops as many dependencies as possible. It is
+not meant to have feature parity with
+[GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
+mock external dependencies where possible.
+
+In order to support multiple versions of CKAN, or even upgrade to new versions
+of CKAN, we support development and testing through the `CKAN_VERSION`
+environment variable.
+
+    $ make CKAN_VERSION=2.10 test
+
+
```

### Comparing `ckanext-googleanalyticsbasic-0.2.0/ckanext_googleanalyticsbasic.egg-info/SOURCES.txt` & `ckanext-googleanalyticsbasic-0.2.1/ckanext_googleanalyticsbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalyticsbasic-0.2.0/setup.py` & `ckanext-googleanalyticsbasic-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ckanext-googleanalyticsbasic',
-    version='0.2.0',
+    version='0.2.1',
     description="Basic extension to add google analytics tracking code in page header",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3'
     ],  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     keywords='',
```

