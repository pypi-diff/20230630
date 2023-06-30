# Comparing `tmp/dask-cuda-23.8.0a230629.tar.gz` & `tmp/dask-cuda-23.8.0a230630.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cuda-23.8.0a230629.tar", last modified: Thu Jun 29 05:08:05 2023, max compression
+gzip compressed data, was "dask-cuda-23.8.0a230630.tar", last modified: Fri Jun 30 05:07:59 2023, max compression
```

## Comparing `dask-cuda-23.8.0a230629.tar` & `dask-cuda-23.8.0a230630.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.500080 dask-cuda-23.8.0a230629/
--rw-r--r--   0 root         (0) root         (0)    11348 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-29 05:08:05.496080 dask-cuda-23.8.0a230629/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.500080 dask-cuda-23.8.0a230629/dask_cuda/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-06-29 05:08:05.500080 dask-cuda-23.8.0a230629/dask_cuda/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.492080 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6393 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cudf_groupby.py
--rw-r--r--   0 root         (0) root         (0)    12437 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cudf_merge.py
--rw-r--r--   0 root         (0) root         (0)     8598 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cudf_shuffle.py
--rw-r--r--   0 root         (0) root         (0)    10752 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cupy.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cupy_map_overlap.py
--rw-r--r--   0 root         (0) root         (0)    26888 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/benchmarks/utils.py
--rw-r--r--   0 root         (0) root         (0)    15870 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/cli.py
--rw-r--r--   0 root         (0) root         (0)     8589 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/disk_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.492080 dask-cuda-23.8.0a230629/dask_cuda/explicit_comms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/explicit_comms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10478 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/explicit_comms/comms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.492080 dask-cuda-23.8.0a230629/dask_cuda/explicit_comms/dataframe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/explicit_comms/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20056 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/explicit_comms/dataframe/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/get_device_memory_objects.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/is_device_object.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/is_spillable_object.py
--rw-r--r--   0 root         (0) root         (0)    17302 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/proxify_device_objects.py
--rw-r--r--   0 root         (0) root         (0)    30850 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    29880 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/proxy_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.496080 dask-cuda-23.8.0a230629/dask_cuda/tests/
--rw-r--r--   0 root         (0) root         (0)     4910 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_cudf_builtin_spilling.py
--rw-r--r--   0 root         (0) root         (0)    15517 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_dask_cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     5882 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_dgx.py
--rw-r--r--   0 root         (0) root         (0)    11150 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_explicit_comms.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_gds.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_initialize.py
--rw-r--r--   0 root         (0) root         (0)    15940 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)    18492 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    23370 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)     9452 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_spill.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/tests/test_worker_spec.py
--rw-r--r--   0 root         (0) root         (0)    29398 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/utils.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/dask_cuda/worker_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.488080 dask-cuda-23.8.0a230629/dask_cuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-29 05:08:05.000000 dask-cuda-23.8.0a230629/dask_cuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-06-29 05:08:05.000000 dask-cuda-23.8.0a230629/dask_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 05:08:05.000000 dask-cuda-23.8.0a230629/dask_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-29 05:08:05.000000 dask-cuda-23.8.0a230629/dask_cuda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-29 05:08:05.000000 dask-cuda-23.8.0a230629/dask_cuda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-29 05:08:05.000000 dask-cuda-23.8.0a230629/dask_cuda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.480080 dask-cuda-23.8.0a230629/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.496080 dask-cuda-23.8.0a230629/examples/ucx/
--rw-r--r--   0 root         (0) root         (0)     1262 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/examples/ucx/client_initialize.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/examples/ucx/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3251 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:08:05.496080 dask-cuda-23.8.0a230629/rtd/
--rw-r--r--   0 root         (0) root         (0)     6223 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/rtd/conf.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 05:08:05.500080 dask-cuda-23.8.0a230629/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-29 05:07:55.000000 dask-cuda-23.8.0a230629/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.921280 dask-cuda-23.8.0a230630/
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-30 05:07:59.921280 dask-cuda-23.8.0a230630/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.921280 dask-cuda-23.8.0a230630/dask_cuda/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-06-30 05:07:59.921280 dask-cuda-23.8.0a230630/dask_cuda/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.917279 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/common.py
+-rw-r--r--   0 root         (0) root         (0)     8894 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cudf_groupby.py
+-rw-r--r--   0 root         (0) root         (0)    12437 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cudf_merge.py
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cudf_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)    10752 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cupy.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cupy_map_overlap.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/benchmarks/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15870 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8589 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/disk_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.917279 dask-cuda-23.8.0a230630/dask_cuda/explicit_comms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/explicit_comms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/explicit_comms/comms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.917279 dask-cuda-23.8.0a230630/dask_cuda/explicit_comms/dataframe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/explicit_comms/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20056 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/explicit_comms/dataframe/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/get_device_memory_objects.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/is_device_object.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/is_spillable_object.py
+-rw-r--r--   0 root         (0) root         (0)    17302 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/proxify_device_objects.py
+-rw-r--r--   0 root         (0) root         (0)    30850 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    29880 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/proxy_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.921280 dask-cuda-23.8.0a230630/dask_cuda/tests/
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_cudf_builtin_spilling.py
+-rw-r--r--   0 root         (0) root         (0)    15517 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_dask_cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_dgx.py
+-rw-r--r--   0 root         (0) root         (0)    11150 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_explicit_comms.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_gds.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_initialize.py
+-rw-r--r--   0 root         (0) root         (0)    15940 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    18492 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    23370 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     9452 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_spill.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/tests/test_worker_spec.py
+-rw-r--r--   0 root         (0) root         (0)    29398 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/dask_cuda/worker_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.913279 dask-cuda-23.8.0a230630/dask_cuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-30 05:07:59.000000 dask-cuda-23.8.0a230630/dask_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-06-30 05:07:59.000000 dask-cuda-23.8.0a230630/dask_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 05:07:59.000000 dask-cuda-23.8.0a230630/dask_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-30 05:07:59.000000 dask-cuda-23.8.0a230630/dask_cuda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-30 05:07:59.000000 dask-cuda-23.8.0a230630/dask_cuda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-30 05:07:59.000000 dask-cuda-23.8.0a230630/dask_cuda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.905279 dask-cuda-23.8.0a230630/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.921280 dask-cuda-23.8.0a230630/examples/ucx/
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/examples/ucx/client_initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/examples/ucx/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3251 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 05:07:59.921280 dask-cuda-23.8.0a230630/rtd/
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/rtd/conf.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 05:07:59.921280 dask-cuda-23.8.0a230630/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-30 05:07:51.000000 dask-cuda-23.8.0a230630/setup.py
```

### Comparing `dask-cuda-23.8.0a230629/LICENSE` & `dask-cuda-23.8.0a230630/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/PKG-INFO` & `dask-cuda-23.8.0a230630/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230629
+Version: 23.8.0a230630
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.8.0a230629/README.md` & `dask-cuda-23.8.0a230630/README.md`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/__init__.py` & `dask-cuda-23.8.0a230630/dask_cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/benchmarks/common.py` & `dask-cuda-23.8.0a230630/dask_cuda/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cudf_groupby.py` & `dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cudf_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cudf_merge.py` & `dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cudf_merge.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cudf_shuffle.py` & `dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cudf_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cupy.py` & `dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cupy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/benchmarks/local_cupy_map_overlap.py` & `dask-cuda-23.8.0a230630/dask_cuda/benchmarks/local_cupy_map_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/benchmarks/utils.py` & `dask-cuda-23.8.0a230630/dask_cuda/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/cli.py` & `dask-cuda-23.8.0a230630/dask_cuda/cli.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/cuda_worker.py` & `dask-cuda-23.8.0a230630/dask_cuda/cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/device_host_file.py` & `dask-cuda-23.8.0a230630/dask_cuda/device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/disk_io.py` & `dask-cuda-23.8.0a230630/dask_cuda/disk_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import os
 import os.path
 import pathlib
 import tempfile
 import threading
 import weakref
 from typing import Callable, Iterable, Mapping, Optional, Union
@@ -160,25 +161,27 @@
 
     Returns
     -------
     header: dict
         A dict of metadata
     """
     cuda_frames = tuple(hasattr(f, "__cuda_array_interface__") for f in frames)
-    frame_lengths = tuple(map(nbytes, frames))
+
     if gds and any(cuda_frames):
         import kvikio
 
+        # Write each frame consecutively into `path` in parallel
         with kvikio.CuFile(path, "w") as f:
-            for frame, length in zip(frames, frame_lengths):
-                f.pwrite(buf=frame, count=length, file_offset=0, buf_offset=0).get()
+            file_offsets = itertools.accumulate(map(nbytes, frames), initial=0)
+            futures = [f.pwrite(b, file_offset=o) for b, o in zip(frames, file_offsets)]
+            for each_fut in futures:
+                each_fut.get()
     else:
         with open(path, "wb") as f:
-            for frame in frames:
-                f.write(frame)
+            os.writev(f.fileno(), frames)  # type: ignore
     return {
         "method": "stdio",
         "path": SpillToDiskFile(path),
         "frame-lengths": tuple(map(nbytes, frames)),
         "shared-filesystem": shared_filesystem,
         "cuda-frames": cuda_frames,
     }
@@ -196,28 +199,26 @@
         match the GDS option set by the prior `disk_write()` call.
 
     Returns
     -------
     frames: list
         List of read frames
     """
-    ret = []
+    ret: list = [
+        get_new_cuda_buffer()(length)
+        if gds and is_cuda
+        else np.empty((length,), dtype="u1")
+        for length, is_cuda in zip(header["frame-lengths"], header["cuda-frames"])
+    ]
     if gds:
         import kvikio  # isort:skip
 
-        with kvikio.CuFile(header["path"], "rb") as f:
-            file_offset = 0
-            for length, is_cuda in zip(header["frame-lengths"], header["cuda-frames"]):
-                if is_cuda:
-                    buf = get_new_cuda_buffer()(length)
-                else:
-                    buf = np.empty((length,), dtype="u1")
-                f.pread(
-                    buf=buf, count=length, file_offset=file_offset, buf_offset=0
-                ).get()
-                file_offset += length
-                ret.append(buf)
+        with kvikio.CuFile(str(header["path"]), "r") as f:
+            # Read each frame consecutively from `path` in parallel
+            file_offsets = itertools.accumulate((b.nbytes for b in ret), initial=0)
+            futures = [f.pread(b, file_offset=o) for b, o in zip(ret, file_offsets)]
+            for each_fut in futures:
+                each_fut.get()
     else:
         with open(str(header["path"]), "rb") as f:
-            for length in header["frame-lengths"]:
-                ret.append(f.read(length))
+            os.readv(f.fileno(), ret)  # type: ignore
     return ret
```

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/explicit_comms/comms.py` & `dask-cuda-23.8.0a230630/dask_cuda/explicit_comms/comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/explicit_comms/dataframe/shuffle.py` & `dask-cuda-23.8.0a230630/dask_cuda/explicit_comms/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/get_device_memory_objects.py` & `dask-cuda-23.8.0a230630/dask_cuda/get_device_memory_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/initialize.py` & `dask-cuda-23.8.0a230630/dask_cuda/initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/is_device_object.py` & `dask-cuda-23.8.0a230630/dask_cuda/is_device_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/is_spillable_object.py` & `dask-cuda-23.8.0a230630/dask_cuda/is_spillable_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/local_cuda_cluster.py` & `dask-cuda-23.8.0a230630/dask_cuda/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/proxify_device_objects.py` & `dask-cuda-23.8.0a230630/dask_cuda/proxify_device_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/proxify_host_file.py` & `dask-cuda-23.8.0a230630/dask_cuda/proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/proxy_object.py` & `dask-cuda-23.8.0a230630/dask_cuda/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_cudf_builtin_spilling.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_cudf_builtin_spilling.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_dask_cuda_worker.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_dask_cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_device_host_file.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_dgx.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_dgx.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_explicit_comms.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_explicit_comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_gds.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_gds.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_initialize.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_local_cuda_cluster.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_proxify_host_file.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_proxy.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_spill.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_spill.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_utils.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/tests/test_worker_spec.py` & `dask-cuda-23.8.0a230630/dask_cuda/tests/test_worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/utils.py` & `dask-cuda-23.8.0a230630/dask_cuda/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda/worker_spec.py` & `dask-cuda-23.8.0a230630/dask_cuda/worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/dask_cuda.egg-info/PKG-INFO` & `dask-cuda-23.8.0a230630/dask_cuda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230629
+Version: 23.8.0a230630
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.8.0a230629/dask_cuda.egg-info/SOURCES.txt` & `dask-cuda-23.8.0a230630/dask_cuda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/examples/ucx/client_initialize.py` & `dask-cuda-23.8.0a230630/examples/ucx/client_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/examples/ucx/local_cuda_cluster.py` & `dask-cuda-23.8.0a230630/examples/ucx/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/pyproject.toml` & `dask-cuda-23.8.0a230630/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/rtd/conf.py` & `dask-cuda-23.8.0a230630/rtd/conf.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230629/setup.py` & `dask-cuda-23.8.0a230630/setup.py`

 * *Files identical despite different names*

