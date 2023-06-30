# Comparing `tmp/nobuco-0.5.4.tar.gz` & `tmp/nobuco-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.5.4.tar", last modified: Tue Jun 20 17:25:59 2023, max compression
+gzip compressed data, was "nobuco-0.5.5.tar", last modified: Fri Jun 30 19:09:26 2023, max compression
```

## Comparing `nobuco-0.5.4.tar` & `nobuco-0.5.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.123032 nobuco-0.5.4/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.4/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    24637 2023-06-20 17:25:59.123032 nobuco-0.5.4/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    22803 2023-06-20 17:23:27.000000 nobuco-0.5.4/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-19 19:46:46.000000 nobuco-0.5.4/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.4/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.4/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-06-19 20:43:10.000000 nobuco-0.5.4/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.4/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.4/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.4/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.119032 nobuco-0.5.4/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.4/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-19 11:09:59.000000 nobuco-0.5.4/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-19 13:20:31.000000 nobuco-0.5.4/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.4/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.4/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.4/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-06-20 11:58:19.000000 nobuco-0.5.4/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-19 13:27:23.000000 nobuco-0.5.4/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14354 2023-06-20 11:35:42.000000 nobuco-0.5.4/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.4/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-06-20 12:20:54.000000 nobuco-0.5.4/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.4/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-06-19 21:15:29.000000 nobuco-0.5.4/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-06-19 13:43:03.000000 nobuco-0.5.4/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.4/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6449 2023-06-20 11:32:28.000000 nobuco-0.5.4/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11315 2023-06-20 11:52:34.000000 nobuco-0.5.4/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.4/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-19 20:13:01.000000 nobuco-0.5.4/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.123032 nobuco-0.5.4/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.4/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.4/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.123032 nobuco-0.5.4/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    24637 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-20 17:20:57.000000 nobuco-0.5.4/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-20 17:25:59.123032 nobuco-0.5.4/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.176802 nobuco-0.5.5/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.5/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24625 2023-06-30 19:09:26.176802 nobuco-0.5.5/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22791 2023-06-30 19:07:43.000000 nobuco-0.5.5/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.168802 nobuco-0.5.5/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-06-23 09:29:01.000000 nobuco-0.5.5/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-30 18:23:08.000000 nobuco-0.5.5/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.5/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-06-30 18:23:14.000000 nobuco-0.5.5/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.5/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.5/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.176802 nobuco-0.5.5/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14354 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9135 2023-06-30 18:40:38.000000 nobuco-0.5.5/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6449 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11315 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.176802 nobuco-0.5.5/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.176802 nobuco-0.5.5/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24625 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-30 18:54:51.000000 nobuco-0.5.5/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-30 19:09:26.176802 nobuco-0.5.5/setup.cfg
```

### Comparing `nobuco-0.5.4/LICENSE` & `nobuco-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/PKG-INFO` & `nobuco-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.4
+Version: 0.5.5
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -576,37 +576,31 @@
 | Arm CPU           | 4.6 ms     | **2.9** ms | 0.6x    |
 | Arm CPU (XNNPACK) | **2.1** ms | FAIL       | —       |
 | Arm GPU (OpenCL)  | 21.8 ms    | FAIL       | —       |
 
 Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
 Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
 No transpose ops were added this time, so who's to blame?
-It suffices to see what `torch.trace` gives us:
+It suffices to see what `torch.onnx.export` gives us:
 
-<table>
-<tr>
-<th>slice_relu.onnx</th>
-</tr>
-<tr>
-<td>
-<img src="docs/slice_relu_onnx.png" width="100%">
-</td>
-</tr>
-</table>
+<p align="center">
+  <img src="docs/slice_relu_onnx.png" width="100%">
+  <b>slice_relu.onnx</b>
+</p>
 
 `onnx_tf` does a fair job optimizing the graph it's given,
 but combining consecutive `slice` ops seems to be too much to ask.
-It also leaves out garbage nodes sometimes (see free-floating `While` in this example).
+It also leaves out garbage nodes sometimes (note the free-floating `While` in this example).
 
 Nobuco evades these types of problems by simply not dealing with `onnx`.
 
-<table>
+<table align="center">
   <tr>
-    <th>slice_relu_nobuco.tflite</th>
-    <th>slice_relu_onnxtf.tflite</th>
+    <th>slice_relu_nobuco</th>
+    <th>slice_relu_onnxtf</th>
   </tr>
   <tr>
     <td>
       <p align="center">
         <img src="docs/slice_relu_nobuco.png" width="60%">
       </p>
     </td>
```

### Comparing `nobuco-0.5.4/README.md` & `nobuco-0.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -540,37 +540,31 @@
 | Arm CPU           | 4.6 ms     | **2.9** ms | 0.6x    |
 | Arm CPU (XNNPACK) | **2.1** ms | FAIL       | —       |
 | Arm GPU (OpenCL)  | 21.8 ms    | FAIL       | —       |
 
 Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
 Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
 No transpose ops were added this time, so who's to blame?
-It suffices to see what `torch.trace` gives us:
+It suffices to see what `torch.onnx.export` gives us:
 
-<table>
-<tr>
-<th>slice_relu.onnx</th>
-</tr>
-<tr>
-<td>
-<img src="docs/slice_relu_onnx.png" width="100%">
-</td>
-</tr>
-</table>
+<p align="center">
+  <img src="docs/slice_relu_onnx.png" width="100%">
+  <b>slice_relu.onnx</b>
+</p>
 
 `onnx_tf` does a fair job optimizing the graph it's given,
 but combining consecutive `slice` ops seems to be too much to ask.
-It also leaves out garbage nodes sometimes (see free-floating `While` in this example).
+It also leaves out garbage nodes sometimes (note the free-floating `While` in this example).
 
 Nobuco evades these types of problems by simply not dealing with `onnx`.
 
-<table>
+<table align="center">
   <tr>
-    <th>slice_relu_nobuco.tflite</th>
-    <th>slice_relu_onnxtf.tflite</th>
+    <th>slice_relu_nobuco</th>
+    <th>slice_relu_onnxtf</th>
   </tr>
   <tr>
     <td>
       <p align="center">
         <img src="docs/slice_relu_nobuco.png" width="60%">
       </p>
     </td>
```

### Comparing `nobuco-0.5.4/nobuco/__init__.py` & `nobuco-0.5.5/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/commons.py` & `nobuco-0.5.5/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/convert.py` & `nobuco-0.5.5/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/converters/channel_ordering.py` & `nobuco-0.5.5/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/converters/node_converter.py` & `nobuco-0.5.5/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/converters/tensor.py` & `nobuco-0.5.5/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/converters/type_cast.py` & `nobuco-0.5.5/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/converters/validation.py` & `nobuco-0.5.5/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/entity/keras.py` & `nobuco-0.5.5/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/entity/pytorch.py` & `nobuco-0.5.5/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/funcs.py` & `nobuco-0.5.5/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/layers/channel_order.py` & `nobuco-0.5.5/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/layers/container.py` & `nobuco-0.5.5/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/layers/weight.py` & `nobuco-0.5.5/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/locate/link.py` & `nobuco-0.5.5/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/locate/locate.py` & `nobuco-0.5.5/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/activation.py` & `nobuco-0.5.5/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/attention.py` & `nobuco-0.5.5/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/boolean.py` & `nobuco-0.5.5/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/boolean_mask.py` & `nobuco-0.5.5/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/comparison.py` & `nobuco-0.5.5/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/convolution.py` & `nobuco-0.5.5/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/dropout.py` & `nobuco-0.5.5/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/interpolation.py` & `nobuco-0.5.5/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/linear.py` & `nobuco-0.5.5/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/math.py` & `nobuco-0.5.5/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/misc.py` & `nobuco-0.5.5/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/normalization.py` & `nobuco-0.5.5/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/padding.py` & `nobuco-0.5.5/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/pooling.py` & `nobuco-0.5.5/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/recurrent.py` & `nobuco-0.5.5/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/slice.py` & `nobuco-0.5.5/nobuco/node_converters/slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     shape = tensors[0].shape
     for tens in tensors:
         shape = tf.broadcast_dynamic_shape(shape, tens.shape)
     tensors = [tf.broadcast_to(t, shape) for t in tensors]
     return tensors
 
 
-def slice_assign(sliced_tensor, slice_args, assigned_tensor, is_scatter=False):
+def slice_assign(sliced_tensor, slice_args, assigned_tensor):
     slice_args = _ensure_iterable(slice_args)
     """Assign a tensor to the slice of another tensor.
     No broadcast is performed.
     Args:
         - sliced_tensor (tf.Tensor): the tensor whose slice you want changed.
         - assigned_tensor (tf.Tensor): the tensor which you want assigned.
         - *slice_args (str or slice): the slices arguments. Can be ':', '...'
@@ -111,36 +111,25 @@
         sliced_shape = [tf.size(r) for r in corresponding_ranges] + left_out_shape
     elif n_indexed_dims == len(corresponding_ranges):
         mesh_ranges = broadcast(corresponding_ranges)
         sliced_shape = [tf.size(mesh_ranges[0])] + left_out_shape
     else:
         raise Exception('This slice configuration is currently not supported')
 
-    update_indices = tf.stack([
-        tf.reshape(slicing_range, (-1,))
-        for slicing_range in mesh_ranges
-    ], axis=-1)
-
     if isinstance(assigned_tensor, TF_TENSOR_CLASSES) and len(assigned_tensor.shape) == len(scatted_nd_perm):
         assigned_tensor = tf.transpose(assigned_tensor, scatted_nd_perm)
 
-    if is_scatter:
-        assigned_tensor_reshaped = assigned_tensor
-    else:
-        assigned_tensor_reshaped = to_shape_and_dtype(assigned_tensor, sliced_shape, sliced_tensor.dtype)
-        assigned_tensor_reshaped = tf.reshape(assigned_tensor_reshaped, [-1] + left_out_shape)
-
-    # NOTE: the tensors are reshaped to allow for easier indexing with
-    sliced_tensor_reshaped = tf.transpose(sliced_tensor, perm=scatted_nd_perm)
+    assigned_tensor = to_shape_and_dtype(assigned_tensor, sliced_shape, sliced_tensor.dtype)
+    sliced_tensor = tf.transpose(sliced_tensor, perm=scatted_nd_perm)
+    update_indices = tf.stack(mesh_ranges, axis=-1)
 
-    # finalisation
     sliced_tensor_reshaped = tf.tensor_scatter_nd_update(
-        tensor=sliced_tensor_reshaped,
+        tensor=sliced_tensor,
         indices=update_indices,
-        updates=assigned_tensor_reshaped,
+        updates=assigned_tensor,
     )
     sliced_tensor_updated = tf.transpose(sliced_tensor_reshaped, perm=inverse_scatter_nd_perm)
     return sliced_tensor_updated
 
 
 def slice_assign_boolean_mask_scatter(sliced_tensor, slice_args, assigned_tensor):
     update_indices = tf.where(slice_args)
```

### Comparing `nobuco-0.5.4/nobuco/node_converters/tensor_cast.py` & `nobuco-0.5.5/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/tensor_creation.py` & `nobuco-0.5.5/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.5.5/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/trace/tensor_storage.py` & `nobuco-0.5.5/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/trace/trace.py` & `nobuco-0.5.5/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/util.py` & `nobuco-0.5.5/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/vis/console_stylizer.py` & `nobuco-0.5.5/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco/vis/html_stylizer.py` & `nobuco-0.5.5/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/nobuco.egg-info/PKG-INFO` & `nobuco-0.5.5/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.4
+Version: 0.5.5
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -576,37 +576,31 @@
 | Arm CPU           | 4.6 ms     | **2.9** ms | 0.6x    |
 | Arm CPU (XNNPACK) | **2.1** ms | FAIL       | —       |
 | Arm GPU (OpenCL)  | 21.8 ms    | FAIL       | —       |
 
 Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
 Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
 No transpose ops were added this time, so who's to blame?
-It suffices to see what `torch.trace` gives us:
+It suffices to see what `torch.onnx.export` gives us:
 
-<table>
-<tr>
-<th>slice_relu.onnx</th>
-</tr>
-<tr>
-<td>
-<img src="docs/slice_relu_onnx.png" width="100%">
-</td>
-</tr>
-</table>
+<p align="center">
+  <img src="docs/slice_relu_onnx.png" width="100%">
+  <b>slice_relu.onnx</b>
+</p>
 
 `onnx_tf` does a fair job optimizing the graph it's given,
 but combining consecutive `slice` ops seems to be too much to ask.
-It also leaves out garbage nodes sometimes (see free-floating `While` in this example).
+It also leaves out garbage nodes sometimes (note the free-floating `While` in this example).
 
 Nobuco evades these types of problems by simply not dealing with `onnx`.
 
-<table>
+<table align="center">
   <tr>
-    <th>slice_relu_nobuco.tflite</th>
-    <th>slice_relu_onnxtf.tflite</th>
+    <th>slice_relu_nobuco</th>
+    <th>slice_relu_onnxtf</th>
   </tr>
   <tr>
     <td>
       <p align="center">
         <img src="docs/slice_relu_nobuco.png" width="60%">
       </p>
     </td>
```

### Comparing `nobuco-0.5.4/nobuco.egg-info/SOURCES.txt` & `nobuco-0.5.5/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.4/pyproject.toml` & `nobuco-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.5.4"
+version = "0.5.5"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

