# Comparing `tmp/optimum-intel-1.9.2.tar.gz` & `tmp/optimum-intel-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-intel-1.9.2.tar", last modified: Mon Jun 26 22:28:05 2023, max compression
+gzip compressed data, was "optimum-intel-1.9.3.tar", last modified: Fri Jun 30 16:19:34 2023, max compression
```

## Comparing `optimum-intel-1.9.2.tar` & `optimum-intel-1.9.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.766608 optimum-intel-1.9.2/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.756608 optimum-intel-1.9.2/optimum/commands/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.766608 optimum-intel-1.9.2/optimum/commands/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/commands/neural_compressor/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/commands/neural_compressor/quantize.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.766608 optimum-intel-1.9.2/optimum/commands/register/
--rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/commands/register/register_inc.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.766608 optimum-intel-1.9.2/optimum/intel/
--rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.776608 optimum-intel-1.9.2/optimum/intel/generation/
--rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/generation/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/generation/modeling.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.776608 optimum-intel-1.9.2/optimum/intel/ipex/
--rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/ipex/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/ipex/inference.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.776608 optimum-intel-1.9.2/optimum/intel/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3801 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/launcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/neural_coder_adaptor.py
--rw-r--r--   0 ella      (1000) ella      (1000)    28880 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    39154 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/neural_compressor/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/optimum/intel/openvino/
--rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15434 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18258 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_base_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17577 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_decoder.py
--rw-r--r--   0 ella      (1000) ella      (1000)    28970 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18032 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    14161 2023-06-26 22:24:45.000000 optimum-intel-1.9.2/optimum/intel/openvino/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/openvino/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/optimum/intel/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/constant.py
--rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_ipex_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_neural_compressor_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     9057 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/optimum/intel/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/optimum/intel/utils/modeling_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-26 22:25:58.000000 optimum-intel-1.9.2/optimum/intel/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/optimum_intel.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-26 22:28:04.000000 optimum-intel-1.9.2/optimum_intel.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/entry_points.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-26 22:28:04.000000 optimum-intel-1.9.2/optimum_intel.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)      441 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-26 22:28:05.000000 optimum-intel-1.9.2/optimum_intel.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-06-26 22:24:01.000000 optimum-intel-1.9.2/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-26 22:28:05.786608 optimum-intel-1.9.2/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     2671 2023-06-26 22:25:33.000000 optimum-intel-1.9.2/setup.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.346316 optimum-intel-1.9.3/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.346316 optimum-intel-1.9.3/optimum/commands/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/commands/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/commands/neural_compressor/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/commands/neural_compressor/quantize.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/commands/register/register_inc.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/intel/
+-rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/intel/generation/
+-rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/generation/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/generation/modeling.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/intel/ipex/
+-rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/ipex/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/ipex/inference.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/intel/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3801 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/launcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/neural_coder_adaptor.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    28880 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    39154 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/optimum/intel/openvino/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/openvino/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-06-30 15:23:44.000000 optimum-intel-1.9.3/optimum/intel/openvino/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15386 2023-06-30 15:34:13.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18209 2023-06-30 15:34:13.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_base_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17272 2023-06-30 15:36:28.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    28923 2023-06-30 15:34:13.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18209 2023-06-30 15:36:28.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    14186 2023-06-30 15:38:45.000000 optimum-intel-1.9.3/optimum/intel/openvino/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-06-30 15:23:44.000000 optimum-intel-1.9.3/optimum/intel/openvino/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/openvino/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-06-30 15:23:44.000000 optimum-intel-1.9.3/optimum/intel/openvino/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/optimum/intel/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_ipex_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_neural_compressor_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9057 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/modeling_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-30 15:47:07.000000 optimum-intel-1.9.3/optimum/intel/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/optimum_intel.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-30 15:50:15.000000 optimum-intel-1.9.3/optimum_intel.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)      441 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     2671 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/setup.py
```

### Comparing `optimum-intel-1.9.2/LICENSE` & `optimum-intel-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/MANIFEST.in` & `optimum-intel-1.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/PKG-INFO` & `optimum-intel-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.9.2
+Version: 1.9.3
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.9.2/README.md` & `optimum-intel-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/commands/neural_compressor/base.py` & `optimum-intel-1.9.3/optimum/commands/neural_compressor/base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/commands/neural_compressor/quantize.py` & `optimum-intel-1.9.3/optimum/commands/neural_compressor/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/commands/register/register_inc.py` & `optimum-intel-1.9.3/optimum/commands/register/register_inc.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/__init__.py` & `optimum-intel-1.9.3/optimum/intel/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/generation/__init__.py` & `optimum-intel-1.9.3/optimum/intel/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/generation/modeling.py` & `optimum-intel-1.9.3/optimum/intel/generation/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/ipex/inference.py` & `optimum-intel-1.9.3/optimum/intel/ipex/inference.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/neural_compressor/__init__.py` & `optimum-intel-1.9.3/optimum/intel/neural_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/neural_compressor/configuration.py` & `optimum-intel-1.9.3/optimum/intel/neural_compressor/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/neural_compressor/modeling_diffusion.py` & `optimum-intel-1.9.3/optimum/intel/neural_compressor/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/neural_compressor/neural_coder_adaptor.py` & `optimum-intel-1.9.3/optimum/intel/neural_compressor/neural_coder_adaptor.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/neural_compressor/quantization.py` & `optimum-intel-1.9.3/optimum/intel/neural_compressor/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/neural_compressor/trainer.py` & `optimum-intel-1.9.3/optimum/intel/neural_compressor/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/neural_compressor/trainer_seq2seq.py` & `optimum-intel-1.9.3/optimum/intel/neural_compressor/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/neural_compressor/utils.py` & `optimum-intel-1.9.3/optimum/intel/neural_compressor/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/__init__.py` & `optimum-intel-1.9.3/optimum/intel/openvino/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/configuration.py` & `optimum-intel-1.9.3/optimum/intel/openvino/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/modeling.py` & `optimum-intel-1.9.3/optimum/intel/openvino/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/modeling_base.py` & `optimum-intel-1.9.3/optimum/intel/openvino/modeling_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,30 +259,29 @@
             use_auth_token (`str` or `bool`):
                 Is needed to load models from a private repository
             revision (`str`):
                 Revision is the specific model version to use. It can be a branch name, a tag name, or a commit id
             kwargs (`Dict`, *optional*):
                 kwargs will be passed to the model during initialization
         """
-        if task is None:
-            task = cls._auto_model_to_task(cls.auto_model_class)
+        task = task or cls.export_feature
 
         model_kwargs = {
             "revision": revision,
             "use_auth_token": use_auth_token,
             "cache_dir": cache_dir,
             "subfolder": subfolder,
             "local_files_only": local_files_only,
             "force_download": force_download,
             "trust_remote_code": trust_remote_code,
         }
 
         model = TasksManager.get_model_from_task(task, model_id, **model_kwargs)
-
         model_type = model.config.model_type.replace("_", "-")
+
         onnx_config_class = TasksManager.get_exporter_config_constructor(
             exporter="onnx",
             model=model,
             task=task,
             model_name=model_id,
             model_type=model_type,
         )
```

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/modeling_base_seq2seq.py` & `optimum-intel-1.9.3/optimum/intel/openvino/modeling_base_seq2seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,17 +293,15 @@
                 Revision is the specific model version to use. It can be a branch name, a tag name, or a commit id
             kwargs (`Dict`, *optional*):
                 kwargs will be passed to the model during initialization
         """
         encoder_file_name = os.path.join("encoder", ONNX_ENCODER_NAME)
         decoder_file_name = os.path.join("decoder", ONNX_DECODER_NAME)
         decoder_with_past_file_name = os.path.join("decoder_with_past", ONNX_DECODER_WITH_PAST_NAME)
-
-        if task is None:
-            task = cls._auto_model_to_task(cls.auto_model_class)
+        task = task or cls.export_feature
 
         save_dir = TemporaryDirectory()
         save_dir_path = Path(save_dir.name)
 
         model_kwargs = {
             "revision": revision,
             "use_auth_token": use_auth_token,
```

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/modeling_decoder.py` & `optimum-intel-1.9.3/optimum/intel/openvino/modeling_decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,20 +152,15 @@
         **kwargs,
     ):
         if config.model_type not in _SUPPORTED_ARCHITECTURES:
             logger.warning(
                 f"This architecture : {config.model_type} was not validated, only :{', '.join(_SUPPORTED_ARCHITECTURES)} architectures were "
                 "validated, use at your own risk."
             )
-
-        model_file_name = ONNX_WEIGHTS_NAME
-
-        if task is None:
-            task = cls._auto_model_to_task(cls.auto_model_class)
-
+        task = task or cls.export_feature
         save_dir = TemporaryDirectory()
         save_dir_path = Path(save_dir.name)
         model_kwargs = {
             "revision": revision,
             "use_auth_token": use_auth_token,
             "cache_dir": cache_dir,
             "subfolder": subfolder,
@@ -184,25 +179,25 @@
             model.transformer._prepare_attn_mask = _prepare_attn_mask
         elif config.model_type == "llama":
             model.model._prepare_decoder_attention_mask = _prepare_decoder_attention_mask
         elif config.model_type in {"blenderbot-small", "blenderbot", "opt", "pegasus", "bart"}:
             model.model.decoder._prepare_decoder_attention_mask = _prepare_decoder_attention_mask
 
         # Export the model to the ONNX format
-        export(model=model, config=onnx_config, output=save_dir_path / model_file_name)
+        export(model=model, config=onnx_config, output=save_dir_path / ONNX_WEIGHTS_NAME)
 
         return cls._from_pretrained(
             model_id=save_dir_path,
             config=config,
             from_onnx=True,
             use_auth_token=use_auth_token,
             revision=revision,
             force_download=force_download,
             cache_dir=cache_dir,
-            file_name=model_file_name,
+            file_name=ONNX_WEIGHTS_NAME,
             local_files_only=local_files_only,
             use_cache=use_cache,
             **kwargs,
         )
 
     def _reshape(
         self,
@@ -233,14 +228,19 @@
         model.reshape(shapes)
         return model
 
     def reshape(self, batch_size: int, sequence_length: int):
         logger.warning("Static shapes are not supported for causal language model.")
         return self
 
+    def compile(self):
+        if self.request is None:
+            super().compile()
+            self.request = self.request.create_infer_request()
+
 
 @add_start_docstrings(
     """
     OpenVINO Model with a causal language modeling head on top (linear layer with weights tied to the input
     embeddings).
     """,
     MODEL_START_DOCSTRING,
@@ -269,15 +269,15 @@
         if self.use_cache and past_key_values is not None:
             input_ids = input_ids[:, -1:]
 
         inputs = {}
         if past_key_values is not None:
             # Flatten the past_key_values
             past_key_values = tuple(
-                np.array(past_key_value) for pkv_per_layer in past_key_values for past_key_value in pkv_per_layer
+                past_key_value for pkv_per_layer in past_key_values for past_key_value in pkv_per_layer
             )
             # Add the past_key_values to the decoder inputs
             inputs = dict(zip(self.key_value_input_names, past_key_values))
 
         # Create empty past_key_values for decoder_with_past first generation step
         elif self.use_cache:
             shape_input_ids = input_ids.shape
@@ -297,23 +297,22 @@
         inputs["input_ids"] = np.array(input_ids)
 
         # Add the attention_mask inputs when needed
         if "attention_mask" in self.input_names and attention_mask is not None:
             inputs["attention_mask"] = np.array(attention_mask)
 
         # Run inference
-        outputs = self.request(inputs, shared_memory=True)
+        self.request.start_async(inputs, shared_memory=True)
+        self.request.wait()
 
-        logits = torch.from_numpy(outputs["logits"]).to(self.device)
+        logits = torch.from_numpy(self.request.get_tensor("logits").data).to(self.device)
 
         if self.use_cache:
             # Tuple of length equal to : number of layer * number of past_key_value per decoder layer (2 corresponds to the self-attention layer)
-            past_key_values = tuple(
-                torch.from_numpy(outputs[key]).to(self.device) for key in self.key_value_output_names
-            )
+            past_key_values = tuple(self.request.get_tensor(key).data for key in self.key_value_output_names)
             # Tuple of tuple of length `n_layers`, with each tuple of length equal to 2 (k/v of self-attention)
             past_key_values = tuple(
                 past_key_values[i : i + self.num_pkv] for i in range(0, len(past_key_values), self.num_pkv)
             )
         else:
             past_key_values = None
 
@@ -341,44 +340,38 @@
         self, past_key_values: Tuple[Tuple[torch.Tensor]], beam_idx: torch.Tensor
     ) -> Tuple[Tuple[torch.Tensor]]:
         """
         This function is used to re-order the `past_key_values` cache if [`~PreTrainedModel.beam_search`] or
         [`~PreTrainedModel.beam_sample`] is called.
         This is required to match `past_key_values` with the correct beam_idx at every generation step.
         """
+
         if self.config.model_type == "bloom":
             return self._reorder_cache_bloom(past_key_values, beam_idx)
 
         # from transformers.models.gpt2.modeling_gpt2.GPT2LMHeadModel._reorder_cache
         return tuple(
-            tuple(past_state.index_select(0, beam_idx.to(past_state.device)) for past_state in layer_past)
-            for layer_past in past_key_values
+            tuple(np.take(past_state, beam_idx, 0) for past_state in layer_past) for layer_past in past_key_values
         )
 
     # Copied from transformers.models.bloom.modeling_bloom.BloomForCausalLM._reorder_cache
     def _reorder_cache_bloom(
         self, past_key_values: Tuple[Tuple[torch.Tensor]], beam_idx: torch.Tensor
     ) -> Tuple[Tuple[torch.Tensor]]:
         """
         This function is used to re-order the `past_key_values` cache if [`~PreTrainedModel.beam_search`] or
         [`~PreTrainedModel.beam_sample`] is called for bloom architecture.
         This is required to match `past_key_values` with the correct beam_idx at every generation step.
         """
         standardized_past = self._convert_to_standard_cache(past_key_values, batch_size=len(beam_idx))
 
-        # Get a copy of `beam_idx` on all the devices where we need those indices.
-        device_to_beam_idx = {
-            past_state.device: beam_idx.to(past_state.device)
-            for layer_past in past_key_values
-            for past_state in layer_past
-        }
         reordered_past = tuple(
             (
-                layer_past[0].index_select(0, device_to_beam_idx[layer_past[0].device]),
-                layer_past[1].index_select(0, device_to_beam_idx[layer_past[0].device]),
+                np.take(layer_past[0], beam_idx, 0),
+                np.take(layer_past[1], beam_idx, 0),
             )
             for layer_past in standardized_past
         )
         return self._convert_to_bloom_cache(reordered_past)
 
     # Copied from transformers.models.bloom.modeling_bloom.BloomPreTrainedModel._convert_to_bloom_cache
     @staticmethod
@@ -388,16 +381,16 @@
         """
         batch_size, num_heads, head_dim, seq_length = past_key_value[0][0].shape
         batch_size_times_num_heads = batch_size * num_heads
         # key:  [batch_size, num_heads, head_dim, seq_length] -> [batch_size * num_heads, head_dim, seq_length]
         # value: [batch_size, num_heads, seq_length, head_dim] -> [batch_size * num_heads, seq_length, head_dim]
         return tuple(
             (
-                layer_past[0].view(batch_size_times_num_heads, head_dim, seq_length),
-                layer_past[1].view(batch_size_times_num_heads, seq_length, head_dim),
+                layer_past[0].reshape((batch_size_times_num_heads, head_dim, seq_length)),
+                layer_past[1].reshape((batch_size_times_num_heads, seq_length, head_dim)),
             )
             for layer_past in past_key_value
         )
 
     # Adapted from transformers.models.bloom.modeling_bloom.BloomPreTrainedModel._convert_to_standard_cache
     def _convert_to_standard_cache(
         self, past_key_value: Tuple[Tuple[torch.Tensor]], batch_size: int
@@ -410,16 +403,16 @@
 
         batch_size_times_num_heads, head_dim, seq_length = past_key_value[0][0].shape
         num_heads = batch_size_times_num_heads // batch_size
         # key: [batch_size * num_heads, head_dim, seq_length] -> [batch_size, num_heads, head_dim, seq_length]
         # value: [batch_size * num_heads, seq_length, head_dim] -> [batch_size, num_heads, seq_length, head_dim]
         return tuple(
             (
-                layer_past[0].view(batch_size, num_heads, head_dim, seq_length),
-                layer_past[1].view(batch_size, num_heads, seq_length, head_dim),
+                layer_past[0].reshape((batch_size, num_heads, head_dim, seq_length)),
+                layer_past[1].reshape((batch_size, num_heads, seq_length, head_dim)),
             )
             for layer_past in past_key_value
         )
 
     def can_generate(self):
         """Returns True to validate the check that the model using `GenerationMixin.generate()` can indeed generate."""
         return True
```

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/modeling_diffusion.py` & `optimum-intel-1.9.3/optimum/intel/openvino/modeling_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,16 +284,16 @@
         tokenizer: "CLIPTokenizer" = None,
         scheduler: Union["DDIMScheduler", "PNDMScheduler", "LMSDiscreteScheduler"] = None,
         feature_extractor: Optional["CLIPFeatureExtractor"] = None,
         **kwargs,
     ):
         if is_torch_version(">", "1.13.1") and is_torch_version("<=", "2.0.1"):
             register_custom_scaled_dot_product_attention_export()
-        if task is None:
-            task = cls._auto_model_to_task(cls.auto_model_class)
+        task = task or cls.export_feature
+
         save_dir = TemporaryDirectory()
         save_dir_path = Path(save_dir.name)
 
         model_kwargs = {
             "revision": revision,
             "use_auth_token": use_auth_token,
             "cache_dir": cache_dir,
```

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/modeling_seq2seq.py` & `optimum-intel-1.9.3/optimum/intel/openvino/modeling_seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
+import numpy as np
 import openvino
 import torch
 import transformers
 from openvino.runtime import Core
 from transformers import AutoConfig, AutoModelForSeq2SeqLM
 from transformers.file_utils import add_start_docstrings, add_start_docstrings_to_model_forward
 from transformers.modeling_outputs import BaseModelOutput, Seq2SeqLMOutput
@@ -245,15 +246,15 @@
     # Copied from transformers.models.bart.modeling_bart.BartForConditionalGeneration._reorder_cache
     @staticmethod
     def _reorder_cache(past, beam_idx) -> Tuple[Tuple[torch.FloatTensor]]:
         reordered_past = ()
         for layer_past in past:
             # Cached cross_attention states don't have to be reordered -> they are always the same
             reordered_past += (
-                tuple(past_state.index_select(0, beam_idx) for past_state in layer_past[:2]) + layer_past[2:],
+                tuple(np.take(past_state, beam_idx, 0) for past_state in layer_past[:2]) + layer_past[2:],
             )
         return reordered_past
 
     def reshape(self, batch_size: int, sequence_length: int):
         """
         Propagates the given input shapes on the model's layers, fixing the inputs shapes of the model.
 
@@ -351,14 +352,16 @@
 
     def __init__(self, model: openvino.runtime.Model, device: str, ov_config: Dict):
         self.model = model
         self._device = device
         self.device = torch.device("cpu")
         self.input_names = {key.get_any_name(): idx for idx, key in enumerate(self.model.inputs)}
         self.key_value_input_names = [key for key in self.input_names if "key_values" in key]
+        self.output_names = {key.get_any_name(): idx for idx, key in enumerate(self.model.outputs)}
+        self.key_value_output_names = [key for key in self.output_names if "key_values" in key or "present" in key]
         is_legacy = any("past_key_values" in key.get_any_name() for key in self.model.outputs)
 
         if len(self.key_value_input_names) > 0 and not is_legacy:
             self.use_past = True
             self.num_pkv = 2
         else:
             self.use_past = False
@@ -395,24 +398,21 @@
             inputs["encoder_attention_mask"] = encoder_attention_mask
 
         # Add the encoder_hidden_states inputs when needed
         if "encoder_hidden_states" in self.input_names and encoder_hidden_states is not None:
             inputs["encoder_hidden_states"] = encoder_hidden_states
 
         # Run inference
-        outputs = self.request(inputs, shared_memory=True)
-        logits = torch.from_numpy(outputs["logits"]).to(self.device)
+        self.request.start_async(inputs, shared_memory=True)
+        self.request.wait()
+        logits = torch.from_numpy(self.request.get_tensor("logits").data).to(self.device)
 
         # Tuple of length equal to : number of layer * number of past_key_value per decoder layer (2 corresponds to the
         # self-attention layer and 2 to the cross-attention layer)
-        out_past_key_values = tuple(
-            torch.from_numpy(outputs[next(iter(key))]).to(self.device)
-            for key in outputs.names()
-            if ("key_values" in next(iter(key)) or "present" in next(iter(key)))
-        )
+        out_past_key_values = tuple(self.request.get_tensor(key).data for key in self.key_value_output_names)
 
         # Tuple of tuple of length `n_layers`, with each tuple of length equal to:
         # * 4 for the decoder without cache (k/v of self-attention + k/v of cross-attention)
         # * 2 for the decoder with cache (k/v of self-attention as cross-attention cache is constant)
         if self.use_past is False:
             out_past_key_values = tuple(
                 out_past_key_values[i : i + self.num_pkv] for i in range(0, len(out_past_key_values), self.num_pkv)
@@ -428,8 +428,8 @@
 
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
 
     def _compile(self):
         if self.request is None:
             logger.info("Compiling the decoder...")
-            self.request = core.compile_model(self.model, self._device, self.ov_config)
+            self.request = core.compile_model(self.model, self._device, self.ov_config).create_infer_request()
```

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/quantization.py` & `optimum-intel-1.9.3/optimum/intel/openvino/quantization.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 #  limitations under the License.
 
 import inspect
 import io
 import logging
 from itertools import chain
 from pathlib import Path
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
+import nncf
 import openvino
 import torch
 import transformers
 from datasets import Dataset, load_dataset
 from huggingface_hub import HfApi
 from nncf import NNCFConfig
 from nncf.torch import create_compressed_model, register_default_init_args
 from nncf.torch.dynamic_graph.io_handling import wrap_nncf_model_inputs_with_objwalk
 from nncf.torch.initialization import PTInitializingDataLoader
 from nncf.torch.nncf_network import NNCFNetwork
 from openvino._offline_transformations import compress_quantize_weights_transformation
-from openvino.runtime import Core
+from openvino.runtime import Core, Tensor
 from torch.onnx import export as onnx_export
 from torch.utils._pytree import tree_map
 from torch.utils.data import DataLoader, RandomSampler
 from transformers import DataCollator, PreTrainedModel, default_data_collator
 
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import OnnxConfig
```

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/trainer.py` & `optimum-intel-1.9.3/optimum/intel/openvino/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/training_args.py` & `optimum-intel-1.9.3/optimum/intel/openvino/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/openvino/utils.py` & `optimum-intel-1.9.3/optimum/intel/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/__init__.py` & `optimum-intel-1.9.3/optimum/intel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/constant.py` & `optimum-intel-1.9.3/optimum/intel/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/dummy_ipex_objects.py` & `optimum-intel-1.9.3/optimum/intel/utils/dummy_ipex_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py` & `optimum-intel-1.9.3/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/dummy_neural_compressor_objects.py` & `optimum-intel-1.9.3/optimum/intel/utils/dummy_neural_compressor_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py` & `optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_and_nncf_objects.py` & `optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_and_nncf_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/dummy_openvino_objects.py` & `optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/import_utils.py` & `optimum-intel-1.9.3/optimum/intel/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/utils/modeling_utils.py` & `optimum-intel-1.9.3/optimum/intel/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/optimum/intel/version.py` & `optimum-intel-1.9.3/optimum/intel/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.9.2"
+__version__ = "1.9.3"
```

### Comparing `optimum-intel-1.9.2/optimum_intel.egg-info/PKG-INFO` & `optimum-intel-1.9.3/optimum_intel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.9.2
+Version: 1.9.3
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.9.2/optimum_intel.egg-info/SOURCES.txt` & `optimum-intel-1.9.3/optimum_intel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/pyproject.toml` & `optimum-intel-1.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/setup.cfg` & `optimum-intel-1.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.2/setup.py` & `optimum-intel-1.9.3/setup.py`

 * *Files identical despite different names*

