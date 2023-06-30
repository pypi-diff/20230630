# Comparing `tmp/lazyops-0.2.8.tar.gz` & `tmp/lazyops-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyops-0.2.8.tar", last modified: Thu Jan  5 03:21:35 2023, max compression
+gzip compressed data, was "lazyops-0.2.9.tar", last modified: Sat Jan  7 04:38:33 2023, max compression
```

## Comparing `lazyops-0.2.8.tar` & `lazyops-0.2.9.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.114702 lazyops-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-05 03:21:25.000000 lazyops-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-05 03:21:25.000000 lazyops-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-05 03:21:35.114702 lazyops-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-05 03:21:25.000000 lazyops-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.106702 lazyops-0.2.8/lazyops/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.106702 lazyops-0.2.8/lazyops/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/configs/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/configs/k8s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.106702 lazyops-0.2.8/lazyops/imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/imports/_aiohttpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/imports/_aiokeydb.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/imports/_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/imports/_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/imports/_psutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/imports/_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/imports/_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.106702 lazyops-0.2.8/lazyops/types/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40893 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/types/classprops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/types/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.110702 lazyops-0.2.8/lazyops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/utils/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.110702 lazyops-0.2.8/lazyops/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.110702 lazyops-0.2.8/lazyops/v1/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/experimental/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/experimental/gptj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.110702 lazyops-0.2.8/lazyops/v1/lazyclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyclasses/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyclasses/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyclasses/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyclasses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.110702 lazyops-0.2.8/lazyops/v1/lazyconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyconfig/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyconfig/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyconfig/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyconfig/tfserving.proto
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyconfig/tfserving_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33862 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyconfig/tfserving_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.110702 lazyops-0.2.8/lazyops/v1/lazydatabase/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazydatabase/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazydatabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazydatabase/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazydatabase/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazydatabase/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazydatabase/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazydatabase/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.110702 lazyops-0.2.8/lazyops/v1/lazyio/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyio/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyio/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyio/async_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyio/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.114702 lazyops-0.2.8/lazyops/v1/lazyrpc/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyrpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyrpc/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30860 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyrpc/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyrpc/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyrpc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazyrpc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.114702 lazyops-0.2.8/lazyops/v1/lazysources/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazysources/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazysources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.114702 lazyops-0.2.8/lazyops/v1/lazysources/gdelt/
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazysources/gdelt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazysources/gdelt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazysources/gdelt/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazysources/gdelt/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazysources/gdelt/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/lazysources/gdelt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/mp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/v1/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-05 03:21:25.000000 lazyops-0.2.8/lazyops/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:21:35.106702 lazyops-0.2.8/lazyops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-05 03:21:35.000000 lazyops-0.2.8/lazyops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-01-05 03:21:35.000000 lazyops-0.2.8/lazyops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 03:21:35.000000 lazyops-0.2.8/lazyops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-05 03:21:35.000000 lazyops-0.2.8/lazyops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-05 03:21:35.000000 lazyops-0.2.8/lazyops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 03:21:35.114702 lazyops-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-05 03:21:25.000000 lazyops-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.436811 lazyops-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-07 04:38:23.000000 lazyops-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-07 04:38:23.000000 lazyops-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-07 04:38:33.436811 lazyops-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-07 04:38:23.000000 lazyops-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.424811 lazyops-0.2.9/lazyops/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.428810 lazyops-0.2.9/lazyops/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/configs/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/configs/k8s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.428810 lazyops-0.2.9/lazyops/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_aiohttpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_aiokeydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/imports/_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.428810 lazyops-0.2.9/lazyops/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40893 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/classprops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.428810 lazyops-0.2.9/lazyops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/experimental/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/experimental/gptj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/lazyclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyclasses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/lazyconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33862 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/lazydatabase/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazydatabase/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.432811 lazyops-0.2.9/lazyops/v1/lazyio/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/async_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyio/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.436811 lazyops-0.2.9/lazyops/v1/lazyrpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30860 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazyrpc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.436811 lazyops-0.2.9/lazyops/v1/lazysources/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.436811 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/lazysources/gdelt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/mp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/v1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-07 04:38:23.000000 lazyops-0.2.9/lazyops/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 04:38:33.424811 lazyops-0.2.9/lazyops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-07 04:38:33.000000 lazyops-0.2.9/lazyops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 04:38:33.436811 lazyops-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-07 04:38:23.000000 lazyops-0.2.9/setup.py
```

### Comparing `lazyops-0.2.8/LICENSE` & `lazyops-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/PKG-INFO` & `lazyops-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyops
-Version: 0.2.8
+Version: 0.2.9
 Summary: A collection of submodules/patterns that are commonly used within Internal Development
 Home-page: https://github.com/trisongz/lazyops
 Author: Tri Songz
 Author-email: ts@growthengineai.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyops-0.2.8/README.md` & `lazyops-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/configs/base.py` & `lazyops-0.2.9/lazyops/configs/base.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/configs/cloud.py` & `lazyops-0.2.9/lazyops/configs/cloud.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/configs/k8s.py` & `lazyops-0.2.9/lazyops/configs/k8s.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/imports/_aiohttpx.py` & `lazyops-0.2.9/lazyops/imports/_aiohttpx.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/imports/_aiokeydb.py` & `lazyops-0.2.9/lazyops/imports/_aiokeydb.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/imports/_fileio.py` & `lazyops-0.2.9/lazyops/imports/_fileio.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/imports/_k8s.py` & `lazyops-0.2.9/lazyops/imports/_k8s.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/imports/_psutil.py` & `lazyops-0.2.9/lazyops/imports/_psutil.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/imports/_torch.py` & `lazyops-0.2.9/lazyops/imports/_torch.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/imports/_transformers.py` & `lazyops-0.2.9/lazyops/imports/_transformers.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/types/classprops.py` & `lazyops-0.2.9/lazyops/types/classprops.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/types/common.py` & `lazyops-0.2.9/lazyops/types/common.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/types/formatting.py` & `lazyops-0.2.9/lazyops/types/formatting.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/types/models.py` & `lazyops-0.2.9/lazyops/types/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/utils/__init__.py` & `lazyops-0.2.9/lazyops/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/utils/helpers.py` & `lazyops-0.2.9/lazyops/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/utils/imports.py` & `lazyops-0.2.9/lazyops/utils/imports.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/utils/lazylib.py` & `lazyops-0.2.9/lazyops/utils/lazylib.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/utils/logs.py` & `lazyops-0.2.9/lazyops/utils/logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import warnings
 import atexit as _atexit
 
 from loguru import _defaults
 from loguru._logger import Core as _Core
 from loguru._logger import Logger as _Logger
-from typing import Any
+from typing import Any, Union
 
 # Use this section to filter out warnings from other modules
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = os.getenv('TF_CPP_MIN_LOG_LEVEL', '3')
 warnings.filterwarnings('ignore', message='Unverified HTTPS request')
 warnings.filterwarnings("ignore", message = "Unclosed client session")
 
 
@@ -122,23 +122,25 @@
             exception=record.exc_info
         ).log(level, record.getMessage())
 
 
 class CustomizeLogger:
 
     @classmethod
-    def make_default_logger(cls, level: str = "INFO"):
+    def make_default_logger(cls, level: Union[str, int] = "INFO"):
         # todo adjust this later to use a ConfigModel
+        if isinstance(level, str):
+            level = level.upper()
         logger.remove()
         logger.add(
             sys.stdout,
             enqueue=True,
             backtrace=True,
             colorize=True,
-            level=level.upper(),
+            level=level,
             format=cls.logger_formatter,
         )
         logging.basicConfig(handlers=[InterceptHandler()], level=0)
         *options, extra = logger._options
         return Logger(logger._core, *options, {**extra})
         # return logger
```

### Comparing `lazyops-0.2.8/lazyops/utils/serialization.py` & `lazyops-0.2.9/lazyops/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/utils/system.py` & `lazyops-0.2.9/lazyops/utils/system.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/__init__.py` & `lazyops-0.2.9/lazyops/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/apis.py` & `lazyops-0.2.9/lazyops/v1/apis.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/common.py` & `lazyops-0.2.9/lazyops/v1/common.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/envs.py` & `lazyops-0.2.9/lazyops/v1/envs.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/experimental/gptj.py` & `lazyops-0.2.9/lazyops/v1/experimental/gptj.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyclasses/core.py` & `lazyops-0.2.9/lazyops/v1/lazyclasses/core.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyconfig/_base.py` & `lazyops-0.2.9/lazyops/v1/lazyconfig/_base.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyconfig/nginx.py` & `lazyops-0.2.9/lazyops/v1/lazyconfig/nginx.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyconfig/tfserving.proto` & `lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving.proto`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyconfig/tfserving_api.py` & `lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving_api.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyconfig/tfserving_pb2.py` & `lazyops-0.2.9/lazyops/v1/lazyconfig/tfserving_pb2.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazydatabase/_base.py` & `lazyops-0.2.9/lazyops/v1/lazydatabase/_base.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazydatabase/backends.py` & `lazyops-0.2.9/lazyops/v1/lazydatabase/backends.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazydatabase/core.py` & `lazyops-0.2.9/lazyops/v1/lazydatabase/core.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazydatabase/models.py` & `lazyops-0.2.9/lazyops/v1/lazydatabase/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyio/__init__.py` & `lazyops-0.2.9/lazyops/v1/lazyio/__init__.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyio/async_ops.py` & `lazyops-0.2.9/lazyops/v1/lazyio/async_ops.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyio/models.py` & `lazyops-0.2.9/lazyops/v1/lazyio/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyrpc/README.md` & `lazyops-0.2.9/lazyops/v1/lazyrpc/README.md`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyrpc/__init__.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyrpc/_base.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/_base.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyrpc/core.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/core.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyrpc/dependencies.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/dependencies.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyrpc/exceptions.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazyrpc/models.py` & `lazyops-0.2.9/lazyops/v1/lazyrpc/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazysources/gdelt/README.md` & `lazyops-0.2.9/lazyops/v1/lazysources/gdelt/README.md`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazysources/gdelt/core.py` & `lazyops-0.2.9/lazyops/v1/lazysources/gdelt/core.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazysources/gdelt/filters.py` & `lazyops-0.2.9/lazyops/v1/lazysources/gdelt/filters.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/lazysources/gdelt/models.py` & `lazyops-0.2.9/lazyops/v1/lazysources/gdelt/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/models.py` & `lazyops-0.2.9/lazyops/v1/models.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/mp.py` & `lazyops-0.2.9/lazyops/v1/mp.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/mp_utils.py` & `lazyops-0.2.9/lazyops/v1/mp_utils.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/retry.py` & `lazyops-0.2.9/lazyops/v1/retry.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops/v1/utils.py` & `lazyops-0.2.9/lazyops/v1/utils.py`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/lazyops.egg-info/PKG-INFO` & `lazyops-0.2.9/lazyops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyops
-Version: 0.2.8
+Version: 0.2.9
 Summary: A collection of submodules/patterns that are commonly used within Internal Development
 Home-page: https://github.com/trisongz/lazyops
 Author: Tri Songz
 Author-email: ts@growthengineai.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyops-0.2.8/lazyops.egg-info/SOURCES.txt` & `lazyops-0.2.9/lazyops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyops-0.2.8/setup.py` & `lazyops-0.2.9/setup.py`

 * *Files identical despite different names*

