# Comparing `tmp/unstructured_inference-0.5.3.tar.gz` & `tmp/unstructured_inference-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.5.3.tar", last modified: Thu Jun 29 17:36:14 2023, max compression
+gzip compressed data, was "unstructured_inference-0.5.4.tar", last modified: Thu Jun 29 22:24:50 2023, max compression
```

## Comparing `unstructured_inference-0.5.3.tar` & `unstructured_inference-0.5.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.543450 unstructured_inference-0.5.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.543450 unstructured_inference-0.5.3/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.543450 unstructured_inference-0.5.3/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/detectron2onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/largemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24059 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.543450 unstructured_inference-0.5.3/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.589525 unstructured_inference-0.5.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.589525 unstructured_inference-0.5.4/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.593525 unstructured_inference-0.5.4/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/largemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24059 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.589525 unstructured_inference-0.5.4/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.5.3/PKG-INFO` & `unstructured_inference-0.5.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.3/README.md` & `unstructured_inference-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/setup.py` & `unstructured_inference-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/inference/elements.py` & `unstructured_inference-0.5.4/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/inference/layout.py` & `unstructured_inference-0.5.4/unstructured_inference/inference/layout.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.5.4/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/inference/ordering.py` & `unstructured_inference-0.5.4/unstructured_inference/inference/ordering.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,11 +23,11 @@
     full_page_threshold_factor
         multiplied by the page width to find the minimum width an elements need to be
         for it to be considered a full page width element.
     """
     if len(layout) == 0:
         return []
 
-    layout.sort(key=lambda element: element.y1)
+    layout.sort(key=lambda element: (element.y1, element.x1, element.y2, element.x2))
     # NOTE(alan): Temporarily revert to orginal logic pending fixing the new logic
     # See code prior to this commit for new logic.
     return layout
```

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/base.py` & `unstructured_inference-0.5.4/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.5.4/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/detectron2onnx.py` & `unstructured_inference-0.5.4/unstructured_inference/models/detectron2onnx.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/donut.py` & `unstructured_inference-0.5.4/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/largemodel.py` & `unstructured_inference-0.5.4/unstructured_inference/models/largemodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.5.4/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/tables.py` & `unstructured_inference-0.5.4/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.5.4/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.5.4/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/models/yolox.py` & `unstructured_inference-0.5.4/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.5.4/unstructured_inference/patches/pdfminer.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/utils.py` & `unstructured_inference-0.5.4/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference/visualize.py` & `unstructured_inference-0.5.4/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.3/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.5.4/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.3/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.5.4/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

