# Comparing `tmp/snake_opencv-0.1.6.tar.gz` & `tmp/snake_opencv-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_opencv-0.1.6.tar", max compression
+gzip compressed data, was "snake_opencv-0.1.7.tar", max compression
```

## Comparing `snake_opencv-0.1.6.tar` & `snake_opencv-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.6/LICENSE
--rw-r--r--   0        0        0      346 2023-05-28 23:17:20.546476 snake_opencv-0.1.6/README.md
--rw-r--r--   0        0        0      686 2023-06-09 16:58:51.083870 snake_opencv-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.6/snake_opencv/__init__.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.6/snake_opencv/core/__init__.py
--rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.6/snake_opencv/core/binding.py
--rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.6/snake_opencv/core/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.6/snake_opencv/dnn/__init__.py
--rw-r--r--   0        0        0     3649 2023-05-28 23:04:14.326704 snake_opencv-0.1.6/snake_opencv/dnn/binding.py
--rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.6/snake_opencv/dnn/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.6/snake_opencv/highgui/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.6/snake_opencv/highgui/binding.py
--rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.6/snake_opencv/highgui/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.6/snake_opencv/imgcodecs/__init__.py
--rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.6/snake_opencv/imgcodecs/binding.py
--rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.6/snake_opencv/imgcodecs/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.6/snake_opencv/imgproc/__init__.py
--rw-r--r--   0        0        0    46800 2023-06-09 16:55:09.639974 snake_opencv-0.1.6/snake_opencv/imgproc/binding.py
--rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.6/snake_opencv/imgproc/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.6/snake_opencv/photo/__init__.py
--rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.6/snake_opencv/photo/binding.py
--rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.6/snake_opencv/photo/const.py
--rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.6/snake_opencv/py.typed
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.6/snake_opencv/videoio/__init__.py
--rw-r--r--   0        0        0     7320 2023-05-28 22:54:24.723745 snake_opencv-0.1.6/snake_opencv/videoio/binding.py
--rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.6/snake_opencv/videoio/const.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 snake_opencv-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.7/LICENSE
+-rw-r--r--   0        0        0      346 2023-05-28 23:17:20.546476 snake_opencv-0.1.7/README.md
+-rw-r--r--   0        0        0      686 2023-06-30 20:22:06.990377 snake_opencv-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.7/snake_opencv/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.7/snake_opencv/core/__init__.py
+-rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.7/snake_opencv/core/binding.py
+-rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.7/snake_opencv/core/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.7/snake_opencv/dnn/__init__.py
+-rw-r--r--   0        0        0     3649 2023-05-28 23:04:14.326704 snake_opencv-0.1.7/snake_opencv/dnn/binding.py
+-rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.7/snake_opencv/dnn/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.7/snake_opencv/highgui/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.7/snake_opencv/highgui/binding.py
+-rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.7/snake_opencv/highgui/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.7/snake_opencv/imgcodecs/__init__.py
+-rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.7/snake_opencv/imgcodecs/binding.py
+-rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.7/snake_opencv/imgcodecs/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.7/snake_opencv/imgproc/__init__.py
+-rw-r--r--   0        0        0    48391 2023-06-30 20:21:28.750359 snake_opencv-0.1.7/snake_opencv/imgproc/binding.py
+-rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.7/snake_opencv/imgproc/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.7/snake_opencv/photo/__init__.py
+-rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.7/snake_opencv/photo/binding.py
+-rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.7/snake_opencv/photo/const.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.7/snake_opencv/py.typed
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.7/snake_opencv/videoio/__init__.py
+-rw-r--r--   0        0        0     7320 2023-05-28 22:54:24.723745 snake_opencv-0.1.7/snake_opencv/videoio/binding.py
+-rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.7/snake_opencv/videoio/const.py
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 snake_opencv-0.1.7/PKG-INFO
```

### Comparing `snake_opencv-0.1.6/LICENSE` & `snake_opencv-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/pyproject.toml` & `snake_opencv-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snake-opencv"
-version = "0.1.6"
+version = "0.1.7"
 repository = "https://github.com/cospectrum/snake-opencv"
 description = "Snake case opencv with type annotations"
 license = "Apache-2.0"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "snake_opencv"}]
```

### Comparing `snake_opencv-0.1.6/snake_opencv/core/binding.py` & `snake_opencv-0.1.7/snake_opencv/core/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/core/const.py` & `snake_opencv-0.1.7/snake_opencv/core/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/dnn/binding.py` & `snake_opencv-0.1.7/snake_opencv/dnn/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/dnn/const.py` & `snake_opencv-0.1.7/snake_opencv/dnn/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/highgui/binding.py` & `snake_opencv-0.1.7/snake_opencv/highgui/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/highgui/const.py` & `snake_opencv-0.1.7/snake_opencv/highgui/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/imgcodecs/binding.py` & `snake_opencv-0.1.7/snake_opencv/imgcodecs/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/imgcodecs/const.py` & `snake_opencv-0.1.7/snake_opencv/imgcodecs/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/imgproc/binding.py` & `snake_opencv-0.1.7/snake_opencv/imgproc/binding.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     'get_rotation_matrix_2d',
     'median_blur',
     'blur',
     'bilateral_filter',
     'point_polygon_test',
     'contour_area',
     'convex_hull',
+    'approx_poly_dp',
+    'arc_length',
 ]
 
 
 LineType = Literal[-1, 4, 8, 16]
 
 Width = int
 Height = int
@@ -1282,7 +1284,47 @@
             vector: std::vector<int> implies returnPoints=false,
             std::vector<Point> implies returnPoints=true.
 
     Note: points and hull should be different arrays, inplace processing isn't
     supported.
     """
     return cv2.convexHull(points, hull, clockwise, return_points)  # type: ignore
+
+
+def arc_length(curve: np.ndarray, closed: bool) -> float:
+    """Calculates a contour perimeter or a curve length.
+
+    The function computes a curve length or a closed contour perimeter.
+
+    Args:
+        curve: Input vector of 2D points, stored in std::vector or Mat.
+        closed: Flag indicating whether the curve is closed or not.
+    """
+    return cv2.arcLength(curve, closed)  # type: ignore
+
+
+def approx_poly_dp(
+    curve: np.ndarray,
+    epsilon: float,
+    closed: bool,
+    approx_cruve: Optional[np.ndarray] = None,
+) -> np.ndarray:
+    """Approximates a polygonal curve(s) with the specified precision.
+
+    The function cv::approxPolyDP approximates a curve or a polygon with
+    another curve/polygon with less vertices so that the distance between them
+    is less or equal to the specified precision. It uses the Douglas-Peucker
+    algorithm http://en.wikipedia.org/wiki/Ramer-Douglas-Peucker_algorithm
+
+    Args:
+        curve: Input vector of a 2D point stored in std::vector or Mat
+        epsilon:
+            Parameter specifying the approximation accuracy. This is the
+            maximum distance between the original curve and its approximation.
+        closed:
+            If true, the approximated curve is closed (its first and last
+            vertices are connected). Otherwise, it is not closed.
+        approx_curve:
+            Result of the approximation. The type should match the type of the
+            input curve.
+    """
+    return cv2.approxPolyDP(curve, epsilon, closed, approx_cruve)  # type: ignore
```

### Comparing `snake_opencv-0.1.6/snake_opencv/imgproc/const.py` & `snake_opencv-0.1.7/snake_opencv/imgproc/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/photo/binding.py` & `snake_opencv-0.1.7/snake_opencv/photo/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/photo/const.py` & `snake_opencv-0.1.7/snake_opencv/photo/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/videoio/binding.py` & `snake_opencv-0.1.7/snake_opencv/videoio/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/snake_opencv/videoio/const.py` & `snake_opencv-0.1.7/snake_opencv/videoio/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.6/PKG-INFO` & `snake_opencv-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake-opencv
-Version: 0.1.6
+Version: 0.1.7
 Summary: Snake case opencv with type annotations
 Home-page: https://github.com/cospectrum/snake-opencv
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

