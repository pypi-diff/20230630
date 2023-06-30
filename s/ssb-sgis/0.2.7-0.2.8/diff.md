# Comparing `tmp/ssb_sgis-0.2.7.tar.gz` & `tmp/ssb_sgis-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.2.7.tar", max compression
+gzip compressed data, was "ssb_sgis-0.2.8.tar", max compression
```

## Comparing `ssb_sgis-0.2.7.tar` & `ssb_sgis-0.2.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1074 2023-06-21 06:43:58.051659 ssb_sgis-0.2.7/LICENSE
--rw-r--r--   0        0        0     7543 2023-06-21 06:43:58.051659 ssb_sgis-0.2.7/README.md
--rw-r--r--   0        0        0     2539 2023-06-21 06:44:22.819867 ssb_sgis-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2368 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/dapla.py
--rw-r--r--   0        0        0      576 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8080 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    17659 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5870 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    14520 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    11862 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6888 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    22646 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     9887 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/geopandas_tools/to_geodataframe.py
--rw-r--r--   0        0        0     2674 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0     6479 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/examine.py
--rw-r--r--   0        0        0    23631 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1923 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20499 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    18611 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/map.py
--rw-r--r--   0        0        0    15961 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6218 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2017 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4487 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    12433 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    12369 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0     9375 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3359 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    66761 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12643 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6767 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0        0 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/py.typed
--rw-r--r--   0        0        0     3774 2023-06-21 06:43:58.087659 ssb_sgis-0.2.7/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-30 09:31:18.003938 ssb_sgis-0.2.8/LICENSE
+-rw-r--r--   0        0        0     7543 2023-06-30 09:31:18.003938 ssb_sgis-0.2.8/README.md
+-rw-r--r--   0        0        0     2539 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2445 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/dapla.py
+-rw-r--r--   0        0        0      576 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8780 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    17930 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5870 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    14520 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    11862 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6888 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    22635 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0    12458 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/geopandas_tools/to_geodataframe.py
+-rw-r--r--   0        0        0     2669 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0     6479 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/examine.py
+-rw-r--r--   0        0        0    25138 2023-06-30 09:31:34.076245 ssb_sgis-0.2.8/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1923 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20499 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    18611 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    15961 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6218 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12433 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    12369 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0     9375 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3359 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    66761 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12643 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6767 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/py.typed
+-rw-r--r--   0        0        0     3774 2023-06-30 09:31:18.035939 ssb_sgis-0.2.8/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.8/PKG-INFO
```

### Comparing `ssb_sgis-0.2.7/LICENSE` & `ssb_sgis-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/README.md` & `ssb_sgis-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/pyproject.toml` & `ssb_sgis-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.2.7"
+version = "0.2.8"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
```

### Comparing `ssb_sgis-0.2.7/src/sgis/__init__.py` & `ssb_sgis-0.2.8/src/sgis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # flake8: noqa: F401
 from .geopandas_tools.buffer_dissolve_explode import (
     buff,
     buffdiss,
     buffdissexp,
+    buffdissexp_by_cluster,
     dissexp,
+    dissexp_by_cluster,
 )
 from .geopandas_tools.general import (
     bounds_to_points,
     bounds_to_polygon,
     clean_clip,
     clean_geoms,
     coordinate_array,
@@ -19,14 +21,15 @@
     random_points,
     rename_geometry_if,
     to_lines,
 )
 from .geopandas_tools.geometry_types import (
     get_geom_type,
     is_single_geom_type,
+    make_all_singlepart,
     to_single_geom_type,
 )
 from .geopandas_tools.neighbors import (
     get_all_distances,
     get_k_nearest_neighbors,
     get_neighbor_indices,
     k_nearest_neighbors,
```

### Comparing `ssb_sgis-0.2.7/src/sgis/dapla.py` & `ssb_sgis-0.2.8/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/exceptions.py` & `ssb_sgis-0.2.8/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.2.8/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 - The buff function returns a GeoDataFrame, the geopandas method returns a GeoSeries.
 """
 
 from geopandas import GeoDataFrame, GeoSeries
 
 from .geometry_types import make_all_singlepart
+from .polygon_operations import get_polygon_clusters
 
 
 def _decide_ignore_index(kwargs: dict) -> tuple[dict, bool]:
     if "ignore_index" in kwargs:
         return kwargs, kwargs.pop("ignore_index")
 
     if not kwargs.get("by", None):
@@ -186,14 +187,39 @@
     dissolved[geom_col] = dissolved.make_valid()
 
     return make_all_singlepart(
         dissolved, ignore_index=ignore_index, index_parts=index_parts
     )
 
 
+def dissexp_by_cluster(gdf: GeoDataFrame) -> GeoDataFrame:
+    return (
+        gdf.explode(ignore_index=True)
+        .pipe(get_polygon_clusters, cluster_col="cluster")
+        .pipe(dissexp, by="cluster")
+        .reset_index(drop=True)
+    )
+
+
+def buffdissexp_by_cluster(
+    gdf: GeoDataFrame,
+    distance: int | float,
+    *,
+    resolution: int = 50,
+    copy: bool = True,
+) -> GeoDataFrame:
+    return (
+        buff(gdf, distance, resolution=resolution, copy=copy)
+        .explode(ignore_index=True)
+        .pipe(get_polygon_clusters, cluster_col="cluster")
+        .pipe(dissexp, by="cluster")
+        .reset_index(drop=True)
+    )
+
+
 def buff(
     gdf: GeoDataFrame | GeoSeries,
     distance: int | float,
     resolution: int = 50,
     copy: bool = True,
     **buffer_kwargs,
 ) -> GeoDataFrame:
```

### Comparing `ssb_sgis-0.2.7/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.2.8/src/sgis/geopandas_tools/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 
 import geopandas as gpd
 import numpy as np
+import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 from geopandas.array import GeometryDtype
 from shapely import (
     Geometry,
     box,
     extract_unique_points,
     get_exterior_ring,
@@ -515,19 +516,25 @@
         gdf = to_single_geom_type(gdf, "line")
 
         lines.append(gdf)
 
     if len(lines) == 1:
         return lines[0]
 
-    unioned = lines[0].overlay(lines[1], how="union", keep_geom_type=True)
+    if len(lines[0]) and len(lines[1]):
+        unioned = lines[0].overlay(lines[1], how="union", keep_geom_type=True)
+    else:
+        unioned = pd.concat([lines[0], lines[1]], ignore_index=True)
 
     if len(lines) > 2:
         for line_gdf in lines[2:]:
-            unioned = unioned.overlay(line_gdf, how="union", keep_geom_type=True)
+            if len(line_gdf):
+                unioned = unioned.overlay(line_gdf, how="union", keep_geom_type=True)
+            else:
+                unioned = pd.concat([unioned, line_gdf], ignore_index=True)
 
     return make_all_singlepart(unioned, ignore_index=True)
 
 
 def clean_clip(
     gdf: GeoDataFrame | GeoSeries,
     mask: GeoDataFrame | GeoSeries | Geometry,
```

### Comparing `ssb_sgis-0.2.7/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.2.8/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.2.8/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.2.8/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.2.8/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.2.8/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,155 @@
 from shapely.ops import unary_union
 
 from .general import _push_geom_col, to_lines
 from .neighbors import get_neighbor_indices
 from .overlay import clean_overlay
 
 
+def get_polygon_clusters(
+    *gdfs: GeoDataFrame | GeoSeries,
+    cluster_col: str = "cluster",
+    allow_multipart: bool = False,
+) -> GeoDataFrame | tuple[GeoDataFrame]:
+    """Find which polygons overlap without dissolving.
+
+    Devides polygons into clusters in a fast and precice manner by using spatial join
+    and networkx to find the connected components, i.e. overlapping geometries.
+    If multiple GeoDataFrames are given, the clusters will be based on all
+    combined.
+
+    This can be used instead of dissolve+explode, or before dissolving by the cluster
+    column. This has been tested to be a lot faster if there are many
+    non-overlapping polygons, but somewhat slower than dissolve+explode if most
+    polygons overlap.
+
+    Args:
+        gdfs: One or more GeoDataFrames of polygons.
+        cluster_col: Name of the resulting cluster column.
+        allow_multipart: Whether to allow mutipart geometries in the gdfs.
+            Defaults to False to avoid confusing results.
+
+    Returns:
+        One or more GeoDataFrames (same amount as was given) with a new cluster column.
+
+    Examples
+    --------
+
+    Create geometries with three clusters of overlapping polygons.
+
+    >>> import sgis as sg
+    >>> gdf = sg.to_gdf([(0, 0), (1, 1), (0, 1), (4, 4), (4, 3), (7, 7)])
+    >>> buffered = sg.buff(gdf, 1)
+    >>> gdf
+                                                geometry
+    0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
+    1  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
+    2  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
+    3  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
+    4  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
+    5  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
+
+    Add a cluster column to the GeoDataFrame:
+
+    >>> gdf = sg.get_polygon_clusters(gdf, cluster_col="cluster")
+    >>> gdf
+       cluster                                           geometry
+    0        0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
+    1        0  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
+    2        0  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
+    3        1  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
+    4        1  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
+    5        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
+
+    If multiple GeoDataFrames are given, all are returned with common
+    cluster values.
+
+    >>> gdf2 = sg.to_gdf([(0, 0), (7, 7)])
+    >>> gdf, gdf2 = sg.get_polygon_clusters(gdf, gdf2, cluster_col="cluster")
+    >>> gdf2
+       cluster                 geometry
+    0        0  POINT (0.00000 0.00000)
+    1        2  POINT (7.00000 7.00000)
+    >>> gdf
+       cluster                                           geometry
+    0        0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
+    1        0  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
+    2        0  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
+    3        1  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
+    4        1  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
+    5        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
+
+    Dissolving 'by' the cluster column will make the dissolve much
+    faster if there are a lot of non-overlapping polygons.
+
+    >>> dissolved = gdf.dissolve(by="cluster", as_index=False)
+    >>> dissolved
+       cluster                                           geometry
+    0        0  POLYGON ((0.99951 -0.03141, 0.99803 -0.06279, ...
+    1        1  POLYGON ((4.99951 2.96859, 4.99803 2.93721, 4....
+    2        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
+    """
+    if isinstance(gdfs[-1], str):
+        *gdfs, cluster_col = gdfs
+
+    concated = pd.DataFrame()
+    orig_indices = ()
+    for i, gdf in enumerate(gdfs):
+        if isinstance(gdf, GeoSeries):
+            gdf = gdf.to_frame()
+
+        if not isinstance(gdf, GeoDataFrame):
+            raise TypeError("'gdfs' should be GeoDataFrames or GeoSeries.")
+
+        if not allow_multipart and len(gdf) != len(gdf.explode(index_parts=False)):
+            raise ValueError(
+                "All geometries should be exploded to singlepart "
+                "in order to get correct polygon clusters. "
+                "To allow multipart geometries, set allow_multipart=True"
+            )
+
+        orig_indices = orig_indices + (gdf.index,)
+
+        gdf["i__"] = i
+
+        concated = pd.concat([concated, gdf], ignore_index=True)
+
+    neighbors = get_neighbor_indices(concated, concated)
+
+    edges = [(source, target) for source, target in neighbors.items()]
+
+    graph = nx.Graph()
+    graph.add_edges_from(edges)
+
+    component_mapper = {
+        j: i
+        for i, component in enumerate(nx.connected_components(graph))
+        for j in component
+    }
+
+    concated[cluster_col] = component_mapper
+
+    concated = _push_geom_col(concated)
+
+    n_gdfs = concated["i__"].unique()
+
+    if len(n_gdfs) == 1:
+        concated.index = orig_indices[0]
+        return concated.drop(["i__"], axis=1)
+
+    unconcated = ()
+    for i in n_gdfs:
+        gdf = concated[concated["i__"] == i]
+        gdf.index = orig_indices[i]
+        gdf = gdf.drop(["i__"], axis=1)
+        unconcated = unconcated + (gdf,)
+
+    return unconcated
+
+
 def eliminate_by_longest(
     gdf: GeoDataFrame,
     to_eliminate: GeoDataFrame,
     *,
     remove_isolated: bool = False,
     ignore_index: bool = False,
     aggfunc: str | dict | list = "first",
@@ -211,154 +352,14 @@
     if not remove_isolated:
         isolated = joined.loc[joined["index_right"].isna()]
         eliminated = pd.concat([eliminated, isolated])
 
     return eliminated
 
 
-def get_polygon_clusters(
-    *gdfs: GeoDataFrame | GeoSeries,
-    cluster_col: str = "cluster",
-    allow_multipart: bool = False,
-) -> GeoDataFrame | tuple[GeoDataFrame]:
-    """Find which polygons overlap without dissolving.
-
-    Devides polygons into clusters in a fast and precice manner by using spatial join
-    and networkx to find the connected components, i.e. overlapping geometries.
-    If multiple GeoDataFrames are given, the clusters will be based on all
-    combined.
-
-    This can be used instead of dissolve+explode, or before dissolving by the cluster
-    column. This has been tested to be a lot faster if there are many
-    non-overlapping polygons, but somewhat slower than dissolve+explode if most
-    polygons overlap.
-
-    Args:
-        gdfs: One or more GeoDataFrames of polygons.
-        cluster_col: Name of the resulting cluster column.
-        allow_multipart: Whether to allow mutipart geometries in the gdfs.
-            Defaults to False to avoid confusing results.
-
-    Returns:
-        One or more GeoDataFrames (same amount as was given) with a new cluster column.
-
-    Examples
-    --------
-
-    Create geometries with three clusters of overlapping polygons.
-
-    >>> import sgis as sg
-    >>> gdf = sg.to_gdf([(0, 0), (1, 1), (0, 1), (4, 4), (4, 3), (7, 7)])
-    >>> buffered = sg.buff(gdf, 1)
-    >>> gdf
-                                                geometry
-    0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
-    1  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
-    2  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
-    3  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
-    4  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
-    5  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
-
-    Add a cluster column to the GeoDataFrame:
-
-    >>> gdf = sg.get_polygon_clusters(gdf, cluster_col="cluster")
-    >>> gdf
-       cluster                                           geometry
-    0        0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
-    1        0  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
-    2        0  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
-    3        1  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
-    4        1  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
-    5        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
-
-    If multiple GeoDataFrames are given, all are returned with common
-    cluster values.
-
-    >>> gdf2 = sg.to_gdf([(0, 0), (7, 7)])
-    >>> gdf, gdf2 = sg.get_polygon_clusters(gdf, gdf2, cluster_col="cluster")
-    >>> gdf2
-       cluster                 geometry
-    0        0  POINT (0.00000 0.00000)
-    1        2  POINT (7.00000 7.00000)
-    >>> gdf
-       cluster                                           geometry
-    0        0  POLYGON ((1.00000 0.00000, 0.99951 -0.03141, 0...
-    1        0  POLYGON ((2.00000 1.00000, 1.99951 0.96859, 1....
-    2        0  POLYGON ((1.00000 1.00000, 0.99951 0.96859, 0....
-    3        1  POLYGON ((5.00000 4.00000, 4.99951 3.96859, 4....
-    4        1  POLYGON ((5.00000 3.00000, 4.99951 2.96859, 4....
-    5        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
-
-    Dissolving 'by' the cluster column will make the dissolve much
-    faster if there are a lot of non-overlapping polygons.
-
-    >>> dissolved = gdf.dissolve(by="cluster", as_index=False)
-    >>> dissolved
-       cluster                                           geometry
-    0        0  POLYGON ((0.99951 -0.03141, 0.99803 -0.06279, ...
-    1        1  POLYGON ((4.99951 2.96859, 4.99803 2.93721, 4....
-    2        2  POLYGON ((8.00000 7.00000, 7.99951 6.96859, 7....
-    """
-    if isinstance(gdfs[-1], str):
-        *gdfs, cluster_col = gdfs
-
-    concated = pd.DataFrame()
-    orig_indices = ()
-    for i, gdf in enumerate(gdfs):
-        if isinstance(gdf, GeoSeries):
-            gdf = gdf.to_frame()
-
-        if not isinstance(gdf, GeoDataFrame):
-            raise TypeError("'gdfs' should be one or more GeoDataFrames or GeoSeries.")
-
-        if not allow_multipart and len(gdf) != len(gdf.explode(index_parts=False)):
-            raise ValueError(
-                "All geometries should be exploded to singlepart "
-                "in order to get correct polygon clusters. "
-                "To allow multipart geometries, set allow_multipart=True"
-            )
-
-        orig_indices = orig_indices + (gdf.index,)
-        gdf["i__"] = i
-
-        concated = pd.concat([concated, gdf], ignore_index=True)
-
-    neighbors = get_neighbor_indices(concated, concated)
-
-    edges = [(source, target) for source, target in neighbors.items()]
-
-    graph = nx.Graph()
-    graph.add_edges_from(edges)
-
-    component_mapper = {
-        j: i
-        for i, component in enumerate(nx.connected_components(graph))
-        for j in component
-    }
-
-    concated[cluster_col] = component_mapper
-
-    concated = _push_geom_col(concated)
-
-    n_gdfs = concated["i__"].unique()
-
-    if len(n_gdfs) == 1:
-        concated.index = orig_indices[0]
-        return concated.drop(["i__"], axis=1)
-
-    unconcated = ()
-    for i in n_gdfs:
-        gdf = concated[concated["i__"] == i]
-        gdf.index = orig_indices[i]
-        gdf = gdf.drop(["i__"], axis=1)
-        unconcated = unconcated + (gdf,)
-
-    return unconcated
-
-
 def get_overlapping_polygons(
     gdf: GeoDataFrame | GeoSeries, ignore_index: bool = False
 ) -> GeoDataFrame | GeoSeries:
     """Find the areas that overlap.
 
     Does an intersection with itself and keeps only the duplicated geometries. The
     index of 'gdf' is preserved.
```

### Comparing `ssb_sgis-0.2.7/src/sgis/geopandas_tools/to_geodataframe.py` & `ssb_sgis-0.2.8/src/sgis/geopandas_tools/to_geodataframe.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numbers
 from collections.abc import Iterator, Sized
 
 import geopandas as gpd
 import pandas as pd
+import shapely
 from geopandas import GeoDataFrame, GeoSeries
 from pandas.api.types import is_array_like, is_dict_like, is_list_like
 from shapely import Geometry, box, wkb, wkt
 from shapely.geometry import Point
 from shapely.ops import unary_union
 
 
@@ -124,15 +125,15 @@
     3   POINT Z (1.000 50.000 77.000)
     4  POINT Z (58.000 49.000 46.000)
     """
     if isinstance(geom, GeoDataFrame):
         raise TypeError("'to_gdf' doesn't accept GeoDataFrames as input type.")
 
     if isinstance(geom, GeoSeries):
-        geom_col = "geometry" if not geometry else geometry
+        geom_col = geometry if geometry else "geometry"
         return _geoseries_to_gdf(geom, geom_col, crs, **kwargs)
 
     geom_col = _find_geometry_column(geom, geometry)
     index = kwargs.get("index", None)
 
     if is_array_like(geom_col):
         geometry = GeoSeries((_make_one_shapely_geom(g) for g in geometry), index=index)
@@ -140,16 +141,34 @@
 
     # get done with the iterators that get consumed by 'all' statements
     if isinstance(geom, Iterator) and not isinstance(geom, Sized):
         geom = GeoSeries((_make_one_shapely_geom(g) for g in geom), index=index)
         return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
 
     if not is_dict_like(geom):
-        geom = GeoSeries(_make_shapely_geoms(geom), index=index)
-        return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
+        if not hasattr(geom, "__iter__") and hasattr(geom, "__dict__"):
+            if all(attr in geom.__dict__ for attr in ["minx", "miny", "maxx", "maxy"]):
+                geom = GeoSeries(
+                    shapely.box(*(geom.minx, geom.miny, geom.maxx, geom.maxy)),
+                    index=index,
+                )
+                return GeoDataFrame(
+                    {geom_col: geom}, geometry=geom_col, crs=crs, **kwargs
+                )
+        if hasattr(geom, "__iter__") and all(isinstance(g, dict) for g in geom):
+            crs = crs if crs else _get_crs(geom)
+            geom = pd.concat(GeoSeries(_from_json(g)) for g in geom)
+            if index is not None:
+                geom.index = index
+            else:
+                geom = geom.reset_index(drop=True)
+            return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
+        else:
+            geom = GeoSeries(_make_shapely_geoms(geom), index=index)
+            return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
 
     # now we have dict, Series or DataFrame
 
     geom = geom.copy()
 
     # preserve Series/DataFrame index, overrides kwargs for now
     index = geom.index if hasattr(geom, "index") else kwargs.get("index", None)
@@ -173,18 +192,69 @@
         else:
             geoseries = GeoSeries(_make_shapely_geoms(geom.iloc[:, 0]), index=index)
         return GeoDataFrame({key: geoseries}, geometry=key, crs=crs, **kwargs)
 
     if geometry and geom_col not in geom or isinstance(geom, pd.DataFrame):
         raise ValueError("Cannot find geometry column(s)", geometry)
 
+    # geojson, __geo_interface__
+    if (
+        isinstance(geom, dict)
+        and sum(key in geom for key in ["type", "coordinates", "features"]) >= 2
+    ):
+        if "geometry" in geom:
+            geometry = "geometry"
+
+        crs = crs if crs else _get_crs(geom)
+        print(crs)
+        geom = GeoSeries(_from_json(geom), index=index)
+        return GeoDataFrame({geom_col: geom}, geometry=geom_col, crs=crs, **kwargs)
+
     geoseries = _series_like_to_geoseries(geom, index=index)
     return GeoDataFrame(geometry=geoseries, crs=crs, **kwargs)
 
 
+def _get_crs(geom):
+    if not is_dict_like(geom) and is_dict_like(geom[0]):
+        crss = list({_get_crs(g) for g in geom})
+        if len(crss) == 1:
+            return crss[0]
+        return None
+    if "properties" in geom:
+        return _get_crs(geom["properties"])
+    if "crs" in geom:
+        geom = geom["crs"]
+        while is_dict_like(geom):
+            if "properties" in geom:
+                geom = geom["properties"]
+            elif "name" in geom:
+                geom = geom["name"]
+            else:
+                return None
+        return geom
+    return None
+
+
+def _from_json(geom: dict):
+    if not isinstance(geom, dict) and isinstance(geom[0], dict):
+        return [_from_json(g) for g in geom]
+    if "geometry" in geom:
+        return _from_json(geom["geometry"])
+    if "features" in geom:
+        return _from_json(geom["features"])
+    coords = geom["coordinates"]
+    constructor = eval("shapely.geometry." + geom.get("type", Point))
+    try:
+        return constructor(coords)
+    except TypeError:
+        while len(coords) == 1:
+            coords = coords[0]
+        return constructor(coords)
+
+
 def _series_like_to_geoseries(geom, index):
     if index is None:
         index = geom.keys()
     if isinstance(geom, dict):
         return GeoSeries(_make_shapely_geoms(list(geom.values())), index=index)
     else:
         return GeoSeries(_make_shapely_geoms(geom.values), index=index)
@@ -248,14 +318,16 @@
         return True
     return False
 
 
 def _make_shapely_geoms(geom):
     if _is_one_geometry(geom):
         return _make_one_shapely_geom(geom)
+    if isinstance(geom, dict) and "coordinates" in geom:
+        return _from_json(geom)
     return (_make_one_shapely_geom(g) for g in geom)
 
 
 def _make_one_shapely_geom(geom):
     """Create shapely geometry from wkt, wkb or coordinate tuple.
 
     Works recursively if the object is a nested iterable.
```

### Comparing `ssb_sgis-0.2.7/src/sgis/helpers.py` & `ssb_sgis-0.2.8/src/sgis/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 
 
 def get_name(var: object, n: int = 5) -> str | None:
     """Searches through the local variables down one level at a time."""
     frame = inspect.currentframe().f_back.f_back
 
     for _ in range(n):
-        locals_ = frame.f_locals
-
-        names = [var_name for var_name, var_val in locals_.items() if var_val is var]
+        names = [
+            var_name for var_name, var_val in frame.f_locals.items() if var_val is var
+        ]
         if names and len(names) == 1:
             return names[0]
 
         names = [name for name in names if not name.startswith("_")]
 
         if names and len(names) == 1:
             return names[0]
```

### Comparing `ssb_sgis-0.2.7/src/sgis/maps/examine.py` & `ssb_sgis-0.2.8/src/sgis/maps/examine.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/maps/explore.py` & `ssb_sgis-0.2.8/src/sgis/maps/explore.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Interactive map of one or more GeoDataFrames with layers that can be toggles on/off.
 
 This module holds the Explore class, which is the basis for the explore, samplemap and
 clipmap functions from the 'maps' module.
 """
 import warnings
+from numbers import Number
 from statistics import mean
 
 import branca as bc
 import folium
 import matplotlib
 import numpy as np
 import pandas as pd
 from folium import plugins
 from geopandas import GeoDataFrame
 from IPython.display import display
 from jinja2 import Template
+from shapely import Geometry
 from shapely.geometry import LineString
 
 from ..geopandas_tools.general import clean_geoms, make_all_singlepart
-from ..geopandas_tools.geometry_types import get_geom_type
+from ..geopandas_tools.geometry_types import get_geom_type, to_single_geom_type
 from ..geopandas_tools.to_geodataframe import to_gdf
 from ..helpers import unit_is_degrees
 from .httpserver import run_html_server
 from .map import Map
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
@@ -106,14 +108,25 @@
         if not self.browser and "show_in_browser" in kwargs:
             self.browser = kwargs.pop("show_in_browser")
         if not self.browser and "in_browser" in kwargs:
             self.browser = kwargs.pop("in_browser")
 
         super().__init__(*gdfs, column=column, **kwargs)
 
+        # remove columns not renerable by leaflet (list columns etc.)
+        new_gdfs = []
+        for gdf in self.gdfs:
+            cols_to_keep = [
+                col
+                for col in gdf.columns
+                if isinstance(gdf[col].iloc[0], (Number, str, Geometry))
+            ]
+            new_gdfs.append(gdf[cols_to_keep])
+        self._gdfs = new_gdfs
+
         self.popup = popup
         self.max_zoom = max_zoom
         self.smooth_factor = smooth_factor
         self.prefer_canvas = prefer_canvas
         self.measure_control = measure_control
         self.geocoder = geocoder
         self.save = save
@@ -262,14 +275,15 @@
         """Buffer gdf if mixed geometry types. Expode to singlepart.
 
         Because Folium does not handle mixed geometries well.
         """
 
         new_gdfs = []
         for gdf in self._gdfs:
+            print(gdf)
             if get_geom_type(gdf) == "mixed" and not unit_is_degrees(gdf):
                 gdf[gdf._geometry_column_name] = gdf.buffer(0.01)
             gdf = make_all_singlepart(gdf)
             new_gdfs.append(gdf)
         self._gdfs = new_gdfs
         self._gdf = pd.concat(new_gdfs, ignore_index=True)
         self._nan_idx = self._gdf[self._column].isna()
@@ -611,15 +625,34 @@
                 marker = folium.CircleMarker(**marker_kwds)
             else:
                 raise ValueError(
                     "Only 'marker', 'circle', and 'circle_marker' are "
                     "supported as marker values"
                 )
 
-        gdf = clean_geoms(gdf)
+        gdf = clean_geoms(gdf).pipe(make_all_singlepart)
+        if get_geom_type(gdf) == "mixed":
+            if gdf.geom_type.str.lower().str.contains("polygon").any():
+                warnings.warn(
+                    "GeoJsonTooltip is not configured to render for GeoJson "
+                    "GeometryCollection geometries. Keeping only polygons."
+                )
+                gdf = to_single_geom_type(gdf, geom_type="polygon")
+            elif gdf.geom_type.str.lower().str.contains("line").any():
+                warnings.warn(
+                    "GeoJsonTooltip is not configured to render for GeoJson "
+                    "GeometryCollection geometries. Keeping only lines."
+                )
+                gdf = to_single_geom_type(gdf, geom_type="line")
+            else:
+                warnings.warn(
+                    "GeoJsonTooltip is not configured to render for GeoJson "
+                    "GeometryCollection geometries. Keeping only points."
+                )
+                gdf = to_single_geom_type(gdf, geom_type="point")
 
         # prepare tooltip and popup
         if isinstance(gdf, GeoDataFrame):
             # add named index to the tooltip
             if gdf.index.name is not None:
                 gdf = gdf.reset_index()
             # specify fields to show in the tooltip
```

### Comparing `ssb_sgis-0.2.7/src/sgis/maps/httpserver.py` & `ssb_sgis-0.2.8/src/sgis/maps/httpserver.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/maps/legend.py` & `ssb_sgis-0.2.8/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/maps/map.py` & `ssb_sgis-0.2.8/src/sgis/maps/map.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/maps/maps.py` & `ssb_sgis-0.2.8/src/sgis/maps/maps.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.2.8/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/cutting_lines.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/networkanalysis.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-0.2.8/src/sgis/networkanalysis/nodes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/src/sgis/read_parquet.py` & `ssb_sgis-0.2.8/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.7/PKG-INFO` & `ssb_sgis-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.2.7
+Version: 0.2.8
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
```

