# Comparing `tmp/fibsem_tools-4.0.2.tar.gz` & `tmp/fibsem_tools-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibsem_tools-4.0.2.tar", max compression
+gzip compressed data, was "fibsem_tools-4.0.3.tar", max compression
```

## Comparing `fibsem_tools-4.0.2.tar` & `fibsem_tools-4.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-02-21 23:22:56.299056 fibsem_tools-4.0.2/LICENSE
--rw-r--r--   0        0        0     1425 2023-05-05 14:06:24.893362 fibsem_tools-4.0.2/pyproject.toml
--rw-r--r--   0        0        0      183 2023-04-25 22:22:07.080776 fibsem_tools-4.0.2/src/fibsem_tools/__init__.py
--rw-r--r--   0        0        0      606 2023-04-02 16:17:29.203986 fibsem_tools-4.0.2/src/fibsem_tools/cli/tiff2zarr.css
--rw-r--r--   0        0        0    13481 2023-04-02 16:17:29.204298 fibsem_tools-4.0.2/src/fibsem_tools/cli/tiff2zarr.py
--rw-r--r--   0        0        0        0 2023-03-23 18:13:14.517927 fibsem_tools-4.0.2/src/fibsem_tools/io/__init__.py
--rw-r--r--   0        0        0     7473 2023-05-05 14:06:19.025368 fibsem_tools-4.0.2/src/fibsem_tools/io/core.py
--rw-r--r--   0        0        0    13817 2023-05-04 17:46:58.084105 fibsem_tools-4.0.2/src/fibsem_tools/io/dask.py
--rw-r--r--   0        0        0    31797 2023-05-04 18:29:01.063113 fibsem_tools-4.0.2/src/fibsem_tools/io/dat.py
--rw-r--r--   0        0        0     2258 2023-03-23 19:35:10.739676 fibsem_tools-4.0.2/src/fibsem_tools/io/h5.py
--rw-r--r--   0        0        0     5081 2023-05-04 18:29:01.063414 fibsem_tools-4.0.2/src/fibsem_tools/io/mrc.py
--rw-r--r--   0        0        0     6819 2023-05-04 18:29:01.063658 fibsem_tools-4.0.2/src/fibsem_tools/io/multiscale.py
--rw-r--r--   0        0        0       36 2023-03-23 19:35:10.687732 fibsem_tools-4.0.2/src/fibsem_tools/io/neuroglancer.py
--rw-r--r--   0        0        0     2341 2023-03-23 19:45:26.756642 fibsem_tools-4.0.2/src/fibsem_tools/io/server.py
--rw-r--r--   0        0        0      431 2023-05-04 18:29:01.063967 fibsem_tools-4.0.2/src/fibsem_tools/io/tif.py
--rw-r--r--   0        0        0     4340 2023-05-04 18:29:01.064387 fibsem_tools-4.0.2/src/fibsem_tools/io/util.py
--rw-r--r--   0        0        0     1504 2023-05-04 18:29:01.064928 fibsem_tools-4.0.2/src/fibsem_tools/io/xr.py
--rw-r--r--   0        0        0    15179 2023-05-04 18:29:01.065422 fibsem_tools-4.0.2/src/fibsem_tools/io/zarr.py
--rw-r--r--   0        0        0        0 2023-02-21 23:22:56.301100 fibsem_tools-4.0.2/src/fibsem_tools/metadata/__init__.py
--rw-r--r--   0        0        0     3195 2023-05-04 17:46:58.085649 fibsem_tools-4.0.2/src/fibsem_tools/metadata/cosem.py
--rw-r--r--   0        0        0     3479 2023-05-04 17:46:58.086178 fibsem_tools-4.0.2/src/fibsem_tools/metadata/groundtruth.py
--rw-r--r--   0        0        0     2123 2023-03-16 20:03:20.243743 fibsem_tools-4.0.2/src/fibsem_tools/metadata/neuroglancer.py
--rw-r--r--   0        0        0     3371 2023-05-04 18:29:01.065840 fibsem_tools-4.0.2/src/fibsem_tools/metadata/transform.py
--rw-r--r--   0        0        0        0 2023-03-23 17:36:07.629685 fibsem_tools-4.0.2/src/fibsem_tools/py.typed
--rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 fibsem_tools-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-21 23:22:56.299056 fibsem_tools-4.0.3/LICENSE
+-rw-r--r--   0        0        0     1425 2023-06-30 03:00:58.568689 fibsem_tools-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-04-25 22:22:07.080776 fibsem_tools-4.0.3/src/fibsem_tools/__init__.py
+-rw-r--r--   0        0        0      606 2023-04-02 16:17:29.203986 fibsem_tools-4.0.3/src/fibsem_tools/cli/tiff2zarr.css
+-rw-r--r--   0        0        0    13481 2023-04-02 16:17:29.204298 fibsem_tools-4.0.3/src/fibsem_tools/cli/tiff2zarr.py
+-rw-r--r--   0        0        0        0 2023-03-23 18:13:14.517927 fibsem_tools-4.0.3/src/fibsem_tools/io/__init__.py
+-rw-r--r--   0        0        0     7473 2023-06-03 02:33:21.215760 fibsem_tools-4.0.3/src/fibsem_tools/io/core.py
+-rw-r--r--   0        0        0    13817 2023-05-04 17:46:58.084105 fibsem_tools-4.0.3/src/fibsem_tools/io/dask.py
+-rw-r--r--   0        0        0    31797 2023-05-04 18:29:01.063113 fibsem_tools-4.0.3/src/fibsem_tools/io/dat.py
+-rw-r--r--   0        0        0     2258 2023-03-23 19:35:10.739676 fibsem_tools-4.0.3/src/fibsem_tools/io/h5.py
+-rw-r--r--   0        0        0     5081 2023-05-04 18:29:01.063414 fibsem_tools-4.0.3/src/fibsem_tools/io/mrc.py
+-rw-r--r--   0        0        0     6819 2023-06-30 02:59:04.599128 fibsem_tools-4.0.3/src/fibsem_tools/io/multiscale.py
+-rw-r--r--   0        0        0       36 2023-03-23 19:35:10.687732 fibsem_tools-4.0.3/src/fibsem_tools/io/neuroglancer.py
+-rw-r--r--   0        0        0     2341 2023-03-23 19:45:26.756642 fibsem_tools-4.0.3/src/fibsem_tools/io/server.py
+-rw-r--r--   0        0        0      431 2023-05-04 18:29:01.063967 fibsem_tools-4.0.3/src/fibsem_tools/io/tif.py
+-rw-r--r--   0        0        0     4340 2023-06-23 02:17:18.787649 fibsem_tools-4.0.3/src/fibsem_tools/io/util.py
+-rw-r--r--   0        0        0     1504 2023-05-04 18:29:01.064928 fibsem_tools-4.0.3/src/fibsem_tools/io/xr.py
+-rw-r--r--   0        0        0    15193 2023-06-30 02:59:04.599753 fibsem_tools-4.0.3/src/fibsem_tools/io/zarr.py
+-rw-r--r--   0        0        0        0 2023-02-21 23:22:56.301100 fibsem_tools-4.0.3/src/fibsem_tools/metadata/__init__.py
+-rw-r--r--   0        0        0     3195 2023-06-30 02:59:04.600205 fibsem_tools-4.0.3/src/fibsem_tools/metadata/cosem.py
+-rw-r--r--   0        0        0     4120 2023-06-30 02:59:06.586970 fibsem_tools-4.0.3/src/fibsem_tools/metadata/groundtruth.py
+-rw-r--r--   0        0        0     2123 2023-06-30 02:59:04.600763 fibsem_tools-4.0.3/src/fibsem_tools/metadata/neuroglancer.py
+-rw-r--r--   0        0        0     3371 2023-06-30 02:59:04.601504 fibsem_tools-4.0.3/src/fibsem_tools/metadata/transform.py
+-rw-r--r--   0        0        0        0 2023-03-23 17:36:07.629685 fibsem_tools-4.0.3/src/fibsem_tools/py.typed
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 fibsem_tools-4.0.3/PKG-INFO
```

### Comparing `fibsem_tools-4.0.2/LICENSE` & `fibsem_tools-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/pyproject.toml` & `fibsem_tools-4.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fibsem-tools"
-version = "4.0.2"
+version = "4.0.3"
 description = "Tools for processing FIBSEM datasets"
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 distributed = ">=2021.10.0"
```

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/cli/tiff2zarr.css` & `fibsem_tools-4.0.3/src/fibsem_tools/cli/tiff2zarr.css`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/cli/tiff2zarr.py` & `fibsem_tools-4.0.3/src/fibsem_tools/cli/tiff2zarr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/core.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/core.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/dask.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/dask.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/dat.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/dat.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/h5.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/h5.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/mrc.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/mrc.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/multiscale.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/multiscale.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/server.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/server.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/util.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/util.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/xr.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/xr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/io/zarr.py` & `fibsem_tools-4.0.3/src/fibsem_tools/io/zarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,27 +325,28 @@
         coords = [
             stt_coord(array.shape[idx], ax, scales[ax], translates[ax], units[ax])
             for idx, ax in enumerate(output_axes)
         ]
     elif (multiscales := group.attrs.get("multiscales", None)) is not None:
         if len(multiscales) > 0:
             multiscale = multiscales[0]
-            if (ngff_version := multiscale.get("version", None)) == "0.4":
+            ngff_version = multiscale.get("version", None)
+            if ngff_version == "0.4":
                 from pydantic_ome_ngff.v04 import Multiscale
-            elif multiscale["version"] == "0.5-dev":
+            elif ngff_version == "0.5-dev":
                 from pydantic_ome_ngff.latest import Multiscale
             else:
                 raise ValueError(
                     f"""
                     Could not resolve the version of the multiscales metadata 
                     found in the group metadata {dict(group.attrs)}
                     """
                 )
         else:
-            raise ValueError("Multiscales attribute was empty")
+            raise ValueError("Multiscales attribute was empty.")
         xarray_adapters = get_adapters(ngff_version)
         multiscales_meta = [Multiscale(**entry) for entry in multiscales]
         transforms = []
         axes = []
         matched_multiscale = None
         matched_dataset = None
         # find the correct element in multiscales.datasets for this array
```

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/metadata/cosem.py` & `fibsem_tools-4.0.3/src/fibsem_tools/metadata/cosem.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/metadata/groundtruth.py` & `fibsem_tools-4.0.3/src/fibsem_tools/metadata/groundtruth.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,34 +37,29 @@
     annotation_type: AnnotationType = AnnotationType.semantic
 
 
 classNameDict = {
     1: InstanceName(short="ECS", long="Extracellular Space"),
     2: InstanceName(short="Plasma membrane", long="Plasma membrane"),
     3: InstanceName(short="Mito membrane", long="Mitochondrial membrane"),
-    4: InstanceName(
-        short="Mito lumen",
-        long="Mitochondrial lumen",
-    ),
+    4: InstanceName(short="Mito lumen",long="Mitochondrial lumen"),
     5: InstanceName(short="Mito DNA", long="Mitochondrial DNA"),
     6: InstanceName(short="Golgi Membrane", long="Golgi apparatus membrane"),
     7: InstanceName(short="Golgi lumen", long="Golgi apparatus lumen"),
     8: InstanceName(short="Vesicle membrane", long="Vesicle membrane"),
     9: InstanceName(short="Vesicle lumen", long="VesicleLumen"),
     10: InstanceName(short="MVB membrane", long="Multivesicular body membrane"),
     11: InstanceName(short="MVB lumen", long="Multivesicular body lumen"),
     12: InstanceName(short="Lysosome membrane", long="Lysosome membrane"),
     13: InstanceName(short="Lysosome lumen", long="Lysosome membrane"),
     14: InstanceName(short="LD membrane", long="Lipid droplet membrane"),
     15: InstanceName(short="LD lumen", long="Lipid droplet lumen"),
     16: InstanceName(short="ER membrane", long="Endoplasmic reticulum membrane"),
     17: InstanceName(short="ER lumen", long="Endoplasmic reticulum membrane"),
-    18: InstanceName(
-        short="ERES membrane", long="Endoplasmic reticulum exit site membrane"
-    ),
+    18: InstanceName(short="ERES membrane", long="Endoplasmic reticulum exit site membrane"),
     19: InstanceName(short="ERES lumen", long="Endoplasmic reticulum exit site lumen"),
     20: InstanceName(short="NE membrane", long="Nuclear envelope membrane"),
     21: InstanceName(short="NE lumen", long="Nuclear envelope lumen"),
     22: InstanceName(short="Nuclear pore out", long="Nuclear pore out"),
     23: InstanceName(short="Nuclear pore in", long="Nuclear pore in"),
     24: InstanceName(short="HChrom", long="Heterochromatin"),
     25: InstanceName(short="NHChrom", long="Nuclear heterochromatin"),
@@ -78,8 +73,17 @@
     33: InstanceName(short="Subdistal appendages", long="Subdistal appendages"),
     34: InstanceName(short="Ribosomes", long="Ribsoomes"),
     35: InstanceName(short="Cytosol", long="Cytosol"),
     36: InstanceName(short="Microtubules in", long="Microtubules in"),
     37: InstanceName(short="Nucleus combined", long="Nucleus combined"),
     38: InstanceName(short="Vimentin", long="Vimentin"),
     39: InstanceName(short="Glycogen", long="Glycogen"),
+    40: InstanceName(short="Cardiac neurons", long="Cardiac neurons"),
+    41: InstanceName(short="Endothelial cells", long="Endothelial cells"),
+    42: InstanceName(short="Cardiomyocytes", long="Cardiomyocytes"),
+    43: InstanceName(short="Epicardial cells", long="Epicardial cells"),
+    44: InstanceName(short="Parietal pericardial cells", long="Parietal pericardial cells"),
+    45: InstanceName(short="Red blood cells", long="Red blood cells"),
+    46: InstanceName(short="White blood cells", long="White blood cells"),
+    47: InstanceName(short="Peroxisome membrane", long="Peroxisome membrane"),
+    48: InstanceName(short="Peroxisome lumen", long="Peroxisome lumen"),
 }
```

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/metadata/neuroglancer.py` & `fibsem_tools-4.0.3/src/fibsem_tools/metadata/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/src/fibsem_tools/metadata/transform.py` & `fibsem_tools-4.0.3/src/fibsem_tools/metadata/transform.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.2/PKG-INFO` & `fibsem_tools-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibsem-tools
-Version: 4.0.2
+Version: 4.0.3
 Summary: Tools for processing FIBSEM datasets
 License: MIT
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

