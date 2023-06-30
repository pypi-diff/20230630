# Comparing `tmp/rembg-2.0.48.tar.gz` & `tmp/rembg-2.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.48.tar", last modified: Thu Jun 29 23:48:04 2023, max compression
+gzip compressed data, was "rembg-2.0.49.tar", last modified: Fri Jun 30 00:48:08 2023, max compression
```

## Comparing `rembg-2.0.48.tar` & `rembg-2.0.49.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 23:46:48.000000 rembg-2.0.48/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 23:46:48.000000 rembg-2.0.48/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-29 23:48:04.068781 rembg-2.0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-06-29 23:46:48.000000 rembg-2.0.48/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-29 23:46:48.000000 rembg-2.0.48/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.072781 rembg-2.0.48/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 23:48:04.072781 rembg-2.0.48/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 23:48:04.072781 rembg-2.0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-29 23:46:48.000000 rembg-2.0.48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-29 23:46:48.000000 rembg-2.0.48/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-29 23:46:48.000000 rembg-2.0.48/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 00:46:58.000000 rembg-2.0.49/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-30 00:46:58.000000 rembg-2.0.49/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-30 00:48:08.546652 rembg-2.0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-06-30 00:46:58.000000 rembg-2.0.49/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-30 00:46:58.000000 rembg-2.0.49/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-30 00:46:58.000000 rembg-2.0.49/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 00:48:08.000000 rembg-2.0.49/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 00:48:08.546652 rembg-2.0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-30 00:46:58.000000 rembg-2.0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:08.546652 rembg-2.0.49/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-30 00:46:58.000000 rembg-2.0.49/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-30 00:46:58.000000 rembg-2.0.49/versioneer.py
```

### Comparing `rembg-2.0.48/LICENSE.txt` & `rembg-2.0.49/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/PKG-INFO` & `rembg-2.0.49/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.48
+Version: 2.0.49
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.48/README.md` & `rembg-2.0.49/README.md`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/bg.py` & `rembg-2.0.49/rembg/bg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/cli.py` & `rembg-2.0.49/rembg/cli.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/commands/b_command.py` & `rembg-2.0.49/rembg/commands/b_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/commands/i_command.py` & `rembg-2.0.49/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/commands/p_command.py` & `rembg-2.0.49/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/commands/s_command.py` & `rembg-2.0.49/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/session_factory.py` & `rembg-2.0.49/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/__init__.py` & `rembg-2.0.49/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/base.py` & `rembg-2.0.49/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/dis_anime.py` & `rembg-2.0.49/rembg/sessions/dis_anime.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/dis_general_use.py` & `rembg-2.0.49/rembg/sessions/dis_general_use.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/sam.py` & `rembg-2.0.49/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/silueta.py` & `rembg-2.0.49/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/u2net.py` & `rembg-2.0.49/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.49/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/u2net_custom.py` & `rembg-2.0.49/rembg/sessions/u2net_custom.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 import os
 from typing import List
 
 import numpy as np
+import onnxruntime as ort
 import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 
 from .base import BaseSession
 
 
 class U2netCustomSession(BaseSession):
+    def __init__(
+        self,
+        model_name: str,
+        sess_opts: ort.SessionOptions,
+        providers=None,
+        *args,
+        **kwargs
+    ):
+        model_path = kwargs.get("model_path")
+        if model_path is None:
+            raise ValueError("model_path is required")
+
+        super().__init__(model_name, sess_opts, providers, *args, **kwargs)
+
     def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         ort_outs = self.inner_session.run(
             None,
             self.normalize(
                 img, (0.485, 0.456, 0.406), (0.229, 0.224, 0.225), (320, 320)
             ),
         )
@@ -30,16 +45,15 @@
         mask = mask.resize(img.size, Image.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         model_path = kwargs.get("model_path")
-
         if model_path is None:
-            raise ValueError("model_path is required")
+            return
 
         return os.path.abspath(os.path.expanduser(model_path))
 
     @classmethod
     def name(cls, *args, **kwargs):
         return "u2net_custom"
```

### Comparing `rembg-2.0.48/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.49/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg/sessions/u2netp.py` & `rembg-2.0.49/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/rembg.egg-info/PKG-INFO` & `rembg-2.0.49/rembg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.48
+Version: 2.0.49
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.48/rembg.egg-info/SOURCES.txt` & `rembg-2.0.49/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/setup.py` & `rembg-2.0.49/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/tests/test_remove.py` & `rembg-2.0.49/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.48/versioneer.py` & `rembg-2.0.49/versioneer.py`

 * *Files identical despite different names*

