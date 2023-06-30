# Comparing `tmp/fnapy-1.4.0.tar.gz` & `tmp/fnapy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fnapy-1.4.0.tar", last modified: Thu Jun 29 16:25:19 2023, max compression
+gzip compressed data, was "dist/fnapy-1.4.1.tar", last modified: Fri Jun 30 10:02:41 2023, max compression
```

## Comparing `fnapy-1.4.0.tar` & `fnapy-1.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-29 16:25:19.000000 fnapy-1.4.0/
--rw-rw-r--   0 damien    (1000) damien    (1000)      135 2023-05-29 09:36:13.000000 fnapy-1.4.0/AUTHORS.rst
--rw-rw-r--   0 damien    (1000) damien    (1000)     1067 2023-05-29 09:36:13.000000 fnapy-1.4.0/LICENSE.txt
--rw-rw-r--   0 damien    (1000) damien    (1000)      243 2023-05-29 09:36:13.000000 fnapy-1.4.0/MANIFEST.in
--rw-rw-r--   0 damien    (1000) damien    (1000)     5811 2023-06-29 16:25:19.000000 fnapy-1.4.0/PKG-INFO
--rw-rw-r--   0 damien    (1000) damien    (1000)      585 2023-05-29 09:36:13.000000 fnapy-1.4.0/README.rst
-drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-29 16:25:19.000000 fnapy-1.4.0/docs/
--rw-rw-r--   0 damien    (1000) damien    (1000)     4554 2023-06-29 15:19:05.000000 fnapy-1.4.0/docs/CHANGELOG.rst
--rw-rw-r--   0 damien    (1000) damien    (1000)     6758 2023-05-29 09:36:13.000000 fnapy-1.4.0/docs/Makefile
--rw-rw-r--   0 damien    (1000) damien    (1000)      553 2023-05-29 09:36:13.000000 fnapy-1.4.0/docs/api.rst
--rw-rw-r--   0 damien    (1000) damien    (1000)     5320 2023-06-29 15:06:59.000000 fnapy-1.4.0/docs/conf.py
--rw-rw-r--   0 damien    (1000) damien    (1000)      474 2023-05-29 09:36:13.000000 fnapy-1.4.0/docs/index.rst
--rw-rw-r--   0 damien    (1000) damien    (1000)     6699 2023-05-29 09:36:13.000000 fnapy-1.4.0/docs/make.bat
--rw-rw-r--   0 damien    (1000) damien    (1000)     8417 2023-06-29 15:15:40.000000 fnapy-1.4.0/docs/quickstart.rst
-drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy/
--rw-rw-r--   0 damien    (1000) damien    (1000)       22 2023-06-29 15:20:03.000000 fnapy-1.4.0/fnapy/__init__.py
--rw-rw-r--   0 damien    (1000) damien    (1000)     2311 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/compat.py
--rw-rw-r--   0 damien    (1000) damien    (1000)     8092 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/config.py
--rw-rw-r--   0 damien    (1000) damien    (1000)     2627 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/connection.py
--rw-rw-r--   0 damien    (1000) damien    (1000)      740 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/exceptions.py
--rw-rw-r--   0 damien    (1000) damien    (1000)    24093 2023-05-29 09:36:13.000000 fnapy-1.4.0/fnapy/fnapy_manager.py
--rw-rw-r--   0 damien    (1000) damien    (1000)    16862 2023-06-29 14:54:57.000000 fnapy-1.4.0/fnapy/utils.py
-drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/
--rw-rw-r--   0 damien    (1000) damien    (1000)     5811 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/PKG-INFO
--rw-rw-r--   0 damien    (1000) damien    (1000)      469 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/SOURCES.txt
--rw-rw-r--   0 damien    (1000) damien    (1000)        1 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/dependency_links.txt
--rw-rw-r--   0 damien    (1000) damien    (1000)       24 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/requires.txt
--rw-rw-r--   0 damien    (1000) damien    (1000)       12 2023-06-29 16:25:19.000000 fnapy-1.4.0/fnapy.egg-info/top_level.txt
--rw-rw-r--   0 damien    (1000) damien    (1000)        1 2023-06-29 14:18:54.000000 fnapy-1.4.0/fnapy.egg-info/zip-safe
--rw-rw-r--   0 damien    (1000) damien    (1000)      398 2023-06-29 16:25:19.000000 fnapy-1.4.0/setup.cfg
--rw-rw-r--   0 damien    (1000) damien    (1000)     1687 2023-05-29 09:36:13.000000 fnapy-1.4.0/setup.py
+drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-30 10:02:41.000000 fnapy-1.4.1/
+-rw-rw-r--   0 damien    (1000) damien    (1000)      135 2023-05-29 09:36:13.000000 fnapy-1.4.1/AUTHORS.rst
+-rw-rw-r--   0 damien    (1000) damien    (1000)     1067 2023-05-29 09:36:13.000000 fnapy-1.4.1/LICENSE.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)      243 2023-05-29 09:36:13.000000 fnapy-1.4.1/MANIFEST.in
+-rw-rw-r--   0 damien    (1000) damien    (1000)     5939 2023-06-30 10:02:41.000000 fnapy-1.4.1/PKG-INFO
+-rw-rw-r--   0 damien    (1000) damien    (1000)      585 2023-05-29 09:36:13.000000 fnapy-1.4.1/README.rst
+drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-30 10:02:41.000000 fnapy-1.4.1/docs/
+-rw-rw-r--   0 damien    (1000) damien    (1000)     4682 2023-06-30 09:53:41.000000 fnapy-1.4.1/docs/CHANGELOG.rst
+-rw-rw-r--   0 damien    (1000) damien    (1000)     6758 2023-05-29 09:36:13.000000 fnapy-1.4.1/docs/Makefile
+-rw-rw-r--   0 damien    (1000) damien    (1000)      553 2023-05-29 09:36:13.000000 fnapy-1.4.1/docs/api.rst
+-rw-rw-r--   0 damien    (1000) damien    (1000)     5320 2023-06-30 09:53:50.000000 fnapy-1.4.1/docs/conf.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)      474 2023-05-29 09:36:13.000000 fnapy-1.4.1/docs/index.rst
+-rw-rw-r--   0 damien    (1000) damien    (1000)     6699 2023-05-29 09:36:13.000000 fnapy-1.4.1/docs/make.bat
+-rw-rw-r--   0 damien    (1000) damien    (1000)     8475 2023-06-30 09:55:04.000000 fnapy-1.4.1/docs/quickstart.rst
+drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-30 10:02:41.000000 fnapy-1.4.1/fnapy/
+-rw-rw-r--   0 damien    (1000) damien    (1000)       22 2023-06-30 09:57:18.000000 fnapy-1.4.1/fnapy/__init__.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)     2311 2023-05-29 09:36:13.000000 fnapy-1.4.1/fnapy/compat.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)     8217 2023-06-30 09:48:32.000000 fnapy-1.4.1/fnapy/config.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)     2627 2023-05-29 09:36:13.000000 fnapy-1.4.1/fnapy/connection.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)      740 2023-05-29 09:36:13.000000 fnapy-1.4.1/fnapy/exceptions.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)    24093 2023-05-29 09:36:13.000000 fnapy-1.4.1/fnapy/fnapy_manager.py
+-rw-rw-r--   0 damien    (1000) damien    (1000)    16862 2023-06-29 14:54:57.000000 fnapy-1.4.1/fnapy/utils.py
+drwxrwxr-x   0 damien    (1000) damien    (1000)        0 2023-06-30 10:02:41.000000 fnapy-1.4.1/fnapy.egg-info/
+-rw-rw-r--   0 damien    (1000) damien    (1000)     5939 2023-06-30 10:02:41.000000 fnapy-1.4.1/fnapy.egg-info/PKG-INFO
+-rw-rw-r--   0 damien    (1000) damien    (1000)      469 2023-06-30 10:02:41.000000 fnapy-1.4.1/fnapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)        1 2023-06-30 10:02:41.000000 fnapy-1.4.1/fnapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)       24 2023-06-30 10:02:41.000000 fnapy-1.4.1/fnapy.egg-info/requires.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)       12 2023-06-30 10:02:41.000000 fnapy-1.4.1/fnapy.egg-info/top_level.txt
+-rw-rw-r--   0 damien    (1000) damien    (1000)        1 2023-06-29 14:18:54.000000 fnapy-1.4.1/fnapy.egg-info/zip-safe
+-rw-rw-r--   0 damien    (1000) damien    (1000)      398 2023-06-30 10:02:41.000000 fnapy-1.4.1/setup.cfg
+-rw-rw-r--   0 damien    (1000) damien    (1000)     1687 2023-05-29 09:36:13.000000 fnapy-1.4.1/setup.py
```

### Comparing `fnapy-1.4.0/LICENSE.txt` & `fnapy-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/PKG-INFO` & `fnapy-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnapy
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python API for FNAC WebServices
 Home-page: https://github.com/alexandriagroup/fnapy
 Author: Taurus Olson
 Author-email: taurusolson@gmail.com
 License: MIT
 Keywords: api,fnac,python,webservices
 Classifier: Development Status :: 4 - Beta
@@ -51,14 +51,20 @@
 Change log
 ==========
 
 All notable changes to this project will be documented in this file.
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
+[1.4.1] - 2023-06-30
+--------------------
+Fixed
+*****
+* `update_offers` and `query_offers` accept the parameter `time_to_ship`
+
 [1.4.0] - 2023-06-29
 --------------------
 Changed
 *******
 * Allow `update_offers` to accept more code types when passing a dictionary
 
 [1.3.0] - 2021-01-07
```

### Comparing `fnapy-1.4.0/README.rst` & `fnapy-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/docs/CHANGELOG.rst` & `fnapy-1.4.1/docs/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 Change log
 ==========
 
 All notable changes to this project will be documented in this file.
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
+[1.4.1] - 2023-06-30
+--------------------
+Fixed
+*****
+* `update_offers` and `query_offers` accept the parameter `time_to_ship`
+
 [1.4.0] - 2023-06-29
 --------------------
 Changed
 *******
 * Allow `update_offers` to accept more code types when passing a dictionary
 
 [1.3.0] - 2021-01-07
```

### Comparing `fnapy-1.4.0/docs/Makefile` & `fnapy-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/docs/api.rst` & `fnapy-1.4.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/docs/conf.py` & `fnapy-1.4.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 # -- Project information -----------------------------------------------------
 
 project = u'fnapy'
 copyright = u'2019, Taurus Olson'
 author = u'Taurus Olson'
 
 # The short X.Y version
-version = u'1.4.0'
+version = u'1.4.1'
 # The full version, including alpha/beta/rc tags
-release = u'1.4.0'
+release = u'1.4.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `fnapy-1.4.0/docs/make.bat` & `fnapy-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/docs/quickstart.rst` & `fnapy-1.4.1/docs/quickstart.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     offer_data2 = {'product_reference':'5030917077418',
             'offer_reference':'B067-F0D-75E',
             'price':20, 'product_state':11, 'quantity':16, 
             'description': 'New product - 2-3 days shipping, from France'}
     offer_data3 = {'product_reference':{'value': '9780262510875', 'type': 'Ean'},
             'offer_reference':'B76A-CD5-444',
             'price':80.0, 'product_state':11, 'quantity':10,
-            'description': 'New product - 2-3 days shipping, from France'}
+            'description': 'New product - 2-3 days shipping, from France', 'time_to_ship': 5}
     offer_data4 = {'product_reference': {'value': '1593275919', 'type': 'Isbn'},
         'offer_reference': 'A31F-B6C-95F',
         'price': 30.0, 'product_state': 11, 'quantity': 1,
         'description': 'New product - 2-3 days shipping, from France'
     }
 
     response = manager.update_offers([offers_data1, offer_data2, offer_data3, offer_data4])
@@ -80,14 +80,15 @@
       <offer>
         <product_reference type="Ean">9780262510875</product_reference>
         <offer_reference type="SellerSku"><![CDATA[B76A-CD5-444]]></offer_reference>
         <price>80.0</price>
         <product_state>11</product_state>
         <quantity>10</quantity>
         <description><![CDATA[New product - 2-3 days shipping, from France]]></description>
+        <time_to_ship>5</time_to_ship>
       </offer>
       <offer>
         <product_reference type="Isbn">1593275919</product_reference>
         <offer_reference type="SellerSku"><![CDATA[A31F-B6C-95F]]></offer_reference>
         <price>30.0</price>
         <product_state>11</product_state>
         <quantity>1</quantity>
```

### Comparing `fnapy-1.4.0/fnapy/compat.py` & `fnapy-1.4.1/fnapy/compat.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/fnapy/config.py` & `fnapy-1.4.1/fnapy/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 client_order_comment_id = Parameter(
     "client_order_comment_id", "Order unique identifier filter from fnac"
 )
 
 product_reference = Parameter("product_reference", "Product referenc")
 offer_reference = Parameter("offer_reference", "Offer reference")
 price = Parameter("price", "Offer price")
+time_to_ship = Parameter("time_to_ship", "Add a specific time to ship (if is activate)")
 product_state = Parameter("product_state", "Product state of offer")
 description = Parameter("description", "Product description")
 internal_comment = Parameter(
     "internal_comment", "Offer internal comment for personal use"
 )
 showcase = Parameter("showcase", "Offer position in shop’s showcase")
 treatment = Parameter("treatment", "Treatment to do on offer")
@@ -136,26 +137,28 @@
 REQUEST_ELEMENTS["offers_query"] = (
     paging,
     date,
     quantity,
     product_fnac_id,
     offer_fnac_id,
     offer_seller_id,
+    time_to_ship,
 )
 REQUEST_ELEMENTS["offers_update"] = (
     product_reference,
     offer_reference,
     price,
     product_state,
     quantity.change_desc("Offer quantity"),
     description,
     internal_comment,
     showcase,
     treatment,
     pictures,
+    time_to_ship,
 )
 REQUEST_ELEMENTS["orders_query"] = (
     paging,
     date,
     sort_by,
     product_fnac_id,
     offer_fnac_id,
```

### Comparing `fnapy-1.4.0/fnapy/connection.py` & `fnapy-1.4.1/fnapy/connection.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/fnapy/exceptions.py` & `fnapy-1.4.1/fnapy/exceptions.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/fnapy/fnapy_manager.py` & `fnapy-1.4.1/fnapy/fnapy_manager.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/fnapy/utils.py` & `fnapy-1.4.1/fnapy/utils.py`

 * *Files identical despite different names*

### Comparing `fnapy-1.4.0/fnapy.egg-info/PKG-INFO` & `fnapy-1.4.1/fnapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnapy
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python API for FNAC WebServices
 Home-page: https://github.com/alexandriagroup/fnapy
 Author: Taurus Olson
 Author-email: taurusolson@gmail.com
 License: MIT
 Keywords: api,fnac,python,webservices
 Classifier: Development Status :: 4 - Beta
@@ -51,14 +51,20 @@
 Change log
 ==========
 
 All notable changes to this project will be documented in this file.
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
+[1.4.1] - 2023-06-30
+--------------------
+Fixed
+*****
+* `update_offers` and `query_offers` accept the parameter `time_to_ship`
+
 [1.4.0] - 2023-06-29
 --------------------
 Changed
 *******
 * Allow `update_offers` to accept more code types when passing a dictionary
 
 [1.3.0] - 2021-01-07
```

### Comparing `fnapy-1.4.0/setup.py` & `fnapy-1.4.1/setup.py`

 * *Files identical despite different names*

