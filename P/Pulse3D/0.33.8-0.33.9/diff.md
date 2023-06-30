# Comparing `tmp/Pulse3D-0.33.8.tar.gz` & `tmp/Pulse3D-0.33.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.8.tar", last modified: Fri Jun 16 17:10:06 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.9.tar", last modified: Fri Jun 30 00:55:26 2023, max compression
```

## Comparing `Pulse3D-0.33.8.tar` & `Pulse3D-0.33.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.077524 Pulse3D-0.33.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 17:10:06.081524 Pulse3D-0.33.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.069524 Pulse3D-0.33.8/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.065524 Pulse3D-0.33.8/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.073524 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-16 17:09:07.000000 Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-16 17:10:06.081524 Pulse3D-0.33.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.069524 Pulse3D-0.33.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.077524 Pulse3D-0.33.8/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 17:10:06.000000 Pulse3D-0.33.8/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-16 17:10:06.000000 Pulse3D-0.33.8/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:09:51.000000 Pulse3D-0.33.8/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.077524 Pulse3D-0.33.8/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-16 17:09:28.000000 Pulse3D-0.33.8/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:10:06.077524 Pulse3D-0.33.8/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/nb_peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33794 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-16 17:09:04.000000 Pulse3D-0.33.8/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:55:26.347187 Pulse3D-0.33.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-30 00:55:26.347187 Pulse3D-0.33.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:55:26.347187 Pulse3D-0.33.9/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-30 00:54:22.000000 Pulse3D-0.33.9/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:55:26.343187 Pulse3D-0.33.9/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:55:26.347187 Pulse3D-0.33.9/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 00:54:22.000000 Pulse3D-0.33.9/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-30 00:54:22.000000 Pulse3D-0.33.9/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 00:54:22.000000 Pulse3D-0.33.9/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-30 00:54:22.000000 Pulse3D-0.33.9/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-30 00:54:22.000000 Pulse3D-0.33.9/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 00:55:26.351187 Pulse3D-0.33.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:55:26.343187 Pulse3D-0.33.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:55:26.347187 Pulse3D-0.33.9/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-30 00:55:26.000000 Pulse3D-0.33.9/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-30 00:55:26.000000 Pulse3D-0.33.9/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:55:10.000000 Pulse3D-0.33.9/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:55:26.347187 Pulse3D-0.33.9/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 00:54:46.000000 Pulse3D-0.33.9/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-30 00:54:46.000000 Pulse3D-0.33.9/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 00:54:46.000000 Pulse3D-0.33.9/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-30 00:54:46.000000 Pulse3D-0.33.9/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-30 00:54:46.000000 Pulse3D-0.33.9/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:55:26.347187 Pulse3D-0.33.9/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18562 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49386 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/nb_peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33376 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-30 00:54:17.000000 Pulse3D-0.33.9/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.8/LICENSE` & `Pulse3D-0.33.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/PKG-INFO` & `Pulse3D-0.33.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.8
+Version: 0.33.9
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.8/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.9/mantarray-magnet-finding/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 """Setup configuration."""
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name="mantarray_magnet_finding",
-    version="0.5.2",
+    version="0.5.1",
     description="Magnet Finding",
     url="https://github.com/CuriBio/mantarray-magnet-finding",
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
         "nptyping==1.4.4",
         "numpy==1.23.4",  # Tanner (12/3/21): pinned for numba compatibility
         "scipy==1.9.3",
-        "numba==0.57.0",
+        "numba==0.56.4",
         "stdlib_utils>=0.4.4",
         "labware-domain-models>=0.3.1",
         "h5py>=3.7.0",
         "immutabledict>=2.2.1",
     ],
     zip_safe=False,
     include_package_data=True,
@@ -31,14 +31,13 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 )
```

### Comparing `Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.9/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.9/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/setup.py` & `Pulse3D-0.33.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.8",
+    version="0.33.9",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.8/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.9/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.8
+Version: 0.33.9
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.8/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.9/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.9/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.9/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.9/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/constants.py` & `Pulse3D-0.33.9/src/pulse3D/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     from importlib import metadata
 except ImportError:  # pragma: no cover
     import importlib_metadata as metadata  # type: ignore
 PACKAGE_VERSION = metadata.version("pulse3D")
 
 TWENTY_FOUR_WELL_PLATE = LabwareDefinition(row_count=4, column_count=6)
 
-
 NUM_CHANNELS_24_WELL_PLATE = 24 * NUM_CHANNELS_PER_WELL
 
 MIN_SUPPORTED_FILE_VERSION = "0.1.1"
 CURRENT_BETA1_HDF5_FILE_FORMAT_VERSION = "0.4.2"
 CURRENT_BETA2_HDF5_FILE_FORMAT_VERSION = "1.0.0"
 FILE_FORMAT_VERSION_METADATA_KEY = "File Format Version"
 FILE_MIGRATION_PATHS = immutabledict({"0.3.1": "0.4.1", "0.4.1": "0.4.2"})
@@ -204,14 +203,26 @@
 DEFAULT_NB_RELATIVE_PROMINENCE_FACTOR = 0.2
 DEFAULT_NB_WIDTH_FACTORS = (0, 5)
 DEFAULT_NB_HEIGHT_FACTOR = 0
 DEFAULT_NB_VALLEY_SEARCH_DUR = 1
 DEFAULT_NB_UPSLOPE_DUR = 0.07
 DEFAULT_NB_UPSLOPE_NOISE_ALLOWANCE_DUR = 0.01
 
+DEFAULT_NB_PARAMS = immutabledict(
+    {
+        DEFAULT_NB_NOISE_PROMINENCE_FACTOR: "Noise Prominence Factor",
+        DEFAULT_NB_RELATIVE_PROMINENCE_FACTOR: "Relative Prominence Factor",
+        DEFAULT_NB_WIDTH_FACTORS: "Width Factor",
+        DEFAULT_NB_HEIGHT_FACTOR: "Height Factor",
+        DEFAULT_NB_VALLEY_SEARCH_DUR: "Valley Search Duration",
+        DEFAULT_NB_UPSLOPE_DUR: "Upslope Duration",
+        DEFAULT_NB_UPSLOPE_NOISE_ALLOWANCE_DUR: "Upslope Noise Allowance Duration",
+    }
+)
+
 # twitch indices keys
 PRIOR_PEAK_INDEX_UUID = uuid.UUID("80df90dc-21f8-4cad-a164-89436909b30a")
 PRIOR_VALLEY_INDEX_UUID = uuid.UUID("72ba9466-c203-41b6-ac30-337b4a17a124")
 SUBSEQUENT_PEAK_INDEX_UUID = uuid.UUID("7e37325b-6681-4623-b192-39f154350f36")
 SUBSEQUENT_VALLEY_INDEX_UUID = uuid.UUID("fd47ba6b-ee4d-4674-9a89-56e0db7f3d97")
 
 # filters
@@ -303,16 +314,14 @@
 
 STIM_CHART_HEIGHT_CELLS = CHART_HEIGHT_CELLS - 2
 STIM_CHART_HEIGHT = DEFAULT_CELL_HEIGHT * STIM_CHART_HEIGHT_CELLS
 
 CHART_FIXED_WIDTH_CELLS = 8
 CHART_FIXED_WIDTH = DEFAULT_CELL_WIDTH * CHART_FIXED_WIDTH_CELLS
 
-PEAK_VALLEY_COLUMN_START = 100
-STIM_DATA_COLUMN_START = 200
 SECONDS_PER_CELL = 2.5
 
 CALCULATED_METRIC_DISPLAY_NAMES = {
     TWITCH_PERIOD_UUID: "Twitch Period (seconds)",
     TWITCH_FREQUENCY_UUID: "Twitch Frequency (Hz)",
     AMPLITUDE_UUID: "Active Twitch Force (μN)",
     FRACTION_MAX_UUID: "Fraction of Maximum Active Twitch Force (μN)",
```

### Comparing `Pulse3D-0.33.8/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.9/src/pulse3D/excel_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
+from labware_domain_models import get_row_and_column_from_well_name
 import numpy as np
 import pandas as pd
 from scipy import interpolate
 
 from .constants import *
 from .exceptions import *
 from .metrics import WellGroupMetric
@@ -44,33 +45,35 @@
     well_index: int,
     well_name: str,
     indices,
     tissue_data,
     detector_type: str,
     continuous_waveform_sheet,
     waveform_charts,
+    peak_valley_start_col: int,
 ) -> None:
     if detector_type == "Valley":
         label = "Relaxation"
         offset = 1
         marker_color = "#D95F02"
     else:
         label = "Contraction"
         offset = 0
         marker_color = "#7570B3"
 
-    result_column = xl_col_to_name(PEAK_VALLEY_COLUMN_START + (well_index * 2) + offset)
+    result_column = xl_col_to_name(peak_valley_start_col + (well_index * 2) + offset)
     continuous_waveform_sheet.write(f"{result_column}1", f"{well_name} {detector_type} Values")
 
     for idx in indices:
         # we can use the peak/valley indices directly because we are using the interpolated data
         row = idx + 2
         continuous_waveform_sheet.write(f"{result_column}{row}", tissue_data[1, idx])
 
     upper_x_bound_cell = tissue_data.shape[1]
+
     for chart in waveform_charts:
         chart.add_series(
             {
                 "name": label,
                 "categories": f"='continuous-waveforms'!$A$2:$A${upper_x_bound_cell}",
                 "values": f"='continuous-waveforms'!${result_column}$2:${result_column}${upper_x_bound_cell}",
                 "marker": {
@@ -81,18 +84,25 @@
                 },
                 "line": {"none": True},
             }
         )
 
 
 def add_stim_data_series(
-    charts, format, charge_unit, col_offset: int, series_label: str, upper_x_bound_cell: int, y_axis_bounds
+    charts,
+    format,
+    charge_unit,
+    col_offset: int,
+    series_label: str,
+    upper_x_bound_cell: int,
+    y_axis_bounds,
+    stim_data_start_col,
 ) -> None:
-    stim_timepoints_col = xl_col_to_name(STIM_DATA_COLUMN_START)
-    stim_session_col = xl_col_to_name(STIM_DATA_COLUMN_START + col_offset)
+    stim_timepoints_col = xl_col_to_name(stim_data_start_col)
+    stim_session_col = xl_col_to_name(stim_data_start_col + col_offset)
 
     series_params: Dict[str, Any] = {
         "name": series_label,
         "categories": f"='continuous-waveforms'!${stim_timepoints_col}$2:${stim_timepoints_col}${upper_x_bound_cell}",
         "values": f"='continuous-waveforms'!${stim_session_col}$2:${stim_session_col}${upper_x_bound_cell}",
         "line": {"color": "#d1d128"},
     }
@@ -113,22 +123,24 @@
 def create_force_frequency_relationship_charts(
     force_frequency_sheet,
     force_frequency_chart,
     well_index: int,
     well_name: str,
     num_data_points: int,
     num_per_twitch_metrics: int,
+    well_row: int,
+    well_col: int,
 ) -> None:
-    well_row = well_index * num_per_twitch_metrics
+    row = well_index * num_per_twitch_metrics
     last_column = xl_col_to_name(num_data_points)
 
     force_frequency_chart.add_series(
         {
-            "categories": f"='{PER_TWITCH_METRICS_SHEET_NAME}'!$B${well_row + 7}:${last_column}${well_row + 7}",
-            "values": f"='{PER_TWITCH_METRICS_SHEET_NAME}'!$B${well_row + 5}:${last_column}${well_row + 5}",
+            "categories": f"='{PER_TWITCH_METRICS_SHEET_NAME}'!$B${row + 7}:${last_column}${row + 7}",
+            "values": f"='{PER_TWITCH_METRICS_SHEET_NAME}'!$B${row + 5}:${last_column}${row + 5}",
             "marker": {"type": "diamond", "size": 7},
             "line": {"none": True},
         }
     )
 
     force_frequency_chart.set_legend({"none": True})
     x_axis_label = CALCULATED_METRIC_DISPLAY_NAMES[TWITCH_FREQUENCY_UUID]
@@ -136,29 +148,29 @@
     force_frequency_chart.set_x_axis({"name": x_axis_label})
     y_axis_label = CALCULATED_METRIC_DISPLAY_NAMES[AMPLITUDE_UUID]
 
     force_frequency_chart.set_y_axis({"name": y_axis_label, "major_gridlines": {"visible": 0}})
     force_frequency_chart.set_size({"width": CHART_FIXED_WIDTH, "height": CHART_HEIGHT})
     force_frequency_chart.set_title({"name": f"Well {well_name}"})
 
-    well_row, well_col = TWENTY_FOUR_WELL_PLATE.get_row_and_column_from_well_index(well_index)
-
     force_frequency_sheet.insert_chart(
         1 + well_row * (CHART_HEIGHT_CELLS + 1),
         1 + well_col * (CHART_FIXED_WIDTH_CELLS + 1),
         force_frequency_chart,
     )
 
 
 def create_frequency_vs_time_charts(
     frequency_chart_sheet,
     frequency_chart,
     well_info: Dict[str, Any],
     num_data_points: int,
     num_per_twitch_metrics,
+    well_row: int,
+    well_col: int,
 ) -> None:
     well_index = well_info["well_index"]
 
     row = well_index * num_per_twitch_metrics
     last_column = xl_col_to_name(num_data_points)
 
     frequency_chart.add_series(
@@ -183,23 +195,22 @@
     y_axis_label = CALCULATED_METRIC_DISPLAY_NAMES[TWITCH_FREQUENCY_UUID]
 
     frequency_chart.set_y_axis({"name": y_axis_label, "min": 0, "major_gridlines": {"visible": 0}})
 
     frequency_chart.set_size({"width": CHART_FIXED_WIDTH, "height": CHART_HEIGHT})
     frequency_chart.set_title({"name": f"Well {well_info['well_name']}"})
 
-    well_row, well_col = TWENTY_FOUR_WELL_PLATE.get_row_and_column_from_well_index(well_index)
-
     frequency_chart_sheet.insert_chart(
         1 + well_row * (CHART_HEIGHT_CELLS + 1), 1 + well_col * (CHART_FIXED_WIDTH_CELLS + 1), frequency_chart
     )
 
 
 def write_xlsx(
     plate_recording: PlateRecording,
+    output_dir: Optional[str] = None,
     normalize_y_axis: bool = True,
     max_y: Union[int, float] = None,
     start_time: Union[float, int] = 0,
     end_time: Union[float, int] = np.inf,
     twitch_widths: Tuple[int, ...] = DEFAULT_TWITCH_WIDTHS,
     baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS,
     noise_prominence_factor: Union[int, float] = DEFAULT_NB_NOISE_PROMINENCE_FACTOR,
@@ -272,36 +283,61 @@
     if end_time <= start_time:
         raise ValueError("Window end time must be greater than window start time")
 
     end_time = min(end_time, max_final_time_secs)
     is_full_analysis = start_time == 0 and end_time == max_final_time_secs
 
     # create output file name
+    if output_dir is None:
+        output_dir = os.getcwd()
+
     input_file_name_no_ext = os.path.splitext(os.path.basename(plate_recording.path))[0]
     file_suffix = "full" if is_full_analysis else f"{start_time}-{end_time}"
-    output_file_name = f"{input_file_name_no_ext}_{file_suffix}.xlsx"
+    output_file_path = os.path.join(output_dir, f"{input_file_name_no_ext}_{file_suffix}.xlsx")
 
     if plate_recording.is_optical_recording:
         post_stiffness_factor_label = NOT_APPLICABLE_LABEL
     elif first_wf.stiffness_override:
         # reverse dict to use the stiffness factor as a key and get the label value
         post_stiffness_factor_label = {v: k for k, v in POST_STIFFNESS_LABEL_TO_FACTOR.items()}[
             first_wf.stiffness_factor
         ]
     else:
         post_stiffness_factor_label = get_stiffness_label(get_experiment_id(first_wf[PLATE_BARCODE_UUID]))
 
-    stim_barcode_display = first_wf.get(STIM_BARCODE_UUID)
-    if stim_barcode_display is None or stim_barcode_display == str(NOT_APPLICABLE_H5_METADATA):
-        stim_barcode_display = NOT_APPLICABLE_LABEL
+    stim_barcode_display = NOT_APPLICABLE_LABEL
+    if plate_recording.contains_stim_data and (
+        (stim_barcode := first_wf.get(STIM_BARCODE_UUID)) not in (None, str(NOT_APPLICABLE_H5_METADATA))
+    ):
+        stim_barcode_display = stim_barcode
 
     platemap_label_display_rows = [
         ("", label, ", ".join(well_names)) for label, well_names in plate_recording.platemap_labels.items()
     ]
 
+    peak_finding_params_to_compare = {
+        DEFAULT_NB_NOISE_PROMINENCE_FACTOR: noise_prominence_factor,
+        DEFAULT_NB_RELATIVE_PROMINENCE_FACTOR: relative_prominence_factor,
+        DEFAULT_NB_WIDTH_FACTORS: width_factors,
+        DEFAULT_NB_HEIGHT_FACTOR: height_factor,
+        DEFAULT_NB_VALLEY_SEARCH_DUR: valley_search_duration,
+        DEFAULT_NB_UPSLOPE_DUR: upslope_duration,
+        DEFAULT_NB_UPSLOPE_NOISE_ALLOWANCE_DUR: upslope_noise_allowance_duration,
+    }
+
+    peak_finding_display_rows = [
+        ("", DEFAULT_NB_PARAMS[default_val], str(given_val))
+        for default_val, given_val in peak_finding_params_to_compare.items()
+        if default_val != given_val
+    ]
+
+    # only add this section header if necessary
+    if len(peak_finding_display_rows) > 0:
+        peak_finding_display_rows.insert(0, ("User-defined Peak Finding Params:", "", ""))
+
     # create metadata sheet format as DataFrame
     metadata_rows = [
         ("Recording Information:", "", ""),
         ("", "Plate Barcode", first_wf[PLATE_BARCODE_UUID]),
         ("", "Stimulation Lid Barcode", stim_barcode_display),
         (
             "",
@@ -319,45 +355,46 @@
         ("", "Firmware Version (Main Controller)", first_wf.get(MAIN_FIRMWARE_VERSION_UUID, "")),
         ("Output Format:", "", ""),
         ("", "Pulse3D Version", PACKAGE_VERSION),
         ("", "File Creation Timestamp", str(datetime.datetime.utcnow().replace(microsecond=0))),
         ("", "Analysis Type (Full or Windowed)", "Full" if is_full_analysis else "Windowed"),
         ("", "Analysis Start Time (seconds)", f"{start_time:.1f}"),
         ("", "Analysis End Time (seconds)", f"{end_time:.1f}"),
+        *peak_finding_display_rows,
     ]
+
     metadata_df = pd.DataFrame(
         {col: [row[i] for row in metadata_rows] for i, col in enumerate(("A", "B", "C"))}
     )
 
     twitch_width_percents = tuple(
         sorted(
             set([*twitch_widths, *(100 - np.array(twitch_widths, dtype=int)), *DEFAULT_TWITCH_WIDTH_PERCENTS])
         )
     )
 
     log.info("Computing data metrics for each well.")
 
     recording_plotting_info = []
     max_force_of_recording = 0
-    for well_file in plate_recording:
+    for well_index, well_file in enumerate(plate_recording):
         # initialize some data structures
         error_msg = None
 
         # necessary for concatenating DFs together, in event that peak-finding fails and produces empty DF
         dfs = init_dfs(twitch_widths_range=twitch_width_percents)
         metrics = tuple(
             concat([dfs[k][j] for j in dfs[k].keys()], axis=1) for k in ("per_twitch", "aggregate")
         )
         peaks_and_valleys = (np.array([]), np.array([]))
 
         if well_file is None:
             continue
 
-        well_index = well_file[WELL_INDEX_UUID]
-        well_name = TWENTY_FOUR_WELL_PLATE.get_well_name_from_well_index(well_index)
+        well_name = well_file[WELL_NAME_UUID]
 
         # find bounding indices with respect to well recording
         well_start_idx, well_end_idx = truncate(
             source_series=interpolated_timepoints_us,
             lower_bound=well_file.force[0][0],
             upper_bound=well_file.force[0][-1],
         )
@@ -435,15 +472,15 @@
             error_msg = "Not Enough Twitches Detected"
 
         # the rest of the code will expect time to be in seconds, so convert here
         interpolated_well_data[0] /= MICRO_TO_BASE_CONVERSION
 
         well_info = {
             "well_index": well_index,
-            "well_name": TWENTY_FOUR_WELL_PLATE.get_well_name_from_well_index(well_index),
+            "well_name": well_name,
             "platemap_label": well_file[PLATEMAP_LABEL_UUID],
             "tissue_data": interpolated_well_data,
             "peaks_and_valleys": peaks_and_valleys,
             "metrics": metrics,
         }
         if error_msg:
             well_info["error_msg"] = error_msg
@@ -471,29 +508,29 @@
     y_axis_bounds = {"tissue": {"max": max_y, "min": 0}}
 
     stim_plotting_info: Dict[str, Any] = _get_stim_plotting_data(
         plate_recording, start_time, end_time, stim_waveform_format, normalize_y_axis, y_axis_bounds
     )
 
     _write_xlsx(
-        output_file_name=output_file_name,
+        output_file_path=output_file_path,
         metadata_df=metadata_df,
         continuous_waveforms_df=continuous_waveforms_df,
         stim_protocols_df=stim_protocols_df,
         stim_plotting_info=stim_plotting_info,
         recording_plotting_info=recording_plotting_info,
         y_axis_bounds=y_axis_bounds,
         include_stim_protocols=include_stim_protocols,
         twitch_widths=twitch_widths,
         baseline_widths_to_use=baseline_widths_to_use,
         group_metrics_list=group_metrics_list,
     )
 
     log.info("Done")
-    return output_file_name
+    return output_file_path
 
 
 def _create_stim_protocols_df(plate_recording):
     unassigned_wells = []
     stim_protocols_dict = {
         "Title": {
             "Unassigned Wells": "Unassigned Wells:",
@@ -560,16 +597,16 @@
 
     start_time_us = int(start_time * MICRO_TO_BASE_CONVERSION)
     end_time_us = int(end_time * MICRO_TO_BASE_CONVERSION)
 
     # insert this first since dict insertion order matters for the data frame creation
     stim_waveforms_dict = {"Stim Time (seconds)": None}
 
-    for well_idx, wf in enumerate(plate_recording):
-        well_name = TWENTY_FOUR_WELL_PLATE.get_well_name_from_well_index(well_idx)
+    for wf in plate_recording:
+        well_name = wf[WELL_NAME_UUID]
 
         if not wf.stim_sessions:
             continue
 
         stim_protocol = json.loads(wf[STIMULATION_PROTOCOL_UUID])
 
         charge_units[well_name] = "mA" if stim_protocol["stimulation_type"] == "C" else "mV"
@@ -611,90 +648,118 @@
         "chart_format": stim_waveform_format,
         "charge_units": charge_units,
         "stim_waveform_df": stim_waveform_df,
     }
 
 
 def _write_xlsx(
-    output_file_name: str,
+    output_file_path: str,
     metadata_df: pd.DataFrame,
     continuous_waveforms_df: pd.DataFrame,
     stim_protocols_df: pd.DataFrame,
     stim_plotting_info: Dict[str, Any],
     recording_plotting_info: List[Dict[Any, Any]],
     y_axis_bounds: Dict[str, Dict[str, Any]],
     include_stim_protocols: bool = False,
     twitch_widths: Tuple[int, ...] = DEFAULT_TWITCH_WIDTHS,
     baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS,
     group_metrics_list: List[Dict[str, Any]] = [],
 ):
-    log.info(f"Writing {output_file_name}")
-    with pd.ExcelWriter(output_file_name) as writer:
+    log.info(f"Writing {output_file_path}")
+    with pd.ExcelWriter(output_file_path) as writer:
         _write_metadata(writer, metadata_df)
 
         if include_stim_protocols:
             _write_stim_protocols(writer, stim_protocols_df)
 
         continuous_waveforms_sheet = _write_continuous_waveforms(writer, continuous_waveforms_df)
 
         if stim_plotting_info:
-            _write_stim_waveforms(writer, stim_plotting_info["stim_waveform_df"])
+            # multiply by 3 to account for as many peak and valley columns for each well
+            # 100 to offset between peak/valley columns and stim data
+            stim_data_start_col = len(list(continuous_waveforms_df)) * 3 + 100
+            _write_stim_waveforms(writer, stim_plotting_info["stim_waveform_df"], stim_data_start_col)
+
+        # this is used to check if a couple xlsx files are being analyzed, could be more exact and check for 24/96/384
+        # but without this, the snapshot, time-force, and twitch-freq charts have a ton of white space calculating row/column
+        is_complete_plate_recording = len(recording_plotting_info) >= 24
 
         # waveform snapshot/full
         wb = writer.book
         snapshot_sheet = wb.add_worksheet("continuous-waveform-snapshot")
         full_sheet = wb.add_worksheet("full-continuous-waveform-plots")
+
         for rec_info_idx, well_info in enumerate(recording_plotting_info):
+            well_row, well_col = _get_row_and_column_for_well(
+                well_info["well_name"], is_complete_plate_recording, rec_info_idx
+            )
+
             log.info(f'Creating waveform charts for well {well_info["well_name"]}')
             create_waveform_charts(
                 y_axis_bounds,
                 well_info,
                 continuous_waveforms_df,
                 wb,
                 continuous_waveforms_sheet,
                 snapshot_sheet,
                 full_sheet,
                 stim_plotting_info,
                 rec_info_idx,  # used to remove whitespace in full-continuous-waveform-plots
+                well_row,
+                well_col,
             )
 
         _write_aggregate_metrics(
             writer, recording_plotting_info, twitch_widths, baseline_widths_to_use, group_metrics_list
         )
 
         num_metrics = _write_per_twitch_metrics(
             writer, recording_plotting_info, twitch_widths, baseline_widths_to_use
         )
 
         # freq/force charts
         force_freq_sheet = wb.add_worksheet(FORCE_FREQUENCY_RELATIONSHIP_SHEET)
         freq_vs_time_sheet = wb.add_worksheet(TWITCH_FREQUENCIES_CHART_SHEET_NAME)
 
-        for well_info in recording_plotting_info:
+        for rec_info_idx, well_info in enumerate(recording_plotting_info):
             well_metrics = well_info["metrics"]
+
             if not well_metrics:
                 continue
+
             num_data_points = len(well_metrics[0])
 
             force_freq_chart = wb.add_chart({"type": "scatter", "subtype": "straight"})
             freq_vs_time_chart = wb.add_chart({"type": "scatter", "subtype": "straight"})
 
+            well_row, well_col = _get_row_and_column_for_well(
+                well_info["well_name"], is_complete_plate_recording, rec_info_idx
+            )
+
             log.info(f"Creating frequency vs time chart for well {well_info['well_name']}")
             create_frequency_vs_time_charts(
-                freq_vs_time_sheet, freq_vs_time_chart, well_info, num_data_points, num_metrics
+                freq_vs_time_sheet,
+                freq_vs_time_chart,
+                well_info,
+                num_data_points,
+                num_metrics,
+                well_row,
+                well_col,
             )
 
             log.info(f"Creating force frequency relationship chart for well {well_info['well_name']}")
             create_force_frequency_relationship_charts(
                 force_freq_sheet,
                 force_freq_chart,
                 well_info["well_index"],
                 well_info["well_name"],
                 num_data_points,  # number of twitches
                 num_metrics,
+                well_row,
+                well_col,
             )
 
         log.info("Saving file")
 
 
 def _write_metadata(writer, metadata_df):
     log.info("Writing H5 file metadata")
@@ -739,18 +804,18 @@
 
     for iter_well_idx in range(1, 24):
         continuous_waveforms_sheet.set_column(iter_well_idx, iter_well_idx, 13)
 
     return continuous_waveforms_sheet
 
 
-def _write_stim_waveforms(writer, stim_waveform_df):
+def _write_stim_waveforms(writer, stim_waveform_df, stim_data_start_col):
     log.info("Writing stim data")
     stim_waveform_df.to_excel(
-        writer, sheet_name="continuous-waveforms", index=False, startcol=STIM_DATA_COLUMN_START
+        writer, sheet_name="continuous-waveforms", index=False, startcol=stim_data_start_col
     )
 
 
 def _write_aggregate_metrics(
     writer, recording_plotting_info, twitch_widths, baseline_widths_to_use, group_metrics_list
 ):
     log.info("Writing aggregate metrics.")
@@ -773,14 +838,16 @@
     continuous_waveforms_df,
     wb,
     continuous_waveforms_sheet,
     snapshot_sheet,
     full_sheet,
     stim_plotting_info,
     rec_info_idx,
+    well_row,
+    well_col,
 ):
     well_idx = well_info["well_index"]
     well_name = well_info["well_name"]
 
     # maximum snapshot size is 10 seconds
     snapshot_lower_x_bound = well_info["tissue_data"][0, 0]
     snapshot_upper_x_bound = min(
@@ -887,39 +954,45 @@
 
         stim_waveform_df = stim_plotting_info["stim_waveform_df"]
         for col_idx, col_title in enumerate(stim_waveform_df):
             if not col_title.startswith(well_name):
                 continue
 
             series_label = col_title.split("-")[-1].strip()
+            # multiply by 3 to account for as many peak and valley columns for each well
+            # 100 to offset between peak/valley columns and stim data
+            stim_data_start_col = len(list(continuous_waveforms_df)) * 3 + 100
             add_stim_data_series(
                 charts=[chart],
                 format=stim_chart_format,
                 charge_unit=stim_plotting_info["charge_units"][well_name],
                 col_offset=col_idx,
                 series_label=series_label,
                 upper_x_bound_cell=len(stim_waveform_df["Stim Time (seconds)"]),
                 y_axis_bounds=y_axis_bounds["stim"],
+                stim_data_start_col=stim_data_start_col,
             )
 
     peaks, valleys = well_info["peaks_and_valleys"]
     log.info(f"Adding peak detection series for well {well_name}")
 
     for detector_type, indices in [("Peak", peaks), ("Valley", valleys)]:
+        # offset by 50 to make it less obvious to users
+        peak_valley_start_col = len(list(continuous_waveforms_df)) + 50
         add_peak_detection_series(
             well_index=well_idx,
             well_name=well_name,
             indices=indices,
             tissue_data=well_info["tissue_data"],
             detector_type=detector_type,
             continuous_waveform_sheet=continuous_waveforms_sheet,
             waveform_charts=[snapshot_chart, full_chart],
+            peak_valley_start_col=peak_valley_start_col,
         )
 
-    well_row, well_col = TWENTY_FOUR_WELL_PLATE.get_row_and_column_from_well_index(df_column - 1)
     snapshot_sheet.insert_chart(
         well_row * (CHART_HEIGHT_CELLS + 1), well_col * (CHART_FIXED_WIDTH_CELLS + 1), snapshot_chart
     )
 
     cells_per_well = CHART_HEIGHT_CELLS + 1
     if stim_chart_format == "stacked":
         cells_per_well += STIM_CHART_HEIGHT_CELLS
@@ -1109,7 +1182,18 @@
 
         concat_aggregate_df = concat(
             [aggregate_dfs[metric_type] for metric_type in aggregate_dfs.keys()], axis=1
         )
         all_group_metrics.append({"name": label, "metrics": concat_aggregate_df})
 
     return all_group_metrics
+
+
+def _get_row_and_column_for_well(
+    well_name: str, is_complete_recording: bool, rec_info_idx: int
+) -> Tuple[int, int]:
+    # used to remove whitespace in snapshot, force frequency, and twitch-frequency sheets if only a few xlsx files were given
+    return (
+        get_row_and_column_from_well_name(well_name)
+        if is_complete_recording
+        else TWENTY_FOUR_WELL_PLATE.get_row_and_column_from_well_index(rec_info_idx)
+    )
```

### Comparing `Pulse3D-0.33.8/src/pulse3D/exceptions.py` & `Pulse3D-0.33.9/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.9/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/metrics.py` & `Pulse3D-0.33.9/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/nb_peak_detection.py` & `Pulse3D-0.33.9/src/pulse3D/nb_peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.9/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.9/src/pulse3D/plate_recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 
         if stiffness_factor not in (*POST_STIFFNESS_OVERRIDE_OPTIONS, None):
             raise ValueError(
                 f"Invalid Post Stiffness {stiffness_factor}, must be in {POST_STIFFNESS_OVERRIDE_OPTIONS}"
             )
 
         self.has_inverted_post_magnet = has_inverted_post_magnet
-
         self.stiffness_override = stiffness_factor is not None
 
         if file_path.endswith(".h5"):
             self.is_force_data = True
             self.is_magnetic_data = True
 
             self._load_data_from_h5_file(file_path)
@@ -105,15 +104,15 @@
             )
 
             if self.stiffness_override:
                 self.stiffness_factor = stiffness_factor
             elif not self.get(IS_CALIBRATION_FILE_UUID, False):
                 # earlier versions of files do not have the IS_CALIBRATION_FILE_UUID in their metadata
                 experiment_id = get_experiment_id(self[PLATE_BARCODE_UUID])
-                self.stiffness_factor = get_stiffness_factor(experiment_id, self[WELL_INDEX_UUID])
+                self.stiffness_factor = get_stiffness_factor(experiment_id, self[WELL_NAME_UUID])
             else:
                 # calibration recordings do not have an associated barcode or post stiffness since they
                 # are creatd when a plate is not even on the istrument, so just set the stiffness factor to 1
                 self.stiffness_factor = CALIBRATION_STIFFNESS_FACTOR
 
             if self.version < VersionInfo.parse("1.0.0"):  # type: ignore
                 # Ref data not yet added to Beta 2 files
@@ -158,25 +157,25 @@
             self.attrs = {k: v for k, v in _load_optical_file_attrs(self._excel_sheet).items()}
             self.version = self[FILE_FORMAT_VERSION_METADATA_KEY]
             self.is_magnetic_data = False
             self.is_force_data = (
                 "y" in str(_get_excel_metadata_value(self._excel_sheet, TWITCHES_POINT_UP_UUID)).lower()
             )
             self.stiffness_factor = None
+
             for uuid_ in (PLATEMAP_NAME_UUID, PLATEMAP_LABEL_UUID):
                 self[uuid_] = NOT_APPLICABLE_LABEL
             # skip all other transforms
             self.force = self[TISSUE_SENSOR_READINGS].copy()
             # timepoints still need to be in µs
             self.force[0] *= MICRO_TO_BASE_CONVERSION
 
     def _load_data_from_h5_file(self, file_path: str) -> None:
         with h5py.File(file_path, "r") as h5_file:
             self.file_name = os.path.basename(h5_file.filename)
-
             self.attrs = {attr: h5_file.attrs[attr] for attr in list(h5_file.attrs)}
             self.version = self[FILE_FORMAT_VERSION_METADATA_KEY]
 
             if self.version < VersionInfo.parse("1.0.0"):
                 # load sensor data. This is only possible to do here for Beta 1 data files
                 self[TISSUE_SENSOR_READINGS] = self._load_reading(h5_file, TISSUE_SENSOR_READINGS)
                 self[REFERENCE_SENSOR_READINGS] = self._load_reading(h5_file, REFERENCE_SENSOR_READINGS)
@@ -336,16 +335,17 @@
         stiffness_factor: Optional[int] = None,
         inverted_post_magnet_wells: Optional[List[str]] = None,
         well_groups: Optional[Dict[str, List[str]]] = None,
     ):
         self.path = path
         self.wells = []
         self._iter = 0
-        # this may get overwritten later
+        # these may get overwritten later
         self.is_optical_recording = False
+        self.contains_stim_data = False
 
         # Tanner (11/16/22): due to the needs of the scientists for the full analysis,
         # these params should only be used in the recording snapshot.
         # These params also have no effect on Beta 1 data.
         if start_time < 0:
             raise ValueError("'start_time' must be >= 0")
         if end_time and start_time >= end_time:
@@ -373,14 +373,20 @@
                 self.path, stiffness_factor, inverted_post_magnet_wells
             )
 
         # make sure at least one WellFile was loaded
         if not any(self.wells):
             raise NoRecordingFilesLoadedError()
 
+        if len(self.wells) > len(set(w[WELL_NAME_UUID] for w in self.wells)):
+            raise DuplicateWellsFoundError()
+
+        # ensure wells are in correct order A1, B1,.., A2, B2,...
+        self.wells.sort(key=lambda w: (int(w[WELL_NAME_UUID][1:]), w[WELL_NAME_UUID][0]))
+
         # set up platemap info
         first_avaliable_well = next(iter(self))
         self.platemap_name = first_avaliable_well[PLATEMAP_NAME_UUID]
         platemap_labels = defaultdict(list)
 
         for well_file in self:
             if well_groups is None:
@@ -406,14 +412,16 @@
                 self._process_plate_data(calibration_recordings)
 
                 if self.wells[0][FILE_FORMAT_VERSION_METADATA_KEY] >= VersionInfo.parse(
                     MIN_FILE_VERSION_FOR_STIM_INTERPOLATION
                 ):
                     self._process_stim_data()
 
+            self.contains_stim_data = any(wf.stim_sessions for wf in self)
+
     def _process_plate_data(self, calibration_recordings):
         if not all(isinstance(well_file, WellFile) for well_file in self.wells) or len(self.wells) != 24:
             raise NotImplementedError("All 24 wells must have a recording file present")
 
         if (
             not all(isinstance(well_file, WellFile) for well_file in calibration_recordings)
             or len(calibration_recordings) != 24
@@ -530,31 +538,24 @@
             for col_title in stim_col_titles:
                 stim_session_raw = np.array([stim_timepoints, df[col_title]])
                 stim_session = stim_session_raw[:, ~np.isnan(stim_session_raw[1])].astype(int)
                 wf.stim_sessions.append(stim_session)
 
     def _load_optical_well_files(self, file_paths: List[str], stiffness_factor: Union[int, None]):
         self.is_optical_recording = True
-        if not self.wells:
-            # TODO parameterize number of wells here, set to 24 max for now
-            self.wells = [None] * 24
 
         for xlsx_path in file_paths:
             # check if xlsx is correct format and not pulse3d output file
             if _get_num_of_sheets(xlsx_path) > 1:
                 raise IncorrectOpticalFileFormatError(
                     f"Incorrect number of sheets found for file {os.path.basename(xlsx_path)}"
                 )
 
             well_file = WellFile(xlsx_path, stiffness_factor=stiffness_factor)
-            # check if user attempts to upload multiple files for the same well
-            if self.wells[well_file[WELL_INDEX_UUID]] is not None:
-                raise DuplicateWellsFoundError(f"Duplicate well found for {well_file[WELL_NAME_UUID]}")
-
-            self.wells[well_file[WELL_INDEX_UUID]] = well_file
+            self.wells.append(well_file)
 
     def to_dataframe(self, include_stim_data=True) -> pd.DataFrame:
         """Creates DataFrame from PlateRecording with all the data
         interpolated, normalized, and scaled.
 
         The returned dataframe contains one column for time in ms and
         one column for each well.
@@ -564,14 +565,15 @@
 
         # add interpolated force timepoints
         if self._created_from_dataframe:
             raise NotImplementedError("Cannot export a DF if created from a DF. Just use the original")
 
         min_time = min([wf.force[0, 0] for wf in self])
         max_time = max([wf.force[0, -1] for wf in self])
+
         interp_period = (
             first_well[INTERPOLATION_VALUE_UUID] if self.is_optical_recording else INTERPOLATED_DATA_PERIOD_US
         )
         interp_timepoints = np.arange(min_time, max_time + interp_period, interp_period)
 
         data = {"Time (s)": pd.Series(interp_timepoints)}
 
@@ -594,19 +596,19 @@
         is_outputting_stim_data = (
             aggregate_stim_timepoints_us is not None and aggregate_stim_timepoints_us.any()
         )
         if is_outputting_stim_data:
             data["Stim Time (µs)"] = pd.Series(aggregate_stim_timepoints_us_for_plotting)
 
         # iterating over self.wells instead of using __iter__ so well_idx is preserved
-        for well_idx, wf in enumerate(self.wells):
+        for wf in self.wells:
             if not wf:
                 continue
 
-            well_name = wf.get(WELL_NAME_UUID, TWENTY_FOUR_WELL_PLATE.get_well_name_from_well_index(well_idx))
+            well_name = wf.get(WELL_NAME_UUID)
 
             # add raw force data
             data[f"{well_name}__raw"] = pd.Series(wf.force[1, :])
 
             # add unit adjusted + normalized force data
             start_idx, end_idx = truncate(
                 source_series=interp_timepoints, lower_bound=wf.force[0, 0], upper_bound=wf.force[0, -1]
@@ -760,29 +762,22 @@
         float(sampling_period)
         if interpolation_value_str is None
         else float(interpolation_value_str) * MICRO_TO_BASE_CONVERSION
     )
 
     begin_recording = _get_excel_metadata_value(sheet, UTC_BEGINNING_RECORDING_UUID)
     begin_recording = datetime.datetime.strptime(begin_recording, "%Y-%m-%d %H:%M:%S")  # type: ignore
-
-    twenty_four_well = LabwareDefinition(row_count=4, column_count=6)
     well_name = _get_excel_metadata_value(sheet, WELL_NAME_UUID)
 
-    # some provided sample xlsx files contained well names like A001 and B001
-    if well_name is not None:
-        well_name = well_name.replace("0", "")
-
     attrs = {
         FILE_FORMAT_VERSION_METADATA_KEY: NOT_APPLICABLE_LABEL,
         TISSUE_SENSOR_READINGS: raw_tissue_reading,
         REFERENCE_SENSOR_READINGS: np.zeros(raw_tissue_reading.shape),
         str(INTERPOLATION_VALUE_UUID): interpolation_value,
         str(TISSUE_SAMPLING_PERIOD_UUID): sampling_period,
         str(UTC_BEGINNING_RECORDING_UUID): begin_recording,
         str(MANTARRAY_SERIAL_NUMBER_UUID): _get_excel_metadata_value(sheet, MANTARRAY_SERIAL_NUMBER_UUID),
         str(PLATE_BARCODE_UUID): _get_excel_metadata_value(sheet, PLATE_BARCODE_UUID),
         str(WELL_NAME_UUID): well_name,
-        str(WELL_INDEX_UUID): twenty_four_well.get_well_index_from_well_name(well_name),
     }
 
     return attrs
```

### Comparing `Pulse3D-0.33.8/src/pulse3D/plotting.py` & `Pulse3D-0.33.9/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/stimulation.py` & `Pulse3D-0.33.9/src/pulse3D/stimulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -212,20 +212,24 @@
 
 def aggregate_timepoints(timepoints_from_wells: List[NDArray[(1, Any), float]]) -> NDArray[(1, Any), float]:
     unique_timepoints = set(t for timepoints in timepoints_from_wells for t in timepoints)
     return np.array(sorted(unique_timepoints), dtype=float)
 
 
 def realign_interpolated_stim_data(
-    new_timepoints: NDArray[(1, Any), float], orignal_stim_status_data: NDArray[(2, Any), float]
+    new_timepoints: NDArray[(1, Any), float], original_stim_status_data: NDArray[(2, Any), float]
 ) -> NDArray[(1, Any), float]:
-    adjusted_interpolated_stim_data = np.full((len(new_timepoints)), np.NaN)
-    orignal_timepoints_list = orignal_stim_status_data[0].tolist()
-    for new_idx, new_t in enumerate(new_timepoints):
-        try:
-            old_idx = orignal_timepoints_list.index(new_t)
-        except ValueError:
-            continue
-        else:
-            orignal_timepoints_list[old_idx] = None  # remove since there will be duplicate timepoints
-            adjusted_interpolated_stim_data[new_idx] = orignal_stim_status_data[1, old_idx]
+    adjusted_interpolated_stim_data = np.full(len(new_timepoints), np.NaN)
+
+    old_idx = 0
+    curr_time, curr_charge = original_stim_status_data[:, old_idx]
+    for new_idx, new_time in enumerate(new_timepoints):
+        if new_time == curr_time:
+            adjusted_interpolated_stim_data[new_idx] = curr_charge
+
+            old_idx += 1
+            try:
+                curr_time, curr_charge = original_stim_status_data[:, old_idx]
+            except IndexError:
+                break
+
     return adjusted_interpolated_stim_data
```

### Comparing `Pulse3D-0.33.8/src/pulse3D/transforms.py` & `Pulse3D-0.33.9/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.8/src/pulse3D/utils.py` & `Pulse3D-0.33.9/src/pulse3D/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from .constants import MAX_CARDIAC_EXPERIMENT_ID
 from .constants import MAX_EXPERIMENT_ID
 from .constants import MAX_SKM_EXPERIMENT_ID
 from .constants import MAX_VARIABLE_EXPERIMENT_ID
 from .constants import MIN_EXPERIMENT_ID
 from .constants import POST_STIFFNESS_LABEL_TO_FACTOR
 from .constants import SKM_STIFFNESS_LABEL
-from .constants import TWENTY_FOUR_WELL_PLATE
 from .constants import VARIABLE_STIFFNESS_LABEL
 from .constants import WELL_NAME_UUID
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -32,33 +31,33 @@
     return int(barcode[-3:])
 
 
 def get_stiffness_label(barcode_experiment_id: int) -> str:
     return _get_stiffness_info(barcode_experiment_id)[0]
 
 
-def get_stiffness_factor(barcode_experiment_id: int, well_idx: int) -> int:
-    return _get_stiffness_info(barcode_experiment_id, well_idx)[1]
+def get_stiffness_factor(barcode_experiment_id: int, well_name: str) -> int:
+    return _get_stiffness_info(barcode_experiment_id, well_name)[1]
 
 
-def _get_stiffness_info(barcode_experiment_id: int, well_idx: Optional[int] = None) -> Tuple[str, int]:
+def _get_stiffness_info(barcode_experiment_id: int, well_name: Optional[str] = None) -> Tuple[str, int]:
     if not (MIN_EXPERIMENT_ID <= barcode_experiment_id <= MAX_EXPERIMENT_ID):
         raise ValueError(f"Experiment ID must be in the range 000-999, not {barcode_experiment_id}")
 
     well_row_label = None
 
     if barcode_experiment_id <= MAX_CARDIAC_EXPERIMENT_ID:
         stiffness_label = CARDIAC_STIFFNESS_LABEL
     elif barcode_experiment_id <= MAX_SKM_EXPERIMENT_ID:
         stiffness_label = SKM_STIFFNESS_LABEL
     elif barcode_experiment_id <= MAX_VARIABLE_EXPERIMENT_ID:
         stiffness_label = VARIABLE_STIFFNESS_LABEL
         # if no well index given, assume the stiffness factor isn't needed by the caller
-        if well_idx is not None:
-            well_row_label = TWENTY_FOUR_WELL_PLATE.get_well_name_from_well_index(well_idx)[0]
+        if well_name is not None:
+            well_row_label = well_name[0]
     else:
         # if experiment ID does not have a stiffness factor defined (currently 300-999) then just use the value for Cardiac
         stiffness_label = CARDIAC_STIFFNESS_LABEL
 
     stiffness_factor = POST_STIFFNESS_LABEL_TO_FACTOR[stiffness_label]
     if well_row_label:
         stiffness_factor = stiffness_factor[well_row_label]
```

