# Comparing `tmp/pymasmovil-0.0.8.tar.gz` & `tmp/pymasmovil-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymasmovil-0.0.8.tar", last modified: Fri Oct  9 12:56:50 2020, max compression
+gzip compressed data, was "dist/pymasmovil-0.0.9.tar", last modified: Thu Oct 22 08:07:02 2020, max compression
```

## Comparing `pymasmovil-0.0.8.tar` & `pymasmovil-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     6254 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4698 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil/errors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/errors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/errors/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      189 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/errors/http_error.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/errors/mm_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/models/account.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/models/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/models/contract.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/models/new_line_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2376 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/models/order_item.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/pymasmovil/models/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6254 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      603 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        9 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/pymasmovil.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-10-09 12:56:50.000000 pymasmovil-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      775 2020-10-09 12:56:39.000000 pymasmovil-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     6254 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil/errors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2383 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/errors/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      189 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/errors/http_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/errors/mm_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/models/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4120 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/models/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/models/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/models/new_line_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/models/order_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/pymasmovil/models/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6254 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      603 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        9 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/pymasmovil.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-10-22 08:07:02.000000 pymasmovil-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      775 2020-10-22 08:06:51.000000 pymasmovil-0.0.9/setup.py
```

### Comparing `pymasmovil-0.0.8/PKG-INFO` & `pymasmovil-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymasmovil
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for the Más Móvil's B2B API
 Home-page: https://gitlab.com/coopdevs/pymasmovil
 Author: Coopdevs
 Author-email: gerard.funosas@somconnexio.coop
 Maintainer: Daniel Palomar, Pau Pérez, Gerard Funosas
 License: UNKNOWN
 Description: # Más Móvil Python API client
```

### Comparing `pymasmovil-0.0.8/README.md` & `pymasmovil-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pymasmovil-0.0.8/pymasmovil/client.py` & `pymasmovil-0.0.9/pymasmovil/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,14 +53,33 @@
         return self._send_request(
             verb="POST",
             url="{url}{route}".format(url=self.base_url, route=route),
             params=params,
             payload=body,
         ).json()
 
+    def patch(self, route, params, body):
+        """ Sends a PATCH HTTP request
+
+        Args:
+            route (str): String with the route to the endpoint
+            params (tuple): Tuple with optional parameters of the request to send
+            body (dict): Dict with the body of the request to send
+
+        Return:
+            **response**: Returns the response object
+        """
+
+        return self._send_request(
+            verb="PATCH",
+            url="{url}{route}".format(url=self.base_url, route=route),
+            params=params,
+            payload=body,
+        ).json()
+
     def _send_request(self, verb, url, payload=None, params={}):
         """send the API request using the *requests.request* method
 
         Args:
             payload (dict), params (dict)
 
         Returns:
```

### Comparing `pymasmovil-0.0.8/pymasmovil/errors/exceptions.py` & `pymasmovil-0.0.9/pymasmovil/errors/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,13 +44,24 @@
     def __init__(self, is_portability, missing_argument_list):
         request_type = "portability" if is_portability else "new phone number registration"
 
         self.message = self.message.format(request_type, ', '.join(missing_argument_list))
         super().__init__(self.message)
 
 
+class TariffChangeRequiredParamsError(Exception):
+    """Exception raised when some required parameters to build a tariff change request
+    are missing."""
+
+    message = "Missing or empty required attributes for the requested {}: {}"
+
+    def __init__(self, update_type, missing_argument_list):
+        self.message = self.message.format(update_type, ', '.join(missing_argument_list))
+        super().__init__(self.message)
+
+
 class UnknownMMError(Exception):
     """Raised when the MM API returns an error with an unknown structure"""
 
     def __init__(self, MM_response_body):
         self.message = MM_response_body
         super().__init__(self.message)
```

### Comparing `pymasmovil-0.0.8/pymasmovil/errors/mm_error.py` & `pymasmovil-0.0.9/pymasmovil/errors/mm_error.py`

 * *Files identical despite different names*

### Comparing `pymasmovil-0.0.8/pymasmovil/models/account.py` & `pymasmovil-0.0.9/pymasmovil/models/account.py`

 * *Files identical despite different names*

### Comparing `pymasmovil-0.0.8/pymasmovil/models/contract.py` & `pymasmovil-0.0.9/pymasmovil/models/contract.py`

 * *Files identical despite different names*

### Comparing `pymasmovil-0.0.8/pymasmovil/models/new_line_request.py` & `pymasmovil-0.0.9/pymasmovil/models/new_line_request.py`

 * *Files identical despite different names*

### Comparing `pymasmovil-0.0.8/pymasmovil/models/order_item.py` & `pymasmovil-0.0.9/pymasmovil/models/order_item.py`

 * *Files identical despite different names*

### Comparing `pymasmovil-0.0.8/pymasmovil/models/session.py` & `pymasmovil-0.0.9/pymasmovil/models/session.py`

 * *Files identical despite different names*

### Comparing `pymasmovil-0.0.8/pymasmovil.egg-info/PKG-INFO` & `pymasmovil-0.0.9/pymasmovil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymasmovil
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for the Más Móvil's B2B API
 Home-page: https://gitlab.com/coopdevs/pymasmovil
 Author: Coopdevs
 Author-email: gerard.funosas@somconnexio.coop
 Maintainer: Daniel Palomar, Pau Pérez, Gerard Funosas
 License: UNKNOWN
 Description: # Más Móvil Python API client
```

### Comparing `pymasmovil-0.0.8/pymasmovil.egg-info/SOURCES.txt` & `pymasmovil-0.0.9/pymasmovil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymasmovil-0.0.8/setup.py` & `pymasmovil-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     README = f.read()
 
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 setup(
     name='pymasmovil',
     version=VERSION,
     author='Coopdevs',
     author_email='gerard.funosas@somconnexio.coop',
     maintainer='Daniel Palomar, Pau Pérez, Gerard Funosas',
```

