# Comparing `tmp/live_parquet-0.3.0.tar.gz` & `tmp/live_parquet-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/live_parquet-0.3.0.tar", last modified: Thu Jun 29 17:16:04 2023, max compression
+gzip compressed data, was "dist/live_parquet-0.4.0.tar", last modified: Fri Jun 30 12:54:47 2023, max compression
```

## Comparing `live_parquet-0.3.0.tar` & `live_parquet-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-29 17:16:04.755590 live_parquet-0.3.0/
--rw-r--r--   0 sultanfaisal   (502) staff       (20)     1030 2023-06-29 17:16:04.755435 live_parquet-0.3.0/PKG-INFO
--rw-r--r--   0 sultanfaisal   (502) staff       (20)      296 2023-06-29 15:51:54.000000 live_parquet-0.3.0/README.md
-drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-29 17:16:04.755216 live_parquet-0.3.0/live_parquet.egg-info/
--rw-r--r--   0 sultanfaisal   (502) staff       (20)     1030 2023-06-29 17:16:04.000000 live_parquet-0.3.0/live_parquet.egg-info/PKG-INFO
--rw-r--r--   0 sultanfaisal   (502) staff       (20)      197 2023-06-29 17:16:04.000000 live_parquet-0.3.0/live_parquet.egg-info/SOURCES.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)        1 2023-06-29 17:16:04.000000 live_parquet-0.3.0/live_parquet.egg-info/dependency_links.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)       51 2023-06-29 17:16:04.000000 live_parquet-0.3.0/live_parquet.egg-info/requires.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)        1 2023-06-29 17:16:04.000000 live_parquet-0.3.0/live_parquet.egg-info/top_level.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)       38 2023-06-29 17:16:04.755639 live_parquet-0.3.0/setup.cfg
--rw-r--r--   0 sultanfaisal   (502) staff       (20)      968 2023-06-29 17:15:57.000000 live_parquet-0.3.0/setup.py
+drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-30 12:54:47.217369 live_parquet-0.4.0/
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)     1030 2023-06-30 12:54:47.217232 live_parquet-0.4.0/PKG-INFO
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)      296 2023-06-29 15:51:54.000000 live_parquet-0.4.0/README.md
+drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-30 12:54:47.217028 live_parquet-0.4.0/live_parquet.egg-info/
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)     1030 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/PKG-INFO
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)      236 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/SOURCES.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)        1 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/dependency_links.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       65 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/entry_points.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       51 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/requires.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)        1 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/top_level.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       38 2023-06-30 12:54:47.217414 live_parquet-0.4.0/setup.cfg
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)     1093 2023-06-30 12:54:42.000000 live_parquet-0.4.0/setup.py
```

### Comparing `live_parquet-0.3.0/PKG-INFO` & `live_parquet-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live_parquet
-Version: 0.3.0
+Version: 0.4.0
 Summary: A command-line tool to view Parquet files in real-time
 Home-page: UNKNOWN
 Author: Sultan Razin
 License: UNKNOWN
 Description: # Live Parquet
         
         A command-line tool that allows you to monitor the contents of a Parquet file in real-time. The tool prints the top 5 rows of the Parquet file whenever the file size changes.
```

### Comparing `live_parquet-0.3.0/live_parquet.egg-info/PKG-INFO` & `live_parquet-0.4.0/live_parquet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-parquet
-Version: 0.3.0
+Version: 0.4.0
 Summary: A command-line tool to view Parquet files in real-time
 Home-page: UNKNOWN
 Author: Sultan Razin
 License: UNKNOWN
 Description: # Live Parquet
         
         A command-line tool that allows you to monitor the contents of a Parquet file in real-time. The tool prints the top 5 rows of the Parquet file whenever the file size changes.
```

### Comparing `live_parquet-0.3.0/setup.py` & `live_parquet-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="live_parquet",
-    version="0.3.0",
+    version="0.4.0",
     author="Sultan Razin",
     description="A command-line tool to view Parquet files in real-time",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
+    entry_points={
+        "console_scripts": [
+            "live_parquet=live_parquet.main:read_parquet",
+        ],
+    },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

