# Comparing `tmp/eodc-2023.6.8.tar.gz` & `tmp/eodc-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.8.tar", max compression
+gzip compressed data, was "eodc-2023.6.9.tar", max compression
```

## Comparing `eodc-2023.6.8.tar` & `eodc-2023.6.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-27 12:34:34.781284 eodc-2023.6.8/README.md
--rw-r--r--   0        0        0      213 2023-06-27 12:34:34.781284 eodc-2023.6.8/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-27 12:34:34.781284 eodc-2023.6.8/eodc/dask.py
--rw-r--r--   0        0        0    11579 2023-06-27 12:34:34.781284 eodc-2023.6.8/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-27 12:34:34.781284 eodc-2023.6.8/eodc/settings.py
--rw-r--r--   0        0        0     1207 2023-06-27 12:34:34.781284 eodc-2023.6.8/pyproject.toml
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 eodc-2023.6.8/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-29 11:54:54.077811 eodc-2023.6.9/README.md
+-rw-r--r--   0        0        0      213 2023-06-29 11:54:54.077811 eodc-2023.6.9/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-29 11:54:54.077811 eodc-2023.6.9/eodc/dask.py
+-rw-r--r--   0        0        0    11584 2023-06-29 11:54:54.077811 eodc-2023.6.9/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-29 11:54:54.077811 eodc-2023.6.9/eodc/settings.py
+-rw-r--r--   0        0        0     1207 2023-06-29 11:54:54.077811 eodc-2023.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 eodc-2023.6.9/PKG-INFO
```

### Comparing `eodc-2023.6.8/README.md` & `eodc-2023.6.9/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.8/eodc/dask.py` & `eodc-2023.6.9/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.8/eodc/faas.py` & `eodc-2023.6.9/eodc/faas.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         self, sen2like_parameters: Sen2LikeParameters, target_product: str = "L2F"
     ) -> list[Item]:
         from sen2like_processor_bindings.model import get_output_stac_item_paths
 
         stac_item_paths = get_output_stac_item_paths(
             sen2like_parameters, target_product=target_product
         )
-        stac_items = [Item.from_file(path) for path in stac_item_paths]
+        stac_items = [Item.from_file(str(path)) for path in stac_item_paths]
         return stac_items
 
 
 class OpenEO(FaasProcessorBase):
     @classmethod
     def get_instance(cls):
         return cls(processor_details=FaasProcessor.OpenEO.value)
```

### Comparing `eodc-2023.6.8/pyproject.toml` & `eodc-2023.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.8"
+version = "2023.6.9"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2023.6.8/PKG-INFO` & `eodc-2023.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.8
+Version: 2023.6.9
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

