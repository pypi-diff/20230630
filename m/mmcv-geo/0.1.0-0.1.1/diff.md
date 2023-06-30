# Comparing `tmp/mmcv_geo-0.1.0.tar.gz` & `tmp/mmcv_geo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcv_geo-0.1.0.tar", max compression
+gzip compressed data, was "mmcv_geo-0.1.1.tar", max compression
```

## Comparing `mmcv_geo-0.1.0.tar` & `mmcv_geo-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-24 11:26:59.255825 mmcv_geo-0.1.0/README.md
--rw-r--r--   0        0        0       20 2023-06-24 13:20:45.416743 mmcv_geo-0.1.0/mmcv_geo/__init__.py
--rw-r--r--   0        0        0       79 2023-06-24 13:20:06.031744 mmcv_geo-0.1.0/mmcv_geo/image/__init__.py
--rw-r--r--   0        0        0      155 2023-06-24 13:20:07.964744 mmcv_geo-0.1.0/mmcv_geo/image/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1824 2023-06-24 13:25:16.080740 mmcv_geo-0.1.0/mmcv_geo/image/__pycache__/io.cpython-39.pyc
--rw-r--r--   0        0        0     1884 2023-06-24 13:25:14.095740 mmcv_geo-0.1.0/mmcv_geo/image/io.py
--rw-r--r--   0        0        0      572 2023-06-24 13:31:42.459736 mmcv_geo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 mmcv_geo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 11:26:59.255825 mmcv_geo-0.1.1/README.md
+-rw-r--r--   0        0        0       66 2023-06-30 09:56:59.196726 mmcv_geo-0.1.1/mmcv_geo/__init__.py
+-rw-r--r--   0        0        0      223 2023-06-30 10:11:23.274716 mmcv_geo-0.1.1/mmcv_geo/image/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-30 10:06:12.933720 mmcv_geo-0.1.1/mmcv_geo/image/io.py
+-rw-r--r--   0        0        0      572 2023-06-30 10:13:53.351714 mmcv_geo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 mmcv_geo-0.1.1/PKG-INFO
```

### Comparing `mmcv_geo-0.1.0/mmcv_geo/image/io.py` & `mmcv_geo-0.1.1/mmcv_geo/image/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 from typing import Optional
 import numpy as np
 import io
 from mmcv.image.io import supported_backends as mmcv_supported_backends
 from mmcv.image.io import use_backend as mmcv_use_backend
 from mmcv.image.io import imfrombytes as mmcv_imfrombytes
-from mmcv.image import io as mmcv_io
 try:
     import rasterio as rio
 except ImportError:
     rio = None
 
-mmcv_supported_backends+=['geotiff']
-mmcv_io.supported_backends=mmcv_supported_backends
+supported_backends=mmcv_supported_backends+['geotiff']
+# mmcv_io.supported_backends=mmcv_supported_backends
 def use_backend(backend: str) -> None:
     """Select a backend for image decoding.
 
     Args:
         backend (str): The image decoding backend type. Options are `cv2`,
         `pillow`, `turbojpeg` (see https://github.com/lilohuang/PyTurboJPEG)
         , `tifffile`and `GTiff`. `turbojpeg` is faster but it only supports `.jpeg`
         file format.
     """
-    assert backend in mmcv_supported_backends
+    assert backend in supported_backends, f'backend: {backend} is not supported'
     global imread_backend
     imread_backend = backend
    
     if imread_backend == 'geotiff':
         if rio is None:
             raise ImportError('`rasterio` is not installed')
     mmcv_use_backend(backend)
 
-mmcv_io.use_backend=use_backend
+# mmcv_io.use_backend=use_backend
 
 def imfrombytes(content: bytes,
                 flag: str = 'color',
                 channel_order: str = 'bgr',
                 backend: Optional[str] = None) -> np.ndarray:
     
     if backend is None:
         backend = imread_backend
-    if backend not in mmcv_supported_backends:
+    if backend not in supported_backends:
         raise ValueError(
             f'backend: {backend} is not supported. Supported '
             "backends are 'cv2', 'turbojpeg', 'pillow', 'tifffile' and 'geotiff'.")
     if backend == 'geotiff':
         with io.BytesIO(content) as buff,rio.io.MemoryFile(buff) as memfile:
             with memfile.open() as dataset:
                 img = dataset.read()
             return img.transpose(1,2,0)
     else:
         return mmcv_imfrombytes(content, flag, channel_order, backend)
 
-mmcv_io.imfrombytes=imfrombytes
+# mmcv_io.imfrombytes=imfrombytes
```

### Comparing `mmcv_geo-0.1.0/pyproject.toml` & `mmcv_geo-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mmcv-geo"
-version = "0.1.0"
+version = "0.1.1"
 description = "the geospatial extension of mmcv 2"
 authors = ["Mengjia Liu <jaeliu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "mmcv_geo"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

