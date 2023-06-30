# Comparing `tmp/th2_grpc_sim-5.0.0.dev5387674261.tar.gz` & `tmp/th2_grpc_sim-5.0.0.dev5420121459.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_sim-5.0.0.dev5387674261.tar", last modified: Tue Jun 27 08:43:01 2023, max compression
+gzip compressed data, was "dist/th2_grpc_sim-5.0.0.dev5420121459.tar", last modified: Fri Jun 30 06:49:00 2023, max compression
```

## Comparing `th2_grpc_sim-5.0.0.dev5387674261.tar` & `th2_grpc_sim-5.0.0.dev5420121459.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-06-27 08:42:12.000000 th2_grpc_sim-5.0.0.dev5387674261/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-27 08:42:12.000000 th2_grpc_sim-5.0.0.dev5387674261/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-06-27 08:42:12.000000 th2_grpc_sim-5.0.0.dev5387674261/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-06-27 08:42:12.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4469 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-27 08:42:42.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-27 08:43:01.000000 th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-06-30 06:48:05.000000 th2_grpc_sim-5.0.0.dev5420121459/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-30 06:48:05.000000 th2_grpc_sim-5.0.0.dev5420121459/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-06-30 06:48:05.000000 th2_grpc_sim-5.0.0.dev5420121459/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-06-30 06:48:05.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2586 2023-06-30 06:48:59.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-06-30 06:48:59.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-06-30 06:48:59.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-30 06:48:40.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-30 06:49:00.000000 th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim.egg-info/top_level.txt
```

### Comparing `th2_grpc_sim-5.0.0.dev5387674261/PKG-INFO` & `th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_grpc_sim
-Version: 5.0.0.dev5387674261
+Name: th2-grpc-sim
+Version: 5.0.0.dev5420121459
 Summary: th2_grpc_sim
 Home-page: https://github.com/th2-net/th2-grpc-sim
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim library
```

### Comparing `th2_grpc_sim-5.0.0.dev5387674261/README.md` & `th2_grpc_sim-5.0.0.dev5420121459/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5387674261/setup.py` & `th2_grpc_sim-5.0.0.dev5420121459/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-sim',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
         'mypy-protobuf==3.2',
-        'grpcio-tools==1.48.1'
+        'grpcio-tools==1.50.0'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
     }
```

### Comparing `th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim.proto` & `th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim_pb2.pyi` & `th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim_pb2_grpc.py` & `th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim/sim_service.py` & `th2_grpc_sim-5.0.0.dev5420121459/th2_grpc_sim/sim_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5387674261/th2_grpc_sim.egg-info/PKG-INFO` & `th2_grpc_sim-5.0.0.dev5420121459/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-grpc-sim
-Version: 5.0.0.dev5387674261
+Name: th2_grpc_sim
+Version: 5.0.0.dev5420121459
 Summary: th2_grpc_sim
 Home-page: https://github.com/th2-net/th2-grpc-sim
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim library
```

