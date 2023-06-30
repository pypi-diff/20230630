# Comparing `tmp/elifecleaner-0.9.0.tar.gz` & `tmp/elifecleaner-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elifecleaner-0.9.0.tar", last modified: Sat Dec 18 01:33:52 2021, max compression
+gzip compressed data, was "dist/elifecleaner-0.9.1.tar", last modified: Wed Jan  5 16:55:38 2022, max compression
```

## Comparing `elifecleaner-0.9.0.tar` & `elifecleaner-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       38 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      946 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/PKG-INFO
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/elifecleaner.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      946 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/elifecleaner.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       23 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/elifecleaner.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       13 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/elifecleaner.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)        1 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/elifecleaner.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      357 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/elifecleaner.egg-info/SOURCES.txt
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-12-18 01:33:52.000000 elifecleaner-0.9.0/elifecleaner/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1010 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/elifecleaner/pdf_utils.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)    12746 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/elifecleaner/parse.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     6627 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/elifecleaner/transform.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      544 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/elifecleaner/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1704 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/elifecleaner/zip_lib.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      376 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/README.md
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       24 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      822 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/setup.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1088 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       56 2021-12-18 01:33:25.000000 elifecleaner-0.9.0/requirements.txt
+drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       38 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      946 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/PKG-INFO
+drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/elifecleaner.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      946 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/elifecleaner.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       23 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/elifecleaner.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       13 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/elifecleaner.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)        1 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/elifecleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      357 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/elifecleaner.egg-info/SOURCES.txt
+drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2022-01-05 16:55:38.000000 elifecleaner-0.9.1/elifecleaner/
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1010 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/elifecleaner/pdf_utils.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)    12746 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/elifecleaner/parse.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     6627 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/elifecleaner/transform.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      544 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/elifecleaner/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1652 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/elifecleaner/zip_lib.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      376 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/README.md
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       24 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      822 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/setup.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1088 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       56 2022-01-05 16:55:11.000000 elifecleaner-0.9.1/requirements.txt
```

### Comparing `elifecleaner-0.9.0/PKG-INFO` & `elifecleaner-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elifecleaner
-Version: 0.9.0
+Version: 0.9.1
 Summary: Clean and transform article submission files into a consistent format.
 Home-page: https://github.com/elifesciences/elife-cleaner
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elifecleaner-0.9.0/elifecleaner.egg-info/PKG-INFO` & `elifecleaner-0.9.1/elifecleaner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elifecleaner
-Version: 0.9.0
+Version: 0.9.1
 Summary: Clean and transform article submission files into a consistent format.
 Home-page: https://github.com/elifesciences/elife-cleaner
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elifecleaner-0.9.0/elifecleaner/pdf_utils.py` & `elifecleaner-0.9.1/elifecleaner/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `elifecleaner-0.9.0/elifecleaner/parse.py` & `elifecleaner-0.9.1/elifecleaner/parse.py`

 * *Files identical despite different names*

### Comparing `elifecleaner-0.9.0/elifecleaner/transform.py` & `elifecleaner-0.9.1/elifecleaner/transform.py`

 * *Files identical despite different names*

### Comparing `elifecleaner-0.9.0/elifecleaner/__init__.py` & `elifecleaner-0.9.1/elifecleaner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.NullHandler())
 
 
 def configure_logging(filename, level=logging.INFO, format_string=None):
```

### Comparing `elifecleaner-0.9.0/elifecleaner/zip_lib.py` & `elifecleaner-0.9.1/elifecleaner/zip_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,16 @@
     # sort by file name
     zip_asset_infos = sorted(zip_asset_infos, key=lambda asset: asset.filename)
     return zip_asset_infos
 
 
 def unzip_file(open_zipfile, zip_file_info, output_path):
     "read the zip_file_info from the open_zipfile and write to output_path"
-    with open_zipfile.open(zip_file_info) as zip_content:
-        with open(output_path, "wb") as output_file:
-            output_file.write(zip_content.read())
+    with open(output_path, "wb") as output_file:
+        output_file.write(open_zipfile.read(zip_file_info))
 
 
 def unzip_zip(file_name, temp_dir):
     "unzip certain files and return the local paths"
     asset_file_name_map = OrderedDict()
     zip_asset_infos = profile_zip(file_name)
```

### Comparing `elifecleaner-0.9.0/setup.py` & `elifecleaner-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `elifecleaner-0.9.0/LICENSE` & `elifecleaner-0.9.1/LICENSE`

 * *Files identical despite different names*

