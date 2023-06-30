# Comparing `tmp/modular_cli_sdk-1.1.1.tar.gz` & `tmp/modular_cli_sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/onsha/Develop/EPAM/temp-modular-cli-sdk/dist/.tmp-8nppxv3l/modular_cli_sdk-1.1.1.tar", last modified: Fri Jun 30 09:23:45 2023, max compression
+gzip compressed data, was "/Users/onsha/Develop/EPAM/temp-modular-cli-sdk/dist/.tmp-1daljmnz/modular_cli_sdk-1.1.2.tar", last modified: Fri Jun 30 09:32:35 2023, max compression
```

## Comparing `modular_cli_sdk-1.1.1.tar` & `modular_cli_sdk-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:23:45.607035 modular_cli_sdk-1.1.1/
--rw-r--r--   0 onsha      (501) staff       (20)    11357 2023-06-29 14:19:12.000000 modular_cli_sdk-1.1.1/LICENSE
--rw-r--r--   0 onsha      (501) staff       (20)     2723 2023-06-30 09:23:45.607159 modular_cli_sdk-1.1.1/PKG-INFO
--rw-r--r--   0 onsha      (501) staff       (20)     2222 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/README.md
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:23:45.601365 modular_cli_sdk-1.1.1/modular_cli_sdk/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:23:45.603858 modular_cli_sdk-1.1.1/modular_cli_sdk/client/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/client/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     6814 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/client/ssm_client.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:23:45.605874 modular_cli_sdk-1.1.1/modular_cli_sdk/commons/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/commons/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      186 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/commons/constants.py
--rw-r--r--   0 onsha      (501) staff       (20)      526 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/commons/exception.py
--rw-r--r--   0 onsha      (501) staff       (20)     2621 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/commons/logger.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:23:45.606574 modular_cli_sdk-1.1.1/modular_cli_sdk/services/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/services/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     7546 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/modular_cli_sdk/services/credentials_manager.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:23:45.603094 modular_cli_sdk-1.1.1/modular_cli_sdk.egg-info/
--rw-r--r--   0 onsha      (501) staff       (20)     2723 2023-06-30 09:23:45.000000 modular_cli_sdk-1.1.1/modular_cli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 onsha      (501) staff       (20)      574 2023-06-30 09:23:45.000000 modular_cli_sdk-1.1.1/modular_cli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 onsha      (501) staff       (20)        1 2023-06-30 09:23:45.000000 modular_cli_sdk-1.1.1/modular_cli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 onsha      (501) staff       (20)       54 2023-06-30 09:23:45.000000 modular_cli_sdk-1.1.1/modular_cli_sdk.egg-info/requires.txt
--rw-r--r--   0 onsha      (501) staff       (20)       16 2023-06-30 09:23:45.000000 modular_cli_sdk-1.1.1/modular_cli_sdk.egg-info/top_level.txt
--rw-r--r--   0 onsha      (501) staff       (20)       86 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/pyproject.toml
--rw-r--r--   0 onsha      (501) staff       (20)      695 2023-06-30 09:23:45.607763 modular_cli_sdk-1.1.1/setup.cfg
--rw-r--r--   0 onsha      (501) staff       (20)       37 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.1/setup.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:32:35.801102 modular_cli_sdk-1.1.2/
+-rw-r--r--   0 onsha      (501) staff       (20)    11357 2023-06-29 14:19:12.000000 modular_cli_sdk-1.1.2/LICENSE
+-rw-r--r--   0 onsha      (501) staff       (20)     2181 2023-06-30 09:32:35.801204 modular_cli_sdk-1.1.2/PKG-INFO
+-rw-r--r--   0 onsha      (501) staff       (20)     1680 2023-06-30 09:32:16.000000 modular_cli_sdk-1.1.2/README.md
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:32:35.795986 modular_cli_sdk-1.1.2/modular_cli_sdk/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:32:35.798002 modular_cli_sdk-1.1.2/modular_cli_sdk/client/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/client/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     6814 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/client/ssm_client.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:32:35.800022 modular_cli_sdk-1.1.2/modular_cli_sdk/commons/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/commons/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      186 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/commons/constants.py
+-rw-r--r--   0 onsha      (501) staff       (20)      526 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/commons/exception.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2621 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/commons/logger.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:32:35.800657 modular_cli_sdk-1.1.2/modular_cli_sdk/services/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/services/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7546 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/modular_cli_sdk/services/credentials_manager.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:32:35.797539 modular_cli_sdk-1.1.2/modular_cli_sdk.egg-info/
+-rw-r--r--   0 onsha      (501) staff       (20)     2181 2023-06-30 09:32:35.000000 modular_cli_sdk-1.1.2/modular_cli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 onsha      (501) staff       (20)      574 2023-06-30 09:32:35.000000 modular_cli_sdk-1.1.2/modular_cli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 onsha      (501) staff       (20)        1 2023-06-30 09:32:35.000000 modular_cli_sdk-1.1.2/modular_cli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       54 2023-06-30 09:32:35.000000 modular_cli_sdk-1.1.2/modular_cli_sdk.egg-info/requires.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       16 2023-06-30 09:32:35.000000 modular_cli_sdk-1.1.2/modular_cli_sdk.egg-info/top_level.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       86 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/pyproject.toml
+-rw-r--r--   0 onsha      (501) staff       (20)      695 2023-06-30 09:32:35.801703 modular_cli_sdk-1.1.2/setup.cfg
+-rw-r--r--   0 onsha      (501) staff       (20)       37 2023-06-29 15:07:43.000000 modular_cli_sdk-1.1.2/setup.py
```

### Comparing `modular_cli_sdk-1.1.1/LICENSE` & `modular_cli_sdk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_cli_sdk-1.1.1/PKG-INFO` & `modular_cli_sdk-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 Metadata-Version: 2.1
 Name: modular_cli_sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: Core component for CLI tools built atop of Modular Framework
 Home-page: https://github.com/epam/modular-cli-sdk
 Author: EPAM Systems
 Author-email: support@syndicate.team
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: hvac
 License-File: LICENSE
 
-# This is a temporary repository used to remap projects before push to Github
-
 # Modular CLI SDK
-
-
-### [Building distribution archives](https://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archives)
-- Make sure you have the latest version of PyPA’s build installed: `python3 -m pip install --upgrade build`
-- Run the command form the same directory where `pyptoject.toml` is located: `python3 -m build`
-- This command should output a lot of text and once completed should generate two files in the dist directory:
-```
-dist/
-    modular_cli_sdk-{version}.tar.gz
-    modular_cli_sdk-{version}-py3-none-any.whl
-```
+Modular CLI SDK is a core component for CLI tools built atop of Modular Framework
 
 ### Installation
 To install Modular CLI SDK please use `pip` command:
 * standard installation `pip install "modular_cli_sdk"`
 
 ### Usage:
 #### 1. Credentials Manager
@@ -56,23 +44,23 @@
 configuration.credentials_manager.store(config=$config_dict)
 configuration.credentials_manager.extract()
 configuration.credentials_manager.extract()
 ```
 
 * store(config= ) # saving given configuration  
   Parameters:
-  * config (dict) [Required] - takes a dictionary with tool configuration data  
+  * `config` (dict) [Required] - takes a dictionary with tool configuration data  
   Return type:
-  * str  
+  * `str`  
 
 * extract() # retrieve saved configuration  
   Parameters:
-  * None  
+  * `None`  
   Return type:
-  * dict
+  * `dict`
 
 * clean_up() # delete saved configuration 
   Parameters:
-  * None  
+  * `None`  
   Return type:
-  * str  
+  * `str`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `modular_cli_sdk-1.1.1/README.md` & `modular_cli_sdk-1.1.2/modular_cli_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# This is a temporary repository used to remap projects before push to Github
+Metadata-Version: 2.1
+Name: modular-cli-sdk
+Version: 1.1.2
+Summary: Core component for CLI tools built atop of Modular Framework
+Home-page: https://github.com/epam/modular-cli-sdk
+Author: EPAM Systems
+Author-email: support@syndicate.team
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: hvac
+License-File: LICENSE
 
 # Modular CLI SDK
-
-
-### [Building distribution archives](https://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archives)
-- Make sure you have the latest version of PyPA’s build installed: `python3 -m pip install --upgrade build`
-- Run the command form the same directory where `pyptoject.toml` is located: `python3 -m build`
-- This command should output a lot of text and once completed should generate two files in the dist directory:
-```
-dist/
-    modular_cli_sdk-{version}.tar.gz
-    modular_cli_sdk-{version}-py3-none-any.whl
-```
+Modular CLI SDK is a core component for CLI tools built atop of Modular Framework
 
 ### Installation
 To install Modular CLI SDK please use `pip` command:
 * standard installation `pip install "modular_cli_sdk"`
 
 ### Usage:
 #### 1. Credentials Manager
@@ -41,23 +44,23 @@
 configuration.credentials_manager.store(config=$config_dict)
 configuration.credentials_manager.extract()
 configuration.credentials_manager.extract()
 ```
 
 * store(config= ) # saving given configuration  
   Parameters:
-  * config (dict) [Required] - takes a dictionary with tool configuration data  
+  * `config` (dict) [Required] - takes a dictionary with tool configuration data  
   Return type:
-  * str  
+  * `str`  
 
 * extract() # retrieve saved configuration  
   Parameters:
-  * None  
+  * `None`  
   Return type:
-  * dict
+  * `dict`
 
 * clean_up() # delete saved configuration 
   Parameters:
-  * None  
+  * `None`  
   Return type:
-  * str  
-  
+  * `str`  
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `modular_cli_sdk-1.1.1/modular_cli_sdk/client/ssm_client.py` & `modular_cli_sdk-1.1.2/modular_cli_sdk/client/ssm_client.py`

 * *Files identical despite different names*

### Comparing `modular_cli_sdk-1.1.1/modular_cli_sdk/commons/exception.py` & `modular_cli_sdk-1.1.2/modular_cli_sdk/commons/exception.py`

 * *Files identical despite different names*

### Comparing `modular_cli_sdk-1.1.1/modular_cli_sdk/commons/logger.py` & `modular_cli_sdk-1.1.2/modular_cli_sdk/commons/logger.py`

 * *Files identical despite different names*

### Comparing `modular_cli_sdk-1.1.1/modular_cli_sdk/services/credentials_manager.py` & `modular_cli_sdk-1.1.2/modular_cli_sdk/services/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `modular_cli_sdk-1.1.1/modular_cli_sdk.egg-info/SOURCES.txt` & `modular_cli_sdk-1.1.2/modular_cli_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modular_cli_sdk-1.1.1/setup.cfg` & `modular_cli_sdk-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modular_cli_sdk
-version = 1.1.1
+version = 1.1.2
 requires-python = >=3.8
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 license = Apache-2.0
 description = Core component for CLI tools built atop of Modular Framework
```

