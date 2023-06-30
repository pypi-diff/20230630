# Comparing `tmp/pyRotd-0.6.0.tar.gz` & `tmp/pyRotd-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRotd-0.6.0.tar", last modified: Tue Jun 20 04:56:50 2023, max compression
+gzip compressed data, was "pyRotd-0.6.1.tar", last modified: Fri Jun 30 16:31:43 2023, max compression
```

## Comparing `pyRotd-0.6.0.tar` & `pyRotd-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:50.905299 pyRotd-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 04:56:39.000000 pyRotd-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-20 04:56:39.000000 pyRotd-0.6.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 04:56:39.000000 pyRotd-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-20 04:56:39.000000 pyRotd-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 04:56:39.000000 pyRotd-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-20 04:56:50.905299 pyRotd-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-20 04:56:39.000000 pyRotd-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:50.905299 pyRotd-0.6.0/pyRotd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:50.905299 pyRotd-0.6.0/pyrotd/
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-06-20 04:56:39.000000 pyRotd-0.6.0/pyrotd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 04:56:39.000000 pyRotd-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 04:56:50.905299 pyRotd-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-20 04:56:39.000000 pyRotd-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:50.905299 pyRotd-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:39.000000 pyRotd-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-20 04:56:39.000000 pyRotd-0.6.0/tests/test_osc_resp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-20 04:56:39.000000 pyRotd-0.6.0/tests/test_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:43.739389 pyRotd-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 16:31:33.000000 pyRotd-0.6.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-30 16:31:33.000000 pyRotd-0.6.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-30 16:31:33.000000 pyRotd-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-30 16:31:33.000000 pyRotd-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 16:31:33.000000 pyRotd-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-30 16:31:43.739389 pyRotd-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-30 16:31:33.000000 pyRotd-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:43.739389 pyRotd-0.6.1/pyRotd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-30 16:31:43.000000 pyRotd-0.6.1/pyRotd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-30 16:31:43.000000 pyRotd-0.6.1/pyRotd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:31:43.000000 pyRotd-0.6.1/pyRotd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 16:31:43.000000 pyRotd-0.6.1/pyRotd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 16:31:43.000000 pyRotd-0.6.1/pyRotd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:43.739389 pyRotd-0.6.1/pyrotd/
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-06-30 16:31:33.000000 pyRotd-0.6.1/pyrotd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 16:31:33.000000 pyRotd-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-30 16:31:43.739389 pyRotd-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-30 16:31:33.000000 pyRotd-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:43.739389 pyRotd-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:33.000000 pyRotd-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-30 16:31:33.000000 pyRotd-0.6.1/tests/test_osc_resp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-30 16:31:33.000000 pyRotd-0.6.1/tests/test_spectra.py
```

### Comparing `pyRotd-0.6.0/HISTORY.rst` & `pyRotd-0.6.1/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 History
 =======
 
+0.6.1 (2023-06-30)
+------------------
+- Tests np.version to accommodate change in keywords of np.percentile
+
 0.6.0 (2023-06-19)
 ------------------
 - Added optimization based on Stewart et al. (2017) algorithm
 - Added support for computing rotated PGA, PGV, and PGD
 
 0.5.4 (2018-07-27)
 ------------------
```

### Comparing `pyRotd-0.6.0/LICENSE` & `pyRotd-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRotd-0.6.0/LICENSE.txt` & `pyRotd-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyRotd-0.6.0/PKG-INFO` & `pyRotd-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRotd
-Version: 0.6.0
+Version: 0.6.1
 Summary: Rotated response spectrum calculation implemented in Python.
 Home-page: http://github.com/arkottke/pyrotd
 Author: Albert Kottke
 Author-email: albert.kottke@gmail.com
 License: MIT
 Keywords: response spectrum,earthquake ground motion
 Classifier: Development Status :: 4 - Beta
@@ -92,14 +92,18 @@
    :target: https://zenodo.org/badge/latestdoi/2800441
 
 
 
 History
 =======
 
+0.6.1 (2023-06-30)
+------------------
+- Tests np.version to accommodate change in keywords of np.percentile
+
 0.6.0 (2023-06-19)
 ------------------
 - Added optimization based on Stewart et al. (2017) algorithm
 - Added support for computing rotated PGA, PGV, and PGD
 
 0.5.4 (2018-07-27)
 ------------------
```

### Comparing `pyRotd-0.6.0/README.rst` & `pyRotd-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyRotd-0.6.0/pyRotd.egg-info/PKG-INFO` & `pyRotd-0.6.1/pyRotd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRotd
-Version: 0.6.0
+Version: 0.6.1
 Summary: Rotated response spectrum calculation implemented in Python.
 Home-page: http://github.com/arkottke/pyrotd
 Author: Albert Kottke
 Author-email: albert.kottke@gmail.com
 License: MIT
 Keywords: response spectrum,earthquake ground motion
 Classifier: Development Status :: 4 - Beta
@@ -92,14 +92,18 @@
    :target: https://zenodo.org/badge/latestdoi/2800441
 
 
 
 History
 =======
 
+0.6.1 (2023-06-30)
+------------------
+- Tests np.version to accommodate change in keywords of np.percentile
+
 0.6.0 (2023-06-19)
 ------------------
 - Added optimization based on Stewart et al. (2017) algorithm
 - Added support for computing rotated PGA, PGV, and PGD
 
 0.5.4 (2018-07-27)
 ------------------
```

### Comparing `pyRotd-0.6.0/pyrotd/__init__.py` & `pyRotd-0.6.1/pyrotd/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/python
 import sys
 
 import numpy as np
 from pkg_resources import get_distribution
+from numpy.lib import NumpyVersion
 
 if sys.version_info >= (3, 6):
     import functools
     import multiprocessing
 
     processes = max(multiprocessing.cpu_count() - 1, 1)
 else:
     processes = 1
 
 __author__ = "Albert Kottke"
-__copyright__ = "Copyright 2016-18 Albert Kottke"
+__copyright__ = "Copyright 2016-23 Albert Kottke"
 __license__ = "MIT"
 __title__ = "pyrotd"
 __version__ = get_distribution("pyrotd").version
 
 G_TO_CMPS = 980.665
 
 
@@ -145,16 +146,23 @@
     radians = np.radians(angles)
     coeffs = np.c_[np.cos(radians), np.sin(radians)]
     rotated_time_series = np.dot(coeffs, accels)
     # Sort this array based on the response
     peak_responses = np.abs(rotated_time_series).max(axis=1)
     rotated = np.rec.fromarrays([angles, peak_responses], names="angle,peak_resp")
     rotated.sort(order="peak_resp")
+
     # Get the peak response at the requested percentiles
-    p_peak_resps = np.percentile(rotated.peak_resp, percentiles, method="linear")
+    if NumpyVersion(np.__version__) < "1.22.0":
+        p_peak_resps = np.percentile(
+            rotated.peak_resp, percentiles, interpolation="linear"
+        )
+    else:
+        p_peak_resps = np.percentile(rotated.peak_resp, percentiles, method="linear")
+
     # Can only return the orientations for the minimum and maximum value as the
     # orientation is not unique (i.e., two values correspond to the 50%
     # percentile).
     p_angles = np.select(
         [np.isclose(percentiles, 0), np.isclose(percentiles, 100), True],
         [rotated.angle[0], rotated.angle[-1], np.nan],
     )
```

### Comparing `pyRotd-0.6.0/setup.py` & `pyRotd-0.6.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = fp.read()
 
 with open("HISTORY.rst") as fp:
     history = fp.read()
 
 setup(
     name="pyRotd",
-    version="0.6.0",
+    version="0.6.1",
     description="Rotated response spectrum calculation implemented in Python.",
     long_description=readme + "\n\n" + history,
     url="http://github.com/arkottke/pyrotd",
     author="Albert Kottke",
     author_email="albert.kottke@gmail.com",
     packages=find_packages(),
     install_requires=[
```

### Comparing `pyRotd-0.6.0/tests/test_osc_resp.py` & `pyRotd-0.6.1/tests/test_osc_resp.py`

 * *Files identical despite different names*

### Comparing `pyRotd-0.6.0/tests/test_spectra.py` & `pyRotd-0.6.1/tests/test_spectra.py`

 * *Files identical despite different names*

