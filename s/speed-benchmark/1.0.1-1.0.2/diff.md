# Comparing `tmp/speed-benchmark-1.0.1.tar.gz` & `tmp/speed-benchmark-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speed-benchmark-1.0.1.tar", last modified: Fri Jun 30 05:03:06 2023, max compression
+gzip compressed data, was "speed-benchmark-1.0.2.tar", last modified: Fri Jun 30 05:14:38 2023, max compression
```

## Comparing `speed-benchmark-1.0.1.tar` & `speed-benchmark-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/speed_benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/speed_benchmark/speed_benchmark/
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/speed_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/speed_benchmark/speed_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/speed_benchmark/visualization/
--rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/visualization/generate_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 05:02:56.000000 speed-benchmark-1.0.1/speed_benchmark/visualization/line_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:03:06.298960 speed-benchmark-1.0.1/speed_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 05:03:06.000000 speed-benchmark-1.0.1/speed_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/speed_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/speed_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/speed_benchmark/visualization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/visualization/generate_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/visualization/line_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/speed_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/top_level.txt
```

### Comparing `speed-benchmark-1.0.1/PKG-INFO` & `speed-benchmark-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speed-benchmark
-Version: 1.0.1
+Version: 1.0.2
 Summary: A generic speed benchmark library.
 Home-page: https://github.com/shenmishajing/speed_benchmark
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/speed_benchmark
 Project-URL: Issue tracker, https://github.com/shenmishajing/speed_benchmark/issues
```

### Comparing `speed-benchmark-1.0.1/README.md` & `speed-benchmark-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `speed-benchmark-1.0.1/setup.py` & `speed-benchmark-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="speed-benchmark",
-    version="1.0.1",
+    version="1.0.2",
     description="A generic speed benchmark library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/speed_benchmark",
     project_urls={
```

### Comparing `speed-benchmark-1.0.1/speed_benchmark/speed_benchmark/speed_benchmark.py` & `speed-benchmark-1.0.2/speed_benchmark/speed_benchmark.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pandas import DataFrame
 
 try:
     import torch
 except ImportError:
     torch = None
 
-from ..visualization import draw_line_chart
+from .visualization import draw_line_chart
 
 
 def visualize_speed_benchmark_res(result, output_path, main_arg_name, save_table):
     index = sorted(result)
     data = {}
     std_data = {}
     for i, ind in enumerate(index):
@@ -88,14 +88,22 @@
         funcs = {f.__name__: f for f in funcs}
     elif isinstance(funcs, dict):
         funcs = {funcs.__name__: funcs}
 
     if not isinstance(args["data"], dict):
         args["data"] = {d[args["main_arg_name"]]: d for d in args["data"]}
 
+    for k in args["data"]:
+        if isinstance(args["data"][k], tuple | list):
+            args["data"][k] = {"args": args["data"][k]}
+        elif isinstance(args["data"][k], dict) and (
+            "kwargs" not in args["data"][k] and "args" not in args["data"][k]
+        ):
+            args["data"][k] = {"kwargs": args["data"][k]}
+
     if torch is not None:
         if pre_func is None:
             pre_func = torch.cuda.synchronize
         if post_func is None:
             post_func = torch.cuda.synchronize
     else:
         if pre_func is None:
@@ -115,21 +123,21 @@
         result[main_arg] = {}
         except_res = None
         for func_name, func in funcs.items():
             result[main_arg][func_name] = []
             cur_res = result[main_arg][func_name]
 
             for _ in range(warmup):
-                func(**data)
+                func(*data.get("args", ()), **data.get("kwargs", {}))
 
             for _ in range(repeat):
                 pre_func()
                 duration = time.perf_counter()
                 for _ in range(num):
-                    func_res = func(**data)
+                    func_res = func(*data.get("args", ()), **data.get("kwargs", {}))
                 post_func()
                 duration = time.perf_counter() - duration
                 duration /= num
 
                 cur_res.append(duration)
 
             if check_result_func is not None:
```

### Comparing `speed-benchmark-1.0.1/speed_benchmark/visualization/line_chart.py` & `speed-benchmark-1.0.2/speed_benchmark/visualization/line_chart.py`

 * *Files identical despite different names*

### Comparing `speed-benchmark-1.0.1/speed_benchmark.egg-info/PKG-INFO` & `speed-benchmark-1.0.2/speed_benchmark.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speed-benchmark
-Version: 1.0.1
+Version: 1.0.2
 Summary: A generic speed benchmark library.
 Home-page: https://github.com/shenmishajing/speed_benchmark
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/speed_benchmark
 Project-URL: Issue tracker, https://github.com/shenmishajing/speed_benchmark/issues
```

