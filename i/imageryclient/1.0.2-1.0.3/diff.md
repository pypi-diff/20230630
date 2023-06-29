# Comparing `tmp/imageryclient-1.0.2.tar.gz` & `tmp/imageryclient-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imageryclient-1.0.2.tar", last modified: Mon May  8 17:55:09 2023, max compression
+gzip compressed data, was "imageryclient-1.0.3.tar", last modified: Thu Jun 29 22:21:36 2023, max compression
```

## Comparing `imageryclient-1.0.2.tar` & `imageryclient-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-08 17:55:09.570518 imageryclient-1.0.2/
--rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:21:56.000000 imageryclient-1.0.2/LICENSE
--rw-r--r--   0 caseysm    (501) staff       (20)       49 2022-11-16 18:21:56.000000 imageryclient-1.0.2/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)     1554 2023-05-08 17:55:09.570395 imageryclient-1.0.2/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)    16014 2023-05-08 17:45:33.000000 imageryclient-1.0.2/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-08 17:55:09.569291 imageryclient-1.0.2/imageryclient/
--rw-r--r--   0 caseysm    (501) staff       (20)      133 2023-05-08 17:54:59.000000 imageryclient-1.0.2/imageryclient/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11089 2022-11-29 01:10:22.000000 imageryclient-1.0.2/imageryclient/composite.py
--rw-r--r--   0 caseysm    (501) staff       (20)    39350 2023-05-08 17:39:36.000000 imageryclient-1.0.2/imageryclient/imagery.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6359 2022-11-29 01:07:39.000000 imageryclient-1.0.2/imageryclient/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-08 17:55:09.570226 imageryclient-1.0.2/imageryclient.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)     1554 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      356 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       81 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       14 2023-05-08 17:55:09.000000 imageryclient-1.0.2/imageryclient.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2022-11-28 07:21:09.000000 imageryclient-1.0.2/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-08 17:55:09.570563 imageryclient-1.0.2/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1166 2022-11-16 18:21:56.000000 imageryclient-1.0.2/setup.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1254 2022-11-16 18:21:56.000000 imageryclient-1.0.2/short_readme.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-06-29 22:21:36.686398 imageryclient-1.0.3/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:21:56.000000 imageryclient-1.0.3/LICENSE
+-rw-r--r--   0 caseysm    (501) staff       (20)       49 2022-11-16 18:21:56.000000 imageryclient-1.0.3/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)     1554 2023-06-29 22:21:36.686074 imageryclient-1.0.3/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)    16014 2023-05-08 17:45:33.000000 imageryclient-1.0.3/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-06-29 22:21:36.684172 imageryclient-1.0.3/imageryclient/
+-rw-r--r--   0 caseysm    (501) staff       (20)      133 2023-06-29 22:21:23.000000 imageryclient-1.0.3/imageryclient/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    11089 2022-11-29 01:10:22.000000 imageryclient-1.0.3/imageryclient/composite.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    40224 2023-06-29 22:19:16.000000 imageryclient-1.0.3/imageryclient/imagery.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6579 2023-06-29 22:20:49.000000 imageryclient-1.0.3/imageryclient/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-06-29 22:21:36.685469 imageryclient-1.0.3/imageryclient.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1554 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      356 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       81 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       14 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2022-11-28 07:21:09.000000 imageryclient-1.0.3/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-06-29 22:21:36.686484 imageryclient-1.0.3/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1166 2022-11-16 18:21:56.000000 imageryclient-1.0.3/setup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1254 2022-11-16 18:21:56.000000 imageryclient-1.0.3/short_readme.md
```

### Comparing `imageryclient-1.0.2/LICENSE` & `imageryclient-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imageryclient-1.0.2/PKG-INFO` & `imageryclient-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageryclient
-Version: 1.0.2
+Version: 1.0.3
 Summary: Front end tools for composite images for EM connectomics
 Home-page: https://github.com/ceesem/ImageryClient
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imageryclient-1.0.2/README.md` & `imageryclient-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `imageryclient-1.0.2/imageryclient/composite.py` & `imageryclient-1.0.3/imageryclient/composite.py`

 * *Files identical despite different names*

### Comparing `imageryclient-1.0.2/imageryclient/imagery.py` & `imageryclient-1.0.3/imageryclient/imagery.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,15 @@
         root_ids="all",
         bbox_size=None,
         image_size=None,
         mip=None,
         resolution=None,
         timestamp=None,
         scale_to_bounds=None,
+        convert_to_int64=True,
     ):
         """Get a cutout of the segmentation imagery for some or all root ids between set bounds.
         Note that if all root ids are requested in a large region, it could take a long time to query
         all supervoxels.
 
         Parameters
         ----------
@@ -443,15 +444,18 @@
             Mip level of the segmentation if something other than the defualt is wanted, by default None
         resolution : list-like, optional
             Voxel resolution used when specifying bounds bounds and bbox_size (but not image_size). If none, defaults to client default.
         timestamp : datetime or None, optional
             Timestamp to use for dynamic segmentation data
         scale_to_bounds : bool or None, optional
             If True, rescales image to the same size as the bounds. Default is None, which rescales if mip is not set but otherwise does not.
-
+        convert_to_int64 : bool, optional
+            If True, converts segmentation data to int64 from uint64 if it is safe to do so. Default is True.
+            If not safe, raises a warning and does not convert from uint64.
+            
         Returns
         -------
         numpy.ndarray
             Array whose elements correspond to the root id (or, if root_ids=None, the supervoxel id) at each voxel.
         """
         if self.segmentation_cv is None:
             return np.array([])
@@ -493,17 +497,23 @@
                 np.squeeze(
                     self.segmentation_cv.download(
                         bbox,
                         segids=root_ids,
                         mip=mip,
                         coord_resolution=resolution,
                         timestamp=timestamp,
+                        agglomerate=False,
                     )
                 )
             )
+        if convert_to_int64:
+            if utils.safe_to_convert_uint64(seg):
+                seg = seg.astype(np.int64)
+            else:
+                raise Warning('Could not convert to int64 because values are too large. Returning as uint64.')
 
         if scale_to_bounds:
             return utils.rescale_to_bounds(
                 seg,
                 self._compute_bounds(bounds, bbox_size),  # downloading changes the bbox
             )
         else:
@@ -573,14 +583,15 @@
         resize=True,
         split_segmentations=False,
         include_null_root=False,
         bbox_size=None,
         resolution=None,
         timestamp=None,
         scale_to_bounds=None,
+        convert_to_int64=True,
     ):
 
         """Download aligned and scaled imagery and segmentation data at a given resolution.
 
         Parameters
         ----------
         bounds : 2x3 list of ints
@@ -606,15 +617,17 @@
             as the center.
         resolution : list-like, optional
             Voxel resolution used when specifying bounds bounds and bbox_size (but not image_size). If none, defaults to client default.
         timestamp : datetime or None, optional
             Timestamp to use for dynamic segmentation data
         scale_to_bounds : bool or None, optional
             If True, rescales image to the same size as the bounds. Default is None, which rescales if mip is not set but otherwise does not.
-
+        convert_to_int64 : bool, optional
+            If True, converts segmentation data to int64 from uint64 if it is safe to do so. Default is True.
+            If not safe, raises a warning and does not convert from uint64.
 
         Returns
         -------
         cloudvolume.VolumeCutout
             Imagery volume cutout
 
         numpy.ndarray or dict
@@ -657,14 +670,15 @@
                 bounds,
                 root_ids=root_ids,
                 mip=segmentation_mip,
                 bbox_size=bbox_size,
                 resolution=resolution,
                 timestamp=timestamp,
                 scale_to_bounds=scale_to_bounds_seg,
+                convert_to_int64=convert_to_int64,
             )
             seg_shape = seg.shape
         else:
             seg = self.split_segmentation_cutout(
                 bounds,
                 root_ids=root_ids,
                 mip=segmentation_mip,
```

### Comparing `imageryclient-1.0.2/imageryclient/utils.py` & `imageryclient-1.0.3/imageryclient/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,7 +222,16 @@
     split_segmentation = {}
     for root_id in np.unique(seg_img):
         if include_null_root is False:
             if root_id == 0:
                 continue
         split_segmentation[root_id] = (seg_img == root_id).astype(int)
     return split_segmentation
+
+
+def safe_to_convert_uint64(val):
+  """Returns True if the uint64 value is safe to convert to an int64, False otherwise."""
+  max_int64 = 2**64 - 1
+  if np.any(val > max_int64):
+    return False
+  else:
+    return True
```

### Comparing `imageryclient-1.0.2/imageryclient.egg-info/PKG-INFO` & `imageryclient-1.0.3/imageryclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageryclient
-Version: 1.0.2
+Version: 1.0.3
 Summary: Front end tools for composite images for EM connectomics
 Home-page: https://github.com/ceesem/ImageryClient
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imageryclient-1.0.2/setup.py` & `imageryclient-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `imageryclient-1.0.2/short_readme.md` & `imageryclient-1.0.3/short_readme.md`

 * *Files identical despite different names*

