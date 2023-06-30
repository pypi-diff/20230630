# Comparing `tmp/element-calcium-imaging-0.7.5.tar.gz` & `tmp/element-calcium-imaging-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-calcium-imaging-0.7.5.tar", last modified: Wed Jun 21 02:47:51 2023, max compression
+gzip compressed data, was "element-calcium-imaging-0.7.6.tar", last modified: Fri Jun 30 21:14:49 2023, max compression
```

## Comparing `element-calcium-imaging-0.7.5.tar` & `element-calcium-imaging-0.7.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:47:51.007014 element-calcium-imaging-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-21 02:47:51.007014 element-calcium-imaging-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:47:51.003014 element-calcium-imaging-0.7.5/element_calcium_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    66523 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63721 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/imaging_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    74252 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/imaging_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/imaging_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:47:51.007014 element-calcium-imaging-0.7.5/element_calcium_imaging/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/plotting/cell_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/element_calcium_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:47:51.007014 element-calcium-imaging-0.7.5/element_calcium_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-21 02:47:50.000000 element-calcium-imaging-0.7.5/element_calcium_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-21 02:47:50.000000 element-calcium-imaging-0.7.5/element_calcium_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 02:47:50.000000 element-calcium-imaging-0.7.5/element_calcium_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-21 02:47:50.000000 element-calcium-imaging-0.7.5/element_calcium_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 02:47:50.000000 element-calcium-imaging-0.7.5/element_calcium_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 02:47:51.007014 element-calcium-imaging-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-21 02:47:47.000000 element-calcium-imaging-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:49.780861 element-calcium-imaging-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-30 21:14:49.780861 element-calcium-imaging-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:49.776861 element-calcium-imaging-0.7.6/element_calcium_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66550 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63748 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74306 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:49.780861 element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/cell_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:49.776861 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:14:49.780861 element-calcium-imaging-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/setup.py
```

### Comparing `element-calcium-imaging-0.7.5/LICENSE` & `element-calcium-imaging-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.5/PKG-INFO` & `element-calcium-imaging-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.5
+Version: 0.7.6
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
@@ -14,55 +14,59 @@
 Provides-Extra: nd2
 Provides-Extra: suite2p
 Provides-Extra: tests
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/element-calcium-imaging.svg)](http://badge.fury.io/py/element-calcium-imaging)
 
-# DataJoint Element - Functional Calcium Imaging
+# DataJoint Element for Functional Calcium Imaging
 
 DataJoint Element for functional calcium imaging with 
 [ScanImage](https://docs.scanimage.org/), 
 [Scanbox](https://scanbox.org/),
 [Nikon NIS-Elements](https://www.microscope.healthcare.nikon.com/products/software/nis-elements), 
 and `Bruker Prairie View` acquisition software; and 
 [Suite2p](https://github.com/MouseLand/suite2p), 
 [CaImAn](https://github.com/flatironinstitute/CaImAn), and
 [EXTRACT](https://github.com/schnitzer-lab/EXTRACT-public) analysis 
 software. DataJoint Elements collectively standardize and automate
 data collection and analysis for neuroscience experiments. Each Element is a modular
 pipeline for data storage and processing with corresponding database tables that can be
-combined with other Elements to assemble a fully functional pipeline. This repository also provides a tutorial environment and notebooks to learn the pipeline.
+combined with other Elements to assemble a fully functional pipeline. This repository 
+also provides a tutorial environment and notebooks to learn the pipeline.
 
 ## Experiment Flowchart
 
 ![flowchart](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/flowchart.svg)
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
-+ We have designed three variations of the pipeline to handle different use cases. Displayed above is the default `imaging` schema.  Details on all of the `imaging` schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) documentation page.
++ We have designed three variations of the pipeline to handle different use cases. 
+Displayed above is the default `imaging` schema.  Details on all of the `imaging` 
+schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/
+element-calcium-imaging/latest/pipeline/) documentation page.
 
 ## Getting Started
 
-
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
      ```
 
 + [Interactive tutorial on GitHub Codespaces](#interactive-tutorial)
 
 + [Documentation](https://datajoint.com/docs/elements/element-calcium-imaging)
 
 ## Support
 
-+ If you need help getting started or run into any errors, please contact our team by email at support@datajoint.com.
++ If you need help getting started or run into any errors, please open a GitHub Issue 
+or contact our team by email at support@datajoint.com.
 
 ## Interactive Tutorial
 
 + The easiest way to learn about DataJoint Elements is to use the tutorial notebooks within the included interactive environment configured using [Dev Container](https://containers.dev/).
 
 ### Launch Environment
```

### Comparing `element-calcium-imaging-0.7.5/README.md` & `element-calcium-imaging-0.7.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 [![PyPI version](https://badge.fury.io/py/element-calcium-imaging.svg)](http://badge.fury.io/py/element-calcium-imaging)
 
-# DataJoint Element - Functional Calcium Imaging
+# DataJoint Element for Functional Calcium Imaging
 
 DataJoint Element for functional calcium imaging with 
 [ScanImage](https://docs.scanimage.org/), 
 [Scanbox](https://scanbox.org/),
 [Nikon NIS-Elements](https://www.microscope.healthcare.nikon.com/products/software/nis-elements), 
 and `Bruker Prairie View` acquisition software; and 
 [Suite2p](https://github.com/MouseLand/suite2p), 
 [CaImAn](https://github.com/flatironinstitute/CaImAn), and
 [EXTRACT](https://github.com/schnitzer-lab/EXTRACT-public) analysis 
 software. DataJoint Elements collectively standardize and automate
 data collection and analysis for neuroscience experiments. Each Element is a modular
 pipeline for data storage and processing with corresponding database tables that can be
-combined with other Elements to assemble a fully functional pipeline. This repository also provides a tutorial environment and notebooks to learn the pipeline.
+combined with other Elements to assemble a fully functional pipeline. This repository 
+also provides a tutorial environment and notebooks to learn the pipeline.
 
 ## Experiment Flowchart
 
 ![flowchart](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/flowchart.svg)
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
-+ We have designed three variations of the pipeline to handle different use cases. Displayed above is the default `imaging` schema.  Details on all of the `imaging` schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) documentation page.
++ We have designed three variations of the pipeline to handle different use cases. 
+Displayed above is the default `imaging` schema.  Details on all of the `imaging` 
+schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/
+element-calcium-imaging/latest/pipeline/) documentation page.
 
 ## Getting Started
 
-
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
      ```
 
 + [Interactive tutorial on GitHub Codespaces](#interactive-tutorial)
 
 + [Documentation](https://datajoint.com/docs/elements/element-calcium-imaging)
 
 ## Support
 
-+ If you need help getting started or run into any errors, please contact our team by email at support@datajoint.com.
++ If you need help getting started or run into any errors, please open a GitHub Issue 
+or contact our team by email at support@datajoint.com.
 
 ## Interactive Tutorial
 
 + The easiest way to learn about DataJoint Elements is to use the tutorial notebooks within the included interactive environment configured using [Dev Container](https://containers.dev/).
 
 ### Launch Environment
```

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging/analysis.py` & `element-calcium-imaging-0.7.6/element_calcium_imaging/analysis.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging/imaging.py` & `element-calcium-imaging-0.7.6/element_calcium_imaging/imaging.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,15 +524,15 @@
 
                 _, extract_dataset = get_loader_result(key, ProcessingTask)
                 key["processing_time"] = extract_dataset.creation_time
 
         else:
             raise ValueError(f"Unknown task mode: {task_mode}")
 
-        self.insert1(key)
+        self.insert1({**key, "package_version": ""})
 
 
 @schema
 class Curation(dj.Manual):
     """Curated results
 
     If no curation is applied, the curation_output_dir can be set to
```

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging/imaging_no_curation.py` & `element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_no_curation.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,15 +524,15 @@
 
                 _, extract_dataset = get_loader_result(key, ProcessingTask)
                 key["processing_time"] = extract_dataset.creation_time
 
         else:
             raise ValueError(f"Unknown task mode: {task_mode}")
 
-        self.insert1(key)
+        self.insert1({**key, "package_version": ""})
 
 
 # -------------- Motion Correction --------------
 
 
 @schema
 class MotionCorrection(dj.Imported):
```

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging/imaging_preprocess.py` & `element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
                 "Pre-processing steps are not implemented."
                 "Please overwrite this `make` function with"
                 "desired pre-processing steps."
             )
         else:
             raise ValueError(f"Unknown task mode: {task_mode}")
 
-        self.insert1(key)
+        self.insert1({**key, "package_version": ""})
 
 
 @schema
 class ProcessingMethod(dj.Lookup):
     """Package used for processing of calcium imaging data (e.g. Suite2p, CaImAn, etc.).
 
     Attributes:
@@ -737,15 +737,15 @@
 
                 _, extract_dataset = get_loader_result(key, ProcessingTask)
                 key["processing_time"] = extract_dataset.creation_time
 
         else:
             raise ValueError(f"Unknown task mode: {task_mode}")
 
-        self.insert1(key)
+        self.insert1({**key, "package_version": ""})
 
 
 @schema
 class Curation(dj.Manual):
     """Curated results
 
     If no curation is applied, the curation_output_dir can be set to
```

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging/imaging_report.py` & `element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_report.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging/plotting/cell_plot.py` & `element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/cell_plot.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging/plotting/widget.py` & `element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging/scan.py` & `element-calcium-imaging-0.7.6/element_calcium_imaging/scan.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging.egg-info/PKG-INFO` & `element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.5
+Version: 0.7.6
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
@@ -14,55 +14,59 @@
 Provides-Extra: nd2
 Provides-Extra: suite2p
 Provides-Extra: tests
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/element-calcium-imaging.svg)](http://badge.fury.io/py/element-calcium-imaging)
 
-# DataJoint Element - Functional Calcium Imaging
+# DataJoint Element for Functional Calcium Imaging
 
 DataJoint Element for functional calcium imaging with 
 [ScanImage](https://docs.scanimage.org/), 
 [Scanbox](https://scanbox.org/),
 [Nikon NIS-Elements](https://www.microscope.healthcare.nikon.com/products/software/nis-elements), 
 and `Bruker Prairie View` acquisition software; and 
 [Suite2p](https://github.com/MouseLand/suite2p), 
 [CaImAn](https://github.com/flatironinstitute/CaImAn), and
 [EXTRACT](https://github.com/schnitzer-lab/EXTRACT-public) analysis 
 software. DataJoint Elements collectively standardize and automate
 data collection and analysis for neuroscience experiments. Each Element is a modular
 pipeline for data storage and processing with corresponding database tables that can be
-combined with other Elements to assemble a fully functional pipeline. This repository also provides a tutorial environment and notebooks to learn the pipeline.
+combined with other Elements to assemble a fully functional pipeline. This repository 
+also provides a tutorial environment and notebooks to learn the pipeline.
 
 ## Experiment Flowchart
 
 ![flowchart](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/flowchart.svg)
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
-+ We have designed three variations of the pipeline to handle different use cases. Displayed above is the default `imaging` schema.  Details on all of the `imaging` schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) documentation page.
++ We have designed three variations of the pipeline to handle different use cases. 
+Displayed above is the default `imaging` schema.  Details on all of the `imaging` 
+schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/
+element-calcium-imaging/latest/pipeline/) documentation page.
 
 ## Getting Started
 
-
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
      ```
 
 + [Interactive tutorial on GitHub Codespaces](#interactive-tutorial)
 
 + [Documentation](https://datajoint.com/docs/elements/element-calcium-imaging)
 
 ## Support
 
-+ If you need help getting started or run into any errors, please contact our team by email at support@datajoint.com.
++ If you need help getting started or run into any errors, please open a GitHub Issue 
+or contact our team by email at support@datajoint.com.
 
 ## Interactive Tutorial
 
 + The easiest way to learn about DataJoint Elements is to use the tutorial notebooks within the included interactive environment configured using [Dev Container](https://containers.dev/).
 
 ### Launch Environment
```

### Comparing `element-calcium-imaging-0.7.5/element_calcium_imaging.egg-info/SOURCES.txt` & `element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.5/setup.py` & `element-calcium-imaging-0.7.6/setup.py`

 * *Files identical despite different names*

