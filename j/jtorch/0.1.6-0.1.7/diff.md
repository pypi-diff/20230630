# Comparing `tmp/jtorch-0.1.6.tar.gz` & `tmp/jtorch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtorch-0.1.6.tar", last modified: Sun Jun 25 15:05:25 2023, max compression
+gzip compressed data, was "jtorch-0.1.7.tar", last modified: Fri Jun 30 15:33:37 2023, max compression
```

## Comparing `jtorch-0.1.6.tar` & `jtorch-0.1.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11621 2023-03-19 10:14:44.000000 jtorch-0.1.6/LICENSE.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       88 2023-03-19 10:14:44.000000 jtorch-0.1.6/MANIFEST.in
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4635 2023-06-25 15:05:25.681466 jtorch-0.1.6/PKG-INFO
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4182 2023-03-19 10:14:44.000000 jtorch-0.1.6/README.md
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7823 2023-06-18 12:36:10.000000 jtorch-0.1.6/python/jtorch/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4045 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/autograd.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1044 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/compiler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      667 2023-06-06 14:38:33.000000 jtorch-0.1.6/python/jtorch/cuda.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      550 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/distributed.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      253 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/misc.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/nn/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1472 2023-05-12 10:49:11.000000 jtorch-0.1.6/python/jtorch/nn/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      209 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/nn/init.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/nn/utils/
--rw-r--r--   0 cjld      (1000) cjld      (1000)        0 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/nn/utils/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       21 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/nn/utils/rnn.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      979 2023-06-04 13:28:13.000000 jtorch-0.1.6/python/jtorch/optim.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/src/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2426 2023-04-03 01:50:53.000000 jtorch-0.1.6/python/jtorch/src/jtorch_core.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      899 2023-05-13 04:25:41.000000 jtorch-0.1.6/python/jtorch/src/jtorch_core.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/test/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      547 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/test/test_conflict_func.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1522 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/test/test_function.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      676 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/test/test_misc.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2662 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/test/test_tutorial.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/tutorial/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1324 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad1.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2381 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad2.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3122 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad3.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2862 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad4.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1866 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad5_optim.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1963 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad6_module.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2507 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/auto_grad7_dynet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3040 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/tutorial/quickstart.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/utils/
--rw-r--r--   0 cjld      (1000) cjld      (1000)       84 2023-04-01 23:25:04.000000 jtorch-0.1.6/python/jtorch/utils/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       22 2023-03-29 22:23:26.000000 jtorch-0.1.6/python/jtorch/utils/checkpoint.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2386 2023-04-01 23:25:04.000000 jtorch-0.1.6/python/jtorch/utils/data.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      330 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/utils/dtype.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      772 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/utils/pip_publish.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/vision/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1475 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/_internally_replaced_utils.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch/vision/datasets/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      160 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/datasets/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    21973 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/datasets/mnist.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    19124 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/datasets/utils.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4134 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/datasets/vision.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       30 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/transforms.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    23314 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/jtorch/vision/utils.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/jtorch.egg-info/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4635 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/PKG-INFO
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1528 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/SOURCES.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)        1 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/dependency_links.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       25 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/requires.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       13 2023-06-25 15:05:25.000000 jtorch-0.1.6/python/jtorch.egg-info/top_level.txt
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-25 15:05:25.681466 jtorch-0.1.6/python/torch/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1858 2023-04-01 23:25:04.000000 jtorch-0.1.6/python/torch/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       29 2023-03-19 10:14:44.000000 jtorch-0.1.6/python/torch/autograd.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       38 2023-06-25 15:05:25.681466 jtorch-0.1.6/setup.cfg
--rw-r--r--   0 cjld      (1000) cjld      (1000)      885 2023-06-25 15:00:37.000000 jtorch-0.1.6/setup.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.477511 jtorch-0.1.7/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11621 2023-03-19 10:14:44.000000 jtorch-0.1.7/LICENSE.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       88 2023-03-19 10:14:44.000000 jtorch-0.1.7/MANIFEST.in
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4635 2023-06-30 15:33:37.477511 jtorch-0.1.7/PKG-INFO
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4182 2023-03-19 10:14:44.000000 jtorch-0.1.7/README.md
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.466678 jtorch-0.1.7/python/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.466678 jtorch-0.1.7/python/jtorch/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7876 2023-06-30 15:27:45.000000 jtorch-0.1.7/python/jtorch/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4045 2023-03-29 22:23:26.000000 jtorch-0.1.7/python/jtorch/autograd.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1044 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/compiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      667 2023-06-06 14:38:33.000000 jtorch-0.1.7/python/jtorch/cuda.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      550 2023-03-29 22:23:26.000000 jtorch-0.1.7/python/jtorch/distributed.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      253 2023-03-29 22:23:26.000000 jtorch-0.1.7/python/jtorch/misc.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.466678 jtorch-0.1.7/python/jtorch/nn/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1472 2023-05-12 10:49:11.000000 jtorch-0.1.7/python/jtorch/nn/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      209 2023-03-29 22:23:26.000000 jtorch-0.1.7/python/jtorch/nn/init.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.466678 jtorch-0.1.7/python/jtorch/nn/utils/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)        0 2023-03-29 22:23:26.000000 jtorch-0.1.7/python/jtorch/nn/utils/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       21 2023-03-29 22:23:26.000000 jtorch-0.1.7/python/jtorch/nn/utils/rnn.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      979 2023-06-04 13:28:13.000000 jtorch-0.1.7/python/jtorch/optim.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.466678 jtorch-0.1.7/python/jtorch/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2426 2023-04-03 01:50:53.000000 jtorch-0.1.7/python/jtorch/src/jtorch_core.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      899 2023-05-13 04:25:41.000000 jtorch-0.1.7/python/jtorch/src/jtorch_core.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.466678 jtorch-0.1.7/python/jtorch/test/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      547 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/test/test_conflict_func.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1522 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/test/test_function.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      676 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/test/test_misc.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2662 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/test/test_tutorial.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.466678 jtorch-0.1.7/python/jtorch/tutorial/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1324 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/tutorial/auto_grad1.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2381 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/tutorial/auto_grad2.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3122 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/tutorial/auto_grad3.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2862 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/tutorial/auto_grad4.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1866 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/tutorial/auto_grad5_optim.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1963 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/tutorial/auto_grad6_module.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2507 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/tutorial/auto_grad7_dynet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3040 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/tutorial/quickstart.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.477511 jtorch-0.1.7/python/jtorch/utils/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       84 2023-04-01 23:25:04.000000 jtorch-0.1.7/python/jtorch/utils/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       22 2023-03-29 22:23:26.000000 jtorch-0.1.7/python/jtorch/utils/checkpoint.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2386 2023-04-01 23:25:04.000000 jtorch-0.1.7/python/jtorch/utils/data.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      330 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/utils/dtype.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      772 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/utils/pip_publish.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.477511 jtorch-0.1.7/python/jtorch/vision/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1475 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/vision/_internally_replaced_utils.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.477511 jtorch-0.1.7/python/jtorch/vision/datasets/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      160 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/vision/datasets/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    21973 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/vision/datasets/mnist.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    19124 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/vision/datasets/utils.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4134 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/vision/datasets/vision.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       30 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/vision/transforms.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    23314 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/jtorch/vision/utils.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.466678 jtorch-0.1.7/python/jtorch.egg-info/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4635 2023-06-30 15:33:37.000000 jtorch-0.1.7/python/jtorch.egg-info/PKG-INFO
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1528 2023-06-30 15:33:37.000000 jtorch-0.1.7/python/jtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)        1 2023-06-30 15:33:37.000000 jtorch-0.1.7/python/jtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       25 2023-06-30 15:33:37.000000 jtorch-0.1.7/python/jtorch.egg-info/requires.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       13 2023-06-30 15:33:37.000000 jtorch-0.1.7/python/jtorch.egg-info/top_level.txt
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:37.477511 jtorch-0.1.7/python/torch/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1858 2023-04-01 23:25:04.000000 jtorch-0.1.7/python/torch/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       29 2023-03-19 10:14:44.000000 jtorch-0.1.7/python/torch/autograd.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       38 2023-06-30 15:33:37.477511 jtorch-0.1.7/setup.cfg
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      885 2023-06-30 15:30:22.000000 jtorch-0.1.7/setup.py
```

### Comparing `jtorch-0.1.6/LICENSE.txt` & `jtorch-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/PKG-INFO` & `jtorch-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtorch
-Version: 0.1.6
+Version: 0.1.7
 Summary: jtorch project
 Home-page: https://github.com/JITTorch/jtorch
 Author: jtorch
 Author-email: jtorch@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/JITTorch/jtorch/issues
 Platform: UNKNOWN
```

### Comparing `jtorch-0.1.6/README.md` & `jtorch-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/__init__.py` & `jtorch-0.1.7/python/jtorch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,19 @@
         if not has_dtype and "dtype" in kw:
             dtype = kw["dtype"]
             del kw["dtype"]
         if "device" in kw:
             del kw["device"]
         args, kw = handle_dtype(args, kw, dtype)
         ret = func(*args, **kw)
-        if requires_grad is not None:
-            ret.requires_grad = requires_grad
-        if dtype is not None:
-            ret.astype(dtype)
+        if isinstance(ret, jt.Var):
+            if requires_grad is not None:
+                ret.requires_grad = requires_grad
+            if dtype is not None:
+                ret.astype(dtype)
         return ret
     return inner
         
 
 import inspect
 _wrapper_keys = set(["shape", "start", "size"])
 _wrapper_keys.add("x")
```

### Comparing `jtorch-0.1.6/python/jtorch/autograd.py` & `jtorch-0.1.7/python/jtorch/autograd.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/compiler.py` & `jtorch-0.1.7/python/jtorch/compiler.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/cuda.py` & `jtorch-0.1.7/python/jtorch/cuda.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/distributed.py` & `jtorch-0.1.7/python/jtorch/distributed.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/nn/__init__.py` & `jtorch-0.1.7/python/jtorch/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/optim.py` & `jtorch-0.1.7/python/jtorch/optim.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/src/jtorch_core.cc` & `jtorch-0.1.7/python/jtorch/src/jtorch_core.cc`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/src/jtorch_core.h` & `jtorch-0.1.7/python/jtorch/src/jtorch_core.h`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/test/test_conflict_func.py` & `jtorch-0.1.7/python/jtorch/test/test_conflict_func.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/test/test_function.py` & `jtorch-0.1.7/python/jtorch/test/test_function.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/test/test_misc.py` & `jtorch-0.1.7/python/jtorch/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/test/test_tutorial.py` & `jtorch-0.1.7/python/jtorch/test/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/tutorial/auto_grad1.py` & `jtorch-0.1.7/python/jtorch/tutorial/auto_grad1.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/tutorial/auto_grad2.py` & `jtorch-0.1.7/python/jtorch/tutorial/auto_grad2.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/tutorial/auto_grad3.py` & `jtorch-0.1.7/python/jtorch/tutorial/auto_grad3.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/tutorial/auto_grad4.py` & `jtorch-0.1.7/python/jtorch/tutorial/auto_grad4.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/tutorial/auto_grad5_optim.py` & `jtorch-0.1.7/python/jtorch/tutorial/auto_grad5_optim.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/tutorial/auto_grad6_module.py` & `jtorch-0.1.7/python/jtorch/tutorial/auto_grad6_module.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/tutorial/auto_grad7_dynet.py` & `jtorch-0.1.7/python/jtorch/tutorial/auto_grad7_dynet.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/tutorial/quickstart.py` & `jtorch-0.1.7/python/jtorch/tutorial/quickstart.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/utils/data.py` & `jtorch-0.1.7/python/jtorch/utils/data.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/utils/pip_publish.py` & `jtorch-0.1.7/python/jtorch/utils/pip_publish.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/vision/_internally_replaced_utils.py` & `jtorch-0.1.7/python/jtorch/vision/_internally_replaced_utils.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/vision/datasets/mnist.py` & `jtorch-0.1.7/python/jtorch/vision/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/vision/datasets/utils.py` & `jtorch-0.1.7/python/jtorch/vision/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/vision/datasets/vision.py` & `jtorch-0.1.7/python/jtorch/vision/datasets/vision.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch/vision/utils.py` & `jtorch-0.1.7/python/jtorch/vision/utils.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/jtorch.egg-info/PKG-INFO` & `jtorch-0.1.7/python/jtorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtorch
-Version: 0.1.6
+Version: 0.1.7
 Summary: jtorch project
 Home-page: https://github.com/JITTorch/jtorch
 Author: jtorch
 Author-email: jtorch@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/JITTorch/jtorch/issues
 Platform: UNKNOWN
```

### Comparing `jtorch-0.1.6/python/jtorch.egg-info/SOURCES.txt` & `jtorch-0.1.7/python/jtorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/python/torch/__init__.py` & `jtorch-0.1.7/python/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `jtorch-0.1.6/setup.py` & `jtorch-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jtorch",
-    version="0.1.6",
+    version="0.1.7",
     author="jtorch",
     author_email="jtorch@qq.com",
     description="jtorch project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JITTorch/jtorch",
     project_urls={
```

