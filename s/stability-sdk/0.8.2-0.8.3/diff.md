# Comparing `tmp/stability-sdk-0.8.2.tar.gz` & `tmp/stability-sdk-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability-sdk-0.8.2.tar", last modified: Tue Jun 27 23:22:03 2023, max compression
+gzip compressed data, was "stability-sdk-0.8.3.tar", last modified: Fri Jun 30 14:18:41 2023, max compression
```

## Comparing `stability-sdk-0.8.2.tar` & `stability-sdk-0.8.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.810775 stability-sdk-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.810775 stability-sdk-0.8.2/src/stability_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/src/stability_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/src/stability_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55306 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/src/stability_sdk/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    37904 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/src/stability_sdk/animation_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    28265 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/src/stability_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/src/stability_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37427 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/project/
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-27 23:21:46.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.810775 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:21:47.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-27 23:21:47.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-06-27 23:21:47.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:21:47.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-27 23:21:47.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-27 23:21:47.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-27 23:21:47.000000 stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/src/stability_sdk/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/src/stability_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/src/stability_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-27 23:22:03.000000 stability-sdk-0.8.2/src/stability_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-27 23:22:03.000000 stability-sdk-0.8.2/src/stability_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 23:22:03.000000 stability-sdk-0.8.2/src/stability_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 23:22:03.000000 stability-sdk-0.8.2/src/stability_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 23:22:03.000000 stability-sdk-0.8.2/src/stability_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:22:03.814775 stability-sdk-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/tests/test_animator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-27 23:21:44.000000 stability-sdk-0.8.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.019077 stability-sdk-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55475 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37904 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/animation_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28265 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37427 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/tests/test_animator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/tests/test_utils.py
```

### Comparing `stability-sdk-0.8.2/LICENSE` & `stability-sdk-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/PKG-INFO` & `stability-sdk-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.8.2
+Version: 0.8.3
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
@@ -79,20 +79,21 @@
 ## SDK Usage
 
 Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
-usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] [--start_schedule START_SCHEDULE]
-                 [--end_schedule END_SCHEDULE] [--cfg_scale CFG_SCALE] [--sampler SAMPLER]
-                 [--steps STEPS] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
-                 [--num_samples NUM_SAMPLES] [--artifact_types ARTIFACT_TYPES]
-                 [--no-store] [--show] [--init_image INIT_IMAGE] [--mask_image MASK_IMAGE]
-                 [prompt ...]
+usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] 
+                [--start_schedule START_SCHEDULE] [--end_schedule END_SCHEDULE] 
+                [--cfg_scale CFG_SCALE] [--sampler SAMPLER] [--steps STEPS] 
+                [--style_preset STYLE_PRESET] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
+                [--num_samples NUM_SAMPLES] [--artifact_types ARTIFACT_TYPES]
+                [--no-store] [--show] [--init_image INIT_IMAGE] [--mask_image MASK_IMAGE]
+                [prompt ...]
 
 positional arguments:
   prompt
 
 options:
   -h, --help            show this help message and exit
   --height HEIGHT, -H HEIGHT
@@ -107,14 +108,18 @@
   --cfg_scale CFG_SCALE, -C CFG_SCALE
                         [7.0] CFG scale factor
   --sampler SAMPLER, -A SAMPLER
                         [auto-select] (ddim, plms, k_euler, k_euler_ancestral, k_heun, k_dpm_2,
                         k_dpm_2_ancestral, k_lms, k_dpmpp_2m, k_dpmpp_2s_ancestral)
   --steps STEPS, -s STEPS
                         [auto] number of steps
+  --style_preset STYLE_PRESET
+                        [none] (3d-model, analog-film, anime, cinematic, comic-book, digital-art, enhance, 
+                        fantasy-art, isometric, line-art, low-poly, modeling-compound, neon-punk, origami, 
+                        photographic, pixel-art, tile-texture)
   --seed SEED, -S SEED  random seed to use
   --prefix PREFIX, -p PREFIX
                         output prefixes for artifacts
   --artifact_types ARTIFACT_TYPES, -t ARTIFACT_TYPES
                         filter artifacts by type (ARTIFACT_IMAGE, ARTIFACT_TEXT, ARTIFACT_CLASSIFICATIONS, etc)
   --no-store            do not write out artifacts
   --num_samples NUM_SAMPLES, -n NUM_SAMPLES
```

### Comparing `stability-sdk-0.8.2/README.md` & `stability-sdk-0.8.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,20 +44,21 @@
 ## SDK Usage
 
 Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
-usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] [--start_schedule START_SCHEDULE]
-                 [--end_schedule END_SCHEDULE] [--cfg_scale CFG_SCALE] [--sampler SAMPLER]
-                 [--steps STEPS] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
-                 [--num_samples NUM_SAMPLES] [--artifact_types ARTIFACT_TYPES]
-                 [--no-store] [--show] [--init_image INIT_IMAGE] [--mask_image MASK_IMAGE]
-                 [prompt ...]
+usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] 
+                [--start_schedule START_SCHEDULE] [--end_schedule END_SCHEDULE] 
+                [--cfg_scale CFG_SCALE] [--sampler SAMPLER] [--steps STEPS] 
+                [--style_preset STYLE_PRESET] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
+                [--num_samples NUM_SAMPLES] [--artifact_types ARTIFACT_TYPES]
+                [--no-store] [--show] [--init_image INIT_IMAGE] [--mask_image MASK_IMAGE]
+                [prompt ...]
 
 positional arguments:
   prompt
 
 options:
   -h, --help            show this help message and exit
   --height HEIGHT, -H HEIGHT
@@ -72,14 +73,18 @@
   --cfg_scale CFG_SCALE, -C CFG_SCALE
                         [7.0] CFG scale factor
   --sampler SAMPLER, -A SAMPLER
                         [auto-select] (ddim, plms, k_euler, k_euler_ancestral, k_heun, k_dpm_2,
                         k_dpm_2_ancestral, k_lms, k_dpmpp_2m, k_dpmpp_2s_ancestral)
   --steps STEPS, -s STEPS
                         [auto] number of steps
+  --style_preset STYLE_PRESET
+                        [none] (3d-model, analog-film, anime, cinematic, comic-book, digital-art, enhance, 
+                        fantasy-art, isometric, line-art, low-poly, modeling-compound, neon-punk, origami, 
+                        photographic, pixel-art, tile-texture)
   --seed SEED, -S SEED  random seed to use
   --prefix PREFIX, -p PREFIX
                         output prefixes for artifacts
   --artifact_types ARTIFACT_TYPES, -t ARTIFACT_TYPES
                         filter artifacts by type (ARTIFACT_IMAGE, ARTIFACT_TEXT, ARTIFACT_CLASSIFICATIONS, etc)
   --no-store            do not write out artifacts
   --num_samples NUM_SAMPLES, -n NUM_SAMPLES
```

### Comparing `stability-sdk-0.8.2/setup.py` & `stability-sdk-0.8.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 
 with open('README.md','r') as f:
     README = f.read()
 
 setup(
     name='stability-sdk',
-    version='0.8.2',
+    version='0.8.3',
     author='Stability AI',
     author_email='support@stability.ai',
     maintainer='Stability AI',
     maintainer_email='support@stability.ai',
     url='https://beta.dreamstudio.ai/',
     download_url='https://github.com/Stability-AI/stability-sdk/',
     description='Python SDK for interacting with stability.ai APIs',
```

### Comparing `stability-sdk-0.8.2/src/stability_sdk/__main__.py` & `stability-sdk-0.8.3/src/stability_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/animation.py` & `stability-sdk-0.8.3/src/stability_sdk/animation.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,18 @@
         self.start_frame_idx: int = 0
         self.video_prev_frame: Optional[Image.Image] = None
         self.video_reader: Optional[cv2.VideoCapture] = None
 
         # configure Api to retry on classifier obfuscations
         self.api._retry_obfuscation = True
 
+        # two stage 1024 model requires longer timeout
+        if self.args.model.startswith('stable-diffusion-xl-1024'):
+            self.api._request_timeout = 120.0
+
         # create output directory
         if self.out_dir is not None:
             os.makedirs(self.out_dir, exist_ok=True)
         elif self.args.save_depth_maps or self.args.save_inpaint_masks:
             raise ValueError('out_dir must be specified when saving depth maps or inpaint masks')
 
         self.setup_animation(resume)
```

### Comparing `stability-sdk-0.8.2/src/stability_sdk/animation_ui.py` & `stability-sdk-0.8.3/src/stability_sdk/animation_ui.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/api.py` & `stability-sdk-0.8.3/src/stability_sdk/api.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/client.py` & `stability-sdk-0.8.3/src/stability_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         safety: bool = True,
         classifiers: Optional[generation.ClassifierParameters] = None,
         guidance_preset: generation.GuidancePreset = generation.GUIDANCE_PRESET_NONE,
         guidance_cuts: int = 0,
         guidance_strength: Optional[float] = None,
         guidance_prompt: Union[str, generation.Prompt] = None,
         guidance_models: List[str] = None,
+        style_preset: Optional[str] = None
     ) -> Generator[generation.Answer, None, None]:
         """
         Generate images from a prompt.
 
         :param prompt: Prompt to generate images from.
         :param init_image: Init image.
         :param mask_image: Mask image
@@ -190,14 +191,15 @@
         :param safety: DEPRECATED/UNUSED - Cannot be disabled.
         :param classifiers: DEPRECATED/UNUSED - Has no effect on image generation.
         :param guidance_preset: Guidance preset to use. See generation.GuidancePreset for supported values.
         :param guidance_cuts: Number of cuts to use for guidance.
         :param guidance_strength: Strength of the guidance. We recommend values in range [0.0,1.0]. A good default is 0.25
         :param guidance_prompt: Prompt to use for guidance, defaults to `prompt` argument (above) if not specified.
         :param guidance_models: Models to use for guidance.
+        :param style_preset: Style preset name to use (see https://platform.stability.ai/rest-api#tag/v1generation)
         :return: Generator of Answer objects.
         """
         if (prompt is None) and (init_image is None):
             raise ValueError("prompt and/or init_image must be provided")
 
         if (mask_image is not None) and (init_image is None):
             raise ValueError(
@@ -284,15 +286,21 @@
             width=width,
             seed=seed,
             steps=steps,
             samples=samples,
             parameters=[generation.StepParameter(**step_parameters)],
         )
 
-        return self.emit_request(prompt=prompts, image_parameters=image_parameters)
+        if style_preset and style_preset.lower() != 'none':
+            extras = Struct()
+            extras.update({ '$IPC': { "preset": style_preset } })
+        else:
+            extras = None
+
+        return self.emit_request(prompt=prompts, image_parameters=image_parameters, extra_parameters=extras)
     
     def upscale(
         self,
         init_image: Image.Image,
         height: int = None,
         width: int = None,
         prompt: Union[str, generation.Prompt] = None,
@@ -387,17 +395,18 @@
                     logger.info(
                         f"Got keepalive {answer.answer_id} in " f"{duration:0.2f}s"
                     )
 
             yield answer
             start = time.time()
 
-def process_cli(logger: logging.Logger = None,
-                warn_client_call_deprecated: bool = True,
-                ):
+def process_cli(
+    logger: logging.Logger = None,
+    warn_client_call_deprecated: bool = True,
+):
     if not logger:
         logger = logging.getLogger(__name__)
         logger.setLevel(level=logging.INFO)
 
         # Set up logging for output to console.
         fh = logging.StreamHandler()
         fh_formatter = logging.Formatter(
@@ -520,14 +529,15 @@
         help="[auto-select] (" + ", ".join(SAMPLERS.keys()) + ")",
     )
     parser_generate.add_argument(
         "--steps", "-s", type=int, default=None, help="[auto] number of steps"
     )
     parser_generate.add_argument(
         "--seed", "-S", type=int, default=0, help="random seed to use")
+    parser_generate.add_argument("--style_preset", type=str, help="style preset name")
     parser_generate.add_argument(
         "--prefix",
         "-p",
         type=str,
         default="generation_",
         help="output prefixes for artifacts",
     )
@@ -627,14 +637,15 @@
             "start_schedule": args.start_schedule,
             "end_schedule": args.end_schedule,
             "cfg_scale": args.cfg_scale,            
             "seed": args.seed,
             "samples": args.num_samples,
             "init_image": args.init_image,
             "mask_image": args.mask_image,
+            "style_preset": args.style_preset,
         }
 
         if args.sampler:
             request["sampler"] = sampler_from_string(args.sampler)
 
         if args.steps:
             request["steps"] = args.steps
```

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/project/project_pb2.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/project_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/protobuf.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py` & `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/matrix.py` & `stability-sdk-0.8.3/src/stability_sdk/matrix.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk/utils.py` & `stability-sdk-0.8.3/src/stability_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/src/stability_sdk.egg-info/PKG-INFO` & `stability-sdk-0.8.3/src/stability_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.8.2
+Version: 0.8.3
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
@@ -79,20 +79,21 @@
 ## SDK Usage
 
 Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
-usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] [--start_schedule START_SCHEDULE]
-                 [--end_schedule END_SCHEDULE] [--cfg_scale CFG_SCALE] [--sampler SAMPLER]
-                 [--steps STEPS] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
-                 [--num_samples NUM_SAMPLES] [--artifact_types ARTIFACT_TYPES]
-                 [--no-store] [--show] [--init_image INIT_IMAGE] [--mask_image MASK_IMAGE]
-                 [prompt ...]
+usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] 
+                [--start_schedule START_SCHEDULE] [--end_schedule END_SCHEDULE] 
+                [--cfg_scale CFG_SCALE] [--sampler SAMPLER] [--steps STEPS] 
+                [--style_preset STYLE_PRESET] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
+                [--num_samples NUM_SAMPLES] [--artifact_types ARTIFACT_TYPES]
+                [--no-store] [--show] [--init_image INIT_IMAGE] [--mask_image MASK_IMAGE]
+                [prompt ...]
 
 positional arguments:
   prompt
 
 options:
   -h, --help            show this help message and exit
   --height HEIGHT, -H HEIGHT
@@ -107,14 +108,18 @@
   --cfg_scale CFG_SCALE, -C CFG_SCALE
                         [7.0] CFG scale factor
   --sampler SAMPLER, -A SAMPLER
                         [auto-select] (ddim, plms, k_euler, k_euler_ancestral, k_heun, k_dpm_2,
                         k_dpm_2_ancestral, k_lms, k_dpmpp_2m, k_dpmpp_2s_ancestral)
   --steps STEPS, -s STEPS
                         [auto] number of steps
+  --style_preset STYLE_PRESET
+                        [none] (3d-model, analog-film, anime, cinematic, comic-book, digital-art, enhance, 
+                        fantasy-art, isometric, line-art, low-poly, modeling-compound, neon-punk, origami, 
+                        photographic, pixel-art, tile-texture)
   --seed SEED, -S SEED  random seed to use
   --prefix PREFIX, -p PREFIX
                         output prefixes for artifacts
   --artifact_types ARTIFACT_TYPES, -t ARTIFACT_TYPES
                         filter artifacts by type (ARTIFACT_IMAGE, ARTIFACT_TEXT, ARTIFACT_CLASSIFICATIONS, etc)
   --no-store            do not write out artifacts
   --num_samples NUM_SAMPLES, -n NUM_SAMPLES
```

### Comparing `stability-sdk-0.8.2/src/stability_sdk.egg-info/SOURCES.txt` & `stability-sdk-0.8.3/src/stability_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/tests/test_animator.py` & `stability-sdk-0.8.3/tests/test_animator.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/tests/test_api.py` & `stability-sdk-0.8.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/tests/test_client.py` & `stability-sdk-0.8.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.2/tests/test_utils.py` & `stability-sdk-0.8.3/tests/test_utils.py`

 * *Files identical despite different names*

