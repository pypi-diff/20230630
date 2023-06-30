# Comparing `tmp/EasyDeL-0.0.6.tar.gz` & `tmp/EasyDeL-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyDeL-0.0.6.tar", last modified: Wed Jun 28 13:19:05 2023, max compression
+gzip compressed data, was "EasyDeL-0.0.7.tar", last modified: Fri Jun 30 18:02:36 2023, max compression
```

## Comparing `EasyDeL-0.0.6.tar` & `EasyDeL-0.0.7.tar`

### file list

```diff
@@ -1,56 +1,62 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDeL.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6280 2023-06-28 13:19:05.000000 EasyDeL-0.0.6/EasyDeL.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1256 2023-06-28 13:19:05.000000 EasyDeL-0.0.6/EasyDeL.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-28 13:19:05.000000 EasyDeL-0.0.6/EasyDeL.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-06-28 13:19:05.000000 EasyDeL-0.0.6/EasyDeL.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-28 13:19:05.000000 EasyDeL-0.0.6/EasyDeL.egg-info/top_level.txt
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1502 2023-06-27 07:17:54.000000 EasyDeL-0.0.6/EasyDel/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/configs/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       78 2023-06-28 13:18:01.000000 EasyDeL-0.0.6/EasyDel/configs/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5646 2023-06-28 13:11:11.000000 EasyDeL-0.0.6/EasyDel/configs/configs.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/modules/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1041 2023-06-24 06:51:39.000000 EasyDeL-0.0.6/EasyDel/modules/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/modules/falcon/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       88 2023-06-15 10:29:08.000000 EasyDeL-0.0.6/EasyDel/modules/falcon/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    19533 2023-06-28 07:51:37.000000 EasyDeL-0.0.6/EasyDel/modules/falcon/modelling_falcon_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/modules/gpt_j/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      130 2023-06-13 13:41:25.000000 EasyDeL-0.0.6/EasyDel/modules/gpt_j/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    31319 2023-06-13 13:41:25.000000 EasyDeL-0.0.6/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/modules/gpt_neo_x/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       94 2023-06-24 06:51:39.000000 EasyDeL-0.0.6/EasyDel/modules/gpt_neo_x/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    16080 2023-06-24 06:51:39.000000 EasyDeL-0.0.6/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/modules/llama/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      150 2023-06-15 07:43:43.000000 EasyDeL-0.0.6/EasyDel/modules/llama/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    34041 2023-06-27 08:27:15.000000 EasyDeL-0.0.6/EasyDel/modules/llama/modelling_llama_flax.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17266 2023-06-26 09:30:53.000000 EasyDeL-0.0.6/EasyDel/modules/llama/modelling_llama_pytorch.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/modules/lucid_transformer/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       95 2023-06-12 11:40:22.000000 EasyDeL-0.0.6/EasyDel/modules/lucid_transformer/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13472 2023-06-28 07:13:59.000000 EasyDeL-0.0.6/EasyDel/modules/lucid_transformer/modelling_lt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/modules/mosaic_mpt/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-15 07:43:43.000000 EasyDeL-0.0.6/EasyDel/modules/mosaic_mpt/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17799 2023-06-25 09:09:59.000000 EasyDeL-0.0.6/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/serve/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-17 08:13:44.000000 EasyDeL-0.0.6/EasyDel/serve/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1482 2023-06-17 08:09:33.000000 EasyDeL-0.0.6/EasyDel/serve/serve_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/trainer/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      146 2023-06-27 07:17:54.000000 EasyDeL-0.0.6/EasyDel/trainer/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8996 2023-06-26 10:53:42.000000 EasyDeL-0.0.6/EasyDel/trainer/config.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    21478 2023-06-28 13:18:01.000000 EasyDeL-0.0.6/EasyDel/trainer/fsdp_train.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      402 2023-06-11 11:51:31.000000 EasyDeL-0.0.6/EasyDel/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2023-06-11 11:51:31.000000 EasyDeL-0.0.6/EasyDel/utils/checker.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4584 2023-06-26 09:09:30.000000 EasyDeL-0.0.6/EasyDel/utils/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/EasyDel/weight_convertor/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-06-17 06:47:56.000000 EasyDeL-0.0.6/EasyDel/weight_convertor/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6215 2023-06-18 09:17:09.000000 EasyDeL-0.0.6/EasyDel/weight_convertor/falcon.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5077 2023-06-24 06:51:39.000000 EasyDeL-0.0.6/EasyDel/weight_convertor/llama.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9833 2023-06-17 12:12:31.000000 EasyDeL-0.0.6/EasyDel/weight_convertor/mpt.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      858 2023-06-17 10:41:48.000000 EasyDeL-0.0.6/EasyDel/weight_convertor/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-11 11:51:31.000000 EasyDeL-0.0.6/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6280 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5386 2023-06-28 07:19:22.000000 EasyDeL-0.0.6/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      608 2023-06-24 06:51:39.000000 EasyDeL-0.0.6/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-28 13:19:05.304205 EasyDeL-0.0.6/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2023-06-28 13:18:01.000000 EasyDeL-0.0.6/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDeL.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1404 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-30 18:02:35.000000 EasyDeL-0.0.7/EasyDeL.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1712 2023-06-30 08:03:06.000000 EasyDeL-0.0.7/EasyDel/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/configs/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       78 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/configs/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5646 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/configs/configs.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1284 2023-06-30 08:03:06.000000 EasyDeL-0.0.7/EasyDel/modules/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/falcon/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       88 2023-06-15 12:27:13.000000 EasyDeL-0.0.7/EasyDel/modules/falcon/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    19533 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/modules/falcon/modelling_falcon_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/gpt_j/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      130 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/modules/gpt_j/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    31319 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/gpt_neo_x/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       94 2023-06-23 11:08:05.000000 EasyDeL-0.0.7/EasyDel/modules/gpt_neo_x/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    16080 2023-06-23 11:13:00.000000 EasyDeL-0.0.7/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/llama/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      150 2023-06-14 16:42:09.000000 EasyDeL-0.0.7/EasyDel/modules/llama/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    34041 2023-06-27 16:24:48.000000 EasyDeL-0.0.7/EasyDel/modules/llama/modelling_llama_flax.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17266 2023-06-26 16:41:56.000000 EasyDeL-0.0.7/EasyDel/modules/llama/modelling_llama_pytorch.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/lucid_transformer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       95 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/modules/lucid_transformer/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13472 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/modules/lucid_transformer/modelling_lt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/mosaic_mpt/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-14 16:34:35.000000 EasyDeL-0.0.7/EasyDel/modules/mosaic_mpt/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17799 2023-06-22 04:42:44.000000 EasyDeL-0.0.7/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/palm/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-30 08:01:08.000000 EasyDeL-0.0.7/EasyDel/modules/palm/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    16353 2023-06-30 07:08:03.000000 EasyDeL-0.0.7/EasyDel/modules/palm/modelling_palm_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/modules/t5/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       75 2023-06-30 08:01:08.000000 EasyDeL-0.0.7/EasyDel/modules/t5/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    59589 2023-06-30 07:56:15.000000 EasyDeL-0.0.7/EasyDel/modules/t5/modelling_t5_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.051000 EasyDeL-0.0.7/EasyDel/serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1482 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/serve/serve_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/EasyDel/trainer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      146 2023-06-26 17:06:26.000000 EasyDeL-0.0.7/EasyDel/trainer/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8944 2023-06-29 08:35:15.000000 EasyDeL-0.0.7/EasyDel/trainer/config.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    21478 2023-06-29 05:59:18.000000 EasyDeL-0.0.7/EasyDel/trainer/fsdp_train.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/EasyDel/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      402 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/EasyDel/utils/checker.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4584 2023-06-26 16:41:56.000000 EasyDeL-0.0.7/EasyDel/utils/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/EasyDel/weight_convertor/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-06-15 13:20:11.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6215 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/falcon.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5077 2023-06-22 11:28:16.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/llama.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9833 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/mpt.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      858 2023-06-18 16:37:39.000000 EasyDeL-0.0.7/EasyDel/weight_convertor/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-14 16:25:08.000000 EasyDeL-0.0.7/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5471 2023-06-30 07:58:59.000000 EasyDeL-0.0.7/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      608 2023-06-23 10:45:58.000000 EasyDeL-0.0.7/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-30 18:02:36.055000 EasyDeL-0.0.7/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2023-06-30 08:08:21.000000 EasyDeL-0.0.7/setup.py
```

### Comparing `EasyDeL-0.0.6/EasyDeL.egg-info/PKG-INFO` & `EasyDeL-0.0.7/EasyDeL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDeL
-Version: 0.0.6
+Version: 0.0.7
 Summary: An open-source library to make training faster and more optimized in Jax/Flax
 Home-page: https://github.com/erfanzar/EasyDeL
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
@@ -37,16 +37,18 @@
 
 ## Available Models Are
 
 - Llama     (Support `FSDP`, `MP`,` DP`)
 - GPT-J     (Support `FSDP`, `MP`,` DP`)
 - LT        (Support `FSDP`, `MP`, `DP`)
 - MosaicMPT (Support `FSDP`, `MP`,` DP`)
-- GPTNeoX   (TODO `FSDP`, `MP`, `DP`)
+- GPTNeoX   (Support `FSDP`, `MP`, `DP`)
 - Falcon    (Support `FSDP`, `MP`, `DP`)
+- Palm      (Support `FSDP`, `MP`, `DP`)
+- T5        (Support `FSDP`, `MP`, `DP`)
 
 you can also tell me the model you want in Flax/Jax version and ill try my best to build it ;)
 
 ## FineTuning
 
 with using EasyDel FineTuning LLM (CausalLanguageModels) are easy as much as possible with using Jax and Flax
 and having the benefit of TPUs for the best speed here's a simple code to use in order to finetune your own MPT / LLama
```

### Comparing `EasyDeL-0.0.6/EasyDeL.egg-info/SOURCES.txt` & `EasyDeL-0.0.7/EasyDeL.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 EasyDel/modules/llama/__init__.py
 EasyDel/modules/llama/modelling_llama_flax.py
 EasyDel/modules/llama/modelling_llama_pytorch.py
 EasyDel/modules/lucid_transformer/__init__.py
 EasyDel/modules/lucid_transformer/modelling_lt_flax.py
 EasyDel/modules/mosaic_mpt/__init__.py
 EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
+EasyDel/modules/palm/__init__.py
+EasyDel/modules/palm/modelling_palm_flax.py
+EasyDel/modules/t5/__init__.py
+EasyDel/modules/t5/modelling_t5_flax.py
 EasyDel/serve/__init__.py
 EasyDel/serve/serve_utils.py
 EasyDel/trainer/__init__.py
 EasyDel/trainer/config.py
 EasyDel/trainer/fsdp_train.py
 EasyDel/utils/__init__.py
 EasyDel/utils/checker.py
```

### Comparing `EasyDeL-0.0.6/EasyDel/__init__.py` & `EasyDeL-0.0.7/EasyDel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,22 @@
     from .utils import make_shard_and_gather_fns
 if is_tensorflow_available():
     ...
 if is_flax_available():
     from .modules import FlaxLlamaModel, LlamaConfig, FlaxLlamaForCausalLM, LlamaModel, LlamaForCausalLM, \
         FlaxLTModelModule, FlaxLTConfig, FlaxLTForCausalLM, FlaxLTModel, GPTJConfig, FlaxGPTJModule, \
         FlaxGPTJForCausalLMModule, FlaxGPTJModel, FlaxGPTJForCausalLM, FlaxMptForCausalLM, MptConfig, FlaxMptModel, \
-        FlaxFalconForCausalLM, FlaxFalconModel, FalconConfig, FlaxGPTNeoXForCausalLM, GPTNeoXConfig, FlaxGPTNeoXModel
+        FlaxFalconForCausalLM, FlaxFalconModel, FalconConfig, FlaxGPTNeoXForCausalLM, GPTNeoXConfig, FlaxGPTNeoXModel, \
+        FlaxT5ForConditionalGeneration, FlaxT5Model, FlaxPalmForCausalLM, PalmModel, PalmConfig
 from .trainer import finetuner, TrainArguments, fsdp_train_step
 
 __all__ = __version__, 'package_checker', 'is_jax_available', 'is_torch_available', 'is_flax_available', \
     'is_tensorflow_available', "finetuner", "TrainArguments", "fsdp_train_step", \
     'LlamaConfig', 'LlamaForCausalLM', 'LlamaModel', 'FlaxLlamaForCausalLM', \
     'FlaxLlamaModel', 'FlaxGPTJModule', 'FlaxGPTJForCausalLMModule', \
     'FlaxGPTJModel', 'FlaxGPTJForCausalLM', 'GPTJConfig', \
     'FlaxLTModel', 'FlaxLTConfig', 'FlaxLTModelModule', 'FlaxLTForCausalLM', \
     "FlaxMptForCausalLM", "MptConfig", "FlaxMptModel", \
     "FlaxFalconForCausalLM", "FlaxFalconModel", "FalconConfig", \
-    "FlaxGPTNeoXForCausalLM", "GPTNeoXConfig", "FlaxGPTNeoXModel"
+    "FlaxGPTNeoXForCausalLM", "GPTNeoXConfig", "FlaxGPTNeoXModel", \
+    "FlaxT5ForConditionalGeneration", "FlaxT5Model", \
+    "FlaxPalmForCausalLM", "PalmModel", "PalmConfig"
```

### Comparing `EasyDeL-0.0.6/EasyDel/configs/configs.py` & `EasyDeL-0.0.7/EasyDel/configs/configs.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/modules/__init__.py` & `EasyDeL-0.0.7/EasyDel/modules/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from .llama import LlamaConfig, LlamaModel, LlamaForCausalLM, FlaxLlamaModel, FlaxLlamaForCausalLM
 from .gpt_j import FlaxGPTJModule, FlaxGPTJForCausalLMModule, FlaxGPTJModel, FlaxGPTJForCausalLM, GPTJConfig
 from .lucid_transformer import FlaxLTModel, FlaxLTConfig, FlaxLTModelModule, FlaxLTForCausalLM
 from .mosaic_mpt import MptConfig, FlaxMptModel, FlaxMptForCausalLM
 from .falcon import FalconConfig, FlaxFalconModel, FlaxFalconForCausalLM
 from .gpt_neo_x import FlaxGPTNeoXForCausalLM, GPTNeoXConfig, FlaxGPTNeoXModel
+from .palm import PalmConfig, PalmModel, FlaxPalmForCausalLM
+from .t5 import FlaxT5ForConditionalGeneration, FlaxT5Model
 
 __all__ = ['LlamaConfig', 'LlamaForCausalLM', 'LlamaModel', 'FlaxLlamaForCausalLM', 'FlaxLlamaModel',
            'FlaxGPTJModule', 'FlaxGPTJForCausalLMModule', 'FlaxGPTJModel', 'FlaxGPTJForCausalLM', 'GPTJConfig',
            'FlaxLTModel', 'FlaxLTConfig', 'FlaxLTModelModule', 'FlaxLTForCausalLM',
            "MptConfig", "FlaxMptModel", "FlaxMptForCausalLM",
            "FalconConfig", "FlaxFalconModel", "FlaxFalconForCausalLM",
-           "FlaxGPTNeoXForCausalLM", "GPTNeoXConfig", "FlaxGPTNeoXModel"
+           "FlaxGPTNeoXForCausalLM", "GPTNeoXConfig", "FlaxGPTNeoXModel",
+           "FlaxT5ForConditionalGeneration", "FlaxT5Model",
+           "PalmConfig", "PalmModel", "FlaxPalmForCausalLM"
+
            ]
```

### Comparing `EasyDeL-0.0.6/EasyDel/modules/falcon/modelling_falcon_flax.py` & `EasyDeL-0.0.7/EasyDel/modules/falcon/modelling_falcon_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py` & `EasyDeL-0.0.7/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py` & `EasyDeL-0.0.7/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/modules/llama/modelling_llama_flax.py` & `EasyDeL-0.0.7/EasyDel/modules/llama/modelling_llama_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/modules/llama/modelling_llama_pytorch.py` & `EasyDeL-0.0.7/EasyDel/modules/llama/modelling_llama_pytorch.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/modules/lucid_transformer/modelling_lt_flax.py` & `EasyDeL-0.0.7/EasyDel/modules/lucid_transformer/modelling_lt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py` & `EasyDeL-0.0.7/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/serve/serve_utils.py` & `EasyDeL-0.0.7/EasyDel/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/trainer/config.py` & `EasyDeL-0.0.7/EasyDel/trainer/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,14 @@
                     steps=steps,
                     **self.extra_optimizer_kwargs
                 )
             elif self.scheduler == 'cosine':
                 tx, sc = fjutils.optimizers.get_lion_with_cosine_scheduler(
                     learning_rate=self.learning_rate,
                     steps=steps,
-                    weight_decay=self.weight_decay,
                     **self.extra_optimizer_kwargs
                 )
             elif self.scheduler == 'none':
                 tx, sc = fjutils.optimizers.get_lion_with_linear_scheduler(
                     learning_rate_start=self.learning_rate,
                     learning_rate_end=self.learning_rate,
                     steps=steps,
```

### Comparing `EasyDeL-0.0.6/EasyDel/trainer/fsdp_train.py` & `EasyDeL-0.0.7/EasyDel/trainer/fsdp_train.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/utils/utils.py` & `EasyDeL-0.0.7/EasyDel/utils/utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/weight_convertor/falcon.py` & `EasyDeL-0.0.7/EasyDel/weight_convertor/falcon.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/weight_convertor/llama.py` & `EasyDeL-0.0.7/EasyDel/weight_convertor/llama.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/weight_convertor/mpt.py` & `EasyDeL-0.0.7/EasyDel/weight_convertor/mpt.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/EasyDel/weight_convertor/utils.py` & `EasyDeL-0.0.7/EasyDel/weight_convertor/utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/LICENSE` & `EasyDeL-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/PKG-INFO` & `EasyDeL-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDeL
-Version: 0.0.6
+Version: 0.0.7
 Summary: An open-source library to make training faster and more optimized in Jax/Flax
 Home-page: https://github.com/erfanzar/EasyDeL
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
@@ -37,16 +37,18 @@
 
 ## Available Models Are
 
 - Llama     (Support `FSDP`, `MP`,` DP`)
 - GPT-J     (Support `FSDP`, `MP`,` DP`)
 - LT        (Support `FSDP`, `MP`, `DP`)
 - MosaicMPT (Support `FSDP`, `MP`,` DP`)
-- GPTNeoX   (TODO `FSDP`, `MP`, `DP`)
+- GPTNeoX   (Support `FSDP`, `MP`, `DP`)
 - Falcon    (Support `FSDP`, `MP`, `DP`)
+- Palm      (Support `FSDP`, `MP`, `DP`)
+- T5        (Support `FSDP`, `MP`, `DP`)
 
 you can also tell me the model you want in Flax/Jax version and ill try my best to build it ;)
 
 ## FineTuning
 
 with using EasyDel FineTuning LLM (CausalLanguageModels) are easy as much as possible with using Jax and Flax
 and having the benefit of TPUs for the best speed here's a simple code to use in order to finetune your own MPT / LLama
```

### Comparing `EasyDeL-0.0.6/README.md` & `EasyDeL-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 ## Available Models Are
 
 - Llama     (Support `FSDP`, `MP`,` DP`)
 - GPT-J     (Support `FSDP`, `MP`,` DP`)
 - LT        (Support `FSDP`, `MP`, `DP`)
 - MosaicMPT (Support `FSDP`, `MP`,` DP`)
-- GPTNeoX   (TODO `FSDP`, `MP`, `DP`)
+- GPTNeoX   (Support `FSDP`, `MP`, `DP`)
 - Falcon    (Support `FSDP`, `MP`, `DP`)
+- Palm      (Support `FSDP`, `MP`, `DP`)
+- T5        (Support `FSDP`, `MP`, `DP`)
 
 you can also tell me the model you want in Flax/Jax version and ill try my best to build it ;)
 
 ## FineTuning
 
 with using EasyDel FineTuning LLM (CausalLanguageModels) are easy as much as possible with using Jax and Flax
 and having the benefit of TPUs for the best speed here's a simple code to use in order to finetune your own MPT / LLama
```

### Comparing `EasyDeL-0.0.6/pyproject.toml` & `EasyDeL-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.6/setup.py` & `EasyDeL-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyDeL',
-    version='0.0.6',
+    version='0.0.7',
     author='Erfan Zare Chavoshi',
     author_email='erfanzare82@eyahoo.com',
     description='An open-source library to make training faster and more optimized in Jax/Flax',
     url='https://github.com/erfanzar/EasyDeL',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

