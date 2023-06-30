# Comparing `tmp/surfa-0.5.0.tar.gz` & `tmp/surfa-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfa-0.5.0.tar", last modified: Thu Jun 15 16:05:51 2023, max compression
+gzip compressed data, was "surfa-0.6.0.tar", last modified: Fri Jun 30 19:29:34 2023, max compression
```

## Comparing `surfa-0.5.0.tar` & `surfa-0.6.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.205039 surfa-0.5.0/
--rw-r--r--   0 andrew     (501) staff       (20)      870 2023-06-15 16:05:51.204927 surfa-0.5.0/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)       69 2023-06-15 16:05:37.000000 surfa-0.5.0/pyproject.toml
--rw-r--r--   0 andrew     (501) staff       (20)       38 2023-06-15 16:05:51.205074 surfa-0.5.0/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)     2924 2023-06-15 16:05:37.000000 surfa-0.5.0/setup.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.198626 surfa-0.5.0/surfa/
--rw-r--r--   0 andrew     (501) staff       (20)      664 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/__init__.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.199905 surfa-0.5.0/surfa/core/
--rw-r--r--   0 andrew     (501) staff       (20)      123 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3974 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/array.py
--rw-r--r--   0 andrew     (501) staff       (20)    18376 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/framed.py
--rw-r--r--   0 andrew     (501) staff       (20)      755 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/istype.py
--rw-r--r--   0 andrew     (501) staff       (20)     8479 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/labels.py
--rw-r--r--   0 andrew     (501) staff       (20)     6084 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/slicing.py
--rw-r--r--   0 andrew     (501) staff       (20)    15408 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/freesurfer.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.200245 surfa-0.5.0/surfa/image/
--rw-r--r--   0 andrew     (501) staff       (20)      116 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/image/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    38553 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/image/framed.py
--rw-r--r--   0 andrew     (501) staff       (20)  3167456 2023-06-15 16:05:50.000000 surfa-0.5.0/surfa/image/interp.c
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.202847 surfa-0.5.0/surfa/io/
--rw-r--r--   0 andrew     (501) staff       (20)      236 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     4966 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/affine.py
--rw-r--r--   0 andrew     (501) staff       (20)    25706 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/framed.py
--rw-r--r--   0 andrew     (501) staff       (20)     6620 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/fsio.py
--rw-r--r--   0 andrew     (501) staff       (20)     3848 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/labels.py
--rw-r--r--   0 andrew     (501) staff       (20)    12464 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/mesh.py
--rw-r--r--   0 andrew     (501) staff       (20)     2773 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/protocol.py
--rw-r--r--   0 andrew     (501) staff       (20)     2233 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/utils.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.203791 surfa-0.5.0/surfa/mesh/
--rw-r--r--   0 andrew     (501) staff       (20)       86 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3003 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/cache.py
--rw-r--r--   0 andrew     (501) staff       (20)   277113 2023-06-15 16:05:50.000000 surfa-0.5.0/surfa/mesh/intersection.c
--rw-r--r--   0 andrew     (501) staff       (20)     9567 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/intersection.h
--rw-r--r--   0 andrew     (501) staff       (20)    26913 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/mesh.py
--rw-r--r--   0 andrew     (501) staff       (20)     1339 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/overlay.py
--rw-r--r--   0 andrew     (501) staff       (20)    14900 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/sphere.py
--rw-r--r--   0 andrew     (501) staff       (20)     5711 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/pipeline.py
--rw-r--r--   0 andrew     (501) staff       (20)     3719 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/system.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.204394 surfa-0.5.0/surfa/transform/
--rw-r--r--   0 andrew     (501) staff       (20)      369 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    22054 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/affine.py
--rw-r--r--   0 andrew     (501) staff       (20)    18060 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/geometry.py
--rw-r--r--   0 andrew     (501) staff       (20)     3938 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/orientation.py
--rw-r--r--   0 andrew     (501) staff       (20)     2193 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/space.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.204659 surfa-0.5.0/surfa/vis/
--rw-r--r--   0 andrew     (501) staff       (20)       56 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/vis/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    10570 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/vis/freeview.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.199180 surfa-0.5.0/surfa.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)      870 2023-06-15 16:05:50.000000 surfa-0.5.0/surfa.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      944 2023-06-15 16:05:51.000000 surfa-0.5.0/surfa.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2023-06-15 16:05:50.000000 surfa-0.5.0/surfa.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       39 2023-06-15 16:05:51.000000 surfa-0.5.0/surfa.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)        6 2023-06-15 16:05:51.000000 surfa-0.5.0/surfa.egg-info/top_level.txt
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.204762 surfa-0.5.0/test/
--rw-r--r--   0 andrew     (501) staff       (20)     8354 2023-06-15 16:05:37.000000 surfa-0.5.0/test/test_framed.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.150743 surfa-0.6.0/
+-rw-r--r--   0 andrew     (501) staff       (20)      833 2023-06-30 19:29:34.150503 surfa-0.6.0/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)       69 2023-06-30 19:28:34.000000 surfa-0.6.0/pyproject.toml
+-rw-r--r--   0 andrew     (501) staff       (20)       38 2023-06-30 19:29:34.150782 surfa-0.6.0/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)     2924 2023-06-30 19:28:34.000000 surfa-0.6.0/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.135004 surfa-0.6.0/surfa/
+-rw-r--r--   0 andrew     (501) staff       (20)      664 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/__init__.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.136628 surfa-0.6.0/surfa/core/
+-rw-r--r--   0 andrew     (501) staff       (20)      123 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/core/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3974 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/core/array.py
+-rw-r--r--   0 andrew     (501) staff       (20)    18376 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/core/framed.py
+-rw-r--r--   0 andrew     (501) staff       (20)      755 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/core/istype.py
+-rw-r--r--   0 andrew     (501) staff       (20)     8479 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/core/labels.py
+-rw-r--r--   0 andrew     (501) staff       (20)     6084 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/core/slicing.py
+-rw-r--r--   0 andrew     (501) staff       (20)    15408 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/freesurfer.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.140646 surfa-0.6.0/surfa/image/
+-rw-r--r--   0 andrew     (501) staff       (20)      116 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/image/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    39770 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/image/framed.py
+-rw-r--r--   0 andrew     (501) staff       (20)  3167162 2023-06-30 19:29:33.000000 surfa-0.6.0/surfa/image/interp.c
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.147425 surfa-0.6.0/surfa/io/
+-rw-r--r--   0 andrew     (501) staff       (20)      236 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/io/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     4966 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/io/affine.py
+-rw-r--r--   0 andrew     (501) staff       (20)    25706 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/io/framed.py
+-rw-r--r--   0 andrew     (501) staff       (20)     6620 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/io/fsio.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3848 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/io/labels.py
+-rw-r--r--   0 andrew     (501) staff       (20)    13886 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/io/mesh.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2773 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/io/protocol.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2233 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/io/utils.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.149295 surfa-0.6.0/surfa/mesh/
+-rw-r--r--   0 andrew     (501) staff       (20)      125 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/mesh/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3003 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/mesh/cache.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5270 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/mesh/distance.py
+-rw-r--r--   0 andrew     (501) staff       (20)   276816 2023-06-30 19:29:33.000000 surfa-0.6.0/surfa/mesh/intersection.c
+-rw-r--r--   0 andrew     (501) staff       (20)     9567 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/mesh/intersection.h
+-rw-r--r--   0 andrew     (501) staff       (20)    26913 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/mesh/mesh.py
+-rw-r--r--   0 andrew     (501) staff       (20)     1339 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/mesh/overlay.py
+-rw-r--r--   0 andrew     (501) staff       (20)    15003 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/mesh/sphere.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5711 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/pipeline.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3719 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/system.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.149994 surfa-0.6.0/surfa/transform/
+-rw-r--r--   0 andrew     (501) staff       (20)      369 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/transform/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    22054 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/transform/affine.py
+-rw-r--r--   0 andrew     (501) staff       (20)    17992 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/transform/geometry.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3938 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/transform/orientation.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2193 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/transform/space.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.150221 surfa-0.6.0/surfa/vis/
+-rw-r--r--   0 andrew     (501) staff       (20)       56 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/vis/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10570 2023-06-30 19:28:34.000000 surfa-0.6.0/surfa/vis/freeview.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.135692 surfa-0.6.0/surfa.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)      833 2023-06-30 19:29:34.000000 surfa-0.6.0/surfa.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      967 2023-06-30 19:29:34.000000 surfa-0.6.0/surfa.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2023-06-30 19:29:34.000000 surfa-0.6.0/surfa.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       39 2023-06-30 19:29:34.000000 surfa-0.6.0/surfa.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        6 2023-06-30 19:29:34.000000 surfa-0.6.0/surfa.egg-info/top_level.txt
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-30 19:29:34.150335 surfa-0.6.0/test/
+-rw-r--r--   0 andrew     (501) staff       (20)     8354 2023-06-30 19:28:34.000000 surfa-0.6.0/test/test_framed.py
```

### Comparing `surfa-0.5.0/PKG-INFO` & `surfa-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: surfa
-Version: 0.5.0
+Version: 0.6.0
 Summary: Utilities for medical image and surface processing.
 Home-page: https://github.com/freesurfer/surfa
 Author: Andrew Hoopes
 Author-email: freesurfer@nmr.mgh.harvard.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 
 Surfa is a collection of Python utilities for medical image
 analysis and mesh-based surface processing. It provides tools that operate on 3D image
 arrays and triangular meshes with consideration of their representation in a world (or
 scanner) coordinate system. While broad in scope, surfa is developed with particular
 emphasis on neuroimaging applications.
-
-
```

### Comparing `surfa-0.5.0/setup.py` & `surfa-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/__init__.py` & `surfa-0.6.0/surfa/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # _____
 # SURFA
 #
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 
 from . import system
 
 from .core import stack
 from .core import labels
 from .core import slicing
 from .core import LabelLookup
```

### Comparing `surfa-0.5.0/surfa/core/array.py` & `surfa-0.6.0/surfa/core/array.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/core/framed.py` & `surfa-0.6.0/surfa/core/framed.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/core/istype.py` & `surfa-0.6.0/surfa/core/istype.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/core/labels.py` & `surfa-0.6.0/surfa/core/labels.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/core/slicing.py` & `surfa-0.6.0/surfa/core/slicing.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/freesurfer.py` & `surfa-0.6.0/surfa/freesurfer.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/image/framed.py` & `surfa-0.6.0/surfa/image/framed.py`

 * *Files 2% similar despite different names*

```diff
@@ -835,14 +835,48 @@
         bincounts = [np.bincount(cc.framed_data[..., i].flat)[1:] for i in range(cc.nframes)]
         topk = [(-bc).argsort()[:k] + 1 for bc in bincounts]
         mask = [np.isin(cc.framed_data[..., i], topk[i]) for i in range(self.nframes)]
         if fill:
             mask = [scipy.ndimage.binary_fill_holes(m) for m in mask]
         return stack([self.new(m) for m in mask])
 
+    def distance(self):
+        """
+        Compute the distance transform representing distances outside the binary object.
+
+        See Also
+        --------
+        signed_distance : Compute the signed distance transform.
+
+        Returns
+        -------
+        sdt : !class
+        """
+        sampling = self.geom.voxsize[:self.basedim]
+        dt = lambda x: scipy.ndimage.distance_transform_edt(1 - x, sampling=sampling)
+        return stack([self.new(dt(self.framed_data[..., i])) for i in range(self.nframes)])
+
+    def signed_distance(self):
+        """
+        Compute the signed distance transform of the binary image. Negative values represent
+        distances inside the binary object, and positive values represent distances outside the object.
+
+        See Also
+        --------
+        signed_distance : Compute the distance transform outside the binary object.
+
+        Returns
+        -------
+        sdt : !class
+        """
+        sampling = self.geom.voxsize[:self.basedim]
+        dt = lambda x: scipy.ndimage.distance_transform_edt(x, sampling=sampling)
+        sdt = lambda x: dt(1 - x) - dt(x)
+        return stack([self.new(sdt(self.framed_data[..., i])) for i in range(self.nframes)])
+
 
 class Slice(FramedImage):
 
     def __init__(self, data, geometry=None, labels=None, metadata=None):
         """
         2D image class defining an array with data frames and associated geometry.
```

### Comparing `surfa-0.5.0/surfa/image/interp.c` & `surfa-0.6.0/surfa/image/interp.c`

 * *Files 0% similar despite different names*

```diff
@@ -1109,195 +1109,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":693
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":700
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":705
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":716
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":720
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":723
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":727
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1328,42 +1328,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":731
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":733
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -53956,15 +53956,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_mat, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_disp, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -53973,29 +53973,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":736
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -54006,15 +54006,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -54023,29 +54023,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":739
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -54056,15 +54056,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -54073,29 +54073,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":742
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -54106,15 +54106,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -54123,29 +54123,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":745
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -54156,15 +54156,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -54173,29 +54173,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":748
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -54206,212 +54206,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":752
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":754
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":931
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":936
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":937
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -54427,15 +54427,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -54443,53 +54443,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":943
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":944
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -54497,30 +54497,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -54535,15 +54535,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -54559,15 +54559,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -54575,53 +54575,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":949
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":950
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -54629,30 +54629,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -54667,15 +54667,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -54691,15 +54691,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -54707,53 +54707,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":955
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":956
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":957
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -54761,30 +54761,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -54799,176 +54799,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":979
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":994
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1004
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1011
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1018
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -69092,26 +69092,26 @@
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 951, __pyx_L1_error)
```

### Comparing `surfa-0.5.0/surfa/io/affine.py` & `surfa-0.6.0/surfa/io/affine.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/io/framed.py` & `surfa-0.6.0/surfa/io/framed.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/io/fsio.py` & `surfa-0.6.0/surfa/io/fsio.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/io/labels.py` & `surfa-0.6.0/surfa/io/labels.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/io/mesh.py` & `surfa-0.6.0/surfa/io/mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -361,12 +361,66 @@
         faces = self.nib.gifti.GiftiDataArray(mesh.faces, 'triangle')
 
         gii.add_gifti_data_array(vertices)
         gii.add_gifti_data_array(faces)
         self.nib.gifti.write(gii, filename)
 
 
+class WavefrontIO(protocol.IOProtocol):
+    """
+    Mesh IO protocol for wavefront obj files.
+    """
+
+    name = 'obj'
+    extensions = ('.obj',)
+
+    def __init__(self):
+        try:
+            import trimesh
+        except ImportError:
+            raise ImportError('the trimesh python package must be installed for wavefront surface IO')
+        self.trimesh = trimesh
+
+    def load(self, filename):
+        """
+        Load a wavefront mesh file into a Mesh object.
+
+        Parameters
+        ----------
+        filename : str
+            File path to read.
+
+        Returns
+        -------
+        mesh : Mesh
+            A Mesh object loaded from file.
+        """
+        tmesh = self.trimesh.exchange.load(filename, process=False)
+        return Mesh(tmesh.vertices, tmesh.faces, space='world')
+
+    def save(self, mesh, filename):
+        """
+        Save a Mesh object to a wavefront mesh file.
+
+        Parameters
+        ----------
+        mesh : Mesh
+            Mesh to save.
+        filename : str
+            Destination file path.
+        """
+        parameters = dict(
+            header='SPACE=RAS\n',
+            include_color=False,
+            include_texture=False,
+            return_texture=False,
+            write_texture=True)
+        mesh = mesh.convert(space='world')
+        self.trimesh.Trimesh(mesh.vertices, mesh.faces, process=False).export(filename, **parameters)
+
+
 # enabled mesh IO protocol classes
 mesh_io_protocols = [
     FreesurferSurfaceIO,
     GiftiIO,
+    WavefrontIO,
 ]
```

### Comparing `surfa-0.5.0/surfa/io/protocol.py` & `surfa-0.6.0/surfa/io/protocol.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/io/utils.py` & `surfa-0.6.0/surfa/io/utils.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/mesh/cache.py` & `surfa-0.6.0/surfa/mesh/cache.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/mesh/intersection.c` & `surfa-0.6.0/surfa/mesh/intersection.c`

 * *Files 1% similar despite different names*

```diff
@@ -1042,195 +1042,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":693
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":700
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":705
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":716
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":720
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":723
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":727
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1257,42 +1257,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":731
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":733
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2525,15 +2525,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_arr_selected);
   __Pyx_XDECREF((PyObject *)__pyx_v_arr_neighbors);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2542,29 +2542,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":736
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2575,15 +2575,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2592,29 +2592,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":739
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2625,15 +2625,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2642,29 +2642,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":742
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2675,15 +2675,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2692,29 +2692,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":745
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2725,15 +2725,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2742,29 +2742,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":748
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2775,212 +2775,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":752
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":754
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":931
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":936
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":937
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2996,15 +2996,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3012,53 +3012,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":943
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":944
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -3066,30 +3066,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3104,15 +3104,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3128,15 +3128,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3144,53 +3144,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":949
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":950
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -3198,30 +3198,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3236,15 +3236,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3260,15 +3260,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3276,53 +3276,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":955
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":956
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":957
+      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -3330,30 +3330,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3368,176 +3368,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":979
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":994
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1004
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1011
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1018
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3636,26 +3636,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
@@ -4042,15 +4042,15 @@
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `surfa-0.5.0/surfa/mesh/intersection.h` & `surfa-0.6.0/surfa/mesh/intersection.h`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/mesh/mesh.py` & `surfa-0.6.0/surfa/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/mesh/overlay.py` & `surfa-0.6.0/surfa/mesh/overlay.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/mesh/sphere.py` & `surfa-0.6.0/surfa/mesh/sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,18 @@
     target = conform_sphere(target)
 
     # compute the k-nearest triangles to each target point. this is used to limit the
     # number of triangles that are considered for each target point
     centers = source.triangles.mean(1)
     nearest = cKDTree(centers).query(target.vertices, k=neighborhood, workers=-1)[1].T
 
+    # ensure nearest is a 2D array
+    if neighborhood == 1:
+        nearest = nearest[np.newaxis, :]
+
     # initialize
     intersecting_faces = np.full(target.nvertices, -1, dtype=np.int64)
     intersecting_barycenters = np.zeros((target.nvertices, 3), dtype=np.float64)
 
     dot = lambda a, b: np.dot(a * b, [1.0] * a.shape[1])
     tolerance = np.finfo(np.float64).resolution * 100
```

### Comparing `surfa-0.5.0/surfa/pipeline.py` & `surfa-0.6.0/surfa/pipeline.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/system.py` & `surfa-0.6.0/surfa/system.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/transform/affine.py` & `surfa-0.6.0/surfa/transform/affine.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/transform/geometry.py` & `surfa-0.6.0/surfa/transform/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,19 +333,18 @@
         """
         func = lambda : self.vox2world @ self.surf2vox
         return self._retrieve_or_compute_affine('sw', func)
 
     @property
     def vox2vxm(self):
         # voxel morph centers the col,row,slice
-        M = np.eye(4);
-        M[0][3] = (self._shape[0]-1)/2;
-        M[1][3] = (self._shape[1]-1)/2;
-        M[2][3] = (self._shape[2]-1)/2;
-        return(Affine(M));
+        M = np.eye(4)
+        M[:3,3] = -((np.array(self._shape) - 1) / 2)
+
+        return(Affine(M))
 
     @property
     def vxm2vox(self):
         return(self.vox2vxm.inv())
 
     def _retrieve_or_compute_affine(self, name, func):
         """
```

### Comparing `surfa-0.5.0/surfa/transform/orientation.py` & `surfa-0.6.0/surfa/transform/orientation.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/transform/space.py` & `surfa-0.6.0/surfa/transform/space.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa/vis/freeview.py` & `surfa-0.6.0/surfa/vis/freeview.py`

 * *Files identical despite different names*

### Comparing `surfa-0.5.0/surfa.egg-info/PKG-INFO` & `surfa-0.6.0/surfa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: surfa
-Version: 0.5.0
+Version: 0.6.0
 Summary: Utilities for medical image and surface processing.
 Home-page: https://github.com/freesurfer/surfa
 Author: Andrew Hoopes
 Author-email: freesurfer@nmr.mgh.harvard.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 
 Surfa is a collection of Python utilities for medical image
 analysis and mesh-based surface processing. It provides tools that operate on 3D image
 arrays and triangular meshes with consideration of their representation in a world (or
 scanner) coordinate system. While broad in scope, surfa is developed with particular
 emphasis on neuroimaging applications.
-
-
```

### Comparing `surfa-0.5.0/surfa.egg-info/SOURCES.txt` & `surfa-0.6.0/surfa.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 surfa/io/fsio.py
 surfa/io/labels.py
 surfa/io/mesh.py
 surfa/io/protocol.py
 surfa/io/utils.py
 surfa/mesh/__init__.py
 surfa/mesh/cache.py
+surfa/mesh/distance.py
 surfa/mesh/intersection.c
 surfa/mesh/intersection.h
 surfa/mesh/mesh.py
 surfa/mesh/overlay.py
 surfa/mesh/sphere.py
 surfa/transform/__init__.py
 surfa/transform/affine.py
```

### Comparing `surfa-0.5.0/test/test_framed.py` & `surfa-0.6.0/test/test_framed.py`

 * *Files identical despite different names*

