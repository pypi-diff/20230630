# Comparing `tmp/vision6D-0.2.6.tar.gz` & `tmp/vision6D-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.2.6.tar", last modified: Sat Jun 24 04:19:13 2023, max compression
+gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-cr8lmfij\vision6D-0.2.8.tar", last modified: Fri Jun 30 14:18:17 2023, max compression
```

## Comparing `vision6D-0.2.6.tar` & `vision6D-0.2.8.tar`

### file list

```diff
@@ -1,31 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 04:19:13.112982 vision6D-0.2.6/
--rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.2.6/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1361 2023-06-24 04:19:13.113980 vision6D-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.2.6/README.md
--rw-rw-rw-   0        0        0      406 2023-06-02 21:40:49.000000 vision6D-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0     2050 2023-06-24 04:19:13.116981 vision6D-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      277 2023-06-24 04:13:08.000000 vision6D-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:19:12.903985 vision6D-0.2.6/test/
--rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.6/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.6/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:19:12.968980 vision6D-0.2.6/vision6D/
--rw-rw-rw-   0        0        0    65799 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/GUI.py
--rw-rw-rw-   0        0        0      910 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:19:13.086981 vision6D-0.2.6/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.6/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.6/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-06-06 19:10:46.000000 vision6D-0.2.6/vision6D/data/style.qss
-drwxrwxrwx   0        0        0        0 2023-06-24 04:19:13.110981 vision6D-0.2.6/vision6D/entry/
--rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.2.6/vision6D/entry/__init__.py
--rw-rw-rw-   0        0        0      422 2023-06-24 04:14:35.000000 vision6D-0.2.6/vision6D/entry/main.py
--rw-rw-rw-   0        0        0    17032 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    15676 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/utils.py
--rw-rw-rw-   0        0        0    24790 2023-06-24 04:12:06.000000 vision6D-0.2.6/vision6D/widgets_gui.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:19:13.030981 vision6D-0.2.6/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1361 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 04:19:12.000000 vision6D-0.2.6/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.213688 vision6D-0.2.8/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1361 2023-06-30 14:18:17.213688 vision6D-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.2.8/README.md
+-rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0     2050 2023-06-30 14:18:17.217684 vision6D-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      345 2023-06-30 14:14:27.000000 vision6D-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.076685 vision6D-0.2.8/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.8/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.8/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.088681 vision6D-0.2.8/vision6D/
+-rw-rw-rw-   0        0        0     1050 2023-06-26 14:07:57.000000 vision6D-0.2.8/vision6D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.151682 vision6D-0.2.8/vision6D/components/
+-rw-rw-rw-   0        0        0      403 2023-06-25 23:11:35.000000 vision6D-0.2.8/vision6D/components/__init__.py
+-rw-rw-rw-   0        0        0     1735 2023-06-25 17:11:58.000000 vision6D-0.2.8/vision6D/components/camera_store.py
+-rw-rw-rw-   0        0        0     2417 2023-06-26 02:53:06.000000 vision6D-0.2.8/vision6D/components/folder_store.py
+-rw-rw-rw-   0        0        0     1998 2023-06-27 14:55:28.000000 vision6D-0.2.8/vision6D/components/image_store.py
+-rw-rw-rw-   0        0        0     2756 2023-06-28 13:51:18.000000 vision6D-0.2.8/vision6D/components/mask_store.py
+-rw-rw-rw-   0        0        0     6338 2023-06-27 14:55:54.000000 vision6D-0.2.8/vision6D/components/mesh_store.py
+-rw-rw-rw-   0        0        0      242 2023-06-24 14:48:03.000000 vision6D-0.2.8/vision6D/components/singleton.py
+-rw-rw-rw-   0        0        0     1983 2023-06-26 03:58:35.000000 vision6D-0.2.8/vision6D/components/video_store.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.167685 vision6D-0.2.8/vision6D/containers/
+-rw-rw-rw-   0        0        0      429 2023-06-26 19:34:52.000000 vision6D-0.2.8/vision6D/containers/__init__.py
+-rw-rw-rw-   0        0        0     3815 2023-06-27 01:22:39.000000 vision6D-0.2.8/vision6D/containers/camera_container.py
+-rw-rw-rw-   0        0        0     4027 2023-06-29 13:21:48.000000 vision6D-0.2.8/vision6D/containers/image_container.py
+-rw-rw-rw-   0        0        0     5492 2023-06-29 13:21:55.000000 vision6D-0.2.8/vision6D/containers/mask_container.py
+-rw-rw-rw-   0        0        0    17728 2023-06-29 13:22:01.000000 vision6D-0.2.8/vision6D/containers/mesh_container.py
+-rw-rw-rw-   0        0        0    11023 2023-06-29 14:00:00.000000 vision6D-0.2.8/vision6D/containers/pnp_container.py
+-rw-rw-rw-   0        0        0     9570 2023-06-28 23:58:17.000000 vision6D-0.2.8/vision6D/containers/video_folder_container.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.179691 vision6D-0.2.8/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.8/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0    12109 2023-06-06 19:10:46.000000 vision6D-0.2.8/vision6D/data/style.qss
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.183685 vision6D-0.2.8/vision6D/entry/
+-rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.2.8/vision6D/entry/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-06-26 13:21:29.000000 vision6D-0.2.8/vision6D/entry/main.py
+-rw-rw-rw-   0        0        0    33624 2023-06-29 13:18:10.000000 vision6D-0.2.8/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    16150 2023-06-28 23:06:33.000000 vision6D-0.2.8/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.210687 vision6D-0.2.8/vision6D/widgets/
+-rw-rw-rw-   0        0        0      583 2023-06-26 03:46:38.000000 vision6D-0.2.8/vision6D/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3216 2023-06-26 04:19:25.000000 vision6D-0.2.8/vision6D/widgets/calibration_pop_window.py
+-rw-rw-rw-   0        0        0     1789 2023-06-26 04:18:34.000000 vision6D-0.2.8/vision6D/widgets/camera_props_input_dialog.py
+-rw-rw-rw-   0        0        0     1437 2023-06-28 02:56:35.000000 vision6D-0.2.8/vision6D/widgets/custom_qt_interactor.py
+-rw-rw-rw-   0        0        0     2314 2023-06-26 16:29:32.000000 vision6D-0.2.8/vision6D/widgets/get_text_dialog.py
+-rw-rw-rw-   0        0        0     3539 2023-06-27 03:53:28.000000 vision6D-0.2.8/vision6D/widgets/label_window.py
+-rw-rw-rw-   0        0        0     1063 2023-06-26 04:18:12.000000 vision6D-0.2.8/vision6D/widgets/popup_dialog.py
+-rw-rw-rw-   0        0        0     6876 2023-06-26 04:17:38.000000 vision6D-0.2.8/vision6D/widgets/video_player.py
+-rw-rw-rw-   0        0        0     5509 2023-06-26 04:17:03.000000 vision6D-0.2.8/vision6D/widgets/video_sampler.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:18:17.132683 vision6D-0.2.8/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1361 2023-06-30 14:18:16.000000 vision6D-0.2.8/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1363 2023-06-30 14:18:17.000000 vision6D-0.2.8/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:18:16.000000 vision6D-0.2.8/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-30 14:18:16.000000 vision6D-0.2.8/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-06-30 14:18:16.000000 vision6D-0.2.8/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 14:18:17.000000 vision6D-0.2.8/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.2.6/LICENSE` & `vision6D-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.6/PKG-INFO` & `vision6D-0.2.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.6
+Version: 0.2.8
 Summary: vision6D: A tool for 6D pose estimation annotation
-Home-page: https://github.com/ykzzky/vision6D
+Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `vision6D-0.2.6/README.md` & `vision6D-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.6/setup.cfg` & `vision6D-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e36 0d0a 7572  sion = 0.2.6..ur
+00000020: 7369 6f6e 203d 2030 2e32 2e38 0d0a 7572  sion = 0.2.8..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.2.6/test/test_create_dataset.py` & `vision6D-0.2.8/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.6/test/test_projection.py` & `vision6D-0.2.8/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.6/vision6D/__init__.py` & `vision6D-0.2.8/vision6D/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,10 +26,20 @@
     # },
 }
 
 # Setup the logging configuration
 logging.config.dictConfig(LOGGING_CONFIG)
 
 from .mainwindow import MyMainWindow
-from .GUI import Interface
 from . import utils
-from . import widgets_gui
+from . import widgets
+from . import components
+from . import containers
+
+all = [
+    'MyMainWindow',
+    'Interface',
+    'utils',
+    'widgets',
+    'components',
+    'containers'
+]
```

### Comparing `vision6D-0.2.6/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.2.8/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.6/vision6D/data/style.qss` & `vision6D-0.2.8/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.6/vision6D/utils.py` & `vision6D-0.2.8/vision6D/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import __future__
 import copy
-from typing import Type
 import logging
 
 import numpy as np
 import pathlib
 import os
 import pyvista as pv
 import matplotlib.pyplot as plt
 from easydict import EasyDict
 import trimesh
 from PIL import Image
 import cv2
-import pygeodesic.geodesic as geodesic
+# import pygeodesic.geodesic as geodesic
 import vtk.util.numpy_support as vtknp
 import json
 
 CWD = pathlib.Path(os.path.abspath(__file__)).parent
 logger = logging.getLogger("vision6D")
 
 def fread(fid, _len, _type):
@@ -400,7 +399,20 @@
 
 def get_mesh_actor_scalars(actor):
     input = actor.GetMapper().GetInput()
     point_data = input.GetPointData()
     scalars = point_data.GetScalars()
     if scalars: scalars = vtknp.vtk_to_numpy(scalars)
     return scalars
+
+def create_render(w, h):
+    render = pv.Plotter(window_size=[w, h], lighting=None, off_screen=True) 
+    render.set_background('black')
+    assert render.background_color == "black", "render's background need to be black"
+    return render
+
+# Calculate the rotation error
+def angler_distance(R_a, R_b):
+    R_diff = np.dot(R_a, R_b.T)
+    angle_diff_rad = np.arccos(np.clip((np.trace(R_diff) - 1) / 2, -1, 1))
+    angle_diff_deg = np.degrees(angle_diff_rad)
+    return angle_diff_deg
```

### Comparing `vision6D-0.2.6/vision6D.egg-info/PKG-INFO` & `vision6D-0.2.8/vision6D.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.6
+Version: 0.2.8
 Summary: vision6D: A tool for 6D pose estimation annotation
-Home-page: https://github.com/ykzzky/vision6D
+Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

