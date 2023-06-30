# Comparing `tmp/dea-tools-0.2.8.dev96.tar.gz` & `tmp/dea-tools-0.2.8.dev97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dea-tools-0.2.8.dev96.tar", last modified: Mon May 22 00:06:13 2023, max compression
+gzip compressed data, was "dea-tools-0.2.8.dev97.tar", last modified: Mon May 22 04:23:59 2023, max compression
```

## Comparing `dea-tools-0.2.8.dev96.tar` & `dea-tools-0.2.8.dev97.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:06:13.003174 dea-tools-0.2.8.dev96/dea_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/dea_tools/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32250 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/miningrehab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/bom.py
--rw-r--r--   0 runner    (1001) docker     (123)    62213 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)    60087 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    52113 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (123)    39758 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/landcover.py
--rw-r--r--   0 runner    (1001) docker     (123)    37726 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/pyfes_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/dea_tools/waterbodies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/dea_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-22 00:06:11.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 00:06:12.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:06:11.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 00:06:11.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 00:06:11.000000 dea-tools-0.2.8.dev96/dea_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:06:13.007174 dea-tools-0.2.8.dev96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-22 00:03:00.000000 dea-tools-0.2.8.dev96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:23:59.864842 dea-tools-0.2.8.dev97/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-22 04:23:59.864842 dea-tools-0.2.8.dev97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:23:59.864842 dea-tools-0.2.8.dev97/dea_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:23:59.864842 dea-tools-0.2.8.dev97/dea_tools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32250 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/app/animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/app/changefilmstrips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/app/crophealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/app/deacoastlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/app/imageexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/app/miningrehab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/app/widgetconstructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/bandindices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/bom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62213 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60087 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/coastal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52113 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/datahandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39758 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/landcover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37726 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/pyfes_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/dea_tools/waterbodies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:23:59.864842 dea-tools-0.2.8.dev97/dea_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-22 04:23:58.000000 dea-tools-0.2.8.dev97/dea_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 04:23:59.000000 dea-tools-0.2.8.dev97/dea_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:23:58.000000 dea-tools-0.2.8.dev97/dea_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 04:23:58.000000 dea-tools-0.2.8.dev97/dea_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 04:23:58.000000 dea-tools-0.2.8.dev97/dea_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 04:23:59.864842 dea-tools-0.2.8.dev97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-22 04:21:40.000000 dea-tools-0.2.8.dev97/setup.py
```

### Comparing `dea-tools-0.2.8.dev96/LICENSE` & `dea-tools-0.2.8.dev97/LICENSE`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/PKG-INFO` & `dea-tools-0.2.8.dev97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev96
+Version: 0.2.8.dev97
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: earth.observation@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.2.8.dev96/README.rst` & `dea-tools-0.2.8.dev97/README.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/app/animations.py` & `dea-tools-0.2.8.dev97/dea_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/app/changefilmstrips.py` & `dea-tools-0.2.8.dev97/dea_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/app/crophealth.py` & `dea-tools-0.2.8.dev97/dea_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/app/deacoastlines.py` & `dea-tools-0.2.8.dev97/dea_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/app/imageexport.py` & `dea-tools-0.2.8.dev97/dea_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/app/miningrehab.py` & `dea-tools-0.2.8.dev97/dea_tools/app/miningrehab.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/app/widgetconstructors.py` & `dea-tools-0.2.8.dev97/dea_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/bandindices.py` & `dea-tools-0.2.8.dev97/dea_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/bom.py` & `dea-tools-0.2.8.dev97/dea_tools/bom.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/classification.py` & `dea-tools-0.2.8.dev97/dea_tools/classification.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/climate.py` & `dea-tools-0.2.8.dev97/dea_tools/climate.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/coastal.py` & `dea-tools-0.2.8.dev97/dea_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/dask.py` & `dea-tools-0.2.8.dev97/dea_tools/dask.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/datahandling.py` & `dea-tools-0.2.8.dev97/dea_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/landcover.py` & `dea-tools-0.2.8.dev97/dea_tools/landcover.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/plotting.py` & `dea-tools-0.2.8.dev97/dea_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/pyfes_model.py` & `dea-tools-0.2.8.dev97/dea_tools/pyfes_model.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/spatial.py` & `dea-tools-0.2.8.dev97/dea_tools/spatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # Import required packages
 import dask
 import fiona
 import warnings
 import collections
 import odc.geo.xr
 import numpy as np
+import pandas as pd
 import xarray as xr
 import geopandas as gpd
 import rasterio.features
 import scipy.interpolate
 import multiprocessing as mp
 from scipy import ndimage as nd
 from skimage.measure import label
@@ -295,14 +296,15 @@
     da,
     z_values=[0.0],
     crs=None,
     attribute_df=None,
     output_path=None,
     min_vertices=2,
     dim="time",
+    time_format="%Y-%m-%d",
     errors="ignore",
     verbose=True,
 ):
     """
     Uses `skimage.measure.find_contours` to extract multiple z-value
     contour lines from a two-dimensional array (e.g. multiple elevations
     from a single DEM), or one z-value for each array along a specified
@@ -311,15 +313,15 @@
     timestep in an xarray timeseries).
 
     Contours are returned as a geopandas.GeoDataFrame with one row per
     z-value or one row per array along a specified dimension. The
     `attribute_df` parameter can be used to pass custom attributes
     to the output contour features.
 
-    Last modified: November 2022
+    Last modified: May 2023
 
     Parameters
     ----------
     da : xarray DataArray
         A two-dimensional or multi-dimensional array from which
         contours are extracted. If a two-dimensional array is provided,
         the analysis will run in 'single array, multiple z-values' mode
@@ -352,14 +354,18 @@
         and end point). Higher values remove smaller contours,
         potentially removing noise from the output dataset.
     dim : string, optional
         The name of the dimension along which to extract contours when
         operating in 'single z-value, multiple arrays' mode. The default
         is 'time', which extracts contours for each array along the time
         dimension.
+    time_format : string, optional
+        The format used to convert `numpy.datetime64` values to strings
+        if applied to data with a "time" dimension. Defaults to
+        "%Y-%m-%d".
     errors : string, optional
         If 'raise', then any failed contours will raise an exception.
         If 'ignore' (the default), a list of failed contours will be
         printed. If no contours are returned, an exception will always
         be raised.
     verbose : bool, optional
         Print debugging messages. Default is True.
@@ -383,14 +389,16 @@
         with less than X vertices.
         """
 
         # Extracts contours from array, and converts each discrete
         # contour into a Shapely LineString feature. If the function
         # returns a KeyError, this may be due to an unresolved issue in
         # scikit-image: https://github.com/scikit-image/scikit-image/issues/4830
+        # A temporary workaround is to peturb the z-value by a tiny
+        # amount (1e-12) before using it to extract the contour.
         try:
             line_features = [
                 LineString(i[:, [1, 0]])
                 for i in find_contours(da_i.data, z_value)
                 if i.shape[0] >= min_vertices
             ]
         except KeyError:
@@ -398,21 +406,33 @@
                 LineString(i[:, [1, 0]])
                 for i in find_contours(da_i.data, z_value + 1e-12)
                 if i.shape[0] >= min_vertices
             ]
 
         # Output resulting lines into a single combined MultiLineString
         return MultiLineString(line_features)
-    
+
+    def _time_format(i, time_format):
+        """
+        Converts numpy.datetime64 into formatted strings;
+        otherwise returns data as-is.
+        """
+        if isinstance(i, np.datetime64):
+            ts = pd.to_datetime(str(i))
+            i = ts.strftime(time_format)
+        return i
+
     # Verify input data is a xr.DataArray
     if not isinstance(da, xr.DataArray):
-        raise ValueError("The input `da` is not an xarray.DataArray. "
-                         "If you supplied an xarray.Dataset, pass in one "
-                         "of its data variables using the syntax "
-                         "`da=ds.<variable name>`.")
+        raise ValueError(
+            "The input `da` is not an xarray.DataArray. "
+            "If you supplied an xarray.Dataset, pass in one "
+            "of its data variables using the syntax "
+            "`da=ds.<variable name>`."
+        )
 
     # Add GeoBox and odc.* accessor to array using `odc-geo`
     da = add_geobox(da, crs)
 
     # If z_values is supplied is not a list, convert to list:
     z_values = (
         z_values
@@ -428,38 +448,41 @@
 
     # Test number of dimensions in supplied data array
     if len(da.shape) == 2:
         if verbose:
             print(f"Operating in multiple z-value, single array mode")
         dim = "z_value"
         contour_arrays = {
-            str(i)[0:10]: _contours_to_multiline(da, i, min_vertices) for i in z_values
+            _time_format(i, time_format): _contours_to_multiline(da, i, min_vertices)
+            for i in z_values
         }
 
     else:
         # Test if only a single z-value is given when operating in
         # single z-value, multiple arrays mode
         if verbose:
             print(f"Operating in single z-value, multiple arrays mode")
         if len(z_values) > 1:
             raise ValueError(
                 "Please provide a single z-value when operating "
                 "in single z-value, multiple arrays mode"
             )
 
         contour_arrays = {
-            str(i)[0:10]: _contours_to_multiline(da_i, z_values[0], min_vertices)
+            _time_format(i, time_format): _contours_to_multiline(
+                da_i, z_values[0], min_vertices
+            )
             for i, da_i in da.groupby(dim)
         }
 
     # If attributes are provided, add the contour keys to that dataframe
     if attribute_df is not None:
         try:
             attribute_df.insert(0, dim, contour_arrays.keys())
-            
+
         # If this fails, it is due to the applied attribute table not
         # matching the structure of the loaded data
         except ValueError:
             if len(da.shape) == 2:
                 raise ValueError(
                     f"The provided `attribute_df` contains a different "
                     f"number of rows ({len(attribute_df.index)}) "
@@ -522,15 +545,16 @@
             )
     elif empty_contours.any() and errors == "raise":
         raise Exception(f"Failed to generate contours: {failed}")
     elif empty_contours.any() and errors == "ignore":
         if verbose:
             print(f"Failed to generate contours: {failed}")
 
-    # If asked to write out file, test if geojson or shapefile
+    # If asked to write out file, test if GeoJSON or ESRI Shapefile. If
+    # GeoJSON, convert to EPSG:4326 before exporting.
     if output_path and output_path.endswith(".geojson"):
         if verbose:
             print(f"Writing contours to {output_path}")
         contours_gdf.to_crs("EPSG:4326").to_file(filename=output_path)
 
     if output_path and output_path.endswith(".shp"):
         if verbose:
```

### Comparing `dea-tools-0.2.8.dev96/dea_tools/temporal.py` & `dea-tools-0.2.8.dev97/dea_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/validation.py` & `dea-tools-0.2.8.dev97/dea_tools/validation.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools/waterbodies.py` & `dea-tools-0.2.8.dev97/dea_tools/waterbodies.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/dea_tools.egg-info/PKG-INFO` & `dea-tools-0.2.8.dev97/dea_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev96
+Version: 0.2.8.dev97
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: earth.observation@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.2.8.dev96/dea_tools.egg-info/SOURCES.txt` & `dea-tools-0.2.8.dev97/dea_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/index.rst` & `dea-tools-0.2.8.dev97/index.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev96/setup.py` & `dea-tools-0.2.8.dev97/setup.py`

 * *Files identical despite different names*

