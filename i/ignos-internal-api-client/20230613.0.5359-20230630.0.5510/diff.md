# Comparing `tmp/ignos-internal-api-client-20230613.0.5359.tar.gz` & `tmp/ignos-internal-api-client-20230630.0.5510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignos-internal-api-client-20230613.0.5359.tar", last modified: Tue Jun 13 10:33:58 2023, max compression
+gzip compressed data, was "ignos-internal-api-client-20230630.0.5510.tar", last modified: Fri Jun 30 18:42:10 2023, max compression
```

## Comparing `ignos-internal-api-client-20230613.0.5359.tar` & `ignos-internal-api-client-20230630.0.5510.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/
--rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.843078 ignos-internal-api-client-20230613.0.5359/ignos/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.843078 ignos-internal-api-client-20230613.0.5359/ignos/internal/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.843078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.843078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/
--rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6182 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_patch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    78836 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_vendor.py
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.847078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/
--rw-r--r--   0 vsts      (1001) docker     (123)      823 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6358 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3009 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.847078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1503 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   102360 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.847078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/
--rw-r--r--   0 vsts      (1001) docker     (123)     2768 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (123)    59185 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1503 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   120947 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1256 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      982 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.171125 ignos-internal-api-client-20230630.0.5510/
+-rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-06-30 18:42:10.171125 ignos-internal-api-client-20230630.0.5510/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.163125 ignos-internal-api-client-20230630.0.5510/ignos/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.163125 ignos-internal-api-client-20230630.0.5510/ignos/internal/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.163125 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.167125 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/
+-rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6182 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    78836 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_vendor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.167125 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/
+-rw-r--r--   0 vsts      (1001) docker     (123)      823 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6358 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3009 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.167125 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1503 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   102360 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.167125 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2768 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    59535 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.167125 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1503 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   120947 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-30 18:42:10.171125 ignos-internal-api-client-20230630.0.5510/ignos_internal_api_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-06-30 18:42:10.000000 ignos-internal-api-client-20230630.0.5510/ignos_internal_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1256 2023-06-30 18:42:10.000000 ignos-internal-api-client-20230630.0.5510/ignos_internal_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-30 18:42:10.000000 ignos-internal-api-client-20230630.0.5510/ignos_internal_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-06-30 18:42:10.000000 ignos-internal-api-client-20230630.0.5510/ignos_internal_api_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-30 18:42:10.000000 ignos-internal-api-client-20230630.0.5510/ignos_internal_api_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-30 18:42:10.171125 ignos-internal-api-client-20230630.0.5510/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      982 2023-06-30 18:41:54.000000 ignos-internal-api-client-20230630.0.5510/setup.py
```

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/__init__.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_client.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_client.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_configuration.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_patch.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_serialization.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_serialization.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_vendor.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/_vendor.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/__init__.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_client.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/_client.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_configuration.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_patch.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/__init__.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/_operations.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/_patch.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/__init__.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_enums.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_models.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1010,43 +1010,55 @@
 
     :ivar asset_external_id: Required.
     :vartype asset_external_id: str
     :ivar asset_name: Required.
     :vartype asset_name: str
     :ivar factory_asset_external_id: Required.
     :vartype factory_asset_external_id: str
+    :ivar has_solar_panels:
+    :vartype has_solar_panels: bool
     """
 
     _validation = {
         "asset_external_id": {"required": True, "min_length": 1},
         "asset_name": {"required": True, "min_length": 1},
         "factory_asset_external_id": {"required": True, "min_length": 1},
     }
 
     _attribute_map = {
         "asset_external_id": {"key": "assetExternalId", "type": "str"},
         "asset_name": {"key": "assetName", "type": "str"},
         "factory_asset_external_id": {"key": "factoryAssetExternalId", "type": "str"},
+        "has_solar_panels": {"key": "hasSolarPanels", "type": "bool"},
     }
 
     def __init__(
-        self, *, asset_external_id: str, asset_name: str, factory_asset_external_id: str, **kwargs: Any
+        self,
+        *,
+        asset_external_id: str,
+        asset_name: str,
+        factory_asset_external_id: str,
+        has_solar_panels: Optional[bool] = None,
+        **kwargs: Any
     ) -> None:
         """
         :keyword asset_external_id: Required.
         :paramtype asset_external_id: str
         :keyword asset_name: Required.
         :paramtype asset_name: str
         :keyword factory_asset_external_id: Required.
         :paramtype factory_asset_external_id: str
+        :keyword has_solar_panels:
+        :paramtype has_solar_panels: bool
         """
         super().__init__(**kwargs)
         self.asset_external_id = asset_external_id
         self.asset_name = asset_name
         self.factory_asset_external_id = factory_asset_external_id
+        self.has_solar_panels = has_solar_panels
 
 
 class PowerRegionDto(_serialization.Model):
     """PowerRegionDto.
 
     :ivar id:
     :vartype id: str
```

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_patch.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/__init__.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/_operations.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/_patch.py` & `ignos-internal-api-client-20230630.0.5510/ignos/internal/api/client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/SOURCES.txt` & `ignos-internal-api-client-20230630.0.5510/ignos_internal_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230613.0.5359/setup.py` & `ignos-internal-api-client-20230630.0.5510/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 # coding: utf-8
 from setuptools import setup, find_packages
 
 
 PACKAGE_NAME = "ignos-internal-api-client"
-version = "20230613.0.5359"
+version = "20230630.0.5510"
 setup(
     name=PACKAGE_NAME,
     version=version,
     description="ignos-internal-api-client",
     author_email="",
     url="",
     keywords="azure, azure sdk",
```

