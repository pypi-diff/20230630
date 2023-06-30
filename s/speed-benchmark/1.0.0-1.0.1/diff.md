# Comparing `tmp/speed-benchmark-1.0.0.tar.gz` & `tmp/speed-benchmark-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speed-benchmark-1.0.0.tar", last modified: Fri Jun 30 04:56:32 2023, max compression
+gzip compressed data, was "speed-benchmark-1.0.1.tar", last modified: Fri Jun 30 05:03:06 2023, max compression
```

## Comparing `speed-benchmark-1.0.0.tar` & `speed-benchmark-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:56:32.118629 speed-benchmark-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 04:56:32.118629 speed-benchmark-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 04:56:16.000000 speed-benchmark-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 04:56:32.118629 speed-benchmark-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-06-30 04:56:16.000000 speed-benchmark-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:56:32.118629 speed-benchmark-1.0.0/speed_benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 04:56:16.000000 speed-benchmark-1.0.0/speed_benchmark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:56:32.118629 speed-benchmark-1.0.0/speed_benchmark/speed_benchmark/
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-06-30 04:56:16.000000 speed-benchmark-1.0.0/speed_benchmark/speed_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-30 04:56:16.000000 speed-benchmark-1.0.0/speed_benchmark/speed_benchmark/speed_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:56:32.118629 speed-benchmark-1.0.0/speed_benchmark/visualization/
--rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-06-30 04:56:16.000000 speed-benchmark-1.0.0/speed_benchmark/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 04:56:16.000000 speed-benchmark-1.0.0/speed_benchmark/visualization/generate_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 04:56:16.000000 speed-benchmark-1.0.0/speed_benchmark/visualization/line_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:56:32.118629 speed-benchmark-1.0.0/speed_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 04:56:32.000000 speed-benchmark-1.0.0/speed_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-30 04:56:32.000000 speed-benchmark-1.0.0/speed_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 04:56:32.000000 speed-benchmark-1.0.0/speed_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 04:56:32.000000 speed-benchmark-1.0.0/speed_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 04:56:32.000000 speed-benchmark-1.0.0/speed_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/speed_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/speed_benchmark/speed_benchmark/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/speed_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/speed_benchmark/speed_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/speed_benchmark/visualization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/visualization/generate_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/visualization/line_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/speed_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/top_level.txt
```

### Comparing `speed-benchmark-1.0.0/PKG-INFO` & `speed-benchmark-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speed-benchmark
-Version: 1.0.0
+Version: 1.0.1
 Summary: A generic speed benchmark library.
 Home-page: https://github.com/shenmishajing/speed_benchmark
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/speed_benchmark
 Project-URL: Issue tracker, https://github.com/shenmishajing/speed_benchmark/issues
```

### Comparing `speed-benchmark-1.0.0/README.md` & `speed-benchmark-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `speed-benchmark-1.0.0/setup.py` & `speed-benchmark-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="speed-benchmark",
-    version="1.0.0",
+    version="1.0.1",
     description="A generic speed benchmark library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/speed_benchmark",
     project_urls={
```

### Comparing `speed-benchmark-1.0.0/speed_benchmark/speed_benchmark/speed_benchmark.py` & `speed-benchmark-1.0.1/speed_benchmark/speed_benchmark/speed_benchmark.py`

 * *Files identical despite different names*

### Comparing `speed-benchmark-1.0.0/speed_benchmark/visualization/line_chart.py` & `speed-benchmark-1.0.1/speed_benchmark/visualization/line_chart.py`

 * *Files identical despite different names*

### Comparing `speed-benchmark-1.0.0/speed_benchmark.egg-info/PKG-INFO` & `speed-benchmark-1.0.1/speed_benchmark.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speed-benchmark
-Version: 1.0.0
+Version: 1.0.1
 Summary: A generic speed benchmark library.
 Home-page: https://github.com/shenmishajing/speed_benchmark
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/speed_benchmark
 Project-URL: Issue tracker, https://github.com/shenmishajing/speed_benchmark/issues
```

