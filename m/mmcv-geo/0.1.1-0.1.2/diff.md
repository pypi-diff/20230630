# Comparing `tmp/mmcv_geo-0.1.1.tar.gz` & `tmp/mmcv_geo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcv_geo-0.1.1.tar", max compression
+gzip compressed data, was "mmcv_geo-0.1.2.tar", max compression
```

## Comparing `mmcv_geo-0.1.1.tar` & `mmcv_geo-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-24 11:26:59.255825 mmcv_geo-0.1.1/README.md
--rw-r--r--   0        0        0       66 2023-06-30 09:56:59.196726 mmcv_geo-0.1.1/mmcv_geo/__init__.py
--rw-r--r--   0        0        0      223 2023-06-30 10:11:23.274716 mmcv_geo-0.1.1/mmcv_geo/image/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-30 10:06:12.933720 mmcv_geo-0.1.1/mmcv_geo/image/io.py
--rw-r--r--   0        0        0      572 2023-06-30 10:13:53.351714 mmcv_geo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 mmcv_geo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 11:26:59.255825 mmcv_geo-0.1.2/README.md
+-rw-r--r--   0        0        0       66 2023-06-30 09:56:59.196726 mmcv_geo-0.1.2/mmcv_geo/__init__.py
+-rw-r--r--   0        0        0      223 2023-06-30 10:11:23.274716 mmcv_geo-0.1.2/mmcv_geo/image/__init__.py
+-rw-r--r--   0        0        0     1897 2023-06-30 10:27:34.778705 mmcv_geo-0.1.2/mmcv_geo/image/io.py
+-rw-r--r--   0        0        0      572 2023-06-30 10:27:48.127704 mmcv_geo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 mmcv_geo-0.1.2/PKG-INFO
```

### Comparing `mmcv_geo-0.1.1/mmcv_geo/image/io.py` & `mmcv_geo-0.1.2/mmcv_geo/image/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,12 +42,12 @@
         raise ValueError(
             f'backend: {backend} is not supported. Supported '
             "backends are 'cv2', 'turbojpeg', 'pillow', 'tifffile' and 'geotiff'.")
     if backend == 'geotiff':
         with io.BytesIO(content) as buff,rio.io.MemoryFile(buff) as memfile:
             with memfile.open() as dataset:
                 img = dataset.read()
-            return img.transpose(1,2,0)
+        return img.transpose(1,2,0)
     else:
         return mmcv_imfrombytes(content, flag, channel_order, backend)
 
 # mmcv_io.imfrombytes=imfrombytes
```

### Comparing `mmcv_geo-0.1.1/pyproject.toml` & `mmcv_geo-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mmcv-geo"
-version = "0.1.1"
+version = "0.1.2"
 description = "the geospatial extension of mmcv 2"
 authors = ["Mengjia Liu <jaeliu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "mmcv_geo"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

