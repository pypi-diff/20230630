# Comparing `tmp/drive_ibd-2.0.3.tar.gz` & `tmp/drive_ibd-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive_ibd-2.0.3.tar", max compression
+gzip compressed data, was "drive_ibd-2.0.4.tar", max compression
```

## Comparing `drive_ibd-2.0.3.tar` & `drive_ibd-2.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1096 2023-05-02 16:23:38.534742 drive_ibd-2.0.3/README.md
--rw-r--r--   0        0        0       23 2023-05-08 17:12:27.774702 drive_ibd-2.0.3/drive/__init__.py
--rw-r--r--   0        0        0       45 2023-05-04 19:56:44.572942 drive_ibd-2.0.3/drive/cluster/__init__.py
--rw-r--r--   0        0        0    17869 2023-05-23 17:27:33.288051 drive_ibd-2.0.3/drive/cluster/cluster.py
--rw-r--r--   0        0        0    10145 2023-06-26 19:00:49.383493 drive_ibd-2.0.3/drive/drive.py
--rw-r--r--   0        0        0      129 2023-04-11 15:57:06.666606 drive_ibd-2.0.3/drive/factory/__init__.py
--rw-r--r--   0        0        0     1515 2023-05-03 21:40:36.665638 drive_ibd-2.0.3/drive/factory/factory.py
--rw-r--r--   0        0        0      784 2023-05-03 21:40:36.649638 drive_ibd-2.0.3/drive/factory/loader.py
--rw-r--r--   0        0        0       30 2023-06-22 19:24:49.749173 drive_ibd-2.0.3/drive/filters/__init__.py
--rw-r--r--   0        0        0    17183 2023-06-27 18:29:28.100126 drive_ibd-2.0.3/drive/filters/filter.py
--rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.0.3/drive/log/.git
--rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.0.3/drive/log/.gitignore
--rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.0.3/drive/log/README.md
--rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.0.3/drive/log/__init__.py
--rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.0.3/drive/log/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.0.3/drive/log/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6230 2023-06-22 19:16:27.189955 drive_ibd-2.0.3/drive/log/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.0.3/drive/log/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     4240 2023-05-23 17:27:33.148055 drive_ibd-2.0.3/drive/log/logger.py
--rw-r--r--   0        0        0      248 2023-06-21 16:46:23.320291 drive_ibd-2.0.3/drive/models/__init__.py
--rw-r--r--   0        0        0      503 2023-06-21 16:46:16.772455 drive_ibd-2.0.3/drive/models/choices.py
--rw-r--r--   0        0        0      694 2023-05-04 22:02:59.468876 drive_ibd-2.0.3/drive/models/data_container.py
--rw-r--r--   0        0        0     4493 2023-06-27 18:13:44.556344 drive_ibd-2.0.3/drive/models/generate_indices.py
--rw-r--r--   0        0        0     2161 2023-05-04 16:45:00.827439 drive_ibd-2.0.3/drive/models/networks.py
--rw-r--r--   0        0        0      617 2023-04-13 21:14:00.109726 drive_ibd-2.0.3/drive/models/types.py
--rw-r--r--   0        0        0        0 2023-05-03 14:34:54.522918 drive_ibd-2.0.3/drive/plugins/__init__.py
--rw-r--r--   0        0        0     4352 2023-06-27 18:14:16.239555 drive_ibd-2.0.3/drive/plugins/network_writer.py
--rw-r--r--   0        0        0    10084 2023-05-23 17:30:22.059715 drive_ibd-2.0.3/drive/plugins/pvalues.py
--rw-r--r--   0        0        0       59 2023-05-03 21:40:36.641638 drive_ibd-2.0.3/drive/utilities/callbacks/__init__.py
--rw-r--r--   0        0        0     1520 2023-05-03 21:40:36.657638 drive_ibd-2.0.3/drive/utilities/callbacks/callbacks.py
--rw-r--r--   0        0        0     2222 2023-05-02 19:24:58.309743 drive_ibd-2.0.3/drive/utilities/load_phenotypes.py
--rw-r--r--   0        0        0      121 2023-05-03 21:42:41.142428 drive_ibd-2.0.3/drive/utilities/parser/__init__.py
--rw-r--r--   0        0        0     9196 2023-05-23 17:27:33.204053 drive_ibd-2.0.3/drive/utilities/parser/case_file_parser.py
--rw-r--r--   0        0        0      919 2023-05-04 20:29:24.747764 drive_ibd-2.0.3/drive/utilities/parser/phenotype_descriptions_parser.py
--rw-r--r--   0        0        0     2171 2023-06-30 15:37:27.116947 drive_ibd-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 drive_ibd-2.0.3/setup.py
--rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 drive_ibd-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-02 16:23:38.534742 drive_ibd-2.0.4/README.md
+-rw-r--r--   0        0        0       23 2023-05-08 17:12:27.774702 drive_ibd-2.0.4/drive/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-04 19:56:44.572942 drive_ibd-2.0.4/drive/cluster/__init__.py
+-rw-r--r--   0        0        0    17869 2023-05-23 17:27:33.288051 drive_ibd-2.0.4/drive/cluster/cluster.py
+-rw-r--r--   0        0        0    10145 2023-06-26 19:00:49.383493 drive_ibd-2.0.4/drive/drive.py
+-rw-r--r--   0        0        0      129 2023-04-11 15:57:06.666606 drive_ibd-2.0.4/drive/factory/__init__.py
+-rw-r--r--   0        0        0     1529 2023-06-30 15:43:04.548543 drive_ibd-2.0.4/drive/factory/factory.py
+-rw-r--r--   0        0        0      784 2023-05-03 21:40:36.649638 drive_ibd-2.0.4/drive/factory/loader.py
+-rw-r--r--   0        0        0       30 2023-06-22 19:24:49.749173 drive_ibd-2.0.4/drive/filters/__init__.py
+-rw-r--r--   0        0        0    17183 2023-06-27 18:29:28.100126 drive_ibd-2.0.4/drive/filters/filter.py
+-rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.0.4/drive/log/.git
+-rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.0.4/drive/log/.gitignore
+-rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.0.4/drive/log/README.md
+-rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.0.4/drive/log/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.0.4/drive/log/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.0.4/drive/log/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6230 2023-06-22 19:16:27.189955 drive_ibd-2.0.4/drive/log/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.0.4/drive/log/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     4240 2023-05-23 17:27:33.148055 drive_ibd-2.0.4/drive/log/logger.py
+-rw-r--r--   0        0        0      248 2023-06-21 16:46:23.320291 drive_ibd-2.0.4/drive/models/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-21 16:46:16.772455 drive_ibd-2.0.4/drive/models/choices.py
+-rw-r--r--   0        0        0      694 2023-05-04 22:02:59.468876 drive_ibd-2.0.4/drive/models/data_container.py
+-rw-r--r--   0        0        0     4493 2023-06-27 18:13:44.556344 drive_ibd-2.0.4/drive/models/generate_indices.py
+-rw-r--r--   0        0        0     2161 2023-05-04 16:45:00.827439 drive_ibd-2.0.4/drive/models/networks.py
+-rw-r--r--   0        0        0      617 2023-04-13 21:14:00.109726 drive_ibd-2.0.4/drive/models/types.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:34:54.522918 drive_ibd-2.0.4/drive/plugins/__init__.py
+-rw-r--r--   0        0        0     4352 2023-06-27 18:14:16.239555 drive_ibd-2.0.4/drive/plugins/network_writer.py
+-rw-r--r--   0        0        0    10084 2023-05-23 17:30:22.059715 drive_ibd-2.0.4/drive/plugins/pvalues.py
+-rw-r--r--   0        0        0       59 2023-05-03 21:40:36.641638 drive_ibd-2.0.4/drive/utilities/callbacks/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-03 21:40:36.657638 drive_ibd-2.0.4/drive/utilities/callbacks/callbacks.py
+-rw-r--r--   0        0        0     2222 2023-05-02 19:24:58.309743 drive_ibd-2.0.4/drive/utilities/load_phenotypes.py
+-rw-r--r--   0        0        0      121 2023-05-03 21:42:41.142428 drive_ibd-2.0.4/drive/utilities/parser/__init__.py
+-rw-r--r--   0        0        0     9196 2023-05-23 17:27:33.204053 drive_ibd-2.0.4/drive/utilities/parser/case_file_parser.py
+-rw-r--r--   0        0        0      919 2023-05-04 20:29:24.747764 drive_ibd-2.0.4/drive/utilities/parser/phenotype_descriptions_parser.py
+-rw-r--r--   0        0        0     2178 2023-06-30 15:43:26.312025 drive_ibd-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 drive_ibd-2.0.4/setup.py
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 drive_ibd-2.0.4/PKG-INFO
```

### Comparing `drive_ibd-2.0.3/README.md` & `drive_ibd-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/cluster/cluster.py` & `drive_ibd-2.0.4/drive/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/drive.py` & `drive_ibd-2.0.4/drive/drive.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/factory/factory.py` & `drive_ibd-2.0.4/drive/factory/factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     """
     Error that is raised if the user tries to load a plugin
     that is not there
     """
 
     def __init__(self, plugin_type: str) -> None:
         super().__init__(
-            f"Plugin, {plugin_type} not found in the plugins folder. Make sure you loaded the plugin into the json file."
+            f"Plugin, {plugin_type} not found in the plugins folder. Make sure you loaded the plugin into the json file."  # noqa: E501
         )
 
 
 class AnalysisObj(Protocol):
     """Interface defining of an analysis object"""
 
     def analyze(self, **kwargs) -> Any:
```

### Comparing `drive_ibd-2.0.3/drive/factory/loader.py` & `drive_ibd-2.0.4/drive/factory/loader.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/filters/filter.py` & `drive_ibd-2.0.4/drive/filters/filter.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/log/README.md` & `drive_ibd-2.0.4/drive/log/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/log/__pycache__/logger.cpython-311.pyc` & `drive_ibd-2.0.4/drive/log/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/log/__pycache__/logger.cpython-39.pyc` & `drive_ibd-2.0.4/drive/log/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/log/logger.py` & `drive_ibd-2.0.4/drive/log/logger.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/models/data_container.py` & `drive_ibd-2.0.4/drive/models/data_container.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/models/generate_indices.py` & `drive_ibd-2.0.4/drive/models/generate_indices.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/models/networks.py` & `drive_ibd-2.0.4/drive/models/networks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/models/types.py` & `drive_ibd-2.0.4/drive/models/types.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/plugins/network_writer.py` & `drive_ibd-2.0.4/drive/plugins/network_writer.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/plugins/pvalues.py` & `drive_ibd-2.0.4/drive/plugins/pvalues.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/utilities/callbacks/callbacks.py` & `drive_ibd-2.0.4/drive/utilities/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/utilities/load_phenotypes.py` & `drive_ibd-2.0.4/drive/utilities/load_phenotypes.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/utilities/parser/case_file_parser.py` & `drive_ibd-2.0.4/drive/utilities/parser/case_file_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/drive/utilities/parser/phenotype_descriptions_parser.py` & `drive_ibd-2.0.4/drive/utilities/parser/phenotype_descriptions_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.3/pyproject.toml` & `drive_ibd-2.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drive-ibd"
-version = "2.0.3"
+version = "2.0.4"
 description = "cli tool to identify networks of individuals who share IBD segments overlapping loci of interest"
 authors = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>", "Jennifer E. Below <jennifer.e.below@vumc.org>"]
 maintainers = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>"]
 repository = "https://github.com/belowlab/drive"
 homepage = "https://belowlab.github.io/drive/"
 readme = "README.md"
 keywords = ["python", "genetics", "identity by descent", "relatedness"]
@@ -13,15 +13,15 @@
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 packages = [
     {include = "drive"},
-    { include = "drive/factory" }
+    { include = "factory", from="drive"}
 ]
 
 [tool.poetry.scripts]
 drive = 'drive.drive:app'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `drive_ibd-2.0.3/setup.py` & `drive_ibd-2.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
+package_dir = \
+{'': 'drive'}
+
 packages = \
 ['drive',
  'drive.cluster',
  'drive.factory',
  'drive.filters',
  'drive.log',
  'drive.models',
@@ -25,22 +28,23 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['drive = drive.drive:app']}
 
 setup_kwargs = {
     'name': 'drive-ibd',
-    'version': '2.0.3',
+    'version': '2.0.4',
     'description': 'cli tool to identify networks of individuals who share IBD segments overlapping loci of interest',
     'long_description': '# DRIVE:\n\nThis repository contains the source code for the tool DRIVE v1.0.0. Distant Relatedness for Identification and Variant Evaluation (DRIVE) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implemented a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://belowlab.github.io/drive/)\n\n## Installing DRIVE:\nDRIVE is available on PYPI and can easily be installed using the following command:\n\n```bash\npip install drive-ibd\n```\n\nIf the user wishes to develop DRIVE or install the program from source then they can clone the repository. This process is described under the section called "Github Installation" in the documentation.\n\n### Reporting issues:\nIf you wish to report a bug or propose a feature you can find templates under the .github/ISSUE_TEMPLATE directory.',
     'author': 'James Baker',
     'author_email': 'james.baker@vanderbilt.edu',
     'maintainer': 'James Baker',
     'maintainer_email': 'james.baker@vanderbilt.edu',
     'url': 'https://belowlab.github.io/drive/',
+    'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<3.12',
 }
```

### Comparing `drive_ibd-2.0.3/PKG-INFO` & `drive_ibd-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drive-ibd
-Version: 2.0.3
+Version: 2.0.4
 Summary: cli tool to identify networks of individuals who share IBD segments overlapping loci of interest
 Home-page: https://belowlab.github.io/drive/
 Keywords: python,genetics,identity by descent,relatedness
 Author: James Baker
 Author-email: james.baker@vanderbilt.edu
 Maintainer: James Baker
 Maintainer-email: james.baker@vanderbilt.edu
```

