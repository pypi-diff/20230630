# Comparing `tmp/tvdcn-0.2.7.tar.gz` & `tmp/tvdcn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.2.7.tar", last modified: Sun Jun  4 20:31:18 2023, max compression
+gzip compressed data, was "tvdcn-0.3.0.tar", last modified: Fri Jun 30 15:54:22 2023, max compression
```

## Comparing `tvdcn-0.2.7.tar` & `tvdcn-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.596329 tvdcn-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-04 20:29:30.000000 tvdcn-0.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-04 20:29:30.000000 tvdcn-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-04 20:31:18.596329 tvdcn-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-04 20:29:30.000000 tvdcn-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-04 20:29:30.000000 tvdcn-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 20:29:30.000000 tvdcn-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-04 20:31:18.596329 tvdcn-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-04 20:29:30.000000 tvdcn-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.584329 tvdcn-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.584329 tvdcn-0.2.7/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.584329 tvdcn-0.2.7/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.588328 tvdcn-0.2.7/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.592329 tvdcn-0.2.7/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.592329 tvdcn-0.2.7/tvdcn/csrc/ops/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)    23154 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    29884 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    38246 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    29905 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30898 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35780 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.592329 tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.596329 tvdcn-0.2.7/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.596329 tvdcn-0.2.7/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    36102 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    39157 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.584329 tvdcn-0.2.7/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.044675 tvdcn-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 15:52:27.000000 tvdcn-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 15:52:27.000000 tvdcn-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-30 15:54:22.044675 tvdcn-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-30 15:52:27.000000 tvdcn-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-30 15:52:27.000000 tvdcn-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 15:52:27.000000 tvdcn-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 15:54:22.048675 tvdcn-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-30 15:52:27.000000 tvdcn-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.032675 tvdcn-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.032675 tvdcn-0.3.0/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.036675 tvdcn-0.3.0/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.036675 tvdcn-0.3.0/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.040675 tvdcn-0.3.0/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27047 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35454 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.040675 tvdcn-0.3.0/tvdcn/csrc/ops/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)    23346 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    30172 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    38630 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    26844 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30614 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27619 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31385 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.044675 tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.044675 tvdcn-0.3.0/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.044675 tvdcn-0.3.0/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31021 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34045 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.036675 tvdcn-0.3.0/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.2.7/LICENSE.txt` & `tvdcn-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/PKG-INFO` & `tvdcn-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.7
+Version: 0.3.0
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.2.7/README.md` & `tvdcn-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/pyproject.toml` & `tvdcn-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/setup.cfg` & `tvdcn-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/setup.py` & `tvdcn-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.3.0/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/tests/test_grad.py` & `tvdcn-0.3.0/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -138,30 +138,30 @@
             }
         }
 
         void arr2col_cpu(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     input.scalar_type(), "arr2col_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto columns_accessor =
                             columns.accessor<scalar_t, 4>();
                     TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
@@ -227,30 +227,30 @@
             }
         }
 
         void col2arr_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "col2arr_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
                     auto grad_input_accessor =
                             grad_input.accessor<scalar_t, 3>();
                     TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
@@ -321,31 +321,31 @@
         }
 
         void deform_conv1d_compute_grad_offset_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (!deformable) return;
             const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv1d_compute_grad_offset_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto grad_offset_accessor =
                             grad_offset.accessor<scalar_t, 5>();
                     TVDCN_DISPATCH_CONDITION(modulated, ([&] {
@@ -415,31 +415,31 @@
             }
         }
 
         void deform_conv1d_compute_grad_mask_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (!modulated) return;
             const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv1d_compute_grad_mask_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto grad_mask_accessor =
                             grad_mask.accessor<scalar_t, 4>();
                     TVDCN_DISPATCH_CONDITION(deformable, ([&] {
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #include <ATen/ATen.h>
-#include "cpu_helpers.h"
+#include "cuda_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
+            constexpr float threadsFraction = 0.75;
+
             template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t sample(
-                    const at::TensorAccessor<scalar_t, 4> input,
+            __device__ __forceinline__ scalar_t sample(
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const index_t y,
                     const index_t x) {
                 return (0 <= y && y < height && 0 <= x && x < width) ? input[b][c][y][x] : static_cast<scalar_t>(0);
             }
 
             template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t interpolate_sample(
-                    const at::TensorAccessor<scalar_t, 4> input,
+            __device__ __forceinline__ scalar_t interpolate_sample(
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const scalar_t y,
                     const scalar_t x) {
                 if (y <= -1 || height <= y || x <= -1 || width <= x)
@@ -49,30 +51,30 @@
                 if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
                 if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
                 if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
                 return val;
             }
 
             template<typename scalar_t, typename index_t>
-            __forceinline__ void insert(
-                    at::TensorAccessor<scalar_t, 4> output,
+            __device__ __forceinline__ void insert(
+                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> output,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const index_t y,
                     const index_t x,
                     const scalar_t val) {
                 if (0 <= y && y < height && 0 <= x && x < width)
-                    output[b][c][y][x] += val;
+                    gpuAtomicAdd(&output[b][c][y][x], val);
             }
 
             template<typename scalar_t, typename index_t>
-            __forceinline__ void interpolate_insert(
-                    at::TensorAccessor<scalar_t, 4> output,
+            __device__ __forceinline__ void interpolate_insert(
+                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> output,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const scalar_t y,
                     const scalar_t x,
                     const scalar_t val) {
@@ -87,23 +89,23 @@
                 scalar_t dx_l = 1 - dx_h;
 
                 bool valid_y_l = 0 <= y_l && y_l < height;
                 bool valid_y_h = 0 <= y_h && y_h < height;
                 bool valid_x_l = 0 <= x_l && x_l < width;
                 bool valid_x_h = 0 <= x_h && x_h < width;
 
-                if (valid_y_l && valid_x_l) output[b][c][y_l][x_l] += dy_l * dx_l * val;
-                if (valid_y_l && valid_x_h) output[b][c][y_l][x_h] += dy_l * dx_h * val;
-                if (valid_y_h && valid_x_l) output[b][c][y_h][x_l] += dy_h * dx_l * val;
-                if (valid_y_h && valid_x_h) output[b][c][y_h][x_h] += dy_h * dx_h * val;
+                if (valid_y_l && valid_x_l) gpuAtomicAdd(&output[b][c][y_l][x_l], dy_l * dx_l * val);
+                if (valid_y_l && valid_x_h) gpuAtomicAdd(&output[b][c][y_l][x_h], dy_l * dx_h * val);
+                if (valid_y_h && valid_x_l) gpuAtomicAdd(&output[b][c][y_h][x_l], dy_h * dx_l * val);
+                if (valid_y_h && valid_x_h) gpuAtomicAdd(&output[b][c][y_h][x_h], dy_h * dx_h * val);
             }
 
             template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t coordinate_weight(
-                    const at::TensorAccessor<scalar_t, 4> input,
+            __device__ __forceinline__ scalar_t coordinate_weight(
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const scalar_t y,
                     const scalar_t x,
                     const index_t direction) {
@@ -128,19 +130,19 @@
                 if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
                 if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
                 return val;
             }
         }
 
         template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static void im2col_kernel(
+        static __global__ void im2col_kernel(
                 const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
+                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
+                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
                 const index_t stride_h,
                 const index_t stride_w,
                 const index_t pad_h,
@@ -148,16 +150,16 @@
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t in_channels,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 6> columns) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns) {
+            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t w = index % out_w;
                 const index_t h = (index / out_w) % out_h;
                 const index_t c = (index / (out_w * out_h)) % in_channels;
                 const index_t b = index / (out_w * out_h * in_channels);
 
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
@@ -180,52 +182,56 @@
 
                         columns[c][i][j][b][h][w] = val * mask_val;
                     }
                 }
             }
         }
 
-        void im2col_cpu(
+        void im2col_cuda(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
+            at::cuda::CUDAGuard device_guard(input.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+            const unsigned int threads = GET_THREADS(threadsFraction);
+            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "im2col_cpu", ([&] {
+                    input.scalar_type(), "im2col_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto columns_accessor =
-                            columns.accessor<scalar_t, 6>();
+                            columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>();
                     TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        im2col_kernel<deformable, modulated, scalar_t, index_t>(
+                        im2col_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
                                 n_kernels,
-                                input.accessor<scalar_t, 4>(),
-                                offset.accessor<scalar_t, 7>(),
-                                mask.accessor<scalar_t, 6>(),
+                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
+                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
                                 stride_h,
                                 stride_w,
                                 pad_h,
@@ -237,22 +243,23 @@
                                 in_channels,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 columns_accessor);
                     }));
                 }));
             }));
+            C10_CUDA_KERNEL_LAUNCH_CHECK();
         }
 
         template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static void col2im_kernel(
+        static __global__ void col2im_kernel(
                 const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
+                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
+                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
+                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
                 const index_t in_channels,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
                 const index_t stride_h,
                 const index_t stride_w,
@@ -260,16 +267,16 @@
                 const index_t pad_w,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 4> grad_input) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> grad_input) {
+            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t j = index % weight_w;
                 const index_t i = (index / weight_w) % weight_h;
                 const index_t w = (index / (weight_w * weight_h)) % out_w;
                 const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
                 const index_t c = (index / (weight_w * weight_h * out_w * out_h)) % in_channels;
                 const index_t b = (index / (weight_w * weight_h * out_w * out_h * in_channels));
 
@@ -291,52 +298,56 @@
                             x + offset[b][offset_group_idx][i][j][1][h][w],
                             val);
                 else
                     insert(grad_input, b, c, height, width, y, x, val);
             }
         }
 
-        void col2im_cpu(
+        void col2im_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
+            at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+            const unsigned int threads = GET_THREADS(threadsFraction);
+            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2im_cpu", ([&] {
+                    columns.scalar_type(), "col2im_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
                     auto grad_input_accessor =
-                            grad_input.accessor<scalar_t, 4>();
+                            grad_input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>();
                     TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        col2im_kernel<deformable, modulated, scalar_t, index_t>(
+                        col2im_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
                                 n_kernels,
-                                columns.accessor<scalar_t, 6>(),
-                                offset.accessor<scalar_t, 7>(),
-                                mask.accessor<scalar_t, 6>(),
+                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
+                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
                                 in_channels,
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
                                 stride_h,
                                 stride_w,
@@ -348,23 +359,24 @@
                                 out_w,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_input_accessor);
                     }));
                 }));
             }));
+            C10_CUDA_KERNEL_LAUNCH_CHECK();
         }
 
         template<bool modulated, typename scalar_t, typename index_t>
-        static void deform_conv2d_compute_grad_offset_kernel(
+        static __global__ void deform_conv2d_compute_grad_offset_kernel(
                 const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
+                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
+                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
+                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
                 const index_t stride_h,
                 const index_t stride_w,
                 const index_t pad_h,
@@ -372,16 +384,16 @@
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t offset_groups,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 7> grad_offset) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> grad_offset) {
+            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t o = index % 2;
                 const index_t j = (index / 2) % weight_w;
                 const index_t i = (index / (2 * weight_w)) % weight_h;
                 const index_t w = (index / (2 * weight_w * weight_h)) % out_w;
                 const index_t h = (index / (2 * weight_w * weight_h * out_w)) % out_h;
                 const index_t g = (index / (2 * weight_w * weight_h * out_w * out_h)) % offset_groups;
                 const index_t b = index / (2 * weight_w * weight_h * out_w * out_h * offset_groups);
@@ -408,55 +420,59 @@
                     grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
             }
         }
 
-        void deform_conv2d_compute_grad_offset_cpu(
+        void deform_conv2d_compute_grad_offset_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (!deformable) return;
+            at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_h * out_w * weight_h * weight_w * 2;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+            const unsigned int threads = GET_THREADS(threadsFraction);
+            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_offset_cpu", ([&] {
+                    columns.scalar_type(), "deform_conv2d_compute_grad_offset_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto grad_offset_accessor =
-                            grad_offset.accessor<scalar_t, 7>();
+                            grad_offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>();
                     TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                        deform_conv2d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
+                        deform_conv2d_compute_grad_offset_kernel<modulated, scalar_t, index_t><<<blocks, threads>>>(
                                 n_kernels,
-                                columns.accessor<scalar_t, 6>(),
-                                input.accessor<scalar_t, 4>(),
-                                offset.accessor<scalar_t, 7>(),
-                                mask.accessor<scalar_t, 6>(),
+                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
+                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
                                 stride_h,
                                 stride_w,
                                 pad_h,
@@ -468,22 +484,23 @@
                                 offset_groups,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_offset_accessor);
                     }));
                 }));
             }));
+            C10_CUDA_KERNEL_LAUNCH_CHECK();
         }
 
         template<bool deformable, typename scalar_t, typename index_t>
-        static void deform_conv2d_compute_grad_mask_kernel(
+        static __global__ void deform_conv2d_compute_grad_mask_kernel(
                 const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
+                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
+                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
                 const index_t stride_h,
                 const index_t stride_w,
                 const index_t pad_h,
@@ -491,16 +508,16 @@
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t mask_groups,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 6> grad_mask) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> grad_mask) {
+            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t j = index % weight_w;
                 const index_t i = (index / weight_w) % weight_h;
                 const index_t w = (index / (weight_w * weight_h)) % out_w;
                 const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
                 const index_t g = (index / (weight_w * weight_h * out_w * out_h)) % mask_groups;
                 const index_t b = index / (out_w * out_h * weight_w * weight_h * mask_groups);
 
@@ -525,53 +542,57 @@
                     grad_mask_val += columns[c][i][j][b][h][w] * val;
                 }
 
                 grad_mask[b][g][i][j][h][w] = grad_mask_val;
             }
         }
 
-        void deform_conv2d_compute_grad_mask_cpu(
+        void deform_conv2d_compute_grad_mask_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (!modulated) return;
+            at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_h * out_w * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+            const unsigned int threads = GET_THREADS(threadsFraction);
+            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_mask_cpu", ([&] {
+                    columns.scalar_type(), "deform_conv2d_compute_grad_mask_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto grad_mask_accessor =
-                            grad_mask.accessor<scalar_t, 6>();
+                            grad_mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>();
                     TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                        deform_conv2d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
+                        deform_conv2d_compute_grad_mask_kernel<deformable, scalar_t, index_t><<<blocks, threads>>>(
                                 n_kernels,
-                                columns.accessor<scalar_t, 6>(),
-                                input.accessor<scalar_t, 4>(),
-                                offset.accessor<scalar_t, 7>(),
+                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
                                 stride_h,
                                 stride_w,
                                 pad_h,
@@ -583,10 +604,11 @@
                                 mask_groups,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_mask_accessor);
                     }));
                 }));
             }));
+            C10_CUDA_KERNEL_LAUNCH_CHECK();
         }
     }
 }
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -261,42 +261,42 @@
             }
         }
 
         void vol2col_cpu(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_d * out_h * out_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     input.scalar_type(), "vol2col_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto columns_accessor =
                             columns.accessor<scalar_t, 8>();
                     TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
@@ -394,43 +394,43 @@
             }
         }
 
         void col2vol_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             const int64_t n_kernels =
                     (int64_t) batch_sz * in_channels * out_d * out_h * out_w * weight_d * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "col2vol_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
                     auto grad_input_accessor =
                             grad_input.accessor<scalar_t, 5>();
                     TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
@@ -537,44 +537,44 @@
         }
 
         void deform_conv3d_compute_grad_offset_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (!deformable) return;
             const int64_t n_kernels =
                     (int64_t) batch_sz * offset_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w * 3;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv3d_compute_grad_offset_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto grad_offset_accessor =
                             grad_offset.accessor<scalar_t, 9>();
                     TVDCN_DISPATCH_CONDITION(modulated, ([&] {
@@ -676,44 +676,44 @@
             }
         }
 
         void deform_conv3d_compute_grad_mask_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (!modulated) return;
             const int64_t n_kernels =
                     (int64_t) batch_sz * mask_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv3d_compute_grad_mask_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto grad_mask_accessor =
                             grad_mask.accessor<scalar_t, 8>();
                     TVDCN_DISPATCH_CONDITION(deformable, ([&] {
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu` & `tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu`

 * *Files 3% similar despite different names*

```diff
@@ -140,31 +140,31 @@
             }
         }
 
         void arr2col_cuda(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             at::cuda::CUDAGuard device_guard(input.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             const unsigned int threads = GET_THREADS(threadsFraction);
             const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     input.scalar_type(), "arr2col_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
@@ -234,31 +234,31 @@
             }
         }
 
         void col2arr_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             const unsigned int threads = GET_THREADS(threadsFraction);
             const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "col2arr_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
@@ -333,32 +333,32 @@
         }
 
         void deform_conv1d_compute_grad_offset_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (!deformable) return;
             at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             const unsigned int threads = GET_THREADS(threadsFraction);
             const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv1d_compute_grad_offset_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
@@ -432,32 +432,32 @@
             }
         }
 
         void deform_conv1d_compute_grad_mask_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (!modulated) return;
             at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_w * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             const unsigned int threads = GET_THREADS(threadsFraction);
             const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv1d_compute_grad_mask_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu` & `tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #include <ATen/ATen.h>
-#include "cuda_helpers.h"
+#include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
-            constexpr float threadsFraction = 0.75;
-
             template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t sample(
-                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+            __forceinline__ scalar_t sample(
+                    const at::TensorAccessor<scalar_t, 4> input,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const index_t y,
                     const index_t x) {
                 return (0 <= y && y < height && 0 <= x && x < width) ? input[b][c][y][x] : static_cast<scalar_t>(0);
             }
 
             template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t interpolate_sample(
-                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+            __forceinline__ scalar_t interpolate_sample(
+                    const at::TensorAccessor<scalar_t, 4> input,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const scalar_t y,
                     const scalar_t x) {
                 if (y <= -1 || height <= y || x <= -1 || width <= x)
@@ -51,30 +49,30 @@
                 if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
                 if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
                 if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
                 return val;
             }
 
             template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ void insert(
-                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> output,
+            __forceinline__ void insert(
+                    at::TensorAccessor<scalar_t, 4> output,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const index_t y,
                     const index_t x,
                     const scalar_t val) {
                 if (0 <= y && y < height && 0 <= x && x < width)
-                    gpuAtomicAdd(&output[b][c][y][x], val);
+                    output[b][c][y][x] += val;
             }
 
             template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ void interpolate_insert(
-                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> output,
+            __forceinline__ void interpolate_insert(
+                    at::TensorAccessor<scalar_t, 4> output,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const scalar_t y,
                     const scalar_t x,
                     const scalar_t val) {
@@ -89,23 +87,23 @@
                 scalar_t dx_l = 1 - dx_h;
 
                 bool valid_y_l = 0 <= y_l && y_l < height;
                 bool valid_y_h = 0 <= y_h && y_h < height;
                 bool valid_x_l = 0 <= x_l && x_l < width;
                 bool valid_x_h = 0 <= x_h && x_h < width;
 
-                if (valid_y_l && valid_x_l) gpuAtomicAdd(&output[b][c][y_l][x_l], dy_l * dx_l * val);
-                if (valid_y_l && valid_x_h) gpuAtomicAdd(&output[b][c][y_l][x_h], dy_l * dx_h * val);
-                if (valid_y_h && valid_x_l) gpuAtomicAdd(&output[b][c][y_h][x_l], dy_h * dx_l * val);
-                if (valid_y_h && valid_x_h) gpuAtomicAdd(&output[b][c][y_h][x_h], dy_h * dx_h * val);
+                if (valid_y_l && valid_x_l) output[b][c][y_l][x_l] += dy_l * dx_l * val;
+                if (valid_y_l && valid_x_h) output[b][c][y_l][x_h] += dy_l * dx_h * val;
+                if (valid_y_h && valid_x_l) output[b][c][y_h][x_l] += dy_h * dx_l * val;
+                if (valid_y_h && valid_x_h) output[b][c][y_h][x_h] += dy_h * dx_h * val;
             }
 
             template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t coordinate_weight(
-                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+            __forceinline__ scalar_t coordinate_weight(
+                    const at::TensorAccessor<scalar_t, 4> input,
                     const index_t b,
                     const index_t c,
                     const index_t height,
                     const index_t width,
                     const scalar_t y,
                     const scalar_t x,
                     const index_t direction) {
@@ -130,19 +128,19 @@
                 if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
                 if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
                 return val;
             }
         }
 
         template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static __global__ void im2col_kernel(
+        static void im2col_kernel(
                 const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
+                const at::TensorAccessor<scalar_t, 4> input,
+                const at::TensorAccessor<scalar_t, 7> offset,
+                const at::TensorAccessor<scalar_t, 6> mask,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
                 const index_t stride_h,
                 const index_t stride_w,
                 const index_t pad_h,
@@ -150,16 +148,16 @@
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t in_channels,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                at::TensorAccessor<scalar_t, 6> columns) {
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t w = index % out_w;
                 const index_t h = (index / out_w) % out_h;
                 const index_t c = (index / (out_w * out_h)) % in_channels;
                 const index_t b = index / (out_w * out_h * in_channels);
 
                 const index_t offset_group_idx = c / c_per_offset_group;
                 const index_t mask_group_idx = c / c_per_mask_group;
@@ -182,56 +180,52 @@
 
                         columns[c][i][j][b][h][w] = val * mask_val;
                     }
                 }
             }
         }
 
-        void im2col_cuda(
+        void im2col_cpu(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
-            at::cuda::CUDAGuard device_guard(input.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "im2col_cuda", ([&] {
+                    input.scalar_type(), "im2col_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto columns_accessor =
-                            columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>();
+                            columns.accessor<scalar_t, 6>();
                     TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        im2col_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
+                        im2col_kernel<deformable, modulated, scalar_t, index_t>(
                                 n_kernels,
-                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                input.accessor<scalar_t, 4>(),
+                                offset.accessor<scalar_t, 7>(),
+                                mask.accessor<scalar_t, 6>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
                                 stride_h,
                                 stride_w,
                                 pad_h,
@@ -243,23 +237,22 @@
                                 in_channels,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 columns_accessor);
                     }));
                 }));
             }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
         }
 
         template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static __global__ void col2im_kernel(
+        static void col2im_kernel(
                 const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
+                const at::TensorAccessor<scalar_t, 6> columns,
+                const at::TensorAccessor<scalar_t, 7> offset,
+                const at::TensorAccessor<scalar_t, 6> mask,
                 const index_t in_channels,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
                 const index_t stride_h,
                 const index_t stride_w,
@@ -267,16 +260,16 @@
                 const index_t pad_w,
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> grad_input) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                at::TensorAccessor<scalar_t, 4> grad_input) {
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t j = index % weight_w;
                 const index_t i = (index / weight_w) % weight_h;
                 const index_t w = (index / (weight_w * weight_h)) % out_w;
                 const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
                 const index_t c = (index / (weight_w * weight_h * out_w * out_h)) % in_channels;
                 const index_t b = (index / (weight_w * weight_h * out_w * out_h * in_channels));
 
@@ -298,56 +291,52 @@
                             x + offset[b][offset_group_idx][i][j][1][h][w],
                             val);
                 else
                     insert(grad_input, b, c, height, width, y, x, val);
             }
         }
 
-        void col2im_cuda(
+        void col2im_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
-            at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2im_cuda", ([&] {
+                    columns.scalar_type(), "col2im_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
                     auto grad_input_accessor =
-                            grad_input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>();
+                            grad_input.accessor<scalar_t, 4>();
                     TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        col2im_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
+                        col2im_kernel<deformable, modulated, scalar_t, index_t>(
                                 n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                columns.accessor<scalar_t, 6>(),
+                                offset.accessor<scalar_t, 7>(),
+                                mask.accessor<scalar_t, 6>(),
                                 in_channels,
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
                                 stride_h,
                                 stride_w,
@@ -359,24 +348,23 @@
                                 out_w,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_input_accessor);
                     }));
                 }));
             }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
         }
 
         template<bool modulated, typename scalar_t, typename index_t>
-        static __global__ void deform_conv2d_compute_grad_offset_kernel(
+        static void deform_conv2d_compute_grad_offset_kernel(
                 const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
+                const at::TensorAccessor<scalar_t, 6> columns,
+                const at::TensorAccessor<scalar_t, 4> input,
+                const at::TensorAccessor<scalar_t, 7> offset,
+                const at::TensorAccessor<scalar_t, 6> mask,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
                 const index_t stride_h,
                 const index_t stride_w,
                 const index_t pad_h,
@@ -384,16 +372,16 @@
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t offset_groups,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> grad_offset) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                at::TensorAccessor<scalar_t, 7> grad_offset) {
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t o = index % 2;
                 const index_t j = (index / 2) % weight_w;
                 const index_t i = (index / (2 * weight_w)) % weight_h;
                 const index_t w = (index / (2 * weight_w * weight_h)) % out_w;
                 const index_t h = (index / (2 * weight_w * weight_h * out_w)) % out_h;
                 const index_t g = (index / (2 * weight_w * weight_h * out_w * out_h)) % offset_groups;
                 const index_t b = index / (2 * weight_w * weight_h * out_w * out_h * offset_groups);
@@ -420,59 +408,55 @@
                     grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
                 }
 
                 grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
             }
         }
 
-        void deform_conv2d_compute_grad_offset_cuda(
+        void deform_conv2d_compute_grad_offset_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (!deformable) return;
-            at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_h * out_w * weight_h * weight_w * 2;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_offset_cuda", ([&] {
+                    columns.scalar_type(), "deform_conv2d_compute_grad_offset_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto grad_offset_accessor =
-                            grad_offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>();
+                            grad_offset.accessor<scalar_t, 7>();
                     TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                        deform_conv2d_compute_grad_offset_kernel<modulated, scalar_t, index_t><<<blocks, threads>>>(
+                        deform_conv2d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
                                 n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                columns.accessor<scalar_t, 6>(),
+                                input.accessor<scalar_t, 4>(),
+                                offset.accessor<scalar_t, 7>(),
+                                mask.accessor<scalar_t, 6>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
                                 stride_h,
                                 stride_w,
                                 pad_h,
@@ -484,23 +468,22 @@
                                 offset_groups,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_offset_accessor);
                     }));
                 }));
             }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
         }
 
         template<bool deformable, typename scalar_t, typename index_t>
-        static __global__ void deform_conv2d_compute_grad_mask_kernel(
+        static void deform_conv2d_compute_grad_mask_kernel(
                 const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
+                const at::TensorAccessor<scalar_t, 6> columns,
+                const at::TensorAccessor<scalar_t, 4> input,
+                const at::TensorAccessor<scalar_t, 7> offset,
                 const index_t height,
                 const index_t width,
                 const index_t weight_h,
                 const index_t weight_w,
                 const index_t stride_h,
                 const index_t stride_w,
                 const index_t pad_h,
@@ -508,16 +491,16 @@
                 const index_t dilation_h,
                 const index_t dilation_w,
                 const index_t out_h,
                 const index_t out_w,
                 const index_t mask_groups,
                 const index_t c_per_offset_group,
                 const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> grad_mask) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                at::TensorAccessor<scalar_t, 6> grad_mask) {
+            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
                 const index_t j = index % weight_w;
                 const index_t i = (index / weight_w) % weight_h;
                 const index_t w = (index / (weight_w * weight_h)) % out_w;
                 const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
                 const index_t g = (index / (weight_w * weight_h * out_w * out_h)) % mask_groups;
                 const index_t b = index / (out_w * out_h * weight_w * weight_h * mask_groups);
 
@@ -542,57 +525,53 @@
                     grad_mask_val += columns[c][i][j][b][h][w] * val;
                 }
 
                 grad_mask[b][g][i][j][h][w] = grad_mask_val;
             }
         }
 
-        void deform_conv2d_compute_grad_mask_cuda(
+        void deform_conv2d_compute_grad_mask_cpu(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (!modulated) return;
-            at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_h * out_w * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_mask_cuda", ([&] {
+                    columns.scalar_type(), "deform_conv2d_compute_grad_mask_cpu", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
                     auto grad_mask_accessor =
-                            grad_mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>();
+                            grad_mask.accessor<scalar_t, 6>();
                     TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                        deform_conv2d_compute_grad_mask_kernel<deformable, scalar_t, index_t><<<blocks, threads>>>(
+                        deform_conv2d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
                                 n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
+                                columns.accessor<scalar_t, 6>(),
+                                input.accessor<scalar_t, 4>(),
+                                offset.accessor<scalar_t, 7>(),
                                 height,
                                 width,
                                 weight_h,
                                 weight_w,
                                 stride_h,
                                 stride_w,
                                 pad_h,
@@ -604,11 +583,10 @@
                                 mask_groups,
                                 c_per_offset_group,
                                 c_per_mask_group,
                                 grad_mask_accessor);
                     }));
                 }));
             }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
         }
     }
 }
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu` & `tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu`

 * *Files 2% similar despite different names*

```diff
@@ -263,43 +263,43 @@
             }
         }
 
         void vol2col_cuda(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             at::cuda::CUDAGuard device_guard(input.get_device());
             const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_d * out_h * out_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             const unsigned int threads = GET_THREADS(threadsFraction);
             const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     input.scalar_type(), "vol2col_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
@@ -401,44 +401,44 @@
             }
         }
 
         void col2vol_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels =
                     (int64_t) batch_sz * in_channels * out_d * out_h * out_w * weight_d * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             const unsigned int threads = GET_THREADS(threadsFraction);
             const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "col2vol_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
@@ -549,45 +549,45 @@
         }
 
         void deform_conv3d_compute_grad_offset_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (!deformable) return;
             at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels =
                     (int64_t) batch_sz * offset_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w * 3;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             const unsigned int threads = GET_THREADS(threadsFraction);
             const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv3d_compute_grad_offset_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
@@ -693,45 +693,45 @@
             }
         }
 
         void deform_conv3d_compute_grad_mask_cuda(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (!modulated) return;
             at::cuda::CUDAGuard device_guard(columns.get_device());
             const int64_t n_kernels =
                     (int64_t) batch_sz * mask_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w;
-            const int c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
 
             const unsigned int threads = GET_THREADS(threadsFraction);
             const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
 
             AT_DISPATCH_FLOATING_TYPES_AND_HALF(
                     columns.scalar_type(), "deform_conv3d_compute_grad_mask_cuda", ([&] {
                 TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -77,22 +77,20 @@
     namespace ops {
         at::Tensor deform_conv1d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const int stride,
-                const int padding,
-                const int dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                at::IntArrayRef stride,
+                at::IntArrayRef padding,
+                at::IntArrayRef dilation,
+                int64_t groups,
+                bool deformable,
+                bool modulated) {
             at::CheckedFrom c = "deform_conv1d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
@@ -103,49 +101,66 @@
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 3)
+            TORCH_CHECK(weight_c.ndimension() == 3)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
-            TORCH_CHECK(weight_c.ndimension() == 3)
 
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_w = input_c.size(2);
+            int64_t batch_sz = input_c.size(0);
+            int64_t in_channels = input_c.size(1);
+            int64_t in_w = input_c.size(2);
 
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(0);
-            int weight_w = weight_c.size(2);
+            int64_t out_channels = weight_c.size(0);
+            int64_t weight_w = weight_c.size(2);
 
-            int stride_w = stride;
+            int64_t stride_w = stride[0];
 
-            int pad_w = padding;
+            int64_t pad_w = padding[0];
 
-            int dilation_w = dilation;
+            int64_t dilation_w = dilation[0];
 
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+            int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
             TORCH_CHECK(
                     weight_w > 0,
                     " weight_w: ",
                     weight_w)
             TORCH_CHECK(
                     stride_w > 0,
                     " stride_w: ",
                     stride_w)
             TORCH_CHECK(pad_w >= 0, " pad_w: ", pad_w)
             TORCH_CHECK(dilation_w > 0, " dilation_w: ", dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+            int64_t offset_groups = offset.size(1) / weight_w;
+            int64_t mask_groups = mask.size(1) / weight_w;
+
+            TORCH_CHECK(!deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2).\nGot offset.size(1)=",
+                        offset.size(1),
+                        ", while weight.size(2)=",
+                        weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+
+            TORCH_CHECK(!modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2).\nGot mask.size(1)=",
+                        mask.size(1),
+                        ", while weight.size(2)=",
+                        weight_w)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
@@ -239,15 +254,15 @@
                                       in_channels * weight_w / groups,
                                       n_parallel_imgs * out_w},
                                      input_c.options());
             auto columns_view = columns.view({in_channels,
                                               weight_w,
                                               n_parallel_imgs,
                                               out_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
+            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 arr2col(
                         input_c[b],
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_w,
                         weight_w,
@@ -258,15 +273,15 @@
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
-                for (int g = 0; g < groups; g++) {
+                for (int64_t g = 0; g < groups; g++) {
                     output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
                 }
             }
 
             output_buf = output_buf.view({batch_sz / n_parallel_imgs,
                                           out_channels,
                                           n_parallel_imgs,
@@ -274,248 +289,245 @@
             output_buf.transpose_(1, 2);
             output.copy_(output_buf);
             output = output.view({batch_sz, out_channels, out_w});
 
             return output + bias_c.view({1, out_channels, 1});
         }
 
-        std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv1d_backward(
-                const at::Tensor &grad_out,
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const int stride,
-                const int padding,
-                const int dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
-            at::Tensor grad_out_c = grad_out.contiguous();
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_w = input_c.size(2);
-
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int out_channels = weight_c.size(0);
-            int weight_w = weight_c.size(2);
-
-            int stride_w = stride;
-
-            int pad_w = padding;
-
-            int dilation_w = dilation;
-
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
-
-            auto grad_input = at::zeros_like(input_c);
-            auto grad_weight = at::zeros_like(weight_c);
-            auto grad_offset = at::zeros_like(offset_c);
-            auto grad_mask = at::zeros_like(mask_c);
-            auto grad_bias = at::ones_like(bias_c);
-
-            // Separate into blocks
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_w});
-            grad_input = grad_input.view_as(input_c);
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+        namespace detail {
+            std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
+            _deform_conv1d_backward(
+                    const at::Tensor &grad_out,
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const at::Tensor &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups,
+                    bool deformable,
+                    bool modulated) {
+                at::Tensor grad_out_c = grad_out.contiguous();
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = offset.contiguous();
+                at::Tensor mask_c = mask.contiguous();
+                at::Tensor bias_c = bias.contiguous();
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_w = input_c.size(2);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(0);
+                int64_t weight_w = weight_c.size(2);
+
+                int64_t stride_w = stride[0];
+
+                int64_t pad_w = padding[0];
+
+                int64_t dilation_w = dilation[0];
+
+                int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+
+                int64_t offset_groups = offset.size(1) / weight_w;
+                int64_t mask_groups = mask.size(1) / weight_w;
+
+                auto grad_input = at::zeros_like(input_c);
+                auto grad_weight = at::zeros_like(weight_c);
+                auto grad_offset = at::zeros_like(offset_c);
+                auto grad_mask = at::zeros_like(mask_c);
+                auto grad_bias = at::ones_like(bias_c);
+
+                // Separate into blocks
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_w});
+                grad_input = grad_input.view_as(input_c);
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_w,
+                                              1,
+                                              out_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0});
+                grad_offset = grad_offset.view_as(offset_c);
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_w,
-                                          1,
                                           out_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          0, 0, 0, 0});
-            grad_offset = grad_offset.view_as(offset_c);
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_w,
-                                      out_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0});
-            grad_mask = grad_mask.view_as(mask_c);
-
-            // Separate channels into convolution groups
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          groups,
-                                          out_channels / groups,
-                                          out_w}).permute({0, 2, 3, 1, 4}).contiguous();
+                                          0, 0, 0});
+                grad_mask = grad_mask.view_as(mask_c);
 
-            weight_c = weight_c.view({groups,
-                                      out_channels / groups,
-                                      in_channels / groups,
-                                      weight_w});
-            grad_weight = grad_weight.view_as(weight_c);
-
-            auto columns = at::empty({groups,
-                                      in_channels * weight_w / groups,
-                                      n_parallel_imgs * out_w},
-                                     input_c.options());
-            auto columns_view = columns.view({in_channels,
-                                              weight_w,
+                // Separate channels into convolution groups
+                grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
-                                              out_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
-                }
+                                              groups,
+                                              out_channels / groups,
+                                              out_w}).permute({0, 2, 3, 1, 4}).contiguous();
 
-                auto grad_offset_b = grad_offset[b];
-                deform_conv1d_compute_grad_offset(
-                        columns_view,
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_offset_b);
-
-                auto grad_mask_b = grad_mask[b];
-                deform_conv1d_compute_grad_mask(
-                        columns_view,
-                        input_c[b],
-                        offset_c[b],
-                        in_channels,
-                        in_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_mask_b);
-
-                auto grad_input_b = grad_input[b];
-                col2arr(
-                        columns_view,
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_input_b);
-
-                arr2col(
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
-
-                for (int g = 0; g < groups; g++) {
-                    grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                weight_c = weight_c.view({groups,
+                                          out_channels / groups,
+                                          in_channels / groups,
+                                          weight_w});
+                grad_weight = grad_weight.view_as(weight_c);
+
+                auto columns = at::empty({groups,
+                                          in_channels * weight_w / groups,
+                                          n_parallel_imgs * out_w},
+                                         input_c.options());
+                auto columns_view = columns.view({in_channels,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  out_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    columns.zero_();
+                    for (int64_t g = 0; g < groups; g++) {
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
+                    }
+
+                    auto grad_offset_b = grad_offset[b];
+                    deform_conv1d_compute_grad_offset(
+                            columns_view,
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_offset_b);
+
+                    auto grad_mask_b = grad_mask[b];
+                    deform_conv1d_compute_grad_mask(
+                            columns_view,
+                            input_c[b],
+                            offset_c[b],
+                            in_channels,
+                            in_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_mask_b);
+
+                    auto grad_input_b = grad_input[b];
+                    col2arr(
+                            columns_view,
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_input_b);
+
+                    arr2col(
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
+
+                    for (int64_t g = 0; g < groups; g++) {
+                        grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    }
                 }
-            }
 
-            grad_input = grad_input.view_as(input);
-            grad_weight = grad_weight.view_as(weight);
-            grad_offset = grad_offset.view_as(offset);
-            grad_mask = grad_mask.view_as(mask);
-            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
+                grad_input = grad_input.view_as(input);
+                grad_weight = grad_weight.view_as(weight);
+                grad_offset = grad_offset.view_as(offset);
+                grad_mask = grad_mask.view_as(mask);
+                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
 
-            return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+                return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+            }
         }
 
         class DeformConv1dFunction
                 : public torch::autograd::Function<DeformConv1dFunction> {
         public:
             static torch::autograd::variable_list forward(
                     torch::autograd::AutogradContext *ctx,
                     const torch::autograd::Variable &input,
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
-                    int64_t stride,
-                    int64_t pad,
-                    int64_t dilation,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
                     int64_t groups,
-                    int64_t offset_groups,
-                    int64_t mask_groups,
                     bool deformable,
                     bool modulated) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv1d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
-                        pad,
+                        padding,
                         dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride"] = stride;
-                ctx->saved_data["pad"] = pad;
-                ctx->saved_data["dilation"] = dilation;
+                ctx->saved_data["stride"] = stride.vec();
+                ctx->saved_data["padding"] = padding.vec();
+                ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["offset_groups"] = offset_groups;
-                ctx->saved_data["mask_groups"] = mask_groups;
                 ctx->saved_data["deformable"] = deformable;
                 ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
@@ -526,36 +538,32 @@
                 auto saved = ctx->get_saved_variables();
                 auto input = saved[0];
                 auto weight = saved[1];
                 auto offset = saved[2];
                 auto mask = saved[3];
                 auto bias = saved[4];
 
-                auto stride = ctx->saved_data["stride"].toInt();
-                auto pad = ctx->saved_data["pad"].toInt();
-                auto dilation = ctx->saved_data["dilation"].toInt();
+                auto stride = ctx->saved_data["stride"].toIntVector();
+                auto padding = ctx->saved_data["padding"].toIntVector();
+                auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
-                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
                 auto deformable = ctx->saved_data["deformable"].toBool();
                 auto modulated = ctx->saved_data["modulated"].toBool();
 
-                auto grads = deform_conv1d_backward(
+                auto grads = detail::_deform_conv1d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
-                        pad,
+                        padding,
                         dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
@@ -568,46 +576,45 @@
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv1d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const int64_t stride,
-                const int64_t pad,
-                const int64_t dilation,
-                const int64_t groups,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                const at::optional<at::Tensor> &offset = {},
+                const at::optional<at::Tensor> &mask = {},
+                const at::optional<at::Tensor> &bias = {},
+                at::IntArrayRef stride = 1,
+                at::IntArrayRef padding = 0,
+                at::IntArrayRef dilation = 1,
+                int64_t groups = 1) {
             C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv1d");
             auto result = DeformConv1dFunction::apply(
                     input,
                     weight,
-                    offset,
-                    mask,
-                    bias,
+                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
                     stride,
-                    pad,
+                    padding,
                     dilation,
                     groups,
-                    offset_groups,
-                    mask_groups,
-                    deformable,
-                    modulated);
+                    offset.has_value(),
+                    mask.has_value());
             return result[0];
         }
+
+        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
+            m.def("tvdcn::deform_conv1d(Tensor input, Tensor weight, "
+                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
+                  "int[1] stride=1, int[1] padding=0, int[1] dilation=1, int groups=1) -> Tensor",
+                  &deform_conv1d);
+        }
     }
 }
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -77,22 +77,20 @@
     namespace ops {
         at::Tensor deform_conv2d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const std::pair<int, int> &stride,
-                const std::pair<int, int> &padding,
-                const std::pair<int, int> &dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                at::IntArrayRef stride,
+                at::IntArrayRef padding,
+                at::IntArrayRef dilation,
+                int64_t groups,
+                bool deformable,
+                bool modulated) {
             at::CheckedFrom c = "deform_conv2d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
@@ -103,40 +101,40 @@
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 4)
+            TORCH_CHECK(weight_c.ndimension() == 4)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
-            TORCH_CHECK(weight_c.ndimension() == 4)
 
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_h = input_c.size(2);
-            int in_w = input_c.size(3);
+            int64_t batch_sz = input_c.size(0);
+            int64_t in_channels = input_c.size(1);
+            int64_t in_h = input_c.size(2);
+            int64_t in_w = input_c.size(3);
 
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(0);
-            int weight_h = weight_c.size(2);
-            int weight_w = weight_c.size(3);
+            int64_t out_channels = weight_c.size(0);
+            int64_t weight_h = weight_c.size(2);
+            int64_t weight_w = weight_c.size(3);
 
-            int stride_h = stride.first;
-            int stride_w = stride.second;
+            int64_t stride_h = stride[0];
+            int64_t stride_w = stride[1];
 
-            int pad_h = padding.first;
-            int pad_w = padding.second;
+            int64_t pad_h = padding[0];
+            int64_t pad_w = padding[1];
 
-            int dilation_h = dilation.first;
-            int dilation_w = dilation.second;
+            int64_t dilation_h = dilation[0];
+            int64_t dilation_w = dilation[1];
 
-            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+            int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
+            int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
             TORCH_CHECK(
                     weight_h > 0 && weight_w > 0,
                     "weight_h: ",
                     weight_h,
                     " weight_w: ",
                     weight_w)
@@ -147,15 +145,32 @@
                     " stride_w: ",
                     stride_w)
             TORCH_CHECK(pad_h >= 0 && pad_w >= 0, "pad_h: ", pad_h, " pad_w: ", pad_w)
             TORCH_CHECK(dilation_h > 0 && dilation_w > 0, "dilation_h: ", dilation_h, " dilation_w: ", dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+            int64_t offset_groups = offset.size(1) / (2 * weight_h * weight_w);
+            int64_t mask_groups = mask.size(1) / (weight_h * weight_w);
+
+            TORCH_CHECK(!deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
+                        offset.size(1),
+                        ", while 2 * weight.size(2) * weight.size(3)=",
+                        2 * weight_h * weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+
+            TORCH_CHECK(!modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
+                        mask.size(1),
+                        ", while weight.size(2) * weight.size(3)=",
+                        weight_h * weight_w)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
@@ -272,15 +287,15 @@
                                      input_c.options());
             auto columns_view = columns.view({in_channels,
                                               weight_h,
                                               weight_w,
                                               n_parallel_imgs,
                                               out_h,
                                               out_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
+            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 im2col(
                         input_c[b],
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_h,
                         in_w,
@@ -297,15 +312,15 @@
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
-                for (int g = 0; g < groups; g++) {
+                for (int64_t g = 0; g < groups; g++) {
                     output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
                 }
             }
 
             output_buf = output_buf.view({batch_sz / n_parallel_imgs,
                                           out_channels,
                                           n_parallel_imgs,
@@ -314,293 +329,284 @@
             output_buf.transpose_(1, 2);
             output.copy_(output_buf);
             output = output.view({batch_sz, out_channels, out_h, out_w});
 
             return output + bias_c.view({1, out_channels, 1, 1});
         }
 
-        std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv2d_backward(
-                const at::Tensor &grad_out,
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const std::pair<int, int> &stride,
-                const std::pair<int, int> &padding,
-                const std::pair<int, int> &dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
-            at::Tensor grad_out_c = grad_out.contiguous();
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_h = input_c.size(2);
-            int in_w = input_c.size(3);
-
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int out_channels = weight_c.size(0);
-            int weight_h = weight_c.size(2);
-            int weight_w = weight_c.size(3);
-
-            int stride_h = stride.first;
-            int stride_w = stride.second;
-
-            int pad_h = padding.first;
-            int pad_w = padding.second;
-
-            int dilation_h = dilation.first;
-            int dilation_w = dilation.second;
-
-            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
-
-            auto grad_input = at::zeros_like(input_c);
-            auto grad_weight = at::zeros_like(weight_c);
-            auto grad_offset = at::zeros_like(offset_c);
-            auto grad_mask = at::zeros_like(mask_c);
-            auto grad_bias = at::ones_like(bias_c);
-
-            // Separate into blocks
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_h,
-                                    in_w});
-            grad_input = grad_input.view_as(input_c);
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+        namespace detail {
+            std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
+            _deform_conv2d_backward(
+                    const at::Tensor &grad_out,
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const at::Tensor &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups,
+                    bool deformable,
+                    bool modulated) {
+                at::Tensor grad_out_c = grad_out.contiguous();
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = offset.contiguous();
+                at::Tensor mask_c = mask.contiguous();
+                at::Tensor bias_c = bias.contiguous();
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_h = input_c.size(2);
+                int64_t in_w = input_c.size(3);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(0);
+                int64_t weight_h = weight_c.size(2);
+                int64_t weight_w = weight_c.size(3);
+
+                int64_t stride_h = stride[0];
+                int64_t stride_w = stride[1];
+
+                int64_t pad_h = padding[0];
+                int64_t pad_w = padding[1];
+
+                int64_t dilation_h = dilation[0];
+                int64_t dilation_w = dilation[1];
+
+                int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
+                int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+
+                int64_t offset_groups = offset.size(1) / (2 * weight_h * weight_w);
+                int64_t mask_groups = mask.size(1) / (weight_h * weight_w);
+
+                auto grad_input = at::zeros_like(input_c);
+                auto grad_weight = at::zeros_like(weight_c);
+                auto grad_offset = at::zeros_like(offset_c);
+                auto grad_mask = at::zeros_like(mask_c);
+                auto grad_bias = at::ones_like(bias_c);
+
+                // Separate into blocks
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_h,
+                                        in_w});
+                grad_input = grad_input.view_as(input_c);
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_h,
+                                              weight_w,
+                                              2,
+                                              out_h,
+                                              out_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0, 0, 0});
+                grad_offset = grad_offset.view_as(offset_c);
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_h,
                                           weight_w,
-                                          2,
                                           out_h,
                                           out_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0});
-            grad_offset = grad_offset.view_as(offset_c);
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_h,
-                                      weight_w,
-                                      out_h,
-                                      out_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0, 0, 0});
-            grad_mask = grad_mask.view_as(mask_c);
+                                          0, 0, 0, 0, 0});
+                grad_mask = grad_mask.view_as(mask_c);
 
-            // Separate channels into convolution groups
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          groups,
-                                          out_channels / groups,
-                                          out_h,
-                                          out_w}).permute({0, 2, 3, 1, 4, 5}).contiguous();
-
-            weight_c = weight_c.view({groups,
-                                      out_channels / groups,
-                                      in_channels / groups,
-                                      weight_h,
-                                      weight_w});
-            grad_weight = grad_weight.view_as(weight_c);
-
-            auto columns = at::empty({groups,
-                                      in_channels * weight_h * weight_w / groups,
-                                      n_parallel_imgs * out_h * out_w},
-                                     input_c.options());
-            auto columns_view = columns.view({in_channels,
-                                              weight_h,
-                                              weight_w,
+                // Separate channels into convolution groups
+                grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
+                                              groups,
+                                              out_channels / groups,
                                               out_h,
-                                              out_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
-                }
+                                              out_w}).permute({0, 2, 3, 1, 4, 5}).contiguous();
 
-                auto grad_offset_b = grad_offset[b];
-                deform_conv2d_compute_grad_offset(
-                        columns_view,
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_offset_b);
-
-                auto grad_mask_b = grad_mask[b];
-                deform_conv2d_compute_grad_mask(
-                        columns_view,
-                        input_c[b],
-                        offset_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_mask_b);
-
-                auto grad_input_b = grad_input[b];
-                col2im(
-                        columns_view,
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_input_b);
-
-                im2col(
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
+                weight_c = weight_c.view({groups,
+                                          out_channels / groups,
+                                          in_channels / groups,
+                                          weight_h,
+                                          weight_w});
+                grad_weight = grad_weight.view_as(weight_c);
 
-                for (int g = 0; g < groups; g++) {
-                    grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                auto columns = at::empty({groups,
+                                          in_channels * weight_h * weight_w / groups,
+                                          n_parallel_imgs * out_h * out_w},
+                                         input_c.options());
+                auto columns_view = columns.view({in_channels,
+                                                  weight_h,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  out_h,
+                                                  out_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    columns.zero_();
+                    for (int64_t g = 0; g < groups; g++) {
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
+                    }
+
+                    auto grad_offset_b = grad_offset[b];
+                    deform_conv2d_compute_grad_offset(
+                            columns_view,
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_h,
+                            in_w,
+                            weight_h,
+                            weight_w,
+                            stride_h,
+                            stride_w,
+                            pad_h,
+                            pad_w,
+                            dilation_h,
+                            dilation_w,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_offset_b);
+
+                    auto grad_mask_b = grad_mask[b];
+                    deform_conv2d_compute_grad_mask(
+                            columns_view,
+                            input_c[b],
+                            offset_c[b],
+                            in_channels,
+                            in_h,
+                            in_w,
+                            weight_h,
+                            weight_w,
+                            stride_h,
+                            stride_w,
+                            pad_h,
+                            pad_w,
+                            dilation_h,
+                            dilation_w,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_mask_b);
+
+                    auto grad_input_b = grad_input[b];
+                    col2im(
+                            columns_view,
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_h,
+                            in_w,
+                            weight_h,
+                            weight_w,
+                            stride_h,
+                            stride_w,
+                            pad_h,
+                            pad_w,
+                            dilation_h,
+                            dilation_w,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_input_b);
+
+                    im2col(
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_h,
+                            in_w,
+                            weight_h,
+                            weight_w,
+                            stride_h,
+                            stride_w,
+                            pad_h,
+                            pad_w,
+                            dilation_h,
+                            dilation_w,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
+
+                    for (int64_t g = 0; g < groups; g++) {
+                        grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    }
                 }
-            }
 
-            grad_input = grad_input.view_as(input);
-            grad_weight = grad_weight.view_as(weight);
-            grad_offset = grad_offset.view_as(offset);
-            grad_mask = grad_mask.view_as(mask);
-            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
+                grad_input = grad_input.view_as(input);
+                grad_weight = grad_weight.view_as(weight);
+                grad_offset = grad_offset.view_as(offset);
+                grad_mask = grad_mask.view_as(mask);
+                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
 
-            return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+                return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+            }
         }
 
         class DeformConv2dFunction
                 : public torch::autograd::Function<DeformConv2dFunction> {
         public:
             static torch::autograd::variable_list forward(
                     torch::autograd::AutogradContext *ctx,
                     const torch::autograd::Variable &input,
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
-                    int64_t stride_h,
-                    int64_t stride_w,
-                    int64_t pad_h,
-                    int64_t pad_w,
-                    int64_t dilation_h,
-                    int64_t dilation_w,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
                     int64_t groups,
-                    int64_t offset_groups,
-                    int64_t mask_groups,
                     bool deformable,
                     bool modulated) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv2d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
-                        std::make_pair(stride_h, stride_w),
-                        std::make_pair(pad_h, pad_w),
-                        std::make_pair(dilation_h, dilation_w),
+                        stride,
+                        padding,
+                        dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride_h"] = stride_h;
-                ctx->saved_data["stride_w"] = stride_w;
-                ctx->saved_data["pad_h"] = pad_h;
-                ctx->saved_data["pad_w"] = pad_w;
-                ctx->saved_data["dilation_h"] = dilation_h;
-                ctx->saved_data["dilation_w"] = dilation_w;
+                ctx->saved_data["stride"] = stride.vec();
+                ctx->saved_data["padding"] = padding.vec();
+                ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["offset_groups"] = offset_groups;
-                ctx->saved_data["mask_groups"] = mask_groups;
                 ctx->saved_data["deformable"] = deformable;
                 ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
@@ -611,39 +617,32 @@
                 auto saved = ctx->get_saved_variables();
                 auto input = saved[0];
                 auto weight = saved[1];
                 auto offset = saved[2];
                 auto mask = saved[3];
                 auto bias = saved[4];
 
-                auto stride_h = ctx->saved_data["stride_h"].toInt();
-                auto stride_w = ctx->saved_data["stride_w"].toInt();
-                auto pad_h = ctx->saved_data["pad_h"].toInt();
-                auto pad_w = ctx->saved_data["pad_w"].toInt();
-                auto dilation_h = ctx->saved_data["dilation_h"].toInt();
-                auto dilation_w = ctx->saved_data["dilation_w"].toInt();
+                auto stride = ctx->saved_data["stride"].toIntVector();
+                auto padding = ctx->saved_data["padding"].toIntVector();
+                auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
-                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
                 auto deformable = ctx->saved_data["deformable"].toBool();
                 auto modulated = ctx->saved_data["modulated"].toBool();
 
-                auto grads = deform_conv2d_backward(
+                auto grads = detail::_deform_conv2d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
-                        std::make_pair(stride_h, stride_w),
-                        std::make_pair(pad_h, pad_w),
-                        std::make_pair(dilation_h, dilation_w),
+                        stride,
+                        padding,
+                        dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
@@ -656,55 +655,45 @@
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv2d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t groups,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                const at::optional<at::Tensor> &offset = {},
+                const at::optional<at::Tensor> &mask = {},
+                const at::optional<at::Tensor> &bias = {},
+                at::IntArrayRef stride = 1,
+                at::IntArrayRef padding = 0,
+                at::IntArrayRef dilation = 1,
+                int64_t groups = 1) {
             C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv2d");
             auto result = DeformConv2dFunction::apply(
                     input,
                     weight,
-                    offset,
-                    mask,
-                    bias,
-                    stride_h,
-                    stride_w,
-                    pad_h,
-                    pad_w,
-                    dilation_h,
-                    dilation_w,
+                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    stride,
+                    padding,
+                    dilation,
                     groups,
-                    offset_groups,
-                    mask_groups,
-                    deformable,
-                    modulated);
+                    offset.has_value(),
+                    mask.has_value());
             return result[0];
         }
+
+        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
+            m.def("tvdcn::deform_conv2d(Tensor input, Tensor weight, "
+                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
+                  "int[2] stride=1, int[2] padding=0, int[2] dilation=1, int groups=1) -> Tensor",
+                  &deform_conv2d);
+        }
     }
 }
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -77,22 +77,20 @@
     namespace ops {
         at::Tensor deform_conv3d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const std::tuple<int, int, int> &stride,
-                const std::tuple<int, int, int> &padding,
-                const std::tuple<int, int, int> &dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                at::IntArrayRef stride,
+                at::IntArrayRef padding,
+                at::IntArrayRef dilation,
+                int64_t groups,
+                bool deformable,
+                bool modulated) {
             at::CheckedFrom c = "deform_conv3d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
@@ -103,46 +101,46 @@
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 5)
+            TORCH_CHECK(weight_c.ndimension() == 5)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
-            TORCH_CHECK(weight_c.ndimension() == 5)
 
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_d = input_c.size(2);
-            int in_h = input_c.size(3);
-            int in_w = input_c.size(4);
-
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int out_channels = weight_c.size(0);
-            int weight_d = weight_c.size(2);
-            int weight_h = weight_c.size(3);
-            int weight_w = weight_c.size(4);
-
-            int stride_d = std::get<0>(stride);
-            int stride_h = std::get<1>(stride);
-            int stride_w = std::get<2>(stride);
-
-            int pad_d = std::get<0>(padding);
-            int pad_h = std::get<1>(padding);
-            int pad_w = std::get<2>(padding);
-
-            int dilation_d = std::get<0>(dilation);
-            int dilation_h = std::get<1>(dilation);
-            int dilation_w = std::get<2>(dilation);
-
-            int out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
-            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+            int64_t batch_sz = input_c.size(0);
+            int64_t in_channels = input_c.size(1);
+            int64_t in_d = input_c.size(2);
+            int64_t in_h = input_c.size(3);
+            int64_t in_w = input_c.size(4);
+
+            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+            int64_t out_channels = weight_c.size(0);
+            int64_t weight_d = weight_c.size(2);
+            int64_t weight_h = weight_c.size(3);
+            int64_t weight_w = weight_c.size(4);
+
+            int64_t stride_d = stride[0];
+            int64_t stride_h = stride[1];
+            int64_t stride_w = stride[2];
+
+            int64_t pad_d = padding[0];
+            int64_t pad_h = padding[1];
+            int64_t pad_w = padding[2];
+
+            int64_t dilation_d = dilation[0];
+            int64_t dilation_h = dilation[1];
+            int64_t dilation_w = dilation[2];
+
+            int64_t out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
+            int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
+            int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
             TORCH_CHECK(
                     weight_d > 0 && weight_h > 0 && weight_w > 0,
                     "weight_d: ",
                     weight_d,
                     " weight_h: ",
                     weight_h,
@@ -158,15 +156,32 @@
                     stride_w)
             TORCH_CHECK(pad_d >= 0 && pad_h >= 0 && pad_w >= 0, "pad_d: ", pad_d, " pad_h: ", pad_h, " pad_w: ", pad_w)
             TORCH_CHECK(dilation_d > 0 && dilation_h > 0 && dilation_w > 0, "dilation_d: ", dilation_d, " dilation_h: ",
                         dilation_h, " dilation_w: ", dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+            int64_t offset_groups = offset.size(1) / (3 * weight_d * weight_h * weight_w);
+            int64_t mask_groups = mask.size(1) / (weight_d * weight_h * weight_w);
+
+            TORCH_CHECK(!deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
+                        offset.size(1),
+                        ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
+                        3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+
+            TORCH_CHECK(!modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
+                        mask.size(1),
+                        ", while weight.size(2) * weight.size(3) * weight.size(4)=",
+                        weight_d * weight_h * weight_w)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
@@ -306,15 +321,15 @@
                                               weight_d,
                                               weight_h,
                                               weight_w,
                                               n_parallel_imgs,
                                               out_d,
                                               out_h,
                                               out_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
+            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 vol2col(
                         input_c[b],
                         offset_c[b],
                         mask_c[b],
                         in_channels,
                         in_d,
                         in_h,
@@ -337,15 +352,15 @@
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
-                for (int g = 0; g < groups; g++) {
+                for (int64_t g = 0; g < groups; g++) {
                     output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
                 }
             }
 
             output_buf = output_buf.view({batch_sz / n_parallel_imgs,
                                           out_channels,
                                           n_parallel_imgs,
@@ -355,338 +370,323 @@
             output_buf.transpose_(1, 2);
             output.copy_(output_buf);
             output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
 
             return output + bias_c.view({1, out_channels, 1, 1, 1});
         }
 
-        std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv3d_backward(
-                const at::Tensor &grad_out,
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const std::tuple<int, int, int> &stride,
-                const std::tuple<int, int, int> &padding,
-                const std::tuple<int, int, int> &dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
-            at::Tensor grad_out_c = grad_out.contiguous();
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_d = input_c.size(2);
-            int in_h = input_c.size(3);
-            int in_w = input_c.size(4);
-
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int out_channels = weight_c.size(0);
-            int weight_d = weight_c.size(2);
-            int weight_h = weight_c.size(3);
-            int weight_w = weight_c.size(4);
-
-            int stride_d = std::get<0>(stride);
-            int stride_h = std::get<1>(stride);
-            int stride_w = std::get<2>(stride);
-
-            int pad_d = std::get<0>(padding);
-            int pad_h = std::get<1>(padding);
-            int pad_w = std::get<2>(padding);
-
-            int dilation_d = std::get<0>(dilation);
-            int dilation_h = std::get<1>(dilation);
-            int dilation_w = std::get<2>(dilation);
-
-            int out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
-            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
-
-            auto grad_input = at::zeros_like(input_c);
-            auto grad_weight = at::zeros_like(weight_c);
-            auto grad_offset = at::zeros_like(offset_c);
-            auto grad_mask = at::zeros_like(mask_c);
-            auto grad_bias = at::ones_like(bias_c);
-
-            // Separate into blocks
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_d,
-                                    in_h,
-                                    in_w});
-            grad_input = grad_input.view_as(input_c);
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+        namespace detail {
+            std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
+            _deform_conv3d_backward(
+                    const at::Tensor &grad_out,
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const at::Tensor &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups,
+                    bool deformable,
+                    bool modulated) {
+                at::Tensor grad_out_c = grad_out.contiguous();
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = offset.contiguous();
+                at::Tensor mask_c = mask.contiguous();
+                at::Tensor bias_c = bias.contiguous();
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_d = input_c.size(2);
+                int64_t in_h = input_c.size(3);
+                int64_t in_w = input_c.size(4);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(0);
+                int64_t weight_d = weight_c.size(2);
+                int64_t weight_h = weight_c.size(3);
+                int64_t weight_w = weight_c.size(4);
+
+                int64_t stride_d = stride[0];
+                int64_t stride_h = stride[1];
+                int64_t stride_w = stride[2];
+
+                int64_t pad_d = padding[0];
+                int64_t pad_h = padding[1];
+                int64_t pad_w = padding[2];
+
+                int64_t dilation_d = dilation[0];
+                int64_t dilation_h = dilation[1];
+                int64_t dilation_w = dilation[2];
+
+                int64_t out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
+                int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
+                int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+
+                int64_t offset_groups = offset.size(1) / (3 * weight_d * weight_h * weight_w);
+                int64_t mask_groups = mask.size(1) / (weight_d * weight_h * weight_w);
+
+                auto grad_input = at::zeros_like(input_c);
+                auto grad_weight = at::zeros_like(weight_c);
+                auto grad_offset = at::zeros_like(offset_c);
+                auto grad_mask = at::zeros_like(mask_c);
+                auto grad_bias = at::ones_like(bias_c);
+
+                // Separate into blocks
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_d,
+                                        in_h,
+                                        in_w});
+                grad_input = grad_input.view_as(input_c);
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_d,
+                                              weight_h,
+                                              weight_w,
+                                              3,
+                                              out_d,
+                                              out_h,
+                                              out_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0, 0, 0, 0, 0});
+                grad_offset = grad_offset.view_as(offset_c);
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_d,
                                           weight_h,
                                           weight_w,
-                                          3,
                                           out_d,
                                           out_h,
                                           out_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0, 0, 0});
-            grad_offset = grad_offset.view_as(offset_c);
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_d,
-                                      weight_h,
-                                      weight_w,
-                                      out_d,
-                                      out_h,
-                                      out_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0, 0, 0, 0, 0});
-            grad_mask = grad_mask.view_as(mask_c);
-
-            // Separate channels into convolution groups
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          groups,
-                                          out_channels / groups,
-                                          out_d,
-                                          out_h,
-                                          out_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
+                                          0, 0, 0, 0, 0, 0, 0});
+                grad_mask = grad_mask.view_as(mask_c);
 
-            weight_c = weight_c.view({groups,
-                                      out_channels / groups,
-                                      in_channels / groups,
-                                      weight_d,
-                                      weight_h,
-                                      weight_w});
-            grad_weight = grad_weight.view_as(weight_c);
-
-            auto columns = at::empty({groups,
-                                      in_channels * weight_d * weight_h * weight_w / groups,
-                                      n_parallel_imgs * out_d * out_h * out_w},
-                                     input_c.options());
-            auto columns_view = columns.view({in_channels,
-                                              weight_d,
-                                              weight_h,
-                                              weight_w,
+                // Separate channels into convolution groups
+                grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
+                                              groups,
+                                              out_channels / groups,
                                               out_d,
                                               out_h,
-                                              out_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
-                }
+                                              out_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
 
-                auto grad_offset_b = grad_offset[b];
-                deform_conv3d_compute_grad_offset(
-                        columns_view,
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
-                        weight_d,
-                        weight_h,
-                        weight_w,
-                        stride_d,
-                        stride_h,
-                        stride_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
-                        dilation_d,
-                        dilation_h,
-                        dilation_w,
-                        out_d,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_offset_b);
-
-                auto grad_mask_b = grad_mask[b];
-                deform_conv3d_compute_grad_mask(
-                        columns_view,
-                        input_c[b],
-                        offset_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
-                        weight_d,
-                        weight_h,
-                        weight_w,
-                        stride_d,
-                        stride_h,
-                        stride_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
-                        dilation_d,
-                        dilation_h,
-                        dilation_w,
-                        out_d,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_mask_b);
-
-                auto grad_input_b = grad_input[b];
-                col2vol(
-                        columns_view,
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
-                        weight_d,
-                        weight_h,
-                        weight_w,
-                        stride_d,
-                        stride_h,
-                        stride_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
-                        dilation_d,
-                        dilation_h,
-                        dilation_w,
-                        out_d,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_input_b);
-
-                vol2col(
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
-                        weight_d,
-                        weight_h,
-                        weight_w,
-                        stride_d,
-                        stride_h,
-                        stride_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
-                        dilation_d,
-                        dilation_h,
-                        dilation_w,
-                        out_d,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
+                weight_c = weight_c.view({groups,
+                                          out_channels / groups,
+                                          in_channels / groups,
+                                          weight_d,
+                                          weight_h,
+                                          weight_w});
+                grad_weight = grad_weight.view_as(weight_c);
 
-                for (int g = 0; g < groups; g++) {
-                    grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                auto columns = at::empty({groups,
+                                          in_channels * weight_d * weight_h * weight_w / groups,
+                                          n_parallel_imgs * out_d * out_h * out_w},
+                                         input_c.options());
+                auto columns_view = columns.view({in_channels,
+                                                  weight_d,
+                                                  weight_h,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  out_d,
+                                                  out_h,
+                                                  out_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    columns.zero_();
+                    for (int64_t g = 0; g < groups; g++) {
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
+                    }
+
+                    auto grad_offset_b = grad_offset[b];
+                    deform_conv3d_compute_grad_offset(
+                            columns_view,
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_d,
+                            in_h,
+                            in_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            out_d,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_offset_b);
+
+                    auto grad_mask_b = grad_mask[b];
+                    deform_conv3d_compute_grad_mask(
+                            columns_view,
+                            input_c[b],
+                            offset_c[b],
+                            in_channels,
+                            in_d,
+                            in_h,
+                            in_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            out_d,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_mask_b);
+
+                    auto grad_input_b = grad_input[b];
+                    col2vol(
+                            columns_view,
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_d,
+                            in_h,
+                            in_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            out_d,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_input_b);
+
+                    vol2col(
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_d,
+                            in_h,
+                            in_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            out_d,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
+
+                    for (int64_t g = 0; g < groups; g++) {
+                        grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    }
                 }
-            }
 
-            grad_input = grad_input.view_as(input);
-            grad_weight = grad_weight.view_as(weight);
-            grad_offset = grad_offset.view_as(offset);
-            grad_mask = grad_mask.view_as(mask);
-            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
+                grad_input = grad_input.view_as(input);
+                grad_weight = grad_weight.view_as(weight);
+                grad_offset = grad_offset.view_as(offset);
+                grad_mask = grad_mask.view_as(mask);
+                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
 
-            return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+                return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+            }
         }
 
         class DeformConv3dFunction
                 : public torch::autograd::Function<DeformConv3dFunction> {
         public:
             static torch::autograd::variable_list forward(
                     torch::autograd::AutogradContext *ctx,
                     const torch::autograd::Variable &input,
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
-                    int64_t stride_d,
-                    int64_t stride_h,
-                    int64_t stride_w,
-                    int64_t pad_d,
-                    int64_t pad_h,
-                    int64_t pad_w,
-                    int64_t dilation_d,
-                    int64_t dilation_h,
-                    int64_t dilation_w,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
                     int64_t groups,
-                    int64_t offset_groups,
-                    int64_t mask_groups,
                     bool deformable,
                     bool modulated) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv3d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
-                        std::make_tuple(stride_d, stride_h, stride_w),
-                        std::make_tuple(pad_d, pad_h, pad_w),
-                        std::make_tuple(dilation_d, dilation_h, dilation_w),
+                        stride,
+                        padding,
+                        dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride_d"] = stride_d;
-                ctx->saved_data["stride_h"] = stride_h;
-                ctx->saved_data["stride_w"] = stride_w;
-                ctx->saved_data["pad_d"] = pad_d;
-                ctx->saved_data["pad_h"] = pad_h;
-                ctx->saved_data["pad_w"] = pad_w;
-                ctx->saved_data["dilation_d"] = dilation_d;
-                ctx->saved_data["dilation_h"] = dilation_h;
-                ctx->saved_data["dilation_w"] = dilation_w;
+                ctx->saved_data["stride"] = stride.vec();
+                ctx->saved_data["padding"] = padding.vec();
+                ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["offset_groups"] = offset_groups;
-                ctx->saved_data["mask_groups"] = mask_groups;
                 ctx->saved_data["deformable"] = deformable;
                 ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
@@ -697,42 +697,32 @@
                 auto saved = ctx->get_saved_variables();
                 auto input = saved[0];
                 auto weight = saved[1];
                 auto offset = saved[2];
                 auto mask = saved[3];
                 auto bias = saved[4];
 
-                auto stride_d = ctx->saved_data["stride_d"].toInt();
-                auto stride_h = ctx->saved_data["stride_h"].toInt();
-                auto stride_w = ctx->saved_data["stride_w"].toInt();
-                auto pad_d = ctx->saved_data["pad_d"].toInt();
-                auto pad_h = ctx->saved_data["pad_h"].toInt();
-                auto pad_w = ctx->saved_data["pad_w"].toInt();
-                auto dilation_d = ctx->saved_data["dilation_d"].toInt();
-                auto dilation_h = ctx->saved_data["dilation_h"].toInt();
-                auto dilation_w = ctx->saved_data["dilation_w"].toInt();
+                auto stride = ctx->saved_data["stride"].toIntVector();
+                auto padding = ctx->saved_data["padding"].toIntVector();
+                auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
-                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
                 auto deformable = ctx->saved_data["deformable"].toBool();
                 auto modulated = ctx->saved_data["modulated"].toBool();
 
-                auto grads = deform_conv3d_backward(
+                auto grads = detail::_deform_conv3d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
-                        std::make_tuple(stride_d, stride_h, stride_w),
-                        std::make_tuple(pad_d, pad_h, pad_w),
-                        std::make_tuple(dilation_d, dilation_h, dilation_w),
+                        stride,
+                        padding,
+                        dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
@@ -745,64 +735,45 @@
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv3d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t groups,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                const at::optional<at::Tensor> &offset = {},
+                const at::optional<at::Tensor> &mask = {},
+                const at::optional<at::Tensor> &bias = {},
+                at::IntArrayRef stride = 1,
+                at::IntArrayRef padding = 0,
+                at::IntArrayRef dilation = 1,
+                int64_t groups = 1) {
             C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv3d");
             auto result = DeformConv3dFunction::apply(
                     input,
                     weight,
-                    offset,
-                    mask,
-                    bias,
-                    stride_d,
-                    stride_h,
-                    stride_w,
-                    pad_d,
-                    pad_h,
-                    pad_w,
-                    dilation_d,
-                    dilation_h,
-                    dilation_w,
+                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    stride,
+                    padding,
+                    dilation,
                     groups,
-                    offset_groups,
-                    mask_groups,
-                    deformable,
-                    modulated);
+                    offset.has_value(),
+                    mask.has_value());
             return result[0];
         }
+
+        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
+            m.def("tvdcn::deform_conv3d(Tensor input, Tensor weight, "
+                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
+                  "int[3] stride=1, int[3] padding=0, int[3] dilation=1, int groups=1) -> Tensor",
+                  &deform_conv3d);
+        }
     }
 }
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -77,24 +77,22 @@
     namespace ops {
         at::Tensor deform_conv_transpose1d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const int stride,
-                const int padding,
-                const int output_padding,
-                const int dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
-            at::CheckedFrom c = "deform_conv_transpose1d_forward";
+                at::IntArrayRef stride,
+                at::IntArrayRef padding,
+                at::IntArrayRef output_padding,
+                at::IntArrayRef dilation,
+                int64_t groups,
+                bool deformable,
+                bool modulated) {
+            at::CheckedFrom c = "deform_conv_transpose2d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
@@ -104,51 +102,68 @@
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 3)
+            TORCH_CHECK(weight_c.ndimension() == 3)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
-            TORCH_CHECK(weight_c.ndimension() == 3)
 
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_w = input_c.size(2);
+            int64_t batch_sz = input_c.size(0);
+            int64_t in_channels = input_c.size(1);
+            int64_t in_w = input_c.size(2);
 
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(1) * groups;
-            int weight_w = weight_c.size(2);
+            int64_t out_channels = weight_c.size(1) * groups;
+            int64_t weight_w = weight_c.size(2);
 
-            int stride_w = stride;
+            int64_t stride_w = stride[0];
 
-            int pad_w = padding;
+            int64_t pad_w = padding[0];
 
-            int out_pad_w = output_padding;
+            int64_t out_pad_w = output_padding[0];
 
-            int dilation_w = dilation;
+            int64_t dilation_w = dilation[0];
 
-            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+            int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
             TORCH_CHECK(
                     weight_w > 0,
                     " weight_w: ",
                     weight_w)
             TORCH_CHECK(
                     stride_w > 0,
                     " stride_w: ",
                     stride_w)
             TORCH_CHECK(pad_w >= 0, " pad_w: ", pad_w)
             TORCH_CHECK(dilation_w > 0, " dilation_w: ", dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+            int64_t offset_groups = offset.size(1) / weight_w;
+            int64_t mask_groups = mask.size(1) / weight_w;
+
+            TORCH_CHECK(!deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2).\nGot offset.size(1)=",
+                        offset.size(1),
+                        ", while weight.size(2)=",
+                        weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+
+            TORCH_CHECK(!modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2).\nGot mask.size(1)=",
+                        mask.size(1),
+                        ", while weight.size(2)=",
+                        weight_w)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
@@ -231,17 +246,17 @@
                                       out_channels * weight_w / groups,
                                       n_parallel_imgs * in_w},
                                      input_c.options());
             auto columns_view = columns.view({out_channels,
                                               weight_w,
                                               n_parallel_imgs,
                                               in_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
+            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 columns.zero_();
-                for (int g = 0; g < groups; g++) {
+                for (int64_t g = 0; g < groups; g++) {
                     columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
                 }
 
                 auto output_b = output[b];
                 col2arr(
                         columns_view,
                         offset_c[b],
@@ -262,258 +277,255 @@
             }
 
             output = output.view({batch_sz, out_channels, out_w});
 
             return output + bias_c.view({1, out_channels, 1});
         }
 
-        std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv_transpose1d_backward(
-                const at::Tensor &grad_out,
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const int stride,
-                const int padding,
-                const int output_padding,
-                const int dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
-            at::Tensor grad_out_c = grad_out.contiguous();
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
+        namespace detail {
+            std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
+            _deform_conv_transpose1d_backward(
+                    const at::Tensor &grad_out,
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const at::Tensor &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef output_padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups,
+                    bool deformable,
+                    bool modulated) {
+                at::Tensor grad_out_c = grad_out.contiguous();
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = offset.contiguous();
+                at::Tensor mask_c = mask.contiguous();
+                at::Tensor bias_c = bias.contiguous();
 
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_w = input_c.size(2);
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_w = input_c.size(2);
 
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(1) * groups;
-            int weight_w = weight_c.size(2);
+                int64_t out_channels = weight_c.size(1) * groups;
+                int64_t weight_w = weight_c.size(2);
 
-            int stride_w = stride;
+                int64_t stride_w = stride[0];
 
-            int pad_w = padding;
+                int64_t pad_w = padding[0];
 
-            int out_pad_w = output_padding;
+                int64_t out_pad_w = output_padding[0];
 
-            int dilation_w = dilation;
+                int64_t dilation_w = dilation[0];
 
-            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+                int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
-            auto grad_input = at::zeros_like(input_c);
-            auto grad_weight = at::zeros_like(weight_c);
-            auto grad_offset = at::zeros_like(offset_c);
-            auto grad_mask = at::zeros_like(mask_c);
-            auto grad_bias = at::ones_like(bias_c);
+                int64_t offset_groups = offset.size(1) / weight_w;
+                int64_t mask_groups = mask.size(1) / weight_w;
 
-            // Separate into blocks
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          out_channels,
-                                          out_w});
+                auto grad_input = at::zeros_like(input_c);
+                auto grad_weight = at::zeros_like(weight_c);
+                auto grad_offset = at::zeros_like(offset_c);
+                auto grad_mask = at::zeros_like(mask_c);
+                auto grad_bias = at::ones_like(bias_c);
 
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_w});
-            grad_input = grad_input.view_as(input_c);
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                // Separate into blocks
+                grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              out_channels,
+                                              out_w});
+
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_w});
+                grad_input = grad_input.view_as(input_c);
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_w,
+                                              1,
+                                              in_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0});
+                grad_offset = grad_offset.view_as(offset_c);
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_w,
-                                          1,
                                           in_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0});
-            grad_offset = grad_offset.view_as(offset_c);
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_w,
-                                      in_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0});
-            grad_mask = grad_mask.view_as(mask_c);
-
-            auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
-                                             in_channels,
-                                             n_parallel_imgs,
-                                             in_w}, input_c.options());
-
-            // Separate channels into convolution groups
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    groups,
-                                    in_channels / groups,
-                                    in_w}).permute({0, 2, 3, 1, 4}).contiguous();
+                                          0, 0, 0});
+                grad_mask = grad_mask.view_as(mask_c);
 
-            grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
-                                                  groups,
-                                                  grad_input_buf.size(1) / groups,
-                                                  grad_input_buf.size(2),
-                                                  grad_input_buf.size(3)});
-
-            weight_c = weight_c.view({groups,
-                                      in_channels / groups,
-                                      out_channels / groups,
-                                      weight_w});
-            grad_weight = grad_weight.view_as(weight_c);
-
-            auto columns = at::empty({groups,
-                                      out_channels * weight_w / groups,
-                                      n_parallel_imgs * in_w},
-                                     input_c.options());
-            auto columns_view = columns.view({out_channels,
-                                              weight_w,
-                                              n_parallel_imgs,
-                                              in_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
+                                                 in_channels,
+                                                 n_parallel_imgs,
+                                                 in_w}, input_c.options());
+
+                // Separate channels into convolution groups
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        groups,
+                                        in_channels / groups,
+                                        in_w}).permute({0, 2, 3, 1, 4}).contiguous();
+
+                grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
+                                                      groups,
+                                                      grad_input_buf.size(1) / groups,
+                                                      grad_input_buf.size(2),
+                                                      grad_input_buf.size(3)});
+
+                weight_c = weight_c.view({groups,
+                                          in_channels / groups,
+                                          out_channels / groups,
+                                          weight_w});
+                grad_weight = grad_weight.view_as(weight_c);
+
+                auto columns = at::empty({groups,
+                                          out_channels * weight_w / groups,
+                                          n_parallel_imgs * in_w},
+                                         input_c.options());
+                auto columns_view = columns.view({out_channels,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  in_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    columns.zero_();
+                    for (int64_t g = 0; g < groups; g++) {
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                    }
+
+                    auto grad_offset_b = grad_offset[b];
+                    deform_conv1d_compute_grad_offset(
+                            columns_view,
+                            grad_out_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            out_channels,
+                            out_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_offset_b);
+
+                    auto grad_mask_b = grad_mask[b];
+                    deform_conv1d_compute_grad_mask(
+                            columns_view,
+                            grad_out_c[b],
+                            offset_c[b],
+                            out_channels,
+                            out_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_mask_b);
+
+                    arr2col(
+                            grad_out_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            out_channels,
+                            out_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
+
+                    for (int64_t g = 0; g < groups; g++) {
+                        grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                        grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    }
                 }
 
-                auto grad_offset_b = grad_offset[b];
-                deform_conv1d_compute_grad_offset(
-                        columns_view,
-                        grad_out_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_offset_b);
-
-                auto grad_mask_b = grad_mask[b];
-                deform_conv1d_compute_grad_mask(
-                        columns_view,
-                        grad_out_c[b],
-                        offset_c[b],
-                        out_channels,
-                        out_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_mask_b);
+                grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
+                                                      in_channels,
+                                                      n_parallel_imgs,
+                                                      in_w}).transpose_(1, 2);
+                grad_input.copy_(grad_input_buf);
+
+                grad_input = grad_input.view_as(input);
+                grad_weight = grad_weight.view_as(weight);
+                grad_offset = grad_offset.view_as(offset);
+                grad_mask = grad_mask.view_as(mask);
+                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
 
-                arr2col(
-                        grad_out_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
-
-                for (int g = 0; g < groups; g++) {
-                    grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                    grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
-                }
+                return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
-
-            grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
-                                                  in_channels,
-                                                  n_parallel_imgs,
-                                                  in_w}).transpose_(1, 2);
-            grad_input.copy_(grad_input_buf);
-
-            grad_input = grad_input.view_as(input);
-            grad_weight = grad_weight.view_as(weight);
-            grad_offset = grad_offset.view_as(offset);
-            grad_mask = grad_mask.view_as(mask);
-            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
-
-            return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
 
         class DeformConvTranspose1dFunction
                 : public torch::autograd::Function<DeformConvTranspose1dFunction> {
         public:
             static torch::autograd::variable_list forward(
                     torch::autograd::AutogradContext *ctx,
                     const torch::autograd::Variable &input,
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
-                    int64_t stride,
-                    int64_t pad,
-                    int64_t out_pad,
-                    int64_t dilation,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef output_padding,
+                    at::IntArrayRef dilation,
                     int64_t groups,
-                    int64_t offset_groups,
-                    int64_t mask_groups,
                     bool deformable,
                     bool modulated) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv_transpose1d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
-                        pad,
-                        out_pad,
+                        padding,
+                        output_padding,
                         dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride"] = stride;
-                ctx->saved_data["pad"] = pad;
-                ctx->saved_data["out_pad"] = out_pad;
-                ctx->saved_data["dilation"] = dilation;
+                ctx->saved_data["stride"] = stride.vec();
+                ctx->saved_data["padding"] = padding.vec();
+                ctx->saved_data["output_padding"] = output_padding.vec();
+                ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["offset_groups"] = offset_groups;
-                ctx->saved_data["mask_groups"] = mask_groups;
                 ctx->saved_data["deformable"] = deformable;
                 ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
@@ -524,38 +536,34 @@
                 auto saved = ctx->get_saved_variables();
                 auto input = saved[0];
                 auto weight = saved[1];
                 auto offset = saved[2];
                 auto mask = saved[3];
                 auto bias = saved[4];
 
-                auto stride = ctx->saved_data["stride"].toInt();
-                auto pad = ctx->saved_data["pad"].toInt();
-                auto out_pad = ctx->saved_data["out_pad"].toInt();
-                auto dilation = ctx->saved_data["dilation"].toInt();
+                auto stride = ctx->saved_data["stride"].toIntVector();
+                auto padding = ctx->saved_data["padding"].toIntVector();
+                auto output_padding = ctx->saved_data["output_padding"].toIntVector();
+                auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
-                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
                 auto deformable = ctx->saved_data["deformable"].toBool();
                 auto modulated = ctx->saved_data["modulated"].toBool();
 
-                auto grads = deform_conv_transpose1d_backward(
+                auto grads = detail::_deform_conv_transpose1d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
-                        pad,
-                        out_pad,
+                        padding,
+                        output_padding,
                         dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
@@ -569,48 +577,48 @@
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv_transpose1d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const int64_t stride,
-                const int64_t pad,
-                const int64_t out_pad,
-                const int64_t dilation,
-                const int64_t groups,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                const at::optional<at::Tensor> &offset = {},
+                const at::optional<at::Tensor> &mask = {},
+                const at::optional<at::Tensor> &bias = {},
+                at::IntArrayRef stride = 1,
+                at::IntArrayRef padding = 0,
+                at::IntArrayRef output_padding = 0,
+                at::IntArrayRef dilation = 1,
+                int64_t groups = 1) {
             C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose1d");
             auto result = DeformConvTranspose1dFunction::apply(
                     input,
                     weight,
-                    offset,
-                    mask,
-                    bias,
+                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
                     stride,
-                    pad,
-                    out_pad,
+                    padding,
+                    output_padding,
                     dilation,
                     groups,
-                    offset_groups,
-                    mask_groups,
-                    deformable,
-                    modulated);
+                    offset.has_value(),
+                    mask.has_value());
             return result[0];
         }
+
+        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
+            m.def("tvdcn::deform_conv_transpose1d(Tensor input, Tensor weight, "
+                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
+                  "int[1] stride=1, int[1] padding=0, int[1] output_padding=0, "
+                  "int[1] dilation=1, int groups=1) -> Tensor",
+                  &deform_conv_transpose1d);
+        }
     }
 }
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -77,23 +77,21 @@
     namespace ops {
         at::Tensor deform_conv_transpose2d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const std::pair<int, int> &stride,
-                const std::pair<int, int> &padding,
-                const std::pair<int, int> &output_padding,
-                const std::pair<int, int> &dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                at::IntArrayRef stride,
+                at::IntArrayRef padding,
+                at::IntArrayRef output_padding,
+                at::IntArrayRef dilation,
+                int64_t groups,
+                bool deformable,
+                bool modulated) {
             at::CheckedFrom c = "deform_conv_transpose2d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
@@ -104,43 +102,43 @@
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 4)
+            TORCH_CHECK(weight_c.ndimension() == 4)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
-            TORCH_CHECK(weight_c.ndimension() == 4)
 
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_h = input_c.size(2);
-            int in_w = input_c.size(3);
+            int64_t batch_sz = input_c.size(0);
+            int64_t in_channels = input_c.size(1);
+            int64_t in_h = input_c.size(2);
+            int64_t in_w = input_c.size(3);
 
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(1) * groups;
-            int weight_h = weight_c.size(2);
-            int weight_w = weight_c.size(3);
+            int64_t out_channels = weight_c.size(1) * groups;
+            int64_t weight_h = weight_c.size(2);
+            int64_t weight_w = weight_c.size(3);
 
-            int stride_h = stride.first;
-            int stride_w = stride.second;
+            int64_t stride_h = stride[0];
+            int64_t stride_w = stride[1];
 
-            int pad_h = padding.first;
-            int pad_w = padding.second;
+            int64_t pad_h = padding[0];
+            int64_t pad_w = padding[1];
 
-            int out_pad_h = output_padding.first;
-            int out_pad_w = output_padding.second;
+            int64_t out_pad_h = output_padding[0];
+            int64_t out_pad_w = output_padding[1];
 
-            int dilation_h = dilation.first;
-            int dilation_w = dilation.second;
+            int64_t dilation_h = dilation[0];
+            int64_t dilation_w = dilation[1];
 
-            int out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
-            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+            int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
+            int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
             TORCH_CHECK(
                     weight_h > 0 && weight_w > 0,
                     "weight_h: ",
                     weight_h,
                     " weight_w: ",
                     weight_w)
@@ -151,15 +149,32 @@
                     " stride_w: ",
                     stride_w)
             TORCH_CHECK(pad_h >= 0 && pad_w >= 0, "pad_h: ", pad_h, " pad_w: ", pad_w)
             TORCH_CHECK(dilation_h > 0 && dilation_w > 0, "dilation_h: ", dilation_h, " dilation_w: ", dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+            int64_t offset_groups = offset.size(1) / (2 * weight_h * weight_w);
+            int64_t mask_groups = mask.size(1) / (weight_h * weight_w);
+
+            TORCH_CHECK(!deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
+                        offset.size(1),
+                        ", while 2 * weight.size(2) * weight.size(3)=",
+                        2 * weight_h * weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+
+            TORCH_CHECK(!modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
+                        mask.size(1),
+                        ", while weight.size(2) * weight.size(3)=",
+                        weight_h * weight_w)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
@@ -263,17 +278,17 @@
                                      input_c.options());
             auto columns_view = columns.view({out_channels,
                                               weight_h,
                                               weight_w,
                                               n_parallel_imgs,
                                               in_h,
                                               in_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
+            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 columns.zero_();
-                for (int g = 0; g < groups; g++) {
+                for (int64_t g = 0; g < groups; g++) {
                     columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
                 }
 
                 auto output_b = output[b];
                 col2im(
                         columns_view,
                         offset_c[b],
@@ -300,304 +315,293 @@
             }
 
             output = output.view({batch_sz, out_channels, out_h, out_w});
 
             return output + bias_c.view({1, out_channels, 1, 1});
         }
 
-        std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv_transpose2d_backward(
-                const at::Tensor &grad_out,
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const std::pair<int, int> &stride,
-                const std::pair<int, int> &padding,
-                const std::pair<int, int> &output_padding,
-                const std::pair<int, int> &dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
-            at::Tensor grad_out_c = grad_out.contiguous();
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_h = input_c.size(2);
-            int in_w = input_c.size(3);
-
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int out_channels = weight_c.size(1) * groups;
-            int weight_h = weight_c.size(2);
-            int weight_w = weight_c.size(3);
-
-            int stride_h = stride.first;
-            int stride_w = stride.second;
-
-            int pad_h = padding.first;
-            int pad_w = padding.second;
-
-            int out_pad_h = output_padding.first;
-            int out_pad_w = output_padding.second;
-
-            int dilation_h = dilation.first;
-            int dilation_w = dilation.second;
-
-            int out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
-            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
-
-            auto grad_input = at::zeros_like(input_c);
-            auto grad_weight = at::zeros_like(weight_c);
-            auto grad_offset = at::zeros_like(offset_c);
-            auto grad_mask = at::zeros_like(mask_c);
-            auto grad_bias = at::ones_like(bias_c);
-
-            // Separate into blocks
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          out_channels,
-                                          out_h,
-                                          out_w});
+        namespace detail {
+            std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
+            _deform_conv_transpose2d_backward(
+                    const at::Tensor &grad_out,
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const at::Tensor &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef output_padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups,
+                    bool deformable,
+                    bool modulated) {
+                at::Tensor grad_out_c = grad_out.contiguous();
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = offset.contiguous();
+                at::Tensor mask_c = mask.contiguous();
+                at::Tensor bias_c = bias.contiguous();
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_h = input_c.size(2);
+                int64_t in_w = input_c.size(3);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(1) * groups;
+                int64_t weight_h = weight_c.size(2);
+                int64_t weight_w = weight_c.size(3);
+
+                int64_t stride_h = stride[0];
+                int64_t stride_w = stride[1];
+
+                int64_t pad_h = padding[0];
+                int64_t pad_w = padding[1];
+
+                int64_t out_pad_h = output_padding[0];
+                int64_t out_pad_w = output_padding[1];
+
+                int64_t dilation_h = dilation[0];
+                int64_t dilation_w = dilation[1];
+
+                int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
+                int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+
+                int64_t offset_groups = offset.size(1) / (2 * weight_h * weight_w);
+                int64_t mask_groups = mask.size(1) / (weight_h * weight_w);
+
+                auto grad_input = at::zeros_like(input_c);
+                auto grad_weight = at::zeros_like(weight_c);
+                auto grad_offset = at::zeros_like(offset_c);
+                auto grad_mask = at::zeros_like(mask_c);
+                auto grad_bias = at::ones_like(bias_c);
 
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_h,
-                                    in_w});
-            grad_input = grad_input.view_as(input_c);
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                // Separate into blocks
+                grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              out_channels,
+                                              out_h,
+                                              out_w});
+
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_h,
+                                        in_w});
+                grad_input = grad_input.view_as(input_c);
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_h,
+                                              weight_w,
+                                              2,
+                                              in_h,
+                                              in_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0, 0, 0});
+                grad_offset = grad_offset.view_as(offset_c);
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_h,
                                           weight_w,
-                                          2,
                                           in_h,
                                           in_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0});
-            grad_offset = grad_offset.view_as(offset_c);
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_h,
-                                      weight_w,
-                                      in_h,
-                                      in_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0, 0, 0});
-            grad_mask = grad_mask.view_as(mask_c);
-
-            auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
-                                             in_channels,
-                                             n_parallel_imgs,
-                                             in_h,
-                                             in_w}, input_c.options());
-
-            // Separate channels into convolution groups
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    groups,
-                                    in_channels / groups,
-                                    in_h,
-                                    in_w}).permute({0, 2, 3, 1, 4, 5}).contiguous();
-
-            grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
-                                                  groups,
-                                                  grad_input_buf.size(1) / groups,
-                                                  grad_input_buf.size(2),
-                                                  grad_input_buf.size(3),
-                                                  grad_input_buf.size(4)});
-
-            weight_c = weight_c.view({groups,
-                                      in_channels / groups,
-                                      out_channels / groups,
-                                      weight_h,
-                                      weight_w});
-            grad_weight = grad_weight.view_as(weight_c);
-
-            auto columns = at::empty({groups,
-                                      out_channels * weight_h * weight_w / groups,
-                                      n_parallel_imgs * in_h * in_w},
-                                     input_c.options());
-            auto columns_view = columns.view({out_channels,
-                                              weight_h,
-                                              weight_w,
-                                              n_parallel_imgs,
-                                              in_h,
-                                              in_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
-                }
+                                          0, 0, 0, 0, 0});
+                grad_mask = grad_mask.view_as(mask_c);
 
-                auto grad_offset_b = grad_offset[b];
-                deform_conv2d_compute_grad_offset(
-                        columns_view,
-                        grad_out_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_h,
-                        out_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        in_h,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_offset_b);
-
-                auto grad_mask_b = grad_mask[b];
-                deform_conv2d_compute_grad_mask(
-                        columns_view,
-                        grad_out_c[b],
-                        offset_c[b],
-                        out_channels,
-                        out_h,
-                        out_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        in_h,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_mask_b);
-
-                im2col(
-                        grad_out_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_h,
-                        out_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        in_h,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
-
-                for (int g = 0; g < groups; g++) {
-                    grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                    grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
-                }
-            }
+                auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
+                                                 in_channels,
+                                                 n_parallel_imgs,
+                                                 in_h,
+                                                 in_w}, input_c.options());
+
+                // Separate channels into convolution groups
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        groups,
+                                        in_channels / groups,
+                                        in_h,
+                                        in_w}).permute({0, 2, 3, 1, 4, 5}).contiguous();
+
+                grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
+                                                      groups,
+                                                      grad_input_buf.size(1) / groups,
+                                                      grad_input_buf.size(2),
+                                                      grad_input_buf.size(3),
+                                                      grad_input_buf.size(4)});
+
+                weight_c = weight_c.view({groups,
+                                          in_channels / groups,
+                                          out_channels / groups,
+                                          weight_h,
+                                          weight_w});
+                grad_weight = grad_weight.view_as(weight_c);
 
-            grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
-                                                  in_channels,
+                auto columns = at::empty({groups,
+                                          out_channels * weight_h * weight_w / groups,
+                                          n_parallel_imgs * in_h * in_w},
+                                         input_c.options());
+                auto columns_view = columns.view({out_channels,
+                                                  weight_h,
+                                                  weight_w,
                                                   n_parallel_imgs,
                                                   in_h,
-                                                  in_w}).transpose_(1, 2);
-            grad_input.copy_(grad_input_buf);
+                                                  in_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    columns.zero_();
+                    for (int64_t g = 0; g < groups; g++) {
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                    }
+
+                    auto grad_offset_b = grad_offset[b];
+                    deform_conv2d_compute_grad_offset(
+                            columns_view,
+                            grad_out_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            out_channels,
+                            out_h,
+                            out_w,
+                            weight_h,
+                            weight_w,
+                            stride_h,
+                            stride_w,
+                            pad_h,
+                            pad_w,
+                            dilation_h,
+                            dilation_w,
+                            in_h,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_offset_b);
+
+                    auto grad_mask_b = grad_mask[b];
+                    deform_conv2d_compute_grad_mask(
+                            columns_view,
+                            grad_out_c[b],
+                            offset_c[b],
+                            out_channels,
+                            out_h,
+                            out_w,
+                            weight_h,
+                            weight_w,
+                            stride_h,
+                            stride_w,
+                            pad_h,
+                            pad_w,
+                            dilation_h,
+                            dilation_w,
+                            in_h,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_mask_b);
+
+                    im2col(
+                            grad_out_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            out_channels,
+                            out_h,
+                            out_w,
+                            weight_h,
+                            weight_w,
+                            stride_h,
+                            stride_w,
+                            pad_h,
+                            pad_w,
+                            dilation_h,
+                            dilation_w,
+                            in_h,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
+
+                    for (int64_t g = 0; g < groups; g++) {
+                        grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                        grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    }
+                }
 
-            grad_input = grad_input.view_as(input);
-            grad_weight = grad_weight.view_as(weight);
-            grad_offset = grad_offset.view_as(offset);
-            grad_mask = grad_mask.view_as(mask);
-            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
+                grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
+                                                      in_channels,
+                                                      n_parallel_imgs,
+                                                      in_h,
+                                                      in_w}).transpose_(1, 2);
+                grad_input.copy_(grad_input_buf);
+
+                grad_input = grad_input.view_as(input);
+                grad_weight = grad_weight.view_as(weight);
+                grad_offset = grad_offset.view_as(offset);
+                grad_mask = grad_mask.view_as(mask);
+                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
 
-            return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+                return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+            }
         }
 
         class DeformConvTranspose2dFunction
                 : public torch::autograd::Function<DeformConvTranspose2dFunction> {
         public:
             static torch::autograd::variable_list forward(
                     torch::autograd::AutogradContext *ctx,
                     const torch::autograd::Variable &input,
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
-                    int64_t stride_h,
-                    int64_t stride_w,
-                    int64_t pad_h,
-                    int64_t pad_w,
-                    int64_t out_pad_h,
-                    int64_t out_pad_w,
-                    int64_t dilation_h,
-                    int64_t dilation_w,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef output_padding,
+                    at::IntArrayRef dilation,
                     int64_t groups,
-                    int64_t offset_groups,
-                    int64_t mask_groups,
                     bool deformable,
                     bool modulated) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv_transpose2d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
-                        std::make_pair(stride_h, stride_w),
-                        std::make_pair(pad_h, pad_w),
-                        std::make_pair(out_pad_h, out_pad_w),
-                        std::make_pair(dilation_h, dilation_w),
+                        stride,
+                        padding,
+                        output_padding,
+                        dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride_h"] = stride_h;
-                ctx->saved_data["stride_w"] = stride_w;
-                ctx->saved_data["pad_h"] = pad_h;
-                ctx->saved_data["pad_w"] = pad_w;
-                ctx->saved_data["out_pad_h"] = out_pad_h;
-                ctx->saved_data["out_pad_w"] = out_pad_w;
-                ctx->saved_data["dilation_h"] = dilation_h;
-                ctx->saved_data["dilation_w"] = dilation_w;
+                ctx->saved_data["stride"] = stride.vec();
+                ctx->saved_data["padding"] = padding.vec();
+                ctx->saved_data["output_padding"] = output_padding.vec();
+                ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["offset_groups"] = offset_groups;
-                ctx->saved_data["mask_groups"] = mask_groups;
                 ctx->saved_data["deformable"] = deformable;
                 ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
@@ -608,42 +612,34 @@
                 auto saved = ctx->get_saved_variables();
                 auto input = saved[0];
                 auto weight = saved[1];
                 auto offset = saved[2];
                 auto mask = saved[3];
                 auto bias = saved[4];
 
-                auto stride_h = ctx->saved_data["stride_h"].toInt();
-                auto stride_w = ctx->saved_data["stride_w"].toInt();
-                auto pad_h = ctx->saved_data["pad_h"].toInt();
-                auto pad_w = ctx->saved_data["pad_w"].toInt();
-                auto out_pad_h = ctx->saved_data["out_pad_h"].toInt();
-                auto out_pad_w = ctx->saved_data["out_pad_w"].toInt();
-                auto dilation_h = ctx->saved_data["dilation_h"].toInt();
-                auto dilation_w = ctx->saved_data["dilation_w"].toInt();
+                auto stride = ctx->saved_data["stride"].toIntVector();
+                auto padding = ctx->saved_data["padding"].toIntVector();
+                auto output_padding = ctx->saved_data["output_padding"].toIntVector();
+                auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
-                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
                 auto deformable = ctx->saved_data["deformable"].toBool();
                 auto modulated = ctx->saved_data["modulated"].toBool();
 
-                auto grads = deform_conv_transpose2d_backward(
+                auto grads = detail::_deform_conv_transpose2d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
-                        std::make_pair(stride_h, stride_w),
-                        std::make_pair(pad_h, pad_w),
-                        std::make_pair(out_pad_h, out_pad_w),
-                        std::make_pair(dilation_h, dilation_w),
+                        stride,
+                        padding,
+                        output_padding,
+                        dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
@@ -657,60 +653,48 @@
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv_transpose2d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t out_pad_h,
-                const int64_t out_pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t groups,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                const at::optional<at::Tensor> &offset = {},
+                const at::optional<at::Tensor> &mask = {},
+                const at::optional<at::Tensor> &bias = {},
+                at::IntArrayRef stride = 1,
+                at::IntArrayRef padding = 0,
+                at::IntArrayRef output_padding = 0,
+                at::IntArrayRef dilation = 1,
+                int64_t groups = 1) {
             C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose2d");
             auto result = DeformConvTranspose2dFunction::apply(
                     input,
                     weight,
-                    offset,
-                    mask,
-                    bias,
-                    stride_h,
-                    stride_w,
-                    pad_h,
-                    pad_w,
-                    out_pad_h,
-                    out_pad_w,
-                    dilation_h,
-                    dilation_w,
+                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    stride,
+                    padding,
+                    output_padding,
+                    dilation,
                     groups,
-                    offset_groups,
-                    mask_groups,
-                    deformable,
-                    modulated);
+                    offset.has_value(),
+                    mask.has_value());
             return result[0];
         }
+
+        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
+            m.def("tvdcn::deform_conv_transpose2d(Tensor input, Tensor weight, "
+                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
+                  "int[2] stride=1, int[2] padding=0, int[2] output_padding=0, "
+                  "int[2] dilation=1, int groups=1) -> Tensor",
+                  &deform_conv_transpose2d);
+        }
     }
 }
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -77,23 +77,21 @@
     namespace ops {
         at::Tensor deform_conv_transpose3d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const std::tuple<int, int, int> &stride,
-                const std::tuple<int, int, int> &padding,
-                const std::tuple<int, int, int> &output_padding,
-                const std::tuple<int, int, int> &dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                at::IntArrayRef stride,
+                at::IntArrayRef padding,
+                at::IntArrayRef output_padding,
+                at::IntArrayRef dilation,
+                int64_t groups,
+                bool deformable,
+                bool modulated) {
             at::CheckedFrom c = "deform_conv_transpose3d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
@@ -104,50 +102,50 @@
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             TORCH_CHECK(input_c.ndimension() == 5)
+            TORCH_CHECK(weight_c.ndimension() == 5)
             TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
             TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
-            TORCH_CHECK(weight_c.ndimension() == 5)
 
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_d = input_c.size(2);
-            int in_h = input_c.size(3);
-            int in_w = input_c.size(4);
-
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int out_channels = weight_c.size(1) * groups;
-            int weight_d = weight_c.size(2);
-            int weight_h = weight_c.size(3);
-            int weight_w = weight_c.size(4);
-
-            int stride_d = std::get<0>(stride);
-            int stride_h = std::get<1>(stride);
-            int stride_w = std::get<2>(stride);
-
-            int pad_d = std::get<0>(padding);
-            int pad_h = std::get<1>(padding);
-            int pad_w = std::get<2>(padding);
-
-            int out_pad_d = std::get<0>(output_padding);
-            int out_pad_h = std::get<1>(output_padding);
-            int out_pad_w = std::get<2>(output_padding);
-
-            int dilation_d = std::get<0>(dilation);
-            int dilation_h = std::get<1>(dilation);
-            int dilation_w = std::get<2>(dilation);
-
-            int out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
-            int out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
-            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+            int64_t batch_sz = input_c.size(0);
+            int64_t in_channels = input_c.size(1);
+            int64_t in_d = input_c.size(2);
+            int64_t in_h = input_c.size(3);
+            int64_t in_w = input_c.size(4);
+
+            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+            int64_t out_channels = weight_c.size(1) * groups;
+            int64_t weight_d = weight_c.size(2);
+            int64_t weight_h = weight_c.size(3);
+            int64_t weight_w = weight_c.size(4);
+
+            int64_t stride_d = stride[0];
+            int64_t stride_h = stride[1];
+            int64_t stride_w = stride[2];
+
+            int64_t pad_d = padding[0];
+            int64_t pad_h = padding[1];
+            int64_t pad_w = padding[2];
+
+            int64_t out_pad_d = output_padding[0];
+            int64_t out_pad_h = output_padding[1];
+            int64_t out_pad_w = output_padding[2];
+
+            int64_t dilation_d = dilation[0];
+            int64_t dilation_h = dilation[1];
+            int64_t dilation_w = dilation[2];
+
+            int64_t out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
+            int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
+            int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
             TORCH_CHECK(
                     weight_d > 0 && weight_h > 0 && weight_w > 0,
                     "weight_d: ",
                     weight_d,
                     " weight_h: ",
                     weight_h,
@@ -163,15 +161,32 @@
                     stride_w)
             TORCH_CHECK(pad_d >= 0 && pad_h >= 0 && pad_w >= 0, "pad_d: ", pad_d, " pad_h: ", pad_h, " pad_w: ", pad_w)
             TORCH_CHECK(dilation_d > 0 && dilation_h > 0 && dilation_w > 0, "dilation_d: ", dilation_d, " dilation_h: ",
                         dilation_h, " dilation_w: ", dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+            int64_t offset_groups = offset.size(1) / (3 * weight_d * weight_h * weight_w);
+            int64_t mask_groups = mask.size(1) / (weight_d * weight_h * weight_w);
+
+            TORCH_CHECK(!deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
+                        offset.size(1),
+                        ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
+                        3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+
+            TORCH_CHECK(!modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
+                        mask.size(1),
+                        ", while weight.size(2) * weight.size(3) * weight.size(4)=",
+                        weight_d * weight_h * weight_w)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
@@ -296,17 +311,17 @@
                                               weight_d,
                                               weight_h,
                                               weight_w,
                                               n_parallel_imgs,
                                               in_d,
                                               in_h,
                                               in_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
+            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 columns.zero_();
-                for (int g = 0; g < groups; g++) {
+                for (int64_t g = 0; g < groups; g++) {
                     columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
                 }
 
                 auto output_b = output[b];
                 col2vol(
                         columns_view,
                         offset_c[b],
@@ -339,350 +354,331 @@
             }
 
             output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
 
             return output + bias_c.view({1, out_channels, 1, 1, 1});
         }
 
-        std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv_transpose3d_backward(
-                const at::Tensor &grad_out,
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const std::tuple<int, int, int> &stride,
-                const std::tuple<int, int, int> &padding,
-                const std::tuple<int, int, int> &output_padding,
-                const std::tuple<int, int, int> &dilation,
-                const int groups,
-                const int offset_groups,
-                const int mask_groups,
-                const bool deformable,
-                const bool modulated) {
-            at::Tensor grad_out_c = grad_out.contiguous();
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            int batch_sz = input_c.size(0);
-            int in_channels = input_c.size(1);
-            int in_d = input_c.size(2);
-            int in_h = input_c.size(3);
-            int in_w = input_c.size(4);
-
-            int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int out_channels = weight_c.size(1) * groups;
-            int weight_d = weight_c.size(2);
-            int weight_h = weight_c.size(3);
-            int weight_w = weight_c.size(4);
-
-            int stride_d = std::get<0>(stride);
-            int stride_h = std::get<1>(stride);
-            int stride_w = std::get<2>(stride);
-
-            int pad_d = std::get<0>(padding);
-            int pad_h = std::get<1>(padding);
-            int pad_w = std::get<2>(padding);
-
-            int out_pad_d = std::get<0>(output_padding);
-            int out_pad_h = std::get<1>(output_padding);
-            int out_pad_w = std::get<2>(output_padding);
-
-            int dilation_d = std::get<0>(dilation);
-            int dilation_h = std::get<1>(dilation);
-            int dilation_w = std::get<2>(dilation);
-
-            int out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
-            int out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
-            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
-
-            auto grad_input = at::zeros_like(input_c);
-            auto grad_weight = at::zeros_like(weight_c);
-            auto grad_offset = at::zeros_like(offset_c);
-            auto grad_mask = at::zeros_like(mask_c);
-            auto grad_bias = at::ones_like(bias_c);
-
-            // Separate into blocks
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          out_channels,
-                                          out_d,
-                                          out_h,
-                                          out_w});
+        namespace detail {
+            std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
+            _deform_conv_transpose3d_backward(
+                    const at::Tensor &grad_out,
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const at::Tensor &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef output_padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups,
+                    bool deformable,
+                    bool modulated) {
+                at::Tensor grad_out_c = grad_out.contiguous();
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = offset.contiguous();
+                at::Tensor mask_c = mask.contiguous();
+                at::Tensor bias_c = bias.contiguous();
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_d = input_c.size(2);
+                int64_t in_h = input_c.size(3);
+                int64_t in_w = input_c.size(4);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(1) * groups;
+                int64_t weight_d = weight_c.size(2);
+                int64_t weight_h = weight_c.size(3);
+                int64_t weight_w = weight_c.size(4);
+
+                int64_t stride_d = stride[0];
+                int64_t stride_h = stride[1];
+                int64_t stride_w = stride[2];
+
+                int64_t pad_d = padding[0];
+                int64_t pad_h = padding[1];
+                int64_t pad_w = padding[2];
+
+                int64_t out_pad_d = output_padding[0];
+                int64_t out_pad_h = output_padding[1];
+                int64_t out_pad_w = output_padding[2];
+
+                int64_t dilation_d = dilation[0];
+                int64_t dilation_h = dilation[1];
+                int64_t dilation_w = dilation[2];
+
+                int64_t out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
+                int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
+                int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+
+                int64_t offset_groups = offset.size(1) / (3 * weight_d * weight_h * weight_w);
+                int64_t mask_groups = mask.size(1) / (weight_d * weight_h * weight_w);
+
+                auto grad_input = at::zeros_like(input_c);
+                auto grad_weight = at::zeros_like(weight_c);
+                auto grad_offset = at::zeros_like(offset_c);
+                auto grad_mask = at::zeros_like(mask_c);
+                auto grad_bias = at::ones_like(bias_c);
 
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_d,
-                                    in_h,
-                                    in_w});
-            grad_input = grad_input.view_as(input_c);
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                // Separate into blocks
+                grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              out_channels,
+                                              out_d,
+                                              out_h,
+                                              out_w});
+
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_d,
+                                        in_h,
+                                        in_w});
+                grad_input = grad_input.view_as(input_c);
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_d,
+                                              weight_h,
+                                              weight_w,
+                                              3,
+                                              in_d,
+                                              in_h,
+                                              in_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0, 0, 0, 0, 0});
+                grad_offset = grad_offset.view_as(offset_c);
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_d,
                                           weight_h,
                                           weight_w,
-                                          3,
                                           in_d,
                                           in_h,
                                           in_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0, 0, 0});
-            grad_offset = grad_offset.view_as(offset_c);
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_d,
-                                      weight_h,
-                                      weight_w,
-                                      in_d,
-                                      in_h,
-                                      in_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0, 0, 0, 0, 0});
-            grad_mask = grad_mask.view_as(mask_c);
-
-            auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
-                                             in_channels,
-                                             n_parallel_imgs,
-                                             in_d,
-                                             in_h,
-                                             in_w}, input_c.options());
+                                          0, 0, 0, 0, 0, 0, 0});
+                grad_mask = grad_mask.view_as(mask_c);
 
-            // Separate channels into convolution groups
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    groups,
-                                    in_channels / groups,
-                                    in_d,
-                                    in_h,
-                                    in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
-
-            grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
-                                                  groups,
-                                                  grad_input_buf.size(1) / groups,
-                                                  grad_input_buf.size(2),
-                                                  grad_input_buf.size(3),
-                                                  grad_input_buf.size(4),
-                                                  grad_input_buf.size(5)});
-
-            weight_c = weight_c.view({groups,
-                                      in_channels / groups,
-                                      out_channels / groups,
-                                      weight_d,
-                                      weight_h,
-                                      weight_w});
-            grad_weight = grad_weight.view_as(weight_c);
-
-            auto columns = at::empty({groups,
-                                      out_channels * weight_d * weight_h * weight_w / groups,
-                                      n_parallel_imgs * in_d * in_h * in_w},
-                                     input_c.options());
-            auto columns_view = columns.view({out_channels,
-                                              weight_d,
-                                              weight_h,
-                                              weight_w,
-                                              n_parallel_imgs,
-                                              in_d,
-                                              in_h,
-                                              in_w});
-            for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
-                }
-
-                auto grad_offset_b = grad_offset[b];
-                deform_conv3d_compute_grad_offset(
-                        columns_view,
-                        grad_out_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_d,
-                        out_h,
-                        out_w,
-                        weight_d,
-                        weight_h,
-                        weight_w,
-                        stride_d,
-                        stride_h,
-                        stride_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
-                        dilation_d,
-                        dilation_h,
-                        dilation_w,
-                        in_d,
-                        in_h,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_offset_b);
-
-                auto grad_mask_b = grad_mask[b];
-                deform_conv3d_compute_grad_mask(
-                        columns_view,
-                        grad_out_c[b],
-                        offset_c[b],
-                        out_channels,
-                        out_d,
-                        out_h,
-                        out_w,
-                        weight_d,
-                        weight_h,
-                        weight_w,
-                        stride_d,
-                        stride_h,
-                        stride_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
-                        dilation_d,
-                        dilation_h,
-                        dilation_w,
-                        in_d,
-                        in_h,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_mask_b);
-
-                vol2col(
-                        grad_out_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_d,
-                        out_h,
-                        out_w,
-                        weight_d,
-                        weight_h,
-                        weight_w,
-                        stride_d,
-                        stride_h,
-                        stride_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
-                        dilation_d,
-                        dilation_h,
-                        dilation_w,
-                        in_d,
-                        in_h,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
-
-                for (int g = 0; g < groups; g++) {
-                    grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                    grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
-                }
-            }
+                auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
+                                                 in_channels,
+                                                 n_parallel_imgs,
+                                                 in_d,
+                                                 in_h,
+                                                 in_w}, input_c.options());
+
+                // Separate channels into convolution groups
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        groups,
+                                        in_channels / groups,
+                                        in_d,
+                                        in_h,
+                                        in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
+
+                grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
+                                                      groups,
+                                                      grad_input_buf.size(1) / groups,
+                                                      grad_input_buf.size(2),
+                                                      grad_input_buf.size(3),
+                                                      grad_input_buf.size(4),
+                                                      grad_input_buf.size(5)});
+
+                weight_c = weight_c.view({groups,
+                                          in_channels / groups,
+                                          out_channels / groups,
+                                          weight_d,
+                                          weight_h,
+                                          weight_w});
+                grad_weight = grad_weight.view_as(weight_c);
 
-            grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
-                                                  in_channels,
+                auto columns = at::empty({groups,
+                                          out_channels * weight_d * weight_h * weight_w / groups,
+                                          n_parallel_imgs * in_d * in_h * in_w},
+                                         input_c.options());
+                auto columns_view = columns.view({out_channels,
+                                                  weight_d,
+                                                  weight_h,
+                                                  weight_w,
                                                   n_parallel_imgs,
                                                   in_d,
                                                   in_h,
-                                                  in_w}).transpose_(1, 2);
-            grad_input.copy_(grad_input_buf);
+                                                  in_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    columns.zero_();
+                    for (int64_t g = 0; g < groups; g++) {
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                    }
+
+                    auto grad_offset_b = grad_offset[b];
+                    deform_conv3d_compute_grad_offset(
+                            columns_view,
+                            grad_out_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            out_channels,
+                            out_d,
+                            out_h,
+                            out_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            in_d,
+                            in_h,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_offset_b);
+
+                    auto grad_mask_b = grad_mask[b];
+                    deform_conv3d_compute_grad_mask(
+                            columns_view,
+                            grad_out_c[b],
+                            offset_c[b],
+                            out_channels,
+                            out_d,
+                            out_h,
+                            out_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            in_d,
+                            in_h,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_mask_b);
+
+                    vol2col(
+                            grad_out_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            out_channels,
+                            out_d,
+                            out_h,
+                            out_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            in_d,
+                            in_h,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
+
+                    for (int64_t g = 0; g < groups; g++) {
+                        grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                        grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    }
+                }
 
-            grad_input = grad_input.view_as(input);
-            grad_weight = grad_weight.view_as(weight);
-            grad_offset = grad_offset.view_as(offset);
-            grad_mask = grad_mask.view_as(mask);
-            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
+                grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
+                                                      in_channels,
+                                                      n_parallel_imgs,
+                                                      in_d,
+                                                      in_h,
+                                                      in_w}).transpose_(1, 2);
+                grad_input.copy_(grad_input_buf);
+
+                grad_input = grad_input.view_as(input);
+                grad_weight = grad_weight.view_as(weight);
+                grad_offset = grad_offset.view_as(offset);
+                grad_mask = grad_mask.view_as(mask);
+                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
 
-            return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+                return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
+            }
         }
 
         class DeformConvTranspose3dFunction
                 : public torch::autograd::Function<DeformConvTranspose3dFunction> {
         public:
             static torch::autograd::variable_list forward(
                     torch::autograd::AutogradContext *ctx,
                     const torch::autograd::Variable &input,
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
-                    int64_t stride_d,
-                    int64_t stride_h,
-                    int64_t stride_w,
-                    int64_t pad_d,
-                    int64_t pad_h,
-                    int64_t pad_w,
-                    int64_t out_pad_d,
-                    int64_t out_pad_h,
-                    int64_t out_pad_w,
-                    int64_t dilation_d,
-                    int64_t dilation_h,
-                    int64_t dilation_w,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef output_padding,
+                    at::IntArrayRef dilation,
                     int64_t groups,
-                    int64_t offset_groups,
-                    int64_t mask_groups,
                     bool deformable,
                     bool modulated) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv_transpose3d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
-                        std::make_tuple(stride_d, stride_h, stride_w),
-                        std::make_tuple(pad_d, pad_h, pad_w),
-                        std::make_tuple(out_pad_d, out_pad_h, out_pad_w),
-                        std::make_tuple(dilation_d, dilation_h, dilation_w),
+                        stride,
+                        padding,
+                        output_padding,
+                        dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride_d"] = stride_d;
-                ctx->saved_data["stride_h"] = stride_h;
-                ctx->saved_data["stride_w"] = stride_w;
-                ctx->saved_data["pad_d"] = pad_d;
-                ctx->saved_data["pad_h"] = pad_h;
-                ctx->saved_data["pad_w"] = pad_w;
-                ctx->saved_data["out_pad_d"] = out_pad_d;
-                ctx->saved_data["out_pad_h"] = out_pad_h;
-                ctx->saved_data["out_pad_w"] = out_pad_w;
-                ctx->saved_data["dilation_d"] = dilation_d;
-                ctx->saved_data["dilation_h"] = dilation_h;
-                ctx->saved_data["dilation_w"] = dilation_w;
+                ctx->saved_data["stride"] = stride.vec();
+                ctx->saved_data["padding"] = padding.vec();
+                ctx->saved_data["output_padding"] = output_padding.vec();
+                ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["offset_groups"] = offset_groups;
-                ctx->saved_data["mask_groups"] = mask_groups;
                 ctx->saved_data["deformable"] = deformable;
                 ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
@@ -693,46 +689,34 @@
                 auto saved = ctx->get_saved_variables();
                 auto input = saved[0];
                 auto weight = saved[1];
                 auto offset = saved[2];
                 auto mask = saved[3];
                 auto bias = saved[4];
 
-                auto stride_d = ctx->saved_data["stride_d"].toInt();
-                auto stride_h = ctx->saved_data["stride_h"].toInt();
-                auto stride_w = ctx->saved_data["stride_w"].toInt();
-                auto pad_d = ctx->saved_data["pad_d"].toInt();
-                auto pad_h = ctx->saved_data["pad_h"].toInt();
-                auto pad_w = ctx->saved_data["pad_w"].toInt();
-                auto out_pad_d = ctx->saved_data["out_pad_d"].toInt();
-                auto out_pad_h = ctx->saved_data["out_pad_h"].toInt();
-                auto out_pad_w = ctx->saved_data["out_pad_w"].toInt();
-                auto dilation_d = ctx->saved_data["dilation_d"].toInt();
-                auto dilation_h = ctx->saved_data["dilation_h"].toInt();
-                auto dilation_w = ctx->saved_data["dilation_w"].toInt();
+                auto stride = ctx->saved_data["stride"].toIntVector();
+                auto padding = ctx->saved_data["padding"].toIntVector();
+                auto output_padding = ctx->saved_data["output_padding"].toIntVector();
+                auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
-                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
                 auto deformable = ctx->saved_data["deformable"].toBool();
                 auto modulated = ctx->saved_data["modulated"].toBool();
 
-                auto grads = deform_conv_transpose3d_backward(
+                auto grads = detail::_deform_conv_transpose3d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
-                        std::make_tuple(stride_d, stride_h, stride_w),
-                        std::make_tuple(pad_d, pad_h, pad_w),
-                        std::make_tuple(out_pad_d, out_pad_h, out_pad_w),
-                        std::make_tuple(dilation_d, dilation_h, dilation_w),
+                        stride,
+                        padding,
+                        output_padding,
+                        dilation,
                         groups,
-                        offset_groups,
-                        mask_groups,
                         deformable,
                         modulated);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
@@ -746,72 +730,48 @@
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv_transpose3d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t out_pad_d,
-                const int64_t out_pad_h,
-                const int64_t out_pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t groups,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated) {
+                const at::optional<at::Tensor> &offset = {},
+                const at::optional<at::Tensor> &mask = {},
+                const at::optional<at::Tensor> &bias = {},
+                at::IntArrayRef stride = 1,
+                at::IntArrayRef padding = 0,
+                at::IntArrayRef output_padding = 0,
+                at::IntArrayRef dilation = 1,
+                int64_t groups = 1) {
             C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose3d");
             auto result = DeformConvTranspose3dFunction::apply(
                     input,
                     weight,
-                    offset,
-                    mask,
-                    bias,
-                    stride_d,
-                    stride_h,
-                    stride_w,
-                    pad_d,
-                    pad_h,
-                    pad_w,
-                    out_pad_d,
-                    out_pad_h,
-                    out_pad_w,
-                    dilation_d,
-                    dilation_h,
-                    dilation_w,
+                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
+                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    stride,
+                    padding,
+                    output_padding,
+                    dilation,
                     groups,
-                    offset_groups,
-                    mask_groups,
-                    deformable,
-                    modulated);
+                    offset.has_value(),
+                    mask.has_value());
             return result[0];
         }
+
+        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
+            m.def("tvdcn::deform_conv_transpose3d(Tensor input, Tensor weight, "
+                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
+                  "int[3] stride=1, int[3] padding=0, int[3] output_padding=0, "
+                  "int[3] dilation=1, int groups=1) -> Tensor",
+                  &deform_conv_transpose3d);
+        }
     }
 }
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 namespace tvdcn {
     namespace ops {
         void arr2col(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 arr2col_cuda(input,
                              offset,
@@ -66,24 +66,24 @@
             }
         }
 
         void col2arr(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 col2arr_cuda(columns,
                              offset,
@@ -125,24 +125,24 @@
         }
 
         void deform_conv1d_compute_grad_offset(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 deform_conv1d_compute_grad_offset_cuda(columns,
                                                        input,
@@ -185,24 +185,24 @@
             }
         }
 
         void deform_conv1d_compute_grad_mask(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int width,
-                const int weight_w,
-                const int stride_w,
-                const int pad_w,
-                const int dilation_w,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t width,
+                const int64_t weight_w,
+                const int64_t stride_w,
+                const int64_t pad_w,
+                const int64_t dilation_w,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 deform_conv1d_compute_grad_mask_cuda(columns,
                                                      input,
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 namespace tvdcn {
     namespace ops {
         void im2col(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 im2col_cuda(input,
                             offset,
@@ -84,30 +84,30 @@
             }
         }
 
         void col2im(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 col2im_cuda(columns,
                             offset,
@@ -161,30 +161,30 @@
         }
 
         void deform_conv2d_compute_grad_offset(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 deform_conv2d_compute_grad_offset_cuda(columns,
                                                        input,
@@ -239,30 +239,30 @@
             }
         }
 
         void deform_conv2d_compute_grad_mask(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int height,
-                const int width,
-                const int weight_h,
-                const int weight_w,
-                const int stride_h,
-                const int stride_w,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 deform_conv2d_compute_grad_mask_cuda(columns,
                                                      input,
```

### Comparing `tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 
 namespace tvdcn {
     namespace ops {
         void vol2col(
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 vol2col_cuda(input,
                              offset,
@@ -102,36 +102,36 @@
             }
         }
 
         void col2vol(
                 const at::Tensor &columns,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 col2vol_cuda(columns,
                              offset,
@@ -197,36 +197,36 @@
         }
 
         void deform_conv3d_compute_grad_offset(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 deform_conv3d_compute_grad_offset_cuda(columns,
                                                        input,
@@ -293,36 +293,36 @@
             }
         }
 
         void deform_conv3d_compute_grad_mask(
                 const at::Tensor &columns,
                 const at::Tensor &input,
                 const at::Tensor &offset,
-                const int in_channels,
-                const int depth,
-                const int height,
-                const int width,
-                const int weight_d,
-                const int weight_h,
-                const int weight_w,
-                const int stride_d,
-                const int stride_h,
-                const int stride_w,
-                const int pad_d,
-                const int pad_h,
-                const int pad_w,
-                const int dilation_d,
-                const int dilation_h,
-                const int dilation_w,
-                const int out_d,
-                const int out_h,
-                const int out_w,
-                const int batch_sz,
-                const int offset_groups,
-                const int mask_groups,
+                const int64_t in_channels,
+                const int64_t depth,
+                const int64_t height,
+                const int64_t width,
+                const int64_t weight_d,
+                const int64_t weight_h,
+                const int64_t weight_w,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t out_d,
+                const int64_t out_h,
+                const int64_t out_w,
+                const int64_t batch_sz,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.device().is_cuda()) {
 #if defined(WITH_CUDA)
                 deform_conv3d_compute_grad_mask_cuda(columns,
                                                      input,
```

### Comparing `tvdcn-0.2.7/tvdcn/extension.py` & `tvdcn-0.3.0/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.3.0/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.3.0/tvdcn/ops/activations/mask_softmax.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/tvdcn/ops/deform_conv.py` & `tvdcn-0.3.0/tvdcn/ops/deform_conv.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 def deform_conv1d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Tuple[int] = (1,),
-        padding: Tuple[int] = (0,),
-        dilation: Tuple[int] = (1,),
+        stride: _size_1_t = 1,
+        padding: _size_1_t = 0,
+        dilation: _size_1_t = 1,
         groups: int = 1) -> Tensor:
     r"""
     Performs 1D Deformable Convolution.
 
     Arguments:
         input (Tensor[batch_size, in_channels, in_width]): input tensor
         weight (Tensor[out_channels, in_channels // groups, kernel_width]):
@@ -72,75 +72,28 @@
         >>> print(out.shape)
         Output:
         >>>  torch.Size([4, 5, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv1d)
     _assert_has_ops()
-    out_channels = weight.size(0)
 
-    deformable = offset is not None
-    modulated = mask is not None
-
-    if offset is None:
-        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if mask is None:
-        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if bias is None:
-        bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
-
-    stride = _single(stride)
-    pad = _single(padding)
-    dil = _single(dilation)
-
-    weight_w = weight.size(-1)
-    _, n_in_channels, in_w = input.size()
-
-    assert groups == n_in_channels // weight.size(1)
-    offset_groups = offset.size(1) // weight_w
-    mask_groups = mask.size(1) // weight_w
-
-    if deformable and offset_groups == 0:
-        raise RuntimeError(
-            "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size(2).\n"
-            "Got offset.size(1)={}, while weight.size(2)={}".format(
-                offset.size(1), weight_w))
-    if modulated and mask_groups == 0:
-        raise RuntimeError(
-            "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size(2).\n"
-            "Got mask.size(1)={}, while weight.size(2)={}".format(
-                mask.size(1), weight_w))
-
-    return torch.ops.tvdcn.deform_conv1d(
-        input,
-        weight,
-        offset,
-        mask,
-        bias,
-        stride[0],
-        pad[0],
-        dil[0],
-        groups,
-        offset_groups,
-        mask_groups,
-        deformable,
-        modulated)
+    return torch.ops.tvdcn.deform_conv1d(input, weight, offset, mask, bias,
+                                         stride, padding, dilation, groups)
 
 
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Tuple[int, int] = (1, 1),
-        padding: Tuple[int, int] = (0, 0),
-        dilation: Tuple[int, int] = (1, 1),
+        stride: _size_2_t = 1,
+        padding: _size_2_t = 0,
+        dilation: _size_2_t = 1,
         groups: int = 1) -> Tensor:
     r"""
     Performs 2D Deformable Convolution.
 
     References:
         https://arxiv.org/abs/1811.11168
         https://arxiv.org/abs/1703.06211
@@ -179,74 +132,28 @@
         >>> print(out.shape)
         Output:
         >>>  torch.Size([4, 5, 8, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv2d)
     _assert_has_ops()
-    out_channels = weight.size(0)
-
-    deformable = offset is not None
-    modulated = mask is not None
 
-    if offset is None:
-        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if mask is None:
-        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if bias is None:
-        bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
-
-    stride_h, stride_w = _pair(stride)
-    pad_h, pad_w = _pair(padding)
-    dil_h, dil_w = _pair(dilation)
-    weight_h, weight_w = weight.size()[-2:]
-    _, n_in_channels, in_h, in_w = input.size()
-
-    assert groups == n_in_channels // weight.size(1)
-    offset_groups = offset.size(1) // (2 * weight_h * weight_w)
-    mask_groups = mask.size(1) // (weight_h * weight_w)
-
-    if deformable and offset_groups == 0:
-        raise RuntimeError(
-            "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of 2 * weight.size(2) * weight.size(3).\n"
-            "Got offset.size(1)={}, while 2 * weight.size(2) * weight.size(3)={}".format(
-                offset.size(1), 2 * weight_h * weight_w))
-    if modulated and mask_groups == 0:
-        raise RuntimeError(
-            "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size(2) * weight.size(3).\n"
-            "Got mask.size(1)={}, while weight.size(2) * weight.size(3)={}".format(
-                mask.size(1), weight_h * weight_w))
-
-    return torch.ops.tvdcn.deform_conv2d(
-        input,
-        weight,
-        offset,
-        mask,
-        bias,
-        stride_h, stride_w,
-        pad_h, pad_w,
-        dil_h, dil_w,
-        groups,
-        offset_groups,
-        mask_groups,
-        deformable,
-        modulated)
+    return torch.ops.tvdcn.deform_conv2d(input, weight, offset, mask, bias,
+                                         stride, padding, dilation, groups)
 
 
 def deform_conv3d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Tuple[int, int, int] = (1, 1, 1),
-        padding: Tuple[int, int, int] = (0, 0, 0),
-        dilation: Tuple[int, int, int] = (1, 1, 1),
+        stride: _size_3_t = 1,
+        padding: _size_3_t = 0,
+        dilation: _size_3_t = 1,
         groups: int = 1) -> Tensor:
     r"""
     Performs 3D Deformable Convolution.
 
     Arguments:
         input (Tensor[batch_size, in_channels, in_height, in_width, in_depth]): input tensor
         weight (Tensor[out_channels, in_channels // groups, kernel_depth, kernel_height, kernel_width]):
@@ -281,63 +188,17 @@
         >>> print(out.shape)
         Output:
         >>> torch.Size([4, 5, 8, 8, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv3d)
     _assert_has_ops()
-    out_channels = weight.size(0)
-
-    deformable = offset is not None
-    modulated = mask is not None
 
-    if offset is None:
-        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if mask is None:
-        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if bias is None:
-        bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
-
-    stride_d, stride_h, stride_w = _triple(stride)
-    pad_d, pad_h, pad_w = _triple(padding)
-    dil_d, dil_h, dil_w = _triple(dilation)
-    weight_d, weight_h, weight_w = weight.size()[-3:]
-    _, n_in_channels, in_d, in_h, in_w = input.size()
-
-    assert groups == n_in_channels // weight.size(1)
-    offset_groups = offset.size(1) // (3 * weight_d * weight_h * weight_w)
-    mask_groups = mask.size(1) // (weight_d * weight_h * weight_w)
-
-    if deformable and offset_groups == 0:
-        raise RuntimeError(
-            "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\n"
-            "Got offset.size(1)={}, while 3 * weight.size(2) * weight.size(3) * weight.size(4)={}".format(
-                offset.size(1), 3 * weight_d * weight_h * weight_w))
-    if modulated and mask_groups == 0:
-        raise RuntimeError(
-            "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\n"
-            "Got mask.size(1)={}, while weight.size(2) * weight.size(3) * weight.size(4)={}".format(
-                mask.size(1), weight_d * weight_h * weight_w))
-
-    return torch.ops.tvdcn.deform_conv3d(
-        input,
-        weight,
-        offset,
-        mask,
-        bias,
-        stride_d, stride_h, stride_w,
-        pad_d, pad_h, pad_w,
-        dil_d, dil_h, dil_w,
-        groups,
-        offset_groups,
-        mask_groups,
-        deformable,
-        modulated)
+    return torch.ops.tvdcn.deform_conv3d(input, weight, offset, mask, bias,
+                                         stride, padding, dilation, groups)
 
 
 ################################################################################
 # Modules
 ################################################################################
 # noinspection PyMethodOverriding
 class _DeformConvNd(_ConvNd):
```

### Comparing `tvdcn-0.2.7/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.3.0/tvdcn/ops/deform_conv_transpose.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 
 def deform_conv_transpose1d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Tuple[int] = (1,),
-        padding: Tuple[int] = (0,),
-        output_padding: Tuple[int] = (0,),
-        dilation: Tuple[int] = (1,),
+        stride: _size_1_t = 1,
+        padding: _size_1_t = 0,
+        output_padding: _size_1_t = 0,
+        dilation: _size_1_t = 1,
         groups: int = 1) -> Tensor:
     r"""
     Performs 1D Transposed Deformable Convolution.
 
     Arguments:
         input (Tensor[batch_size, in_channels, in_width]): input tensor
         weight (Tensor[in_channels, out_channels // groups, kernel_width]):
@@ -73,77 +73,29 @@
         >>> print(out.shape)
         Output:
         >>>  torch.Size([4, 5, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose1d)
     _assert_has_ops()
-    out_channels = weight.size(1) // groups
 
-    deformable = offset is not None
-    modulated = mask is not None
-
-    if offset is None:
-        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if mask is None:
-        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if bias is None:
-        bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
-
-    stride = _single(stride)
-    pad = _single(padding)
-    out_pad = _single(output_padding)
-    dil = _single(dilation)
-
-    weight_w = weight.size(-1)
-    _, _, in_w = input.size()
-
-    offset_groups = offset.size(1) // weight_w
-    mask_groups = mask.size(1) // weight_w
-
-    if deformable and offset_groups == 0:
-        raise RuntimeError(
-            "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size(2).\n"
-            "Got offset.size(1)={}, while weight.size(2)={}".format(
-                offset.size(1), weight_w))
-    if modulated and mask_groups == 0:
-        raise RuntimeError(
-            "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size(2).\n"
-            "Got mask.size(1)={}, while weight.size(2)={}".format(
-                mask.size(1), weight_w))
-
-    return torch.ops.tvdcn.deform_conv_transpose1d(
-        input,
-        weight,
-        offset,
-        mask,
-        bias,
-        stride[0],
-        pad[0],
-        out_pad[0],
-        dil[0],
-        groups,
-        offset_groups,
-        mask_groups,
-        deformable,
-        modulated)
+    return torch.ops.tvdcn.deform_conv_transpose1d(input, weight, offset, mask, bias,
+                                                   stride, padding, output_padding, dilation, groups)
 
 
 def deform_conv_transpose2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Tuple[int, int] = (1, 1),
-        padding: Tuple[int, int] = (0, 0),
-        output_padding: Tuple[int, int] = (0, 0),
-        dilation: Tuple[int, int] = (1, 1),
+        stride: _size_2_t = 1,
+        padding: _size_2_t = 0,
+        output_padding: _size_2_t = 0,
+        dilation: _size_2_t = 1,
         groups: int = 1) -> Tensor:
     r"""
     Performs 2D Transposed Deformable Convolution.
 
     Arguments:
         input (Tensor[batch_size, in_channels, in_height, in_width]): input tensor
         weight (Tensor[in_channels, out_channels // groups, kernel_height, kernel_width]):
@@ -177,76 +129,29 @@
         >>> print(out.shape)
         Output:
         >>>  torch.Size([4, 5, 10, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose2d)
     _assert_has_ops()
-    out_channels = weight.size(1) // groups
-
-    deformable = offset is not None
-    modulated = mask is not None
 
-    if offset is None:
-        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if mask is None:
-        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if bias is None:
-        bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
-
-    stride_h, stride_w = _pair(stride)
-    pad_h, pad_w = _pair(padding)
-    out_pad_h, out_pad_w = _pair(output_padding)
-    dil_h, dil_w = _pair(dilation)
-    weight_h, weight_w = weight.size()[-2:]
-    _, _, in_h, in_w = input.size()
-
-    offset_groups = offset.size(1) // (2 * weight_h * weight_w)
-    mask_groups = mask.size(1) // (weight_h * weight_w)
-
-    if deformable and offset_groups == 0:
-        raise RuntimeError(
-            "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of 2 * weight.size(2) * weight.size(3).\n"
-            "Got offset.size(1)={}, while 2 * weight.size(2) * weight.size(3)={}".format(
-                offset.size(1), 2 * weight_h * weight_w))
-    if modulated and mask_groups == 0:
-        raise RuntimeError(
-            "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size(2) * weight.size(3).\n"
-            "Got mask.size(1)={}, while weight.size(2) * weight.size(3)={}".format(
-                mask.size(1), weight_h * weight_w))
-
-    return torch.ops.tvdcn.deform_conv_transpose2d(
-        input,
-        weight,
-        offset,
-        mask,
-        bias,
-        stride_h, stride_w,
-        pad_h, pad_w,
-        out_pad_h, out_pad_w,
-        dil_h, dil_w,
-        groups,
-        offset_groups,
-        mask_groups,
-        deformable,
-        modulated)
+    return torch.ops.tvdcn.deform_conv_transpose2d(input, weight, offset, mask, bias,
+                                                   stride, padding, output_padding, dilation, groups)
 
 
 def deform_conv_transpose3d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
         bias: Optional[Tensor] = None,
-        stride: Tuple[int, int, int] = (1, 1, 1),
-        padding: Tuple[int, int, int] = (0, 0, 0),
-        output_padding: Tuple[int, int, int] = (0, 0, 0),
-        dilation: Tuple[int, int, int] = (1, 1, 1),
+        stride: _size_3_t = 1,
+        padding: _size_3_t = 0,
+        output_padding: _size_3_t = 0,
+        dilation: _size_3_t = 1,
         groups: int = 1) -> Tensor:
     r"""
     Performs 3D Transposed Deformable Convolution.
 
     Arguments:
         input (Tensor[batch_size, in_channels, in_height, in_width, in_depth]): input tensor
         weight (Tensor[in_channels, out_channels // groups, kernel_depth, kernel_height, kernel_width]):
@@ -281,64 +186,17 @@
         >>> print(out.shape)
         Output:
         >>> torch.Size([4, 5, 10, 10, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose3d)
     _assert_has_ops()
-    out_channels = weight.size(1) // groups
-
-    deformable = offset is not None
-    modulated = mask is not None
 
-    if offset is None:
-        offset = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if mask is None:
-        mask = torch.zeros((input.size(0), 0), device=input.device, dtype=input.dtype)
-    if bias is None:
-        bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
-
-    stride_d, stride_h, stride_w = _triple(stride)
-    pad_d, pad_h, pad_w = _triple(padding)
-    out_pad_d, out_pad_h, out_pad_w = _triple(output_padding)
-    dil_d, dil_h, dil_w = _triple(dilation)
-    weight_d, weight_h, weight_w = weight.size()[-3:]
-    _, _, in_d, in_h, in_w = input.size()
-
-    offset_groups = offset.size(1) // (3 * weight_d * weight_h * weight_w)
-    mask_groups = mask.size(1) // (weight_d * weight_h * weight_w)
-
-    if deformable and offset_groups == 0:
-        raise RuntimeError(
-            "The shape of the offset tensor at dimension 1 is not valid. It should "
-            "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\n"
-            "Got offset.size(1)={}, while 3 * weight.size(2) * weight.size(3) * weight.size(4)={}".format(
-                offset.size(1), 3 * weight_d * weight_h * weight_w))
-    if modulated and mask_groups == 0:
-        raise RuntimeError(
-            "The shape of the mask tensor at dimension 1 is not valid. It should "
-            "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\n"
-            "Got mask.size(1)={}, while weight.size(2) * weight.size(3) * weight.size(4)={}".format(
-                mask.size(1), weight_d * weight_h * weight_w))
-
-    return torch.ops.tvdcn.deform_conv_transpose3d(
-        input,
-        weight,
-        offset,
-        mask,
-        bias,
-        stride_d, stride_h, stride_w,
-        pad_d, pad_h, pad_w,
-        out_pad_d, out_pad_h, out_pad_w,
-        dil_d, dil_h, dil_w,
-        groups,
-        offset_groups,
-        mask_groups,
-        deformable,
-        modulated)
+    return torch.ops.tvdcn.deform_conv_transpose3d(input, weight, offset, mask, bias,
+                                                   stride, padding, output_padding, dilation, groups)
 
 
 ################################################################################
 # Modules
 ################################################################################
 # noinspection PyMethodOverriding
 class _DeformConvTransposeNd(_DeformConvNd):
```

### Comparing `tvdcn-0.2.7/tvdcn/utils.py` & `tvdcn-0.3.0/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.7/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.3.0/tvdcn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.7
+Version: 0.3.0
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.2.7/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.3.0/tvdcn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

