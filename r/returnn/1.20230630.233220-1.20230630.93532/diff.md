# Comparing `tmp/returnn-1.20230630.233220.tar.gz` & `tmp/returnn-1.20230630.93532.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230630.233220.tar", last modified: Fri Jun 30 21:49:18 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230630.93532.tar", last modified: Fri Jun 30 09:57:43 2023, max compression
```

## Comparing `returnn-1.20230630.233220.tar` & `returnn-1.20230630.93532.tar`

### file list

```diff
@@ -1,449 +1,449 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 21:49:17.000000 returnn-1.20230630.233220/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63112 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 21:48:57.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-30 21:49:01.000000 returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40243 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100183 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36218 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   152240 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40275 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586582 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   543165 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   302020 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/util/gradient_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    35987 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72576 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   561762 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:18.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-30 21:48:55.000000 returnn-1.20230630.233220/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63112 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 09:57:18.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-30 09:57:21.000000 returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40243 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99665 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152284 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40275 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586634 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   543165 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   302020 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/util/gradient_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35987 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72576 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   561922 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:57:43.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-30 09:57:16.000000 returnn-1.20230630.93532/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230630.233220/.gitignore` & `returnn-1.20230630.93532/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/.gitmodules` & `returnn-1.20230630.93532/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/CHANGELOG.md` & `returnn-1.20230630.93532/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/CODEOWNERS` & `returnn-1.20230630.93532/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/CONTRIBUTING.md` & `returnn-1.20230630.93532/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/LICENSE` & `returnn-1.20230630.93532/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/MANIFEST.in` & `returnn-1.20230630.93532/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/PKG-INFO` & `returnn-1.20230630.93532/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230630.233220
+Version: 1.20230630.93532
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230630.233220/README.rst` & `returnn-1.20230630.93532/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/__init__.py` & `returnn-1.20230630.93532/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/12AX.cluster_map` & `returnn-1.20230630.93532/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-fwd.config` & `returnn-1.20230630.93532/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-horovod-mpi.py` & `returnn-1.20230630.93532/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230630.93532/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-hyper-param-tuning.config` & `returnn-1.20230630.93532/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-iter-dataset.py` & `returnn-1.20230630.93532/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-list-devices.py` & `returnn-1.20230630.93532/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-lua-torch-layer.config` & `returnn-1.20230630.93532/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230630.93532/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-returnn-as-framework.py` & `returnn-1.20230630.93532/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-rf.config` & `returnn-1.20230630.93532/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-rhn-enwik8.config` & `returnn-1.20230630.93532/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-sprint-interface.py` & `returnn-1.20230630.93532/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-att-copy.config` & `returnn-1.20230630.93532/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-attention.config` & `returnn-1.20230630.93532/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230630.93532/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230630.93532/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-enc-dec.config` & `returnn-1.20230630.93532/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230630.93532/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230630.93532/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230630.93532/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230630.93532/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230630.93532/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230630.93532/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230630.93532/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230630.93532/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230630.93532/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230630.93532/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-rec-self-att.config` & `returnn-1.20230630.93532/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230630.93532/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230630.93532/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230630.93532/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-torch.config` & `returnn-1.20230630.93532/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230630.93532/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/demo.sh` & `returnn-1.20230630.93532/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230630.93532/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230630.93532/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230630.93532/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/README.txt` & `returnn-1.20230630.93532/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/config_demo` & `returnn-1.20230630.93532/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230630.93532/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/config_real` & `returnn-1.20230630.93532/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230630.93532/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/decode.py` & `returnn-1.20230630.93532/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230630.93532/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230630.93532/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230630.93532/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230630.93532/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230630.93532/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230630.93532/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230630.93532/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230630.93532/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230630.93532/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230630.93532/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/__init__.py` & `returnn-1.20230630.93532/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/__main__.py` & `returnn-1.20230630.93532/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/__old_mod_loader__.py` & `returnn-1.20230630.93532/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/__setup__.py` & `returnn-1.20230630.93532/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/config.py` & `returnn-1.20230630.93532/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/audio.py` & `returnn-1.20230630.93532/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/basic.py` & `returnn-1.20230630.93532/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/bundle_file.py` & `returnn-1.20230630.93532/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/cached.py` & `returnn-1.20230630.93532/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/cached2.py` & `returnn-1.20230630.93532/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/generating.py` & `returnn-1.20230630.93532/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/hdf.py` & `returnn-1.20230630.93532/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/lm.py` & `returnn-1.20230630.93532/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/map.py` & `returnn-1.20230630.93532/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/meta.py` & `returnn-1.20230630.93532/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/multi_proc.py` & `returnn-1.20230630.93532/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/normalization_data.py` & `returnn-1.20230630.93532/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/numpy_dump.py` & `returnn-1.20230630.93532/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/raw_wav.py` & `returnn-1.20230630.93532/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/sprint.py` & `returnn-1.20230630.93532/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/stereo.py` & `returnn-1.20230630.93532/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230630.93532/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/datasets/util/vocabulary.py` & `returnn-1.20230630.93532/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/engine/base.py` & `returnn-1.20230630.93532/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/engine/batch.py` & `returnn-1.20230630.93532/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230630.93532/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230630.93532/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230630.93532/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230630.93532/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/graph_editor/edit.py` & `returnn-1.20230630.93532/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230630.93532/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/graph_editor/select.py` & `returnn-1.20230630.93532/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230630.93532/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/graph_editor/transform.py` & `returnn-1.20230630.93532/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/extern/graph_editor/util.py` & `returnn-1.20230630.93532/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/forward_iface.py` & `returnn-1.20230630.93532/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/__init__.py` & `returnn-1.20230630.93532/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/_backend.py` & `returnn-1.20230630.93532/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/_numpy_backend.py` & `returnn-1.20230630.93532/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/_utils.py` & `returnn-1.20230630.93532/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/array_.py` & `returnn-1.20230630.93532/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/attention.py` & `returnn-1.20230630.93532/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/cond.py` & `returnn-1.20230630.93532/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/const.py` & `returnn-1.20230630.93532/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/container.py` & `returnn-1.20230630.93532/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/conv.py` & `returnn-1.20230630.93532/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/device.py` & `returnn-1.20230630.93532/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/dims.py` & `returnn-1.20230630.93532/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/dropout.py` & `returnn-1.20230630.93532/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/dtype.py` & `returnn-1.20230630.93532/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/encoder/base.py` & `returnn-1.20230630.93532/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/encoder/conformer.py` & `returnn-1.20230630.93532/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/init.py` & `returnn-1.20230630.93532/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/linear.py` & `returnn-1.20230630.93532/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/loop.py` & `returnn-1.20230630.93532/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/loss.py` & `returnn-1.20230630.93532/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/math_.py` & `returnn-1.20230630.93532/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/matmul.py` & `returnn-1.20230630.93532/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/module.py` & `returnn-1.20230630.93532/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/normalization.py` & `returnn-1.20230630.93532/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/parameter.py` & `returnn-1.20230630.93532/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/rand.py` & `returnn-1.20230630.93532/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/rec.py` & `returnn-1.20230630.93532/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/reduce.py` & `returnn-1.20230630.93532/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/run_ctx.py` & `returnn-1.20230630.93532/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/signal.py` & `returnn-1.20230630.93532/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/state.py` & `returnn-1.20230630.93532/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/tensor_array.py` & `returnn-1.20230630.93532/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/frontend/types.py` & `returnn-1.20230630.93532/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/import_/common.py` & `returnn-1.20230630.93532/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/import_/git.py` & `returnn-1.20230630.93532/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/import_/import_.py` & `returnn-1.20230630.93532/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/learning_rate_control.py` & `returnn-1.20230630.93532/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/log.py` & `returnn-1.20230630.93532/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/native_op.cpp` & `returnn-1.20230630.93532/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/native_op.py` & `returnn-1.20230630.93532/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/pretrain.py` & `returnn-1.20230630.93532/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/sprint/cache.py` & `returnn-1.20230630.93532/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/sprint/control.py` & `returnn-1.20230630.93532/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/sprint/error_signals.py` & `returnn-1.20230630.93532/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/sprint/extern_interface.py` & `returnn-1.20230630.93532/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/sprint/interface.py` & `returnn-1.20230630.93532/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/_dim_extra.py` & `returnn-1.20230630.93532/returnn/tensor/_dim_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -2848,3415 +2848,3383 @@
 0000b1f0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
 0000b200: 2020 2020 2061 6c6c 6f77 5f73 616d 655f       allow_same_
 0000b210: 7370 6174 6961 6c5f 6469 6d20 3d20 616c  spatial_dim = al
 0000b220: 6c6f 775f 7361 6d65 5f66 6561 7475 7265  low_same_feature
 0000b230: 5f64 696d 0a20 2020 2020 2020 2073 656c  _dim.        sel
 0000b240: 665f 6261 7365 203d 2073 656c 662e 6765  f_base = self.ge
 0000b250: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
-0000b260: 6173 6528 7361 6d65 5f64 696d 3d54 7275  ase(same_dim=Tru
-0000b270: 6529 2069 6620 6465 7269 7665 645f 6d61  e) if derived_ma
-0000b280: 7463 6865 7320 656c 7365 2073 656c 662e  tches else self.
-0000b290: 6765 745f 7361 6d65 5f62 6173 6528 290a  get_same_base().
-0000b2a0: 2020 2020 2020 2020 6f74 6865 725f 6261          other_ba
-0000b2b0: 7365 203d 206f 7468 6572 2e67 6574 5f73  se = other.get_s
-0000b2c0: 616d 655f 6465 7269 7665 645f 6261 7365  ame_derived_base
-0000b2d0: 2873 616d 655f 6469 6d3d 5472 7565 2920  (same_dim=True) 
-0000b2e0: 6966 2064 6572 6976 6564 5f6d 6174 6368  if derived_match
-0000b2f0: 6573 2065 6c73 6520 6f74 6865 722e 6765  es else other.ge
-0000b300: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-0000b310: 2020 2020 2020 6966 2073 656c 665f 6261        if self_ba
-0000b320: 7365 2069 7320 6f74 6865 725f 6261 7365  se is other_base
-0000b330: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000b340: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-0000b350: 2020 6966 2073 656c 665f 6261 7365 2e64    if self_base.d
-0000b360: 6572 6976 6564 5f66 726f 6d5f 6f70 2061  erived_from_op a
-0000b370: 6e64 206f 7468 6572 5f62 6173 652e 6465  nd other_base.de
-0000b380: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-0000b390: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000b3a0: 6c66 5f62 6173 652e 6465 7269 7665 645f  lf_base.derived_
-0000b3b0: 6672 6f6d 5f6f 7020 3d3d 206f 7468 6572  from_op == other
-0000b3c0: 5f62 6173 652e 6465 7269 7665 645f 6672  _base.derived_fr
-0000b3d0: 6f6d 5f6f 703a 0a20 2020 2020 2020 2020  om_op:.         
-0000b3e0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000b3f0: 7565 0a20 2020 2020 2020 2073 656c 665f  ue.        self_
-0000b400: 6b69 6e64 203d 2073 656c 662e 6b69 6e64  kind = self.kind
-0000b410: 0a20 2020 2020 2020 206f 7468 6572 5f6b  .        other_k
-0000b420: 696e 6420 3d20 6f74 6865 722e 6b69 6e64  ind = other.kind
-0000b430: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000b440: 5f6b 696e 6420 3d3d 206f 7468 6572 5f6b  _kind == other_k
-0000b450: 696e 6420 3d3d 2044 696d 5479 7065 732e  ind == DimTypes.
-0000b460: 4665 6174 7572 6520 616e 6420 6967 6e6f  Feature and igno
-0000b470: 7265 5f66 6561 7475 7265 5f64 696d 3a0a  re_feature_dim:.
-0000b480: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000b490: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-0000b4a0: 6966 2074 7265 6174 5f66 6561 7475 7265  if treat_feature
-0000b4b0: 5f61 735f 7370 6174 6961 6c3a 0a20 2020  _as_spatial:.   
-0000b4c0: 2020 2020 2020 2020 2023 204e 6f74 653a           # Note:
-0000b4d0: 204e 6f20 6b69 6e64 2061 7420 616c 6c3a   No kind at all:
-0000b4e0: 2052 6569 6e74 6572 7072 6574 2074 7265   Reinterpret tre
-0000b4f0: 6174 5f66 6561 7475 7265 5f61 735f 7370  at_feature_as_sp
-0000b500: 6174 6961 6c20 6120 6269 743a 0a20 2020  atial a bit:.   
-0000b510: 2020 2020 2020 2020 2023 2041 7373 756d           # Assum
-0000b520: 6520 7468 6174 2077 6520 7761 6e74 2074  e that we want t
-0000b530: 6865 6d20 616c 6c20 746f 2062 6520 6861  hem all to be ha
-0000b540: 6e64 6c65 6420 7468 6520 7361 6d65 2c20  ndled the same, 
-0000b550: 6e6f 206d 6174 7465 7220 7468 6520 6b69  no matter the ki
-0000b560: 6e64 2e0a 2020 2020 2020 2020 2020 2020  nd..            
-0000b570: 2320 2845 7863 6570 7420 6f66 2062 6174  # (Except of bat
-0000b580: 6368 2064 696d 206b 696e 642c 2077 6869  ch dim kind, whi
-0000b590: 6368 2069 7320 7374 696c 6c20 6578 636c  ch is still excl
-0000b5a0: 7564 6564 2068 6572 652e 290a 2020 2020  uded here.).    
-0000b5b0: 2020 2020 2020 2020 6966 2073 656c 665f          if self_
-0000b5c0: 6b69 6e64 203d 3d20 4469 6d54 7970 6573  kind == DimTypes
-0000b5d0: 2e46 6561 7475 7265 206f 7220 6e6f 7420  .Feature or not 
-0000b5e0: 7365 6c66 5f6b 696e 643a 0a20 2020 2020  self_kind:.     
-0000b5f0: 2020 2020 2020 2020 2020 2073 656c 665f             self_
-0000b600: 6b69 6e64 203d 2044 696d 5479 7065 732e  kind = DimTypes.
-0000b610: 5370 6174 6961 6c0a 2020 2020 2020 2020  Spatial.        
-0000b620: 2020 2020 6966 206f 7468 6572 5f6b 696e      if other_kin
-0000b630: 6420 3d3d 2044 696d 5479 7065 732e 4665  d == DimTypes.Fe
-0000b640: 6174 7572 6520 6f72 206e 6f74 206f 7468  ature or not oth
-0000b650: 6572 5f6b 696e 643a 0a20 2020 2020 2020  er_kind:.       
-0000b660: 2020 2020 2020 2020 206f 7468 6572 5f6b           other_k
-0000b670: 696e 6420 3d20 4469 6d54 7970 6573 2e53  ind = DimTypes.S
-0000b680: 7061 7469 616c 0a20 2020 2020 2020 2069  patial.        i
-0000b690: 6620 7365 6c66 2e64 696d 656e 7369 6f6e  f self.dimension
-0000b6a0: 2021 3d20 6f74 6865 722e 6469 6d65 6e73   != other.dimens
-0000b6b0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-0000b6c0: 2069 6620 6272 6f61 6463 6173 745f 6d61   if broadcast_ma
-0000b6d0: 7463 6865 7320 616e 6420 2873 656c 662e  tches and (self.
-0000b6e0: 6469 6d65 6e73 696f 6e20 3d3d 2031 206f  dimension == 1 o
-0000b6f0: 7220 6f74 6865 722e 6469 6d65 6e73 696f  r other.dimensio
-0000b700: 6e20 3d3d 2031 293a 0a20 2020 2020 2020  n == 1):.       
-0000b710: 2020 2020 2020 2020 2070 6173 7320 2023           pass  #
-0000b720: 2070 6173 7320 6f6e 0a20 2020 2020 2020   pass on.       
-0000b730: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000b740: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b750: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-0000b760: 6966 2073 656c 665f 6b69 6e64 2021 3d20  if self_kind != 
-0000b770: 6f74 6865 725f 6b69 6e64 3a0a 2020 2020  other_kind:.    
-0000b780: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0000b790: 616c 7365 0a20 2020 2020 2020 2069 6620  alse.        if 
-0000b7a0: 7365 6c66 5f6b 696e 6420 3d3d 206f 7468  self_kind == oth
-0000b7b0: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
-0000b7c0: 7065 732e 4261 7463 683a 0a20 2020 2020  pes.Batch:.     
-0000b7d0: 2020 2020 2020 2023 204e 6f74 653a 2054         # Note: T
-0000b7e0: 6869 7320 6d69 6768 7420 6265 2069 6e63  his might be inc
-0000b7f0: 6f72 7265 6374 2069 6e20 736f 6d65 2063  orrect in some c
-0000b800: 6173 6573 2c0a 2020 2020 2020 2020 2020  ases,.          
-0000b810: 2020 2320 652e 672e 2066 6f72 2062 6561    # e.g. for bea
-0000b820: 6d20 7365 6172 6368 2077 6865 6e20 7765  m search when we
-0000b830: 2068 6176 6520 7468 6520 6265 616d 2068   have the beam h
-0000b840: 6964 6465 6e20 696e 2074 6865 2062 6174  idden in the bat
-0000b850: 6368 2064 696d 2c0a 2020 2020 2020 2020  ch dim,.        
-0000b860: 2020 2020 2320 6f72 2077 6865 6e20 7765      # or when we
-0000b870: 2075 7365 6420 4d65 7267 6544 696d 734c   used MergeDimsL
-0000b880: 6179 6572 206f 6e20 7468 6520 6261 7463  ayer on the batc
-0000b890: 6820 6178 6973 2c20 6f72 2073 6f2e 0a20  h axis, or so.. 
-0000b8a0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
-0000b8b0: 6d69 6768 7420 6e65 6564 2074 6f20 6578  might need to ex
-0000b8c0: 7465 6e64 2074 6865 206c 6f67 6963 2068  tend the logic h
-0000b8d0: 6572 6520 6c61 7465 722e 0a20 2020 2020  ere later..     
-0000b8e0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000b8f0: 7565 0a20 2020 2020 2020 2069 6620 4265  ue.        if Be
-0000b900: 6861 7669 6f72 5665 7273 696f 6e2e 6765  haviorVersion.ge
-0000b910: 7428 2920 3e3d 2031 363a 0a20 2020 2020  t() >= 16:.     
-0000b920: 2020 2020 2020 2023 2045 6974 6865 7220         # Either 
-0000b930: 7365 6c66 206f 7220 6f74 6865 7220 6973  self or other is
-0000b940: 2073 6f6d 6520 6469 6d20 7461 6720 6578   some dim tag ex
-0000b950: 706c 6963 6974 6c79 2063 7265 6174 6564  plicitly created
-0000b960: 2062 7920 7468 6520 7573 6572 2c0a 2020   by the user,.  
-0000b970: 2020 2020 2020 2020 2020 2320 616e 6420            # and 
-0000b980: 7468 6579 2061 7265 206e 6f74 2074 6865  they are not the
-0000b990: 2073 616d 652c 2073 6f20 7765 206e 6576   same, so we nev
-0000b9a0: 6572 2074 7265 6174 2074 6865 6d20 6173  er treat them as
-0000b9b0: 2065 7175 616c 2e0a 2020 2020 2020 2020   equal..        
-0000b9c0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0000b9d0: 6175 746f 5f67 656e 6572 6174 6564 206f  auto_generated o
-0000b9e0: 7220 6e6f 7420 6f74 6865 722e 6175 746f  r not other.auto
-0000b9f0: 5f67 656e 6572 6174 6564 3a0a 2020 2020  _generated:.    
-0000ba00: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000ba10: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
-0000ba20: 2061 6e64 2028 0a20 2020 2020 2020 2020   and (.         
-0000ba30: 2020 2020 2020 2020 2020 2028 7365 6c66             (self
-0000ba40: 2e64 696d 656e 7369 6f6e 203d 3d20 3120  .dimension == 1 
-0000ba50: 616e 6420 7365 6c66 2e61 7574 6f5f 6765  and self.auto_ge
-0000ba60: 6e65 7261 7465 6429 206f 7220 286f 7468  nerated) or (oth
-0000ba70: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
-0000ba80: 3120 616e 6420 6f74 6865 722e 6175 746f  1 and other.auto
-0000ba90: 5f67 656e 6572 6174 6564 290a 2020 2020  _generated).    
-0000baa0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2020 2070 6173 7320 2023 2065 7863 6570     pass  # excep
-0000bad0: 7469 6f6e 2c20 616c 6c6f 7720 6272 6f61  tion, allow broa
-0000bae0: 6463 6173 7420 6c6f 6769 630a 2020 2020  dcast logic.    
-0000baf0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000bb00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bb10: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000bb20: 7365 0a20 2020 2020 2020 2069 6620 7365  se.        if se
-0000bb30: 6c66 5f6b 696e 6420 3d3d 206f 7468 6572  lf_kind == other
-0000bb40: 5f6b 696e 6420 3d3d 2044 696d 5479 7065  _kind == DimType
-0000bb50: 732e 4665 6174 7572 653a 0a20 2020 2020  s.Feature:.     
-0000bb60: 2020 2020 2020 2069 6620 616c 6c6f 775f         if allow_
-0000bb70: 7361 6d65 5f66 6561 7475 7265 5f64 696d  same_feature_dim
-0000bb80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bb90: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000bba0: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
-0000bbb0: 6e64 203d 3d20 6f74 6865 725f 6b69 6e64  nd == other_kind
-0000bbc0: 203d 3d20 4469 6d54 7970 6573 2e53 7061   == DimTypes.Spa
-0000bbd0: 7469 616c 3a0a 2020 2020 2020 2020 2020  tial:.          
-0000bbe0: 2020 6966 2061 6c6c 6f77 5f73 616d 655f    if allow_same_
-0000bbf0: 7370 6174 6961 6c5f 6469 6d3a 0a20 2020  spatial_dim:.   
-0000bc00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000bc10: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
-0000bc20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc40: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000bc50: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000bc60: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
-0000bc70: 2061 6e64 2028 7365 6c66 2e64 696d 656e   and (self.dimen
-0000bc80: 7369 6f6e 203d 3d20 3120 6f72 206f 7468  sion == 1 or oth
-0000bc90: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
-0000bca0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-0000bcb0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000bcc0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000bcd0: 6966 2075 6e6b 6e6f 776e 5f73 7061 7469  if unknown_spati
-0000bce0: 616c 5f6d 6174 6368 6573 2061 6e64 2028  al_matches and (
-0000bcf0: 2873 656c 662e 6479 6e5f 7369 7a65 2069  (self.dyn_size i
-0000bd00: 7320 4e6f 6e65 2920 6f72 2028 6f74 6865  s None) or (othe
-0000bd10: 722e 6479 6e5f 7369 7a65 2069 7320 4e6f  r.dyn_size is No
-0000bd20: 6e65 2929 3a0a 2020 2020 2020 2020 2020  ne)):.          
-0000bd30: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0000bd40: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-0000bd50: 2075 6e64 6566 696e 6564 5f6d 6174 6368   undefined_match
-0000bd60: 6573 2061 6e64 2028 7365 6c66 2e75 6e64  es and (self.und
-0000bd70: 6566 696e 6564 206f 7220 6f74 6865 722e  efined or other.
-0000bd80: 756e 6465 6669 6e65 6429 3a0a 2020 2020  undefined):.    
-0000bd90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000bda0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-0000bdb0: 2320 496e 2070 7269 6e63 6970 6c65 2c20  # In principle, 
-0000bdc0: 7765 2077 6f75 6c64 2077 616e 7420 746f  we would want to
-0000bdd0: 2063 6865 636b 2066 6f72 2069 6465 6e74   check for ident
-0000bde0: 6974 7920 2873 656c 6620 6973 206f 7468  ity (self is oth
-0000bdf0: 6572 292e 0a20 2020 2020 2020 2023 2057  er)..        # W
-0000be00: 6520 6375 7272 656e 746c 7920 7573 6520  e currently use 
-0000be10: 7468 6520 6465 7363 7269 7074 696f 6e20  the description 
-0000be20: 6265 6361 7573 6520 7468 6520 6964 656e  because the iden
-0000be30: 7469 7479 2077 6f75 6c64 206e 6f74 2062  tity would not b
-0000be40: 6520 7468 6520 7361 6d65 0a20 2020 2020  e the same.     
-0000be50: 2020 2023 2069 6e20 6361 7365 206f 6620     # in case of 
-0000be60: 7465 6d70 6c61 7465 2063 6f6e 7374 7275  template constru
-0000be70: 6374 696f 6e20 7768 6572 6520 6120 6469  ction where a di
-0000be80: 6d20 7461 6720 6973 206f 6e63 6520 6372  m tag is once cr
-0000be90: 6561 7465 6420 666f 7220 6120 7465 6d70  eated for a temp
-0000bea0: 6c61 7465 206c 6179 6572 2c0a 2020 2020  late layer,.    
-0000beb0: 2020 2020 2320 616e 6420 7468 656e 206c      # and then l
-0000bec0: 6174 6572 2061 6761 696e 2066 6f72 2074  ater again for t
-0000bed0: 6865 2072 6561 6c20 6c61 7965 722e 0a20  he real layer.. 
-0000bee0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-0000bef0: 7574 6f5f 6765 6e65 7261 7465 6420 616e  uto_generated an
-0000bf00: 6420 6f74 6865 722e 6175 746f 5f67 656e  d other.auto_gen
-0000bf10: 6572 6174 6564 2061 6e64 2073 656c 662e  erated and self.
-0000bf20: 6465 7363 7269 7074 696f 6e20 3d3d 206f  description == o
-0000bf30: 7468 6572 2e64 6573 6372 6970 7469 6f6e  ther.description
-0000bf40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000bf50: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-0000bf60: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-0000bf70: 2020 2020 6465 6620 5f5f 6571 5f5f 2873      def __eq__(s
-0000bf80: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-0000bf90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000bfa0: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
-0000bfb0: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-0000bfc0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-0000bfd0: 3a72 6574 7572 6e3a 203a 6675 6e63 3a60  :return: :func:`
-0000bfe0: 6973 5f65 7175 616c 6020 7769 7468 2064  is_equal` with d
-0000bff0: 6566 6175 6c74 206f 7074 696f 6e73 0a20  efault options. 
-0000c000: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c010: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-0000c020: 616e 6365 286f 7468 6572 2c20 5f64 2e44  ance(other, _d.D
-0000c030: 696d 293a 0a20 2020 2020 2020 2020 2020  im):.           
-0000c040: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-0000c050: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000c060: 662e 6973 5f65 7175 616c 286f 7468 6572  f.is_equal(other
-0000c070: 290a 0a20 2020 2064 6566 205f 5f6e 655f  )..    def __ne_
-0000c080: 5f28 7365 6c66 3a20 4469 6d2c 206f 7468  _(self: Dim, oth
-0000c090: 6572 3a20 4469 6d29 3a0a 2020 2020 2020  er: Dim):.      
-0000c0a0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-0000c0b0: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
-0000c0c0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-0000c0d0: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
-0000c0e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c0f0: 6e6f 7420 2873 656c 6620 3d3d 206f 7468  not (self == oth
-0000c100: 6572 290a 0a20 2020 2064 6566 205f 5f68  er)..    def __h
-0000c110: 6173 685f 5f28 7365 6c66 293a 0a20 2020  ash__(self):.   
-0000c120: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c130: 203a 7274 7970 653a 2069 6e74 0a20 2020   :rtype: int.   
-0000c140: 2020 2020 203a 7265 7475 726e 3a20 6861       :return: ha
-0000c150: 7368 2c20 6d61 7463 6869 6e67 2074 6f20  sh, matching to 
-0000c160: 3a66 756e 633a 605f 5f65 715f 5f60 0a20  :func:`__eq__`. 
-0000c170: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c180: 2020 2023 2054 6869 7320 6d75 7374 206d     # This must m
-0000c190: 6174 6368 2074 6865 2062 6568 6176 696f  atch the behavio
-0000c1a0: 7220 696e 205f 5f65 715f 5f2c 2077 6869  r in __eq__, whi
-0000c1b0: 6368 2069 7320 6973 5f65 7175 616c 2077  ch is is_equal w
-0000c1c0: 6974 6820 6465 6661 756c 7420 6f70 7469  ith default opti
-0000c1d0: 6f6e 732e 0a20 2020 2020 2020 2023 2049  ons..        # I
-0000c1e0: 2e65 2e20 6469 6666 6572 656e 7420 6861  .e. different ha
-0000c1f0: 7368 2069 6d70 6c69 6573 206e 6f74 2065  sh implies not e
-0000c200: 7175 616c 2028 6275 7420 7361 6d65 2068  qual (but same h
-0000c210: 6173 6820 6e6f 7420 6e65 6365 7373 6172  ash not necessar
-0000c220: 696c 7920 6571 7561 6c29 2e0a 2020 2020  ily equal)..    
-0000c230: 2020 2020 6966 2073 656c 662e 7370 6563      if self.spec
-0000c240: 6961 6c3a 0a20 2020 2020 2020 2020 2020  ial:.           
-0000c250: 2072 6574 7572 6e20 6861 7368 2869 6428   return hash(id(
-0000c260: 7365 6c66 2929 0a20 2020 2020 2020 2069  self)).        i
-0000c270: 6620 7365 6c66 2e69 735f 6261 7463 685f  f self.is_batch_
-0000c280: 6469 6d28 293a 0a20 2020 2020 2020 2020  dim():.         
-0000c290: 2020 2072 6574 7572 6e20 6861 7368 2828     return hash((
-0000c2a0: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-0000c2b0: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
-0000c2c0: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
-0000c2d0: 2e44 696d 2e5f 5f68 6173 685f 5f2c 2073  .Dim.__hash__, s
-0000c2e0: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
-0000c2f0: 2020 6261 7365 203d 2073 656c 662e 6765    base = self.ge
-0000c300: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-0000c310: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
-0000c320: 6520 6973 206e 6f74 2073 656c 663a 0a20  e is not self:. 
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000c340: 6574 7572 6e20 6861 7368 2862 6173 6529  eturn hash(base)
-0000c350: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c360: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
-0000c370: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
-0000c380: 2020 2020 2020 7265 7475 726e 2068 6173        return has
-0000c390: 6828 7365 6c66 2e64 6572 6976 6564 5f66  h(self.derived_f
-0000c3a0: 726f 6d5f 6f70 290a 2020 2020 2020 2020  rom_op).        
-0000c3b0: 2020 2020 6966 2073 656c 662e 6175 746f      if self.auto
-0000c3c0: 5f67 656e 6572 6174 6564 3a0a 2020 2020  _generated:.    
-0000c3d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c3e0: 726e 2068 6173 6828 2862 6173 652e 6b69  rn hash((base.ki
-0000c3f0: 6e64 2c20 6261 7365 2e64 696d 656e 7369  nd, base.dimensi
-0000c400: 6f6e 2c20 6261 7365 2e64 6573 6372 6970  on, base.descrip
-0000c410: 7469 6f6e 2929 0a20 2020 2020 2020 2020  tion)).         
-0000c420: 2020 2072 6574 7572 6e20 6861 7368 2869     return hash(i
-0000c430: 6428 6261 7365 2929 0a0a 2020 2020 6465  d(base))..    de
-0000c440: 6620 5f5f 6c74 5f5f 2873 656c 663a 2044  f __lt__(self: D
-0000c450: 696d 2c20 6f74 6865 723a 2044 696d 293a  im, other: Dim):
-0000c460: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c470: 2020 2020 2044 6566 696e 6520 736f 6d65       Define some
-0000c480: 206f 7264 6572 2e20 5468 6973 2069 7320   order. This is 
-0000c490: 6a75 7374 2073 7563 6820 7468 6174 2060  just such that `
-0000c4a0: 736f 7274 6564 6020 776f 726b 732c 206f  sorted` works, o
-0000c4b0: 7220 736f 6d65 2064 6966 6620 7265 706f  r some diff repo
-0000c4c0: 7274 696e 672c 206f 7220 736f 2e0a 2020  rting, or so..  
-0000c4d0: 2020 2020 2020 4974 2069 7320 6f6e 2073        It is on s
-0000c4e0: 796d 626f 6c69 6320 6c65 7665 6c2c 2069  ymbolic level, i
-0000c4f0: 2e65 2e20 6974 2064 6f65 7320 6e6f 7420  .e. it does not 
-0000c500: 636f 6e73 6964 6572 2074 6865 2061 6374  consider the act
-0000c510: 7561 6c20 6469 6d65 6e73 696f 6e20 7661  ual dimension va
-0000c520: 6c75 652e 0a20 2020 2020 2020 2054 6865  lue..        The
-0000c530: 2064 6566 696e 6564 206f 7264 6572 2073   defined order s
-0000c540: 6f6d 6577 6861 7420 6172 6269 7472 6172  omewhat arbitrar
-0000c550: 792c 2073 6f20 646f 206e 6f74 2072 656c  y, so do not rel
-0000c560: 7920 6f6e 2074 6865 2065 7861 6374 2062  y on the exact b
-0000c570: 6568 6176 696f 722c 0a20 2020 2020 2020  ehavior,.       
-0000c580: 2061 7320 7468 6973 206d 6967 6874 2063   as this might c
-0000c590: 6861 6e67 6520 6174 2073 6f6d 6520 6c61  hange at some la
-0000c5a0: 7465 7220 706f 696e 742e 0a20 2020 2020  ter point..     
-0000c5b0: 2020 2043 7572 7265 6e74 6c79 2c20 6974     Currently, it
-0000c5c0: 2064 6570 656e 6473 206f 6e20 7468 6520   depends on the 
-0000c5d0: 6372 6561 7469 6f6e 2069 6e64 6578 2e0a  creation index..
-0000c5e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000c5f0: 4469 6d20 6f74 6865 723a 0a20 2020 2020  Dim other:.     
-0000c600: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-0000c610: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c620: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000c630: 7461 6e63 6528 6f74 6865 722c 2028 5f64  tance(other, (_d
-0000c640: 2e44 696d 2c20 5f6d 2e4d 6172 6b65 6444  .Dim, _m.MarkedD
-0000c650: 696d 2929 3a0a 2020 2020 2020 2020 2020  im)):.          
-0000c660: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0000c670: 7228 2263 616e 6e6f 7420 636f 6d70 6172  r("cannot compar
-0000c680: 6520 2572 2077 6974 6820 2572 2220 2520  e %r with %r" % 
-0000c690: 2873 656c 662c 206f 7468 6572 2929 0a20  (self, other)). 
-0000c6a0: 2020 2020 2020 2069 6620 7365 6c66 203d         if self =
-0000c6b0: 3d20 6f74 6865 723a 0a20 2020 2020 2020  = other:.       
-0000c6c0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0000c6d0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0000c6e0: 2064 696d 5f63 6d70 5f76 616c 7565 2873   dim_cmp_value(s
-0000c6f0: 656c 6629 203c 2064 696d 5f63 6d70 5f76  elf) < dim_cmp_v
-0000c700: 616c 7565 286f 7468 6572 290a 0a20 2020  alue(other)..   
-0000c710: 2064 6566 205f 5f67 745f 5f28 7365 6c66   def __gt__(self
-0000c720: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-0000c730: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
-0000c740: 6520 3a66 756e 633a 605f 5f6c 745f 5f60  e :func:`__lt__`
-0000c750: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-0000c760: 6d20 4469 6d20 6f74 6865 723a 0a20 2020  m Dim other:.   
-0000c770: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-0000c780: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-0000c790: 2020 2020 2020 7265 7475 726e 206f 7468        return oth
-0000c7a0: 6572 203c 2073 656c 660a 0a20 2020 2064  er < self..    d
-0000c7b0: 6566 205f 5f67 655f 5f28 7365 6c66 2c20  ef __ge__(self, 
-0000c7c0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-0000c7d0: 7265 7475 726e 206e 6f74 2073 656c 6620  return not self 
-0000c7e0: 3c20 6f74 6865 720a 0a20 2020 2064 6566  < other..    def
-0000c7f0: 205f 5f6c 655f 5f28 7365 6c66 2c20 6f74   __le__(self, ot
-0000c800: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-0000c810: 7475 726e 206e 6f74 2073 656c 6620 3e20  turn not self > 
-0000c820: 6f74 6865 720a 0a20 2020 2064 6566 2067  other..    def g
-0000c830: 6574 5f73 616d 655f 6261 7365 2873 656c  et_same_base(sel
-0000c840: 663a 205f 642e 4469 6d29 202d 3e20 5f64  f: _d.Dim) -> _d
-0000c850: 2e44 696d 3a0a 2020 2020 2020 2020 2222  .Dim:.        ""
-0000c860: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
-0000c870: 6e3a 2073 616d 6520 6261 7365 0a20 2020  n: same base.   
-0000c880: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c890: 2069 6620 6e6f 7420 7365 6c66 2e5f 6578   if not self._ex
-0000c8a0: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
-0000c8b0: 2072 6574 7572 6e20 7365 6c66 0a20 2020   return self.   
-0000c8c0: 2020 2020 2062 6173 6520 3d20 7365 6c66       base = self
-0000c8d0: 0a20 2020 2020 2020 2077 6869 6c65 2062  .        while b
-0000c8e0: 6173 652e 7361 6d65 5f61 733a 0a20 2020  ase.same_as:.   
-0000c8f0: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0000c900: 6261 7365 2e73 616d 655f 6173 0a20 2020  base.same_as.   
-0000c910: 2020 2020 2072 6574 7572 6e20 6261 7365       return base
-0000c920: 0a0a 2020 2020 6465 6620 6765 745f 7361  ..    def get_sa
-0000c930: 6d65 5f64 6572 6976 6564 5f62 6173 6528  me_derived_base(
-0000c940: 7365 6c66 3a20 5f64 2e44 696d 2c20 2a2c  self: _d.Dim, *,
-0000c950: 2073 616d 655f 6469 6d3a 2062 6f6f 6c20   same_dim: bool 
-0000c960: 3d20 4661 6c73 6529 202d 3e20 5f64 2e44  = False) -> _d.D
-0000c970: 696d 3a0a 2020 2020 2020 2020 2222 220a  im:.        """.
-0000c980: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0000c990: 616d 655f 6469 6d3a 2069 6620 5472 7565  ame_dim: if True
-0000c9a0: 2c20 7265 7475 726e 2074 6865 206c 6173  , return the las
-0000c9b0: 7420 6261 7365 2077 6869 6368 2068 6173  t base which has
-0000c9c0: 2074 6865 2073 616d 6520 6469 6d65 6e73   the same dimens
-0000c9d0: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-0000c9e0: 2054 6865 2064 6572 6976 6564 2062 6173   The derived bas
-0000c9f0: 6520 6d69 6768 7420 6861 7665 2061 2064  e might have a d
-0000ca00: 6966 6665 7265 6e74 2064 696d 656e 7369  ifferent dimensi
-0000ca10: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-0000ca20: 496e 2063 6173 6520 6974 2069 7320 6479  In case it is dy
-0000ca30: 6e61 6d69 632c 2074 6865 2064 696d 656e  namic, the dimen
-0000ca40: 7369 6f6e 2069 7320 4e6f 6e65 2c20 736f  sion is None, so
-0000ca50: 2069 7420 6973 2061 6c77 6179 7320 7468   it is always th
-0000ca60: 6520 7361 6d65 2e0a 2020 2020 2020 2020  e same..        
-0000ca70: 2020 2020 496e 2063 6173 6520 6974 2069      In case it i
-0000ca80: 7320 7374 6174 6963 2c20 7468 6572 6520  s static, there 
-0000ca90: 6d69 6768 7420 6265 2061 2064 6966 6665  might be a diffe
-0000caa0: 7265 6e74 2064 696d 656e 7369 6f6e 2e0a  rent dimension..
-0000cab0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-0000cac0: 2073 616d 6520 6261 7365 2c20 6275 7420   same base, but 
-0000cad0: 616c 736f 2063 6f6e 7369 6465 7220 6465  also consider de
-0000cae0: 7269 7665 645f 6672 6f6d 5f2e 2e2e 0a20  rived_from_.... 
-0000caf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000cb00: 2020 206c 6173 745f 6261 7365 5f73 656c     last_base_sel
-0000cb10: 665f 6469 6d20 3d20 7365 6c66 0a20 2020  f_dim = self.   
-0000cb20: 2020 2020 2062 6173 6520 3d20 7365 6c66       base = self
-0000cb30: 0a20 2020 2020 2020 2076 6973 6974 6564  .        visited
-0000cb40: 203d 207b 7d0a 2020 2020 2020 2020 7768   = {}.        wh
-0000cb50: 696c 6520 6261 7365 2e73 616d 655f 6173  ile base.same_as
-0000cb60: 206f 7220 6261 7365 2e64 6572 6976 6564   or base.derived
-0000cb70: 5f66 726f 6d5f 7461 673a 0a20 2020 2020  _from_tag:.     
-0000cb80: 2020 2020 2020 2061 7373 6572 7420 6964         assert id
-0000cb90: 2862 6173 6529 206e 6f74 2069 6e20 7669  (base) not in vi
-0000cba0: 7369 7465 6420 2023 2073 686f 756c 6420  sited  # should 
-0000cbb0: 6e6f 7420 6861 7665 2063 7963 6c65 732e  not have cycles.
-0000cbc0: 206e 6f72 6d61 6c6c 7920 7468 6973 2073   normally this s
-0000cbd0: 686f 756c 6420 6e65 7665 7220 6265 2074  hould never be t
-0000cbe0: 7269 6767 6572 6564 0a20 2020 2020 2020  riggered.       
-0000cbf0: 2020 2020 2076 6973 6974 6564 5b69 6428       visited[id(
-0000cc00: 6261 7365 295d 203d 2062 6173 650a 2020  base)] = base.  
-0000cc10: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
-0000cc20: 652e 7361 6d65 5f61 733a 0a20 2020 2020  e.same_as:.     
-0000cc30: 2020 2020 2020 2020 2020 2062 6173 6520             base 
-0000cc40: 3d20 6261 7365 2e73 616d 655f 6173 0a20  = base.same_as. 
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000cc60: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-0000cc70: 2020 2020 6261 7365 203d 2062 6173 652e      base = base.
-0000cc80: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
-0000cc90: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000cca0: 6572 7420 6261 7365 0a20 2020 2020 2020  ert base.       
-0000ccb0: 2020 2020 2069 6620 6261 7365 2e64 696d       if base.dim
-0000ccc0: 656e 7369 6f6e 203d 3d20 7365 6c66 2e64  ension == self.d
-0000ccd0: 696d 656e 7369 6f6e 3a0a 2020 2020 2020  imension:.      
-0000cce0: 2020 2020 2020 2020 2020 6c61 7374 5f62            last_b
-0000ccf0: 6173 655f 7365 6c66 5f64 696d 203d 2062  ase_self_dim = b
-0000cd00: 6173 650a 2020 2020 2020 2020 7265 7475  ase.        retu
-0000cd10: 726e 206c 6173 745f 6261 7365 5f73 656c  rn last_base_sel
-0000cd20: 665f 6469 6d20 6966 2073 616d 655f 6469  f_dim if same_di
-0000cd30: 6d20 656c 7365 2062 6173 650a 0a20 2020  m else base..   
-0000cd40: 2064 6566 2067 6574 5f64 6572 6976 6564   def get_derived
-0000cd50: 5f62 6173 6573 5f73 6574 2873 656c 6629  _bases_set(self)
-0000cd60: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000cd70: 2020 2020 2020 3a72 7479 7065 3a20 7365        :rtype: se
-0000cd80: 745b 4469 6d5d 0a20 2020 2020 2020 2022  t[Dim].        "
-0000cd90: 2222 0a20 2020 2020 2020 2072 6573 203d  "".        res =
-0000cda0: 2073 6574 2829 0a20 2020 2020 2020 2071   set().        q
-0000cdb0: 7565 7565 203d 205b 7365 6c66 5d0a 2020  ueue = [self].  
-0000cdc0: 2020 2020 2020 7669 7369 7465 6420 3d20        visited = 
-0000cdd0: 7b7d 2020 2320 7479 7065 3a20 4469 6374  {}  # type: Dict
-0000cde0: 5b69 6e74 2c5f 642e 4469 6d5d 2020 2320  [int,_d.Dim]  # 
-0000cdf0: 6279 2069 640a 2020 2020 2020 2020 7768  by id.        wh
-0000ce00: 696c 6520 7175 6575 653a 0a20 2020 2020  ile queue:.     
-0000ce10: 2020 2020 2020 2062 6173 6520 3d20 7175         base = qu
-0000ce20: 6575 652e 706f 7028 2d31 290a 2020 2020  eue.pop(-1).    
-0000ce30: 2020 2020 2020 2020 6966 2062 6173 652e          if base.
-0000ce40: 7361 6d65 5f61 733a 0a20 2020 2020 2020  same_as:.       
-0000ce50: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0000ce60: 6261 7365 2e73 616d 655f 6173 0a20 2020  base.same_as.   
-0000ce70: 2020 2020 2020 2020 2069 6620 6964 2862           if id(b
-0000ce80: 6173 6529 2069 6e20 7669 7369 7465 643a  ase) in visited:
-0000ce90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cea0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-0000ceb0: 2020 2020 2020 7669 7369 7465 645b 6964        visited[id
-0000cec0: 2862 6173 6529 5d20 3d20 6261 7365 0a20  (base)] = base. 
-0000ced0: 2020 2020 2020 2020 2020 2072 6573 2e61             res.a
-0000cee0: 6464 2862 6173 6529 0a20 2020 2020 2020  dd(base).       
-0000cef0: 2020 2020 2069 6620 6261 7365 2e64 6572       if base.der
-0000cf00: 6976 6564 5f66 726f 6d5f 6f70 3a0a 2020  ived_from_op:.  
-0000cf10: 2020 2020 2020 2020 2020 2020 2020 7175                qu
-0000cf20: 6575 652e 6578 7465 6e64 2862 6173 652e  eue.extend(base.
-0000cf30: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-0000cf40: 696e 7075 7473 290a 2020 2020 2020 2020  inputs).        
-0000cf50: 2020 2020 656c 6966 2062 6173 652e 6465      elif base.de
-0000cf60: 7269 7665 645f 6672 6f6d 5f74 6167 3a0a  rived_from_tag:.
-0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf80: 7175 6575 652e 6170 7065 6e64 2862 6173  queue.append(bas
-0000cf90: 652e 6465 7269 7665 645f 6672 6f6d 5f74  e.derived_from_t
-0000cfa0: 6167 290a 2020 2020 2020 2020 7265 7475  ag).        retu
-0000cfb0: 726e 2072 6573 0a0a 2020 2020 4070 726f  rn res..    @pro
-0000cfc0: 7065 7274 790a 2020 2020 6465 6620 756e  perty.    def un
-0000cfd0: 6465 6669 6e65 6428 7365 6c66 3a20 5f64  defined(self: _d
-0000cfe0: 2e44 696d 2920 2d3e 2062 6f6f 6c3a 0a20  .Dim) -> bool:. 
-0000cff0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d000: 2020 203a 7265 7475 726e 3a20 7768 6574     :return: whet
-0000d010: 6865 7220 7468 6520 756e 6465 6669 6e65  her the undefine
-0000d020: 6420 666c 6167 2069 7320 7365 742c 2069  d flag is set, i
-0000d030: 6e20 7365 6c66 2c20 6261 7365 732c 206f  n self, bases, o
-0000d040: 7220 616e 7920 6465 7269 7665 6420 6261  r any derived ba
-0000d050: 7365 732e 2061 6c73 6f20 7365 6520 3a66  ses. also see :f
-0000d060: 756e 633a 6069 735f 6469 6d5f 6b6e 6f77  unc:`is_dim_know
-0000d070: 6e60 0a20 2020 2020 2020 2022 2222 0a20  n`.        """. 
-0000d080: 2020 2020 2020 2062 6173 6520 3d20 7365         base = se
-0000d090: 6c66 0a20 2020 2020 2020 2076 6973 6974  lf.        visit
-0000d0a0: 6564 203d 207b 7d0a 2020 2020 2020 2020  ed = {}.        
-0000d0b0: 7768 696c 6520 6261 7365 2e73 616d 655f  while base.same_
-0000d0c0: 6173 206f 7220 6261 7365 2e64 6572 6976  as or base.deriv
-0000d0d0: 6564 5f66 726f 6d5f 7461 673a 0a20 2020  ed_from_tag:.   
-0000d0e0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000d0f0: 6964 2862 6173 6529 206e 6f74 2069 6e20  id(base) not in 
-0000d100: 7669 7369 7465 6420 2023 2073 686f 756c  visited  # shoul
-0000d110: 6420 6e6f 7420 6861 7665 2063 7963 6c65  d not have cycle
-0000d120: 732e 206e 6f72 6d61 6c6c 7920 7468 6973  s. normally this
-0000d130: 2073 686f 756c 6420 6e65 7665 7220 6265   should never be
-0000d140: 2074 7269 6767 6572 6564 0a20 2020 2020   triggered.     
-0000d150: 2020 2020 2020 2076 6973 6974 6564 5b69         visited[i
-0000d160: 6428 6261 7365 295d 203d 2062 6173 650a  d(base)] = base.
-0000d170: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
-0000d180: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
-0000d190: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
-0000d1a0: 2020 2020 2020 2020 2069 6620 6261 7365           if base
-0000d1b0: 2e5f 6578 7472 6120 616e 6420 6261 7365  ._extra and base
-0000d1c0: 2e5f 6578 7472 612e 756e 6465 6669 6e65  ._extra.undefine
-0000d1d0: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
-0000d1e0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-0000d1f0: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
-0000d200: 7365 2e73 616d 655f 6173 3a0a 2020 2020  se.same_as:.    
-0000d210: 2020 2020 2020 2020 2020 2020 6261 7365              base
-0000d220: 203d 2062 6173 652e 7361 6d65 5f61 730a   = base.same_as.
-0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d240: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0000d250: 2020 2020 2062 6173 6520 3d20 6261 7365       base = base
-0000d260: 2e64 6572 6976 6564 5f66 726f 6d5f 7461  .derived_from_ta
-0000d270: 670a 2020 2020 2020 2020 2020 2020 6173  g.            as
-0000d280: 7365 7274 2062 6173 650a 2020 2020 2020  sert base.      
-0000d290: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
-0000d2a0: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
-0000d2b0: 6572 0a20 2020 2020 2020 2072 6574 7572  er.        retur
-0000d2c0: 6e20 6261 7365 2e5f 6578 7472 6120 616e  n base._extra an
-0000d2d0: 6420 6261 7365 2e5f 6578 7472 612e 756e  d base._extra.un
-0000d2e0: 6465 6669 6e65 640a 0a20 2020 2064 6566  defined..    def
-0000d2f0: 2064 6563 6c61 7265 5f73 616d 655f 6173   declare_same_as
-0000d300: 2873 656c 663a 205f 642e 4469 6d2c 206f  (self: _d.Dim, o
-0000d310: 7468 6572 3a20 5f64 2e44 696d 293a 0a20  ther: _d.Dim):. 
-0000d320: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d330: 2020 203a 7061 7261 6d20 6f74 6865 723a     :param other:
-0000d340: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d350: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0000d360: 2e63 616e 5f62 655f 7573 6564 5f61 735f  .can_be_used_as_
-0000d370: 6469 6d28 2920 616e 6420 6f74 6865 722e  dim() and other.
-0000d380: 6361 6e5f 6265 5f75 7365 645f 6173 5f64  can_be_used_as_d
-0000d390: 696d 2829 2020 2320 6465 636c 6172 655f  im()  # declare_
-0000d3a0: 7361 6d65 5f61 7320 646f 6573 206e 6f74  same_as does not
-0000d3b0: 206d 616b 6520 7365 6e73 6520 6f74 6865   make sense othe
-0000d3c0: 7277 6973 650a 2020 2020 2020 2020 2320  rwise.        # 
-0000d3d0: 4e6f 7465 3a20 4368 6563 6b20 6069 7360  Note: Check `is`
-0000d3e0: 2c20 6e6f 7420 603d 3d60 2e20 603d 3d60  , not `==`. `==`
-0000d3f0: 2063 616e 2062 6520 7472 7565 2065 7665   can be true eve
-0000d400: 6e20 7468 6f75 6768 2073 616d 655f 6173  n though same_as
-0000d410: 2061 7265 206e 6f74 2074 6865 2073 616d   are not the sam
-0000d420: 6520 696e 7374 616e 6365 2c0a 2020 2020  e instance,.    
-0000d430: 2020 2020 2320 652e 672e 2076 6961 2061      # e.g. via a
-0000d440: 7574 6f5f 6765 6e65 7261 7465 642e 0a20  uto_generated.. 
-0000d450: 2020 2020 2020 2069 6620 7365 6c66 2069         if self i
-0000d460: 7320 6f74 6865 723a 0a20 2020 2020 2020  s other:.       
-0000d470: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000d480: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
-0000d490: 7570 6461 7465 2829 0a20 2020 2020 2020  update().       
-0000d4a0: 2073 656c 662e 5f76 616c 6964 6174 655f   self._validate_
-0000d4b0: 696e 5f63 7572 7265 6e74 5f67 7261 7068  in_current_graph
-0000d4c0: 2829 0a20 2020 2020 2020 206f 7468 6572  ().        other
-0000d4d0: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
-0000d4e0: 7272 656e 745f 6772 6170 6828 290a 2020  rrent_graph().  
-0000d4f0: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
-0000d500: 5f62 6173 6520 3d20 6f74 6865 722e 6765  _base = other.ge
-0000d510: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-0000d520: 2020 2020 2020 6966 2073 656c 6620 6973        if self is
-0000d530: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000d540: 206f 7220 7365 6c66 2e73 616d 655f 6173   or self.same_as
-0000d550: 2069 7320 6f74 6865 725f 7361 6d65 5f62   is other_same_b
-0000d560: 6173 653a 0a20 2020 2020 2020 2020 2020  ase:.           
-0000d570: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000d580: 7365 6c66 5f73 616d 655f 6173 203d 2073  self_same_as = s
-0000d590: 656c 662e 6765 745f 7361 6d65 5f62 6173  elf.get_same_bas
-0000d5a0: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
-0000d5b0: 656c 665f 7361 6d65 5f61 7320 6973 206f  elf_same_as is o
-0000d5c0: 7468 6572 5f73 616d 655f 6261 7365 3a0a  ther_same_base:.
-0000d5d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d5e0: 726e 0a20 2020 2020 2020 2069 6620 6f74  rn.        if ot
-0000d5f0: 6865 725f 7361 6d65 5f62 6173 652e 6765  her_same_base.ge
-0000d600: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
-0000d610: 6173 6528 2920 6973 2073 656c 665f 7361  ase() is self_sa
-0000d620: 6d65 5f61 733a 0a20 2020 2020 2020 2020  me_as:.         
-0000d630: 2020 2023 2057 6520 6163 7475 616c 6c79     # We actually
-0000d640: 2077 616e 7420 6974 2074 6f20 6265 2074   want it to be t
-0000d650: 6865 206f 7468 6572 2077 6179 2061 726f  he other way aro
-0000d660: 756e 642e 0a20 2020 2020 2020 2020 2020  und..           
-0000d670: 2077 6974 6820 7574 696c 2e67 7561 7264   with util.guard
-0000d680: 5f69 6e66 696e 6974 655f 7265 6375 7273  _infinite_recurs
-0000d690: 696f 6e28 5f64 2e44 696d 2e64 6563 6c61  ion(_d.Dim.decla
-0000d6a0: 7265 5f73 616d 655f 6173 2c20 6f74 6865  re_same_as, othe
-0000d6b0: 722c 2073 656c 6629 3a0a 2020 2020 2020  r, self):.      
-0000d6c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d6d0: 206f 7468 6572 2e64 6563 6c61 7265 5f73   other.declare_s
-0000d6e0: 616d 655f 6173 2873 656c 6629 0a20 2020  ame_as(self).   
-0000d6f0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
-0000d700: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-0000d710: 2320 4966 2073 656c 6620 6973 2064 6566  # If self is def
-0000d720: 696e 6564 2028 7365 6c66 2e69 735f 6469  ined (self.is_di
-0000d730: 6d5f 6b6e 6f77 6e29 2c20 6265 2066 6169  m_known), be fai
-0000d740: 7220 746f 206f 7468 6572 2c20 616e 6420  r to other, and 
-0000d750: 6164 6170 7420 6974 2074 6f20 7468 6520  adapt it to the 
-0000d760: 7269 6768 7420 6261 7463 682c 0a20 2020  right batch,.   
-0000d770: 2020 2020 2020 2020 2023 2073 7563 6820           # such 
-0000d780: 7468 6174 206f 7468 6572 2e69 735f 6469  that other.is_di
-0000d790: 6d5f 6b6e 6f77 6e20 6973 2063 6f72 7265  m_known is corre
-0000d7a0: 6374 2c20 6279 2070 6f74 656e 7469 616c  ct, by potential
-0000d7b0: 6c79 2063 6f6d 706c 6574 696e 6720 6974  ly completing it
-0000d7c0: 2e0a 2020 2020 2020 2020 2020 2020 6f74  ..            ot
-0000d7d0: 6865 725f 203d 206f 7468 6572 2e67 6574  her_ = other.get
-0000d7e0: 5f66 6f72 5f62 6174 6368 5f63 7478 2873  _for_batch_ctx(s
-0000d7f0: 656c 662e 6261 7463 682c 2063 7478 3d73  elf.batch, ctx=s
-0000d800: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-0000d810: 5f63 7478 290a 2020 2020 2020 2020 656c  _ctx).        el
-0000d820: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000d830: 6f74 6865 725f 203d 206f 7468 6572 0a20  other_ = other. 
-0000d840: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-0000d850: 2020 2020 2020 2020 2873 656c 662e 6973          (self.is
-0000d860: 5f64 696d 5f6b 6e6f 776e 2829 2061 6e64  _dim_known() and
-0000d870: 206e 6f74 206f 7468 6572 5f2e 6973 5f64   not other_.is_d
-0000d880: 696d 5f6b 6e6f 776e 2829 290a 2020 2020  im_known()).    
-0000d890: 2020 2020 2020 2020 6f72 0a20 2020 2020          or.     
-0000d8a0: 2020 2020 2020 2023 204c 696b 6520 6973         # Like is
-0000d8b0: 5f64 696d 5f6b 6e6f 776e 2062 7574 2066  _dim_known but f
-0000d8c0: 6f72 2073 7461 7469 6320 6469 6d73 2c20  or static dims, 
-0000d8d0: 7765 206d 6967 6874 206b 6e6f 7720 626f  we might know bo
-0000d8e0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-0000d8f0: 2320 6275 7420 7468 6520 6465 7269 7665  # but the derive
-0000d900: 645f 6672 6f6d 5f6f 7020 7374 696c 6c20  d_from_op still 
-0000d910: 776f 756c 6420 7072 6f76 6964 6520 6d6f  would provide mo
-0000d920: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0a  re information..
-0000d930: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
-0000d940: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d950: 6c66 5f73 616d 655f 6173 2e64 6572 6976  lf_same_as.deriv
-0000d960: 6564 5f66 726f 6d5f 6f70 0a20 2020 2020  ed_from_op.     
-0000d970: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
-0000d980: 6f74 206f 7468 6572 5f73 616d 655f 6261  ot other_same_ba
-0000d990: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
-0000d9a0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-0000d9b0: 2020 2061 6e64 206f 7468 6572 206e 6f74     and other not
-0000d9c0: 2069 6e20 7365 6c66 2e67 6574 5f64 6572   in self.get_der
-0000d9d0: 6976 6564 5f62 6173 6573 5f73 6574 2829  ived_bases_set()
-0000d9e0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000d9f0: 2020 2020 2020 2020 2020 206f 7220 286e             or (n
-0000da00: 6f74 2073 656c 662e 756e 6465 6669 6e65  ot self.undefine
-0000da10: 6420 616e 6420 6f74 6865 725f 2e75 6e64  d and other_.und
-0000da20: 6566 696e 6564 290a 2020 2020 2020 2020  efined).        
-0000da30: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
-0000da40: 6974 6820 7574 696c 2e67 7561 7264 5f69  ith util.guard_i
-0000da50: 6e66 696e 6974 655f 7265 6375 7273 696f  nfinite_recursio
-0000da60: 6e28 5f64 2e44 696d 2e64 6563 6c61 7265  n(_d.Dim.declare
-0000da70: 5f73 616d 655f 6173 2c20 6f74 6865 722c  _same_as, other,
-0000da80: 2073 656c 6629 3a0a 2020 2020 2020 2020   self):.        
-0000da90: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0000daa0: 7468 6572 2e64 6563 6c61 7265 5f73 616d  ther.declare_sam
-0000dab0: 655f 6173 2873 656c 6629 0a20 2020 2020  e_as(self).     
-0000dac0: 2020 206f 7468 6572 5f64 6572 6976 6564     other_derived
-0000dad0: 5f62 6173 6573 203d 206f 7468 6572 2e67  _bases = other.g
-0000dae0: 6574 5f64 6572 6976 6564 5f62 6173 6573  et_derived_bases
-0000daf0: 5f73 6574 2829 0a20 2020 2020 2020 2073  _set().        s
-0000db00: 656c 665f 6465 7269 7665 645f 6261 7365  elf_derived_base
-0000db10: 7320 3d20 7365 6c66 2e67 6574 5f64 6572  s = self.get_der
-0000db20: 6976 6564 5f62 6173 6573 5f73 6574 2829  ived_bases_set()
-0000db30: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-0000db40: 725f 6465 7269 7665 645f 6261 7365 7320  r_derived_bases 
-0000db50: 213d 2073 656c 665f 6465 7269 7665 645f  != self_derived_
-0000db60: 6261 7365 7320 616e 6420 7365 6c66 5f64  bases and self_d
-0000db70: 6572 6976 6564 5f62 6173 6573 2e69 7373  erived_bases.iss
-0000db80: 7562 7365 7428 6f74 6865 725f 6465 7269  ubset(other_deri
-0000db90: 7665 645f 6261 7365 7329 3a0a 2020 2020  ved_bases):.    
-0000dba0: 2020 2020 2020 2020 2320 4176 6f69 6420          # Avoid 
-0000dbb0: 6379 636c 6573 206f 6e20 6465 7269 7665  cycles on derive
-0000dbc0: 645f 6672 6f6d 5f74 6167 2e20 6874 7470  d_from_tag. http
-0000dbd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-0000dbe0: 7774 682d 6936 2f72 6574 7572 6e6e 2f69  wth-i6/returnn/i
-0000dbf0: 7373 7565 732f 3130 3534 0a20 2020 2020  ssues/1054.     
-0000dc00: 2020 2020 2020 2077 6974 6820 7574 696c         with util
-0000dc10: 2e67 7561 7264 5f69 6e66 696e 6974 655f  .guard_infinite_
-0000dc20: 7265 6375 7273 696f 6e28 5f64 2e44 696d  recursion(_d.Dim
-0000dc30: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
-0000dc40: 2c20 6f74 6865 722c 2073 656c 6629 3a0a  , other, self):.
-0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc60: 7265 7475 726e 206f 7468 6572 2e64 6563  return other.dec
-0000dc70: 6c61 7265 5f73 616d 655f 6173 2873 656c  lare_same_as(sel
-0000dc80: 6629 0a20 2020 2020 2020 2069 6620 7365  f).        if se
-0000dc90: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
-0000dca0: 2020 2020 2020 2073 656c 662e 5f65 7874         self._ext
-0000dcb0: 7261 2e64 6572 6976 6564 5f66 726f 6d5f  ra.derived_from_
-0000dcc0: 6f70 203d 204e 6f6e 650a 2020 2020 2020  op = None.      
-0000dcd0: 2020 2020 2020 7365 6c66 2e5f 6578 7472        self._extr
-0000dce0: 612e 6465 7269 7665 645f 6672 6f6d 5f74  a.derived_from_t
-0000dcf0: 6167 203d 204e 6f6e 650a 2020 2020 2020  ag = None.      
-0000dd00: 2020 6966 2073 656c 665f 7361 6d65 5f61    if self_same_a
-0000dd10: 7320 6973 206e 6f74 2073 656c 663a 0a20  s is not self:. 
-0000dd20: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000dd30: 7420 6e6f 7420 7365 6c66 5f73 616d 655f  t not self_same_
-0000dd40: 6173 2e73 616d 655f 6173 0a20 2020 2020  as.same_as.     
-0000dd50: 2020 2020 2020 2069 6620 7365 6c66 5f73         if self_s
-0000dd60: 616d 655f 6173 2069 7320 6f74 6865 725f  ame_as is other_
-0000dd70: 7361 6d65 5f62 6173 653a 0a20 2020 2020  same_base:.     
-0000dd80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000dd90: 6e0a 2020 2020 2020 2020 2020 2020 7769  n.            wi
-0000dda0: 7468 2075 7469 6c2e 6775 6172 645f 696e  th util.guard_in
-0000ddb0: 6669 6e69 7465 5f72 6563 7572 7369 6f6e  finite_recursion
-0000ddc0: 285f 642e 4469 6d2e 6465 636c 6172 655f  (_d.Dim.declare_
-0000ddd0: 7361 6d65 5f61 732c 2073 656c 665f 7361  same_as, self_sa
-0000dde0: 6d65 5f61 732c 206f 7468 6572 5f73 616d  me_as, other_sam
-0000ddf0: 655f 6261 7365 293a 0a20 2020 2020 2020  e_base):.       
-0000de00: 2020 2020 2020 2020 2073 656c 665f 7361           self_sa
-0000de10: 6d65 5f61 732e 6465 636c 6172 655f 7361  me_as.declare_sa
-0000de20: 6d65 5f61 7328 6f74 6865 725f 7361 6d65  me_as(other_same
-0000de30: 5f62 6173 6529 0a20 2020 2020 2020 2020  _base).         
-0000de40: 2020 2069 6620 2873 656c 662e 6479 6e5f     if (self.dyn_
-0000de50: 7369 7a65 5f65 7874 2069 7320 4e6f 6e65  size_ext is None
-0000de60: 206f 7220 6e6f 7420 7365 6c66 2e5f 7661   or not self._va
-0000de70: 6c69 6461 7465 5f69 6e5f 6375 7272 656e  lidate_in_curren
-0000de80: 745f 6772 6170 6828 2929 2061 6e64 2073  t_graph()) and s
-0000de90: 656c 665f 7361 6d65 5f61 732e 6479 6e5f  elf_same_as.dyn_
-0000dea0: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-0000deb0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000dec0: 796e 5f73 697a 655f 6578 7420 3d20 7365  yn_size_ext = se
-0000ded0: 6c66 5f73 616d 655f 6173 2e67 6574 5f64  lf_same_as.get_d
-0000dee0: 796e 5f73 697a 655f 6578 745f 666f 725f  yn_size_ext_for_
-0000def0: 6261 7463 685f 6374 7828 0a20 2020 2020  batch_ctx(.     
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000df10: 656c 662e 6261 7463 682c 2073 656c 662e  elf.batch, self.
-0000df20: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-0000df30: 2c20 7465 6d70 6c61 7465 5f6f 6e6c 793d  , template_only=
-0000df40: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000df50: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-0000df60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000df70: 2069 6620 7365 6c66 2e5f 6578 7472 613a   if self._extra:
-0000df80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df90: 2066 6f72 2064 696d 5f20 696e 2073 656c   for dim_ in sel
-0000dfa0: 662e 5f65 7874 7261 2e73 616d 655f 666f  f._extra.same_fo
-0000dfb0: 725f 6261 7463 685f 6374 782e 7661 6c75  r_batch_ctx.valu
-0000dfc0: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
-0000dfd0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
-0000dfe0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-0000dff0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-0000e000: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e010: 6620 6469 6d5f 2e5f 6578 7472 613a 0a20  f dim_._extra:. 
-0000e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e030: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
-0000e040: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
-0000e050: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
-0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e070: 6469 6d5f 2e5f 6578 7472 612e 6465 7269  dim_._extra.deri
-0000e080: 7665 645f 6672 6f6d 5f6f 7020 3d20 4e6f  ved_from_op = No
-0000e090: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000e0a0: 2020 2020 2020 2020 2020 2023 206e 6f69             # noi
-0000e0b0: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
-0000e0c0: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0e0: 2020 2020 6469 6d5f 2e5f 6578 7472 612e      dim_._extra.
-0000e0f0: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
-0000e100: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000e110: 2320 4e6f 7720 6d65 7267 6520 6578 6973  # Now merge exis
-0000e120: 7469 6e67 2076 6172 6961 6e74 732e 2042  ting variants. B
-0000e130: 7574 206f 6e6c 7920 6966 206e 6f74 2064  ut only if not d
-0000e140: 6572 6976 6564 2076 6961 206f 702c 2062  erived via op, b
-0000e150: 6563 6175 7365 2069 6e20 7468 6174 2063  ecause in that c
-0000e160: 6173 652c 2077 6520 6361 6e20 2861 6e64  ase, we can (and
-0000e170: 2073 686f 756c 6421 290a 2020 2020 2020   should!).      
-0000e180: 2020 2320 6175 746f 6d61 7469 6361 6c6c    # automaticall
-0000e190: 7920 696e 6665 7220 6974 2e20 4e6f 7465  y infer it. Note
-0000e1a0: 2074 6861 7420 7765 206f 6e6c 7920 676f   that we only go
-0000e1b0: 7420 6865 7265 2077 6865 6e20 7468 6520  t here when the 
-0000e1c0: 6f74 6865 7220 6973 206e 6f74 2074 6865  other is not the
-0000e1d0: 2073 616d 6520 6469 6d2c 2073 6f20 6974   same dim, so it
-0000e1e0: 206d 6561 6e73 2074 6861 740a 2020 2020   means that.    
-0000e1f0: 2020 2020 2320 7468 6520 6f74 6865 7220      # the other 
-0000e200: 6973 2072 6561 6c6c 7920 6469 6666 6572  is really differ
-0000e210: 656e 742c 2074 6865 2073 697a 6573 2061  ent, the sizes a
-0000e220: 7265 2070 6f74 656e 7469 616c 6c79 2064  re potentially d
-0000e230: 6966 6665 7265 6e74 2c20 6275 7420 7765  ifferent, but we
-0000e240: 2077 616e 7420 746f 206f 7665 7274 616b   want to overtak
-0000e250: 6520 7468 6520 6f74 6865 722e 0a20 2020  e the other..   
-0000e260: 2020 2020 2069 6620 6f74 6865 725f 7361       if other_sa
-0000e270: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
-0000e280: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
-0000e290: 2020 2020 2023 2043 6c65 616e 7570 2065       # Cleanup e
-0000e2a0: 7665 7279 7468 696e 672c 2065 7370 2070  verything, esp p
-0000e2b0: 6f74 656e 7469 616c 2061 6c72 6561 6479  otential already
-0000e2c0: 2063 6f6d 7075 7465 6420 7369 7a65 732c   computed sizes,
-0000e2d0: 2061 7320 7468 6573 6520 6d69 6768 7420   as these might 
-0000e2e0: 6265 2069 6e76 616c 6964 2e0a 2020 2020  be invalid..    
-0000e2f0: 2020 2020 2020 2020 666f 7220 6469 6d5f          for dim_
-0000e300: 2069 6e20 5b73 656c 665f 7361 6d65 5f61   in [self_same_a
-0000e310: 732c 2073 656c 665d 202b 2028 6c69 7374  s, self] + (list
-0000e320: 2873 656c 662e 5f65 7874 7261 2e73 616d  (self._extra.sam
-0000e330: 655f 666f 725f 6261 7463 685f 6374 782e  e_for_batch_ctx.
-0000e340: 7661 6c75 6573 2829 2920 6966 2073 656c  values()) if sel
-0000e350: 662e 5f65 7874 7261 2065 6c73 6520 5b5d  f._extra else []
-0000e360: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000e370: 2020 2069 6620 6469 6d5f 2e64 796e 5f73     if dim_.dyn_s
-0000e380: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
-0000e390: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-0000e3a0: 5f2e 6479 6e5f 7369 7a65 5f65 7874 2e70  _.dyn_size_ext.p
-0000e3b0: 6c61 6365 686f 6c64 6572 203d 204e 6f6e  laceholder = Non
-0000e3c0: 650a 2020 2020 2020 2020 6f74 6865 725f  e.        other_
-0000e3d0: 7361 6d65 5f62 6173 652e 5f6d 6572 6765  same_base._merge
-0000e3e0: 5f73 616d 655f 666f 725f 6261 7463 685f  _same_for_batch_
-0000e3f0: 6374 785f 6469 6374 2873 656c 6629 0a20  ctx_dict(self). 
-0000e400: 2020 2020 2020 206f 7468 6572 2e5f 6d61         other._ma
-0000e410: 7962 655f 7570 6461 7465 2829 0a20 2020  ybe_update().   
-0000e420: 2020 2020 2073 656c 662e 7361 6d65 5f61       self.same_a
-0000e430: 7320 3d20 6f74 6865 725f 7361 6d65 5f62  s = other_same_b
-0000e440: 6173 650a 2020 2020 2020 2020 7365 6c66  ase.        self
-0000e450: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
-0000e460: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000e470: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
-0000e480: 204e 6f6e 6520 616e 6420 6f74 6865 725f   None and other_
-0000e490: 7361 6d65 5f62 6173 652e 6479 6e5f 7369  same_base.dyn_si
-0000e4a0: 7a65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ze is not None:.
-0000e4b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000e4c0: 656c 662e 6479 6e5f 7369 7a65 2069 7320  elf.dyn_size is 
-0000e4d0: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
-0000e4e0: 6173 652e 6479 6e5f 7369 7a65 3a0a 2020  ase.dyn_size:.  
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000e500: 2073 656c 662e 6261 7463 6820 3d3d 206f   self.batch == o
-0000e510: 7468 6572 5f73 616d 655f 6261 7365 2e62  ther_same_base.b
-0000e520: 6174 6368 2061 6e64 2073 656c 662e 636f  atch and self.co
-0000e530: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
-0000e540: 3d20 6f74 6865 725f 7361 6d65 5f62 6173  = other_same_bas
-0000e550: 652e 636f 6e74 726f 6c5f 666c 6f77 5f63  e.control_flow_c
-0000e560: 7478 3a0a 2020 2020 2020 2020 2020 2020  tx:.            
-0000e570: 2020 2020 2020 2020 2320 4e6f 7465 3a20          # Note: 
-0000e580: 496e 7374 6561 6420 6f66 206d 616b 696e  Instead of makin
-0000e590: 6720 7468 6973 2061 2077 6172 6e69 6e67  g this a warning
-0000e5a0: 2c20 7765 2063 6f75 6c64 2061 6c73 6f20  , we could also 
-0000e5b0: 656e 666f 7263 6520 7468 6973 2061 7420  enforce this at 
-0000e5c0: 736f 6d65 2070 6f69 6e74 2e0a 2020 2020  some point..    
-0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5e0: 2320 2020 5468 6520 7573 6572 2073 686f  #   The user sho
-0000e5f0: 756c 6420 6265 2061 626c 6520 746f 2066  uld be able to f
-0000e600: 6978 2060 6578 7465 726e 5f64 6174 6160  ix `extern_data`
-0000e610: 2069 6e20 7468 6520 636f 6e66 6967 0a20   in the config. 
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 2020 2023 2020 2073 7563 6820 7468 6174     #   such that
-0000e640: 2074 6869 7320 6973 2063 6f72 7265 6374   this is correct
-0000e650: 2069 6e20 7468 6520 6669 7273 7420 706c   in the first pl
-0000e660: 6163 652e 0a20 2020 2020 2020 2020 2020  ace..           
-0000e670: 2020 2020 2020 2020 2023 2020 2041 6c73           #   Als
-0000e680: 6f2c 2069 6e20 6164 6469 7469 6f6e 2074  o, in addition t
-0000e690: 6f20 7468 6973 2077 6172 6e69 6e67 2c0a  o this warning,.
-0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6b0: 2020 2020 2320 2020 7765 206d 6967 6874      #   we might
-0000e6c0: 2077 616e 7420 746f 2061 6464 2073 6f6d   want to add som
-0000e6d0: 6520 7275 6e74 696d 6520 6368 6563 6b20  e runtime check 
-0000e6e0: 6f6e 2074 6865 2065 7120 6f66 2074 6865  on the eq of the
-0000e6f0: 2064 796e 2073 697a 6573 2e0a 2020 2020   dyn sizes..    
-0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e710: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e730: 5761 726e 696e 673a 2061 7373 756d 696e  Warning: assumin
-0000e740: 6720 6469 6d20 7461 6773 2061 7265 2073  g dim tags are s
-0000e750: 616d 6520 7769 7468 2064 6966 6665 7265  ame with differe
-0000e760: 6e74 2073 697a 6520 706c 6163 6568 6f6c  nt size placehol
-0000e770: 6465 7273 3a20 2572 2076 7320 2572 220a  ders: %r vs %r".
-0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e790: 2020 2020 2020 2020 2520 2873 656c 662e          % (self.
-0000e7a0: 6479 6e5f 7369 7a65 2c20 6f74 6865 725f  dyn_size, other_
-0000e7b0: 7361 6d65 5f62 6173 652e 6479 6e5f 7369  same_base.dyn_si
-0000e7c0: 7a65 290a 2020 2020 2020 2020 2020 2020  ze).            
-0000e7d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000e7e0: 2020 2320 4966 2077 6520 6861 7665 2061    # If we have a
-0000e7f0: 2064 6566 696e 6564 2073 6f75 7263 652c   defined source,
-0000e800: 2061 6e64 2074 6869 7320 6973 2061 2064   and this is a d
-0000e810: 796e 616d 6963 2073 7061 7469 616c 2061  ynamic spatial a
-0000e820: 7869 732c 2061 6e64 2069 7420 7761 7320  xis, and it was 
-0000e830: 756e 6465 6669 6e65 6420 6265 666f 7265  undefined before
-0000e840: 2c0a 2020 2020 2020 2020 2320 6d61 7962  ,.        # mayb
-0000e850: 6520 7765 2063 616e 206f 7665 7274 616b  e we can overtak
-0000e860: 6520 7468 6520 7369 7a65 5f70 6c61 6365  e the size_place
-0000e870: 686f 6c64 6572 206e 6f77 2e0a 2020 2020  holder now..    
-0000e880: 2020 2020 6966 206f 7468 6572 5f73 616d      if other_sam
-0000e890: 655f 6261 7365 2e64 796e 5f73 697a 6520  e_base.dyn_size 
-0000e8a0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0000e8b0: 7365 6c66 2e5f 6578 7472 6120 616e 6420  self._extra and 
-0000e8c0: 7365 6c66 2e5f 6578 7472 612e 7372 635f  self._extra.src_
-0000e8d0: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-0000e8e0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-0000e8f0: 6e63 6528 7365 6c66 2e5f 6578 7472 612e  nce(self._extra.
-0000e900: 7372 635f 6178 6973 2c20 696e 7429 0a20  src_axis, int). 
-0000e910: 2020 2020 2020 2020 2020 2023 204d 6179             # May
-0000e920: 6265 2069 7420 6368 616e 6765 6420 696e  be it changed in
-0000e930: 2074 6865 206d 6561 6e77 6869 6c65 2c20   the meanwhile, 
-0000e940: 736f 2063 6865 636b 2e0a 2020 2020 2020  so check..      
-0000e950: 2020 2020 2020 7461 6720 3d20 7365 6c66        tag = self
-0000e960: 2e5f 6578 7472 612e 7372 635f 6461 7461  ._extra.src_data
-0000e970: 2e67 6574 5f64 696d 5f74 6167 2873 656c  .get_dim_tag(sel
-0000e980: 662e 5f65 7874 7261 2e73 7263 5f61 7869  f._extra.src_axi
-0000e990: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
-0000e9a0: 6620 7461 672e 6465 7363 7269 7074 696f  f tag.descriptio
-0000e9b0: 6e20 3d3d 2073 656c 662e 6465 7363 7269  n == self.descri
-0000e9c0: 7074 696f 6e20 616e 6420 286e 6f74 2074  ption and (not t
-0000e9d0: 6167 2e64 796e 5f73 697a 655f 6578 7420  ag.dyn_size_ext 
-0000e9e0: 6f72 206e 6f74 2074 6167 2e5f 7661 6c69  or not tag._vali
-0000e9f0: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000ea00: 6772 6170 6828 2929 3a0a 2020 2020 2020  graph()):.      
-0000ea10: 2020 2020 2020 2020 2020 7461 672e 6479            tag.dy
-0000ea20: 6e5f 7369 7a65 5f65 7874 203d 2073 656c  n_size_ext = sel
-0000ea30: 662e 6765 745f 6479 6e5f 7369 7a65 5f65  f.get_dyn_size_e
-0000ea40: 7874 5f66 6f72 5f62 6174 6368 5f63 7478  xt_for_batch_ctx
-0000ea50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ea60: 2020 2020 2020 7461 672e 6261 7463 682c        tag.batch,
-0000ea70: 2074 6167 2e63 6f6e 7472 6f6c 5f66 6c6f   tag.control_flo
-0000ea80: 775f 6374 782c 2074 656d 706c 6174 655f  w_ctx, template_
-0000ea90: 6f6e 6c79 3d54 7275 650a 2020 2020 2020  only=True.      
-0000eaa0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000eab0: 2020 2020 2020 2020 2020 2020 7461 672e              tag.
-0000eac0: 5f6d 6179 6265 5f75 7064 6174 6528 290a  _maybe_update().
-0000ead0: 2020 2020 2020 2020 2320 4966 206f 7468          # If oth
-0000eae0: 6572 7320 6479 6e5f 7369 7a65 2069 7320  ers dyn_size is 
-0000eaf0: 4e6f 6e65 2062 7574 2077 6520 6861 7665  None but we have
-0000eb00: 2061 2064 796e 5f73 697a 652c 206d 6179   a dyn_size, may
-0000eb10: 6265 2075 7064 6174 6520 6f74 6865 7273  be update others
-0000eb20: 2064 796e 5f73 697a 652e 0a20 2020 2020   dyn_size..     
-0000eb30: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
-0000eb40: 697a 6520 6973 206e 6f74 204e 6f6e 6520  ize is not None 
-0000eb50: 616e 6420 6f74 6865 725f 7361 6d65 5f62  and other_same_b
-0000eb60: 6173 652e 6479 6e5f 7369 7a65 2069 7320  ase.dyn_size is 
-0000eb70: 6e6f 7420 7365 6c66 2e64 796e 5f73 697a  not self.dyn_siz
-0000eb80: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0000eb90: 2043 6f75 6c64 2062 6520 756e 7365 7420   Could be unset 
-0000eba0: 6966 2069 7420 636f 6d65 7320 6672 6f6d  if it comes from
-0000ebb0: 2074 6865 2063 6f6e 6669 672c 206f 7220   the config, or 
-0000ebc0: 6672 6f6d 2070 7265 7620 6772 6170 6820  from prev graph 
-0000ebd0: 6372 6561 7469 6f6e 2e0a 2020 2020 2020  creation..      
-0000ebe0: 2020 2020 2020 2320 5468 6973 2069 7320        # This is 
-0000ebf0: 696d 706f 7274 616e 7420 7375 6368 2074  important such t
-0000ec00: 6861 7420 7365 6c66 2e63 616e 5f63 6f6d  hat self.can_com
-0000ec10: 7061 7265 2829 2069 7320 7361 6e65 2e0a  pare() is sane..
-0000ec20: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-0000ec30: 7468 6572 5f73 616d 655f 6261 7365 2e64  ther_same_base.d
-0000ec40: 796e 5f73 697a 6520 6973 204e 6f6e 6520  yn_size is None 
-0000ec50: 6f72 206e 6f74 206f 7468 6572 5f73 616d  or not other_sam
-0000ec60: 655f 6261 7365 2e5f 7661 6c69 6461 7465  e_base._validate
-0000ec70: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
-0000ec80: 6828 293a 0a20 2020 2020 2020 2020 2020  h():.           
-0000ec90: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
-0000eca0: 6261 7365 2e64 796e 5f73 697a 655f 6578  base.dyn_size_ex
-0000ecb0: 7420 3d20 7365 6c66 2e67 6574 5f64 796e  t = self.get_dyn
-0000ecc0: 5f73 697a 655f 6578 745f 666f 725f 6261  _size_ext_for_ba
-0000ecd0: 7463 685f 6374 7828 0a20 2020 2020 2020  tch_ctx(.       
-0000ece0: 2020 2020 2020 2020 2020 2020 206f 7468               oth
-0000ecf0: 6572 5f73 616d 655f 6261 7365 2e62 6174  er_same_base.bat
-0000ed00: 6368 2c20 6f74 6865 725f 7361 6d65 5f62  ch, other_same_b
-0000ed10: 6173 652e 636f 6e74 726f 6c5f 666c 6f77  ase.control_flow
-0000ed20: 5f63 7478 2c20 7465 6d70 6c61 7465 5f6f  _ctx, template_o
-0000ed30: 6e6c 793d 5472 7565 0a20 2020 2020 2020  nly=True.       
-0000ed40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000ed50: 2020 2020 2020 2020 2020 206f 7468 6572             other
-0000ed60: 5f73 616d 655f 6261 7365 2e5f 6d61 7962  _same_base._mayb
-0000ed70: 655f 7570 6461 7465 2829 0a20 2020 2020  e_update().     
-0000ed80: 2020 2069 6620 6e6f 7420 7365 6c66 2e64     if not self.d
-0000ed90: 796e 5f73 697a 655f 6578 7420 6f72 206e  yn_size_ext or n
-0000eda0: 6f74 2073 656c 662e 5f76 616c 6964 6174  ot self._validat
-0000edb0: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
-0000edc0: 7068 2829 3a0a 2020 2020 2020 2020 2020  ph():.          
-0000edd0: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-0000ede0: 6578 7420 3d20 6f74 6865 725f 7361 6d65  ext = other_same
-0000edf0: 5f62 6173 652e 6765 745f 6479 6e5f 7369  _base.get_dyn_si
-0000ee00: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
-0000ee10: 5f63 7478 280a 2020 2020 2020 2020 2020  _ctx(.          
-0000ee20: 2020 2020 2020 7365 6c66 2e62 6174 6368        self.batch
-0000ee30: 2c20 7365 6c66 2e63 6f6e 7472 6f6c 5f66  , self.control_f
-0000ee40: 6c6f 775f 6374 782c 2074 656d 706c 6174  low_ctx, templat
-0000ee50: 655f 6f6e 6c79 3d54 7275 650a 2020 2020  e_only=True.    
-0000ee60: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000ee70: 2020 2020 2020 7365 6c66 2e5f 6d61 7962        self._mayb
-0000ee80: 655f 7570 6461 7465 2829 0a20 2020 2020  e_update().     
-0000ee90: 2020 2065 6c69 6620 6f74 6865 725f 7361     elif other_sa
-0000eea0: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
-0000eeb0: 5f65 7874 2069 7320 4e6f 6e65 206f 7220  _ext is None or 
-0000eec0: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
-0000eed0: 6173 652e 5f76 616c 6964 6174 655f 696e  ase._validate_in
-0000eee0: 5f63 7572 7265 6e74 5f67 7261 7068 2829  _current_graph()
-0000eef0: 3a0a 2020 2020 2020 2020 2020 2020 6f74  :.            ot
-0000ef00: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
-0000ef10: 6e5f 7369 7a65 5f65 7874 203d 2073 656c  n_size_ext = sel
-0000ef20: 662e 6765 745f 6479 6e5f 7369 7a65 5f65  f.get_dyn_size_e
-0000ef30: 7874 5f66 6f72 5f62 6174 6368 5f63 7478  xt_for_batch_ctx
-0000ef40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ef50: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
-0000ef60: 652e 6261 7463 682c 206f 7468 6572 5f73  e.batch, other_s
-0000ef70: 616d 655f 6261 7365 2e63 6f6e 7472 6f6c  ame_base.control
-0000ef80: 5f66 6c6f 775f 6374 782c 2074 656d 706c  _flow_ctx, templ
-0000ef90: 6174 655f 6f6e 6c79 3d54 7275 650a 2020  ate_only=True.  
-0000efa0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000efb0: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
-0000efc0: 6d65 5f62 6173 652e 5f6d 6179 6265 5f75  me_base._maybe_u
-0000efd0: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
-0000efe0: 6966 2073 656c 662e 6973 5f64 696d 5f6b  if self.is_dim_k
-0000eff0: 6e6f 776e 2829 2061 6e64 206f 7468 6572  nown() and other
-0000f000: 2e69 735f 6469 6d5f 6b6e 6f77 6e28 293a  .is_dim_known():
-0000f010: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000f020: 6572 7420 7365 6c66 2e64 696d 656e 7369  ert self.dimensi
-0000f030: 6f6e 203d 3d20 6f74 6865 722e 6469 6d65  on == other.dime
-0000f040: 6e73 696f 6e0a 2020 2020 2020 2020 656c  nsion.        el
-0000f050: 6966 2073 656c 662e 6973 5f64 696d 5f6b  if self.is_dim_k
-0000f060: 6e6f 776e 2829 2061 6e64 206e 6f74 206f  nown() and not o
-0000f070: 7468 6572 2e69 735f 6469 6d5f 6b6e 6f77  ther.is_dim_know
-0000f080: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-0000f090: 206f 7468 6572 2e63 6170 6163 6974 7920   other.capacity 
-0000f0a0: 3d20 7365 6c66 2e63 6170 6163 6974 790a  = self.capacity.
-0000f0b0: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-0000f0c0: 722e 7369 7a65 203d 2073 656c 662e 7369  r.size = self.si
-0000f0d0: 7a65 0a20 2020 2020 2020 2065 6c69 6620  ze.        elif 
-0000f0e0: 6e6f 7420 7365 6c66 2e69 735f 6469 6d5f  not self.is_dim_
-0000f0f0: 6b6e 6f77 6e28 2920 616e 6420 6f74 6865  known() and othe
-0000f100: 722e 6973 5f64 696d 5f6b 6e6f 776e 2829  r.is_dim_known()
-0000f110: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000f120: 6c66 2e63 6170 6163 6974 7920 3d20 6f74  lf.capacity = ot
-0000f130: 6865 722e 6361 7061 6369 7479 0a20 2020  her.capacity.   
-0000f140: 2020 2020 2020 2020 2073 656c 662e 7369           self.si
-0000f150: 7a65 203d 206f 7468 6572 2e73 697a 650a  ze = other.size.
-0000f160: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f170: 766f 6361 6220 616e 6420 6e6f 7420 6f74  vocab and not ot
-0000f180: 6865 725f 7361 6d65 5f62 6173 652e 766f  her_same_base.vo
-0000f190: 6361 623a 0a20 2020 2020 2020 2020 2020  cab:.           
-0000f1a0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000f1b0: 2e76 6f63 6162 203d 2073 656c 662e 766f  .vocab = self.vo
-0000f1c0: 6361 620a 2020 2020 2020 2020 656c 6966  cab.        elif
-0000f1d0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000f1e0: 2e76 6f63 6162 2061 6e64 206e 6f74 2073  .vocab and not s
-0000f1f0: 656c 662e 766f 6361 623a 0a20 2020 2020  elf.vocab:.     
-0000f200: 2020 2020 2020 2073 656c 662e 766f 6361         self.voca
-0000f210: 6220 3d20 6f74 6865 725f 7361 6d65 5f62  b = other_same_b
-0000f220: 6173 652e 766f 6361 620a 2020 2020 2020  ase.vocab.      
-0000f230: 2020 7365 6c66 2e5f 6d61 6b65 5f65 7874    self._make_ext
-0000f240: 7261 2829 0a20 2020 2020 2020 2073 656c  ra().        sel
-0000f250: 665f 7361 6d65 5f61 732e 5f6d 616b 655f  f_same_as._make_
-0000f260: 6578 7472 6128 290a 2020 2020 2020 2020  extra().        
-0000f270: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
-0000f280: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
-0000f290: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
-0000f2a0: 7874 7261 2e61 7574 6f5f 6765 6e65 7261  xtra.auto_genera
-0000f2b0: 7465 6420 3d20 7365 6c66 5f73 616d 655f  ted = self_same_
-0000f2c0: 6173 2e5f 6578 7472 612e 6175 746f 5f67  as._extra.auto_g
-0000f2d0: 656e 6572 6174 6564 203d 206f 7468 6572  enerated = other
-0000f2e0: 5f73 616d 655f 6261 7365 2e61 7574 6f5f  _same_base.auto_
-0000f2f0: 6765 6e65 7261 7465 640a 2020 2020 2020  generated.      
-0000f300: 2020 2320 5461 6b65 206f 7665 7220 6465    # Take over de
-0000f310: 7269 7665 645f 6672 6f6d 5f6f 702e 2048  rived_from_op. H
-0000f320: 6f77 6576 6572 2c20 6f6e 6c79 2069 6620  owever, only if 
-0000f330: 7468 6973 2077 6f75 6c64 206e 6f74 2069  this would not i
-0000f340: 6e74 726f 6475 6365 2063 7963 6c65 7321  ntroduce cycles!
-0000f350: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000f360: 7365 6c66 5f64 6572 6976 6564 5f62 6173  self_derived_bas
-0000f370: 6573 2e69 7373 7570 6572 7365 7428 6f74  es.issuperset(ot
-0000f380: 6865 725f 6465 7269 7665 645f 6261 7365  her_derived_base
-0000f390: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000f3a0: 6966 2073 656c 662e 6465 7269 7665 645f  if self.derived_
-0000f3b0: 6672 6f6d 5f6f 7020 616e 6420 6e6f 7420  from_op and not 
-0000f3c0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
-0000f3d0: 6465 7269 7665 645f 6672 6f6d 5f6f 703a  derived_from_op:
-0000f3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f3f0: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
-0000f400: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
-0000f410: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0000f420: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
-0000f430: 652e 5f6d 616b 655f 6578 7472 6128 292e  e._make_extra().
-0000f440: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-0000f450: 3d20 7365 6c66 2e64 6572 6976 6564 5f66  = self.derived_f
-0000f460: 726f 6d5f 6f70 0a20 2020 2020 2020 2020  rom_op.         
-0000f470: 2020 2065 6c69 6620 6f74 6865 725f 7361     elif other_sa
-0000f480: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
-0000f490: 6672 6f6d 5f6f 7020 616e 6420 6e6f 7420  from_op and not 
-0000f4a0: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
-0000f4b0: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
-0000f4c0: 2020 2020 2020 7365 6c66 2e5f 6d61 6b65        self._make
-0000f4d0: 5f65 7874 7261 2829 2e64 6572 6976 6564  _extra().derived
-0000f4e0: 5f66 726f 6d5f 6f70 203d 206f 7468 6572  _from_op = other
-0000f4f0: 5f73 616d 655f 6261 7365 2e64 6572 6976  _same_base.deriv
-0000f500: 6564 5f66 726f 6d5f 6f70 0a20 2020 2020  ed_from_op.     
-0000f510: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
-0000f520: 6120 616e 6420 6e6f 7420 6f74 6865 725f  a and not other_
-0000f530: 7361 6d65 5f62 6173 652e 6973 5f64 796e  same_base.is_dyn
-0000f540: 616d 6963 2829 3a0a 2020 2020 2020 2020  amic():.        
-0000f550: 2020 2020 2320 5468 6f73 6520 6d69 6768      # Those migh
-0000f560: 7420 6265 2073 6574 2076 6961 2067 6574  t be set via get
-0000f570: 5f62 6174 6368 5f66 6f72 5f63 7478 2066  _batch_for_ctx f
-0000f580: 6f72 2061 6e20 756e 6465 6669 6e65 6420  or an undefined 
-0000f590: 6469 6d2c 0a20 2020 2020 2020 2020 2020  dim,.           
-0000f5a0: 2023 2077 6869 6368 206e 6f77 2062 6563   # which now bec
-0000f5b0: 6f6d 6573 2073 7461 7469 6320 6475 6520  omes static due 
-0000f5c0: 746f 2060 6f74 6865 7260 2e0a 2020 2020  to `other`..    
-0000f5d0: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
-0000f5e0: 7472 612e 6261 7463 6820 3d20 4e6f 6e65  tra.batch = None
-0000f5f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f600: 662e 5f65 7874 7261 2e63 6f6e 7472 6f6c  f._extra.control
-0000f610: 5f66 6c6f 775f 6374 7820 3d20 4e6f 6e65  _flow_ctx = None
-0000f620: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000f630: 206b 6579 2c20 6469 6d5f 2069 6e20 7365   key, dim_ in se
-0000f640: 6c66 2e5f 6578 7472 612e 7361 6d65 5f66  lf._extra.same_f
-0000f650: 6f72 5f62 6174 6368 5f63 7478 2e69 7465  or_batch_ctx.ite
-0000f660: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0000f670: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-0000f680: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-0000f690: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
-0000f6a0: 2020 2020 2020 2064 696d 5f65 7874 7261         dim_extra
-0000f6b0: 203d 2064 696d 5f2e 5f65 7874 7261 0a20   = dim_._extra. 
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f6d0: 6620 6469 6d5f 6578 7472 613a 0a20 2020  f dim_extra:.   
-0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6f0: 2064 696d 5f65 7874 7261 2e62 6174 6368   dim_extra.batch
-0000f700: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000f710: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
-0000f720: 6578 7472 612e 636f 6e74 726f 6c5f 666c  extra.control_fl
-0000f730: 6f77 5f63 7478 203d 204e 6f6e 650a 2020  ow_ctx = None.  
-0000f740: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
-0000f750: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
-0000f760: 2073 656c 665f 203d 2073 656c 662e 6765   self_ = self.ge
-0000f770: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
-0000f780: 6261 7463 683d 7365 6c66 2e62 6174 6368  batch=self.batch
-0000f790: 2c20 6374 783d 7365 6c66 2e63 6f6e 7472  , ctx=self.contr
-0000f7a0: 6f6c 5f66 6c6f 775f 6374 7829 0a20 2020  ol_flow_ctx).   
-0000f7b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000f7c0: 5f20 6973 206e 6f74 2073 656c 663a 0a20  _ is not self:. 
-0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f7e0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-0000f7f0: 5f63 7478 203d 2073 656c 665f 2e63 6f6e  _ctx = self_.con
-0000f800: 7472 6f6c 5f66 6c6f 775f 6374 7820 2023  trol_flow_ctx  #
-0000f810: 206d 6967 6874 2062 6520 6469 6666 6572   might be differ
-0000f820: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-0000f830: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
-0000f840: 655f 6578 7420 3d20 7365 6c66 5f2e 6479  e_ext = self_.dy
-0000f850: 6e5f 7369 7a65 5f65 7874 2020 2320 6d69  n_size_ext  # mi
-0000f860: 6768 7420 6265 2075 6e73 6574 0a0a 2020  ght be unset..  
-0000f870: 2020 6465 6620 5f6d 6572 6765 5f73 616d    def _merge_sam
-0000f880: 655f 666f 725f 6261 7463 685f 6374 785f  e_for_batch_ctx_
-0000f890: 6469 6374 2873 656c 663a 205f 642e 4469  dict(self: _d.Di
-0000f8a0: 6d2c 206f 7468 6572 3a20 5f64 2e44 696d  m, other: _d.Dim
-0000f8b0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000f8c0: 2020 2020 2020 203a 7061 7261 6d20 6f74         :param ot
-0000f8d0: 6865 723a 0a20 2020 2020 2020 2022 2222  her:.        """
-0000f8e0: 0a20 2020 2020 2020 2023 206e 6f69 6e73  .        # noins
-0000f8f0: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
-0000f900: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
-0000f910: 2020 6966 206e 6f74 2073 656c 662e 5f65    if not self._e
-0000f920: 7874 7261 2061 6e64 206e 6f74 206f 7468  xtra and not oth
-0000f930: 6572 2e5f 6578 7472 613a 0a20 2020 2020  er._extra:.     
-0000f940: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000f950: 2020 2020 2020 7365 6c66 2e5f 7661 6c69        self._vali
-0000f960: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000f970: 6772 6170 6828 290a 2020 2020 2020 2020  graph().        
-0000f980: 6966 2073 656c 662e 5f65 7874 7261 3a0a  if self._extra:.
-0000f990: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000f9a0: 5f2c 2064 696d 2069 6e20 6c69 7374 2873  _, dim in list(s
-0000f9b0: 656c 662e 5f65 7874 7261 2e73 616d 655f  elf._extra.same_
-0000f9c0: 666f 725f 6261 7463 685f 6374 782e 6974  for_batch_ctx.it
-0000f9d0: 656d 7328 2929 3a0a 2020 2020 2020 2020  ems()):.        
-0000f9e0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-0000f9f0: 7369 6e73 7461 6e63 6528 6469 6d2c 205f  sinstance(dim, _
-0000fa00: 642e 4469 6d29 0a20 2020 2020 2020 2020  d.Dim).         
-0000fa10: 2020 2020 2020 2064 696d 2e5f 7661 6c69         dim._vali
-0000fa20: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000fa30: 6772 6170 6828 290a 2020 2020 2020 2020  graph().        
-0000fa40: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
-0000fa50: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
-0000fa60: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-0000fa70: 722e 5f65 7874 7261 3a0a 2020 2020 2020  r._extra:.      
-0000fa80: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-0000fa90: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-0000faa0: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
-0000fab0: 2020 2066 6f72 206b 6579 2c20 6469 6d20     for key, dim 
-0000fac0: 696e 206f 7468 6572 2e5f 6578 7472 612e  in other._extra.
-0000fad0: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
-0000fae0: 7478 2e69 7465 6d73 2829 3a0a 2020 2020  tx.items():.    
-0000faf0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000fb00: 6f74 2064 696d 2e5f 7661 6c69 6461 7465  ot dim._validate
-0000fb10: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
-0000fb20: 6828 293a 0a20 2020 2020 2020 2020 2020  h():.           
-0000fb30: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0000fb40: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000fb50: 2020 7365 6c66 5f64 696d 203d 2073 656c    self_dim = sel
-0000fb60: 662e 5f6d 616b 655f 6578 7472 6128 292e  f._make_extra().
-0000fb70: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
-0000fb80: 7478 2e67 6574 286b 6579 2c20 4e6f 6e65  tx.get(key, None
-0000fb90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000fba0: 2020 6966 2073 656c 665f 6469 6d20 616e    if self_dim an
-0000fbb0: 6420 2873 656c 665f 6469 6d2e 6479 6e5f  d (self_dim.dyn_
-0000fbc0: 7369 7a65 5f65 7874 206f 7220 6e6f 7420  size_ext or not 
-0000fbd0: 6469 6d2e 6479 6e5f 7369 7a65 5f65 7874  dim.dyn_size_ext
-0000fbe0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000fbf0: 2020 2020 2020 2063 6f6e 7469 6e75 6520         continue 
-0000fc00: 2023 206b 6565 7020 6f75 7273 0a20 2020   # keep ours.   
-0000fc10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000fc20: 6e6f 7420 6469 6d2e 6479 6e5f 7369 7a65  not dim.dyn_size
-0000fc30: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
-0000fc40: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0000fc50: 7565 2020 2320 756e 6465 6669 6e65 642c  ue  # undefined,
-0000fc60: 2064 6f20 6e6f 7420 6f76 6572 7461 6b65   do not overtake
-0000fc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc80: 2073 656c 662e 5f65 7874 7261 2e73 616d   self._extra.sam
-0000fc90: 655f 666f 725f 6261 7463 685f 6374 785b  e_for_batch_ctx[
-0000fca0: 6b65 795d 203d 2064 696d 0a20 2020 2020  key] = dim.     
-0000fcb0: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
-0000fcc0: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
-0000fcd0: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
-0000fce0: 2020 2020 6f74 6865 722e 5f65 7874 7261      other._extra
-0000fcf0: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-0000fd00: 6374 782e 636c 6561 7228 2920 2023 2077  ctx.clear()  # w
-0000fd10: 6520 6f6e 6c79 2077 616e 7420 746f 2068  e only want to h
-0000fd20: 6176 6520 6974 206f 6e63 650a 0a20 2020  ave it once..   
-0000fd30: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
-0000fd40: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
-0000fd50: 720a 2020 2020 6465 6620 6465 7269 7665  r.    def derive
-0000fd60: 5f66 726f 6d28 7365 6c66 3a20 5f64 2e44  _from(self: _d.D
-0000fd70: 696d 2c20 6261 7365 3a20 5f64 2e44 696d  im, base: _d.Dim
-0000fd80: 2c20 7365 745f 6465 7269 7665 645f 6672  , set_derived_fr
-0000fd90: 6f6d 5f66 6c61 673a 2062 6f6f 6c20 3d20  om_flag: bool = 
-0000fda0: 5472 7565 293a 0a20 2020 2020 2020 2022  True):.        "
-0000fdb0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-0000fdc0: 6d20 6261 7365 3a20 6469 6d0a 2020 2020  m base: dim.    
-0000fdd0: 2020 2020 3a70 6172 616d 2073 6574 5f64      :param set_d
-0000fde0: 6572 6976 6564 5f66 726f 6d5f 666c 6167  erived_from_flag
-0000fdf0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000fe00: 2020 2020 2020 7365 6c66 5f62 6173 6520        self_base 
-0000fe10: 3d20 7365 6c66 2e67 6574 5f73 616d 655f  = self.get_same_
-0000fe20: 6261 7365 2829 0a20 2020 2020 2020 2073  base().        s
-0000fe30: 656c 665f 6261 7365 5f65 7874 7261 203d  elf_base_extra =
-0000fe40: 2073 656c 665f 6261 7365 2e5f 6d61 6b65   self_base._make
-0000fe50: 5f65 7874 7261 2829 0a20 2020 2020 2020  _extra().       
-0000fe60: 2069 6620 7365 745f 6465 7269 7665 645f   if set_derived_
-0000fe70: 6672 6f6d 5f66 6c61 673a 0a20 2020 2020  from_flag:.     
-0000fe80: 2020 2020 2020 2069 6620 7365 6c66 5f62         if self_b
-0000fe90: 6173 655f 6578 7472 612e 6465 7269 7665  ase_extra.derive
-0000fea0: 645f 6672 6f6d 5f74 6167 3a0a 2020 2020  d_from_tag:.    
-0000feb0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000fec0: 7274 2073 656c 665f 6261 7365 5f65 7874  rt self_base_ext
-0000fed0: 7261 2e64 6572 6976 6564 5f66 726f 6d5f  ra.derived_from_
-0000fee0: 7461 6720 3d3d 2062 6173 650a 2020 2020  tag == base.    
-0000fef0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ff00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ff10: 6c66 5f62 6173 655f 6578 7472 612e 6465  lf_base_extra.de
-0000ff20: 7269 7665 645f 6672 6f6d 5f74 6167 203d  rived_from_tag =
-0000ff30: 2062 6173 650a 2020 2020 2020 2020 6966   base.        if
-0000ff40: 2073 656c 662e 6973 5f64 796e 616d 6963   self.is_dynamic
-0000ff50: 2829 206f 7220 6e6f 7420 7365 6c66 2e69  () or not self.i
-0000ff60: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
-0000ff70: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000ff80: 7420 7365 6c66 2e62 6174 6368 2061 6e64  t self.batch and
-0000ff90: 2062 6173 652e 6261 7463 683a 0a20 2020   base.batch:.   
-0000ffa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ffb0: 662e 6261 7463 6820 3d20 6261 7365 2e62  f.batch = base.b
-0000ffc0: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
-0000ffd0: 2020 2020 2073 656c 662e 636f 6e74 726f       self.contro
-0000ffe0: 6c5f 666c 6f77 5f63 7478 203d 2062 6173  l_flow_ctx = bas
-0000fff0: 652e 636f 6e74 726f 6c5f 666c 6f77 5f63  e.control_flow_c
-00010000: 7478 0a20 2020 2020 2020 2020 2020 2020  tx.             
-00010010: 2020 206b 6579 203d 2062 6173 652e 6261     key = base.ba
-00010020: 7463 682c 2062 6173 652e 636f 6e74 726f  tch, base.contro
-00010030: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
-00010040: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00010050: 7420 6b65 7920 6e6f 7420 696e 2073 656c  t key not in sel
-00010060: 665f 6261 7365 5f65 7874 7261 2e73 616d  f_base_extra.sam
-00010070: 655f 666f 725f 6261 7463 685f 6374 780a  e_for_batch_ctx.
-00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010090: 7365 6c66 5f62 6173 655f 6578 7472 612e  self_base_extra.
-000100a0: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
-000100b0: 7478 5b6b 6579 5d20 3d20 7365 6c66 0a20  tx[key] = self. 
-000100c0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000100d0: 7420 7365 6c66 2e64 796e 5f73 697a 655f  t self.dyn_size_
-000100e0: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-000100f0: 2020 2020 2069 6620 6261 7365 2e64 796e       if base.dyn
-00010100: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-00010110: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010120: 6620 6261 7365 2e62 6174 6368 2061 6e64  f base.batch and
-00010130: 2062 6173 652e 6261 7463 6820 3d3d 2073   base.batch == s
-00010140: 656c 662e 6261 7463 6820 616e 6420 6261  elf.batch and ba
-00010150: 7365 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  se.control_flow_
-00010160: 6374 7820 3d3d 2073 656c 662e 636f 6e74  ctx == self.cont
-00010170: 726f 6c5f 666c 6f77 5f63 7478 3a0a 2020  rol_flow_ctx:.  
-00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010190: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-000101a0: 697a 655f 6578 7420 3d20 6261 7365 2e64  ize_ext = base.d
-000101b0: 796e 5f73 697a 655f 6578 742e 636f 7079  yn_size_ext.copy
-000101c0: 5f74 656d 706c 6174 6528 6e61 6d65 3d22  _template(name="
-000101d0: 2573 3a73 697a 6522 2025 2073 656c 665f  %s:size" % self_
-000101e0: 6261 7365 2e64 6573 6372 6970 7469 6f6e  base.description
-000101f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010200: 2020 656c 6966 2062 6173 652e 6973 5f62    elif base.is_b
-00010210: 6174 6368 5f64 696d 2829 3a0a 2020 2020  atch_dim():.    
-00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010230: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00010240: 7420 3d20 5f74 2e54 656e 736f 7228 0a20  t = _t.Tensor(. 
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2020 2020 206e 616d 653d 2225 733a         name="%s:
-00010270: 6261 7463 6822 2025 2073 656c 665f 6261  batch" % self_ba
-00010280: 7365 2e64 6573 6372 6970 7469 6f6e 2c20  se.description, 
-00010290: 7368 6170 653d 2829 2c20 6474 7970 653d  shape=(), dtype=
-000102a0: 2269 6e74 3332 222c 2062 6174 6368 5f64  "int32", batch_d
-000102b0: 696d 5f61 7869 733d 4e6f 6e65 0a20 2020  im_axis=None.   
-000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102d0: 2029 0a0a 2020 2020 6465 6620 636f 7079   )..    def copy
-000102e0: 5f66 726f 6d28 7365 6c66 3a20 4469 6d2c  _from(self: Dim,
-000102f0: 206f 7468 6572 3a20 4469 6d29 3a0a 2020   other: Dim):.  
-00010300: 2020 2020 2020 2222 2264 6566 696e 6522        """define"
-00010310: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00010320: 7369 7a65 203d 206f 7468 6572 2e73 697a  size = other.siz
-00010330: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
-00010340: 6170 6163 6974 7920 3d20 6f74 6865 722e  apacity = other.
-00010350: 6361 7061 6369 7479 0a20 2020 2020 2020  capacity.       
-00010360: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00010370: 7874 203d 206f 7468 6572 2e64 796e 5f73  xt = other.dyn_s
-00010380: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
-00010390: 7365 6c66 2e64 6572 6976 655f 6672 6f6d  self.derive_from
-000103a0: 286f 7468 6572 290a 0a20 2020 2040 636c  (other)..    @cl
-000103b0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-000103c0: 6620 6765 745f 6578 6973 7469 6e67 5f74  f get_existing_t
-000103d0: 6167 5f66 726f 6d5f 636f 6c6c 6563 7469  ag_from_collecti
-000103e0: 6f6e 2863 6c73 2c20 6f74 6865 722c 2074  on(cls, other, t
-000103f0: 6167 732c 2069 735f 6571 7561 6c5f 6f70  ags, is_equal_op
-00010400: 7473 3d4e 6f6e 6529 3a0a 2020 2020 2020  ts=None):.      
-00010410: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00010420: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
-00010430: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-00010440: 6973 745b 4469 6d5d 7c74 7570 6c65 5b44  ist[Dim]|tuple[D
-00010450: 696d 5d7c 7365 745b 4469 6d5d 2074 6167  im]|set[Dim] tag
-00010460: 733a 0a20 2020 2020 2020 203a 7061 7261  s:.        :para
-00010470: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
-00010480: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
-00010490: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
-000104a0: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
-000104b0: 7274 7970 653a 2044 696d 7c4e 6f6e 650a  rtype: Dim|None.
-000104c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000104d0: 2020 2020 6966 2069 735f 6571 7561 6c5f      if is_equal_
-000104e0: 6f70 7473 2069 7320 4e6f 6e65 3a0a 2020  opts is None:.  
-000104f0: 2020 2020 2020 2020 2020 6973 5f65 7175            is_equ
-00010500: 616c 5f6f 7074 7320 3d20 7b7d 0a20 2020  al_opts = {}.   
-00010510: 2020 2020 2023 2057 6520 646f 2070 6f74       # We do pot
-00010520: 656e 7469 616c 206d 756c 7469 706c 6520  ential multiple 
-00010530: 726f 756e 6473 2c20 7375 6368 2074 6861  rounds, such tha
-00010540: 7420 7765 2070 7265 6665 7220 226d 6f72  t we prefer "mor
-00010550: 6520 6571 7561 6c22 2028 7573 696e 6720  e equal" (using 
-00010560: 6c65 7373 2069 735f 6571 7561 6c5f 6f70  less is_equal_op
-00010570: 7473 292e 0a20 2020 2020 2020 2072 6f75  ts)..        rou
-00010580: 6e64 7320 3d20 5b7b 7d5d 0a20 2020 2020  nds = [{}].     
-00010590: 2020 2069 6620 6973 5f65 7175 616c 5f6f     if is_equal_o
-000105a0: 7074 733a 0a20 2020 2020 2020 2020 2020  pts:.           
-000105b0: 2069 6620 2262 726f 6164 6361 7374 5f6d   if "broadcast_m
-000105c0: 6174 6368 6573 2220 696e 2069 735f 6571  atches" in is_eq
-000105d0: 7561 6c5f 6f70 7473 3a0a 2020 2020 2020  ual_opts:.      
-000105e0: 2020 2020 2020 2020 2020 726f 756e 6473            rounds
-000105f0: 2e61 7070 656e 6428 7b6b 3a20 7620 666f  .append({k: v fo
-00010600: 7220 286b 2c20 7629 2069 6e20 6973 5f65  r (k, v) in is_e
-00010610: 7175 616c 5f6f 7074 732e 6974 656d 7328  qual_opts.items(
-00010620: 2920 6966 206b 2021 3d20 2262 726f 6164  ) if k != "broad
-00010630: 6361 7374 5f6d 6174 6368 6573 227d 290a  cast_matches"}).
-00010640: 2020 2020 2020 2020 2020 2020 726f 756e              roun
-00010650: 6473 2e61 7070 656e 6428 6973 5f65 7175  ds.append(is_equ
-00010660: 616c 5f6f 7074 7329 0a20 2020 2020 2020  al_opts).       
-00010670: 2066 6f72 205f 6973 5f65 7175 616c 5f6f   for _is_equal_o
-00010680: 7074 7320 696e 2072 6f75 6e64 733a 0a20  pts in rounds:. 
-00010690: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
-000106a0: 7461 6720 696e 2074 6167 733a 0a20 2020  tag in tags:.   
-000106b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000106c0: 5f74 6167 2e69 735f 6571 7561 6c28 6f74  _tag.is_equal(ot
-000106d0: 6865 722c 202a 2a5f 6973 5f65 7175 616c  her, **_is_equal
-000106e0: 5f6f 7074 7329 3a0a 2020 2020 2020 2020  _opts):.        
-000106f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00010700: 726e 205f 7461 670a 2020 2020 2020 2020  rn _tag.        
-00010710: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00010720: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00010730: 2020 6465 6620 6765 745f 616c 6c5f 6469    def get_all_di
-00010740: 6d65 6e73 696f 6e5f 7461 6773 2863 6c73  mension_tags(cls
-00010750: 2c20 6461 7461 5f6c 6973 742c 2069 735f  , data_list, is_
-00010760: 6571 7561 6c5f 6f70 7473 3d4e 6f6e 652c  equal_opts=None,
-00010770: 2075 6e69 7175 655f 7365 7061 7261 7465   unique_separate
-00010780: 5f61 7865 733d 5472 7565 293a 0a20 2020  _axes=True):.   
-00010790: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000107a0: 203a 7061 7261 6d20 6c69 7374 5b5f 742e   :param list[_t.
-000107b0: 5465 6e73 6f72 5d20 6461 7461 5f6c 6973  Tensor] data_lis
-000107c0: 743a 0a20 2020 2020 2020 203a 7061 7261  t:.        :para
-000107d0: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
-000107e0: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
-000107f0: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
-00010800: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
-00010810: 7061 7261 6d20 626f 6f6c 2075 6e69 7175  param bool uniqu
-00010820: 655f 7365 7061 7261 7465 5f61 7865 733a  e_separate_axes:
-00010830: 2065 2e67 2e20 6461 7461 5f6c 6973 743d   e.g. data_list=
-00010840: 5b44 6174 6120 7769 7468 2073 6861 7065  [Data with shape
-00010850: 2028 422c 352c 352c 3130 295d 2072 6573   (B,5,5,10)] res
-00010860: 756c 7473 2069 6e20 3420 6469 6d20 7461  ults in 4 dim ta
-00010870: 6773 2c20 6e6f 7420 332e 0a20 2020 2020  gs, not 3..     
-00010880: 2020 203a 7265 7475 726e 3a20 6c69 7374     :return: list
-00010890: 206f 6620 6469 6d65 6e73 696f 6e20 7461   of dimension ta
-000108a0: 6773 2c20 6469 6374 2066 6f72 2064 6174  gs, dict for dat
-000108b0: 6120 2d3e 206c 6973 7420 6f66 2064 696d  a -> list of dim
-000108c0: 656e 7369 6f6e 2074 6167 7320 2866 6f72  ension tags (for
-000108d0: 2065 6163 6820 6178 6973 290a 2020 2020   each axis).    
-000108e0: 2020 2020 3a72 7479 7065 3a20 286c 6973      :rtype: (lis
-000108f0: 745b 4469 6d5d 2c20 7574 696c 2e44 6963  t[Dim], util.Dic
-00010900: 7452 6566 4b65 7973 5b5f 742e 5465 6e73  tRefKeys[_t.Tens
-00010910: 6f72 2c20 6c69 7374 5b44 696d 5d5d 290a  or, list[Dim]]).
-00010920: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010930: 2020 2020 7461 6773 203d 205b 5d0a 2020      tags = [].  
-00010940: 2020 2020 2020 6461 7461 5f61 7865 735f        data_axes_
-00010950: 6469 6374 203d 2075 7469 6c2e 4469 6374  dict = util.Dict
-00010960: 5265 664b 6579 7328 2920 2023 2074 7970  RefKeys()  # typ
-00010970: 653a 2075 7469 6c2e 4469 6374 5265 664b  e: util.DictRefK
-00010980: 6579 735b 5f74 2e54 656e 736f 722c 204c  eys[_t.Tensor, L
-00010990: 6973 745b 4469 6d5d 5d0a 2020 2020 2020  ist[Dim]].      
-000109a0: 2020 666f 7220 6461 7461 2069 6e20 6461    for data in da
-000109b0: 7461 5f6c 6973 743a 0a20 2020 2020 2020  ta_list:.       
-000109c0: 2020 2020 2064 6174 615f 6178 6573 5f64       data_axes_d
-000109d0: 6963 745b 6461 7461 5d20 3d20 5b5d 0a20  ict[data] = []. 
-000109e0: 2020 2020 2020 2020 2020 2065 7869 7374             exist
-000109f0: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
-00010a00: 6f6e 5f66 6f72 5f64 6174 6120 3d20 6c69  on_for_data = li
-00010a10: 7374 2874 6167 7329 2069 6620 756e 6971  st(tags) if uniq
-00010a20: 7565 5f73 6570 6172 6174 655f 6178 6573  ue_separate_axes
-00010a30: 2065 6c73 6520 7461 6773 0a20 2020 2020   else tags.     
-00010a40: 2020 2020 2020 2066 6f72 2061 7869 7320         for axis 
-00010a50: 696e 2072 616e 6765 2864 6174 612e 6261  in range(data.ba
-00010a60: 7463 685f 6e64 696d 293a 0a20 2020 2020  tch_ndim):.     
-00010a70: 2020 2020 2020 2020 2020 2074 6167 203d             tag =
-00010a80: 2064 6174 612e 6765 745f 6469 6d5f 7461   data.get_dim_ta
-00010a90: 6728 6178 6973 290a 2020 2020 2020 2020  g(axis).        
-00010aa0: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
-00010ab0: 5f74 6167 203d 2063 6c73 2e67 6574 5f65  _tag = cls.get_e
-00010ac0: 7869 7374 696e 675f 7461 675f 6672 6f6d  xisting_tag_from
-00010ad0: 5f63 6f6c 6c65 6374 696f 6e28 0a20 2020  _collection(.   
-00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010af0: 2074 6167 2c20 7461 6773 3d65 7869 7374   tag, tags=exist
-00010b00: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
-00010b10: 6f6e 5f66 6f72 5f64 6174 612c 2069 735f  on_for_data, is_
-00010b20: 6571 7561 6c5f 6f70 7473 3d69 735f 6571  equal_opts=is_eq
-00010b30: 7561 6c5f 6f70 7473 0a20 2020 2020 2020  ual_opts.       
-00010b40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00010b50: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
-00010b60: 6973 7469 6e67 5f74 6167 3a0a 2020 2020  isting_tag:.    
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 6966 2075 6e69 7175 655f 7365 7061 7261  if unique_separa
-00010b90: 7465 5f61 7865 733a 0a20 2020 2020 2020  te_axes:.       
-00010ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bb0: 2065 7869 7374 696e 675f 7461 675f 636f   existing_tag_co
-00010bc0: 6c6c 6563 7469 6f6e 5f66 6f72 5f64 6174  llection_for_dat
-00010bd0: 612e 7265 6d6f 7665 2865 7869 7374 696e  a.remove(existin
-00010be0: 675f 7461 6729 2020 2320 646f 6e27 7420  g_tag)  # don't 
-00010bf0: 7461 6b65 2069 7420 6167 6169 6e20 666f  take it again fo
-00010c00: 7220 7468 6973 2064 6174 610a 2020 2020  r this data.    
-00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c20: 7265 706c 6163 655f 6578 6973 7469 6e67  replace_existing
-00010c30: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00010c40: 2020 2020 2020 2020 2020 2020 2065 7869               exi
-00010c50: 7374 696e 675f 7461 672e 756e 6465 6669  sting_tag.undefi
-00010c60: 6e65 6420 616e 6420 6e6f 7420 7461 672e  ned and not tag.
-00010c70: 756e 6465 6669 6e65 6420 616e 6420 7461  undefined and ta
-00010c80: 672e 6469 6d65 6e73 696f 6e20 3d3d 2065  g.dimension == e
-00010c90: 7869 7374 696e 675f 7461 672e 6469 6d65  xisting_tag.dime
-00010ca0: 6e73 696f 6e0a 2020 2020 2020 2020 2020  nsion.          
-00010cb0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cd0: 6966 2072 6570 6c61 6365 5f65 7869 7374  if replace_exist
-00010ce0: 696e 673a 2020 2320 5265 706c 6163 6520  ing:  # Replace 
-00010cf0: 7468 6520 6578 6973 7469 6e67 2062 7920  the existing by 
-00010d00: 7468 6520 6e65 7720 7461 672e 0a20 2020  the new tag..   
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 2020 2020 2074 6167 735b 7461 6773 2e69       tags[tags.i
-00010d30: 6e64 6578 2865 7869 7374 696e 675f 7461  ndex(existing_ta
-00010d40: 6729 5d20 3d20 7461 670a 2020 2020 2020  g)] = tag.      
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 2020 666f 7220 5f2c 2064 696d 735f 2069    for _, dims_ i
-00010d70: 6e20 6461 7461 5f61 7865 735f 6469 6374  n data_axes_dict
-00010d80: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010da0: 2020 2020 2020 6469 6d73 5f5b 3a5d 203d        dims_[:] =
-00010db0: 205b 7461 6720 6966 2064 203d 3d20 6578   [tag if d == ex
-00010dc0: 6973 7469 6e67 5f74 6167 2065 6c73 6520  isting_tag else 
-00010dd0: 6420 666f 7220 6420 696e 2064 696d 735f  d for d in dims_
-00010de0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00010df0: 2020 2020 2020 2020 2020 6578 6973 7469            existi
-00010e00: 6e67 5f74 6167 203d 2074 6167 0a20 2020  ng_tag = tag.   
-00010e10: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00010e20: 653a 2020 2320 6e6f 2065 7869 7374 696e  e:  # no existin
-00010e30: 6720 7461 670a 2020 2020 2020 2020 2020  g tag.          
-00010e40: 2020 2020 2020 2020 2020 7461 6773 2e61            tags.a
-00010e50: 7070 656e 6428 7461 6729 0a20 2020 2020  ppend(tag).     
-00010e60: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00010e70: 6178 6573 5f64 6963 745b 6461 7461 5d2e  axes_dict[data].
-00010e80: 6170 7065 6e64 2865 7869 7374 696e 675f  append(existing_
-00010e90: 7461 6720 6f72 2074 6167 290a 2020 2020  tag or tag).    
-00010ea0: 2020 2020 7265 7475 726e 2074 6167 732c      return tags,
-00010eb0: 2064 6174 615f 6178 6573 5f64 6963 740a   data_axes_dict.
-00010ec0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00010ed0: 640a 2020 2020 6465 6620 6765 745f 756e  d.    def get_un
-00010ee0: 6971 5f63 6f6c 6c65 6374 696f 6e28 636c  iq_collection(cl
-00010ef0: 732c 2074 6167 732c 2069 735f 6571 7561  s, tags, is_equa
-00010f00: 6c5f 6f70 7473 3d4e 6f6e 6529 3a0a 2020  l_opts=None):.  
+0000b260: 6173 6528 2920 6966 2064 6572 6976 6564  ase() if derived
+0000b270: 5f6d 6174 6368 6573 2065 6c73 6520 7365  _matches else se
+0000b280: 6c66 2e67 6574 5f73 616d 655f 6261 7365  lf.get_same_base
+0000b290: 2829 0a20 2020 2020 2020 206f 7468 6572  ().        other
+0000b2a0: 5f62 6173 6520 3d20 6f74 6865 722e 6765  _base = other.ge
+0000b2b0: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
+0000b2c0: 6173 6528 2920 6966 2064 6572 6976 6564  ase() if derived
+0000b2d0: 5f6d 6174 6368 6573 2065 6c73 6520 6f74  _matches else ot
+0000b2e0: 6865 722e 6765 745f 7361 6d65 5f62 6173  her.get_same_bas
+0000b2f0: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
+0000b300: 656c 665f 6261 7365 2069 7320 6f74 6865  elf_base is othe
+0000b310: 725f 6261 7365 3a0a 2020 2020 2020 2020  r_base:.        
+0000b320: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000b330: 2020 2020 2020 2020 6966 2073 656c 665f          if self_
+0000b340: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000b350: 6d5f 6f70 2061 6e64 206f 7468 6572 5f62  m_op and other_b
+0000b360: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
+0000b370: 5f6f 703a 0a20 2020 2020 2020 2020 2020  _op:.           
+0000b380: 2069 6620 7365 6c66 5f62 6173 652e 6465   if self_base.de
+0000b390: 7269 7665 645f 6672 6f6d 5f6f 7020 3d3d  rived_from_op ==
+0000b3a0: 206f 7468 6572 5f62 6173 652e 6465 7269   other_base.deri
+0000b3b0: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
+0000b3c0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000b3d0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0000b3e0: 2073 656c 665f 6b69 6e64 203d 2073 656c   self_kind = sel
+0000b3f0: 662e 6b69 6e64 0a20 2020 2020 2020 206f  f.kind.        o
+0000b400: 7468 6572 5f6b 696e 6420 3d20 6f74 6865  ther_kind = othe
+0000b410: 722e 6b69 6e64 0a20 2020 2020 2020 2069  r.kind.        i
+0000b420: 6620 7365 6c66 5f6b 696e 6420 3d3d 206f  f self_kind == o
+0000b430: 7468 6572 5f6b 696e 6420 3d3d 2044 696d  ther_kind == Dim
+0000b440: 5479 7065 732e 4665 6174 7572 6520 616e  Types.Feature an
+0000b450: 6420 6967 6e6f 7265 5f66 6561 7475 7265  d ignore_feature
+0000b460: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
+0000b470: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000b480: 2020 2020 2020 6966 2074 7265 6174 5f66        if treat_f
+0000b490: 6561 7475 7265 5f61 735f 7370 6174 6961  eature_as_spatia
+0000b4a0: 6c3a 0a20 2020 2020 2020 2020 2020 2023  l:.            #
+0000b4b0: 204e 6f74 653a 204e 6f20 6b69 6e64 2061   Note: No kind a
+0000b4c0: 7420 616c 6c3a 2052 6569 6e74 6572 7072  t all: Reinterpr
+0000b4d0: 6574 2074 7265 6174 5f66 6561 7475 7265  et treat_feature
+0000b4e0: 5f61 735f 7370 6174 6961 6c20 6120 6269  _as_spatial a bi
+0000b4f0: 743a 0a20 2020 2020 2020 2020 2020 2023  t:.            #
+0000b500: 2041 7373 756d 6520 7468 6174 2077 6520   Assume that we 
+0000b510: 7761 6e74 2074 6865 6d20 616c 6c20 746f  want them all to
+0000b520: 2062 6520 6861 6e64 6c65 6420 7468 6520   be handled the 
+0000b530: 7361 6d65 2c20 6e6f 206d 6174 7465 7220  same, no matter 
+0000b540: 7468 6520 6b69 6e64 2e0a 2020 2020 2020  the kind..      
+0000b550: 2020 2020 2020 2320 2845 7863 6570 7420        # (Except 
+0000b560: 6f66 2062 6174 6368 2064 696d 206b 696e  of batch dim kin
+0000b570: 642c 2077 6869 6368 2069 7320 7374 696c  d, which is stil
+0000b580: 6c20 6578 636c 7564 6564 2068 6572 652e  l excluded here.
+0000b590: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000b5a0: 2073 656c 665f 6b69 6e64 203d 3d20 4469   self_kind == Di
+0000b5b0: 6d54 7970 6573 2e46 6561 7475 7265 206f  mTypes.Feature o
+0000b5c0: 7220 6e6f 7420 7365 6c66 5f6b 696e 643a  r not self_kind:
+0000b5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b5e0: 2073 656c 665f 6b69 6e64 203d 2044 696d   self_kind = Dim
+0000b5f0: 5479 7065 732e 5370 6174 6961 6c0a 2020  Types.Spatial.  
+0000b600: 2020 2020 2020 2020 2020 6966 206f 7468            if oth
+0000b610: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
+0000b620: 7065 732e 4665 6174 7572 6520 6f72 206e  pes.Feature or n
+0000b630: 6f74 206f 7468 6572 5f6b 696e 643a 0a20  ot other_kind:. 
+0000b640: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000b650: 7468 6572 5f6b 696e 6420 3d20 4469 6d54  ther_kind = DimT
+0000b660: 7970 6573 2e53 7061 7469 616c 0a20 2020  ypes.Spatial.   
+0000b670: 2020 2020 2069 6620 7365 6c66 2e64 696d       if self.dim
+0000b680: 656e 7369 6f6e 2021 3d20 6f74 6865 722e  ension != other.
+0000b690: 6469 6d65 6e73 696f 6e3a 0a20 2020 2020  dimension:.     
+0000b6a0: 2020 2020 2020 2069 6620 6272 6f61 6463         if broadc
+0000b6b0: 6173 745f 6d61 7463 6865 7320 616e 6420  ast_matches and 
+0000b6c0: 2873 656c 662e 6469 6d65 6e73 696f 6e20  (self.dimension 
+0000b6d0: 3d3d 2031 206f 7220 6f74 6865 722e 6469  == 1 or other.di
+0000b6e0: 6d65 6e73 696f 6e20 3d3d 2031 293a 0a20  mension == 1):. 
+0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000b700: 6173 7320 2023 2070 6173 7320 6f6e 0a20  ass  # pass on. 
+0000b710: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000b720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b730: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0000b740: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
+0000b750: 6e64 2021 3d20 6f74 6865 725f 6b69 6e64  nd != other_kind
+0000b760: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000b770: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+0000b780: 2020 2069 6620 7365 6c66 5f6b 696e 6420     if self_kind 
+0000b790: 3d3d 206f 7468 6572 5f6b 696e 6420 3d3d  == other_kind ==
+0000b7a0: 2044 696d 5479 7065 732e 4261 7463 683a   DimTypes.Batch:
+0000b7b0: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
+0000b7c0: 6f74 653a 2054 6869 7320 6d69 6768 7420  ote: This might 
+0000b7d0: 6265 2069 6e63 6f72 7265 6374 2069 6e20  be incorrect in 
+0000b7e0: 736f 6d65 2063 6173 6573 2c0a 2020 2020  some cases,.    
+0000b7f0: 2020 2020 2020 2020 2320 652e 672e 2066          # e.g. f
+0000b800: 6f72 2062 6561 6d20 7365 6172 6368 2077  or beam search w
+0000b810: 6865 6e20 7765 2068 6176 6520 7468 6520  hen we have the 
+0000b820: 6265 616d 2068 6964 6465 6e20 696e 2074  beam hidden in t
+0000b830: 6865 2062 6174 6368 2064 696d 2c0a 2020  he batch dim,.  
+0000b840: 2020 2020 2020 2020 2020 2320 6f72 2077            # or w
+0000b850: 6865 6e20 7765 2075 7365 6420 4d65 7267  hen we used Merg
+0000b860: 6544 696d 734c 6179 6572 206f 6e20 7468  eDimsLayer on th
+0000b870: 6520 6261 7463 6820 6178 6973 2c20 6f72  e batch axis, or
+0000b880: 2073 6f2e 0a20 2020 2020 2020 2020 2020   so..           
+0000b890: 2023 2057 6520 6d69 6768 7420 6e65 6564   # We might need
+0000b8a0: 2074 6f20 6578 7465 6e64 2074 6865 206c   to extend the l
+0000b8b0: 6f67 6963 2068 6572 6520 6c61 7465 722e  ogic here later.
+0000b8c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000b8d0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0000b8e0: 2069 6620 4265 6861 7669 6f72 5665 7273   if BehaviorVers
+0000b8f0: 696f 6e2e 6765 7428 2920 3e3d 2031 363a  ion.get() >= 16:
+0000b900: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
+0000b910: 6974 6865 7220 7365 6c66 206f 7220 6f74  ither self or ot
+0000b920: 6865 7220 6973 2073 6f6d 6520 6469 6d20  her is some dim 
+0000b930: 7461 6720 6578 706c 6963 6974 6c79 2063  tag explicitly c
+0000b940: 7265 6174 6564 2062 7920 7468 6520 7573  reated by the us
+0000b950: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000b960: 2320 616e 6420 7468 6579 2061 7265 206e  # and they are n
+0000b970: 6f74 2074 6865 2073 616d 652c 2073 6f20  ot the same, so 
+0000b980: 7765 206e 6576 6572 2074 7265 6174 2074  we never treat t
+0000b990: 6865 6d20 6173 2065 7175 616c 2e0a 2020  hem as equal..  
+0000b9a0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000b9b0: 2073 656c 662e 6175 746f 5f67 656e 6572   self.auto_gener
+0000b9c0: 6174 6564 206f 7220 6e6f 7420 6f74 6865  ated or not othe
+0000b9d0: 722e 6175 746f 5f67 656e 6572 6174 6564  r.auto_generated
+0000b9e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b9f0: 2020 6966 2062 726f 6164 6361 7374 5f6d    if broadcast_m
+0000ba00: 6174 6368 6573 2061 6e64 2028 0a20 2020  atches and (.   
+0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba20: 2028 7365 6c66 2e64 696d 656e 7369 6f6e   (self.dimension
+0000ba30: 203d 3d20 3120 616e 6420 7365 6c66 2e61   == 1 and self.a
+0000ba40: 7574 6f5f 6765 6e65 7261 7465 6429 206f  uto_generated) o
+0000ba50: 7220 286f 7468 6572 2e64 696d 656e 7369  r (other.dimensi
+0000ba60: 6f6e 203d 3d20 3120 616e 6420 6f74 6865  on == 1 and othe
+0000ba70: 722e 6175 746f 5f67 656e 6572 6174 6564  r.auto_generated
+0000ba80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ba90: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0000baa0: 2020 2020 2020 2020 2070 6173 7320 2023           pass  #
+0000bab0: 2065 7863 6570 7469 6f6e 2c20 616c 6c6f   exception, allo
+0000bac0: 7720 6272 6f61 6463 6173 7420 6c6f 6769  w broadcast logi
+0000bad0: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
+0000bae0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000baf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000bb00: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0000bb10: 2069 6620 7365 6c66 5f6b 696e 6420 3d3d   if self_kind ==
+0000bb20: 206f 7468 6572 5f6b 696e 6420 3d3d 2044   other_kind == D
+0000bb30: 696d 5479 7065 732e 4665 6174 7572 653a  imTypes.Feature:
+0000bb40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bb50: 616c 6c6f 775f 7361 6d65 5f66 6561 7475  allow_same_featu
+0000bb60: 7265 5f64 696d 3a0a 2020 2020 2020 2020  re_dim:.        
+0000bb70: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0000bb80: 7275 650a 2020 2020 2020 2020 6966 2073  rue.        if s
+0000bb90: 656c 665f 6b69 6e64 203d 3d20 6f74 6865  elf_kind == othe
+0000bba0: 725f 6b69 6e64 203d 3d20 4469 6d54 7970  r_kind == DimTyp
+0000bbb0: 6573 2e53 7061 7469 616c 3a0a 2020 2020  es.Spatial:.    
+0000bbc0: 2020 2020 2020 2020 6966 2061 6c6c 6f77          if allow
+0000bbd0: 5f73 616d 655f 7370 6174 6961 6c5f 6469  _same_spatial_di
+0000bbe0: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
+0000bbf0: 2020 2069 6620 7365 6c66 2e64 696d 656e     if self.dimen
+0000bc00: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+0000bc10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bc20: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000bc30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000bc40: 2020 6966 2062 726f 6164 6361 7374 5f6d    if broadcast_m
+0000bc50: 6174 6368 6573 2061 6e64 2028 7365 6c66  atches and (self
+0000bc60: 2e64 696d 656e 7369 6f6e 203d 3d20 3120  .dimension == 1 
+0000bc70: 6f72 206f 7468 6572 2e64 696d 656e 7369  or other.dimensi
+0000bc80: 6f6e 203d 3d20 3129 3a0a 2020 2020 2020  on == 1):.      
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000bca0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+0000bcb0: 2020 2020 2020 6966 2075 6e6b 6e6f 776e        if unknown
+0000bcc0: 5f73 7061 7469 616c 5f6d 6174 6368 6573  _spatial_matches
+0000bcd0: 2061 6e64 2028 2873 656c 662e 6479 6e5f   and ((self.dyn_
+0000bce0: 7369 7a65 2069 7320 4e6f 6e65 2920 6f72  size is None) or
+0000bcf0: 2028 6f74 6865 722e 6479 6e5f 7369 7a65   (other.dyn_size
+0000bd00: 2069 7320 4e6f 6e65 2929 3a0a 2020 2020   is None)):.    
+0000bd10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000bd20: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+0000bd30: 2020 2020 6966 2075 6e64 6566 696e 6564      if undefined
+0000bd40: 5f6d 6174 6368 6573 2061 6e64 2028 7365  _matches and (se
+0000bd50: 6c66 2e75 6e64 6566 696e 6564 206f 7220  lf.undefined or 
+0000bd60: 6f74 6865 722e 756e 6465 6669 6e65 6429  other.undefined)
+0000bd70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bd80: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000bd90: 2020 2020 2020 2320 496e 2070 7269 6e63        # In princ
+0000bda0: 6970 6c65 2c20 7765 2077 6f75 6c64 2077  iple, we would w
+0000bdb0: 616e 7420 746f 2063 6865 636b 2066 6f72  ant to check for
+0000bdc0: 2069 6465 6e74 6974 7920 2873 656c 6620   identity (self 
+0000bdd0: 6973 206f 7468 6572 292e 0a20 2020 2020  is other)..     
+0000bde0: 2020 2023 2057 6520 6375 7272 656e 746c     # We currentl
+0000bdf0: 7920 7573 6520 7468 6520 6465 7363 7269  y use the descri
+0000be00: 7074 696f 6e20 6265 6361 7573 6520 7468  ption because th
+0000be10: 6520 6964 656e 7469 7479 2077 6f75 6c64  e identity would
+0000be20: 206e 6f74 2062 6520 7468 6520 7361 6d65   not be the same
+0000be30: 0a20 2020 2020 2020 2023 2069 6e20 6361  .        # in ca
+0000be40: 7365 206f 6620 7465 6d70 6c61 7465 2063  se of template c
+0000be50: 6f6e 7374 7275 6374 696f 6e20 7768 6572  onstruction wher
+0000be60: 6520 6120 6469 6d20 7461 6720 6973 206f  e a dim tag is o
+0000be70: 6e63 6520 6372 6561 7465 6420 666f 7220  nce created for 
+0000be80: 6120 7465 6d70 6c61 7465 206c 6179 6572  a template layer
+0000be90: 2c0a 2020 2020 2020 2020 2320 616e 6420  ,.        # and 
+0000bea0: 7468 656e 206c 6174 6572 2061 6761 696e  then later again
+0000beb0: 2066 6f72 2074 6865 2072 6561 6c20 6c61   for the real la
+0000bec0: 7965 722e 0a20 2020 2020 2020 2069 6620  yer..        if 
+0000bed0: 7365 6c66 2e61 7574 6f5f 6765 6e65 7261  self.auto_genera
+0000bee0: 7465 6420 616e 6420 6f74 6865 722e 6175  ted and other.au
+0000bef0: 746f 5f67 656e 6572 6174 6564 2061 6e64  to_generated and
+0000bf00: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+0000bf10: 6e20 3d3d 206f 7468 6572 2e64 6573 6372  n == other.descr
+0000bf20: 6970 7469 6f6e 3a0a 2020 2020 2020 2020  iption:.        
+0000bf30: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000bf40: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0000bf50: 616c 7365 0a0a 2020 2020 6465 6620 5f5f  alse..    def __
+0000bf60: 6571 5f5f 2873 656c 662c 206f 7468 6572  eq__(self, other
+0000bf70: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000bf80: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+0000bf90: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
+0000bfa0: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+0000bfb0: 2020 2020 2020 3a72 6574 7572 6e3a 203a        :return: :
+0000bfc0: 6675 6e63 3a60 6973 5f65 7175 616c 6020  func:`is_equal` 
+0000bfd0: 7769 7468 2064 6566 6175 6c74 206f 7074  with default opt
+0000bfe0: 696f 6e73 0a20 2020 2020 2020 2022 2222  ions.        """
+0000bff0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000c000: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+0000c010: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
+0000c020: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0000c030: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+0000c040: 726e 2073 656c 662e 6973 5f65 7175 616c  rn self.is_equal
+0000c050: 286f 7468 6572 290a 0a20 2020 2064 6566  (other)..    def
+0000c060: 205f 5f6e 655f 5f28 7365 6c66 3a20 4469   __ne__(self: Di
+0000c070: 6d2c 206f 7468 6572 3a20 4469 6d29 3a0a  m, other: Dim):.
+0000c080: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c090: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
+0000c0a0: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
+0000c0b0: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
+0000c0c0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0000c0d0: 6574 7572 6e20 6e6f 7420 2873 656c 6620  eturn not (self 
+0000c0e0: 3d3d 206f 7468 6572 290a 0a20 2020 2064  == other)..    d
+0000c0f0: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
+0000c100: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000c110: 2020 2020 2020 203a 7274 7970 653a 2069         :rtype: i
+0000c120: 6e74 0a20 2020 2020 2020 203a 7265 7475  nt.        :retu
+0000c130: 726e 3a20 6861 7368 2c20 6d61 7463 6869  rn: hash, matchi
+0000c140: 6e67 2074 6f20 3a66 756e 633a 605f 5f65  ng to :func:`__e
+0000c150: 715f 5f60 0a20 2020 2020 2020 2022 2222  q__`.        """
+0000c160: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+0000c170: 6d75 7374 206d 6174 6368 2074 6865 2062  must match the b
+0000c180: 6568 6176 696f 7220 696e 205f 5f65 715f  ehavior in __eq_
+0000c190: 5f2c 2077 6869 6368 2069 7320 6973 5f65  _, which is is_e
+0000c1a0: 7175 616c 2077 6974 6820 6465 6661 756c  qual with defaul
+0000c1b0: 7420 6f70 7469 6f6e 732e 0a20 2020 2020  t options..     
+0000c1c0: 2020 2023 2049 2e65 2e20 6469 6666 6572     # I.e. differ
+0000c1d0: 656e 7420 6861 7368 2069 6d70 6c69 6573  ent hash implies
+0000c1e0: 206e 6f74 2065 7175 616c 2028 6275 7420   not equal (but 
+0000c1f0: 7361 6d65 2068 6173 6820 6e6f 7420 6e65  same hash not ne
+0000c200: 6365 7373 6172 696c 7920 6571 7561 6c29  cessarily equal)
+0000c210: 2e0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000c220: 662e 7370 6563 6961 6c3a 0a20 2020 2020  f.special:.     
+0000c230: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
+0000c240: 7368 2869 6428 7365 6c66 2929 0a20 2020  sh(id(self)).   
+0000c250: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+0000c260: 6261 7463 685f 6469 6d28 293a 0a20 2020  batch_dim():.   
+0000c270: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c280: 6861 7368 2828 2929 0a20 2020 2020 2020  hash(()).       
+0000c290: 2077 6974 6820 7574 696c 2e67 7561 7264   with util.guard
+0000c2a0: 5f69 6e66 696e 6974 655f 7265 6375 7273  _infinite_recurs
+0000c2b0: 696f 6e28 5f64 2e44 696d 2e5f 5f68 6173  ion(_d.Dim.__has
+0000c2c0: 685f 5f2c 2073 656c 6629 3a0a 2020 2020  h__, self):.    
+0000c2d0: 2020 2020 2020 2020 6261 7365 203d 2073          base = s
+0000c2e0: 656c 662e 6765 745f 7361 6d65 5f62 6173  elf.get_same_bas
+0000c2f0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000c300: 6966 2062 6173 6520 6973 206e 6f74 2073  if base is not s
+0000c310: 656c 663a 0a20 2020 2020 2020 2020 2020  elf:.           
+0000c320: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
+0000c330: 2862 6173 6529 0a20 2020 2020 2020 2020  (base).         
+0000c340: 2020 2069 6620 7365 6c66 2e64 6572 6976     if self.deriv
+0000c350: 6564 5f66 726f 6d5f 6f70 3a0a 2020 2020  ed_from_op:.    
+0000c360: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c370: 726e 2068 6173 6828 7365 6c66 2e64 6572  rn hash(self.der
+0000c380: 6976 6564 5f66 726f 6d5f 6f70 290a 2020  ived_from_op).  
+0000c390: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000c3a0: 662e 6175 746f 5f67 656e 6572 6174 6564  f.auto_generated
+0000c3b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c3c0: 2020 7265 7475 726e 2068 6173 6828 2862    return hash((b
+0000c3d0: 6173 652e 6b69 6e64 2c20 6261 7365 2e64  ase.kind, base.d
+0000c3e0: 696d 656e 7369 6f6e 2c20 6261 7365 2e64  imension, base.d
+0000c3f0: 6573 6372 6970 7469 6f6e 2929 0a20 2020  escription)).   
+0000c400: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c410: 6861 7368 2869 6428 6261 7365 2929 0a0a  hash(id(base))..
+0000c420: 2020 2020 6465 6620 5f5f 6c74 5f5f 2873      def __lt__(s
+0000c430: 656c 663a 2044 696d 2c20 6f74 6865 723a  elf: Dim, other:
+0000c440: 2044 696d 293a 0a20 2020 2020 2020 2022   Dim):.        "
+0000c450: 2222 0a20 2020 2020 2020 2044 6566 696e  "".        Defin
+0000c460: 6520 736f 6d65 206f 7264 6572 2e20 5468  e some order. Th
+0000c470: 6973 2069 7320 6a75 7374 2073 7563 6820  is is just such 
+0000c480: 7468 6174 2060 736f 7274 6564 6020 776f  that `sorted` wo
+0000c490: 726b 732c 206f 7220 736f 6d65 2064 6966  rks, or some dif
+0000c4a0: 6620 7265 706f 7274 696e 672c 206f 7220  f reporting, or 
+0000c4b0: 736f 2e0a 2020 2020 2020 2020 4974 2069  so..        It i
+0000c4c0: 7320 6f6e 2073 796d 626f 6c69 6320 6c65  s on symbolic le
+0000c4d0: 7665 6c2c 2069 2e65 2e20 6974 2064 6f65  vel, i.e. it doe
+0000c4e0: 7320 6e6f 7420 636f 6e73 6964 6572 2074  s not consider t
+0000c4f0: 6865 2061 6374 7561 6c20 6469 6d65 6e73  he actual dimens
+0000c500: 696f 6e20 7661 6c75 652e 0a20 2020 2020  ion value..     
+0000c510: 2020 2054 6865 2064 6566 696e 6564 206f     The defined o
+0000c520: 7264 6572 2073 6f6d 6577 6861 7420 6172  rder somewhat ar
+0000c530: 6269 7472 6172 792c 2073 6f20 646f 206e  bitrary, so do n
+0000c540: 6f74 2072 656c 7920 6f6e 2074 6865 2065  ot rely on the e
+0000c550: 7861 6374 2062 6568 6176 696f 722c 0a20  xact behavior,. 
+0000c560: 2020 2020 2020 2061 7320 7468 6973 206d         as this m
+0000c570: 6967 6874 2063 6861 6e67 6520 6174 2073  ight change at s
+0000c580: 6f6d 6520 6c61 7465 7220 706f 696e 742e  ome later point.
+0000c590: 0a20 2020 2020 2020 2043 7572 7265 6e74  .        Current
+0000c5a0: 6c79 2c20 6974 2064 6570 656e 6473 206f  ly, it depends o
+0000c5b0: 6e20 7468 6520 6372 6561 7469 6f6e 2069  n the creation i
+0000c5c0: 6e64 6578 2e0a 0a20 2020 2020 2020 203a  ndex...        :
+0000c5d0: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
+0000c5e0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000c5f0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
+0000c600: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+0000c610: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+0000c620: 722c 2028 5f64 2e44 696d 2c20 5f6d 2e4d  r, (_d.Dim, _m.M
+0000c630: 6172 6b65 6444 696d 2929 3a0a 2020 2020  arkedDim)):.    
+0000c640: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+0000c650: 7065 4572 726f 7228 2263 616e 6e6f 7420  peError("cannot 
+0000c660: 636f 6d70 6172 6520 2572 2077 6974 6820  compare %r with 
+0000c670: 2572 2220 2520 2873 656c 662c 206f 7468  %r" % (self, oth
+0000c680: 6572 2929 0a20 2020 2020 2020 2069 6620  er)).        if 
+0000c690: 7365 6c66 203d 3d20 6f74 6865 723a 0a20  self == other:. 
+0000c6a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c6b0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+0000c6c0: 7265 7475 726e 2064 696d 5f63 6d70 5f76  return dim_cmp_v
+0000c6d0: 616c 7565 2873 656c 6629 203c 2064 696d  alue(self) < dim
+0000c6e0: 5f63 6d70 5f76 616c 7565 286f 7468 6572  _cmp_value(other
+0000c6f0: 290a 0a20 2020 2064 6566 205f 5f67 745f  )..    def __gt_
+0000c700: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+0000c710: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c720: 2020 2020 5365 6520 3a66 756e 633a 605f      See :func:`_
+0000c730: 5f6c 745f 5f60 2e0a 0a20 2020 2020 2020  _lt__`...       
+0000c740: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
+0000c750: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
+0000c760: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+0000c770: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0000c780: 726e 206f 7468 6572 203c 2073 656c 660a  rn other < self.
+0000c790: 0a20 2020 2064 6566 205f 5f67 655f 5f28  .    def __ge__(
+0000c7a0: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+0000c7b0: 2020 2020 2020 7265 7475 726e 206e 6f74        return not
+0000c7c0: 2073 656c 6620 3c20 6f74 6865 720a 0a20   self < other.. 
+0000c7d0: 2020 2064 6566 205f 5f6c 655f 5f28 7365     def __le__(se
+0000c7e0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+0000c7f0: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+0000c800: 656c 6620 3e20 6f74 6865 720a 0a20 2020  elf > other..   
+0000c810: 2064 6566 2067 6574 5f73 616d 655f 6261   def get_same_ba
+0000c820: 7365 2873 656c 663a 205f 642e 4469 6d29  se(self: _d.Dim)
+0000c830: 202d 3e20 5f64 2e44 696d 3a0a 2020 2020   -> _d.Dim:.    
+0000c840: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000c850: 3a72 6574 7572 6e3a 2073 616d 6520 6261  :return: same ba
+0000c860: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
+0000c870: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000c880: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
+0000c890: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000c8a0: 6c66 0a20 2020 2020 2020 2062 6173 6520  lf.        base 
+0000c8b0: 3d20 7365 6c66 0a20 2020 2020 2020 2077  = self.        w
+0000c8c0: 6869 6c65 2062 6173 652e 7361 6d65 5f61  hile base.same_a
+0000c8d0: 733a 0a20 2020 2020 2020 2020 2020 2062  s:.            b
+0000c8e0: 6173 6520 3d20 6261 7365 2e73 616d 655f  ase = base.same_
+0000c8f0: 6173 0a20 2020 2020 2020 2072 6574 7572  as.        retur
+0000c900: 6e20 6261 7365 0a0a 2020 2020 6465 6620  n base..    def 
+0000c910: 6765 745f 7361 6d65 5f64 6572 6976 6564  get_same_derived
+0000c920: 5f62 6173 6528 7365 6c66 3a20 5f64 2e44  _base(self: _d.D
+0000c930: 696d 2920 2d3e 205f 642e 4469 6d3a 0a20  im) -> _d.Dim:. 
+0000c940: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c950: 2020 203a 7265 7475 726e 3a20 7361 6d65     :return: same
+0000c960: 2062 6173 652c 2062 7574 2061 6c73 6f20   base, but also 
+0000c970: 636f 6e73 6964 6572 2064 6572 6976 6564  consider derived
+0000c980: 5f66 726f 6d5f 2e2e 2e0a 2020 2020 2020  _from_....      
+0000c990: 2020 2222 220a 2020 2020 2020 2020 6261    """.        ba
+0000c9a0: 7365 203d 2073 656c 660a 2020 2020 2020  se = self.      
+0000c9b0: 2020 7669 7369 7465 6420 3d20 7b7d 0a20    visited = {}. 
+0000c9c0: 2020 2020 2020 2077 6869 6c65 2062 6173         while bas
+0000c9d0: 652e 7361 6d65 5f61 7320 6f72 2062 6173  e.same_as or bas
+0000c9e0: 652e 6465 7269 7665 645f 6672 6f6d 5f74  e.derived_from_t
+0000c9f0: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+0000ca00: 6173 7365 7274 2069 6428 6261 7365 2920  assert id(base) 
+0000ca10: 6e6f 7420 696e 2076 6973 6974 6564 2020  not in visited  
+0000ca20: 2320 7368 6f75 6c64 206e 6f74 2068 6176  # should not hav
+0000ca30: 6520 6379 636c 6573 2e20 6e6f 726d 616c  e cycles. normal
+0000ca40: 6c79 2074 6869 7320 7368 6f75 6c64 206e  ly this should n
+0000ca50: 6576 6572 2062 6520 7472 6967 6765 7265  ever be triggere
+0000ca60: 640a 2020 2020 2020 2020 2020 2020 7669  d.            vi
+0000ca70: 7369 7465 645b 6964 2862 6173 6529 5d20  sited[id(base)] 
+0000ca80: 3d20 6261 7365 0a20 2020 2020 2020 2020  = base.         
+0000ca90: 2020 2069 6620 6261 7365 2e73 616d 655f     if base.same_
+0000caa0: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
+0000cab0: 2020 2020 6261 7365 203d 2062 6173 652e      base = base.
+0000cac0: 7361 6d65 5f61 730a 2020 2020 2020 2020  same_as.        
+0000cad0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000cae0: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+0000caf0: 6520 3d20 6261 7365 2e64 6572 6976 6564  e = base.derived
+0000cb00: 5f66 726f 6d5f 7461 670a 2020 2020 2020  _from_tag.      
+0000cb10: 2020 2020 2020 6173 7365 7274 2062 6173        assert bas
+0000cb20: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0000cb30: 2062 6173 650a 0a20 2020 2064 6566 2067   base..    def g
+0000cb40: 6574 5f64 6572 6976 6564 5f62 6173 6573  et_derived_bases
+0000cb50: 5f73 6574 2873 656c 6629 3a0a 2020 2020  _set(self):.    
+0000cb60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000cb70: 3a72 7479 7065 3a20 7365 745b 4469 6d5d  :rtype: set[Dim]
+0000cb80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000cb90: 2020 2020 2072 6573 203d 2073 6574 2829       res = set()
+0000cba0: 0a20 2020 2020 2020 2071 7565 7565 203d  .        queue =
+0000cbb0: 205b 7365 6c66 5d0a 2020 2020 2020 2020   [self].        
+0000cbc0: 7669 7369 7465 6420 3d20 7b7d 2020 2320  visited = {}  # 
+0000cbd0: 7479 7065 3a20 4469 6374 5b69 6e74 2c5f  type: Dict[int,_
+0000cbe0: 642e 4469 6d5d 2020 2320 6279 2069 640a  d.Dim]  # by id.
+0000cbf0: 2020 2020 2020 2020 7768 696c 6520 7175          while qu
+0000cc00: 6575 653a 0a20 2020 2020 2020 2020 2020  eue:.           
+0000cc10: 2062 6173 6520 3d20 7175 6575 652e 706f   base = queue.po
+0000cc20: 7028 2d31 290a 2020 2020 2020 2020 2020  p(-1).          
+0000cc30: 2020 6966 2062 6173 652e 7361 6d65 5f61    if base.same_a
+0000cc40: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000cc50: 2020 2062 6173 6520 3d20 6261 7365 2e73     base = base.s
+0000cc60: 616d 655f 6173 0a20 2020 2020 2020 2020  ame_as.         
+0000cc70: 2020 2069 6620 6964 2862 6173 6529 2069     if id(base) i
+0000cc80: 6e20 7669 7369 7465 643a 0a20 2020 2020  n visited:.     
+0000cc90: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000cca0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+0000ccb0: 7669 7369 7465 645b 6964 2862 6173 6529  visited[id(base)
+0000ccc0: 5d20 3d20 6261 7365 0a20 2020 2020 2020  ] = base.       
+0000ccd0: 2020 2020 2072 6573 2e61 6464 2862 6173       res.add(bas
+0000cce0: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+0000ccf0: 6620 6261 7365 2e64 6572 6976 6564 5f66  f base.derived_f
+0000cd00: 726f 6d5f 6f70 3a0a 2020 2020 2020 2020  rom_op:.        
+0000cd10: 2020 2020 2020 2020 7175 6575 652e 6578          queue.ex
+0000cd20: 7465 6e64 2862 6173 652e 6465 7269 7665  tend(base.derive
+0000cd30: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
+0000cd40: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000cd50: 6966 2062 6173 652e 6465 7269 7665 645f  if base.derived_
+0000cd60: 6672 6f6d 5f74 6167 3a0a 2020 2020 2020  from_tag:.      
+0000cd70: 2020 2020 2020 2020 2020 7175 6575 652e            queue.
+0000cd80: 6170 7065 6e64 2862 6173 652e 6465 7269  append(base.deri
+0000cd90: 7665 645f 6672 6f6d 5f74 6167 290a 2020  ved_from_tag).  
+0000cda0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000cdb0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000cdc0: 2020 2020 6465 6620 756e 6465 6669 6e65      def undefine
+0000cdd0: 6428 7365 6c66 3a20 5f64 2e44 696d 2920  d(self: _d.Dim) 
+0000cde0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+0000cdf0: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
+0000ce00: 7475 726e 3a20 7768 6574 6865 7220 7468  turn: whether th
+0000ce10: 6520 756e 6465 6669 6e65 6420 666c 6167  e undefined flag
+0000ce20: 2069 7320 7365 742c 2069 6e20 7365 6c66   is set, in self
+0000ce30: 2c20 6261 7365 732c 206f 7220 616e 7920  , bases, or any 
+0000ce40: 6465 7269 7665 6420 6261 7365 732e 2061  derived bases. a
+0000ce50: 6c73 6f20 7365 6520 3a66 756e 633a 6069  lso see :func:`i
+0000ce60: 735f 6469 6d5f 6b6e 6f77 6e60 0a20 2020  s_dim_known`.   
+0000ce70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ce80: 2062 6173 6520 3d20 7365 6c66 0a20 2020   base = self.   
+0000ce90: 2020 2020 2076 6973 6974 6564 203d 207b       visited = {
+0000cea0: 7d0a 2020 2020 2020 2020 7768 696c 6520  }.        while 
+0000ceb0: 6261 7365 2e73 616d 655f 6173 206f 7220  base.same_as or 
+0000cec0: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000ced0: 6d5f 7461 673a 0a20 2020 2020 2020 2020  m_tag:.         
+0000cee0: 2020 2061 7373 6572 7420 6964 2862 6173     assert id(bas
+0000cef0: 6529 206e 6f74 2069 6e20 7669 7369 7465  e) not in visite
+0000cf00: 6420 2023 2073 686f 756c 6420 6e6f 7420  d  # should not 
+0000cf10: 6861 7665 2063 7963 6c65 732e 206e 6f72  have cycles. nor
+0000cf20: 6d61 6c6c 7920 7468 6973 2073 686f 756c  mally this shoul
+0000cf30: 6420 6e65 7665 7220 6265 2074 7269 6767  d never be trigg
+0000cf40: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
+0000cf50: 2076 6973 6974 6564 5b69 6428 6261 7365   visited[id(base
+0000cf60: 295d 203d 2062 6173 650a 2020 2020 2020  )] = base.      
+0000cf70: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
+0000cf80: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
+0000cf90: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
+0000cfa0: 2020 2069 6620 6261 7365 2e5f 6578 7472     if base._extr
+0000cfb0: 6120 616e 6420 6261 7365 2e5f 6578 7472  a and base._extr
+0000cfc0: 612e 756e 6465 6669 6e65 643a 0a20 2020  a.undefined:.   
+0000cfd0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000cfe0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0000cff0: 2020 2020 2069 6620 6261 7365 2e73 616d       if base.sam
+0000d000: 655f 6173 3a0a 2020 2020 2020 2020 2020  e_as:.          
+0000d010: 2020 2020 2020 6261 7365 203d 2062 6173        base = bas
+0000d020: 652e 7361 6d65 5f61 730a 2020 2020 2020  e.same_as.      
+0000d030: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0000d040: 7565 0a20 2020 2020 2020 2020 2020 2062  ue.            b
+0000d050: 6173 6520 3d20 6261 7365 2e64 6572 6976  ase = base.deriv
+0000d060: 6564 5f66 726f 6d5f 7461 670a 2020 2020  ed_from_tag.    
+0000d070: 2020 2020 2020 2020 6173 7365 7274 2062          assert b
+0000d080: 6173 650a 2020 2020 2020 2020 2320 6e6f  ase.        # no
+0000d090: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
+0000d0a0: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
+0000d0b0: 2020 2020 2072 6574 7572 6e20 6261 7365       return base
+0000d0c0: 2e5f 6578 7472 6120 616e 6420 6261 7365  ._extra and base
+0000d0d0: 2e5f 6578 7472 612e 756e 6465 6669 6e65  ._extra.undefine
+0000d0e0: 640a 0a20 2020 2064 6566 2064 6563 6c61  d..    def decla
+0000d0f0: 7265 5f73 616d 655f 6173 2873 656c 663a  re_same_as(self:
+0000d100: 205f 642e 4469 6d2c 206f 7468 6572 3a20   _d.Dim, other: 
+0000d110: 5f64 2e44 696d 293a 0a20 2020 2020 2020  _d.Dim):.       
+0000d120: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+0000d130: 7261 6d20 6f74 6865 723a 0a20 2020 2020  ram other:.     
+0000d140: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+0000d150: 7373 6572 7420 7365 6c66 2e63 616e 5f62  ssert self.can_b
+0000d160: 655f 7573 6564 5f61 735f 6469 6d28 2920  e_used_as_dim() 
+0000d170: 616e 6420 6f74 6865 722e 6361 6e5f 6265  and other.can_be
+0000d180: 5f75 7365 645f 6173 5f64 696d 2829 2020  _used_as_dim()  
+0000d190: 2320 6465 636c 6172 655f 7361 6d65 5f61  # declare_same_a
+0000d1a0: 7320 646f 6573 206e 6f74 206d 616b 6520  s does not make 
+0000d1b0: 7365 6e73 6520 6f74 6865 7277 6973 650a  sense otherwise.
+0000d1c0: 2020 2020 2020 2020 2320 4e6f 7465 3a20          # Note: 
+0000d1d0: 4368 6563 6b20 6069 7360 2c20 6e6f 7420  Check `is`, not 
+0000d1e0: 603d 3d60 2e20 603d 3d60 2063 616e 2062  `==`. `==` can b
+0000d1f0: 6520 7472 7565 2065 7665 6e20 7468 6f75  e true even thou
+0000d200: 6768 2073 616d 655f 6173 2061 7265 206e  gh same_as are n
+0000d210: 6f74 2074 6865 2073 616d 6520 696e 7374  ot the same inst
+0000d220: 616e 6365 2c0a 2020 2020 2020 2020 2320  ance,.        # 
+0000d230: 652e 672e 2076 6961 2061 7574 6f5f 6765  e.g. via auto_ge
+0000d240: 6e65 7261 7465 642e 0a20 2020 2020 2020  nerated..       
+0000d250: 2069 6620 7365 6c66 2069 7320 6f74 6865   if self is othe
+0000d260: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+0000d270: 6574 7572 6e0a 2020 2020 2020 2020 7365  eturn.        se
+0000d280: 6c66 2e5f 6d61 7962 655f 7570 6461 7465  lf._maybe_update
+0000d290: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000d2a0: 5f76 616c 6964 6174 655f 696e 5f63 7572  _validate_in_cur
+0000d2b0: 7265 6e74 5f67 7261 7068 2829 0a20 2020  rent_graph().   
+0000d2c0: 2020 2020 206f 7468 6572 2e5f 7661 6c69       other._vali
+0000d2d0: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
+0000d2e0: 6772 6170 6828 290a 2020 2020 2020 2020  graph().        
+0000d2f0: 6f74 6865 725f 7361 6d65 5f62 6173 6520  other_same_base 
+0000d300: 3d20 6f74 6865 722e 6765 745f 7361 6d65  = other.get_same
+0000d310: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
+0000d320: 6966 2073 656c 6620 6973 206f 7468 6572  if self is other
+0000d330: 5f73 616d 655f 6261 7365 206f 7220 7365  _same_base or se
+0000d340: 6c66 2e73 616d 655f 6173 2069 7320 6f74  lf.same_as is ot
+0000d350: 6865 725f 7361 6d65 5f62 6173 653a 0a20  her_same_base:. 
+0000d360: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d370: 6e0a 2020 2020 2020 2020 7365 6c66 5f73  n.        self_s
+0000d380: 616d 655f 6173 203d 2073 656c 662e 6765  ame_as = self.ge
+0000d390: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
+0000d3a0: 2020 2020 2020 6966 2073 656c 665f 7361        if self_sa
+0000d3b0: 6d65 5f61 7320 6973 206f 7468 6572 5f73  me_as is other_s
+0000d3c0: 616d 655f 6261 7365 3a0a 2020 2020 2020  ame_base:.      
+0000d3d0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000d3e0: 2020 2020 2069 6620 6f74 6865 725f 7361       if other_sa
+0000d3f0: 6d65 5f62 6173 652e 6765 745f 7361 6d65  me_base.get_same
+0000d400: 5f64 6572 6976 6564 5f62 6173 6528 2920  _derived_base() 
+0000d410: 6973 2073 656c 665f 7361 6d65 5f61 733a  is self_same_as:
+0000d420: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+0000d430: 6520 6163 7475 616c 6c79 2077 616e 7420  e actually want 
+0000d440: 6974 2074 6f20 6265 2074 6865 206f 7468  it to be the oth
+0000d450: 6572 2077 6179 2061 726f 756e 642e 0a20  er way around.. 
+0000d460: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000d470: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
+0000d480: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
+0000d490: 2e44 696d 2e64 6563 6c61 7265 5f73 616d  .Dim.declare_sam
+0000d4a0: 655f 6173 2c20 6f74 6865 722c 2073 656c  e_as, other, sel
+0000d4b0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
+0000d4c0: 2020 2020 7265 7475 726e 206f 7468 6572      return other
+0000d4d0: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
+0000d4e0: 2873 656c 6629 0a20 2020 2020 2020 2069  (self).        i
+0000d4f0: 6620 7365 6c66 2e62 6174 6368 3a0a 2020  f self.batch:.  
+0000d500: 2020 2020 2020 2020 2020 2320 4966 2073            # If s
+0000d510: 656c 6620 6973 2064 6566 696e 6564 2028  elf is defined (
+0000d520: 7365 6c66 2e69 735f 6469 6d5f 6b6e 6f77  self.is_dim_know
+0000d530: 6e29 2c20 6265 2066 6169 7220 746f 206f  n), be fair to o
+0000d540: 7468 6572 2c20 616e 6420 6164 6170 7420  ther, and adapt 
+0000d550: 6974 2074 6f20 7468 6520 7269 6768 7420  it to the right 
+0000d560: 6261 7463 682c 0a20 2020 2020 2020 2020  batch,.         
+0000d570: 2020 2023 2073 7563 6820 7468 6174 206f     # such that o
+0000d580: 7468 6572 2e69 735f 6469 6d5f 6b6e 6f77  ther.is_dim_know
+0000d590: 6e20 6973 2063 6f72 7265 6374 2c20 6279  n is correct, by
+0000d5a0: 2070 6f74 656e 7469 616c 6c79 2063 6f6d   potentially com
+0000d5b0: 706c 6574 696e 6720 6974 2e0a 2020 2020  pleting it..    
+0000d5c0: 2020 2020 2020 2020 6f74 6865 725f 203d          other_ =
+0000d5d0: 206f 7468 6572 2e67 6574 5f66 6f72 5f62   other.get_for_b
+0000d5e0: 6174 6368 5f63 7478 2873 656c 662e 6261  atch_ctx(self.ba
+0000d5f0: 7463 682c 2063 7478 3d73 656c 662e 636f  tch, ctx=self.co
+0000d600: 6e74 726f 6c5f 666c 6f77 5f63 7478 290a  ntrol_flow_ctx).
+0000d610: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000d620: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
+0000d630: 203d 206f 7468 6572 0a20 2020 2020 2020   = other.       
+0000d640: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+0000d650: 2020 2873 656c 662e 6973 5f64 696d 5f6b    (self.is_dim_k
+0000d660: 6e6f 776e 2829 2061 6e64 206e 6f74 206f  nown() and not o
+0000d670: 7468 6572 5f2e 6973 5f64 696d 5f6b 6e6f  ther_.is_dim_kno
+0000d680: 776e 2829 290a 2020 2020 2020 2020 2020  wn()).          
+0000d690: 2020 6f72 0a20 2020 2020 2020 2020 2020    or.           
+0000d6a0: 2023 204c 696b 6520 6973 5f64 696d 5f6b   # Like is_dim_k
+0000d6b0: 6e6f 776e 2062 7574 2066 6f72 2073 7461  nown but for sta
+0000d6c0: 7469 6320 6469 6d73 2c20 7765 206d 6967  tic dims, we mig
+0000d6d0: 6874 206b 6e6f 7720 626f 7468 2c0a 2020  ht know both,.  
+0000d6e0: 2020 2020 2020 2020 2020 2320 6275 7420            # but 
+0000d6f0: 7468 6520 6465 7269 7665 645f 6672 6f6d  the derived_from
+0000d700: 5f6f 7020 7374 696c 6c20 776f 756c 6420  _op still would 
+0000d710: 7072 6f76 6964 6520 6d6f 7265 2069 6e66  provide more inf
+0000d720: 6f72 6d61 7469 6f6e 2e0a 2020 2020 2020  ormation..      
+0000d730: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+0000d740: 2020 2020 2020 2020 7365 6c66 5f73 616d          self_sam
+0000d750: 655f 6173 2e64 6572 6976 6564 5f66 726f  e_as.derived_fro
+0000d760: 6d5f 6f70 0a20 2020 2020 2020 2020 2020  m_op.           
+0000d770: 2020 2020 2061 6e64 206e 6f74 206f 7468       and not oth
+0000d780: 6572 5f73 616d 655f 6261 7365 2e64 6572  er_same_base.der
+0000d790: 6976 6564 5f66 726f 6d5f 6f70 0a20 2020  ived_from_op.   
+0000d7a0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+0000d7b0: 206f 7468 6572 206e 6f74 2069 6e20 7365   other not in se
+0000d7c0: 6c66 2e67 6574 5f64 6572 6976 6564 5f62  lf.get_derived_b
+0000d7d0: 6173 6573 5f73 6574 2829 0a20 2020 2020  ases_set().     
+0000d7e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d7f0: 2020 2020 206f 7220 286e 6f74 2073 656c       or (not sel
+0000d800: 662e 756e 6465 6669 6e65 6420 616e 6420  f.undefined and 
+0000d810: 6f74 6865 725f 2e75 6e64 6566 696e 6564  other_.undefined
+0000d820: 290a 2020 2020 2020 2020 293a 0a20 2020  ).        ):.   
+0000d830: 2020 2020 2020 2020 2077 6974 6820 7574           with ut
+0000d840: 696c 2e67 7561 7264 5f69 6e66 696e 6974  il.guard_infinit
+0000d850: 655f 7265 6375 7273 696f 6e28 5f64 2e44  e_recursion(_d.D
+0000d860: 696d 2e64 6563 6c61 7265 5f73 616d 655f  im.declare_same_
+0000d870: 6173 2c20 6f74 6865 722c 2073 656c 6629  as, other, self)
+0000d880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d890: 2020 7265 7475 726e 206f 7468 6572 2e64    return other.d
+0000d8a0: 6563 6c61 7265 5f73 616d 655f 6173 2873  eclare_same_as(s
+0000d8b0: 656c 6629 0a20 2020 2020 2020 206f 7468  elf).        oth
+0000d8c0: 6572 5f64 6572 6976 6564 5f62 6173 6573  er_derived_bases
+0000d8d0: 203d 206f 7468 6572 2e67 6574 5f64 6572   = other.get_der
+0000d8e0: 6976 6564 5f62 6173 6573 5f73 6574 2829  ived_bases_set()
+0000d8f0: 0a20 2020 2020 2020 2073 656c 665f 6465  .        self_de
+0000d900: 7269 7665 645f 6261 7365 7320 3d20 7365  rived_bases = se
+0000d910: 6c66 2e67 6574 5f64 6572 6976 6564 5f62  lf.get_derived_b
+0000d920: 6173 6573 5f73 6574 2829 0a20 2020 2020  ases_set().     
+0000d930: 2020 2069 6620 6f74 6865 725f 6465 7269     if other_deri
+0000d940: 7665 645f 6261 7365 7320 213d 2073 656c  ved_bases != sel
+0000d950: 665f 6465 7269 7665 645f 6261 7365 7320  f_derived_bases 
+0000d960: 616e 6420 7365 6c66 5f64 6572 6976 6564  and self_derived
+0000d970: 5f62 6173 6573 2e69 7373 7562 7365 7428  _bases.issubset(
+0000d980: 6f74 6865 725f 6465 7269 7665 645f 6261  other_derived_ba
+0000d990: 7365 7329 3a0a 2020 2020 2020 2020 2020  ses):.          
+0000d9a0: 2020 2320 4176 6f69 6420 6379 636c 6573    # Avoid cycles
+0000d9b0: 206f 6e20 6465 7269 7665 645f 6672 6f6d   on derived_from
+0000d9c0: 5f74 6167 2e20 6874 7470 733a 2f2f 6769  _tag. https://gi
+0000d9d0: 7468 7562 2e63 6f6d 2f72 7774 682d 6936  thub.com/rwth-i6
+0000d9e0: 2f72 6574 7572 6e6e 2f69 7373 7565 732f  /returnn/issues/
+0000d9f0: 3130 3534 0a20 2020 2020 2020 2020 2020  1054.           
+0000da00: 2077 6974 6820 7574 696c 2e67 7561 7264   with util.guard
+0000da10: 5f69 6e66 696e 6974 655f 7265 6375 7273  _infinite_recurs
+0000da20: 696f 6e28 5f64 2e44 696d 2e64 6563 6c61  ion(_d.Dim.decla
+0000da30: 7265 5f73 616d 655f 6173 2c20 6f74 6865  re_same_as, othe
+0000da40: 722c 2073 656c 6629 3a0a 2020 2020 2020  r, self):.      
+0000da50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000da60: 206f 7468 6572 2e64 6563 6c61 7265 5f73   other.declare_s
+0000da70: 616d 655f 6173 2873 656c 6629 0a20 2020  ame_as(self).   
+0000da80: 2020 2020 2069 6620 7365 6c66 2e5f 6578       if self._ex
+0000da90: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+0000daa0: 2073 656c 662e 5f65 7874 7261 2e64 6572   self._extra.der
+0000dab0: 6976 6564 5f66 726f 6d5f 6f70 203d 204e  ived_from_op = N
+0000dac0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000dad0: 7365 6c66 2e5f 6578 7472 612e 6465 7269  self._extra.deri
+0000dae0: 7665 645f 6672 6f6d 5f74 6167 203d 204e  ved_from_tag = N
+0000daf0: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
+0000db00: 656c 665f 7361 6d65 5f61 7320 6973 206e  elf_same_as is n
+0000db10: 6f74 2073 656c 663a 0a20 2020 2020 2020  ot self:.       
+0000db20: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
+0000db30: 7365 6c66 5f73 616d 655f 6173 2e73 616d  self_same_as.sam
+0000db40: 655f 6173 0a20 2020 2020 2020 2020 2020  e_as.           
+0000db50: 2069 6620 7365 6c66 5f73 616d 655f 6173   if self_same_as
+0000db60: 2069 7320 6f74 6865 725f 7361 6d65 5f62   is other_same_b
+0000db70: 6173 653a 0a20 2020 2020 2020 2020 2020  ase:.           
+0000db80: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000db90: 2020 2020 2020 2020 7769 7468 2075 7469          with uti
+0000dba0: 6c2e 6775 6172 645f 696e 6669 6e69 7465  l.guard_infinite
+0000dbb0: 5f72 6563 7572 7369 6f6e 285f 642e 4469  _recursion(_d.Di
+0000dbc0: 6d2e 6465 636c 6172 655f 7361 6d65 5f61  m.declare_same_a
+0000dbd0: 732c 2073 656c 665f 7361 6d65 5f61 732c  s, self_same_as,
+0000dbe0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000dbf0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000dc00: 2020 2073 656c 665f 7361 6d65 5f61 732e     self_same_as.
+0000dc10: 6465 636c 6172 655f 7361 6d65 5f61 7328  declare_same_as(
+0000dc20: 6f74 6865 725f 7361 6d65 5f62 6173 6529  other_same_base)
+0000dc30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000dc40: 2873 656c 662e 6479 6e5f 7369 7a65 5f65  (self.dyn_size_e
+0000dc50: 7874 2069 7320 4e6f 6e65 206f 7220 6e6f  xt is None or no
+0000dc60: 7420 7365 6c66 2e5f 7661 6c69 6461 7465  t self._validate
+0000dc70: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
+0000dc80: 6828 2929 2061 6e64 2073 656c 665f 7361  h()) and self_sa
+0000dc90: 6d65 5f61 732e 6479 6e5f 7369 7a65 5f65  me_as.dyn_size_e
+0000dca0: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+0000dcb0: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
+0000dcc0: 655f 6578 7420 3d20 7365 6c66 5f73 616d  e_ext = self_sam
+0000dcd0: 655f 6173 2e67 6574 5f64 796e 5f73 697a  e_as.get_dyn_siz
+0000dce0: 655f 6578 745f 666f 725f 6261 7463 685f  e_ext_for_batch_
+0000dcf0: 6374 7828 0a20 2020 2020 2020 2020 2020  ctx(.           
+0000dd00: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
+0000dd10: 7463 682c 2073 656c 662e 636f 6e74 726f  tch, self.contro
+0000dd20: 6c5f 666c 6f77 5f63 7478 2c20 7465 6d70  l_flow_ctx, temp
+0000dd30: 6c61 7465 5f6f 6e6c 793d 5472 7565 0a20  late_only=True. 
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000dd50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000dd60: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000dd70: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
+0000dd80: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
+0000dd90: 696d 5f20 696e 2073 656c 662e 5f65 7874  im_ in self._ext
+0000dda0: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+0000ddb0: 685f 6374 782e 7661 6c75 6573 2829 3a0a  h_ctx.values():.
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddd0: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+0000dde0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+0000ddf0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+0000de00: 2020 2020 2020 2020 2069 6620 6469 6d5f           if dim_
+0000de10: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
+0000de40: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
+0000de50: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000de60: 2020 2020 2020 2020 2020 6469 6d5f 2e5f            dim_._
+0000de70: 6578 7472 612e 6465 7269 7665 645f 6672  extra.derived_fr
+0000de80: 6f6d 5f6f 7020 3d20 4e6f 6e65 0a20 2020  om_op = None.   
+0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dea0: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
+0000deb0: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
+0000dec0: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
+0000ded0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0000dee0: 6d5f 2e5f 6578 7472 612e 6465 7269 7665  m_._extra.derive
+0000def0: 645f 6672 6f6d 5f74 6167 203d 204e 6f6e  d_from_tag = Non
+0000df00: 650a 2020 2020 2020 2020 2320 4e6f 7720  e.        # Now 
+0000df10: 6d65 7267 6520 6578 6973 7469 6e67 2076  merge existing v
+0000df20: 6172 6961 6e74 732e 2042 7574 206f 6e6c  ariants. But onl
+0000df30: 7920 6966 206e 6f74 2064 6572 6976 6564  y if not derived
+0000df40: 2076 6961 206f 702c 2062 6563 6175 7365   via op, because
+0000df50: 2069 6e20 7468 6174 2063 6173 652c 2077   in that case, w
+0000df60: 6520 6361 6e20 2861 6e64 2073 686f 756c  e can (and shoul
+0000df70: 6421 290a 2020 2020 2020 2020 2320 6175  d!).        # au
+0000df80: 746f 6d61 7469 6361 6c6c 7920 696e 6665  tomatically infe
+0000df90: 7220 6974 2e20 4e6f 7465 2074 6861 7420  r it. Note that 
+0000dfa0: 7765 206f 6e6c 7920 676f 7420 6865 7265  we only got here
+0000dfb0: 2077 6865 6e20 7468 6520 6f74 6865 7220   when the other 
+0000dfc0: 6973 206e 6f74 2074 6865 2073 616d 6520  is not the same 
+0000dfd0: 6469 6d2c 2073 6f20 6974 206d 6561 6e73  dim, so it means
+0000dfe0: 2074 6861 740a 2020 2020 2020 2020 2320   that.        # 
+0000dff0: 7468 6520 6f74 6865 7220 6973 2072 6561  the other is rea
+0000e000: 6c6c 7920 6469 6666 6572 656e 742c 2074  lly different, t
+0000e010: 6865 2073 697a 6573 2061 7265 2070 6f74  he sizes are pot
+0000e020: 656e 7469 616c 6c79 2064 6966 6665 7265  entially differe
+0000e030: 6e74 2c20 6275 7420 7765 2077 616e 7420  nt, but we want 
+0000e040: 746f 206f 7665 7274 616b 6520 7468 6520  to overtake the 
+0000e050: 6f74 6865 722e 0a20 2020 2020 2020 2069  other..        i
+0000e060: 6620 6f74 6865 725f 7361 6d65 5f62 6173  f other_same_bas
+0000e070: 652e 6465 7269 7665 645f 6672 6f6d 5f6f  e.derived_from_o
+0000e080: 703a 0a20 2020 2020 2020 2020 2020 2023  p:.            #
+0000e090: 2043 6c65 616e 7570 2065 7665 7279 7468   Cleanup everyth
+0000e0a0: 696e 672c 2065 7370 2070 6f74 656e 7469  ing, esp potenti
+0000e0b0: 616c 2061 6c72 6561 6479 2063 6f6d 7075  al already compu
+0000e0c0: 7465 6420 7369 7a65 732c 2061 7320 7468  ted sizes, as th
+0000e0d0: 6573 6520 6d69 6768 7420 6265 2069 6e76  ese might be inv
+0000e0e0: 616c 6964 2e0a 2020 2020 2020 2020 2020  alid..          
+0000e0f0: 2020 666f 7220 6469 6d5f 2069 6e20 5b73    for dim_ in [s
+0000e100: 656c 665f 7361 6d65 5f61 732c 2073 656c  elf_same_as, sel
+0000e110: 665d 202b 2028 6c69 7374 2873 656c 662e  f] + (list(self.
+0000e120: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000e130: 6261 7463 685f 6374 782e 7661 6c75 6573  batch_ctx.values
+0000e140: 2829 2920 6966 2073 656c 662e 5f65 7874  ()) if self._ext
+0000e150: 7261 2065 6c73 6520 5b5d 293a 0a20 2020  ra else []):.   
+0000e160: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e170: 6469 6d5f 2e64 796e 5f73 697a 655f 6578  dim_.dyn_size_ex
+0000e180: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000e190: 2020 2020 2020 2064 696d 5f2e 6479 6e5f         dim_.dyn_
+0000e1a0: 7369 7a65 5f65 7874 2e70 6c61 6365 686f  size_ext.placeho
+0000e1b0: 6c64 6572 203d 204e 6f6e 650a 2020 2020  lder = None.    
+0000e1c0: 2020 2020 6f74 6865 725f 7361 6d65 5f62      other_same_b
+0000e1d0: 6173 652e 5f6d 6572 6765 5f73 616d 655f  ase._merge_same_
+0000e1e0: 666f 725f 6261 7463 685f 6374 785f 6469  for_batch_ctx_di
+0000e1f0: 6374 2873 656c 6629 0a20 2020 2020 2020  ct(self).       
+0000e200: 206f 7468 6572 2e5f 6d61 7962 655f 7570   other._maybe_up
+0000e210: 6461 7465 2829 0a20 2020 2020 2020 2073  date().        s
+0000e220: 656c 662e 7361 6d65 5f61 7320 3d20 6f74  elf.same_as = ot
+0000e230: 6865 725f 7361 6d65 5f62 6173 650a 2020  her_same_base.  
+0000e240: 2020 2020 2020 7365 6c66 2e5f 6d61 7962        self._mayb
+0000e250: 655f 7570 6461 7465 2829 0a20 2020 2020  e_update().     
+0000e260: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
+0000e270: 697a 6520 6973 206e 6f74 204e 6f6e 6520  ize is not None 
+0000e280: 616e 6420 6f74 6865 725f 7361 6d65 5f62  and other_same_b
+0000e290: 6173 652e 6479 6e5f 7369 7a65 2069 7320  ase.dyn_size is 
+0000e2a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000e2b0: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
+0000e2c0: 6e5f 7369 7a65 2069 7320 6e6f 7420 6f74  n_size is not ot
+0000e2d0: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
+0000e2e0: 6e5f 7369 7a65 3a0a 2020 2020 2020 2020  n_size:.        
+0000e2f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000e300: 6261 7463 6820 3d3d 206f 7468 6572 5f73  batch == other_s
+0000e310: 616d 655f 6261 7365 2e62 6174 6368 2061  ame_base.batch a
+0000e320: 6e64 2073 656c 662e 636f 6e74 726f 6c5f  nd self.control_
+0000e330: 666c 6f77 5f63 7478 203d 3d20 6f74 6865  flow_ctx == othe
+0000e340: 725f 7361 6d65 5f62 6173 652e 636f 6e74  r_same_base.cont
+0000e350: 726f 6c5f 666c 6f77 5f63 7478 3a0a 2020  rol_flow_ctx:.  
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e370: 2020 2320 4e6f 7465 3a20 496e 7374 6561    # Note: Instea
+0000e380: 6420 6f66 206d 616b 696e 6720 7468 6973  d of making this
+0000e390: 2061 2077 6172 6e69 6e67 2c20 7765 2063   a warning, we c
+0000e3a0: 6f75 6c64 2061 6c73 6f20 656e 666f 7263  ould also enforc
+0000e3b0: 6520 7468 6973 2061 7420 736f 6d65 2070  e this at some p
+0000e3c0: 6f69 6e74 2e0a 2020 2020 2020 2020 2020  oint..          
+0000e3d0: 2020 2020 2020 2020 2020 2320 2020 5468            #   Th
+0000e3e0: 6520 7573 6572 2073 686f 756c 6420 6265  e user should be
+0000e3f0: 2061 626c 6520 746f 2066 6978 2060 6578   able to fix `ex
+0000e400: 7465 726e 5f64 6174 6160 2069 6e20 7468  tern_data` in th
+0000e410: 6520 636f 6e66 6967 0a20 2020 2020 2020  e config.       
+0000e420: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+0000e430: 2073 7563 6820 7468 6174 2074 6869 7320   such that this 
+0000e440: 6973 2063 6f72 7265 6374 2069 6e20 7468  is correct in th
+0000e450: 6520 6669 7273 7420 706c 6163 652e 0a20  e first place.. 
+0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e470: 2020 2023 2020 2041 6c73 6f2c 2069 6e20     #   Also, in 
+0000e480: 6164 6469 7469 6f6e 2074 6f20 7468 6973  addition to this
+0000e490: 2077 6172 6e69 6e67 2c0a 2020 2020 2020   warning,.      
+0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e4b0: 2020 7765 206d 6967 6874 2077 616e 7420    we might want 
+0000e4c0: 746f 2061 6464 2073 6f6d 6520 7275 6e74  to add some runt
+0000e4d0: 696d 6520 6368 6563 6b20 6f6e 2074 6865  ime check on the
+0000e4e0: 2065 7120 6f66 2074 6865 2064 796e 2073   eq of the dyn s
+0000e4f0: 697a 6573 2e0a 2020 2020 2020 2020 2020  izes..          
+0000e500: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000e510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e520: 2020 2020 2020 2020 2022 5761 726e 696e           "Warnin
+0000e530: 673a 2061 7373 756d 696e 6720 6469 6d20  g: assuming dim 
+0000e540: 7461 6773 2061 7265 2073 616d 6520 7769  tags are same wi
+0000e550: 7468 2064 6966 6665 7265 6e74 2073 697a  th different siz
+0000e560: 6520 706c 6163 6568 6f6c 6465 7273 3a20  e placeholders: 
+0000e570: 2572 2076 7320 2572 220a 2020 2020 2020  %r vs %r".      
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2520 2873 656c 662e 6479 6e5f 7369    % (self.dyn_si
+0000e5a0: 7a65 2c20 6f74 6865 725f 7361 6d65 5f62  ze, other_same_b
+0000e5b0: 6173 652e 6479 6e5f 7369 7a65 290a 2020  ase.dyn_size).  
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 2020 290a 2020 2020 2020 2020 2320 4966    ).        # If
+0000e5e0: 2077 6520 6861 7665 2061 2064 6566 696e   we have a defin
+0000e5f0: 6564 2073 6f75 7263 652c 2061 6e64 2074  ed source, and t
+0000e600: 6869 7320 6973 2061 2064 796e 616d 6963  his is a dynamic
+0000e610: 2073 7061 7469 616c 2061 7869 732c 2061   spatial axis, a
+0000e620: 6e64 2069 7420 7761 7320 756e 6465 6669  nd it was undefi
+0000e630: 6e65 6420 6265 666f 7265 2c0a 2020 2020  ned before,.    
+0000e640: 2020 2020 2320 6d61 7962 6520 7765 2063      # maybe we c
+0000e650: 616e 206f 7665 7274 616b 6520 7468 6520  an overtake the 
+0000e660: 7369 7a65 5f70 6c61 6365 686f 6c64 6572  size_placeholder
+0000e670: 206e 6f77 2e0a 2020 2020 2020 2020 6966   now..        if
+0000e680: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000e690: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
+0000e6a0: 204e 6f6e 6520 616e 6420 7365 6c66 2e5f   None and self._
+0000e6b0: 6578 7472 6120 616e 6420 7365 6c66 2e5f  extra and self._
+0000e6c0: 6578 7472 612e 7372 635f 6461 7461 3a0a  extra.src_data:.
+0000e6d0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000e6e0: 7274 2069 7369 6e73 7461 6e63 6528 7365  rt isinstance(se
+0000e6f0: 6c66 2e5f 6578 7472 612e 7372 635f 6178  lf._extra.src_ax
+0000e700: 6973 2c20 696e 7429 0a20 2020 2020 2020  is, int).       
+0000e710: 2020 2020 2023 204d 6179 6265 2069 7420       # Maybe it 
+0000e720: 6368 616e 6765 6420 696e 2074 6865 206d  changed in the m
+0000e730: 6561 6e77 6869 6c65 2c20 736f 2063 6865  eanwhile, so che
+0000e740: 636b 2e0a 2020 2020 2020 2020 2020 2020  ck..            
+0000e750: 7461 6720 3d20 7365 6c66 2e5f 6578 7472  tag = self._extr
+0000e760: 612e 7372 635f 6461 7461 2e67 6574 5f64  a.src_data.get_d
+0000e770: 696d 5f74 6167 2873 656c 662e 5f65 7874  im_tag(self._ext
+0000e780: 7261 2e73 7263 5f61 7869 7329 0a20 2020  ra.src_axis).   
+0000e790: 2020 2020 2020 2020 2069 6620 7461 672e           if tag.
+0000e7a0: 6465 7363 7269 7074 696f 6e20 3d3d 2073  description == s
+0000e7b0: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
+0000e7c0: 616e 6420 286e 6f74 2074 6167 2e64 796e  and (not tag.dyn
+0000e7d0: 5f73 697a 655f 6578 7420 6f72 206e 6f74  _size_ext or not
+0000e7e0: 2074 6167 2e5f 7661 6c69 6461 7465 5f69   tag._validate_i
+0000e7f0: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000e800: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000e810: 2020 2020 7461 672e 6479 6e5f 7369 7a65      tag.dyn_size
+0000e820: 5f65 7874 203d 2073 656c 662e 6765 745f  _ext = self.get_
+0000e830: 6479 6e5f 7369 7a65 5f65 7874 5f66 6f72  dyn_size_ext_for
+0000e840: 5f62 6174 6368 5f63 7478 280a 2020 2020  _batch_ctx(.    
+0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e860: 7461 672e 6261 7463 682c 2074 6167 2e63  tag.batch, tag.c
+0000e870: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 782c  ontrol_flow_ctx,
+0000e880: 2074 656d 706c 6174 655f 6f6e 6c79 3d54   template_only=T
+0000e890: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000e8a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000e8b0: 2020 2020 2020 7461 672e 5f6d 6179 6265        tag._maybe
+0000e8c0: 5f75 7064 6174 6528 290a 2020 2020 2020  _update().      
+0000e8d0: 2020 2320 4966 206f 7468 6572 7320 6479    # If others dy
+0000e8e0: 6e5f 7369 7a65 2069 7320 4e6f 6e65 2062  n_size is None b
+0000e8f0: 7574 2077 6520 6861 7665 2061 2064 796e  ut we have a dyn
+0000e900: 5f73 697a 652c 206d 6179 6265 2075 7064  _size, maybe upd
+0000e910: 6174 6520 6f74 6865 7273 2064 796e 5f73  ate others dyn_s
+0000e920: 697a 652e 0a20 2020 2020 2020 2069 6620  ize..        if 
+0000e930: 7365 6c66 2e64 796e 5f73 697a 6520 6973  self.dyn_size is
+0000e940: 206e 6f74 204e 6f6e 6520 616e 6420 6f74   not None and ot
+0000e950: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
+0000e960: 6e5f 7369 7a65 2069 7320 6e6f 7420 7365  n_size is not se
+0000e970: 6c66 2e64 796e 5f73 697a 653a 0a20 2020  lf.dyn_size:.   
+0000e980: 2020 2020 2020 2020 2023 2043 6f75 6c64           # Could
+0000e990: 2062 6520 756e 7365 7420 6966 2069 7420   be unset if it 
+0000e9a0: 636f 6d65 7320 6672 6f6d 2074 6865 2063  comes from the c
+0000e9b0: 6f6e 6669 672c 206f 7220 6672 6f6d 2070  onfig, or from p
+0000e9c0: 7265 7620 6772 6170 6820 6372 6561 7469  rev graph creati
+0000e9d0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+0000e9e0: 2320 5468 6973 2069 7320 696d 706f 7274  # This is import
+0000e9f0: 616e 7420 7375 6368 2074 6861 7420 7365  ant such that se
+0000ea00: 6c66 2e63 616e 5f63 6f6d 7061 7265 2829  lf.can_compare()
+0000ea10: 2069 7320 7361 6e65 2e0a 2020 2020 2020   is sane..      
+0000ea20: 2020 2020 2020 6966 206f 7468 6572 5f73        if other_s
+0000ea30: 616d 655f 6261 7365 2e64 796e 5f73 697a  ame_base.dyn_siz
+0000ea40: 6520 6973 204e 6f6e 6520 6f72 206e 6f74  e is None or not
+0000ea50: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000ea60: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+0000ea70: 7272 656e 745f 6772 6170 6828 293a 0a20  rrent_graph():. 
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000ea90: 7468 6572 5f73 616d 655f 6261 7365 2e64  ther_same_base.d
+0000eaa0: 796e 5f73 697a 655f 6578 7420 3d20 7365  yn_size_ext = se
+0000eab0: 6c66 2e67 6574 5f64 796e 5f73 697a 655f  lf.get_dyn_size_
+0000eac0: 6578 745f 666f 725f 6261 7463 685f 6374  ext_for_batch_ct
+0000ead0: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
+0000eae0: 2020 2020 2020 206f 7468 6572 5f73 616d         other_sam
+0000eaf0: 655f 6261 7365 2e62 6174 6368 2c20 6f74  e_base.batch, ot
+0000eb00: 6865 725f 7361 6d65 5f62 6173 652e 636f  her_same_base.co
+0000eb10: 6e74 726f 6c5f 666c 6f77 5f63 7478 2c20  ntrol_flow_ctx, 
+0000eb20: 7465 6d70 6c61 7465 5f6f 6e6c 793d 5472  template_only=Tr
+0000eb30: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+0000eb40: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000eb50: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
+0000eb60: 6261 7365 2e5f 6d61 7962 655f 7570 6461  base._maybe_upda
+0000eb70: 7465 2829 0a20 2020 2020 2020 2069 6620  te().        if 
+0000eb80: 6e6f 7420 7365 6c66 2e64 796e 5f73 697a  not self.dyn_siz
+0000eb90: 655f 6578 7420 6f72 206e 6f74 2073 656c  e_ext or not sel
+0000eba0: 662e 5f76 616c 6964 6174 655f 696e 5f63  f._validate_in_c
+0000ebb0: 7572 7265 6e74 5f67 7261 7068 2829 3a0a  urrent_graph():.
+0000ebc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ebd0: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
+0000ebe0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000ebf0: 6765 745f 6479 6e5f 7369 7a65 5f65 7874  get_dyn_size_ext
+0000ec00: 5f66 6f72 5f62 6174 6368 5f63 7478 280a  _for_batch_ctx(.
+0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec20: 7365 6c66 2e62 6174 6368 2c20 7365 6c66  self.batch, self
+0000ec30: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000ec40: 782c 2074 656d 706c 6174 655f 6f6e 6c79  x, template_only
+0000ec50: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
+0000ec60: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000ec70: 7365 6c66 2e5f 6d61 7962 655f 7570 6461  self._maybe_upda
+0000ec80: 7465 2829 0a20 2020 2020 2020 2065 6c69  te().        eli
+0000ec90: 6620 6f74 6865 725f 7361 6d65 5f62 6173  f other_same_bas
+0000eca0: 652e 6479 6e5f 7369 7a65 5f65 7874 2069  e.dyn_size_ext i
+0000ecb0: 7320 4e6f 6e65 206f 7220 6e6f 7420 6f74  s None or not ot
+0000ecc0: 6865 725f 7361 6d65 5f62 6173 652e 5f76  her_same_base._v
+0000ecd0: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
+0000ece0: 6e74 5f67 7261 7068 2829 3a0a 2020 2020  nt_graph():.    
+0000ecf0: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
+0000ed00: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
+0000ed10: 5f65 7874 203d 2073 656c 662e 6765 745f  _ext = self.get_
+0000ed20: 6479 6e5f 7369 7a65 5f65 7874 5f66 6f72  dyn_size_ext_for
+0000ed30: 5f62 6174 6368 5f63 7478 280a 2020 2020  _batch_ctx(.    
+0000ed40: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+0000ed50: 725f 7361 6d65 5f62 6173 652e 6261 7463  r_same_base.batc
+0000ed60: 682c 206f 7468 6572 5f73 616d 655f 6261  h, other_same_ba
+0000ed70: 7365 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  se.control_flow_
+0000ed80: 6374 782c 2074 656d 706c 6174 655f 6f6e  ctx, template_on
+0000ed90: 6c79 3d54 7275 650a 2020 2020 2020 2020  ly=True.        
+0000eda0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000edb0: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
+0000edc0: 652e 5f6d 6179 6265 5f75 7064 6174 6528  e._maybe_update(
+0000edd0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000ede0: 662e 6973 5f64 696d 5f6b 6e6f 776e 2829  f.is_dim_known()
+0000edf0: 2061 6e64 206f 7468 6572 2e69 735f 6469   and other.is_di
+0000ee00: 6d5f 6b6e 6f77 6e28 293a 0a20 2020 2020  m_known():.     
+0000ee10: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+0000ee20: 6c66 2e64 696d 656e 7369 6f6e 203d 3d20  lf.dimension == 
+0000ee30: 6f74 6865 722e 6469 6d65 6e73 696f 6e0a  other.dimension.
+0000ee40: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+0000ee50: 662e 6973 5f64 696d 5f6b 6e6f 776e 2829  f.is_dim_known()
+0000ee60: 2061 6e64 206e 6f74 206f 7468 6572 2e69   and not other.i
+0000ee70: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
+0000ee80: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000ee90: 2e63 6170 6163 6974 7920 3d20 7365 6c66  .capacity = self
+0000eea0: 2e63 6170 6163 6974 790a 2020 2020 2020  .capacity.      
+0000eeb0: 2020 2020 2020 6f74 6865 722e 7369 7a65        other.size
+0000eec0: 203d 2073 656c 662e 7369 7a65 0a20 2020   = self.size.   
+0000eed0: 2020 2020 2065 6c69 6620 6e6f 7420 7365       elif not se
+0000eee0: 6c66 2e69 735f 6469 6d5f 6b6e 6f77 6e28  lf.is_dim_known(
+0000eef0: 2920 616e 6420 6f74 6865 722e 6973 5f64  ) and other.is_d
+0000ef00: 696d 5f6b 6e6f 776e 2829 3a0a 2020 2020  im_known():.    
+0000ef10: 2020 2020 2020 2020 7365 6c66 2e63 6170          self.cap
+0000ef20: 6163 6974 7920 3d20 6f74 6865 722e 6361  acity = other.ca
+0000ef30: 7061 6369 7479 0a20 2020 2020 2020 2020  pacity.         
+0000ef40: 2020 2073 656c 662e 7369 7a65 203d 206f     self.size = o
+0000ef50: 7468 6572 2e73 697a 650a 2020 2020 2020  ther.size.      
+0000ef60: 2020 6966 2073 656c 662e 766f 6361 6220    if self.vocab 
+0000ef70: 616e 6420 6e6f 7420 6f74 6865 725f 7361  and not other_sa
+0000ef80: 6d65 5f62 6173 652e 766f 6361 623a 0a20  me_base.vocab:. 
+0000ef90: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000efa0: 5f73 616d 655f 6261 7365 2e76 6f63 6162  _same_base.vocab
+0000efb0: 203d 2073 656c 662e 766f 6361 620a 2020   = self.vocab.  
+0000efc0: 2020 2020 2020 656c 6966 206f 7468 6572        elif other
+0000efd0: 5f73 616d 655f 6261 7365 2e76 6f63 6162  _same_base.vocab
+0000efe0: 2061 6e64 206e 6f74 2073 656c 662e 766f   and not self.vo
+0000eff0: 6361 623a 0a20 2020 2020 2020 2020 2020  cab:.           
+0000f000: 2073 656c 662e 766f 6361 6220 3d20 6f74   self.vocab = ot
+0000f010: 6865 725f 7361 6d65 5f62 6173 652e 766f  her_same_base.vo
+0000f020: 6361 620a 2020 2020 2020 2020 7365 6c66  cab.        self
+0000f030: 2e5f 6d61 6b65 5f65 7874 7261 2829 0a20  ._make_extra(). 
+0000f040: 2020 2020 2020 2073 656c 665f 7361 6d65         self_same
+0000f050: 5f61 732e 5f6d 616b 655f 6578 7472 6128  _as._make_extra(
+0000f060: 290a 2020 2020 2020 2020 2320 6e6f 696e  ).        # noin
+0000f070: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+0000f080: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+0000f090: 2020 2073 656c 662e 5f65 7874 7261 2e61     self._extra.a
+0000f0a0: 7574 6f5f 6765 6e65 7261 7465 6420 3d20  uto_generated = 
+0000f0b0: 7365 6c66 5f73 616d 655f 6173 2e5f 6578  self_same_as._ex
+0000f0c0: 7472 612e 6175 746f 5f67 656e 6572 6174  tra.auto_generat
+0000f0d0: 6564 203d 206f 7468 6572 5f73 616d 655f  ed = other_same_
+0000f0e0: 6261 7365 2e61 7574 6f5f 6765 6e65 7261  base.auto_genera
+0000f0f0: 7465 640a 2020 2020 2020 2020 2320 5461  ted.        # Ta
+0000f100: 6b65 206f 7665 7220 6465 7269 7665 645f  ke over derived_
+0000f110: 6672 6f6d 5f6f 702e 2048 6f77 6576 6572  from_op. However
+0000f120: 2c20 6f6e 6c79 2069 6620 7468 6973 2077  , only if this w
+0000f130: 6f75 6c64 206e 6f74 2069 6e74 726f 6475  ould not introdu
+0000f140: 6365 2063 7963 6c65 7321 0a20 2020 2020  ce cycles!.     
+0000f150: 2020 2069 6620 6e6f 7420 7365 6c66 5f64     if not self_d
+0000f160: 6572 6976 6564 5f62 6173 6573 2e69 7373  erived_bases.iss
+0000f170: 7570 6572 7365 7428 6f74 6865 725f 6465  uperset(other_de
+0000f180: 7269 7665 645f 6261 7365 7329 3a0a 2020  rived_bases):.  
+0000f190: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000f1a0: 662e 6465 7269 7665 645f 6672 6f6d 5f6f  f.derived_from_o
+0000f1b0: 7020 616e 6420 6e6f 7420 6f74 6865 725f  p and not other_
+0000f1c0: 7361 6d65 5f62 6173 652e 6465 7269 7665  same_base.derive
+0000f1d0: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
+0000f1e0: 2020 2020 2020 2020 2020 2023 206e 6f69             # noi
+0000f1f0: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
+0000f200: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
+0000f210: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+0000f220: 725f 7361 6d65 5f62 6173 652e 5f6d 616b  r_same_base._mak
+0000f230: 655f 6578 7472 6128 292e 6465 7269 7665  e_extra().derive
+0000f240: 645f 6672 6f6d 5f6f 7020 3d20 7365 6c66  d_from_op = self
+0000f250: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+0000f260: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000f270: 6620 6f74 6865 725f 7361 6d65 5f62 6173  f other_same_bas
+0000f280: 652e 6465 7269 7665 645f 6672 6f6d 5f6f  e.derived_from_o
+0000f290: 7020 616e 6420 6e6f 7420 7365 6c66 2e64  p and not self.d
+0000f2a0: 6572 6976 6564 5f66 726f 6d5f 6f70 3a0a  erived_from_op:.
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2c0: 7365 6c66 2e5f 6d61 6b65 5f65 7874 7261  self._make_extra
+0000f2d0: 2829 2e64 6572 6976 6564 5f66 726f 6d5f  ().derived_from_
+0000f2e0: 6f70 203d 206f 7468 6572 5f73 616d 655f  op = other_same_
+0000f2f0: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000f300: 6d5f 6f70 0a20 2020 2020 2020 2069 6620  m_op.        if 
+0000f310: 7365 6c66 2e5f 6578 7472 6120 616e 6420  self._extra and 
+0000f320: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
+0000f330: 6173 652e 6973 5f64 796e 616d 6963 2829  ase.is_dynamic()
+0000f340: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000f350: 5468 6f73 6520 6d69 6768 7420 6265 2073  Those might be s
+0000f360: 6574 2076 6961 2067 6574 5f62 6174 6368  et via get_batch
+0000f370: 5f66 6f72 5f63 7478 2066 6f72 2061 6e20  _for_ctx for an 
+0000f380: 756e 6465 6669 6e65 6420 6469 6d2c 0a20  undefined dim,. 
+0000f390: 2020 2020 2020 2020 2020 2023 2077 6869             # whi
+0000f3a0: 6368 206e 6f77 2062 6563 6f6d 6573 2073  ch now becomes s
+0000f3b0: 7461 7469 6320 6475 6520 746f 2060 6f74  tatic due to `ot
+0000f3c0: 6865 7260 2e0a 2020 2020 2020 2020 2020  her`..          
+0000f3d0: 2020 7365 6c66 2e5f 6578 7472 612e 6261    self._extra.ba
+0000f3e0: 7463 6820 3d20 4e6f 6e65 0a20 2020 2020  tch = None.     
+0000f3f0: 2020 2020 2020 2073 656c 662e 5f65 7874         self._ext
+0000f400: 7261 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  ra.control_flow_
+0000f410: 6374 7820 3d20 4e6f 6e65 0a20 2020 2020  ctx = None.     
+0000f420: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+0000f430: 6469 6d5f 2069 6e20 7365 6c66 2e5f 6578  dim_ in self._ex
+0000f440: 7472 612e 7361 6d65 5f66 6f72 5f62 6174  tra.same_for_bat
+0000f450: 6368 5f63 7478 2e69 7465 6d73 2829 3a0a  ch_ctx.items():.
+0000f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f470: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+0000f480: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+0000f490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f4a0: 2064 696d 5f65 7874 7261 203d 2064 696d   dim_extra = dim
+0000f4b0: 5f2e 5f65 7874 7261 0a20 2020 2020 2020  _._extra.       
+0000f4c0: 2020 2020 2020 2020 2069 6620 6469 6d5f           if dim_
+0000f4d0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
+0000f4e0: 2020 2020 2020 2020 2020 2064 696d 5f65             dim_e
+0000f4f0: 7874 7261 2e62 6174 6368 203d 204e 6f6e  xtra.batch = Non
+0000f500: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000f510: 2020 2020 2020 6469 6d5f 6578 7472 612e        dim_extra.
+0000f520: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+0000f530: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000f540: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
+0000f550: 2020 2020 2020 2020 2020 2073 656c 665f             self_
+0000f560: 203d 2073 656c 662e 6765 745f 666f 725f   = self.get_for_
+0000f570: 6261 7463 685f 6374 7828 6261 7463 683d  batch_ctx(batch=
+0000f580: 7365 6c66 2e62 6174 6368 2c20 6374 783d  self.batch, ctx=
+0000f590: 7365 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f  self.control_flo
+0000f5a0: 775f 6374 7829 0a20 2020 2020 2020 2020  w_ctx).         
+0000f5b0: 2020 2069 6620 7365 6c66 5f20 6973 206e     if self_ is n
+0000f5c0: 6f74 2073 656c 663a 0a20 2020 2020 2020  ot self:.       
+0000f5d0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000f5e0: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
+0000f5f0: 2073 656c 665f 2e63 6f6e 7472 6f6c 5f66   self_.control_f
+0000f600: 6c6f 775f 6374 7820 2023 206d 6967 6874  low_ctx  # might
+0000f610: 2062 6520 6469 6666 6572 656e 740a 2020   be different.  
+0000f620: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f630: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
+0000f640: 3d20 7365 6c66 5f2e 6479 6e5f 7369 7a65  = self_.dyn_size
+0000f650: 5f65 7874 2020 2320 6d69 6768 7420 6265  _ext  # might be
+0000f660: 2075 6e73 6574 0a0a 2020 2020 6465 6620   unset..    def 
+0000f670: 5f6d 6572 6765 5f73 616d 655f 666f 725f  _merge_same_for_
+0000f680: 6261 7463 685f 6374 785f 6469 6374 2873  batch_ctx_dict(s
+0000f690: 656c 663a 205f 642e 4469 6d2c 206f 7468  elf: _d.Dim, oth
+0000f6a0: 6572 3a20 5f64 2e44 696d 293a 0a20 2020  er: _d.Dim):.   
+0000f6b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f6c0: 203a 7061 7261 6d20 6f74 6865 723a 0a20   :param other:. 
+0000f6d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f6e0: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
+0000f6f0: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
+0000f700: 6265 720a 2020 2020 2020 2020 6966 206e  ber.        if n
+0000f710: 6f74 2073 656c 662e 5f65 7874 7261 2061  ot self._extra a
+0000f720: 6e64 206e 6f74 206f 7468 6572 2e5f 6578  nd not other._ex
+0000f730: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+0000f740: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000f750: 7365 6c66 2e5f 7661 6c69 6461 7465 5f69  self._validate_i
+0000f760: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000f770: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000f780: 662e 5f65 7874 7261 3a0a 2020 2020 2020  f._extra:.      
+0000f790: 2020 2020 2020 666f 7220 5f2c 2064 696d        for _, dim
+0000f7a0: 2069 6e20 6c69 7374 2873 656c 662e 5f65   in list(self._e
+0000f7b0: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
+0000f7c0: 7463 685f 6374 782e 6974 656d 7328 2929  tch_ctx.items())
+0000f7d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f7e0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+0000f7f0: 6e63 6528 6469 6d2c 205f 642e 4469 6d29  nce(dim, _d.Dim)
+0000f800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f810: 2064 696d 2e5f 7661 6c69 6461 7465 5f69   dim._validate_i
+0000f820: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000f830: 290a 2020 2020 2020 2020 2320 6e6f 696e  ).        # noin
+0000f840: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+0000f850: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+0000f860: 2020 2069 6620 6f74 6865 722e 5f65 7874     if other._ext
+0000f870: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
+0000f880: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+0000f890: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+0000f8a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000f8b0: 206b 6579 2c20 6469 6d20 696e 206f 7468   key, dim in oth
+0000f8c0: 6572 2e5f 6578 7472 612e 7361 6d65 5f66  er._extra.same_f
+0000f8d0: 6f72 5f62 6174 6368 5f63 7478 2e69 7465  or_batch_ctx.ite
+0000f8e0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0000f8f0: 2020 2020 2020 6966 206e 6f74 2064 696d        if not dim
+0000f900: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+0000f910: 7272 656e 745f 6772 6170 6828 293a 0a20  rrent_graph():. 
+0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f930: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+0000f940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f950: 5f64 696d 203d 2073 656c 662e 5f6d 616b  _dim = self._mak
+0000f960: 655f 6578 7472 6128 292e 7361 6d65 5f66  e_extra().same_f
+0000f970: 6f72 5f62 6174 6368 5f63 7478 2e67 6574  or_batch_ctx.get
+0000f980: 286b 6579 2c20 4e6f 6e65 290a 2020 2020  (key, None).    
+0000f990: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000f9a0: 656c 665f 6469 6d20 616e 6420 2873 656c  elf_dim and (sel
+0000f9b0: 665f 6469 6d2e 6479 6e5f 7369 7a65 5f65  f_dim.dyn_size_e
+0000f9c0: 7874 206f 7220 6e6f 7420 6469 6d2e 6479  xt or not dim.dy
+0000f9d0: 6e5f 7369 7a65 5f65 7874 293a 0a20 2020  n_size_ext):.   
+0000f9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9f0: 2063 6f6e 7469 6e75 6520 2023 206b 6565   continue  # kee
+0000fa00: 7020 6f75 7273 0a20 2020 2020 2020 2020  p ours.         
+0000fa10: 2020 2020 2020 2069 6620 6e6f 7420 6469         if not di
+0000fa20: 6d2e 6479 6e5f 7369 7a65 5f65 7874 3a0a  m.dyn_size_ext:.
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa40: 2020 2020 636f 6e74 696e 7565 2020 2320      continue  # 
+0000fa50: 756e 6465 6669 6e65 642c 2064 6f20 6e6f  undefined, do no
+0000fa60: 7420 6f76 6572 7461 6b65 0a20 2020 2020  t overtake.     
+0000fa70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fa80: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000fa90: 6261 7463 685f 6374 785b 6b65 795d 203d  batch_ctx[key] =
+0000faa0: 2064 696d 0a20 2020 2020 2020 2020 2020   dim.           
+0000fab0: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
+0000fac0: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
+0000fad0: 720a 2020 2020 2020 2020 2020 2020 6f74  r.            ot
+0000fae0: 6865 722e 5f65 7874 7261 2e73 616d 655f  her._extra.same_
+0000faf0: 666f 725f 6261 7463 685f 6374 782e 636c  for_batch_ctx.cl
+0000fb00: 6561 7228 2920 2023 2077 6520 6f6e 6c79  ear()  # we only
+0000fb10: 2077 616e 7420 746f 2068 6176 6520 6974   want to have it
+0000fb20: 206f 6e63 650a 0a20 2020 2023 206e 6f69   once..    # noi
+0000fb30: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
+0000fb40: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
+0000fb50: 6465 6620 6465 7269 7665 5f66 726f 6d28  def derive_from(
+0000fb60: 7365 6c66 3a20 5f64 2e44 696d 2c20 6261  self: _d.Dim, ba
+0000fb70: 7365 3a20 5f64 2e44 696d 2c20 7365 745f  se: _d.Dim, set_
+0000fb80: 6465 7269 7665 645f 6672 6f6d 5f66 6c61  derived_from_fla
+0000fb90: 673a 2062 6f6f 6c20 3d20 5472 7565 293a  g: bool = True):
+0000fba0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000fbb0: 2020 2020 203a 7061 7261 6d20 6261 7365       :param base
+0000fbc0: 3a20 6469 6d0a 2020 2020 2020 2020 3a70  : dim.        :p
+0000fbd0: 6172 616d 2073 6574 5f64 6572 6976 6564  aram set_derived
+0000fbe0: 5f66 726f 6d5f 666c 6167 3a0a 2020 2020  _from_flag:.    
+0000fbf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000fc00: 7365 6c66 5f62 6173 6520 3d20 7365 6c66  self_base = self
+0000fc10: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
+0000fc20: 0a20 2020 2020 2020 2073 656c 665f 6261  .        self_ba
+0000fc30: 7365 5f65 7874 7261 203d 2073 656c 665f  se_extra = self_
+0000fc40: 6261 7365 2e5f 6d61 6b65 5f65 7874 7261  base._make_extra
+0000fc50: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0000fc60: 745f 6465 7269 7665 645f 6672 6f6d 5f66  t_derived_from_f
+0000fc70: 6c61 673a 0a20 2020 2020 2020 2020 2020  lag:.           
+0000fc80: 2069 6620 7365 6c66 5f62 6173 655f 6578   if self_base_ex
+0000fc90: 7472 612e 6465 7269 7665 645f 6672 6f6d  tra.derived_from
+0000fca0: 5f74 6167 3a0a 2020 2020 2020 2020 2020  _tag:.          
+0000fcb0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+0000fcc0: 665f 6261 7365 5f65 7874 7261 2e64 6572  f_base_extra.der
+0000fcd0: 6976 6564 5f66 726f 6d5f 7461 6720 3d3d  ived_from_tag ==
+0000fce0: 2062 6173 650a 2020 2020 2020 2020 2020   base.          
+0000fcf0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000fd00: 2020 2020 2020 2020 7365 6c66 5f62 6173          self_bas
+0000fd10: 655f 6578 7472 612e 6465 7269 7665 645f  e_extra.derived_
+0000fd20: 6672 6f6d 5f74 6167 203d 2062 6173 650a  from_tag = base.
+0000fd30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000fd40: 6973 5f64 796e 616d 6963 2829 206f 7220  is_dynamic() or 
+0000fd50: 6e6f 7420 7365 6c66 2e69 735f 6469 6d5f  not self.is_dim_
+0000fd60: 6b6e 6f77 6e28 293a 0a20 2020 2020 2020  known():.       
+0000fd70: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0000fd80: 2e62 6174 6368 2061 6e64 2062 6173 652e  .batch and base.
+0000fd90: 6261 7463 683a 0a20 2020 2020 2020 2020  batch:.         
+0000fda0: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
+0000fdb0: 6820 3d20 6261 7365 2e62 6174 6368 0a20  h = base.batch. 
+0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fdd0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
+0000fde0: 5f63 7478 203d 2062 6173 652e 636f 6e74  _ctx = base.cont
+0000fdf0: 726f 6c5f 666c 6f77 5f63 7478 0a20 2020  rol_flow_ctx.   
+0000fe00: 2020 2020 2020 2020 2020 2020 206b 6579               key
+0000fe10: 203d 2062 6173 652e 6261 7463 682c 2062   = base.batch, b
+0000fe20: 6173 652e 636f 6e74 726f 6c5f 666c 6f77  ase.control_flow
+0000fe30: 5f63 7478 0a20 2020 2020 2020 2020 2020  _ctx.           
+0000fe40: 2020 2020 2061 7373 6572 7420 6b65 7920       assert key 
+0000fe50: 6e6f 7420 696e 2073 656c 665f 6261 7365  not in self_base
+0000fe60: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000fe70: 6261 7463 685f 6374 780a 2020 2020 2020  batch_ctx.      
+0000fe80: 2020 2020 2020 2020 2020 7365 6c66 5f62            self_b
+0000fe90: 6173 655f 6578 7472 612e 7361 6d65 5f66  ase_extra.same_f
+0000fea0: 6f72 5f62 6174 6368 5f63 7478 5b6b 6579  or_batch_ctx[key
+0000feb0: 5d20 3d20 7365 6c66 0a20 2020 2020 2020  ] = self.       
+0000fec0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0000fed0: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
+0000fee0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000fef0: 6620 6261 7365 2e64 796e 5f73 697a 655f  f base.dyn_size_
+0000ff00: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
+0000ff10: 2020 2020 2020 2020 2069 6620 6261 7365           if base
+0000ff20: 2e62 6174 6368 2061 6e64 2062 6173 652e  .batch and base.
+0000ff30: 6261 7463 6820 3d3d 2073 656c 662e 6261  batch == self.ba
+0000ff40: 7463 6820 616e 6420 6261 7365 2e63 6f6e  tch and base.con
+0000ff50: 7472 6f6c 5f66 6c6f 775f 6374 7820 3d3d  trol_flow_ctx ==
+0000ff60: 2073 656c 662e 636f 6e74 726f 6c5f 666c   self.control_fl
+0000ff70: 6f77 5f63 7478 3a0a 2020 2020 2020 2020  ow_ctx:.        
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+0000ffa0: 7420 3d20 6261 7365 2e64 796e 5f73 697a  t = base.dyn_siz
+0000ffb0: 655f 6578 742e 636f 7079 5f74 656d 706c  e_ext.copy_templ
+0000ffc0: 6174 6528 6e61 6d65 3d22 2573 3a73 697a  ate(name="%s:siz
+0000ffd0: 6522 2025 2073 656c 665f 6261 7365 2e64  e" % self_base.d
+0000ffe0: 6573 6372 6970 7469 6f6e 290a 2020 2020  escription).    
+0000fff0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00010000: 2062 6173 652e 6973 5f62 6174 6368 5f64   base.is_batch_d
+00010010: 696d 2829 3a0a 2020 2020 2020 2020 2020  im():.          
+00010020: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00010030: 796e 5f73 697a 655f 6578 7420 3d20 5f74  yn_size_ext = _t
+00010040: 2e54 656e 736f 7228 0a20 2020 2020 2020  .Tensor(.       
+00010050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010060: 206e 616d 653d 2225 733a 6261 7463 6822   name="%s:batch"
+00010070: 2025 2073 656c 665f 6261 7365 2e64 6573   % self_base.des
+00010080: 6372 6970 7469 6f6e 2c20 7368 6170 653d  cription, shape=
+00010090: 2829 2c20 6474 7970 653d 2269 6e74 3332  (), dtype="int32
+000100a0: 222c 2062 6174 6368 5f64 696d 5f61 7869  ", batch_dim_axi
+000100b0: 733d 4e6f 6e65 0a20 2020 2020 2020 2020  s=None.         
+000100c0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+000100d0: 2020 6465 6620 636f 7079 5f66 726f 6d28    def copy_from(
+000100e0: 7365 6c66 3a20 4469 6d2c 206f 7468 6572  self: Dim, other
+000100f0: 3a20 4469 6d29 3a0a 2020 2020 2020 2020  : Dim):.        
+00010100: 2222 2264 6566 696e 6522 2222 0a20 2020  """define""".   
+00010110: 2020 2020 2073 656c 662e 7369 7a65 203d       self.size =
+00010120: 206f 7468 6572 2e73 697a 650a 2020 2020   other.size.    
+00010130: 2020 2020 7365 6c66 2e63 6170 6163 6974      self.capacit
+00010140: 7920 3d20 6f74 6865 722e 6361 7061 6369  y = other.capaci
+00010150: 7479 0a20 2020 2020 2020 2073 656c 662e  ty.        self.
+00010160: 6479 6e5f 7369 7a65 5f65 7874 203d 206f  dyn_size_ext = o
+00010170: 7468 6572 2e64 796e 5f73 697a 655f 6578  ther.dyn_size_ex
+00010180: 740a 2020 2020 2020 2020 7365 6c66 2e64  t.        self.d
+00010190: 6572 6976 655f 6672 6f6d 286f 7468 6572  erive_from(other
+000101a0: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
+000101b0: 686f 640a 2020 2020 6465 6620 6765 745f  hod.    def get_
+000101c0: 6578 6973 7469 6e67 5f74 6167 5f66 726f  existing_tag_fro
+000101d0: 6d5f 636f 6c6c 6563 7469 6f6e 2863 6c73  m_collection(cls
+000101e0: 2c20 6f74 6865 722c 2074 6167 732c 2069  , other, tags, i
+000101f0: 735f 6571 7561 6c5f 6f70 7473 3d4e 6f6e  s_equal_opts=Non
+00010200: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+00010210: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
+00010220: 696d 206f 7468 6572 3a0a 2020 2020 2020  im other:.      
+00010230: 2020 3a70 6172 616d 206c 6973 745b 4469    :param list[Di
+00010240: 6d5d 7c74 7570 6c65 5b44 696d 5d7c 7365  m]|tuple[Dim]|se
+00010250: 745b 4469 6d5d 2074 6167 733a 0a20 2020  t[Dim] tags:.   
+00010260: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
+00010270: 5b73 7472 5d7c 4e6f 6e65 2069 735f 6571  [str]|None is_eq
+00010280: 7561 6c5f 6f70 7473 3a20 7061 7373 6564  ual_opts: passed
+00010290: 2074 6f20 4469 6d2e 6973 5f65 7175 616c   to Dim.is_equal
+000102a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000102b0: 2044 696d 7c4e 6f6e 650a 2020 2020 2020   Dim|None.      
+000102c0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+000102d0: 2069 735f 6571 7561 6c5f 6f70 7473 2069   is_equal_opts i
+000102e0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000102f0: 2020 2020 6973 5f65 7175 616c 5f6f 7074      is_equal_opt
+00010300: 7320 3d20 7b7d 0a20 2020 2020 2020 2023  s = {}.        #
+00010310: 2057 6520 646f 2070 6f74 656e 7469 616c   We do potential
+00010320: 206d 756c 7469 706c 6520 726f 756e 6473   multiple rounds
+00010330: 2c20 7375 6368 2074 6861 7420 7765 2070  , such that we p
+00010340: 7265 6665 7220 226d 6f72 6520 6571 7561  refer "more equa
+00010350: 6c22 2028 7573 696e 6720 6c65 7373 2069  l" (using less i
+00010360: 735f 6571 7561 6c5f 6f70 7473 292e 0a20  s_equal_opts).. 
+00010370: 2020 2020 2020 2072 6f75 6e64 7320 3d20         rounds = 
+00010380: 5b7b 7d5d 0a20 2020 2020 2020 2069 6620  [{}].        if 
+00010390: 6973 5f65 7175 616c 5f6f 7074 733a 0a20  is_equal_opts:. 
+000103a0: 2020 2020 2020 2020 2020 2069 6620 2262             if "b
+000103b0: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
+000103c0: 2220 696e 2069 735f 6571 7561 6c5f 6f70  " in is_equal_op
+000103d0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+000103e0: 2020 2020 726f 756e 6473 2e61 7070 656e      rounds.appen
+000103f0: 6428 7b6b 3a20 7620 666f 7220 286b 2c20  d({k: v for (k, 
+00010400: 7629 2069 6e20 6973 5f65 7175 616c 5f6f  v) in is_equal_o
+00010410: 7074 732e 6974 656d 7328 2920 6966 206b  pts.items() if k
+00010420: 2021 3d20 2262 726f 6164 6361 7374 5f6d   != "broadcast_m
+00010430: 6174 6368 6573 227d 290a 2020 2020 2020  atches"}).      
+00010440: 2020 2020 2020 726f 756e 6473 2e61 7070        rounds.app
+00010450: 656e 6428 6973 5f65 7175 616c 5f6f 7074  end(is_equal_opt
+00010460: 7329 0a20 2020 2020 2020 2066 6f72 205f  s).        for _
+00010470: 6973 5f65 7175 616c 5f6f 7074 7320 696e  is_equal_opts in
+00010480: 2072 6f75 6e64 733a 0a20 2020 2020 2020   rounds:.       
+00010490: 2020 2020 2066 6f72 205f 7461 6720 696e       for _tag in
+000104a0: 2074 6167 733a 0a20 2020 2020 2020 2020   tags:.         
+000104b0: 2020 2020 2020 2069 6620 5f74 6167 2e69         if _tag.i
+000104c0: 735f 6571 7561 6c28 6f74 6865 722c 202a  s_equal(other, *
+000104d0: 2a5f 6973 5f65 7175 616c 5f6f 7074 7329  *_is_equal_opts)
+000104e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000104f0: 2020 2020 2020 7265 7475 726e 205f 7461        return _ta
+00010500: 670a 2020 2020 2020 2020 7265 7475 726e  g.        return
+00010510: 204e 6f6e 650a 0a20 2020 2040 636c 6173   None..    @clas
+00010520: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00010530: 6765 745f 616c 6c5f 6469 6d65 6e73 696f  get_all_dimensio
+00010540: 6e5f 7461 6773 2863 6c73 2c20 6461 7461  n_tags(cls, data
+00010550: 5f6c 6973 742c 2069 735f 6571 7561 6c5f  _list, is_equal_
+00010560: 6f70 7473 3d4e 6f6e 652c 2075 6e69 7175  opts=None, uniqu
+00010570: 655f 7365 7061 7261 7465 5f61 7865 733d  e_separate_axes=
+00010580: 5472 7565 293a 0a20 2020 2020 2020 2022  True):.        "
+00010590: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+000105a0: 6d20 6c69 7374 5b5f 742e 5465 6e73 6f72  m list[_t.Tensor
+000105b0: 5d20 6461 7461 5f6c 6973 743a 0a20 2020  ] data_list:.   
+000105c0: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
+000105d0: 5b73 7472 5d7c 4e6f 6e65 2069 735f 6571  [str]|None is_eq
+000105e0: 7561 6c5f 6f70 7473 3a20 7061 7373 6564  ual_opts: passed
+000105f0: 2074 6f20 4469 6d2e 6973 5f65 7175 616c   to Dim.is_equal
+00010600: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010610: 626f 6f6c 2075 6e69 7175 655f 7365 7061  bool unique_sepa
+00010620: 7261 7465 5f61 7865 733a 2065 2e67 2e20  rate_axes: e.g. 
+00010630: 6461 7461 5f6c 6973 743d 5b44 6174 6120  data_list=[Data 
+00010640: 7769 7468 2073 6861 7065 2028 422c 352c  with shape (B,5,
+00010650: 352c 3130 295d 2072 6573 756c 7473 2069  5,10)] results i
+00010660: 6e20 3420 6469 6d20 7461 6773 2c20 6e6f  n 4 dim tags, no
+00010670: 7420 332e 0a20 2020 2020 2020 203a 7265  t 3..        :re
+00010680: 7475 726e 3a20 6c69 7374 206f 6620 6469  turn: list of di
+00010690: 6d65 6e73 696f 6e20 7461 6773 2c20 6469  mension tags, di
+000106a0: 6374 2066 6f72 2064 6174 6120 2d3e 206c  ct for data -> l
+000106b0: 6973 7420 6f66 2064 696d 656e 7369 6f6e  ist of dimension
+000106c0: 2074 6167 7320 2866 6f72 2065 6163 6820   tags (for each 
+000106d0: 6178 6973 290a 2020 2020 2020 2020 3a72  axis).        :r
+000106e0: 7479 7065 3a20 286c 6973 745b 4469 6d5d  type: (list[Dim]
+000106f0: 2c20 7574 696c 2e44 6963 7452 6566 4b65  , util.DictRefKe
+00010700: 7973 5b5f 742e 5465 6e73 6f72 2c20 6c69  ys[_t.Tensor, li
+00010710: 7374 5b44 696d 5d5d 290a 2020 2020 2020  st[Dim]]).      
+00010720: 2020 2222 220a 2020 2020 2020 2020 7461    """.        ta
+00010730: 6773 203d 205b 5d0a 2020 2020 2020 2020  gs = [].        
+00010740: 6461 7461 5f61 7865 735f 6469 6374 203d  data_axes_dict =
+00010750: 2075 7469 6c2e 4469 6374 5265 664b 6579   util.DictRefKey
+00010760: 7328 2920 2023 2074 7970 653a 2075 7469  s()  # type: uti
+00010770: 6c2e 4469 6374 5265 664b 6579 735b 5f74  l.DictRefKeys[_t
+00010780: 2e54 656e 736f 722c 204c 6973 745b 4469  .Tensor, List[Di
+00010790: 6d5d 5d0a 2020 2020 2020 2020 666f 7220  m]].        for 
+000107a0: 6461 7461 2069 6e20 6461 7461 5f6c 6973  data in data_lis
+000107b0: 743a 0a20 2020 2020 2020 2020 2020 2064  t:.            d
+000107c0: 6174 615f 6178 6573 5f64 6963 745b 6461  ata_axes_dict[da
+000107d0: 7461 5d20 3d20 5b5d 0a20 2020 2020 2020  ta] = [].       
+000107e0: 2020 2020 2065 7869 7374 696e 675f 7461       existing_ta
+000107f0: 675f 636f 6c6c 6563 7469 6f6e 5f66 6f72  g_collection_for
+00010800: 5f64 6174 6120 3d20 6c69 7374 2874 6167  _data = list(tag
+00010810: 7329 2069 6620 756e 6971 7565 5f73 6570  s) if unique_sep
+00010820: 6172 6174 655f 6178 6573 2065 6c73 6520  arate_axes else 
+00010830: 7461 6773 0a20 2020 2020 2020 2020 2020  tags.           
+00010840: 2066 6f72 2061 7869 7320 696e 2072 616e   for axis in ran
+00010850: 6765 2864 6174 612e 6261 7463 685f 6e64  ge(data.batch_nd
+00010860: 696d 293a 0a20 2020 2020 2020 2020 2020  im):.           
+00010870: 2020 2020 2074 6167 203d 2064 6174 612e       tag = data.
+00010880: 6765 745f 6469 6d5f 7461 6728 6178 6973  get_dim_tag(axis
+00010890: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000108a0: 2020 6578 6973 7469 6e67 5f74 6167 203d    existing_tag =
+000108b0: 2063 6c73 2e67 6574 5f65 7869 7374 696e   cls.get_existin
+000108c0: 675f 7461 675f 6672 6f6d 5f63 6f6c 6c65  g_tag_from_colle
+000108d0: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
+000108e0: 2020 2020 2020 2020 2020 2074 6167 2c20             tag, 
+000108f0: 7461 6773 3d65 7869 7374 696e 675f 7461  tags=existing_ta
+00010900: 675f 636f 6c6c 6563 7469 6f6e 5f66 6f72  g_collection_for
+00010910: 5f64 6174 612c 2069 735f 6571 7561 6c5f  _data, is_equal_
+00010920: 6f70 7473 3d69 735f 6571 7561 6c5f 6f70  opts=is_equal_op
+00010930: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00010940: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00010950: 2020 2020 2069 6620 6578 6973 7469 6e67       if existing
+00010960: 5f74 6167 3a0a 2020 2020 2020 2020 2020  _tag:.          
+00010970: 2020 2020 2020 2020 2020 6966 2075 6e69            if uni
+00010980: 7175 655f 7365 7061 7261 7465 5f61 7865  que_separate_axe
+00010990: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000109a0: 2020 2020 2020 2020 2020 2065 7869 7374             exist
+000109b0: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
+000109c0: 6f6e 5f66 6f72 5f64 6174 612e 7265 6d6f  on_for_data.remo
+000109d0: 7665 2865 7869 7374 696e 675f 7461 6729  ve(existing_tag)
+000109e0: 2020 2320 646f 6e27 7420 7461 6b65 2069    # don't take i
+000109f0: 7420 6167 6169 6e20 666f 7220 7468 6973  t again for this
+00010a00: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+00010a10: 2020 2020 2020 2020 2020 7265 706c 6163            replac
+00010a20: 655f 6578 6973 7469 6e67 203d 2028 0a20  e_existing = (. 
+00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a40: 2020 2020 2020 2065 7869 7374 696e 675f         existing_
+00010a50: 7461 672e 756e 6465 6669 6e65 6420 616e  tag.undefined an
+00010a60: 6420 6e6f 7420 7461 672e 756e 6465 6669  d not tag.undefi
+00010a70: 6e65 6420 616e 6420 7461 672e 6469 6d65  ned and tag.dime
+00010a80: 6e73 696f 6e20 3d3d 2065 7869 7374 696e  nsion == existin
+00010a90: 675f 7461 672e 6469 6d65 6e73 696f 6e0a  g_tag.dimension.
+00010aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ab0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00010ac0: 2020 2020 2020 2020 2020 6966 2072 6570            if rep
+00010ad0: 6c61 6365 5f65 7869 7374 696e 673a 2020  lace_existing:  
+00010ae0: 2320 5265 706c 6163 6520 7468 6520 6578  # Replace the ex
+00010af0: 6973 7469 6e67 2062 7920 7468 6520 6e65  isting by the ne
+00010b00: 7720 7461 672e 0a20 2020 2020 2020 2020  w tag..         
+00010b10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00010b20: 6167 735b 7461 6773 2e69 6e64 6578 2865  ags[tags.index(e
+00010b30: 7869 7374 696e 675f 7461 6729 5d20 3d20  xisting_tag)] = 
+00010b40: 7461 670a 2020 2020 2020 2020 2020 2020  tag.            
+00010b50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010b60: 5f2c 2064 696d 735f 2069 6e20 6461 7461  _, dims_ in data
+00010b70: 5f61 7865 735f 6469 6374 2e69 7465 6d73  _axes_dict.items
+00010b80: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ba0: 6469 6d73 5f5b 3a5d 203d 205b 7461 6720  dims_[:] = [tag 
+00010bb0: 6966 2064 203d 3d20 6578 6973 7469 6e67  if d == existing
+00010bc0: 5f74 6167 2065 6c73 6520 6420 666f 7220  _tag else d for 
+00010bd0: 6420 696e 2064 696d 735f 5d0a 2020 2020  d in dims_].    
+00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bf0: 2020 2020 6578 6973 7469 6e67 5f74 6167      existing_tag
+00010c00: 203d 2074 6167 0a20 2020 2020 2020 2020   = tag.         
+00010c10: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
+00010c20: 6e6f 2065 7869 7374 696e 6720 7461 670a  no existing tag.
+00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c40: 2020 2020 7461 6773 2e61 7070 656e 6428      tags.append(
+00010c50: 7461 6729 0a20 2020 2020 2020 2020 2020  tag).           
+00010c60: 2020 2020 2064 6174 615f 6178 6573 5f64       data_axes_d
+00010c70: 6963 745b 6461 7461 5d2e 6170 7065 6e64  ict[data].append
+00010c80: 2865 7869 7374 696e 675f 7461 6720 6f72  (existing_tag or
+00010c90: 2074 6167 290a 2020 2020 2020 2020 7265   tag).        re
+00010ca0: 7475 726e 2074 6167 732c 2064 6174 615f  turn tags, data_
+00010cb0: 6178 6573 5f64 6963 740a 0a20 2020 2040  axes_dict..    @
+00010cc0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+00010cd0: 6465 6620 6765 745f 756e 6971 5f63 6f6c  def get_uniq_col
+00010ce0: 6c65 6374 696f 6e28 636c 732c 2074 6167  lection(cls, tag
+00010cf0: 732c 2069 735f 6571 7561 6c5f 6f70 7473  s, is_equal_opts
+00010d00: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00010d10: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+00010d20: 616d 206c 6973 745b 4469 6d5d 7c74 7570  am list[Dim]|tup
+00010d30: 6c65 5b44 696d 5d7c 7365 745b 4469 6d5d  le[Dim]|set[Dim]
+00010d40: 2074 6167 733a 0a20 2020 2020 2020 203a   tags:.        :
+00010d50: 7061 7261 6d20 6469 6374 5b73 7472 5d7c  param dict[str]|
+00010d60: 4e6f 6e65 2069 735f 6571 7561 6c5f 6f70  None is_equal_op
+00010d70: 7473 3a20 7061 7373 6564 2074 6f20 4469  ts: passed to Di
+00010d80: 6d2e 6973 5f65 7175 616c 0a20 2020 2020  m.is_equal.     
+00010d90: 2020 203a 7274 7970 653a 206c 6973 745b     :rtype: list[
+00010da0: 4469 6d5d 0a20 2020 2020 2020 2022 2222  Dim].        """
+00010db0: 0a20 2020 2020 2020 2072 6573 203d 205b  .        res = [
+00010dc0: 5d0a 2020 2020 2020 2020 666f 7220 7461  ].        for ta
+00010dd0: 6720 696e 2074 6167 733a 0a20 2020 2020  g in tags:.     
+00010de0: 2020 2020 2020 2065 7820 3d20 636c 732e         ex = cls.
+00010df0: 6765 745f 6578 6973 7469 6e67 5f74 6167  get_existing_tag
+00010e00: 5f66 726f 6d5f 636f 6c6c 6563 7469 6f6e  _from_collection
+00010e10: 2874 6167 2c20 7265 732c 2069 735f 6571  (tag, res, is_eq
+00010e20: 7561 6c5f 6f70 7473 3d69 735f 6571 7561  ual_opts=is_equa
+00010e30: 6c5f 6f70 7473 290a 2020 2020 2020 2020  l_opts).        
+00010e40: 2020 2020 6966 206e 6f74 2065 783a 0a20      if not ex:. 
+00010e50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010e60: 6573 2e61 7070 656e 6428 7461 6729 0a20  es.append(tag). 
+00010e70: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00010e80: 730a 0a20 2020 2064 6566 2067 6574 5f73  s..    def get_s
+00010e90: 697a 655f 7465 6e73 6f72 2873 656c 6629  ize_tensor(self)
+00010ea0: 202d 3e20 5f74 2e54 656e 736f 723a 0a20   -> _t.Tensor:. 
+00010eb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010ec0: 2020 203a 7265 7475 726e 3a20 7369 7a65     :return: size
+00010ed0: 2074 656e 736f 722c 206f 7220 6479 6e5f   tensor, or dyn_
+00010ee0: 7369 7a65 5f65 7874 2069 6620 6465 6669  size_ext if defi
+00010ef0: 6e65 640a 2020 2020 2020 2020 3a72 7479  ned.        :rty
+00010f00: 7065 3a20 5f74 2e54 656e 736f 720a 2020  pe: _t.Tensor.  
 00010f10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010f20: 2020 3a70 6172 616d 206c 6973 745b 4469    :param list[Di
-00010f30: 6d5d 7c74 7570 6c65 5b44 696d 5d7c 7365  m]|tuple[Dim]|se
-00010f40: 745b 4469 6d5d 2074 6167 733a 0a20 2020  t[Dim] tags:.   
-00010f50: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
-00010f60: 5b73 7472 5d7c 4e6f 6e65 2069 735f 6571  [str]|None is_eq
-00010f70: 7561 6c5f 6f70 7473 3a20 7061 7373 6564  ual_opts: passed
-00010f80: 2074 6f20 4469 6d2e 6973 5f65 7175 616c   to Dim.is_equal
-00010f90: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00010fa0: 206c 6973 745b 4469 6d5d 0a20 2020 2020   list[Dim].     
-00010fb0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00010fc0: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
-00010fd0: 666f 7220 7461 6720 696e 2074 6167 733a  for tag in tags:
-00010fe0: 0a20 2020 2020 2020 2020 2020 2065 7820  .            ex 
-00010ff0: 3d20 636c 732e 6765 745f 6578 6973 7469  = cls.get_existi
-00011000: 6e67 5f74 6167 5f66 726f 6d5f 636f 6c6c  ng_tag_from_coll
-00011010: 6563 7469 6f6e 2874 6167 2c20 7265 732c  ection(tag, res,
-00011020: 2069 735f 6571 7561 6c5f 6f70 7473 3d69   is_equal_opts=i
-00011030: 735f 6571 7561 6c5f 6f70 7473 290a 2020  s_equal_opts).  
-00011040: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00011050: 2065 783a 0a20 2020 2020 2020 2020 2020   ex:.           
-00011060: 2020 2020 2072 6573 2e61 7070 656e 6428       res.append(
-00011070: 7461 6729 0a20 2020 2020 2020 2072 6574  tag).        ret
-00011080: 7572 6e20 7265 730a 0a20 2020 2064 6566  urn res..    def
-00011090: 2067 6574 5f73 697a 655f 7465 6e73 6f72   get_size_tensor
-000110a0: 2873 656c 6629 202d 3e20 5f74 2e54 656e  (self) -> _t.Ten
-000110b0: 736f 723a 0a20 2020 2020 2020 2022 2222  sor:.        """
-000110c0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000110d0: 3a20 7369 7a65 2074 656e 736f 722c 206f  : size tensor, o
-000110e0: 7220 6479 6e5f 7369 7a65 5f65 7874 2069  r dyn_size_ext i
-000110f0: 6620 6465 6669 6e65 640a 2020 2020 2020  f defined.      
-00011100: 2020 3a72 7479 7065 3a20 5f74 2e54 656e    :rtype: _t.Ten
-00011110: 736f 720a 2020 2020 2020 2020 2222 220a  sor.        """.
-00011120: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011130: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
-00011140: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011150: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00011160: 7874 0a0a 2020 2020 2020 2020 696d 706f  xt..        impo
-00011170: 7274 2072 6574 7572 6e6e 2e66 726f 6e74  rt returnn.front
-00011180: 656e 6420 6173 2072 660a 0a20 2020 2020  end as rf..     
-00011190: 2020 2061 7373 6572 7420 7365 6c66 2e73     assert self.s
-000111a0: 697a 6520 6973 206e 6f74 204e 6f6e 650a  ize is not None.
-000111b0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000111c0: 662e 636f 6e76 6572 745f 746f 5f74 656e  f.convert_to_ten
-000111d0: 736f 7228 7365 6c66 2e73 697a 652c 206e  sor(self.size, n
-000111e0: 616d 653d 2225 733a 7369 7a65 2220 2520  ame="%s:size" % 
-000111f0: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
-00011200: 290a 0a20 2020 2064 6566 2067 6574 5f64  )..    def get_d
-00011210: 696d 5f76 616c 7565 2873 656c 6629 202d  im_value(self) -
-00011220: 3e20 556e 696f 6e5b 696e 742c 205f 742e  > Union[int, _t.
-00011230: 5261 7754 656e 736f 7254 7970 655d 3a0a  RawTensorType]:.
-00011240: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011250: 2020 2020 496e 6665 7273 2074 6865 2064      Infers the d
-00011260: 696d 2074 6869 7320 6178 6973 2073 686f  im this axis sho
-00011270: 756c 6420 6861 7665 2069 6620 756e 6272  uld have if unbr
-00011280: 6f61 6463 6173 7465 642e 0a20 2020 2020  oadcasted..     
-00011290: 2020 2049 6620 6073 656c 662e 7372 635f     If `self.src_
-000112a0: 6461 7461 6020 6861 7320 6120 706c 6163  data` has a plac
-000112b0: 6568 6f6c 6465 722c 2077 696c 6c20 7573  eholder, will us
-000112c0: 6520 7468 6520 7368 6170 6520 6672 6f6d  e the shape from
-000112d0: 2074 6865 7265 2e0a 2020 2020 2020 2020   there..        
-000112e0: 4f74 6865 7277 6973 652c 2075 7365 7320  Otherwise, uses 
-000112f0: 6073 656c 662e 6469 6d65 6e73 696f 6e60  `self.dimension`
-00011300: 2028 6966 2073 7461 7469 6329 206f 7220   (if static) or 
-00011310: 6073 656c 662e 6479 6e5f 7369 7a65 6020  `self.dyn_size` 
-00011320: 2869 6620 6479 6e61 6d69 6329 2e0a 0a20  (if dynamic)... 
-00011330: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00011340: 6d61 7828 7369 7a65 206f 7220 6479 6e5f  max(size or dyn_
-00011350: 7369 7a65 290a 2020 2020 2020 2020 2222  size).        ""
-00011360: 220a 2020 2020 2020 2020 7265 7320 3d20  ".        res = 
-00011370: 7365 6c66 2e67 6574 5f64 696d 5f76 616c  self.get_dim_val
-00011380: 7565 5f74 656e 736f 7228 290a 2020 2020  ue_tensor().    
-00011390: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000113a0: 6528 7265 732c 205f 742e 5465 6e73 6f72  e(res, _t.Tensor
-000113b0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
-000113c0: 7373 6572 7420 7265 732e 6469 6d73 203d  ssert res.dims =
-000113d0: 3d20 2829 0a20 2020 2020 2020 2020 2020  = ().           
-000113e0: 2072 6574 7572 6e20 7265 732e 7261 775f   return res.raw_
-000113f0: 7465 6e73 6f72 0a20 2020 2020 2020 2061  tensor.        a
-00011400: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-00011410: 2872 6573 2c20 696e 7429 0a20 2020 2020  (res, int).     
-00011420: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
-00011430: 2020 2064 6566 2067 6574 5f64 696d 5f76     def get_dim_v
-00011440: 616c 7565 5f74 656e 736f 7228 7365 6c66  alue_tensor(self
-00011450: 2920 2d3e 2055 6e69 6f6e 5b69 6e74 2c20  ) -> Union[int, 
-00011460: 5f74 2e54 656e 736f 725d 3a0a 2020 2020  _t.Tensor]:.    
-00011470: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011480: 496e 6665 7273 2074 6865 2064 696d 2074  Infers the dim t
-00011490: 6869 7320 6178 6973 2073 686f 756c 6420  his axis should 
-000114a0: 6861 7665 2069 6620 756e 6272 6f61 6463  have if unbroadc
-000114b0: 6173 7465 642e 0a20 2020 2020 2020 2049  asted..        I
-000114c0: 6620 6073 656c 662e 7372 635f 6461 7461  f `self.src_data
-000114d0: 6020 6861 7320 6120 706c 6163 6568 6f6c  ` has a placehol
-000114e0: 6465 722c 2077 696c 6c20 7573 6520 7468  der, will use th
-000114f0: 6520 7368 6170 6520 6672 6f6d 2074 6865  e shape from the
-00011500: 7265 2e0a 2020 2020 2020 2020 4f74 6865  re..        Othe
-00011510: 7277 6973 652c 2075 7365 7320 6073 656c  rwise, uses `sel
-00011520: 662e 6469 6d65 6e73 696f 6e60 2028 6966  f.dimension` (if
-00011530: 2073 7461 7469 6329 206f 7220 6073 656c   static) or `sel
-00011540: 662e 6479 6e5f 7369 7a65 6020 2869 6620  f.dyn_size` (if 
-00011550: 6479 6e61 6d69 6329 2e0a 0a20 2020 2020  dynamic)...     
-00011560: 2020 203a 7265 7475 726e 3a20 6d61 7828     :return: max(
-00011570: 7369 7a65 206f 7220 6479 6e5f 7369 7a65  size or dyn_size
-00011580: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00011590: 2020 2020 2020 696d 706f 7274 2072 6574        import ret
-000115a0: 7572 6e6e 2e66 726f 6e74 656e 6420 6173  urnn.frontend as
-000115b0: 2072 660a 0a20 2020 2020 2020 2069 6620   rf..        if 
-000115c0: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
-000115d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000115e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000115f0: 656c 662e 6469 6d65 6e73 696f 6e0a 2020  elf.dimension.  
-00011600: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
-00011610: 6e5f 7369 7a65 5f65 7874 2061 6e64 2073  n_size_ext and s
-00011620: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00011630: 2e70 6c61 6365 686f 6c64 6572 2069 7320  .placeholder is 
-00011640: 6e6f 7420 4e6f 6e65 3a20 2023 2066 6173  not None:  # fas
-00011650: 7420 7061 7468 0a20 2020 2020 2020 2020  t path.         
-00011660: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
-00011670: 697a 655f 6578 742e 6261 7463 685f 6e64  ize_ext.batch_nd
-00011680: 696d 203e 2030 3a0a 2020 2020 2020 2020  im > 0:.        
-00011690: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000116a0: 662e 7265 6475 6365 5f6d 6178 280a 2020  f.reduce_max(.  
-000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116c0: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-000116d0: 6578 742c 0a20 2020 2020 2020 2020 2020  ext,.           
-000116e0: 2020 2020 2020 2020 2061 7869 733d 7365           axis=se
-000116f0: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00011700: 6469 6d5f 7461 6773 2c0a 2020 2020 2020  dim_tags,.      
-00011710: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011720: 4d61 736b 696e 6720 6973 206e 6f74 2061  Masking is not a
-00011730: 6c77 6179 7320 706f 7373 6962 6c65 2068  lways possible h
-00011740: 6572 652c 2065 2e67 2e0a 2020 2020 2020  ere, e.g..      
-00011750: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011760: 7365 6c66 203d 2044 696d 7b27 7365 6c66  self = Dim{'self
-00011770: 2d61 7474 2d6b 6579 7327 5b27 7469 6d65  -att-keys'['time
-00011780: 3a76 6172 3a65 7874 6572 6e5f 6461 7461  :var:extern_data
-00011790: 3a63 6c61 7373 6573 275b 425d 5d7d 2e0a  :classes'[B]]}..
-000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117b0: 2020 2020 7573 655f 6d61 736b 3d46 616c      use_mask=Fal
-000117c0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-000117d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000117e0: 2020 7265 7475 726e 2073 656c 662e 6479    return self.dy
-000117f0: 6e5f 7369 7a65 5f65 7874 0a20 2020 2020  n_size_ext.     
-00011800: 2020 2069 6620 7365 6c66 2e69 735f 6261     if self.is_ba
-00011810: 7463 685f 6469 6d28 293a 0a20 2020 2020  tch_dim():.     
-00011820: 2020 2020 2020 2072 6573 203d 204e 6f6e         res = Non
-00011830: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-00011840: 2073 656c 662e 5f65 7874 7261 2061 6e64   self._extra and
-00011850: 2073 656c 662e 5f65 7874 7261 2e73 7263   self._extra.src
-00011860: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
-00011870: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-00011880: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
-00011890: 612e 6765 745f 6261 7463 685f 6469 6d28  a.get_batch_dim(
-000118a0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000118b0: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
-000118c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000118d0: 6573 203d 2073 656c 662e 6261 7463 682e  es = self.batch.
-000118e0: 6469 6d0a 2020 2020 2020 2020 2020 2020  dim.            
-000118f0: 6966 2069 7369 6e73 7461 6e63 6528 7265  if isinstance(re
-00011900: 732c 2069 6e74 293a 0a20 2020 2020 2020  s, int):.       
-00011910: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00011920: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
-00011930: 6966 2072 6573 2069 7320 6e6f 7420 4e6f  if res is not No
-00011940: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011950: 2020 2020 7265 7475 726e 205f 742e 5465      return _t.Te
-00011960: 6e73 6f72 2822 6261 7463 6822 2c20 6469  nsor("batch", di
-00011970: 6d73 3d28 292c 2064 7479 7065 3d72 662e  ms=(), dtype=rf.
-00011980: 6765 745f 6465 6661 756c 745f 6172 7261  get_default_arra
-00011990: 795f 696e 6465 785f 6474 7970 6528 292c  y_index_dtype(),
-000119a0: 2072 6177 5f74 656e 736f 723d 7265 7329   raw_tensor=res)
-000119b0: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
-000119c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000119d0: 6578 7472 610a 2020 2020 2020 2020 2020  extra.          
-000119e0: 2020 616e 6420 7365 6c66 2e5f 6578 7472    and self._extr
-000119f0: 612e 7372 635f 6461 7461 2069 7320 6e6f  a.src_data is no
-00011a00: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-00011a10: 2020 2061 6e64 2073 656c 662e 5f65 7874     and self._ext
-00011a20: 7261 2e73 7263 5f61 7869 7320 6973 206e  ra.src_axis is n
-00011a30: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-00011a40: 2020 2020 616e 6420 7365 6c66 2e5f 6578      and self._ex
-00011a50: 7472 612e 7372 635f 6461 7461 2e70 6c61  tra.src_data.pla
-00011a60: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
-00011a70: 4e6f 6e65 0a20 2020 2020 2020 2029 3a0a  None.        ):.
-00011a80: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00011a90: 3d20 7365 6c66 2e5f 6578 7472 612e 7372  = self._extra.sr
-00011aa0: 635f 6461 7461 2e67 6574 5f64 696d 2873  c_data.get_dim(s
-00011ab0: 656c 662e 5f65 7874 7261 2e73 7263 5f61  elf._extra.src_a
-00011ac0: 7869 7329 0a20 2020 2020 2020 2020 2020  xis).           
-00011ad0: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
-00011ae0: 6573 2c20 696e 7429 3a0a 2020 2020 2020  es, int):.      
-00011af0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011b00: 2072 6573 0a20 2020 2020 2020 2020 2020   res.           
-00011b10: 2072 6574 7572 6e20 5f74 2e54 656e 736f   return _t.Tenso
-00011b20: 7228 2262 6174 6368 222c 2064 696d 733d  r("batch", dims=
-00011b30: 2829 2c20 6474 7970 653d 7266 2e67 6574  (), dtype=rf.get
-00011b40: 5f64 6566 6175 6c74 5f61 7272 6179 5f69  _default_array_i
-00011b50: 6e64 6578 5f64 7479 7065 2829 2c20 7261  ndex_dtype(), ra
-00011b60: 775f 7465 6e73 6f72 3d72 6573 290a 2020  w_tensor=res).  
-00011b70: 2020 2020 2020 7365 6c66 2e63 6f6d 706c        self.compl
-00011b80: 6574 655f 6479 6e5f 7369 7a65 2829 0a20  ete_dyn_size(). 
-00011b90: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00011ba0: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
-00011bb0: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00011bc0: 742e 706c 6163 6568 6f6c 6465 7220 6973  t.placeholder is
-00011bd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00011be0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00011bf0: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
-00011c00: 685f 6e64 696d 203e 2030 3a0a 2020 2020  h_ndim > 0:.    
-00011c10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011c20: 726e 2072 662e 7265 6475 6365 5f6d 6178  rn rf.reduce_max
-00011c30: 2873 656c 662e 6479 6e5f 7369 7a65 5f65  (self.dyn_size_e
-00011c40: 7874 2c20 6178 6973 3d73 656c 662e 6479  xt, axis=self.dy
-00011c50: 6e5f 7369 7a65 5f65 7874 2e64 696d 5f74  n_size_ext.dim_t
-00011c60: 6167 7329 0a20 2020 2020 2020 2020 2020  ags).           
-00011c70: 2072 6574 7572 6e20 7365 6c66 2e64 796e   return self.dyn
-00011c80: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
-00011c90: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00011ca0: 6e28 2225 733a 206e 6565 6420 706c 6163  n("%s: need plac
-00011cb0: 6568 6f6c 6465 722c 2073 656c 662e 6469  eholder, self.di
-00011cc0: 6d65 6e73 696f 6e20 6f72 2073 656c 662e  mension or self.
-00011cd0: 6479 6e5f 7369 7a65 2066 6f72 2064 696d  dyn_size for dim
-00011ce0: 2076 616c 7565 2220 2520 7365 6c66 290a   value" % self).
-00011cf0: 0a20 2020 2064 6566 2061 7869 735f 7370  .    def axis_sp
-00011d00: 6c69 745f 696e 666f 2873 656c 6629 3a0a  lit_info(self):.
-00011d10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011d20: 2020 2020 3a72 6574 7572 6e3a 2061 7869      :return: axi
-00011d30: 7320 7370 6c69 7420 696e 666f 2e20 7365  s split info. se
-00011d40: 6520 3a66 756e 633a 6067 6574 5f70 6172  e :func:`get_par
-00011d50: 616d 5f61 7865 735f 7370 6c69 745f 696e  am_axes_split_in
-00011d60: 666f 6020 616e 6420 7573 6167 6520 2865  fo` and usage (e
-00011d70: 2e67 2e20 7072 6574 7261 696e 696e 6729  .g. pretraining)
-00011d80: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00011d90: 206c 6973 745b 696e 747c 4e6f 6e65 5d0a   list[int|None].
-00011da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011db0: 2020 2020 7361 6d65 5f62 6173 6520 3d20      same_base = 
-00011dc0: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
-00011dd0: 7365 2829 0a20 2020 2020 2020 206f 7020  se().        op 
-00011de0: 3d20 7365 6c66 2e64 6572 6976 6564 5f66  = self.derived_f
-00011df0: 726f 6d5f 6f70 206f 7220 7361 6d65 5f62  rom_op or same_b
-00011e00: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
-00011e10: 5f6f 700a 2020 2020 2020 2020 6966 206e  _op.        if n
-00011e20: 6f74 206f 703a 0a20 2020 2020 2020 2020  ot op:.         
-00011e30: 2020 2072 6574 7572 6e20 5b73 656c 662e     return [self.
-00011e40: 6469 6d65 6e73 696f 6e5d 0a20 2020 2020  dimension].     
-00011e50: 2020 2069 6620 6f70 2e6b 696e 6420 3d3d     if op.kind ==
-00011e60: 2022 6164 6422 3a0a 2020 2020 2020 2020   "add":.        
-00011e70: 2020 2020 7265 7475 726e 2073 756d 285b      return sum([
-00011e80: 782e 6178 6973 5f73 706c 6974 5f69 6e66  x.axis_split_inf
-00011e90: 6f28 2920 666f 7220 7820 696e 206f 702e  o() for x in op.
-00011ea0: 696e 7075 7473 5d2c 205b 5d29 2020 2320  inputs], [])  # 
-00011eb0: 666c 6174 7465 6e0a 2020 2020 2020 2020  flatten.        
-00011ec0: 6966 206f 702e 6b69 6e64 203d 3d20 226d  if op.kind == "m
-00011ed0: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
-00011ee0: 2072 6573 203d 205b 315d 0a20 2020 2020   res = [1].     
-00011ef0: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
-00011f00: 6f70 2e69 6e70 7574 733a 0a20 2020 2020  op.inputs:.     
-00011f10: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00011f20: 2073 756d 285b 6e20 2a20 782e 6178 6973   sum([n * x.axis
-00011f30: 5f73 706c 6974 5f69 6e66 6f28 2920 6966  _split_info() if
-00011f40: 206e 2069 7320 6e6f 7420 4e6f 6e65 2065   n is not None e
-00011f50: 6c73 6520 4e6f 6e65 2066 6f72 206e 2069  lse None for n i
-00011f60: 6e20 7265 735d 2c20 5b5d 2920 2023 2066  n res], [])  # f
-00011f70: 6c61 7474 656e 0a20 2020 2020 2020 2020  latten.         
-00011f80: 2020 2072 6574 7572 6e20 7265 730a 2020     return res.  
-00011f90: 2020 2020 2020 7265 7475 726e 205b 7365        return [se
-00011fa0: 6c66 2e64 696d 656e 7369 6f6e 5d0a 0a20  lf.dimension].. 
-00011fb0: 2020 2064 6566 205f 6765 745f 7361 6d65     def _get_same
-00011fc0: 5f62 6173 655f 6578 7472 6128 7365 6c66  _base_extra(self
-00011fd0: 2920 2d3e 204f 7074 696f 6e61 6c5b 5f44  ) -> Optional[_D
-00011fe0: 696d 4578 7472 615d 3a0a 2020 2020 2020  imExtra]:.      
-00011ff0: 2020 6966 206e 6f74 2073 656c 662e 5f65    if not self._e
-00012000: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
-00012010: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00012020: 2020 2020 2020 6261 7365 203d 2073 656c        base = sel
-00012030: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
-00012040: 290a 2020 2020 2020 2020 2320 6e6f 696e  ).        # noin
-00012050: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-00012060: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-00012070: 2020 2072 6574 7572 6e20 6261 7365 2e5f     return base._
-00012080: 6578 7472 610a 0a20 2020 2064 6566 205f  extra..    def _
-00012090: 6d61 6b65 5f65 7874 7261 2873 656c 663a  make_extra(self:
-000120a0: 205f 642e 4469 6d29 202d 3e20 5f44 696d   _d.Dim) -> _Dim
-000120b0: 4578 7472 613a 0a20 2020 2020 2020 2069  Extra:.        i
-000120c0: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
-000120d0: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
-000120e0: 656c 662e 5f65 7874 7261 203d 205f 4469  elf._extra = _Di
-000120f0: 6d45 7874 7261 2864 696d 3d73 656c 6629  mExtra(dim=self)
-00012100: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012110: 7365 6c66 2e5f 6578 7472 610a 0a20 2020  self._extra..   
-00012120: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00012130: 6566 2076 6f63 6162 2873 656c 6629 3a0a  ef vocab(self):.
-00012140: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012150: 2020 2020 3a72 7479 7065 3a20 7265 7475      :rtype: retu
-00012160: 726e 6e2e 6461 7461 7365 7473 2e75 7469  rnn.datasets.uti
-00012170: 6c2e 766f 6361 6275 6c61 7279 2e56 6f63  l.vocabulary.Voc
-00012180: 6162 756c 6172 797c 4e6f 6e65 0a20 2020  abulary|None.   
-00012190: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000121a0: 2065 7874 7261 203d 2073 656c 662e 5f67   extra = self._g
-000121b0: 6574 5f73 616d 655f 6261 7365 5f65 7874  et_same_base_ext
-000121c0: 7261 2829 0a20 2020 2020 2020 2069 6620  ra().        if 
-000121d0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
-000121e0: 2020 2072 6574 7572 6e20 6578 7472 612e     return extra.
-000121f0: 766f 6361 620a 2020 2020 2020 2020 7265  vocab.        re
-00012200: 7475 726e 204e 6f6e 650a 0a20 2020 2040  turn None..    @
-00012210: 766f 6361 622e 7365 7474 6572 0a20 2020  vocab.setter.   
-00012220: 2064 6566 2076 6f63 6162 2873 656c 662c   def vocab(self,
-00012230: 2076 6f63 6162 293a 0a20 2020 2020 2020   vocab):.       
-00012240: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00012250: 7261 6d20 7265 7475 726e 6e2e 6461 7461  ram returnn.data
-00012260: 7365 7473 2e75 7469 6c2e 766f 6361 6275  sets.util.vocabu
-00012270: 6c61 7279 2e56 6f63 6162 756c 6172 797c  lary.Vocabulary|
-00012280: 4e6f 6e65 2076 6f63 6162 3a0a 2020 2020  None vocab:.    
-00012290: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000122a0: 6966 2076 6f63 6162 2069 7320 7365 6c66  if vocab is self
-000122b0: 2e76 6f63 6162 3a0a 2020 2020 2020 2020  .vocab:.        
-000122c0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000122d0: 2020 2069 6620 7365 6c66 2e73 616d 655f     if self.same_
-000122e0: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
-000122f0: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
-00012300: 7365 2829 2e76 6f63 6162 203d 2076 6f63  se().vocab = voc
-00012310: 6162 0a20 2020 2020 2020 2020 2020 2072  ab.            r
-00012320: 6574 7572 6e0a 2020 2020 2020 2020 6578  eturn.        ex
-00012330: 7472 6120 3d20 7365 6c66 2e5f 6765 745f  tra = self._get_
-00012340: 7361 6d65 5f62 6173 655f 6578 7472 6128  same_base_extra(
-00012350: 290a 2020 2020 2020 2020 6966 2065 7874  ).        if ext
-00012360: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
-00012370: 6578 7472 612e 766f 6361 6220 3d20 766f  extra.vocab = vo
-00012380: 6361 620a 0a20 2020 2023 2054 6865 206b  cab..    # The k
-00012390: 696e 6420 6f66 206f 7065 7261 7469 6f6e  ind of operation
-000123a0: 7320 7765 2068 6176 653a 0a20 2020 2023  s we have:.    #
-000123b0: 2061 202b 2062 3a20 7061 6464 696e 672c   a + b: padding,
-000123c0: 2063 6f6e 6361 740a 2020 2020 2320 6120   concat.    # a 
-000123d0: 2d20 623a 2077 696e 646f 7720 7769 7468  - b: window with
-000123e0: 2076 616c 6964 2066 7261 6d65 7320 6f6e   valid frames on
-000123f0: 6c79 0a20 2020 2023 2061 202a 2062 3a20  ly.    # a * b: 
-00012400: 6d65 7267 6520 6469 6d73 2c20 7570 7361  merge dims, upsa
-00012410: 6d70 6c65 2c20 7472 616e 7370 6f73 6564  mple, transposed
-00012420: 2063 6f6e 7620 7769 7468 2073 7472 6964   conv with strid
-00012430: 696e 670a 2020 2020 2320 6120 2f20 6220  ing.    # a / b 
-00012440: 2877 6865 6e20 6120 2520 6220 3d3d 2030  (when a % b == 0
-00012450: 293a 2073 706c 6974 2064 696d 732c 2064  ): split dims, d
-00012460: 6f77 6e73 616d 706c 652c 2063 6f6e 7620  ownsample, conv 
-00012470: 7769 7468 2073 7472 6964 696e 670a 2020  with striding.  
-00012480: 2020 2320 6365 696c 6469 7628 612c 2062    # ceildiv(a, b
-00012490: 293a 2063 6f6e 7620 7769 7468 2073 7472  ): conv with str
-000124a0: 6964 696e 670a 2020 2020 2320 6375 7374  iding.    # cust
-000124b0: 6f6d 3a20 7265 7065 6174 2c20 7265 6d6f  om: repeat, remo
-000124c0: 7665 2c20 6d61 736b 2c20 6c6f 6f70 2077  ve, mask, loop w
-000124d0: 6974 6820 6479 6e20 656e 640a 2020 2020  ith dyn end.    
-000124e0: 2320 4e6f 7465 2074 6861 7420 7765 2064  # Note that we d
-000124f0: 6966 6665 7265 6e74 6961 7465 2062 6574  ifferentiate bet
-00012500: 7765 656e 2074 6865 206f 7264 6572 2c20  ween the order, 
-00012510: 692e 652e 2061 202b 2062 2021 3d20 6220  i.e. a + b != b 
-00012520: 2b20 612e 0a20 2020 2023 204e 6f74 6520  + a..    # Note 
-00012530: 7468 6174 2077 6520 616c 7761 7973 2068  that we always h
-00012540: 6176 6520 7468 6520 6173 7375 6d70 7469  ave the assumpti
-00012550: 6f6e 2074 6861 7420 6120 6469 6d65 6e73  on that a dimens
-00012560: 696f 6e20 6973 206e 6f6e 2d6e 6567 6174  ion is non-negat
-00012570: 6976 652e 0a20 2020 2023 2054 6869 7320  ive..    # This 
-00012580: 6173 7375 6d70 7469 6f6e 2069 7320 6e65  assumption is ne
-00012590: 6365 7373 6172 7920 666f 7220 736f 6d65  cessary for some
-000125a0: 2073 696d 706c 6966 6963 6174 696f 6e73   simplifications
-000125b0: 2e0a 2020 2020 2320 6874 7470 733a 2f2f  ..    # https://
-000125c0: 6769 7468 7562 2e63 6f6d 2f72 7774 682d  github.com/rwth-
-000125d0: 6936 2f72 6574 7572 6e6e 2f70 756c 6c2f  i6/returnn/pull/
-000125e0: 3835 330a 0a20 2020 2064 6566 205f 5f61  853..    def __a
-000125f0: 6464 5f5f 2873 656c 663a 2044 696d 2c20  dd__(self: Dim, 
-00012600: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00012610: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-00012620: 616d 2044 696d 7c69 6e74 206f 7468 6572  am Dim|int other
-00012630: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-00012640: 6e3a 2073 656c 6620 2b20 6f74 6865 722e  n: self + other.
-00012650: 206e 6f74 6520 7468 6174 2074 6869 7320   note that this 
-00012660: 6973 206e 6f74 2063 6f6d 6d75 7461 7469  is not commutati
-00012670: 7665 2c20 692e 652e 2064 6966 6665 7265  ve, i.e. differe
-00012680: 6e74 2066 726f 6d20 6f74 6865 7220 2b20  nt from other + 
-00012690: 7365 6c66 2e0a 2020 2020 2020 2020 3a72  self..        :r
-000126a0: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
-000126b0: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
-000126c0: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
-000126d0: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
-000126e0: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
-000126f0: 7874 656e 645f 6164 645f 7375 625f 286f  xtend_add_sub_(o
-00012700: 7468 6572 2c20 6b69 6e64 3d22 6164 6422  ther, kind="add"
-00012710: 2c20 7269 6768 743d 5472 7565 290a 2020  , right=True).  
-00012720: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00012730: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
-00012740: 6465 6620 5f5f 7261 6464 5f5f 2873 656c  def __radd__(sel
-00012750: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
-00012760: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012770: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
-00012780: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
-00012790: 2020 3a72 6574 7572 6e3a 206f 7468 6572    :return: other
-000127a0: 202b 2073 656c 660a 2020 2020 2020 2020   + self.        
-000127b0: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
-000127c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000127d0: 7465 726d 203d 205f 4f70 4c69 6e65 6172  term = _OpLinear
-000127e0: 5465 726d 2e66 726f 6d5f 6469 6d28 7365  Term.from_dim(se
-000127f0: 6c66 290a 2020 2020 2020 2020 7465 726d  lf).        term
-00012800: 2e65 7874 656e 645f 6164 645f 7375 625f  .extend_add_sub_
-00012810: 286f 7468 6572 2c20 6b69 6e64 3d22 6164  (other, kind="ad
-00012820: 6422 2c20 7269 6768 743d 4661 6c73 6529  d", right=False)
-00012830: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012840: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
-00012850: 2020 2064 6566 205f 5f73 7562 5f5f 2873     def __sub__(s
-00012860: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
+00010f20: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
+00010f30: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
+00010f40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00010f50: 6479 6e5f 7369 7a65 5f65 7874 0a0a 2020  dyn_size_ext..  
+00010f60: 2020 2020 2020 696d 706f 7274 2072 6574        import ret
+00010f70: 7572 6e6e 2e66 726f 6e74 656e 6420 6173  urnn.frontend as
+00010f80: 2072 660a 0a20 2020 2020 2020 2061 7373   rf..        ass
+00010f90: 6572 7420 7365 6c66 2e73 697a 6520 6973  ert self.size is
+00010fa0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+00010fb0: 2020 7265 7475 726e 2072 662e 636f 6e76    return rf.conv
+00010fc0: 6572 745f 746f 5f74 656e 736f 7228 7365  ert_to_tensor(se
+00010fd0: 6c66 2e73 697a 652c 206e 616d 653d 2225  lf.size, name="%
+00010fe0: 733a 7369 7a65 2220 2520 7365 6c66 2e64  s:size" % self.d
+00010ff0: 6573 6372 6970 7469 6f6e 290a 0a20 2020  escription)..   
+00011000: 2064 6566 2067 6574 5f64 696d 5f76 616c   def get_dim_val
+00011010: 7565 2873 656c 6629 202d 3e20 556e 696f  ue(self) -> Unio
+00011020: 6e5b 696e 742c 205f 742e 5261 7754 656e  n[int, _t.RawTen
+00011030: 736f 7254 7970 655d 3a0a 2020 2020 2020  sorType]:.      
+00011040: 2020 2222 220a 2020 2020 2020 2020 496e    """.        In
+00011050: 6665 7273 2074 6865 2064 696d 2074 6869  fers the dim thi
+00011060: 7320 6178 6973 2073 686f 756c 6420 6861  s axis should ha
+00011070: 7665 2069 6620 756e 6272 6f61 6463 6173  ve if unbroadcas
+00011080: 7465 642e 0a20 2020 2020 2020 2049 6620  ted..        If 
+00011090: 6073 656c 662e 7372 635f 6461 7461 6020  `self.src_data` 
+000110a0: 6861 7320 6120 706c 6163 6568 6f6c 6465  has a placeholde
+000110b0: 722c 2077 696c 6c20 7573 6520 7468 6520  r, will use the 
+000110c0: 7368 6170 6520 6672 6f6d 2074 6865 7265  shape from there
+000110d0: 2e0a 2020 2020 2020 2020 4f74 6865 7277  ..        Otherw
+000110e0: 6973 652c 2075 7365 7320 6073 656c 662e  ise, uses `self.
+000110f0: 6469 6d65 6e73 696f 6e60 2028 6966 2073  dimension` (if s
+00011100: 7461 7469 6329 206f 7220 6073 656c 662e  tatic) or `self.
+00011110: 6479 6e5f 7369 7a65 6020 2869 6620 6479  dyn_size` (if dy
+00011120: 6e61 6d69 6329 2e0a 0a20 2020 2020 2020  namic)...       
+00011130: 203a 7265 7475 726e 3a20 6d61 7828 7369   :return: max(si
+00011140: 7a65 206f 7220 6479 6e5f 7369 7a65 290a  ze or dyn_size).
+00011150: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011160: 2020 2020 7265 7320 3d20 7365 6c66 2e67      res = self.g
+00011170: 6574 5f64 696d 5f76 616c 7565 5f74 656e  et_dim_value_ten
+00011180: 736f 7228 290a 2020 2020 2020 2020 6966  sor().        if
+00011190: 2069 7369 6e73 7461 6e63 6528 7265 732c   isinstance(res,
+000111a0: 205f 742e 5465 6e73 6f72 293a 0a20 2020   _t.Tensor):.   
+000111b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000111c0: 7265 732e 6469 6d73 203d 3d20 2829 0a20  res.dims == (). 
+000111d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000111e0: 6e20 7265 732e 7261 775f 7465 6e73 6f72  n res.raw_tensor
+000111f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00011200: 6973 696e 7374 616e 6365 2872 6573 2c20  isinstance(res, 
+00011210: 696e 7429 0a20 2020 2020 2020 2072 6574  int).        ret
+00011220: 7572 6e20 7265 730a 0a20 2020 2064 6566  urn res..    def
+00011230: 2067 6574 5f64 696d 5f76 616c 7565 5f74   get_dim_value_t
+00011240: 656e 736f 7228 7365 6c66 2920 2d3e 2055  ensor(self) -> U
+00011250: 6e69 6f6e 5b69 6e74 2c20 5f74 2e54 656e  nion[int, _t.Ten
+00011260: 736f 725d 3a0a 2020 2020 2020 2020 2222  sor]:.        ""
+00011270: 220a 2020 2020 2020 2020 496e 6665 7273  ".        Infers
+00011280: 2074 6865 2064 696d 2074 6869 7320 6178   the dim this ax
+00011290: 6973 2073 686f 756c 6420 6861 7665 2069  is should have i
+000112a0: 6620 756e 6272 6f61 6463 6173 7465 642e  f unbroadcasted.
+000112b0: 0a20 2020 2020 2020 2049 6620 6073 656c  .        If `sel
+000112c0: 662e 7372 635f 6461 7461 6020 6861 7320  f.src_data` has 
+000112d0: 6120 706c 6163 6568 6f6c 6465 722c 2077  a placeholder, w
+000112e0: 696c 6c20 7573 6520 7468 6520 7368 6170  ill use the shap
+000112f0: 6520 6672 6f6d 2074 6865 7265 2e0a 2020  e from there..  
+00011300: 2020 2020 2020 4f74 6865 7277 6973 652c        Otherwise,
+00011310: 2075 7365 7320 6073 656c 662e 6469 6d65   uses `self.dime
+00011320: 6e73 696f 6e60 2028 6966 2073 7461 7469  nsion` (if stati
+00011330: 6329 206f 7220 6073 656c 662e 6479 6e5f  c) or `self.dyn_
+00011340: 7369 7a65 6020 2869 6620 6479 6e61 6d69  size` (if dynami
+00011350: 6329 2e0a 0a20 2020 2020 2020 203a 7265  c)...        :re
+00011360: 7475 726e 3a20 6d61 7828 7369 7a65 206f  turn: max(size o
+00011370: 7220 6479 6e5f 7369 7a65 290a 2020 2020  r dyn_size).    
+00011380: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011390: 696d 706f 7274 2072 6574 7572 6e6e 2e66  import returnn.f
+000113a0: 726f 6e74 656e 6420 6173 2072 660a 0a20  rontend as rf.. 
+000113b0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+000113c0: 696d 656e 7369 6f6e 2069 7320 6e6f 7420  imension is not 
+000113d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000113e0: 2020 7265 7475 726e 2073 656c 662e 6469    return self.di
+000113f0: 6d65 6e73 696f 6e0a 2020 2020 2020 2020  mension.        
+00011400: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
+00011410: 5f65 7874 2061 6e64 2073 656c 662e 6479  _ext and self.dy
+00011420: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
+00011430: 686f 6c64 6572 2069 7320 6e6f 7420 4e6f  holder is not No
+00011440: 6e65 3a20 2023 2066 6173 7420 7061 7468  ne:  # fast path
+00011450: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011460: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00011470: 742e 6261 7463 685f 6e64 696d 203e 2030  t.batch_ndim > 0
+00011480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011490: 2020 7265 7475 726e 2072 662e 7265 6475    return rf.redu
+000114a0: 6365 5f6d 6178 280a 2020 2020 2020 2020  ce_max(.        
+000114b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000114c0: 2e64 796e 5f73 697a 655f 6578 742c 0a20  .dyn_size_ext,. 
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114e0: 2020 2061 7869 733d 7365 6c66 2e64 796e     axis=self.dyn
+000114f0: 5f73 697a 655f 6578 742e 6469 6d5f 7461  _size_ext.dim_ta
+00011500: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
+00011510: 2020 2020 2020 2020 2320 4d61 736b 696e          # Maskin
+00011520: 6720 6973 206e 6f74 2061 6c77 6179 7320  g is not always 
+00011530: 706f 7373 6962 6c65 2068 6572 652c 2065  possible here, e
+00011540: 2e67 2e0a 2020 2020 2020 2020 2020 2020  .g..            
+00011550: 2020 2020 2020 2020 2320 7365 6c66 203d          # self =
+00011560: 2044 696d 7b27 7365 6c66 2d61 7474 2d6b   Dim{'self-att-k
+00011570: 6579 7327 5b27 7469 6d65 3a76 6172 3a65  eys'['time:var:e
+00011580: 7874 6572 6e5f 6461 7461 3a63 6c61 7373  xtern_data:class
+00011590: 6573 275b 425d 5d7d 2e0a 2020 2020 2020  es'[B]]}..      
+000115a0: 2020 2020 2020 2020 2020 2020 2020 7573                us
+000115b0: 655f 6d61 736b 3d46 616c 7365 2c0a 2020  e_mask=False,.  
+000115c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000115d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000115e0: 726e 2073 656c 662e 6479 6e5f 7369 7a65  rn self.dyn_size
+000115f0: 5f65 7874 0a20 2020 2020 2020 2069 6620  _ext.        if 
+00011600: 7365 6c66 2e69 735f 6261 7463 685f 6469  self.is_batch_di
+00011610: 6d28 293a 0a20 2020 2020 2020 2020 2020  m():.           
+00011620: 2072 6573 203d 204e 6f6e 650a 2020 2020   res = None.    
+00011630: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011640: 5f65 7874 7261 2061 6e64 2073 656c 662e  _extra and self.
+00011650: 5f65 7874 7261 2e73 7263 5f64 6174 613a  _extra.src_data:
+00011660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011670: 2072 6573 203d 2073 656c 662e 5f65 7874   res = self._ext
+00011680: 7261 2e73 7263 5f64 6174 612e 6765 745f  ra.src_data.get_
+00011690: 6261 7463 685f 6469 6d28 290a 2020 2020  batch_dim().    
+000116a0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+000116b0: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
+000116c0: 2020 2020 2020 2020 2072 6573 203d 2073           res = s
+000116d0: 656c 662e 6261 7463 682e 6469 6d0a 2020  elf.batch.dim.  
+000116e0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+000116f0: 6e73 7461 6e63 6528 7265 732c 2069 6e74  nstance(res, int
+00011700: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011710: 2020 2072 6574 7572 6e20 7265 730a 2020     return res.  
+00011720: 2020 2020 2020 2020 2020 6966 2072 6573            if res
+00011730: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00011740: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00011750: 7475 726e 205f 742e 5465 6e73 6f72 2822  turn _t.Tensor("
+00011760: 6261 7463 6822 2c20 6469 6d73 3d28 292c  batch", dims=(),
+00011770: 2064 7479 7065 3d72 662e 6765 745f 6465   dtype=rf.get_de
+00011780: 6661 756c 745f 6172 7261 795f 696e 6465  fault_array_inde
+00011790: 785f 6474 7970 6528 292c 2072 6177 5f74  x_dtype(), raw_t
+000117a0: 656e 736f 723d 7265 7329 0a20 2020 2020  ensor=res).     
+000117b0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+000117c0: 2020 2020 7365 6c66 2e5f 6578 7472 610a      self._extra.
+000117d0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+000117e0: 7365 6c66 2e5f 6578 7472 612e 7372 635f  self._extra.src_
+000117f0: 6461 7461 2069 7320 6e6f 7420 4e6f 6e65  data is not None
+00011800: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+00011810: 2073 656c 662e 5f65 7874 7261 2e73 7263   self._extra.src
+00011820: 5f61 7869 7320 6973 206e 6f74 204e 6f6e  _axis is not Non
+00011830: 650a 2020 2020 2020 2020 2020 2020 616e  e.            an
+00011840: 6420 7365 6c66 2e5f 6578 7472 612e 7372  d self._extra.sr
+00011850: 635f 6461 7461 2e70 6c61 6365 686f 6c64  c_data.placehold
+00011860: 6572 2069 7320 6e6f 7420 4e6f 6e65 0a20  er is not None. 
+00011870: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00011880: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
+00011890: 2e5f 6578 7472 612e 7372 635f 6461 7461  ._extra.src_data
+000118a0: 2e67 6574 5f64 696d 2873 656c 662e 5f65  .get_dim(self._e
+000118b0: 7874 7261 2e73 7263 5f61 7869 7329 0a20  xtra.src_axis). 
+000118c0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000118d0: 696e 7374 616e 6365 2872 6573 2c20 696e  instance(res, in
+000118e0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000118f0: 2020 2020 7265 7475 726e 2072 6573 0a20      return res. 
+00011900: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00011910: 6e20 5f74 2e54 656e 736f 7228 2262 6174  n _t.Tensor("bat
+00011920: 6368 222c 2064 696d 733d 2829 2c20 6474  ch", dims=(), dt
+00011930: 7970 653d 7266 2e67 6574 5f64 6566 6175  ype=rf.get_defau
+00011940: 6c74 5f61 7272 6179 5f69 6e64 6578 5f64  lt_array_index_d
+00011950: 7479 7065 2829 2c20 7261 775f 7465 6e73  type(), raw_tens
+00011960: 6f72 3d72 6573 290a 2020 2020 2020 2020  or=res).        
+00011970: 7365 6c66 2e63 6f6d 706c 6574 655f 6479  self.complete_dy
+00011980: 6e5f 7369 7a65 2829 0a20 2020 2020 2020  n_size().       
+00011990: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
+000119a0: 655f 6578 7420 616e 6420 7365 6c66 2e64  e_ext and self.d
+000119b0: 796e 5f73 697a 655f 6578 742e 706c 6163  yn_size_ext.plac
+000119c0: 6568 6f6c 6465 7220 6973 206e 6f74 204e  eholder is not N
+000119d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000119e0: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
+000119f0: 655f 6578 742e 6261 7463 685f 6e64 696d  e_ext.batch_ndim
+00011a00: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00011a10: 2020 2020 2020 7265 7475 726e 2072 662e        return rf.
+00011a20: 7265 6475 6365 5f6d 6178 2873 656c 662e  reduce_max(self.
+00011a30: 6479 6e5f 7369 7a65 5f65 7874 2c20 6178  dyn_size_ext, ax
+00011a40: 6973 3d73 656c 662e 6479 6e5f 7369 7a65  is=self.dyn_size
+00011a50: 5f65 7874 2e64 696d 5f74 6167 7329 0a20  _ext.dim_tags). 
+00011a60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00011a70: 6e20 7365 6c66 2e64 796e 5f73 697a 655f  n self.dyn_size_
+00011a80: 6578 740a 2020 2020 2020 2020 7261 6973  ext.        rais
+00011a90: 6520 4578 6365 7074 696f 6e28 2225 733a  e Exception("%s:
+00011aa0: 206e 6565 6420 706c 6163 6568 6f6c 6465   need placeholde
+00011ab0: 722c 2073 656c 662e 6469 6d65 6e73 696f  r, self.dimensio
+00011ac0: 6e20 6f72 2073 656c 662e 6479 6e5f 7369  n or self.dyn_si
+00011ad0: 7a65 2066 6f72 2064 696d 2076 616c 7565  ze for dim value
+00011ae0: 2220 2520 7365 6c66 290a 0a20 2020 2064  " % self)..    d
+00011af0: 6566 2061 7869 735f 7370 6c69 745f 696e  ef axis_split_in
+00011b00: 666f 2873 656c 6629 3a0a 2020 2020 2020  fo(self):.      
+00011b10: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00011b20: 6574 7572 6e3a 2061 7869 7320 7370 6c69  eturn: axis spli
+00011b30: 7420 696e 666f 2e20 7365 6520 3a66 756e  t info. see :fun
+00011b40: 633a 6067 6574 5f70 6172 616d 5f61 7865  c:`get_param_axe
+00011b50: 735f 7370 6c69 745f 696e 666f 6020 616e  s_split_info` an
+00011b60: 6420 7573 6167 6520 2865 2e67 2e20 7072  d usage (e.g. pr
+00011b70: 6574 7261 696e 696e 6729 0a20 2020 2020  etraining).     
+00011b80: 2020 203a 7274 7970 653a 206c 6973 745b     :rtype: list[
+00011b90: 696e 747c 4e6f 6e65 5d0a 2020 2020 2020  int|None].      
+00011ba0: 2020 2222 220a 2020 2020 2020 2020 7361    """.        sa
+00011bb0: 6d65 5f62 6173 6520 3d20 7365 6c66 2e67  me_base = self.g
+00011bc0: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
+00011bd0: 2020 2020 2020 206f 7020 3d20 7365 6c66         op = self
+00011be0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00011bf0: 206f 7220 7361 6d65 5f62 6173 652e 6465   or same_base.de
+00011c00: 7269 7665 645f 6672 6f6d 5f6f 700a 2020  rived_from_op.  
+00011c10: 2020 2020 2020 6966 206e 6f74 206f 703a        if not op:
+00011c20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011c30: 7572 6e20 5b73 656c 662e 6469 6d65 6e73  urn [self.dimens
+00011c40: 696f 6e5d 0a20 2020 2020 2020 2069 6620  ion].        if 
+00011c50: 6f70 2e6b 696e 6420 3d3d 2022 6164 6422  op.kind == "add"
+00011c60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00011c70: 7475 726e 2073 756d 285b 782e 6178 6973  turn sum([x.axis
+00011c80: 5f73 706c 6974 5f69 6e66 6f28 2920 666f  _split_info() fo
+00011c90: 7220 7820 696e 206f 702e 696e 7075 7473  r x in op.inputs
+00011ca0: 5d2c 205b 5d29 2020 2320 666c 6174 7465  ], [])  # flatte
+00011cb0: 6e0a 2020 2020 2020 2020 6966 206f 702e  n.        if op.
+00011cc0: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
+00011cd0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
+00011ce0: 205b 315d 0a20 2020 2020 2020 2020 2020   [1].           
+00011cf0: 2066 6f72 2078 2069 6e20 6f70 2e69 6e70   for x in op.inp
+00011d00: 7574 733a 0a20 2020 2020 2020 2020 2020  uts:.           
+00011d10: 2020 2020 2072 6573 203d 2073 756d 285b       res = sum([
+00011d20: 6e20 2a20 782e 6178 6973 5f73 706c 6974  n * x.axis_split
+00011d30: 5f69 6e66 6f28 2920 6966 206e 2069 7320  _info() if n is 
+00011d40: 6e6f 7420 4e6f 6e65 2065 6c73 6520 4e6f  not None else No
+00011d50: 6e65 2066 6f72 206e 2069 6e20 7265 735d  ne for n in res]
+00011d60: 2c20 5b5d 2920 2023 2066 6c61 7474 656e  , [])  # flatten
+00011d70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011d80: 7572 6e20 7265 730a 2020 2020 2020 2020  urn res.        
+00011d90: 7265 7475 726e 205b 7365 6c66 2e64 696d  return [self.dim
+00011da0: 656e 7369 6f6e 5d0a 0a20 2020 2064 6566  ension]..    def
+00011db0: 205f 6765 745f 7361 6d65 5f62 6173 655f   _get_same_base_
+00011dc0: 6578 7472 6128 7365 6c66 2920 2d3e 204f  extra(self) -> O
+00011dd0: 7074 696f 6e61 6c5b 5f44 696d 4578 7472  ptional[_DimExtr
+00011de0: 615d 3a0a 2020 2020 2020 2020 6966 206e  a]:.        if n
+00011df0: 6f74 2073 656c 662e 5f65 7874 7261 3a0a  ot self._extra:.
+00011e00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011e10: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+00011e20: 6261 7365 203d 2073 656c 662e 6765 745f  base = self.get_
+00011e30: 7361 6d65 5f62 6173 6528 290a 2020 2020  same_base().    
+00011e40: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+00011e50: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+00011e60: 6d62 6572 0a20 2020 2020 2020 2072 6574  mber.        ret
+00011e70: 7572 6e20 6261 7365 2e5f 6578 7472 610a  urn base._extra.
+00011e80: 0a20 2020 2064 6566 205f 6d61 6b65 5f65  .    def _make_e
+00011e90: 7874 7261 2873 656c 663a 205f 642e 4469  xtra(self: _d.Di
+00011ea0: 6d29 202d 3e20 5f44 696d 4578 7472 613a  m) -> _DimExtra:
+00011eb0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00011ec0: 7365 6c66 2e5f 6578 7472 613a 0a20 2020  self._extra:.   
+00011ed0: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+00011ee0: 7874 7261 203d 205f 4469 6d45 7874 7261  xtra = _DimExtra
+00011ef0: 2864 696d 3d73 656c 6629 0a20 2020 2020  (dim=self).     
+00011f00: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00011f10: 6578 7472 610a 0a20 2020 2040 7072 6f70  extra..    @prop
+00011f20: 6572 7479 0a20 2020 2064 6566 2076 6f63  erty.    def voc
+00011f30: 6162 2873 656c 6629 3a0a 2020 2020 2020  ab(self):.      
+00011f40: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00011f50: 7479 7065 3a20 7265 7475 726e 6e2e 6461  type: returnn.da
+00011f60: 7461 7365 7473 2e75 7469 6c2e 766f 6361  tasets.util.voca
+00011f70: 6275 6c61 7279 2e56 6f63 6162 756c 6172  bulary.Vocabular
+00011f80: 797c 4e6f 6e65 0a20 2020 2020 2020 2022  y|None.        "
+00011f90: 2222 0a20 2020 2020 2020 2065 7874 7261  "".        extra
+00011fa0: 203d 2073 656c 662e 5f67 6574 5f73 616d   = self._get_sam
+00011fb0: 655f 6261 7365 5f65 7874 7261 2829 0a20  e_base_extra(). 
+00011fc0: 2020 2020 2020 2069 6620 6578 7472 613a         if extra:
+00011fd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011fe0: 7572 6e20 6578 7472 612e 766f 6361 620a  urn extra.vocab.
+00011ff0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00012000: 6f6e 650a 0a20 2020 2040 766f 6361 622e  one..    @vocab.
+00012010: 7365 7474 6572 0a20 2020 2064 6566 2076  setter.    def v
+00012020: 6f63 6162 2873 656c 662c 2076 6f63 6162  ocab(self, vocab
+00012030: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012040: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
+00012050: 7475 726e 6e2e 6461 7461 7365 7473 2e75  turnn.datasets.u
+00012060: 7469 6c2e 766f 6361 6275 6c61 7279 2e56  til.vocabulary.V
+00012070: 6f63 6162 756c 6172 797c 4e6f 6e65 2076  ocabulary|None v
+00012080: 6f63 6162 3a0a 2020 2020 2020 2020 2222  ocab:.        ""
+00012090: 220a 2020 2020 2020 2020 6966 2076 6f63  ".        if voc
+000120a0: 6162 2069 7320 7365 6c66 2e76 6f63 6162  ab is self.vocab
+000120b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000120c0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+000120d0: 7365 6c66 2e73 616d 655f 6173 3a0a 2020  self.same_as:.  
+000120e0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+000120f0: 6574 5f73 616d 655f 6261 7365 2829 2e76  et_same_base().v
+00012100: 6f63 6162 203d 2076 6f63 6162 0a20 2020  ocab = vocab.   
+00012110: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00012120: 2020 2020 2020 2020 6578 7472 6120 3d20          extra = 
+00012130: 7365 6c66 2e5f 6765 745f 7361 6d65 5f62  self._get_same_b
+00012140: 6173 655f 6578 7472 6128 290a 2020 2020  ase_extra().    
+00012150: 2020 2020 6966 2065 7874 7261 3a0a 2020      if extra:.  
+00012160: 2020 2020 2020 2020 2020 6578 7472 612e            extra.
+00012170: 766f 6361 6220 3d20 766f 6361 620a 0a20  vocab = vocab.. 
+00012180: 2020 2023 2054 6865 206b 696e 6420 6f66     # The kind of
+00012190: 206f 7065 7261 7469 6f6e 7320 7765 2068   operations we h
+000121a0: 6176 653a 0a20 2020 2023 2061 202b 2062  ave:.    # a + b
+000121b0: 3a20 7061 6464 696e 672c 2063 6f6e 6361  : padding, conca
+000121c0: 740a 2020 2020 2320 6120 2d20 623a 2077  t.    # a - b: w
+000121d0: 696e 646f 7720 7769 7468 2076 616c 6964  indow with valid
+000121e0: 2066 7261 6d65 7320 6f6e 6c79 0a20 2020   frames only.   
+000121f0: 2023 2061 202a 2062 3a20 6d65 7267 6520   # a * b: merge 
+00012200: 6469 6d73 2c20 7570 7361 6d70 6c65 2c20  dims, upsample, 
+00012210: 7472 616e 7370 6f73 6564 2063 6f6e 7620  transposed conv 
+00012220: 7769 7468 2073 7472 6964 696e 670a 2020  with striding.  
+00012230: 2020 2320 6120 2f20 6220 2877 6865 6e20    # a / b (when 
+00012240: 6120 2520 6220 3d3d 2030 293a 2073 706c  a % b == 0): spl
+00012250: 6974 2064 696d 732c 2064 6f77 6e73 616d  it dims, downsam
+00012260: 706c 652c 2063 6f6e 7620 7769 7468 2073  ple, conv with s
+00012270: 7472 6964 696e 670a 2020 2020 2320 6365  triding.    # ce
+00012280: 696c 6469 7628 612c 2062 293a 2063 6f6e  ildiv(a, b): con
+00012290: 7620 7769 7468 2073 7472 6964 696e 670a  v with striding.
+000122a0: 2020 2020 2320 6375 7374 6f6d 3a20 7265      # custom: re
+000122b0: 7065 6174 2c20 7265 6d6f 7665 2c20 6d61  peat, remove, ma
+000122c0: 736b 2c20 6c6f 6f70 2077 6974 6820 6479  sk, loop with dy
+000122d0: 6e20 656e 640a 2020 2020 2320 4e6f 7465  n end.    # Note
+000122e0: 2074 6861 7420 7765 2064 6966 6665 7265   that we differe
+000122f0: 6e74 6961 7465 2062 6574 7765 656e 2074  ntiate between t
+00012300: 6865 206f 7264 6572 2c20 692e 652e 2061  he order, i.e. a
+00012310: 202b 2062 2021 3d20 6220 2b20 612e 0a20   + b != b + a.. 
+00012320: 2020 2023 204e 6f74 6520 7468 6174 2077     # Note that w
+00012330: 6520 616c 7761 7973 2068 6176 6520 7468  e always have th
+00012340: 6520 6173 7375 6d70 7469 6f6e 2074 6861  e assumption tha
+00012350: 7420 6120 6469 6d65 6e73 696f 6e20 6973  t a dimension is
+00012360: 206e 6f6e 2d6e 6567 6174 6976 652e 0a20   non-negative.. 
+00012370: 2020 2023 2054 6869 7320 6173 7375 6d70     # This assump
+00012380: 7469 6f6e 2069 7320 6e65 6365 7373 6172  tion is necessar
+00012390: 7920 666f 7220 736f 6d65 2073 696d 706c  y for some simpl
+000123a0: 6966 6963 6174 696f 6e73 2e0a 2020 2020  ifications..    
+000123b0: 2320 6874 7470 733a 2f2f 6769 7468 7562  # https://github
+000123c0: 2e63 6f6d 2f72 7774 682d 6936 2f72 6574  .com/rwth-i6/ret
+000123d0: 7572 6e6e 2f70 756c 6c2f 3835 330a 0a20  urnn/pull/853.. 
+000123e0: 2020 2064 6566 205f 5f61 6464 5f5f 2873     def __add__(s
+000123f0: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
+00012400: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012410: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00012420: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
+00012430: 2020 2020 3a72 6574 7572 6e3a 2073 656c      :return: sel
+00012440: 6620 2b20 6f74 6865 722e 206e 6f74 6520  f + other. note 
+00012450: 7468 6174 2074 6869 7320 6973 206e 6f74  that this is not
+00012460: 2063 6f6d 6d75 7461 7469 7665 2c20 692e   commutative, i.
+00012470: 652e 2064 6966 6665 7265 6e74 2066 726f  e. different fro
+00012480: 6d20 6f74 6865 7220 2b20 7365 6c66 2e0a  m other + self..
+00012490: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000124a0: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
+000124b0: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
+000124c0: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
+000124d0: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
+000124e0: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
+000124f0: 6164 645f 7375 625f 286f 7468 6572 2c20  add_sub_(other, 
+00012500: 6b69 6e64 3d22 6164 6422 2c20 7269 6768  kind="add", righ
+00012510: 743d 5472 7565 290a 2020 2020 2020 2020  t=True).        
+00012520: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
+00012530: 696d 2829 0a0a 2020 2020 6465 6620 5f5f  im()..    def __
+00012540: 7261 6464 5f5f 2873 656c 663a 2044 696d  radd__(self: Dim
+00012550: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+00012560: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00012570: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
+00012580: 6572 3a0a 2020 2020 2020 2020 3a72 6574  er:.        :ret
+00012590: 7572 6e3a 206f 7468 6572 202b 2073 656c  urn: other + sel
+000125a0: 660a 2020 2020 2020 2020 3a72 7479 7065  f.        :rtype
+000125b0: 3a20 4469 6d0a 2020 2020 2020 2020 2222  : Dim.        ""
+000125c0: 220a 2020 2020 2020 2020 7465 726d 203d  ".        term =
+000125d0: 205f 4f70 4c69 6e65 6172 5465 726d 2e66   _OpLinearTerm.f
+000125e0: 726f 6d5f 6469 6d28 7365 6c66 290a 2020  rom_dim(self).  
+000125f0: 2020 2020 2020 7465 726d 2e65 7874 656e        term.exten
+00012600: 645f 6164 645f 7375 625f 286f 7468 6572  d_add_sub_(other
+00012610: 2c20 6b69 6e64 3d22 6164 6422 2c20 7269  , kind="add", ri
+00012620: 6768 743d 4661 6c73 6529 0a20 2020 2020  ght=False).     
+00012630: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
+00012640: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
+00012650: 205f 5f73 7562 5f5f 2873 656c 662c 206f   __sub__(self, o
+00012660: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012670: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012680: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00012690: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000126a0: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+000126b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000126c0: 7365 6c66 2e73 7562 5f72 6967 6874 286f  self.sub_right(o
+000126d0: 7468 6572 290a 0a20 2020 2064 6566 2073  ther)..    def s
+000126e0: 7562 5f72 6967 6874 2873 656c 663a 2044  ub_right(self: D
+000126f0: 696d 2c20 6f74 6865 7229 3a0a 2020 2020  im, other):.    
+00012700: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012710: 3a70 6172 616d 2044 696d 7c69 6e74 206f  :param Dim|int o
+00012720: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
+00012730: 6574 7572 6e3a 2073 656c 6620 2d20 6f74  eturn: self - ot
+00012740: 6865 720a 2020 2020 2020 2020 3a72 7479  her.        :rty
+00012750: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
+00012760: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
+00012770: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
+00012780: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
+00012790: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
+000127a0: 656e 645f 6164 645f 7375 625f 286f 7468  end_add_sub_(oth
+000127b0: 6572 2c20 6b69 6e64 3d22 7375 6222 2c20  er, kind="sub", 
+000127c0: 7269 6768 743d 5472 7565 290a 2020 2020  right=True).    
+000127d0: 2020 2020 7265 7475 726e 2074 6572 6d2e      return term.
+000127e0: 6173 5f64 696d 2829 0a0a 2020 2020 6465  as_dim()..    de
+000127f0: 6620 7375 625f 6c65 6674 2873 656c 663a  f sub_left(self:
+00012800: 2044 696d 2c20 6f74 6865 7229 3a0a 2020   Dim, other):.  
+00012810: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012820: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
+00012830: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+00012840: 3a72 6574 7572 6e3a 2028 2d6f 7468 6572  :return: (-other
+00012850: 2920 2b20 7365 6c66 0a20 2020 2020 2020  ) + self.       
+00012860: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
 00012870: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012880: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012890: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-000128a0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-000128b0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-000128c0: 6574 7572 6e20 7365 6c66 2e73 7562 5f72  eturn self.sub_r
-000128d0: 6967 6874 286f 7468 6572 290a 0a20 2020  ight(other)..   
-000128e0: 2064 6566 2073 7562 5f72 6967 6874 2873   def sub_right(s
-000128f0: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
-00012900: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012910: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00012920: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
-00012930: 2020 2020 3a72 6574 7572 6e3a 2073 656c      :return: sel
-00012940: 6620 2d20 6f74 6865 720a 2020 2020 2020  f - other.      
-00012950: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
-00012960: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012970: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
-00012980: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
-00012990: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
-000129a0: 726d 2e65 7874 656e 645f 6164 645f 7375  rm.extend_add_su
-000129b0: 625f 286f 7468 6572 2c20 6b69 6e64 3d22  b_(other, kind="
-000129c0: 7375 6222 2c20 7269 6768 743d 5472 7565  sub", right=True
-000129d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000129e0: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
-000129f0: 2020 2020 6465 6620 7375 625f 6c65 6674      def sub_left
-00012a00: 2873 656c 663a 2044 696d 2c20 6f74 6865  (self: Dim, othe
-00012a10: 7229 3a0a 2020 2020 2020 2020 2222 220a  r):.        """.
-00012a20: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-00012a30: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
-00012a40: 2020 2020 2020 3a72 6574 7572 6e3a 2028        :return: (
-00012a50: 2d6f 7468 6572 2920 2b20 7365 6c66 0a20  -other) + self. 
-00012a60: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00012a70: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-00012a80: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-00012a90: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-00012aa0: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00012ab0: 2020 2074 6572 6d2e 6578 7465 6e64 5f61     term.extend_a
-00012ac0: 6464 5f73 7562 5f28 6f74 6865 722c 206b  dd_sub_(other, k
-00012ad0: 696e 643d 2273 7562 222c 2072 6967 6874  ind="sub", right
-00012ae0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00012af0: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
-00012b00: 696d 2829 0a0a 2020 2020 6465 6620 5f5f  im()..    def __
-00012b10: 6d75 6c5f 5f28 7365 6c66 3a20 4469 6d2c  mul__(self: Dim,
-00012b20: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00012b30: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00012b40: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00012b50: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-00012b60: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-00012b70: 2222 0a20 2020 2020 2020 2074 6572 6d20  "".        term 
-00012b80: 3d20 5f4f 704c 696e 6561 7254 6572 6d2e  = _OpLinearTerm.
-00012b90: 6672 6f6d 5f64 696d 2873 656c 6629 0a20  from_dim(self). 
-00012ba0: 2020 2020 2020 2074 6572 6d2e 6578 7465         term.exte
-00012bb0: 6e64 5f6d 756c 5f64 6976 5f28 6f74 6865  nd_mul_div_(othe
-00012bc0: 722c 206b 696e 643d 226d 756c 222c 2072  r, kind="mul", r
-00012bd0: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
-00012be0: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
-00012bf0: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
-00012c00: 205f 5f72 6d75 6c5f 5f28 7365 6c66 3a20   __rmul__(self: 
-00012c10: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
-00012c20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012c30: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012c40: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00012c50: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00012c60: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-00012c70: 6572 6d20 3d20 5f4f 704c 696e 6561 7254  erm = _OpLinearT
-00012c80: 6572 6d2e 6672 6f6d 5f64 696d 2873 656c  erm.from_dim(sel
-00012c90: 6629 0a20 2020 2020 2020 2074 6572 6d2e  f).        term.
-00012ca0: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
-00012cb0: 6f74 6865 722c 206b 696e 643d 226d 756c  other, kind="mul
-00012cc0: 222c 2072 6967 6874 3d46 616c 7365 290a  ", right=False).
-00012cd0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00012ce0: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
-00012cf0: 2020 6465 6620 5f5f 666c 6f6f 7264 6976    def __floordiv
-00012d00: 5f5f 2873 656c 663a 2044 696d 2c20 6f74  __(self: Dim, ot
-00012d10: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
-00012d20: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00012d30: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
-00012d40: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00012d50: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00012d60: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
-00012d70: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
-00012d80: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
-00012d90: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
-00012da0: 6d75 6c5f 6469 765f 286f 7468 6572 2c20  mul_div_(other, 
-00012db0: 6b69 6e64 3d22 666c 6f6f 7264 6976 222c  kind="floordiv",
-00012dc0: 2072 6967 6874 3d54 7275 6529 0a20 2020   right=True).   
-00012dd0: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
-00012de0: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
-00012df0: 6566 205f 5f74 7275 6564 6976 5f5f 2873  ef __truediv__(s
-00012e00: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-00012e10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012e20: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012e30: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00012e40: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00012e50: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00012e60: 6574 7572 6e20 7365 6c66 2e64 6976 5f72  eturn self.div_r
-00012e70: 6967 6874 286f 7468 6572 290a 0a20 2020  ight(other)..   
-00012e80: 2064 6566 2064 6976 5f6c 6566 7428 7365   def div_left(se
-00012e90: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
-00012ea0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012eb0: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
-00012ec0: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
-00012ed0: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-00012ee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012ef0: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
-00012f00: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
-00012f10: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
-00012f20: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
-00012f30: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
-00012f40: 2274 7275 6564 6976 222c 2072 6967 6874  "truediv", right
-00012f50: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00012f60: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
-00012f70: 696d 2829 0a0a 2020 2020 6465 6620 6469  im()..    def di
-00012f80: 765f 7269 6768 7428 7365 6c66 3a20 4469  v_right(self: Di
-00012f90: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
-00012fa0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00012fb0: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
-00012fc0: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
-00012fd0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
-00012fe0: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
-00012ff0: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
-00013000: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
-00013010: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
-00013020: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
-00013030: 6865 722c 206b 696e 643d 2274 7275 6564  her, kind="trued
-00013040: 6976 222c 2072 6967 6874 3d54 7275 6529  iv", right=True)
-00013050: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013060: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
-00013070: 2020 2064 6566 2063 6569 6c64 6976 5f6c     def ceildiv_l
-00013080: 6566 7428 7365 6c66 3a20 4469 6d2c 206f  eft(self: Dim, o
-00013090: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
-000130a0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-000130b0: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
-000130c0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-000130d0: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
-000130e0: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
-000130f0: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
-00013100: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
-00013110: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
-00013120: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
-00013130: 206b 696e 643d 2263 6569 6c64 6976 222c   kind="ceildiv",
-00013140: 2072 6967 6874 3d46 616c 7365 290a 2020   right=False).  
-00013150: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00013160: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
-00013170: 6465 6620 6365 696c 6469 765f 7269 6768  def ceildiv_righ
-00013180: 7428 7365 6c66 3a20 4469 6d2c 206f 7468  t(self: Dim, oth
-00013190: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
-000131a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000131b0: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-000131c0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-000131d0: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-000131e0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-000131f0: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-00013200: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00013210: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
-00013220: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
-00013230: 696e 643d 2263 6569 6c64 6976 222c 2072  ind="ceildiv", r
-00013240: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
-00013250: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
-00013260: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
-00013270: 205f 5f6e 6567 5f5f 2873 656c 6629 3a0a   __neg__(self):.
-00013280: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013290: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-000132a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000132b0: 2020 2020 7265 7475 726e 202d 3120 2a20      return -1 * 
-000132c0: 7365 6c66 0a0a 2020 2020 6465 6620 6973  self..    def is
-000132d0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-000132e0: 5f64 696d 2873 656c 6629 202d 3e20 626f  _dim(self) -> bo
-000132f0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-00013300: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00013310: 2064 6572 6976 6564 206f 7020 6f66 2074   derived op of t
-00013320: 7970 6520 636f 6e73 7461 6e74 0a20 2020  ype constant.   
-00013330: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013340: 2072 6574 7572 6e20 7365 6c66 2e64 6572   return self.der
-00013350: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
-00013360: 2073 656c 662e 6465 7269 7665 645f 6672   self.derived_fr
-00013370: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2263  om_op.kind == "c
-00013380: 6f6e 7374 616e 7422 0a0a 0a64 6566 205f  onstant"...def _
-00013390: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
-000133a0: 6174 6963 5f64 696d 2876 616c 7565 2c20  atic_dim(value, 
-000133b0: 6b69 6e64 3d4e 6f6e 6529 3a0a 2020 2020  kind=None):.    
-000133c0: 2222 220a 2020 2020 3a70 6172 616d 2069  """.    :param i
-000133d0: 6e74 2076 616c 7565 3a0a 2020 2020 3a70  nt value:.    :p
-000133e0: 6172 616d 2045 6e74 6974 797c 4e6f 6e65  aram Entity|None
-000133f0: 206b 696e 643a 0a20 2020 203a 7274 7970   kind:.    :rtyp
-00013400: 653a 2044 696d 0a20 2020 2022 2222 0a20  e: Dim.    """. 
-00013410: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
-00013420: 280a 2020 2020 2020 2020 6469 6d65 6e73  (.        dimens
-00013430: 696f 6e3d 7661 6c75 652c 0a20 2020 2020  ion=value,.     
-00013440: 2020 206b 696e 643d 6b69 6e64 206f 7220     kind=kind or 
-00013450: 4469 6d54 7970 6573 2e55 6e73 7065 6369  DimTypes.Unspeci
-00013460: 6669 6564 2c0a 2020 2020 2020 2020 6465  fied,.        de
-00013470: 7363 7269 7074 696f 6e3d 2275 6e6e 616d  scription="unnam
-00013480: 6564 5f25 7364 696d 5f25 6922 2025 2028  ed_%sdim_%i" % (
-00013490: 6b69 6e64 2e6e 616d 6520 2b20 225f 2220  kind.name + "_" 
-000134a0: 6966 206b 696e 6420 656c 7365 2022 222c  if kind else "",
-000134b0: 2076 616c 7565 292c 0a20 2020 2020 2020   value),.       
-000134c0: 2064 6572 6976 6564 5f66 726f 6d5f 6f70   derived_from_op
-000134d0: 3d4f 7028 6b69 6e64 3d22 636f 6e73 7461  =Op(kind="consta
-000134e0: 6e74 222c 2069 6e70 7574 733d 5b5d 2c20  nt", inputs=[], 
-000134f0: 6174 7472 6962 733d 7b22 7661 6c75 6522  attribs={"value"
-00013500: 3a20 7661 6c75 657d 292c 0a20 2020 2020  : value}),.     
-00013510: 2020 2061 7574 6f5f 6765 6e65 7261 7465     auto_generate
-00013520: 643d 5472 7565 2c0a 2020 2020 290a 0a0a  d=True,.    )...
-00013530: 636c 6173 7320 4f70 3a0a 2020 2020 2222  class Op:.    ""
-00013540: 220a 2020 2020 4f70 206f 6e20 3a63 6c61  ".    Op on :cla
-00013550: 7373 3a60 4469 6d60 2077 6869 6368 2072  ss:`Dim` which r
-00013560: 6573 756c 7473 2069 6e20 6120 6465 7269  esults in a deri
-00013570: 7665 6420 3a63 6c61 7373 3a60 4469 6d60  ved :class:`Dim`
-00013580: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00013590: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000135a0: 2c20 6b69 6e64 2c20 696e 7075 7473 2c20  , kind, inputs, 
-000135b0: 6174 7472 6962 733d 4e6f 6e65 293a 0a20  attribs=None):. 
-000135c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000135d0: 2020 203a 7061 7261 6d20 7374 7220 6b69     :param str ki
-000135e0: 6e64 3a20 2261 6464 222c 2022 7375 6222  nd: "add", "sub"
-000135f0: 2c20 226d 756c 222c 2022 6365 696c 6469  , "mul", "ceildi
-00013600: 7622 0a20 2020 2020 2020 203a 7061 7261  v".        :para
-00013610: 6d20 6c69 7374 5b44 696d 5d20 696e 7075  m list[Dim] inpu
-00013620: 7473 3a0a 2020 2020 2020 2020 3a70 6172  ts:.        :par
-00013630: 616d 2064 6963 745b 7374 725d 7c4e 6f6e  am dict[str]|Non
-00013640: 6520 6174 7472 6962 733a 0a20 2020 2020  e attribs:.     
-00013650: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00013660: 656c 662e 6b69 6e64 203d 206b 696e 640a  elf.kind = kind.
-00013670: 2020 2020 2020 2020 7365 6c66 2e69 6e70          self.inp
-00013680: 7574 7320 3d20 696e 7075 7473 0a20 2020  uts = inputs.   
-00013690: 2020 2020 2073 656c 662e 6f75 7470 7574       self.output
-000136a0: 203d 204e 6f6e 6520 2023 2074 7970 653a   = None  # type:
-000136b0: 204f 7074 696f 6e61 6c5b 5f64 2e44 696d   Optional[_d.Dim
-000136c0: 5d0a 2020 2020 2020 2020 7365 6c66 2e61  ].        self.a
-000136d0: 7474 7269 6273 203d 2061 7474 7269 6273  ttribs = attribs
-000136e0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
-000136f0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00013700: 2020 6174 7472 6962 7320 3d20 2822 2025    attribs = (" %
-00013710: 7222 2025 2073 656c 662e 6174 7472 6962  r" % self.attrib
-00013720: 7329 2069 6620 7365 6c66 2e61 7474 7269  s) if self.attri
-00013730: 6273 2065 6c73 6520 2222 0a20 2020 2020  bs else "".     
-00013740: 2020 2072 6574 7572 6e20 223c 4469 6d2e     return "<Dim.
-00013750: 4f70 2025 7220 2573 2573 3e22 2025 2028  Op %r %s%s>" % (
-00013760: 7365 6c66 2e6b 696e 642c 2073 656c 662e  self.kind, self.
-00013770: 696e 7075 7473 2c20 6174 7472 6962 7329  inputs, attribs)
-00013780: 0a0a 2020 2020 6465 6620 5f76 616c 7565  ..    def _value
-00013790: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000137a0: 7265 7475 726e 2073 656c 662e 6b69 6e64  return self.kind
-000137b0: 2c20 7475 706c 6528 7365 6c66 2e69 6e70  , tuple(self.inp
-000137c0: 7574 7329 2c20 6672 6f7a 656e 7365 7428  uts), frozenset(
-000137d0: 7365 6c66 2e61 7474 7269 6273 2e69 7465  self.attribs.ite
-000137e0: 6d73 2829 2920 6966 2073 656c 662e 6174  ms()) if self.at
-000137f0: 7472 6962 7320 656c 7365 204e 6f6e 650a  tribs else None.
-00013800: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
-00013810: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00013820: 2072 6574 7572 6e20 6861 7368 2873 656c   return hash(sel
-00013830: 662e 5f76 616c 7565 2829 290a 0a20 2020  f._value())..   
-00013840: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
-00013850: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00013860: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013870: 6f74 6865 722c 204f 7029 3a0a 2020 2020  other, Op):.    
-00013880: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00013890: 656c 662e 5f76 616c 7565 2829 203d 3d20  elf._value() == 
-000138a0: 6f74 6865 722e 5f76 616c 7565 2829 0a20  other._value(). 
-000138b0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000138c0: 6c73 650a 0a20 2020 2064 6566 205f 5f6e  lse..    def __n
-000138d0: 655f 5f28 7365 6c66 2c20 6f74 6865 7229  e__(self, other)
-000138e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000138f0: 206e 6f74 2073 656c 662e 5f5f 6571 5f5f   not self.__eq__
-00013900: 286f 7468 6572 290a 0a0a 6465 6620 5f67  (other)...def _g
-00013910: 6574 5f64 6573 6372 6970 7469 6f6e 2864  et_description(d
-00013920: 696d 2c20 6272 6163 6b65 7473 3d54 7275  im, brackets=Tru
-00013930: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-00013940: 3a70 6172 616d 2044 696d 2064 696d 3a0a  :param Dim dim:.
-00013950: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00013960: 6272 6163 6b65 7473 3a20 6164 6420 6272  brackets: add br
-00013970: 6163 6b65 7473 2077 6865 6e20 6e65 6365  ackets when nece
-00013980: 7373 6172 790a 2020 2020 3a72 7479 7065  ssary.    :rtype
-00013990: 3a20 7374 720a 2020 2020 2222 220a 2020  : str.    """.  
-000139a0: 2020 6966 2064 696d 2e64 6573 6372 6970    if dim.descrip
-000139b0: 7469 6f6e 2061 6e64 2064 696d 2e64 6573  tion and dim.des
-000139c0: 6372 6970 7469 6f6e 2e73 7461 7274 7377  cription.startsw
-000139d0: 6974 6828 2275 6e6e 616d 6564 5f22 2920  ith("unnamed_") 
-000139e0: 616e 6420 6469 6d2e 6469 6d65 6e73 696f  and dim.dimensio
-000139f0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00013a00: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00013a10: 7228 6469 6d2e 6469 6d65 6e73 696f 6e29  r(dim.dimension)
-00013a20: 0a20 2020 2069 6620 6469 6d2e 6465 7363  .    if dim.desc
-00013a30: 7269 7074 696f 6e3a 0a20 2020 2020 2020  ription:.       
-00013a40: 2069 6620 6272 6163 6b65 7473 3a0a 2020   if brackets:.  
-00013a50: 2020 2020 2020 2020 2020 696d 706f 7274            import
-00013a60: 2072 650a 0a20 2020 2020 2020 2020 2020   re..           
-00013a70: 2069 6620 7265 2e73 6561 7263 6828 225b   if re.search("[
-00013a80: 2b5c 5c2d 2f20 5d22 2c20 6469 6d2e 6465  +\\-/ ]", dim.de
-00013a90: 7363 7269 7074 696f 6e29 3a0a 2020 2020  scription):.    
-00013aa0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00013ab0: 726e 2022 2825 7329 2220 2520 6469 6d2e  rn "(%s)" % dim.
-00013ac0: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
-00013ad0: 2020 2020 7265 7475 726e 2064 696d 2e64      return dim.d
-00013ae0: 6573 6372 6970 7469 6f6e 0a20 2020 2072  escription.    r
-00013af0: 6574 7572 6e20 2275 6e6e 616d 6564 5f25  eturn "unnamed_%
-00013b00: 735f 6469 6d25 7322 2025 2028 6469 6d2e  s_dim%s" % (dim.
-00013b10: 6b69 6e64 2c20 6469 6d2e 6469 6d65 6e73  kind, dim.dimens
-00013b20: 696f 6e20 6966 2064 696d 2e64 696d 656e  ion if dim.dimen
-00013b30: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
-00013b40: 2065 6c73 6520 223f 2229 0a0a 0a63 6c61   else "?")...cla
-00013b50: 7373 205f 4f70 4d75 6c74 5465 726d 3a0a  ss _OpMultTerm:.
-00013b60: 2020 2020 2222 220a 2020 2020 7265 7072      """.    repr
-00013b70: 6573 656e 7473 2073 7468 206c 696b 6520  esents sth like 
-00013b80: 6120 2a20 6220 2a20 630a 2020 2020 2222  a * b * c.    ""
-00013b90: 220a 0a20 2020 2040 636c 6173 736d 6574  "..    @classmet
-00013ba0: 686f 640a 2020 2020 6465 6620 6672 6f6d  hod.    def from
-00013bb0: 5f64 696d 2863 6c73 2c20 6469 6d3a 205f  _dim(cls, dim: _
-00013bc0: 642e 4469 6d29 202d 3e20 5f4f 704d 756c  d.Dim) -> _OpMul
-00013bd0: 7454 6572 6d3a 0a20 2020 2020 2020 2022  tTerm:.        "
-00013be0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00013bf0: 6d20 6469 6d3a 0a20 2020 2020 2020 203a  m dim:.        :
-00013c00: 7265 7475 726e 3a20 6f70 206d 756c 7420  return: op mult 
-00013c10: 7465 726d 0a20 2020 2020 2020 2022 2222  term.        """
-00013c20: 0a20 2020 2020 2020 2064 696d 203d 2064  .        dim = d
-00013c30: 696d 2e67 6574 5f73 616d 655f 6261 7365  im.get_same_base
-00013c40: 2829 0a20 2020 2020 2020 2069 6620 6469  ().        if di
-00013c50: 6d2e 6469 6d65 6e73 696f 6e20 3d3d 2031  m.dimension == 1
-00013c60: 2061 6e64 2064 696d 2e69 735f 636f 6e73   and dim.is_cons
-00013c70: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-00013c80: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00013c90: 6574 7572 6e20 636c 732e 6f6e 6528 290a  eturn cls.one().
-00013ca0: 2020 2020 2020 2020 6966 2064 696d 2e64          if dim.d
-00013cb0: 6572 6976 6564 5f66 726f 6d5f 6f70 2061  erived_from_op a
-00013cc0: 6e64 2064 696d 2e64 6572 6976 6564 5f66  nd dim.derived_f
-00013cd0: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-00013ce0: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
-00013cf0: 2020 7265 7475 726e 2063 6c73 286c 6973    return cls(lis
-00013d00: 7428 6469 6d2e 6465 7269 7665 645f 6672  t(dim.derived_fr
-00013d10: 6f6d 5f6f 702e 696e 7075 7473 2929 0a20  om_op.inputs)). 
-00013d20: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00013d30: 7328 5b64 696d 5d29 0a0a 2020 2020 4063  s([dim])..    @c
-00013d40: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00013d50: 6566 2066 726f 6d5f 6469 6d5f 6661 6374  ef from_dim_fact
-00013d60: 6f72 7328 636c 732c 2064 696d 7329 3a0a  ors(cls, dims):.
-00013d70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013d80: 2020 2020 3a70 6172 616d 206c 6973 745b      :param list[
-00013d90: 4469 6d5d 2064 696d 733a 0a20 2020 2020  Dim] dims:.     
-00013da0: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
-00013db0: 4f70 4d75 6c74 5465 726d 0a20 2020 2020  OpMultTerm.     
-00013dc0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00013dd0: 6573 203d 2063 6c73 2e6f 6e65 2829 0a20  es = cls.one(). 
-00013de0: 2020 2020 2020 2066 6f72 2064 2069 6e20         for d in 
-00013df0: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
-00013e00: 2020 7265 732e 6578 7465 6e64 5f6d 756c    res.extend_mul
-00013e10: 5f64 6976 5f28 642c 206b 696e 643d 226d  _div_(d, kind="m
-00013e20: 756c 222c 2072 6967 6874 3d54 7275 6529  ul", right=True)
-00013e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013e40: 7265 730a 0a20 2020 2040 636c 6173 736d  res..    @classm
-00013e50: 6574 686f 640a 2020 2020 6465 6620 6f6e  ethod.    def on
-00013e60: 6528 636c 7329 3a0a 2020 2020 2020 2020  e(cls):.        
-00013e70: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
-00013e80: 7065 3a20 4469 6d2e 5f4f 704d 756c 7454  pe: Dim._OpMultT
-00013e90: 6572 6d0a 2020 2020 2020 2020 2222 220a  erm.        """.
-00013ea0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00013eb0: 6c73 285b 5d29 0a0a 2020 2020 6465 6620  ls([])..    def 
-00013ec0: 5f5f 696e 6974 5f5f 2873 656c 662c 2074  __init__(self, t
-00013ed0: 6572 6d73 293a 0a20 2020 2020 2020 2022  erms):.        "
-00013ee0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00013ef0: 6d20 6c69 7374 5b44 696d 5d20 7465 726d  m list[Dim] term
-00013f00: 733a 0a20 2020 2020 2020 2022 2222 0a20  s:.        """. 
-00013f10: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
-00013f20: 7320 3d20 7465 726d 730a 0a20 2020 2064  s = terms..    d
-00013f30: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
-00013f40: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00013f50: 6e20 6861 7368 2874 7570 6c65 2873 656c  n hash(tuple(sel
-00013f60: 662e 7465 726d 7329 290a 0a20 2020 2064  f.terms))..    d
-00013f70: 6566 205f 5f65 715f 5f28 7365 6c66 2c20  ef __eq__(self, 
-00013f80: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00013f90: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-00013fa0: 616d 2044 696d 7c44 696d 2e5f 4f70 4d75  am Dim|Dim._OpMu
-00013fb0: 6c74 5465 726d 206f 7468 6572 3a0a 2020  ltTerm other:.  
-00013fc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013fd0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013fe0: 6f74 6865 722c 205f 4f70 4d75 6c74 5465  other, _OpMultTe
-00013ff0: 726d 293a 0a20 2020 2020 2020 2020 2020  rm):.           
-00014000: 2072 6574 7572 6e20 7365 6c66 2e74 6572   return self.ter
-00014010: 6d73 203d 3d20 6f74 6865 722e 7465 726d  ms == other.term
-00014020: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-00014030: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
-00014040: 5f5f 6e65 5f5f 2873 656c 662c 206f 7468  __ne__(self, oth
-00014050: 6572 293a 0a20 2020 2020 2020 2072 6574  er):.        ret
-00014060: 7572 6e20 6e6f 7420 7365 6c66 2e5f 5f65  urn not self.__e
-00014070: 715f 5f28 6f74 6865 7229 0a0a 2020 2020  q__(other)..    
-00014080: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
-00014090: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-000140a0: 726e 2022 4469 6d2e 5f4f 704d 756c 7454  rn "Dim._OpMultT
-000140b0: 6572 6d28 2572 2922 2025 2028 7365 6c66  erm(%r)" % (self
-000140c0: 2e74 6572 6d73 2c29 0a0a 2020 2020 4070  .terms,)..    @p
-000140d0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000140e0: 6469 6d65 6e73 696f 6e28 7365 6c66 293a  dimension(self):
-000140f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014100: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-00014110: 7c4e 6f6e 650a 2020 2020 2020 2020 2222  |None.        ""
-00014120: 220a 2020 2020 2020 2020 6469 6d20 3d20  ".        dim = 
-00014130: 310a 2020 2020 2020 2020 666f 7220 7061  1.        for pa
-00014140: 7274 2069 6e20 7365 6c66 2e74 6572 6d73  rt in self.terms
-00014150: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00014160: 2070 6172 742e 6469 6d65 6e73 696f 6e20   part.dimension 
-00014170: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00014180: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00014190: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-000141a0: 2064 696d 202a 3d20 7061 7274 2e64 696d   dim *= part.dim
-000141b0: 656e 7369 6f6e 0a20 2020 2020 2020 2072  ension.        r
-000141c0: 6574 7572 6e20 6469 6d0a 0a20 2020 2064  eturn dim..    d
-000141d0: 6566 2062 6173 655f 7465 726d 2873 656c  ef base_term(sel
-000141e0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000141f0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00014200: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00014210: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00014220: 656c 662e 7465 726d 730a 2020 2020 2020  elf.terms.      
-00014230: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
-00014240: 726d 735b 2d31 5d0a 0a20 2020 2064 6566  rms[-1]..    def
-00014250: 2069 735f 6f6e 6528 7365 6c66 293a 0a20   is_one(self):. 
-00014260: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014270: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-00014280: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014290: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
-000142a0: 656c 662e 7465 726d 730a 0a20 2020 2064  elf.terms..    d
-000142b0: 6566 2069 735f 636f 6e73 7461 6e74 5f73  ef is_constant_s
-000142c0: 7461 7469 635f 6469 6d28 7365 6c66 293a  tatic_dim(self):
-000142d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000142e0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-000142f0: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-00014300: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00014310: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
-00014320: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00014330: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014340: 616c 6c28 7465 726d 2e69 735f 636f 6e73  all(term.is_cons
-00014350: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-00014360: 2920 666f 7220 7465 726d 2069 6e20 7365  ) for term in se
-00014370: 6c66 2e74 6572 6d73 290a 0a20 2020 2064  lf.terms)..    d
-00014380: 6566 2063 6f70 7928 7365 6c66 293a 0a20  ef copy(self):. 
-00014390: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000143a0: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
-000143b0: 4f70 4d75 6c74 5465 726d 0a20 2020 2020  OpMultTerm.     
-000143c0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-000143d0: 6574 7572 6e20 5f4f 704d 756c 7454 6572  eturn _OpMultTer
-000143e0: 6d28 6c69 7374 2873 656c 662e 7465 726d  m(list(self.term
-000143f0: 7329 290a 0a20 2020 2064 6566 206e 6567  s))..    def neg
-00014400: 6174 6976 6528 7365 6c66 293a 0a20 2020  ative(self):.   
-00014410: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014420: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
-00014430: 4d75 6c74 5465 726d 0a20 2020 2020 2020  MultTerm.       
-00014440: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00014450: 7365 6c66 2e74 6572 6d73 2061 6e64 2073  self.terms and s
-00014460: 656c 662e 7465 726d 735b 305d 2e69 735f  elf.terms[0].is_
-00014470: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-00014480: 6469 6d28 2920 616e 6420 7365 6c66 2e74  dim() and self.t
-00014490: 6572 6d73 5b30 5d2e 6469 6d65 6e73 696f  erms[0].dimensio
-000144a0: 6e20 3d3d 202d 313a 0a20 2020 2020 2020  n == -1:.       
-000144b0: 2020 2020 2072 6574 7572 6e20 5f4f 704d       return _OpM
-000144c0: 756c 7454 6572 6d28 7365 6c66 2e74 6572  ultTerm(self.ter
-000144d0: 6d73 5b31 3a5d 290a 2020 2020 2020 2020  ms[1:]).        
-000144e0: 7265 7320 3d20 7365 6c66 2e63 6f70 7928  res = self.copy(
-000144f0: 290a 2020 2020 2020 2020 7265 732e 6578  ).        res.ex
-00014500: 7465 6e64 5f6d 756c 5f64 6976 5f28 5f6d  tend_mul_div_(_m
-00014510: 616b 655f 636f 6e73 7461 6e74 5f73 7461  ake_constant_sta
-00014520: 7469 635f 6469 6d28 2d31 292c 206b 696e  tic_dim(-1), kin
-00014530: 643d 226d 756c 222c 2072 6967 6874 3d46  d="mul", right=F
-00014540: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
-00014550: 7475 726e 2072 6573 0a0a 2020 2020 6465  turn res..    de
-00014560: 6620 6469 7669 7369 626c 6528 7365 6c66  f divisible(self
-00014570: 2c20 6f74 6865 722c 2072 6967 6874 293a  , other, right):
-00014580: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014590: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
-000145a0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-000145b0: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
-000145c0: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-000145d0: 6e3a 2077 6865 7468 6572 2077 6520 6361  n: whether we ca
-000145e0: 6e20 6469 7669 6465 206f 7468 6572 2c20  n divide other, 
-000145f0: 7769 7468 6f75 7420 7265 6d61 696e 6465  without remainde
-00014600: 720a 2020 2020 2020 2020 3a72 7479 7065  r.        :rtype
-00014610: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-00014620: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-00014630: 7420 7365 6c66 2e74 6572 6d73 3a0a 2020  t self.terms:.  
-00014640: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014650: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
-00014660: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
-00014670: 6672 6f6d 5f6f 7020 616e 6420 6f74 6865  from_op and othe
-00014680: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00014690: 702e 6b69 6e64 203d 3d20 226d 756c 223a  p.kind == "mul":
-000146a0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-000146b0: 203d 2073 656c 662e 636f 7079 2829 0a20   = self.copy(). 
-000146c0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-000146d0: 6572 6d20 696e 206f 7468 6572 2e64 6572  erm in other.der
-000146e0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-000146f0: 7574 7320 6966 2072 6967 6874 2065 6c73  uts if right els
-00014700: 6520 7265 7665 7273 6564 286f 7468 6572  e reversed(other
-00014710: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00014720: 2e69 6e70 7574 7329 3a0a 2020 2020 2020  .inputs):.      
-00014730: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00014740: 2074 6d70 2e64 6976 6973 6962 6c65 2874   tmp.divisible(t
-00014750: 6572 6d2c 2072 6967 6874 3d72 6967 6874  erm, right=right
-00014760: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014770: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00014780: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00014790: 2020 2020 746d 702e 6578 7465 6e64 5f6d      tmp.extend_m
-000147a0: 756c 5f64 6976 5f28 7465 726d 2c20 6b69  ul_div_(term, ki
-000147b0: 6e64 3d22 7472 7565 6469 7622 2c20 7269  nd="truediv", ri
-000147c0: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
-000147d0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000147e0: 7565 0a20 2020 2020 2020 206d 6f73 745f  ue.        most_
-000147f0: 7265 6365 6e74 5f74 6572 6d20 3d20 7365  recent_term = se
-00014800: 6c66 2e74 6572 6d73 5b2d 3120 6966 2072  lf.terms[-1 if r
-00014810: 6967 6874 2065 6c73 6520 305d 0a20 2020  ight else 0].   
-00014820: 2020 2020 2069 6620 6f74 6865 7220 3d3d       if other ==
-00014830: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
-00014840: 6d3a 0a20 2020 2020 2020 2020 2020 2072  m:.            r
-00014850: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00014860: 2020 2069 6620 6d6f 7374 5f72 6563 656e     if most_recen
-00014870: 745f 7465 726d 2e64 696d 656e 7369 6f6e  t_term.dimension
-00014880: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00014890: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
-000148a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000148b0: 2020 2020 2020 2020 2020 6966 206d 6f73            if mos
-000148c0: 745f 7265 6365 6e74 5f74 6572 6d2e 6469  t_recent_term.di
-000148d0: 6d65 6e73 696f 6e20 2520 6f74 6865 722e  mension % other.
-000148e0: 6469 6d65 6e73 696f 6e20 3d3d 2030 3a0a  dimension == 0:.
-000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014900: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00014910: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00014920: 0a0a 2020 2020 6465 6620 6361 6e5f 7369  ..    def can_si
-00014930: 6d70 6c69 6679 2873 656c 662c 206f 7468  mplify(self, oth
-00014940: 6572 2c20 6b69 6e64 2c20 7269 6768 7429  er, kind, right)
-00014950: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00014960: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00014970: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
-00014980: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
-00014990: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000149a0: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
-000149b0: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
-000149c0: 7468 6572 2077 6520 6361 6e20 7369 6d70  ther we can simp
-000149d0: 6c69 6679 2077 6865 6e20 6170 706c 7969  lify when applyi
-000149e0: 6e67 2074 6869 7320 6f70 6572 6174 696f  ng this operatio
-000149f0: 6e0a 2020 2020 2020 2020 3a72 7479 7065  n.        :rtype
-00014a00: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-00014a10: 2222 0a20 2020 2020 2020 2069 6620 6f74  "".        if ot
-00014a20: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
-00014a30: 5f6f 7020 616e 6420 6f74 6865 722e 6465  _op and other.de
-00014a40: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
-00014a50: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
-00014a60: 2020 2020 2020 2020 2074 6d70 203d 2073           tmp = s
-00014a70: 656c 662e 636f 7079 2829 0a20 2020 2020  elf.copy().     
-00014a80: 2020 2020 2020 2066 6f72 2074 6572 6d20         for term 
-00014a90: 696e 206f 7468 6572 2e64 6572 6976 6564  in other.derived
-00014aa0: 5f66 726f 6d5f 6f70 2e69 6e70 7574 7320  _from_op.inputs 
-00014ab0: 6966 2072 6967 6874 2065 6c73 6520 7265  if right else re
-00014ac0: 7665 7273 6564 286f 7468 6572 2e64 6572  versed(other.der
-00014ad0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-00014ae0: 7574 7329 3a0a 2020 2020 2020 2020 2020  uts):.          
-00014af0: 2020 2020 2020 6966 206e 6f74 2074 6d70        if not tmp
-00014b00: 2e63 616e 5f73 696d 706c 6966 7928 7465  .can_simplify(te
-00014b10: 726d 2c20 6b69 6e64 3d6b 696e 642c 2072  rm, kind=kind, r
-00014b20: 6967 6874 3d72 6967 6874 293a 0a20 2020  ight=right):.   
-00014b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b40: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00014b50: 2020 2020 2020 2020 2020 2020 2020 746d                tm
-00014b60: 702e 6578 7465 6e64 5f6d 756c 5f64 6976  p.extend_mul_div
-00014b70: 5f28 7465 726d 2c20 6b69 6e64 3d6b 696e  _(term, kind=kin
-00014b80: 642c 2072 6967 6874 3d72 6967 6874 290a  d, right=right).
-00014b90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014ba0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00014bb0: 6964 7820 3d20 7365 6c66 2e5f 7369 6d70  idx = self._simp
-00014bc0: 6c69 6679 5f74 6572 6d5f 6964 7828 6f74  lify_term_idx(ot
-00014bd0: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
-00014be0: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
-00014bf0: 2020 2020 2072 6574 7572 6e20 6964 7820       return idx 
-00014c00: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
-00014c10: 2064 6566 205f 7369 6d70 6c69 6679 5f74   def _simplify_t
-00014c20: 6572 6d5f 6964 7828 7365 6c66 2c20 6f74  erm_idx(self, ot
-00014c30: 6865 722c 206b 696e 642c 2072 6967 6874  her, kind, right
-00014c40: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00014c50: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
-00014c60: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
-00014c70: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
-00014c80: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-00014c90: 2062 6f6f 6c20 7269 6768 743a 0a20 2020   bool right:.   
-00014ca0: 2020 2020 203a 7265 7475 726e 3a20 696e       :return: in
-00014cb0: 6465 7820 6f66 2074 6572 6d20 746f 2073  dex of term to s
-00014cc0: 696d 706c 6966 790a 2020 2020 2020 2020  implify.        
-00014cd0: 3a72 7479 7065 3a20 696e 747c 4e6f 6e65  :rtype: int|None
-00014ce0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014cf0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00014d00: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00014d10: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00014d20: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
-00014d30: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
-00014d40: 2020 2020 2020 2320 5765 2077 616e 7420        # We want 
-00014d50: 2862 202a 2061 2920 2f2f 2062 2021 3d20  (b * a) // b != 
-00014d60: 612e 0a20 2020 2020 2020 2020 2020 2023  a..            #
-00014d70: 2048 6f77 6576 6572 2c20 7765 2077 616e   However, we wan
-00014d80: 7420 6820 2a20 2832 202a 2061 202f 2f20  t h * (2 * a // 
-00014d90: 6829 203d 3d20 3220 2a20 612e 0a20 2020  h) == 2 * a..   
-00014da0: 2020 2020 2020 2020 2023 2053 6f2c 2066           # So, f
-00014db0: 6f72 2060 6d75 6c60 2c20 616e 6420 6f6e  or `mul`, and on
-00014dc0: 6c79 2066 6f72 2060 6d75 6c60 2c20 6368  ly for `mul`, ch
-00014dd0: 6563 6b20 616c 6c20 7465 726d 732c 2077  eck all terms, w
-00014de0: 6865 7468 6572 2077 6520 6361 6e20 7369  hether we can si
-00014df0: 6d70 6c69 6679 2073 6f6d 6520 6469 7669  mplify some divi
-00014e00: 7369 6f6e 2d74 6572 6d2e 0a20 2020 2020  sion-term..     
-00014e10: 2020 2020 2020 2066 6f72 2069 2c20 7465         for i, te
-00014e20: 726d 2069 6e20 7265 7665 7273 6564 286c  rm in reversed(l
-00014e30: 6973 7428 656e 756d 6572 6174 6528 7365  ist(enumerate(se
-00014e40: 6c66 2e74 6572 6d73 2929 2920 6966 2072  lf.terms))) if r
-00014e50: 6967 6874 2065 6c73 6520 656e 756d 6572  ight else enumer
-00014e60: 6174 6528 7365 6c66 2e74 6572 6d73 293a  ate(self.terms):
-00014e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014e80: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-00014e90: 6365 2874 6572 6d2c 205f 642e 4469 6d29  ce(term, _d.Dim)
-00014ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014eb0: 2069 6620 7465 726d 2e64 6572 6976 6564   if term.derived
-00014ec0: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
-00014ed0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014ee0: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
-00014ef0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
-00014f00: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
-00014f10: 6874 2220 6966 2072 6967 6874 2065 6c73  ht" if right els
-00014f20: 6520 226c 6566 7422 293a 0a20 2020 2020  e "left"):.     
-00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f40: 2020 2069 6620 7465 726d 2e64 6572 6976     if term.deriv
-00014f50: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
-00014f60: 735b 2d31 5d20 3d3d 206f 7468 6572 3a0a  s[-1] == other:.
-00014f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014f90: 726e 2069 0a20 2020 2020 2020 2020 2020  rn i.           
-00014fa0: 2020 2020 2069 6620 6f74 6865 722e 6465       if other.de
-00014fb0: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-00014fe0: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
-00014ff0: 203d 3d20 2274 7275 6564 6976 5f22 202b   == "truediv_" +
-00015000: 2028 2272 6967 6874 2220 6966 206e 6f74   ("right" if not
-00015010: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
-00015020: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
-00015030: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015040: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00015050: 6f6d 5f6f 702e 696e 7075 7473 5b2d 315d  om_op.inputs[-1]
-00015060: 203d 3d20 7465 726d 3a0a 2020 2020 2020   == term:.      
-00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015080: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
-00015090: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000150a0: 6620 7465 726d 2e69 735f 636f 6e73 7461  f term.is_consta
-000150b0: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
-000150c0: 616e 6420 6f74 6865 722e 6973 5f63 6f6e  and other.is_con
-000150d0: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-000150e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000150f0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00015100: 0a20 2020 2020 2020 2023 2046 6f72 2074  .        # For t
-00015110: 6865 206c 6173 742f 6669 7273 7420 7465  he last/first te
-00015120: 726d 2c20 6578 7472 6120 6368 6563 6b73  rm, extra checks
-00015130: 2e0a 2020 2020 2020 2020 6920 3d20 6c65  ..        i = le
-00015140: 6e28 7365 6c66 2e74 6572 6d73 2920 2d20  n(self.terms) - 
-00015150: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
-00015160: 300a 2020 2020 2020 2020 7465 726d 203d  0.        term =
-00015170: 2073 656c 662e 7465 726d 735b 695d 0a20   self.terms[i]. 
-00015180: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-00015190: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
-000151a0: 6e64 206f 7468 6572 203d 3d20 7465 726d  nd other == term
-000151b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000151c0: 7475 726e 2069 0a20 2020 2020 2020 206f  turn i.        o
-000151d0: 705f 6b69 6e64 203d 206b 696e 6420 2b20  p_kind = kind + 
-000151e0: 225f 2220 2b20 2822 7269 6768 7422 2069  "_" + ("right" i
-000151f0: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
-00015200: 6674 2229 0a20 2020 2020 2020 2069 6620  ft").        if 
-00015210: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
-00015220: 6d5f 6f70 2061 6e64 2074 6572 6d2e 6465  m_op and term.de
-00015230: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
-00015240: 6e64 203d 3d20 6f70 5f6b 696e 643a 0a20  nd == op_kind:. 
-00015250: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015260: 6e20 690a 2020 2020 2020 2020 7265 7475  n i.        retu
-00015270: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
-00015280: 2065 7874 656e 645f 6d75 6c5f 6469 765f   extend_mul_div_
-00015290: 2873 656c 662c 206f 7468 6572 2c20 6b69  (self, other, ki
-000152a0: 6e64 2c20 7269 6768 7429 3a0a 2020 2020  nd, right):.    
-000152b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000152c0: 3a70 6172 616d 2044 696d 206f 7468 6572  :param Dim other
-000152d0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-000152e0: 2073 7472 206b 696e 643a 0a20 2020 2020   str kind:.     
-000152f0: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
-00015300: 6967 6874 3a0a 2020 2020 2020 2020 2222  ight:.        ""
-00015310: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00015320: 206b 696e 6420 696e 207b 226d 756c 222c   kind in {"mul",
-00015330: 2022 666c 6f6f 7264 6976 222c 2022 7472   "floordiv", "tr
-00015340: 7565 6469 7622 2c20 2263 6569 6c64 6976  uediv", "ceildiv
-00015350: 227d 0a20 2020 2020 2020 2069 6620 6f74  "}.        if ot
-00015360: 6865 722e 6973 5f63 6f6e 7374 616e 745f  her.is_constant_
-00015370: 7374 6174 6963 5f64 696d 2829 2061 6e64  static_dim() and
-00015380: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
-00015390: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-000153a0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000153b0: 2020 6966 206e 6f74 2073 656c 662e 7465    if not self.te
-000153c0: 726d 733a 0a20 2020 2020 2020 2020 2020  rms:.           
-000153d0: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
-000153e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-000153f0: 2020 2073 656c 662e 7465 726d 732e 6170     self.terms.ap
-00015400: 7065 6e64 286f 7468 6572 290a 2020 2020  pend(other).    
-00015410: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-00015420: 642e 656e 6473 7769 7468 2822 6469 7622  d.endswith("div"
-00015430: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00015440: 2020 2073 656c 662e 7465 726d 7320 3d20     self.terms = 
-00015450: 5b5f 4f70 4d75 6c74 5465 726d 2e6e 6577  [_OpMultTerm.new
-00015460: 5f64 6976 5f64 696d 2873 656c 662e 6173  _div_dim(self.as
-00015470: 5f64 696d 2829 2c20 6f74 6865 722c 206b  _dim(), other, k
-00015480: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
-00015490: 7269 6768 7429 5d0a 2020 2020 2020 2020  right)].        
-000154a0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000154b0: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-000154c0: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
-000154d0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-000154e0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 226d  om_op.kind == "m
-000154f0: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
-00015500: 2066 6f72 2074 6572 6d20 696e 206f 7468   for term in oth
-00015510: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
-00015520: 6f70 2e69 6e70 7574 7320 6966 2072 6967  op.inputs if rig
-00015530: 6874 2065 6c73 6520 7265 7665 7273 6564  ht else reversed
-00015540: 286f 7468 6572 2e64 6572 6976 6564 5f66  (other.derived_f
-00015550: 726f 6d5f 6f70 2e69 6e70 7574 7329 3a0a  rom_op.inputs):.
-00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015570: 7365 6c66 2e65 7874 656e 645f 6d75 6c5f  self.extend_mul_
-00015580: 6469 765f 2874 6572 6d2c 206b 696e 643d  div_(term, kind=
-00015590: 6b69 6e64 2c20 7269 6768 743d 7269 6768  kind, right=righ
-000155a0: 7429 0a20 2020 2020 2020 2020 2020 2072  t).            r
-000155b0: 6574 7572 6e0a 2020 2020 2020 2020 6964  eturn.        id
-000155c0: 7820 3d20 7365 6c66 2e5f 7369 6d70 6c69  x = self._simpli
-000155d0: 6679 5f74 6572 6d5f 6964 7828 6f74 6865  fy_term_idx(othe
-000155e0: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
-000155f0: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
-00015600: 2020 2069 6620 6964 7820 6973 206e 6f74     if idx is not
-00015610: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00015620: 2020 2074 6572 6d20 3d20 7365 6c66 2e74     term = self.t
-00015630: 6572 6d73 5b69 6478 5d0a 2020 2020 2020  erms[idx].      
-00015640: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-00015650: 6e73 7461 6e63 6528 7465 726d 2c20 5f64  nstance(term, _d
-00015660: 2e44 696d 290a 2020 2020 2020 2020 2020  .Dim).          
-00015670: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
-00015680: 7468 2822 6469 7622 2920 616e 6420 6f74  th("div") and ot
-00015690: 6865 7220 3d3d 2074 6572 6d3a 0a20 2020  her == term:.   
-000156a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000156b0: 662e 7465 726d 732e 706f 7028 6964 7829  f.terms.pop(idx)
-000156c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000156d0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000156e0: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
-000156f0: 6d75 6c22 2061 6e64 2074 6572 6d2e 6465  mul" and term.de
-00015700: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-00015710: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015720: 6620 7465 726d 2e64 6572 6976 6564 5f66  f term.derived_f
-00015730: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-00015740: 7472 7565 6469 765f 2220 2b20 2822 7269  truediv_" + ("ri
-00015750: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
-00015760: 7365 2022 6c65 6674 2229 3a0a 2020 2020  se "left"):.    
-00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015780: 6966 2074 6572 6d2e 6465 7269 7665 645f  if term.derived_
-00015790: 6672 6f6d 5f6f 702e 696e 7075 7473 5b2d  from_op.inputs[-
-000157a0: 315d 203d 3d20 6f74 6865 723a 0a20 2020  1] == other:.   
-000157b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157c0: 2020 2020 2073 656c 662e 7465 726d 735b       self.terms[
-000157d0: 6964 785d 203d 2074 6572 6d2e 6465 7269  idx] = term.deri
-000157e0: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-000157f0: 7473 5b30 5d0a 2020 2020 2020 2020 2020  ts[0].          
-00015800: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015810: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00015820: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
-00015830: 2220 616e 6420 6f74 6865 722e 6465 7269  " and other.deri
-00015840: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
-00015850: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015860: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00015870: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
-00015880: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
-00015890: 6874 2220 6966 206e 6f74 2072 6967 6874  ht" if not right
-000158a0: 2065 6c73 6520 226c 6566 7422 293a 0a20   else "left"):. 
-000158b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158c0: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-000158d0: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-000158e0: 7473 5b2d 315d 203d 3d20 7465 726d 3a0a  ts[-1] == term:.
-000158f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015900: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00015910: 6d73 5b69 6478 5d20 3d20 6f74 6865 722e  ms[idx] = other.
-00015920: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-00015930: 696e 7075 7473 5b30 5d0a 2020 2020 2020  inputs[0].      
-00015940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015950: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00015960: 2020 2020 2069 6620 7465 726d 2e69 735f       if term.is_
-00015970: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-00015980: 6469 6d28 2920 616e 6420 6f74 6865 722e  dim() and other.
-00015990: 6973 5f63 6f6e 7374 616e 745f 7374 6174  is_constant_stat
-000159a0: 6963 5f64 696d 2829 3a0a 2020 2020 2020  ic_dim():.      
-000159b0: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
-000159c0: 6420 3d3d 2022 6d75 6c22 3a0a 2020 2020  d == "mul":.    
-000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159e0: 6966 2074 6572 6d2e 6469 6d65 6e73 696f  if term.dimensio
-000159f0: 6e20 2a20 6f74 6865 722e 6469 6d65 6e73  n * other.dimens
-00015a00: 696f 6e20 3d3d 2031 3a0a 2020 2020 2020  ion == 1:.      
-00015a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a20: 2020 7365 6c66 2e74 6572 6d73 2e70 6f70    self.terms.pop
-00015a30: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
-00015a40: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015a50: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00015a60: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00015a70: 726d 735b 6964 785d 203d 205f 6d61 6b65  rms[idx] = _make
-00015a80: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00015a90: 5f64 696d 2874 6572 6d2e 6469 6d65 6e73  _dim(term.dimens
-00015aa0: 696f 6e20 2a20 6f74 6865 722e 6469 6d65  ion * other.dime
-00015ab0: 6e73 696f 6e2c 206b 696e 643d 7465 726d  nsion, kind=term
-00015ac0: 2e6b 696e 6429 0a20 2020 2020 2020 2020  .kind).         
-00015ad0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015ae0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00015af0: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
-00015b00: 7468 2822 6469 7622 2920 616e 6420 7465  th("div") and te
-00015b10: 726d 2e64 696d 656e 7369 6f6e 2025 206f  rm.dimension % o
-00015b20: 7468 6572 2e64 696d 656e 7369 6f6e 203d  ther.dimension =
-00015b30: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00015b40: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00015b50: 726d 735b 6964 785d 203d 205f 6d61 6b65  rms[idx] = _make
-00015b60: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00015b70: 5f64 696d 2874 6572 6d2e 6469 6d65 6e73  _dim(term.dimens
-00015b80: 696f 6e20 2f2f 206f 7468 6572 2e64 696d  ion // other.dim
-00015b90: 656e 7369 6f6e 2c20 6b69 6e64 3d74 6572  ension, kind=ter
-00015ba0: 6d2e 6b69 6e64 290a 2020 2020 2020 2020  m.kind).        
-00015bb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015bc0: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
-00015bd0: 2020 2023 2046 616c 6c62 6163 6b20 7769     # Fallback wi
-00015be0: 7468 2067 656e 6572 6963 2068 616e 646c  th generic handl
-00015bf0: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
-00015c00: 206f 705f 6b69 6e64 203d 206b 696e 6420   op_kind = kind 
-00015c10: 2b20 225f 2220 2b20 2822 7269 6768 7422  + "_" + ("right"
-00015c20: 2069 6620 7269 6768 7420 656c 7365 2022   if right else "
-00015c30: 6c65 6674 2229 0a20 2020 2020 2020 2020  left").         
-00015c40: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
-00015c50: 6974 6828 2264 6976 2229 2061 6e64 2074  ith("div") and t
-00015c60: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
-00015c70: 5f6f 7020 616e 6420 7465 726d 2e64 6572  _op and term.der
-00015c80: 6976 6564 5f66 726f 6d5f 6f70 2e6b 696e  ived_from_op.kin
-00015c90: 6420 3d3d 206f 705f 6b69 6e64 3a0a 2020  d == op_kind:.  
-00015ca0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00015cb0: 6d65 7261 746f 7220 3d20 7465 726d 2e64  merator = term.d
-00015cc0: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
-00015cd0: 6e70 7574 735b 305d 0a20 2020 2020 2020  nputs[0].       
-00015ce0: 2020 2020 2020 2020 2064 656e 6f6d 696e           denomin
-00015cf0: 6174 6f72 203d 2074 6572 6d2e 6465 7269  ator = term.deri
-00015d00: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-00015d10: 7473 5b31 5d0a 2020 2020 2020 2020 2020  ts[1].          
-00015d20: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00015d30: 5b69 6478 5d20 3d20 5f4f 704d 756c 7454  [idx] = _OpMultT
-00015d40: 6572 6d2e 6e65 775f 6469 765f 6469 6d28  erm.new_div_dim(
-00015d50: 6e75 6d65 7261 746f 722c 2064 656e 6f6d  numerator, denom
-00015d60: 696e 6174 6f72 202a 206f 7468 6572 2c20  inator * other, 
-00015d70: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00015d80: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
-00015d90: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00015da0: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-00015db0: 6e64 7377 6974 6828 2264 6976 2229 3a0a  ndswith("div"):.
-00015dc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015dd0: 2e74 6572 6d73 203d 205b 5f4f 704d 756c  .terms = [_OpMul
-00015de0: 7454 6572 6d2e 6e65 775f 6469 765f 6469  tTerm.new_div_di
-00015df0: 6d28 7365 6c66 2e61 735f 6469 6d28 292c  m(self.as_dim(),
-00015e00: 206f 7468 6572 2c20 6b69 6e64 3d6b 696e   other, kind=kin
-00015e10: 642c 2072 6967 6874 3d72 6967 6874 295d  d, right=right)]
-00015e20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00015e30: 7572 6e0a 2020 2020 2020 2020 6966 206b  urn.        if k
-00015e40: 696e 6420 3d3d 2022 6d75 6c22 3a0a 2020  ind == "mul":.  
-00015e50: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
-00015e60: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
-00015e70: 2020 2020 7365 6c66 2e74 6572 6d73 2e61      self.terms.a
-00015e80: 7070 656e 6428 6f74 6865 7229 0a20 2020  ppend(other).   
-00015e90: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00015ea0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015eb0: 656c 662e 7465 726d 732e 696e 7365 7274  elf.terms.insert
-00015ec0: 2830 2c20 6f74 6865 7229 0a20 2020 2020  (0, other).     
-00015ed0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00015ee0: 2020 2020 2020 6173 7365 7274 2046 616c        assert Fal
-00015ef0: 7365 0a0a 2020 2020 4063 6c61 7373 6d65  se..    @classme
-00015f00: 7468 6f64 0a20 2020 2064 6566 206e 6577  thod.    def new
-00015f10: 5f64 6976 5f64 696d 2863 6c73 2c20 6e75  _div_dim(cls, nu
-00015f20: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
-00015f30: 6174 6f72 2c20 6b69 6e64 2c20 7269 6768  ator, kind, righ
-00015f40: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
-00015f50: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-00015f60: 696d 206e 756d 6572 6174 6f72 3a0a 2020  im numerator:.  
-00015f70: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00015f80: 2064 656e 6f6d 696e 6174 6f72 3a0a 2020   denominator:.  
-00015f90: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
-00015fa0: 206b 696e 643a 2022 666c 6f6f 7264 6976   kind: "floordiv
-00015fb0: 2220 6f72 2022 6365 696c 6469 7622 206f  " or "ceildiv" o
-00015fc0: 7220 2274 7275 6564 6976 220a 2020 2020  r "truediv".    
-00015fd0: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00015fe0: 7269 6768 743a 0a20 2020 2020 2020 203a  right:.        :
-00015ff0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00016000: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-00016010: 696d 5f76 616c 7565 203d 204e 6f6e 650a  im_value = None.
-00016020: 2020 2020 2020 2020 6120 3d20 6e75 6d65          a = nume
-00016030: 7261 746f 722e 6469 6d65 6e73 696f 6e0a  rator.dimension.
-00016040: 2020 2020 2020 2020 6220 3d20 6465 6e6f          b = deno
-00016050: 6d69 6e61 746f 722e 6469 6d65 6e73 696f  minator.dimensio
-00016060: 6e0a 2020 2020 2020 2020 6966 2061 2069  n.        if a i
-00016070: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2062  s not None and b
-00016080: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00016090: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
-000160a0: 6420 3d3d 2022 666c 6f6f 7264 6976 223a  d == "floordiv":
-000160b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000160c0: 2064 696d 5f76 616c 7565 203d 2061 202f   dim_value = a /
-000160d0: 2f20 620a 2020 2020 2020 2020 2020 2020  / b.            
-000160e0: 656c 6966 206b 696e 6420 3d3d 2022 6365  elif kind == "ce
-000160f0: 696c 6469 7622 3a0a 2020 2020 2020 2020  ildiv":.        
-00016100: 2020 2020 2020 2020 6469 6d5f 7661 6c75          dim_valu
-00016110: 6520 3d20 2d28 2d61 202f 2f20 6229 0a20  e = -(-a // b). 
-00016120: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016130: 6620 6120 2520 6220 3d3d 2030 2061 6e64  f a % b == 0 and
-00016140: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-00016150: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
-00016160: 203d 2022 666c 6f6f 7264 6976 2220 2023   = "floordiv"  #
-00016170: 2066 6f72 206e 6963 6572 2064 6573 6372   for nicer descr
-00016180: 6970 7469 6f6e 2c20 616e 6420 646f 6573  iption, and does
-00016190: 206e 6f74 206d 6174 7465 720a 2020 2020   not matter.    
-000161a0: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-000161b0: 6420 3d3d 2022 7472 7565 6469 7622 3a0a  d == "truediv":.
-000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161d0: 6966 2061 2025 2062 2021 3d20 303a 0a20  if a % b != 0:. 
-000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161f0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00016200: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00016210: 2020 2020 2020 2020 2020 2020 2022 2573               "%s
-00016220: 2074 7275 6564 6976 2025 7320 6f6e 6c79   truediv %s only
-00016230: 2061 6c6c 6f77 6564 2069 6620 7468 6520   allowed if the 
-00016240: 7265 7375 6c74 2069 7320 616e 2069 6e74  result is an int
-00016250: 6567 6572 2220 2520 286e 756d 6572 6174  eger" % (numerat
-00016260: 6f72 2c20 6465 6e6f 6d69 6e61 746f 7229  or, denominator)
-00016270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016280: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00016290: 2020 2020 2020 2064 696d 5f76 616c 7565         dim_value
-000162a0: 203d 2061 202f 2f20 620a 2020 2020 2020   = a // b.      
-000162b0: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
-000162c0: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
-000162d0: 2020 2020 2020 2020 6b69 6e64 203d 2022          kind = "
-000162e0: 666c 6f6f 7264 6976 2220 2023 2066 6f72  floordiv"  # for
-000162f0: 206e 6963 6572 2064 6573 6372 6970 7469   nicer descripti
-00016300: 6f6e 2c20 616e 6420 646f 6573 206e 6f74  on, and does not
-00016310: 206d 6174 7465 720a 2020 2020 2020 2020   matter.        
-00016320: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00016330: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00016340: 5661 6c75 6545 7272 6f72 2822 696e 7661  ValueError("inva
-00016350: 6c69 6420 6b69 6e64 2025 7222 2025 2028  lid kind %r" % (
-00016360: 6b69 6e64 2c29 290a 2020 2020 2020 2020  kind,)).        
-00016370: 6966 206b 696e 6420 3d3d 2022 666c 6f6f  if kind == "floo
-00016380: 7264 6976 2220 616e 6420 7269 6768 743a  rdiv" and right:
-00016390: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-000163a0: 6372 6970 7469 6f6e 203d 2022 2573 2f2f  cription = "%s//
-000163b0: 2573 2220 2520 285f 6765 745f 6465 7363  %s" % (_get_desc
-000163c0: 7269 7074 696f 6e28 6e75 6d65 7261 746f  ription(numerato
-000163d0: 7229 2c20 5f67 6574 5f64 6573 6372 6970  r), _get_descrip
-000163e0: 7469 6f6e 2864 656e 6f6d 696e 6174 6f72  tion(denominator
-000163f0: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
-00016400: 6b69 6e64 203d 3d20 2263 6569 6c64 6976  kind == "ceildiv
-00016410: 2220 616e 6420 7269 6768 743a 0a20 2020  " and right:.   
-00016420: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00016430: 7469 6f6e 203d 2022 e28c 8825 732f 2573  tion = "...%s/%s
-00016440: e28c 8922 2025 2028 5f67 6574 5f64 6573  ..." % (_get_des
-00016450: 6372 6970 7469 6f6e 286e 756d 6572 6174  cription(numerat
-00016460: 6f72 292c 205f 6765 745f 6465 7363 7269  or), _get_descri
-00016470: 7074 696f 6e28 6465 6e6f 6d69 6e61 746f  ption(denominato
-00016480: 7229 290a 2020 2020 2020 2020 656c 7365  r)).        else
-00016490: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-000164a0: 7363 7269 7074 696f 6e20 3d20 2225 735f  scription = "%s_
-000164b0: 2573 2825 732c 2025 7329 2220 2520 280a  %s(%s, %s)" % (.
-000164c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164d0: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
-000164e0: 2020 2020 2020 2272 6967 6874 2220 6966        "right" if
-000164f0: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
-00016500: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00016510: 2020 2020 5f67 6574 5f64 6573 6372 6970      _get_descrip
-00016520: 7469 6f6e 286e 756d 6572 6174 6f72 2c20  tion(numerator, 
-00016530: 6272 6163 6b65 7473 3d46 616c 7365 292c  brackets=False),
-00016540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016550: 205f 6765 745f 6465 7363 7269 7074 696f   _get_descriptio
-00016560: 6e28 6465 6e6f 6d69 6e61 746f 722c 2062  n(denominator, b
-00016570: 7261 636b 6574 733d 4661 6c73 6529 2c0a  rackets=False),.
-00016580: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00016590: 2020 2020 2020 6f70 5f6b 696e 6420 3d20        op_kind = 
-000165a0: 6b69 6e64 0a20 2020 2020 2020 2069 6620  kind.        if 
-000165b0: 6120 6973 206e 6f74 204e 6f6e 6520 616e  a is not None an
-000165c0: 6420 6220 6973 206e 6f74 204e 6f6e 6520  d b is not None 
-000165d0: 616e 6420 6120 2520 6220 3d3d 2030 3a0a  and a % b == 0:.
-000165e0: 2020 2020 2020 2020 2020 2020 6f70 5f6b              op_k
-000165f0: 696e 6420 3d20 2274 7275 6564 6976 2220  ind = "truediv" 
-00016600: 2023 206d 616b 6573 2073 6f6d 6520 6f74   # makes some ot
-00016610: 6865 7220 6368 6563 6b73 2073 696d 706c  her checks simpl
-00016620: 6572 0a20 2020 2020 2020 206f 705f 6b69  er.        op_ki
-00016630: 6e64 202b 3d20 225f 2220 2b20 2822 7269  nd += "_" + ("ri
-00016640: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
-00016650: 7365 2022 6c65 6674 2229 0a20 2020 2020  se "left").     
-00016660: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
-00016670: 280a 2020 2020 2020 2020 2020 2020 6465  (.            de
-00016680: 7363 7269 7074 696f 6e3d 6465 7363 7269  scription=descri
-00016690: 7074 696f 6e2c 0a20 2020 2020 2020 2020  ption,.         
-000166a0: 2020 206b 696e 643d 6e75 6d65 7261 746f     kind=numerato
-000166b0: 722e 6b69 6e64 2c0a 2020 2020 2020 2020  r.kind,.        
-000166c0: 2020 2020 6469 6d65 6e73 696f 6e3d 6469      dimension=di
-000166d0: 6d5f 7661 6c75 652c 0a20 2020 2020 2020  m_value,.       
-000166e0: 2020 2020 2064 6572 6976 6564 5f66 726f       derived_fro
-000166f0: 6d5f 6f70 3d4f 7028 6b69 6e64 3d6f 705f  m_op=Op(kind=op_
-00016700: 6b69 6e64 2c20 696e 7075 7473 3d5b 6e75  kind, inputs=[nu
-00016710: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
-00016720: 6174 6f72 5d29 2c0a 2020 2020 2020 2020  ator]),.        
-00016730: 2020 2020 6465 7269 7665 645f 6672 6f6d      derived_from
-00016740: 5f74 6167 3d6e 756d 6572 6174 6f72 2c0a  _tag=numerator,.
-00016750: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00016760: 6566 2061 735f 6469 6d28 7365 6c66 293a  ef as_dim(self):
-00016770: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016780: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00016790: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000167a0: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
-000167b0: 6f6e 6528 293a 0a20 2020 2020 2020 2020  one():.         
-000167c0: 2020 2072 6574 7572 6e20 5f6d 616b 655f     return _make_
-000167d0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-000167e0: 6469 6d28 3129 0a20 2020 2020 2020 2069  dim(1).        i
-000167f0: 6620 6c65 6e28 7365 6c66 2e74 6572 6d73  f len(self.terms
-00016800: 2920 3d3d 2031 3a0a 2020 2020 2020 2020  ) == 1:.        
-00016810: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00016820: 7465 726d 735b 305d 0a20 2020 2020 2020  terms[0].       
-00016830: 2064 696d 5f6b 696e 6420 3d20 5f67 6574   dim_kind = _get
-00016840: 5f6d 6572 6765 645f 6469 6d5f 6b69 6e64  _merged_dim_kind
-00016850: 2873 656c 662e 7465 726d 7329 0a20 2020  (self.terms).   
-00016860: 2020 2020 2072 6574 7572 6e20 5f64 2e44       return _d.D
-00016870: 696d 280a 2020 2020 2020 2020 2020 2020  im(.            
-00016880: 6b69 6e64 3d64 696d 5f6b 696e 642c 0a20  kind=dim_kind,. 
-00016890: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-000168a0: 6970 7469 6f6e 3d22 2a22 2e6a 6f69 6e28  iption="*".join(
-000168b0: 6d61 7028 5f67 6574 5f64 6573 6372 6970  map(_get_descrip
-000168c0: 7469 6f6e 2c20 7365 6c66 2e74 6572 6d73  tion, self.terms
-000168d0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-000168e0: 6469 6d65 6e73 696f 6e3d 7365 6c66 2e64  dimension=self.d
-000168f0: 696d 656e 7369 6f6e 2c0a 2020 2020 2020  imension,.      
-00016900: 2020 2020 2020 6465 7269 7665 645f 6672        derived_fr
-00016910: 6f6d 5f6f 703d 4f70 286b 696e 643d 226d  om_op=Op(kind="m
-00016920: 756c 222c 2069 6e70 7574 733d 6c69 7374  ul", inputs=list
-00016930: 2873 656c 662e 7465 726d 7329 292c 0a20  (self.terms)),. 
-00016940: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
-00016950: 6564 5f66 726f 6d5f 7461 673d 7365 6c66  ed_from_tag=self
-00016960: 2e72 6570 7265 7365 6e74 6174 6976 655f  .representative_
-00016970: 7461 6728 292c 0a20 2020 2020 2020 2029  tag(),.        )
-00016980: 0a0a 2020 2020 6465 6620 7265 7072 6573  ..    def repres
-00016990: 656e 7461 7469 7665 5f74 6167 2873 656c  entative_tag(sel
-000169a0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000169b0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000169c0: 4469 6d7c 4e6f 6e65 0a20 2020 2020 2020  Dim|None.       
-000169d0: 2022 2222 0a20 2020 2020 2020 2023 2041   """.        # A
-000169e0: 6c73 6f20 7365 6520 4469 6d2e 5f4f 704c  lso see Dim._OpL
-000169f0: 696e 6561 7254 6572 6d2e 7265 7072 6573  inearTerm.repres
-00016a00: 656e 7461 7469 7665 5f74 6167 2829 2e0a  entative_tag()..
-00016a10: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
-00016a20: 6669 6e64 2061 6e79 2064 796e 616d 6963  find any dynamic
-00016a30: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
-00016a40: 726d 5f20 696e 2073 656c 662e 7465 726d  rm_ in self.term
-00016a50: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00016a60: 6620 7465 726d 5f2e 6973 5f64 796e 616d  f term_.is_dynam
-00016a70: 6963 2829 3a0a 2020 2020 2020 2020 2020  ic():.          
-00016a80: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00016a90: 6d5f 0a20 2020 2020 2020 2023 204e 6f77  m_.        # Now
-00016aa0: 2066 696e 6420 6e6f 6e2d 756e 7370 6563   find non-unspec
-00016ab0: 6966 6965 642e 0a20 2020 2020 2020 2066  ified..        f
-00016ac0: 6f72 2074 6572 6d5f 2069 6e20 7365 6c66  or term_ in self
-00016ad0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00016ae0: 2020 2020 6966 2074 6572 6d5f 2e6b 696e      if term_.kin
-00016af0: 6420 213d 2044 696d 5479 7065 732e 556e  d != DimTypes.Un
-00016b00: 7370 6563 6966 6965 643a 0a20 2020 2020  specified:.     
-00016b10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00016b20: 6e20 7465 726d 5f0a 2020 2020 2020 2020  n term_.        
-00016b30: 2320 4e6f 7720 6669 6e64 2061 6e79 2e0a  # Now find any..
-00016b40: 2020 2020 2020 2020 666f 7220 7465 726d          for term
-00016b50: 5f20 696e 2073 656c 662e 7465 726d 733a  _ in self.terms:
-00016b60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00016b70: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
-00016b80: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
-00016b90: 636c 6173 7320 5f4f 704c 696e 6561 7254  class _OpLinearT
-00016ba0: 6572 6d3a 0a20 2020 2022 2222 0a20 2020  erm:.    """.   
-00016bb0: 2072 6570 7265 7365 6e74 7320 7374 6820   represents sth 
-00016bc0: 6c69 6b65 2061 202a 2062 202b 2063 0a20  like a * b + c. 
-00016bd0: 2020 2022 2222 0a0a 2020 2020 4063 6c61     """..    @cla
-00016be0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00016bf0: 2066 726f 6d5f 6469 6d28 636c 732c 2064   from_dim(cls, d
-00016c00: 696d 293a 0a20 2020 2020 2020 2022 2222  im):.        """
-00016c10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00016c20: 4469 6d20 6469 6d3a 0a20 2020 2020 2020  Dim dim:.       
-00016c30: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
-00016c40: 4c69 6e65 6172 5465 726d 0a20 2020 2020  LinearTerm.     
-00016c50: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00016c60: 6573 203d 2063 6c73 2e7a 6572 6f28 290a  es = cls.zero().
-00016c70: 2020 2020 2020 2020 7265 732e 6578 7465          res.exte
-00016c80: 6e64 5f61 6464 5f73 7562 5f28 6469 6d2c  nd_add_sub_(dim,
-00016c90: 206b 696e 643d 2261 6464 222c 2072 6967   kind="add", rig
-00016ca0: 6874 3d54 7275 6529 0a20 2020 2020 2020  ht=True).       
-00016cb0: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
-00016cc0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00016cd0: 2020 6465 6620 7a65 726f 2863 6c73 293a    def zero(cls):
-00016ce0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016cf0: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00016d00: 2e5f 4f70 4c69 6e65 6172 5465 726d 0a20  ._OpLinearTerm. 
-00016d10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016d20: 2020 2072 6574 7572 6e20 5f4f 704c 696e     return _OpLin
-00016d30: 6561 7254 6572 6d28 5b5d 290a 0a20 2020  earTerm([])..   
-00016d40: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00016d50: 6c66 2c20 7465 726d 7329 3a0a 2020 2020  lf, terms):.    
-00016d60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00016d70: 3a70 6172 616d 206c 6973 745b 4469 6d2e  :param list[Dim.
-00016d80: 5f4f 704d 756c 7454 6572 6d5d 2074 6572  _OpMultTerm] ter
-00016d90: 6d73 3a0a 2020 2020 2020 2020 2222 220a  ms:.        """.
-00016da0: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00016db0: 6d73 203d 2074 6572 6d73 0a0a 2020 2020  ms = terms..    
-00016dc0: 6465 6620 5f5f 6861 7368 5f5f 2873 656c  def __hash__(sel
-00016dd0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00016de0: 726e 2068 6173 6828 7475 706c 6528 7365  rn hash(tuple(se
-00016df0: 6c66 2e74 6572 6d73 2929 0a0a 2020 2020  lf.terms))..    
-00016e00: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
-00016e10: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00016e20: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
-00016e30: 7468 6572 2c20 5f4f 704c 696e 6561 7254  ther, _OpLinearT
-00016e40: 6572 6d29 3a0a 2020 2020 2020 2020 2020  erm):.          
-00016e50: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
-00016e60: 726d 7320 3d3d 206f 7468 6572 2e74 6572  rms == other.ter
-00016e70: 6d73 0a20 2020 2020 2020 2072 6574 7572  ms.        retur
-00016e80: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00016e90: 205f 5f6e 655f 5f28 7365 6c66 2c20 6f74   __ne__(self, ot
-00016ea0: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-00016eb0: 7475 726e 206e 6f74 2073 656c 662e 5f5f  turn not self.__
-00016ec0: 6571 5f5f 286f 7468 6572 290a 0a20 2020  eq__(other)..   
-00016ed0: 2064 6566 2061 735f 6469 6d28 7365 6c66   def as_dim(self
-00016ee0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00016ef0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00016f00: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-00016f10: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00016f20: 735f 7a65 726f 2829 3a0a 2020 2020 2020  s_zero():.      
-00016f30: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00016f40: 6b65 5f63 6f6e 7374 616e 745f 7374 6174  ke_constant_stat
-00016f50: 6963 5f64 696d 2830 290a 2020 2020 2020  ic_dim(0).      
-00016f60: 2020 6966 206c 656e 2873 656c 662e 7465    if len(self.te
-00016f70: 726d 7329 203d 3d20 313a 0a20 2020 2020  rms) == 1:.     
-00016f80: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00016f90: 6c66 2e74 6572 6d73 5b30 5d2e 6173 5f64  lf.terms[0].as_d
-00016fa0: 696d 2829 0a20 2020 2020 2020 2061 6464  im().        add
-00016fb0: 5f70 6172 7473 203d 205b 5d0a 2020 2020  _parts = [].    
-00016fc0: 2020 2020 6465 7363 5f70 6172 7473 203d      desc_parts =
-00016fd0: 205b 5d0a 2020 2020 2020 2020 6469 6d20   [].        dim 
-00016fe0: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
-00016ff0: 7465 726d 2069 6e20 7365 6c66 2e74 6572  term in self.ter
-00017000: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00017010: 7320 3d20 7465 726d 2e61 735f 6469 6d28  s = term.as_dim(
-00017020: 290a 2020 2020 2020 2020 2020 2020 6164  ).            ad
-00017030: 645f 7061 7274 732e 6170 7065 6e64 2873  d_parts.append(s
-00017040: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
-00017050: 7363 5f70 6172 7473 2e61 7070 656e 6428  sc_parts.append(
-00017060: 5f67 6574 5f64 6573 6372 6970 7469 6f6e  _get_description
-00017070: 2873 2929 0a20 2020 2020 2020 2020 2020  (s)).           
-00017080: 2069 6620 6469 6d20 6973 206e 6f74 204e   if dim is not N
-00017090: 6f6e 6520 616e 6420 732e 6469 6d65 6e73  one and s.dimens
-000170a0: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-000170b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000170c0: 2064 696d 202b 3d20 732e 6469 6d65 6e73   dim += s.dimens
-000170d0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000170e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000170f0: 2020 2020 2020 6469 6d20 3d20 4e6f 6e65        dim = None
-00017100: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00017110: 6164 645f 7061 7274 7329 203d 3d20 313a  add_parts) == 1:
-00017120: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00017130: 7572 6e20 6164 645f 7061 7274 735b 305d  urn add_parts[0]
-00017140: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017150: 5f64 2e44 696d 280a 2020 2020 2020 2020  _d.Dim(.        
-00017160: 2020 2020 6b69 6e64 3d5f 6765 745f 6d65      kind=_get_me
-00017170: 7267 6564 5f64 696d 5f6b 696e 6428 6164  rged_dim_kind(ad
-00017180: 645f 7061 7274 7329 2c0a 2020 2020 2020  d_parts),.      
-00017190: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-000171a0: 6e3d 222b 222e 6a6f 696e 2864 6573 635f  n="+".join(desc_
-000171b0: 7061 7274 7329 2c0a 2020 2020 2020 2020  parts),.        
-000171c0: 2020 2020 6469 6d65 6e73 696f 6e3d 6469      dimension=di
-000171d0: 6d2c 0a20 2020 2020 2020 2020 2020 2064  m,.            d
-000171e0: 6572 6976 6564 5f66 726f 6d5f 6f70 3d4f  erived_from_op=O
-000171f0: 7028 6b69 6e64 3d22 6164 6422 2c20 696e  p(kind="add", in
-00017200: 7075 7473 3d61 6464 5f70 6172 7473 292c  puts=add_parts),
-00017210: 0a20 2020 2020 2020 2020 2020 2064 6572  .            der
-00017220: 6976 6564 5f66 726f 6d5f 7461 673d 7365  ived_from_tag=se
-00017230: 6c66 2e72 6570 7265 7365 6e74 6174 6976  lf.representativ
-00017240: 655f 7461 6728 292c 0a20 2020 2020 2020  e_tag(),.       
-00017250: 2029 0a0a 2020 2020 6465 6620 5f5f 7265   )..    def __re
-00017260: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-00017270: 2020 2020 7265 7475 726e 2022 4469 6d2e      return "Dim.
-00017280: 5f4f 704c 696e 6561 7254 6572 6d28 2572  _OpLinearTerm(%r
-00017290: 2922 2025 2028 7365 6c66 2e74 6572 6d73  )" % (self.terms
-000172a0: 2c29 0a0a 2020 2020 6465 6620 6973 5f7a  ,)..    def is_z
-000172b0: 6572 6f28 7365 6c66 293a 0a20 2020 2020  ero(self):.     
-000172c0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-000172d0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-000172e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000172f0: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
-00017300: 7465 726d 730a 0a20 2020 2064 6566 2065  terms..    def e
-00017310: 7874 656e 645f 6164 645f 7375 625f 2873  xtend_add_sub_(s
-00017320: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
-00017330: 2c20 7269 6768 7429 3a0a 2020 2020 2020  , right):.      
-00017340: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00017350: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
-00017360: 6572 3a0a 2020 2020 2020 2020 3a70 6172  er:.        :par
-00017370: 616d 2073 7472 206b 696e 643a 2022 6164  am str kind: "ad
-00017380: 6422 206f 7220 2273 7562 220a 2020 2020  d" or "sub".    
-00017390: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-000173a0: 7269 6768 743a 206f 7220 6c65 6674 2e20  right: or left. 
-000173b0: 7269 6768 7420 6d65 616e 7320 7365 6c66  right means self
-000173c0: 202b 206f 7468 6572 2c20 6c65 6674 206d   + other, left m
-000173d0: 6561 6e73 206f 7468 6572 202b 2073 656c  eans other + sel
-000173e0: 660a 2020 2020 2020 2020 2222 220a 2020  f.        """.  
-000173f0: 2020 2020 2020 6173 7365 7274 206b 696e        assert kin
-00017400: 6420 696e 207b 2261 6464 222c 2022 7375  d in {"add", "su
-00017410: 6222 7d0a 2020 2020 2020 2020 6f74 6865  b"}.        othe
-00017420: 7220 3d20 7365 6c66 2e5f 6d61 6b65 5f64  r = self._make_d
-00017430: 696d 286f 7468 6572 2c20 6b69 6e64 3d6b  im(other, kind=k
-00017440: 696e 6429 0a20 2020 2020 2020 2069 6620  ind).        if 
-00017450: 6f74 6865 722e 6973 5f63 6f6e 7374 616e  other.is_constan
-00017460: 745f 7374 6174 6963 5f64 696d 2829 2061  t_static_dim() a
-00017470: 6e64 206f 7468 6572 2e64 696d 656e 7369  nd other.dimensi
-00017480: 6f6e 203d 3d20 303a 0a20 2020 2020 2020  on == 0:.       
-00017490: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-000174a0: 2020 2020 6966 206f 7468 6572 2e64 6572      if other.der
-000174b0: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
-000174c0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
-000174d0: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-000174e0: 6164 6422 3a0a 2020 2020 2020 2020 2020  add":.          
-000174f0: 2020 666f 7220 6f74 6865 725f 2069 6e20    for other_ in 
-00017500: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00017510: 6f6d 5f6f 702e 696e 7075 7473 2069 6620  om_op.inputs if 
-00017520: 7269 6768 7420 656c 7365 2072 6576 6572  right else rever
-00017530: 7365 6428 6f74 6865 722e 6465 7269 7665  sed(other.derive
-00017540: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
-00017550: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017560: 2020 2073 656c 662e 6578 7465 6e64 5f61     self.extend_a
-00017570: 6464 5f73 7562 5f28 6f74 6865 725f 2c20  dd_sub_(other_, 
-00017580: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00017590: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
-000175a0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000175b0: 2020 2074 6572 6d20 3d20 5f4f 704d 756c     term = _OpMul
-000175c0: 7454 6572 6d2e 6672 6f6d 5f64 696d 286f  tTerm.from_dim(o
-000175d0: 7468 6572 290a 2020 2020 2020 2020 6e65  ther).        ne
-000175e0: 675f 7465 726d 203d 2074 6572 6d2e 6e65  g_term = term.ne
-000175f0: 6761 7469 7665 2829 0a20 2020 2020 2020  gative().       
-00017600: 2069 6620 6b69 6e64 203d 3d20 2273 7562   if kind == "sub
-00017610: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
-00017620: 6572 6d2c 206e 6567 5f74 6572 6d20 3d20  erm, neg_term = 
-00017630: 6e65 675f 7465 726d 2c20 7465 726d 0a20  neg_term, term. 
-00017640: 2020 2020 2020 206d 6f73 745f 7265 6365         most_rece
-00017650: 6e74 5f74 6572 6d20 3d20 7365 6c66 2e74  nt_term = self.t
-00017660: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
-00017670: 2065 6c73 6520 305d 2069 6620 7365 6c66   else 0] if self
-00017680: 2e74 6572 6d73 2065 6c73 6520 4e6f 6e65  .terms else None
-00017690: 0a20 2020 2020 2020 2069 6620 6d6f 7374  .        if most
-000176a0: 5f72 6563 656e 745f 7465 726d 3a0a 2020  _recent_term:.  
-000176b0: 2020 2020 2020 2020 2020 6966 206d 6f73            if mos
-000176c0: 745f 7265 6365 6e74 5f74 6572 6d20 3d3d  t_recent_term ==
-000176d0: 206e 6567 5f74 6572 6d3a 0a20 2020 2020   neg_term:.     
-000176e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000176f0: 7465 726d 732e 706f 7028 2d31 2069 6620  terms.pop(-1 if 
-00017700: 7269 6768 7420 656c 7365 2030 290a 2020  right else 0).  
-00017710: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00017720: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00017730: 2069 6620 6d6f 7374 5f72 6563 656e 745f   if most_recent_
-00017740: 7465 726d 2e69 735f 636f 6e73 7461 6e74  term.is_constant
-00017750: 5f73 7461 7469 635f 6469 6d28 2920 616e  _static_dim() an
-00017760: 6420 7465 726d 2e69 735f 636f 6e73 7461  d term.is_consta
-00017770: 6e74 5f73 7461 7469 635f 6469 6d28 293a  nt_static_dim():
-00017780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017790: 2073 656c 662e 7465 726d 735b 2d31 2069   self.terms[-1 i
-000177a0: 6620 7269 6768 7420 656c 7365 2030 5d20  f right else 0] 
-000177b0: 3d20 5f4f 704d 756c 7454 6572 6d2e 6672  = _OpMultTerm.fr
-000177c0: 6f6d 5f64 696d 280a 2020 2020 2020 2020  om_dim(.        
-000177d0: 2020 2020 2020 2020 2020 2020 5f6d 616b              _mak
-000177e0: 655f 636f 6e73 7461 6e74 5f73 7461 7469  e_constant_stati
-000177f0: 635f 6469 6d28 6d6f 7374 5f72 6563 656e  c_dim(most_recen
-00017800: 745f 7465 726d 2e64 696d 656e 7369 6f6e  t_term.dimension
-00017810: 202b 2074 6572 6d2e 6469 6d65 6e73 696f   + term.dimensio
-00017820: 6e2c 206b 696e 643d 6f74 6865 722e 6b69  n, kind=other.ki
-00017830: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
-00017840: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00017850: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00017860: 2020 2020 2020 2020 2069 6620 6d6f 7374           if most
-00017870: 5f72 6563 656e 745f 7465 726d 2e74 6572  _recent_term.ter
-00017880: 6d73 2061 6e64 2074 6572 6d2e 7465 726d  ms and term.term
-00017890: 7320 616e 6420 6d6f 7374 5f72 6563 656e  s and most_recen
-000178a0: 745f 7465 726d 2e74 6572 6d73 5b2d 315d  t_term.terms[-1]
-000178b0: 203d 3d20 7465 726d 2e74 6572 6d73 5b2d   == term.terms[-
-000178c0: 315d 3a0a 2020 2020 2020 2020 2020 2020  1]:.            
-000178d0: 2020 2020 2320 4d65 7267 6520 7465 726d      # Merge term
-000178e0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000178f0: 2020 6120 3d20 5f4f 704d 756c 7454 6572    a = _OpMultTer
-00017900: 6d2e 6672 6f6d 5f64 696d 5f66 6163 746f  m.from_dim_facto
-00017910: 7273 286d 6f73 745f 7265 6365 6e74 5f74  rs(most_recent_t
-00017920: 6572 6d2e 7465 726d 735b 3a2d 315d 292e  erm.terms[:-1]).
-00017930: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
-00017940: 2020 2020 2020 2020 2062 203d 205f 4f70           b = _Op
-00017950: 4d75 6c74 5465 726d 2e66 726f 6d5f 6469  MultTerm.from_di
-00017960: 6d5f 6661 6374 6f72 7328 7465 726d 2e74  m_factors(term.t
-00017970: 6572 6d73 5b3a 2d31 5d29 2e61 735f 6469  erms[:-1]).as_di
-00017980: 6d28 290a 2020 2020 2020 2020 2020 2020  m().            
-00017990: 2020 2020 7265 7320 3d20 5f4f 704d 756c      res = _OpMul
-000179a0: 7454 6572 6d2e 6672 6f6d 5f64 696d 2828  tTerm.from_dim((
-000179b0: 6120 2b20 6229 2069 6620 7269 6768 7420  a + b) if right 
-000179c0: 656c 7365 2028 6220 2b20 6129 290a 2020  else (b + a)).  
-000179d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000179e0: 732e 6578 7465 6e64 5f6d 756c 5f64 6976  s.extend_mul_div
-000179f0: 5f28 7465 726d 2e74 6572 6d73 5b2d 315d  _(term.terms[-1]
-00017a00: 2c20 6b69 6e64 3d22 6d75 6c22 2c20 7269  , kind="mul", ri
-00017a10: 6768 743d 5472 7565 290a 2020 2020 2020  ght=True).      
-00017a20: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00017a30: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
-00017a40: 2065 6c73 6520 305d 203d 2072 6573 0a20   else 0] = res. 
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017a60: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00017a70: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-00017a80: 2020 2020 7365 6c66 2e74 6572 6d73 2e61      self.terms.a
-00017a90: 7070 656e 6428 7465 726d 290a 2020 2020  ppend(term).    
-00017aa0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00017ab0: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00017ac0: 2e69 6e73 6572 7428 302c 2074 6572 6d29  .insert(0, term)
-00017ad0: 0a0a 2020 2020 6465 6620 6578 7465 6e64  ..    def extend
-00017ae0: 5f6d 756c 5f64 6976 5f28 7365 6c66 2c20  _mul_div_(self, 
-00017af0: 6f74 6865 722c 206b 696e 642c 2072 6967  other, kind, rig
-00017b00: 6874 293a 0a20 2020 2020 2020 2022 2222  ht):.        """
-00017b10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00017b20: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-00017b30: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-00017b40: 7220 6b69 6e64 3a20 226d 756c 2220 6f72  r kind: "mul" or
-00017b50: 2022 6365 696c 6469 7622 0a20 2020 2020   "ceildiv".     
-00017b60: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
-00017b70: 6967 6874 3a20 6f72 206c 6566 742e 2072  ight: or left. r
-00017b80: 6967 6874 206d 6561 6e73 2073 656c 6620  ight means self 
-00017b90: 2a20 6f74 6865 722c 206c 6566 7420 6d65  * other, left me
-00017ba0: 616e 7320 6f74 6865 7220 2a20 7365 6c66  ans other * self
-00017bb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00017bc0: 2020 2020 2061 7373 6572 7420 6b69 6e64       assert kind
-00017bd0: 2069 6e20 7b22 6d75 6c22 2c20 2266 6c6f   in {"mul", "flo
-00017be0: 6f72 6469 7622 2c20 2274 7275 6564 6976  ordiv", "truediv
-00017bf0: 222c 2022 6365 696c 6469 7622 7d0a 2020  ", "ceildiv"}.  
-00017c00: 2020 2020 2020 6f74 6865 7220 3d20 7365        other = se
-00017c10: 6c66 2e5f 6d61 6b65 5f64 696d 286f 7468  lf._make_dim(oth
-00017c20: 6572 2c20 6b69 6e64 3d6b 696e 6429 0a20  er, kind=kind). 
-00017c30: 2020 2020 2020 2069 6620 6b69 6e64 203d         if kind =
-00017c40: 3d20 226d 756c 2220 616e 6420 7269 6768  = "mul" and righ
-00017c50: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
-00017c60: 6620 6e6f 7420 616c 6c28 7465 726d 2e63  f not all(term.c
-00017c70: 616e 5f73 696d 706c 6966 7928 6f74 6865  an_simplify(othe
-00017c80: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
-00017c90: 6768 743d 7269 6768 7429 2066 6f72 2074  ght=right) for t
-00017ca0: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
-00017cb0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00017cc0: 2020 2020 2320 446f 2069 7420 7468 6520      # Do it the 
-00017cd0: 6f74 6865 7220 7761 7920 6172 6f75 6e64  other way around
-00017ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017cf0: 2073 656c 662e 7465 726d 732c 206f 7468   self.terms, oth
-00017d00: 6572 203d 205f 4f70 4c69 6e65 6172 5465  er = _OpLinearTe
-00017d10: 726d 2e66 726f 6d5f 6469 6d28 6f74 6865  rm.from_dim(othe
-00017d20: 7229 2e74 6572 6d73 2c20 7365 6c66 2e61  r).terms, self.a
-00017d30: 735f 6469 6d28 290a 2020 2020 2020 2020  s_dim().        
-00017d40: 2020 2020 2020 2020 7269 6768 7420 3d20          right = 
-00017d50: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
-00017d60: 206f 7468 6572 2e69 735f 636f 6e73 7461   other.is_consta
-00017d70: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
-00017d80: 616e 6420 6f74 6865 722e 6469 6d65 6e73  and other.dimens
-00017d90: 696f 6e20 3d3d 2031 3a0a 2020 2020 2020  ion == 1:.      
-00017da0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00017db0: 2020 2020 2069 6620 6b69 6e64 2e65 6e64       if kind.end
-00017dc0: 7377 6974 6828 2264 6976 2229 2061 6e64  swith("div") and
-00017dd0: 206c 656e 2873 656c 662e 7465 726d 7329   len(self.terms)
-00017de0: 203e 3d20 323a 0a20 2020 2020 2020 2020   >= 2:.         
-00017df0: 2020 2069 6620 616e 7928 6e6f 7420 7465     if any(not te
-00017e00: 726d 2e64 6976 6973 6962 6c65 286f 7468  rm.divisible(oth
-00017e10: 6572 2c20 7269 6768 743d 7269 6768 7429  er, right=right)
-00017e20: 2066 6f72 2074 6572 6d20 696e 2073 656c   for term in sel
-00017e30: 662e 7465 726d 7329 3a0a 2020 2020 2020  f.terms):.      
-00017e40: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00017e50: 6572 6d73 203d 205b 0a20 2020 2020 2020  erms = [.       
-00017e60: 2020 2020 2020 2020 2020 2020 205f 4f70               _Op
-00017e70: 4d75 6c74 5465 726d 2e66 726f 6d5f 6469  MultTerm.from_di
-00017e80: 6d28 5f4f 704d 756c 7454 6572 6d2e 6e65  m(_OpMultTerm.ne
-00017e90: 775f 6469 765f 6469 6d28 7365 6c66 2e61  w_div_dim(self.a
-00017ea0: 735f 6469 6d28 292c 206f 7468 6572 2c20  s_dim(), other, 
-00017eb0: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00017ec0: 3d72 6967 6874 2929 0a20 2020 2020 2020  =right)).       
-00017ed0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00017ee0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00017ef0: 6e0a 2020 2020 2020 2020 666f 7220 7465  n.        for te
-00017f00: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
-00017f10: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-00017f20: 726d 2e65 7874 656e 645f 6d75 6c5f 6469  rm.extend_mul_di
-00017f30: 765f 286f 7468 6572 2c20 6b69 6e64 3d6b  v_(other, kind=k
-00017f40: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
-00017f50: 290a 0a20 2020 2064 6566 205f 6d61 6b65  )..    def _make
-00017f60: 5f64 696d 2873 656c 662c 206f 7468 6572  _dim(self, other
-00017f70: 2c20 6b69 6e64 293a 0a20 2020 2020 2020  , kind):.       
-00017f80: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00017f90: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00017fa0: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
-00017fb0: 6d20 7374 7220 6b69 6e64 3a0a 2020 2020  m str kind:.    
-00017fc0: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00017fd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00017fe0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00017ff0: 6528 6f74 6865 722c 2069 6e74 293a 0a20  e(other, int):. 
-00018000: 2020 2020 2020 2020 2020 2062 6173 655f             base_
-00018010: 7461 6720 3d20 7365 6c66 2e72 6570 7265  tag = self.repre
-00018020: 7365 6e74 6174 6976 655f 7461 6728 290a  sentative_tag().
+00012880: 2074 6572 6d20 3d20 5f4f 704c 696e 6561   term = _OpLinea
+00012890: 7254 6572 6d2e 6672 6f6d 5f64 696d 2873  rTerm.from_dim(s
+000128a0: 656c 6629 0a20 2020 2020 2020 2074 6572  elf).        ter
+000128b0: 6d2e 6578 7465 6e64 5f61 6464 5f73 7562  m.extend_add_sub
+000128c0: 5f28 6f74 6865 722c 206b 696e 643d 2273  _(other, kind="s
+000128d0: 7562 222c 2072 6967 6874 3d46 616c 7365  ub", right=False
+000128e0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000128f0: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
+00012900: 2020 2020 6465 6620 5f5f 6d75 6c5f 5f28      def __mul__(
+00012910: 7365 6c66 3a20 4469 6d2c 206f 7468 6572  self: Dim, other
+00012920: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012930: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00012940: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+00012950: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00012960: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012970: 2020 2020 2074 6572 6d20 3d20 5f4f 704c       term = _OpL
+00012980: 696e 6561 7254 6572 6d2e 6672 6f6d 5f64  inearTerm.from_d
+00012990: 696d 2873 656c 6629 0a20 2020 2020 2020  im(self).       
+000129a0: 2074 6572 6d2e 6578 7465 6e64 5f6d 756c   term.extend_mul
+000129b0: 5f64 6976 5f28 6f74 6865 722c 206b 696e  _div_(other, kin
+000129c0: 643d 226d 756c 222c 2072 6967 6874 3d54  d="mul", right=T
+000129d0: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
+000129e0: 7572 6e20 7465 726d 2e61 735f 6469 6d28  urn term.as_dim(
+000129f0: 290a 0a20 2020 2064 6566 205f 5f72 6d75  )..    def __rmu
+00012a00: 6c5f 5f28 7365 6c66 3a20 4469 6d2c 206f  l__(self: Dim, o
+00012a10: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012a20: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012a30: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00012a40: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00012a50: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00012a60: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
+00012a70: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
+00012a80: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
+00012a90: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
+00012aa0: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
+00012ab0: 206b 696e 643d 226d 756c 222c 2072 6967   kind="mul", rig
+00012ac0: 6874 3d46 616c 7365 290a 2020 2020 2020  ht=False).      
+00012ad0: 2020 7265 7475 726e 2074 6572 6d2e 6173    return term.as
+00012ae0: 5f64 696d 2829 0a0a 2020 2020 6465 6620  _dim()..    def 
+00012af0: 5f5f 666c 6f6f 7264 6976 5f5f 2873 656c  __floordiv__(sel
+00012b00: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
+00012b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012b20: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
+00012b30: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
+00012b40: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
+00012b50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012b60: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
+00012b70: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
+00012b80: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
+00012b90: 726d 2e65 7874 656e 645f 6d75 6c5f 6469  rm.extend_mul_di
+00012ba0: 765f 286f 7468 6572 2c20 6b69 6e64 3d22  v_(other, kind="
+00012bb0: 666c 6f6f 7264 6976 222c 2072 6967 6874  floordiv", right
+00012bc0: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
+00012bd0: 6574 7572 6e20 7465 726d 2e61 735f 6469  eturn term.as_di
+00012be0: 6d28 290a 0a20 2020 2064 6566 205f 5f74  m()..    def __t
+00012bf0: 7275 6564 6976 5f5f 2873 656c 662c 206f  ruediv__(self, o
+00012c00: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012c10: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012c20: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00012c30: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00012c40: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00012c50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012c60: 7365 6c66 2e64 6976 5f72 6967 6874 286f  self.div_right(o
+00012c70: 7468 6572 290a 0a20 2020 2064 6566 2064  ther)..    def d
+00012c80: 6976 5f6c 6566 7428 7365 6c66 3a20 4469  iv_left(self: Di
+00012c90: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
+00012ca0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00012cb0: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+00012cc0: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
+00012cd0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00012ce0: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
+00012cf0: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
+00012d00: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
+00012d10: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
+00012d20: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
+00012d30: 6865 722c 206b 696e 643d 2274 7275 6564  her, kind="trued
+00012d40: 6976 222c 2072 6967 6874 3d46 616c 7365  iv", right=False
+00012d50: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00012d60: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
+00012d70: 2020 2020 6465 6620 6469 765f 7269 6768      def div_righ
+00012d80: 7428 7365 6c66 3a20 4469 6d2c 206f 7468  t(self: Dim, oth
+00012d90: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
+00012da0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00012db0: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
+00012dc0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+00012dd0: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
+00012de0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
+00012df0: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
+00012e00: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
+00012e10: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
+00012e20: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
+00012e30: 696e 643d 2274 7275 6564 6976 222c 2072  ind="truediv", r
+00012e40: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
+00012e50: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
+00012e60: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
+00012e70: 2063 6569 6c64 6976 5f6c 6566 7428 7365   ceildiv_left(se
+00012e80: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
+00012e90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012ea0: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
+00012eb0: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
+00012ec0: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
+00012ed0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012ee0: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
+00012ef0: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
+00012f00: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
+00012f10: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
+00012f20: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
+00012f30: 2263 6569 6c64 6976 222c 2072 6967 6874  "ceildiv", right
+00012f40: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00012f50: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
+00012f60: 696d 2829 0a0a 2020 2020 6465 6620 6365  im()..    def ce
+00012f70: 696c 6469 765f 7269 6768 7428 7365 6c66  ildiv_right(self
+00012f80: 3a20 4469 6d2c 206f 7468 6572 293a 0a20  : Dim, other):. 
+00012f90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012fa0: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
+00012fb0: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
+00012fc0: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
+00012fd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012fe0: 2074 6572 6d20 3d20 5f4f 704c 696e 6561   term = _OpLinea
+00012ff0: 7254 6572 6d2e 6672 6f6d 5f64 696d 2873  rTerm.from_dim(s
+00013000: 656c 6629 0a20 2020 2020 2020 2074 6572  elf).        ter
+00013010: 6d2e 6578 7465 6e64 5f6d 756c 5f64 6976  m.extend_mul_div
+00013020: 5f28 6f74 6865 722c 206b 696e 643d 2263  _(other, kind="c
+00013030: 6569 6c64 6976 222c 2072 6967 6874 3d54  eildiv", right=T
+00013040: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
+00013050: 7572 6e20 7465 726d 2e61 735f 6469 6d28  urn term.as_dim(
+00013060: 290a 0a20 2020 2064 6566 205f 5f6e 6567  )..    def __neg
+00013070: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00013080: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00013090: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+000130a0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+000130b0: 7475 726e 202d 3120 2a20 7365 6c66 0a0a  turn -1 * self..
+000130c0: 2020 2020 6465 6620 6973 5f63 6f6e 7374      def is_const
+000130d0: 616e 745f 7374 6174 6963 5f64 696d 2873  ant_static_dim(s
+000130e0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+000130f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013100: 2020 3a72 6574 7572 6e3a 2064 6572 6976    :return: deriv
+00013110: 6564 206f 7020 6f66 2074 7970 6520 636f  ed op of type co
+00013120: 6e73 7461 6e74 0a20 2020 2020 2020 2022  nstant.        "
+00013130: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00013140: 6e20 7365 6c66 2e64 6572 6976 6564 5f66  n self.derived_f
+00013150: 726f 6d5f 6f70 2061 6e64 2073 656c 662e  rom_op and self.
+00013160: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00013170: 6b69 6e64 203d 3d20 2263 6f6e 7374 616e  kind == "constan
+00013180: 7422 0a0a 0a64 6566 205f 6d61 6b65 5f63  t"...def _make_c
+00013190: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+000131a0: 696d 2876 616c 7565 2c20 6b69 6e64 3d4e  im(value, kind=N
+000131b0: 6f6e 6529 3a0a 2020 2020 2222 220a 2020  one):.    """.  
+000131c0: 2020 3a70 6172 616d 2069 6e74 2076 616c    :param int val
+000131d0: 7565 3a0a 2020 2020 3a70 6172 616d 2045  ue:.    :param E
+000131e0: 6e74 6974 797c 4e6f 6e65 206b 696e 643a  ntity|None kind:
+000131f0: 0a20 2020 203a 7274 7970 653a 2044 696d  .    :rtype: Dim
+00013200: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+00013210: 7572 6e20 5f64 2e44 696d 280a 2020 2020  urn _d.Dim(.    
+00013220: 2020 2020 6469 6d65 6e73 696f 6e3d 7661      dimension=va
+00013230: 6c75 652c 0a20 2020 2020 2020 206b 696e  lue,.        kin
+00013240: 643d 6b69 6e64 206f 7220 4469 6d54 7970  d=kind or DimTyp
+00013250: 6573 2e55 6e73 7065 6369 6669 6564 2c0a  es.Unspecified,.
+00013260: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00013270: 696f 6e3d 2275 6e6e 616d 6564 5f25 7364  ion="unnamed_%sd
+00013280: 696d 5f25 6922 2025 2028 6b69 6e64 2e6e  im_%i" % (kind.n
+00013290: 616d 6520 2b20 225f 2220 6966 206b 696e  ame + "_" if kin
+000132a0: 6420 656c 7365 2022 222c 2076 616c 7565  d else "", value
+000132b0: 292c 0a20 2020 2020 2020 2064 6572 6976  ),.        deriv
+000132c0: 6564 5f66 726f 6d5f 6f70 3d4f 7028 6b69  ed_from_op=Op(ki
+000132d0: 6e64 3d22 636f 6e73 7461 6e74 222c 2069  nd="constant", i
+000132e0: 6e70 7574 733d 5b5d 2c20 6174 7472 6962  nputs=[], attrib
+000132f0: 733d 7b22 7661 6c75 6522 3a20 7661 6c75  s={"value": valu
+00013300: 657d 292c 0a20 2020 2020 2020 2061 7574  e}),.        aut
+00013310: 6f5f 6765 6e65 7261 7465 643d 5472 7565  o_generated=True
+00013320: 2c0a 2020 2020 290a 0a0a 636c 6173 7320  ,.    )...class 
+00013330: 4f70 3a0a 2020 2020 2222 220a 2020 2020  Op:.    """.    
+00013340: 4f70 206f 6e20 3a63 6c61 7373 3a60 4469  Op on :class:`Di
+00013350: 6d60 2077 6869 6368 2072 6573 756c 7473  m` which results
+00013360: 2069 6e20 6120 6465 7269 7665 6420 3a63   in a derived :c
+00013370: 6c61 7373 3a60 4469 6d60 2e0a 2020 2020  lass:`Dim`..    
+00013380: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+00013390: 6e69 745f 5f28 7365 6c66 2c20 6b69 6e64  nit__(self, kind
+000133a0: 2c20 696e 7075 7473 2c20 6174 7472 6962  , inputs, attrib
+000133b0: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
+000133c0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+000133d0: 7261 6d20 7374 7220 6b69 6e64 3a20 2261  ram str kind: "a
+000133e0: 6464 222c 2022 7375 6222 2c20 226d 756c  dd", "sub", "mul
+000133f0: 222c 2022 6365 696c 6469 7622 0a20 2020  ", "ceildiv".   
+00013400: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
+00013410: 5b44 696d 5d20 696e 7075 7473 3a0a 2020  [Dim] inputs:.  
+00013420: 2020 2020 2020 3a70 6172 616d 2064 6963        :param dic
+00013430: 745b 7374 725d 7c4e 6f6e 6520 6174 7472  t[str]|None attr
+00013440: 6962 733a 0a20 2020 2020 2020 2022 2222  ibs:.        """
+00013450: 0a20 2020 2020 2020 2073 656c 662e 6b69  .        self.ki
+00013460: 6e64 203d 206b 696e 640a 2020 2020 2020  nd = kind.      
+00013470: 2020 7365 6c66 2e69 6e70 7574 7320 3d20    self.inputs = 
+00013480: 696e 7075 7473 0a20 2020 2020 2020 2073  inputs.        s
+00013490: 656c 662e 6f75 7470 7574 203d 204e 6f6e  elf.output = Non
+000134a0: 6520 2023 2074 7970 653a 204f 7074 696f  e  # type: Optio
+000134b0: 6e61 6c5b 5f64 2e44 696d 5d0a 2020 2020  nal[_d.Dim].    
+000134c0: 2020 2020 7365 6c66 2e61 7474 7269 6273      self.attribs
+000134d0: 203d 2061 7474 7269 6273 0a0a 2020 2020   = attribs..    
+000134e0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+000134f0: 6629 3a0a 2020 2020 2020 2020 6174 7472  f):.        attr
+00013500: 6962 7320 3d20 2822 2025 7222 2025 2073  ibs = (" %r" % s
+00013510: 656c 662e 6174 7472 6962 7329 2069 6620  elf.attribs) if 
+00013520: 7365 6c66 2e61 7474 7269 6273 2065 6c73  self.attribs els
+00013530: 6520 2222 0a20 2020 2020 2020 2072 6574  e "".        ret
+00013540: 7572 6e20 223c 4469 6d2e 4f70 2025 7220  urn "<Dim.Op %r 
+00013550: 2573 2573 3e22 2025 2028 7365 6c66 2e6b  %s%s>" % (self.k
+00013560: 696e 642c 2073 656c 662e 696e 7075 7473  ind, self.inputs
+00013570: 2c20 6174 7472 6962 7329 0a0a 2020 2020  , attribs)..    
+00013580: 6465 6620 5f76 616c 7565 2873 656c 6629  def _value(self)
+00013590: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000135a0: 2073 656c 662e 6b69 6e64 2c20 7475 706c   self.kind, tupl
+000135b0: 6528 7365 6c66 2e69 6e70 7574 7329 2c20  e(self.inputs), 
+000135c0: 6672 6f7a 656e 7365 7428 7365 6c66 2e61  frozenset(self.a
+000135d0: 7474 7269 6273 2e69 7465 6d73 2829 2920  ttribs.items()) 
+000135e0: 6966 2073 656c 662e 6174 7472 6962 7320  if self.attribs 
+000135f0: 656c 7365 204e 6f6e 650a 0a20 2020 2064  else None..    d
+00013600: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
+00013610: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00013620: 6e20 6861 7368 2873 656c 662e 5f76 616c  n hash(self._val
+00013630: 7565 2829 290a 0a20 2020 2064 6566 205f  ue())..    def _
+00013640: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
+00013650: 7229 3a0a 2020 2020 2020 2020 6966 2069  r):.        if i
+00013660: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
+00013670: 204f 7029 3a0a 2020 2020 2020 2020 2020   Op):.          
+00013680: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
+00013690: 616c 7565 2829 203d 3d20 6f74 6865 722e  alue() == other.
+000136a0: 5f76 616c 7565 2829 0a20 2020 2020 2020  _value().       
+000136b0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+000136c0: 2020 2064 6566 205f 5f6e 655f 5f28 7365     def __ne__(se
+000136d0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+000136e0: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+000136f0: 656c 662e 5f5f 6571 5f5f 286f 7468 6572  elf.__eq__(other
+00013700: 290a 0a0a 6465 6620 5f67 6574 5f64 6573  )...def _get_des
+00013710: 6372 6970 7469 6f6e 2864 696d 2c20 6272  cription(dim, br
+00013720: 6163 6b65 7473 3d54 7275 6529 3a0a 2020  ackets=True):.  
+00013730: 2020 2222 220a 2020 2020 3a70 6172 616d    """.    :param
+00013740: 2044 696d 2064 696d 3a0a 2020 2020 3a70   Dim dim:.    :p
+00013750: 6172 616d 2062 6f6f 6c20 6272 6163 6b65  aram bool bracke
+00013760: 7473 3a20 6164 6420 6272 6163 6b65 7473  ts: add brackets
+00013770: 2077 6865 6e20 6e65 6365 7373 6172 790a   when necessary.
+00013780: 2020 2020 3a72 7479 7065 3a20 7374 720a      :rtype: str.
+00013790: 2020 2020 2222 220a 2020 2020 6966 2064      """.    if d
+000137a0: 696d 2e64 6573 6372 6970 7469 6f6e 2061  im.description a
+000137b0: 6e64 2064 696d 2e64 6573 6372 6970 7469  nd dim.descripti
+000137c0: 6f6e 2e73 7461 7274 7377 6974 6828 2275  on.startswith("u
+000137d0: 6e6e 616d 6564 5f22 2920 616e 6420 6469  nnamed_") and di
+000137e0: 6d2e 6469 6d65 6e73 696f 6e20 6973 206e  m.dimension is n
+000137f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00013800: 2072 6574 7572 6e20 7374 7228 6469 6d2e   return str(dim.
+00013810: 6469 6d65 6e73 696f 6e29 0a20 2020 2069  dimension).    i
+00013820: 6620 6469 6d2e 6465 7363 7269 7074 696f  f dim.descriptio
+00013830: 6e3a 0a20 2020 2020 2020 2069 6620 6272  n:.        if br
+00013840: 6163 6b65 7473 3a0a 2020 2020 2020 2020  ackets:.        
+00013850: 2020 2020 696d 706f 7274 2072 650a 0a20      import re.. 
+00013860: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00013870: 2e73 6561 7263 6828 225b 2b5c 5c2d 2f20  .search("[+\\-/ 
+00013880: 5d22 2c20 6469 6d2e 6465 7363 7269 7074  ]", dim.descript
+00013890: 696f 6e29 3a0a 2020 2020 2020 2020 2020  ion):.          
+000138a0: 2020 2020 2020 7265 7475 726e 2022 2825        return "(%
+000138b0: 7329 2220 2520 6469 6d2e 6465 7363 7269  s)" % dim.descri
+000138c0: 7074 696f 6e0a 2020 2020 2020 2020 7265  ption.        re
+000138d0: 7475 726e 2064 696d 2e64 6573 6372 6970  turn dim.descrip
+000138e0: 7469 6f6e 0a20 2020 2072 6574 7572 6e20  tion.    return 
+000138f0: 2275 6e6e 616d 6564 5f25 735f 6469 6d25  "unnamed_%s_dim%
+00013900: 7322 2025 2028 6469 6d2e 6b69 6e64 2c20  s" % (dim.kind, 
+00013910: 6469 6d2e 6469 6d65 6e73 696f 6e20 6966  dim.dimension if
+00013920: 2064 696d 2e64 696d 656e 7369 6f6e 2069   dim.dimension i
+00013930: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00013940: 223f 2229 0a0a 0a63 6c61 7373 205f 4f70  "?")...class _Op
+00013950: 4d75 6c74 5465 726d 3a0a 2020 2020 2222  MultTerm:.    ""
+00013960: 220a 2020 2020 7265 7072 6573 656e 7473  ".    represents
+00013970: 2073 7468 206c 696b 6520 6120 2a20 6220   sth like a * b 
+00013980: 2a20 630a 2020 2020 2222 220a 0a20 2020  * c.    """..   
+00013990: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+000139a0: 2020 6465 6620 6672 6f6d 5f64 696d 2863    def from_dim(c
+000139b0: 6c73 2c20 6469 6d3a 205f 642e 4469 6d29  ls, dim: _d.Dim)
+000139c0: 202d 3e20 5f4f 704d 756c 7454 6572 6d3a   -> _OpMultTerm:
+000139d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000139e0: 2020 2020 203a 7061 7261 6d20 6469 6d3a       :param dim:
+000139f0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00013a00: 3a20 6f70 206d 756c 7420 7465 726d 0a20  : op mult term. 
+00013a10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013a20: 2020 2064 696d 203d 2064 696d 2e67 6574     dim = dim.get
+00013a30: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
+00013a40: 2020 2020 2069 6620 6469 6d2e 6469 6d65       if dim.dime
+00013a50: 6e73 696f 6e20 3d3d 2031 2061 6e64 2064  nsion == 1 and d
+00013a60: 696d 2e69 735f 636f 6e73 7461 6e74 5f73  im.is_constant_s
+00013a70: 7461 7469 635f 6469 6d28 293a 0a20 2020  tatic_dim():.   
+00013a80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013a90: 636c 732e 6f6e 6528 290a 2020 2020 2020  cls.one().      
+00013aa0: 2020 6966 2064 696d 2e64 6572 6976 6564    if dim.derived
+00013ab0: 5f66 726f 6d5f 6f70 2061 6e64 2064 696d  _from_op and dim
+00013ac0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00013ad0: 2e6b 696e 6420 3d3d 2022 6d75 6c22 3a0a  .kind == "mul":.
+00013ae0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013af0: 726e 2063 6c73 286c 6973 7428 6469 6d2e  rn cls(list(dim.
+00013b00: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00013b10: 696e 7075 7473 2929 0a20 2020 2020 2020  inputs)).       
+00013b20: 2072 6574 7572 6e20 636c 7328 5b64 696d   return cls([dim
+00013b30: 5d29 0a0a 2020 2020 4063 6c61 7373 6d65  ])..    @classme
+00013b40: 7468 6f64 0a20 2020 2064 6566 2066 726f  thod.    def fro
+00013b50: 6d5f 6469 6d5f 6661 6374 6f72 7328 636c  m_dim_factors(cl
+00013b60: 732c 2064 696d 7329 3a0a 2020 2020 2020  s, dims):.      
+00013b70: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00013b80: 6172 616d 206c 6973 745b 4469 6d5d 2064  aram list[Dim] d
+00013b90: 696d 733a 0a20 2020 2020 2020 203a 7274  ims:.        :rt
+00013ba0: 7970 653a 2044 696d 2e5f 4f70 4d75 6c74  ype: Dim._OpMult
+00013bb0: 5465 726d 0a20 2020 2020 2020 2022 2222  Term.        """
+00013bc0: 0a20 2020 2020 2020 2072 6573 203d 2063  .        res = c
+00013bd0: 6c73 2e6f 6e65 2829 0a20 2020 2020 2020  ls.one().       
+00013be0: 2066 6f72 2064 2069 6e20 6469 6d73 3a0a   for d in dims:.
+00013bf0: 2020 2020 2020 2020 2020 2020 7265 732e              res.
+00013c00: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
+00013c10: 642c 206b 696e 643d 226d 756c 222c 2072  d, kind="mul", r
+00013c20: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
+00013c30: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
+00013c40: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00013c50: 2020 2020 6465 6620 6f6e 6528 636c 7329      def one(cls)
+00013c60: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013c70: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
+00013c80: 6d2e 5f4f 704d 756c 7454 6572 6d0a 2020  m._OpMultTerm.  
+00013c90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013ca0: 2020 7265 7475 726e 2063 6c73 285b 5d29    return cls([])
+00013cb0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00013cc0: 5f5f 2873 656c 662c 2074 6572 6d73 293a  __(self, terms):
+00013cd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013ce0: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
+00013cf0: 5b44 696d 5d20 7465 726d 733a 0a20 2020  [Dim] terms:.   
+00013d00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013d10: 2073 656c 662e 7465 726d 7320 3d20 7465   self.terms = te
+00013d20: 726d 730a 0a20 2020 2064 6566 205f 5f68  rms..    def __h
+00013d30: 6173 685f 5f28 7365 6c66 293a 0a20 2020  ash__(self):.   
+00013d40: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
+00013d50: 2874 7570 6c65 2873 656c 662e 7465 726d  (tuple(self.term
+00013d60: 7329 290a 0a20 2020 2064 6566 205f 5f65  s))..    def __e
+00013d70: 715f 5f28 7365 6c66 2c20 6f74 6865 7229  q__(self, other)
+00013d80: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013d90: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00013da0: 7c44 696d 2e5f 4f70 4d75 6c74 5465 726d  |Dim._OpMultTerm
+00013db0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+00013dc0: 2222 220a 2020 2020 2020 2020 6966 2069  """.        if i
+00013dd0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
+00013de0: 205f 4f70 4d75 6c74 5465 726d 293a 0a20   _OpMultTerm):. 
+00013df0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00013e00: 6e20 7365 6c66 2e74 6572 6d73 203d 3d20  n self.terms == 
+00013e10: 6f74 6865 722e 7465 726d 730a 2020 2020  other.terms.    
+00013e20: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00013e30: 0a0a 2020 2020 6465 6620 5f5f 6e65 5f5f  ..    def __ne__
+00013e40: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+00013e50: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
+00013e60: 7420 7365 6c66 2e5f 5f65 715f 5f28 6f74  t self.__eq__(ot
+00013e70: 6865 7229 0a0a 2020 2020 6465 6620 5f5f  her)..    def __
+00013e80: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
+00013e90: 2020 2020 2020 7265 7475 726e 2022 4469        return "Di
+00013ea0: 6d2e 5f4f 704d 756c 7454 6572 6d28 2572  m._OpMultTerm(%r
+00013eb0: 2922 2025 2028 7365 6c66 2e74 6572 6d73  )" % (self.terms
+00013ec0: 2c29 0a0a 2020 2020 4070 726f 7065 7274  ,)..    @propert
+00013ed0: 790a 2020 2020 6465 6620 6469 6d65 6e73  y.    def dimens
+00013ee0: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
+00013ef0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00013f00: 7274 7970 653a 2069 6e74 7c4e 6f6e 650a  rtype: int|None.
+00013f10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013f20: 2020 2020 6469 6d20 3d20 310a 2020 2020      dim = 1.    
+00013f30: 2020 2020 666f 7220 7061 7274 2069 6e20      for part in 
+00013f40: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
+00013f50: 2020 2020 2020 2020 6966 2070 6172 742e          if part.
+00013f60: 6469 6d65 6e73 696f 6e20 6973 204e 6f6e  dimension is Non
+00013f70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00013f80: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00013f90: 2020 2020 2020 2020 2020 2064 696d 202a             dim *
+00013fa0: 3d20 7061 7274 2e64 696d 656e 7369 6f6e  = part.dimension
+00013fb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013fc0: 6469 6d0a 0a20 2020 2064 6566 2062 6173  dim..    def bas
+00013fd0: 655f 7465 726d 2873 656c 6629 3a0a 2020  e_term(self):.  
+00013fe0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013ff0: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
+00014000: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00014010: 2020 6173 7365 7274 2073 656c 662e 7465    assert self.te
+00014020: 726d 730a 2020 2020 2020 2020 7265 7475  rms.        retu
+00014030: 726e 2073 656c 662e 7465 726d 735b 2d31  rn self.terms[-1
+00014040: 5d0a 0a20 2020 2064 6566 2069 735f 6f6e  ]..    def is_on
+00014050: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00014060: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+00014070: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00014080: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00014090: 7475 726e 206e 6f74 2073 656c 662e 7465  turn not self.te
+000140a0: 726d 730a 0a20 2020 2064 6566 2069 735f  rms..    def is_
+000140b0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+000140c0: 6469 6d28 7365 6c66 293a 0a20 2020 2020  dim(self):.     
+000140d0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+000140e0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+000140f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014100: 6966 206e 6f74 2073 656c 662e 7465 726d  if not self.term
+00014110: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+00014120: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00014130: 2020 2072 6574 7572 6e20 616c 6c28 7465     return all(te
+00014140: 726d 2e69 735f 636f 6e73 7461 6e74 5f73  rm.is_constant_s
+00014150: 7461 7469 635f 6469 6d28 2920 666f 7220  tatic_dim() for 
+00014160: 7465 726d 2069 6e20 7365 6c66 2e74 6572  term in self.ter
+00014170: 6d73 290a 0a20 2020 2064 6566 2063 6f70  ms)..    def cop
+00014180: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
+00014190: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+000141a0: 7970 653a 2044 696d 2e5f 4f70 4d75 6c74  ype: Dim._OpMult
+000141b0: 5465 726d 0a20 2020 2020 2020 2022 2222  Term.        """
+000141c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000141d0: 5f4f 704d 756c 7454 6572 6d28 6c69 7374  _OpMultTerm(list
+000141e0: 2873 656c 662e 7465 726d 7329 290a 0a20  (self.terms)).. 
+000141f0: 2020 2064 6566 206e 6567 6174 6976 6528     def negative(
+00014200: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00014210: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
+00014220: 653a 2044 696d 2e5f 4f70 4d75 6c74 5465  e: Dim._OpMultTe
+00014230: 726d 0a20 2020 2020 2020 2022 2222 0a20  rm.        """. 
+00014240: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00014250: 6572 6d73 2061 6e64 2073 656c 662e 7465  erms and self.te
+00014260: 726d 735b 305d 2e69 735f 636f 6e73 7461  rms[0].is_consta
+00014270: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
+00014280: 616e 6420 7365 6c66 2e74 6572 6d73 5b30  and self.terms[0
+00014290: 5d2e 6469 6d65 6e73 696f 6e20 3d3d 202d  ].dimension == -
+000142a0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
+000142b0: 6574 7572 6e20 5f4f 704d 756c 7454 6572  eturn _OpMultTer
+000142c0: 6d28 7365 6c66 2e74 6572 6d73 5b31 3a5d  m(self.terms[1:]
+000142d0: 290a 2020 2020 2020 2020 7265 7320 3d20  ).        res = 
+000142e0: 7365 6c66 2e63 6f70 7928 290a 2020 2020  self.copy().    
+000142f0: 2020 2020 7265 732e 6578 7465 6e64 5f6d      res.extend_m
+00014300: 756c 5f64 6976 5f28 5f6d 616b 655f 636f  ul_div_(_make_co
+00014310: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
+00014320: 6d28 2d31 292c 206b 696e 643d 226d 756c  m(-1), kind="mul
+00014330: 222c 2072 6967 6874 3d46 616c 7365 290a  ", right=False).
+00014340: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00014350: 6573 0a0a 2020 2020 6465 6620 6469 7669  es..    def divi
+00014360: 7369 626c 6528 7365 6c66 2c20 6f74 6865  sible(self, othe
+00014370: 722c 2072 6967 6874 293a 0a20 2020 2020  r, right):.     
+00014380: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00014390: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
+000143a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000143b0: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
+000143c0: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
+000143d0: 7468 6572 2077 6520 6361 6e20 6469 7669  ther we can divi
+000143e0: 6465 206f 7468 6572 2c20 7769 7468 6f75  de other, withou
+000143f0: 7420 7265 6d61 696e 6465 720a 2020 2020  t remainder.    
+00014400: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00014410: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014420: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00014430: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00014440: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00014450: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
+00014460: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00014470: 7020 616e 6420 6f74 6865 722e 6465 7269  p and other.deri
+00014480: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+00014490: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
+000144a0: 2020 2020 2020 2074 6d70 203d 2073 656c         tmp = sel
+000144b0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+000144c0: 2020 2020 2066 6f72 2074 6572 6d20 696e       for term in
+000144d0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
+000144e0: 726f 6d5f 6f70 2e69 6e70 7574 7320 6966  rom_op.inputs if
+000144f0: 2072 6967 6874 2065 6c73 6520 7265 7665   right else reve
+00014500: 7273 6564 286f 7468 6572 2e64 6572 6976  rsed(other.deriv
+00014510: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
+00014520: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00014530: 2020 2020 6966 206e 6f74 2074 6d70 2e64      if not tmp.d
+00014540: 6976 6973 6962 6c65 2874 6572 6d2c 2072  ivisible(term, r
+00014550: 6967 6874 3d72 6967 6874 293a 0a20 2020  ight=right):.   
+00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014570: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00014580: 2020 2020 2020 2020 2020 2020 2020 746d                tm
+00014590: 702e 6578 7465 6e64 5f6d 756c 5f64 6976  p.extend_mul_div
+000145a0: 5f28 7465 726d 2c20 6b69 6e64 3d22 7472  _(term, kind="tr
+000145b0: 7565 6469 7622 2c20 7269 6768 743d 7269  uediv", right=ri
+000145c0: 6768 7429 0a20 2020 2020 2020 2020 2020  ght).           
+000145d0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+000145e0: 2020 2020 206d 6f73 745f 7265 6365 6e74       most_recent
+000145f0: 5f74 6572 6d20 3d20 7365 6c66 2e74 6572  _term = self.ter
+00014600: 6d73 5b2d 3120 6966 2072 6967 6874 2065  ms[-1 if right e
+00014610: 6c73 6520 305d 0a20 2020 2020 2020 2069  lse 0].        i
+00014620: 6620 6f74 6865 7220 3d3d 206d 6f73 745f  f other == most_
+00014630: 7265 6365 6e74 5f74 6572 6d3a 0a20 2020  recent_term:.   
+00014640: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00014650: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
+00014660: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
+00014670: 2e64 696d 656e 7369 6f6e 2069 7320 6e6f  .dimension is no
+00014680: 7420 4e6f 6e65 2061 6e64 206f 7468 6572  t None and other
+00014690: 2e64 696d 656e 7369 6f6e 2069 7320 6e6f  .dimension is no
+000146a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000146b0: 2020 2020 6966 206d 6f73 745f 7265 6365      if most_rece
+000146c0: 6e74 5f74 6572 6d2e 6469 6d65 6e73 696f  nt_term.dimensio
+000146d0: 6e20 2520 6f74 6865 722e 6469 6d65 6e73  n % other.dimens
+000146e0: 696f 6e20 3d3d 2030 3a0a 2020 2020 2020  ion == 0:.      
+000146f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014700: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
+00014710: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+00014720: 6465 6620 6361 6e5f 7369 6d70 6c69 6679  def can_simplify
+00014730: 2873 656c 662c 206f 7468 6572 2c20 6b69  (self, other, ki
+00014740: 6e64 2c20 7269 6768 7429 3a0a 2020 2020  nd, right):.    
+00014750: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014760: 3a70 6172 616d 2044 696d 206f 7468 6572  :param Dim other
+00014770: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00014780: 2073 7472 206b 696e 643a 0a20 2020 2020   str kind:.     
+00014790: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
+000147a0: 6967 6874 3a0a 2020 2020 2020 2020 3a72  ight:.        :r
+000147b0: 6574 7572 6e3a 2077 6865 7468 6572 2077  eturn: whether w
+000147c0: 6520 6361 6e20 7369 6d70 6c69 6679 2077  e can simplify w
+000147d0: 6865 6e20 6170 706c 7969 6e67 2074 6869  hen applying thi
+000147e0: 7320 6f70 6572 6174 696f 6e0a 2020 2020  s operation.    
+000147f0: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00014800: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014810: 2020 2020 2069 6620 6f74 6865 722e 6465       if other.de
+00014820: 7269 7665 645f 6672 6f6d 5f6f 7020 616e  rived_from_op an
+00014830: 6420 6f74 6865 722e 6465 7269 7665 645f  d other.derived_
+00014840: 6672 6f6d 5f6f 702e 6b69 6e64 203d 3d20  from_op.kind == 
+00014850: 226d 756c 223a 0a20 2020 2020 2020 2020  "mul":.         
+00014860: 2020 2074 6d70 203d 2073 656c 662e 636f     tmp = self.co
+00014870: 7079 2829 0a20 2020 2020 2020 2020 2020  py().           
+00014880: 2066 6f72 2074 6572 6d20 696e 206f 7468   for term in oth
+00014890: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
+000148a0: 6f70 2e69 6e70 7574 7320 6966 2072 6967  op.inputs if rig
+000148b0: 6874 2065 6c73 6520 7265 7665 7273 6564  ht else reversed
+000148c0: 286f 7468 6572 2e64 6572 6976 6564 5f66  (other.derived_f
+000148d0: 726f 6d5f 6f70 2e69 6e70 7574 7329 3a0a  rom_op.inputs):.
+000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148f0: 6966 206e 6f74 2074 6d70 2e63 616e 5f73  if not tmp.can_s
+00014900: 696d 706c 6966 7928 7465 726d 2c20 6b69  implify(term, ki
+00014910: 6e64 3d6b 696e 642c 2072 6967 6874 3d72  nd=kind, right=r
+00014920: 6967 6874 293a 0a20 2020 2020 2020 2020  ight):.         
+00014930: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00014940: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00014950: 2020 2020 2020 2020 746d 702e 6578 7465          tmp.exte
+00014960: 6e64 5f6d 756c 5f64 6976 5f28 7465 726d  nd_mul_div_(term
+00014970: 2c20 6b69 6e64 3d6b 696e 642c 2072 6967  , kind=kind, rig
+00014980: 6874 3d72 6967 6874 290a 2020 2020 2020  ht=right).      
+00014990: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+000149a0: 650a 2020 2020 2020 2020 6964 7820 3d20  e.        idx = 
+000149b0: 7365 6c66 2e5f 7369 6d70 6c69 6679 5f74  self._simplify_t
+000149c0: 6572 6d5f 6964 7828 6f74 6865 722c 206b  erm_idx(other, k
+000149d0: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
+000149e0: 7269 6768 7429 0a20 2020 2020 2020 2072  right).        r
+000149f0: 6574 7572 6e20 6964 7820 6973 206e 6f74  eturn idx is not
+00014a00: 204e 6f6e 650a 0a20 2020 2064 6566 205f   None..    def _
+00014a10: 7369 6d70 6c69 6679 5f74 6572 6d5f 6964  simplify_term_id
+00014a20: 7828 7365 6c66 2c20 6f74 6865 722c 206b  x(self, other, k
+00014a30: 696e 642c 2072 6967 6874 293a 0a20 2020  ind, right):.   
+00014a40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014a50: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
+00014a60: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
+00014a70: 6d20 7374 7220 6b69 6e64 3a0a 2020 2020  m str kind:.    
+00014a80: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+00014a90: 7269 6768 743a 0a20 2020 2020 2020 203a  right:.        :
+00014aa0: 7265 7475 726e 3a20 696e 6465 7820 6f66  return: index of
+00014ab0: 2074 6572 6d20 746f 2073 696d 706c 6966   term to simplif
+00014ac0: 790a 2020 2020 2020 2020 3a72 7479 7065  y.        :rtype
+00014ad0: 3a20 696e 747c 4e6f 6e65 0a20 2020 2020  : int|None.     
+00014ae0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00014af0: 6620 6e6f 7420 7365 6c66 2e74 6572 6d73  f not self.terms
+00014b00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00014b10: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
+00014b20: 2020 6966 206b 696e 6420 3d3d 2022 6d75    if kind == "mu
+00014b30: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+00014b40: 2320 5765 2077 616e 7420 2862 202a 2061  # We want (b * a
+00014b50: 2920 2f2f 2062 2021 3d20 612e 0a20 2020  ) // b != a..   
+00014b60: 2020 2020 2020 2020 2023 2048 6f77 6576           # Howev
+00014b70: 6572 2c20 7765 2077 616e 7420 6820 2a20  er, we want h * 
+00014b80: 2832 202a 2061 202f 2f20 6829 203d 3d20  (2 * a // h) == 
+00014b90: 3220 2a20 612e 0a20 2020 2020 2020 2020  2 * a..         
+00014ba0: 2020 2023 2053 6f2c 2066 6f72 2060 6d75     # So, for `mu
+00014bb0: 6c60 2c20 616e 6420 6f6e 6c79 2066 6f72  l`, and only for
+00014bc0: 2060 6d75 6c60 2c20 6368 6563 6b20 616c   `mul`, check al
+00014bd0: 6c20 7465 726d 732c 2077 6865 7468 6572  l terms, whether
+00014be0: 2077 6520 6361 6e20 7369 6d70 6c69 6679   we can simplify
+00014bf0: 2073 6f6d 6520 6469 7669 7369 6f6e 2d74   some division-t
+00014c00: 6572 6d2e 0a20 2020 2020 2020 2020 2020  erm..           
+00014c10: 2066 6f72 2069 2c20 7465 726d 2069 6e20   for i, term in 
+00014c20: 7265 7665 7273 6564 286c 6973 7428 656e  reversed(list(en
+00014c30: 756d 6572 6174 6528 7365 6c66 2e74 6572  umerate(self.ter
+00014c40: 6d73 2929 2920 6966 2072 6967 6874 2065  ms))) if right e
+00014c50: 6c73 6520 656e 756d 6572 6174 6528 7365  lse enumerate(se
+00014c60: 6c66 2e74 6572 6d73 293a 0a20 2020 2020  lf.terms):.     
+00014c70: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00014c80: 7420 6973 696e 7374 616e 6365 2874 6572  t isinstance(ter
+00014c90: 6d2c 205f 642e 4469 6d29 0a20 2020 2020  m, _d.Dim).     
+00014ca0: 2020 2020 2020 2020 2020 2069 6620 7465             if te
+00014cb0: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
+00014cc0: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+00014cd0: 2020 2020 2020 2020 6966 2074 6572 6d2e          if term.
+00014ce0: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00014cf0: 6b69 6e64 203d 3d20 2274 7275 6564 6976  kind == "truediv
+00014d00: 5f22 202b 2028 2272 6967 6874 2220 6966  _" + ("right" if
+00014d10: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
+00014d20: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
+00014d30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014d40: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
+00014d50: 6d5f 6f70 2e69 6e70 7574 735b 2d31 5d20  m_op.inputs[-1] 
+00014d60: 3d3d 206f 7468 6572 3a0a 2020 2020 2020  == other:.      
+00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d80: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
+00014d90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014da0: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
+00014db0: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
+00014dc0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014dd0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00014de0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
+00014df0: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
+00014e00: 6874 2220 6966 206e 6f74 2072 6967 6874  ht" if not right
+00014e10: 2065 6c73 6520 226c 6566 7422 293a 0a20   else "left"):. 
+00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e30: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
+00014e40: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00014e50: 696e 7075 7473 5b2d 315d 203d 3d20 7465  inputs[-1] == te
+00014e60: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
+00014e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e80: 7265 7475 726e 2069 0a20 2020 2020 2020  return i.       
+00014e90: 2020 2020 2020 2020 2069 6620 7465 726d           if term
+00014ea0: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
+00014eb0: 7469 635f 6469 6d28 2920 616e 6420 6f74  tic_dim() and ot
+00014ec0: 6865 722e 6973 5f63 6f6e 7374 616e 745f  her.is_constant_
+00014ed0: 7374 6174 6963 5f64 696d 2829 3a0a 2020  static_dim():.  
+00014ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ef0: 2020 7265 7475 726e 2069 0a20 2020 2020    return i.     
+00014f00: 2020 2023 2046 6f72 2074 6865 206c 6173     # For the las
+00014f10: 742f 6669 7273 7420 7465 726d 2c20 6578  t/first term, ex
+00014f20: 7472 6120 6368 6563 6b73 2e0a 2020 2020  tra checks..    
+00014f30: 2020 2020 6920 3d20 6c65 6e28 7365 6c66      i = len(self
+00014f40: 2e74 6572 6d73 2920 2d20 3120 6966 2072  .terms) - 1 if r
+00014f50: 6967 6874 2065 6c73 6520 300a 2020 2020  ight else 0.    
+00014f60: 2020 2020 7465 726d 203d 2073 656c 662e      term = self.
+00014f70: 7465 726d 735b 695d 0a20 2020 2020 2020  terms[i].       
+00014f80: 2069 6620 6b69 6e64 2e65 6e64 7377 6974   if kind.endswit
+00014f90: 6828 2264 6976 2229 2061 6e64 206f 7468  h("div") and oth
+00014fa0: 6572 203d 3d20 7465 726d 3a0a 2020 2020  er == term:.    
+00014fb0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00014fc0: 0a20 2020 2020 2020 206f 705f 6b69 6e64  .        op_kind
+00014fd0: 203d 206b 696e 6420 2b20 225f 2220 2b20   = kind + "_" + 
+00014fe0: 2822 7269 6768 7422 2069 6620 7269 6768  ("right" if righ
+00014ff0: 7420 656c 7365 2022 6c65 6674 2229 0a20  t else "left"). 
+00015000: 2020 2020 2020 2069 6620 7465 726d 2e64         if term.d
+00015010: 6572 6976 6564 5f66 726f 6d5f 6f70 2061  erived_from_op a
+00015020: 6e64 2074 6572 6d2e 6465 7269 7665 645f  nd term.derived_
+00015030: 6672 6f6d 5f6f 702e 6b69 6e64 203d 3d20  from_op.kind == 
+00015040: 6f70 5f6b 696e 643a 0a20 2020 2020 2020  op_kind:.       
+00015050: 2020 2020 2072 6574 7572 6e20 690a 2020       return i.  
+00015060: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00015070: 650a 0a20 2020 2064 6566 2065 7874 656e  e..    def exten
+00015080: 645f 6d75 6c5f 6469 765f 2873 656c 662c  d_mul_div_(self,
+00015090: 206f 7468 6572 2c20 6b69 6e64 2c20 7269   other, kind, ri
+000150a0: 6768 7429 3a0a 2020 2020 2020 2020 2222  ght):.        ""
+000150b0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+000150c0: 2044 696d 206f 7468 6572 3a0a 2020 2020   Dim other:.    
+000150d0: 2020 2020 3a70 6172 616d 2073 7472 206b      :param str k
+000150e0: 696e 643a 0a20 2020 2020 2020 203a 7061  ind:.        :pa
+000150f0: 7261 6d20 626f 6f6c 2072 6967 6874 3a0a  ram bool right:.
+00015100: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015110: 2020 2020 6173 7365 7274 206b 696e 6420      assert kind 
+00015120: 696e 207b 226d 756c 222c 2022 666c 6f6f  in {"mul", "floo
+00015130: 7264 6976 222c 2022 7472 7565 6469 7622  rdiv", "truediv"
+00015140: 2c20 2263 6569 6c64 6976 227d 0a20 2020  , "ceildiv"}.   
+00015150: 2020 2020 2069 6620 6f74 6865 722e 6973       if other.is
+00015160: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+00015170: 5f64 696d 2829 2061 6e64 206f 7468 6572  _dim() and other
+00015180: 2e64 696d 656e 7369 6f6e 203d 3d20 313a  .dimension == 1:
+00015190: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000151a0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
+000151b0: 6f74 2073 656c 662e 7465 726d 733a 0a20  ot self.terms:. 
+000151c0: 2020 2020 2020 2020 2020 2069 6620 6b69             if ki
+000151d0: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
+000151e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000151f0: 662e 7465 726d 732e 6170 7065 6e64 286f  f.terms.append(o
+00015200: 7468 6572 290a 2020 2020 2020 2020 2020  ther).          
+00015210: 2020 656c 6966 206b 696e 642e 656e 6473    elif kind.ends
+00015220: 7769 7468 2822 6469 7622 293a 0a20 2020  with("div"):.   
+00015230: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015240: 662e 7465 726d 7320 3d20 5b5f 4f70 4d75  f.terms = [_OpMu
+00015250: 6c74 5465 726d 2e6e 6577 5f64 6976 5f64  ltTerm.new_div_d
+00015260: 696d 2873 656c 662e 6173 5f64 696d 2829  im(self.as_dim()
+00015270: 2c20 6f74 6865 722c 206b 696e 643d 6b69  , other, kind=ki
+00015280: 6e64 2c20 7269 6768 743d 7269 6768 7429  nd, right=right)
+00015290: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
+000152a0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+000152b0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+000152c0: 6f6d 5f6f 7020 616e 6420 6f74 6865 722e  om_op and other.
+000152d0: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+000152e0: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
+000152f0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+00015300: 6572 6d20 696e 206f 7468 6572 2e64 6572  erm in other.der
+00015310: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
+00015320: 7574 7320 6966 2072 6967 6874 2065 6c73  uts if right els
+00015330: 6520 7265 7665 7273 6564 286f 7468 6572  e reversed(other
+00015340: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015350: 2e69 6e70 7574 7329 3a0a 2020 2020 2020  .inputs):.      
+00015360: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+00015370: 7874 656e 645f 6d75 6c5f 6469 765f 2874  xtend_mul_div_(t
+00015380: 6572 6d2c 206b 696e 643d 6b69 6e64 2c20  erm, kind=kind, 
+00015390: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
+000153a0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000153b0: 2020 2020 2020 2020 6964 7820 3d20 7365          idx = se
+000153c0: 6c66 2e5f 7369 6d70 6c69 6679 5f74 6572  lf._simplify_ter
+000153d0: 6d5f 6964 7828 6f74 6865 722c 206b 696e  m_idx(other, kin
+000153e0: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
+000153f0: 6768 7429 0a20 2020 2020 2020 2069 6620  ght).        if 
+00015400: 6964 7820 6973 206e 6f74 204e 6f6e 653a  idx is not None:
+00015410: 0a20 2020 2020 2020 2020 2020 2074 6572  .            ter
+00015420: 6d20 3d20 7365 6c66 2e74 6572 6d73 5b69  m = self.terms[i
+00015430: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
+00015440: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+00015450: 6528 7465 726d 2c20 5f64 2e44 696d 290a  e(term, _d.Dim).
+00015460: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00015470: 696e 642e 656e 6473 7769 7468 2822 6469  ind.endswith("di
+00015480: 7622 2920 616e 6420 6f74 6865 7220 3d3d  v") and other ==
+00015490: 2074 6572 6d3a 0a20 2020 2020 2020 2020   term:.         
+000154a0: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
+000154b0: 732e 706f 7028 6964 7829 0a20 2020 2020  s.pop(idx).     
+000154c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000154d0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+000154e0: 206b 696e 6420 3d3d 2022 6d75 6c22 2061   kind == "mul" a
+000154f0: 6e64 2074 6572 6d2e 6465 7269 7665 645f  nd term.derived_
+00015500: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
+00015510: 2020 2020 2020 2020 2069 6620 7465 726d           if term
+00015520: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015530: 2e6b 696e 6420 3d3d 2022 7472 7565 6469  .kind == "truedi
+00015540: 765f 2220 2b20 2822 7269 6768 7422 2069  v_" + ("right" i
+00015550: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
+00015560: 6674 2229 3a0a 2020 2020 2020 2020 2020  ft"):.          
+00015570: 2020 2020 2020 2020 2020 6966 2074 6572            if ter
+00015580: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
+00015590: 702e 696e 7075 7473 5b2d 315d 203d 3d20  p.inputs[-1] == 
+000155a0: 6f74 6865 723a 0a20 2020 2020 2020 2020  other:.         
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000155c0: 656c 662e 7465 726d 735b 6964 785d 203d  elf.terms[idx] =
+000155d0: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
+000155e0: 6f6d 5f6f 702e 696e 7075 7473 5b30 5d0a  om_op.inputs[0].
+000155f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015600: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00015610: 2020 2020 2020 2020 2020 2069 6620 6b69             if ki
+00015620: 6e64 203d 3d20 226d 756c 2220 616e 6420  nd == "mul" and 
+00015630: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00015640: 6f6d 5f6f 703a 0a20 2020 2020 2020 2020  om_op:.         
+00015650: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
+00015660: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00015670: 6b69 6e64 203d 3d20 2274 7275 6564 6976  kind == "truediv
+00015680: 5f22 202b 2028 2272 6967 6874 2220 6966  _" + ("right" if
+00015690: 206e 6f74 2072 6967 6874 2065 6c73 6520   not right else 
+000156a0: 226c 6566 7422 293a 0a20 2020 2020 2020  "left"):.       
+000156b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000156c0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+000156d0: 6f6d 5f6f 702e 696e 7075 7473 5b2d 315d  om_op.inputs[-1]
+000156e0: 203d 3d20 7465 726d 3a0a 2020 2020 2020   == term:.      
+000156f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015700: 2020 7365 6c66 2e74 6572 6d73 5b69 6478    self.terms[idx
+00015710: 5d20 3d20 6f74 6865 722e 6465 7269 7665  ] = other.derive
+00015720: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
+00015730: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00015740: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015750: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+00015760: 6620 7465 726d 2e69 735f 636f 6e73 7461  f term.is_consta
+00015770: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
+00015780: 616e 6420 6f74 6865 722e 6973 5f63 6f6e  and other.is_con
+00015790: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
+000157a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000157b0: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
+000157c0: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
+000157d0: 2020 2020 2020 2020 2020 6966 2074 6572            if ter
+000157e0: 6d2e 6469 6d65 6e73 696f 6e20 2a20 6f74  m.dimension * ot
+000157f0: 6865 722e 6469 6d65 6e73 696f 6e20 3d3d  her.dimension ==
+00015800: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00015810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015820: 2e74 6572 6d73 2e70 6f70 2869 6478 290a  .terms.pop(idx).
+00015830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015840: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00015850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015860: 2020 2073 656c 662e 7465 726d 735b 6964     self.terms[id
+00015870: 785d 203d 205f 6d61 6b65 5f63 6f6e 7374  x] = _make_const
+00015880: 616e 745f 7374 6174 6963 5f64 696d 2874  ant_static_dim(t
+00015890: 6572 6d2e 6469 6d65 6e73 696f 6e20 2a20  erm.dimension * 
+000158a0: 6f74 6865 722e 6469 6d65 6e73 696f 6e2c  other.dimension,
+000158b0: 206b 696e 643d 7465 726d 2e6b 696e 6429   kind=term.kind)
+000158c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000158d0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+000158e0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+000158f0: 696e 642e 656e 6473 7769 7468 2822 6469  ind.endswith("di
+00015900: 7622 2920 616e 6420 7465 726d 2e64 696d  v") and term.dim
+00015910: 656e 7369 6f6e 2025 206f 7468 6572 2e64  ension % other.d
+00015920: 696d 656e 7369 6f6e 203d 3d20 303a 0a20  imension == 0:. 
+00015930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015940: 2020 2073 656c 662e 7465 726d 735b 6964     self.terms[id
+00015950: 785d 203d 205f 6d61 6b65 5f63 6f6e 7374  x] = _make_const
+00015960: 616e 745f 7374 6174 6963 5f64 696d 2874  ant_static_dim(t
+00015970: 6572 6d2e 6469 6d65 6e73 696f 6e20 2f2f  erm.dimension //
+00015980: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
+00015990: 2c20 6b69 6e64 3d74 6572 6d2e 6b69 6e64  , kind=term.kind
+000159a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000159b0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000159c0: 2020 2020 2020 2020 2020 2020 2023 2046               # F
+000159d0: 616c 6c62 6163 6b20 7769 7468 2067 656e  allback with gen
+000159e0: 6572 6963 2068 616e 646c 696e 672e 0a20  eric handling.. 
+000159f0: 2020 2020 2020 2020 2020 206f 705f 6b69             op_ki
+00015a00: 6e64 203d 206b 696e 6420 2b20 225f 2220  nd = kind + "_" 
+00015a10: 2b20 2822 7269 6768 7422 2069 6620 7269  + ("right" if ri
+00015a20: 6768 7420 656c 7365 2022 6c65 6674 2229  ght else "left")
+00015a30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00015a40: 6b69 6e64 2e65 6e64 7377 6974 6828 2264  kind.endswith("d
+00015a50: 6976 2229 2061 6e64 2074 6572 6d2e 6465  iv") and term.de
+00015a60: 7269 7665 645f 6672 6f6d 5f6f 7020 616e  rived_from_op an
+00015a70: 6420 7465 726d 2e64 6572 6976 6564 5f66  d term.derived_f
+00015a80: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 206f  rom_op.kind == o
+00015a90: 705f 6b69 6e64 3a0a 2020 2020 2020 2020  p_kind:.        
+00015aa0: 2020 2020 2020 2020 6e75 6d65 7261 746f          numerato
+00015ab0: 7220 3d20 7465 726d 2e64 6572 6976 6564  r = term.derived
+00015ac0: 5f66 726f 6d5f 6f70 2e69 6e70 7574 735b  _from_op.inputs[
+00015ad0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+00015ae0: 2020 2064 656e 6f6d 696e 6174 6f72 203d     denominator =
+00015af0: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
+00015b00: 6f6d 5f6f 702e 696e 7075 7473 5b31 5d0a  om_op.inputs[1].
+00015b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b20: 7365 6c66 2e74 6572 6d73 5b69 6478 5d20  self.terms[idx] 
+00015b30: 3d20 5f4f 704d 756c 7454 6572 6d2e 6e65  = _OpMultTerm.ne
+00015b40: 775f 6469 765f 6469 6d28 6e75 6d65 7261  w_div_dim(numera
+00015b50: 746f 722c 2064 656e 6f6d 696e 6174 6f72  tor, denominator
+00015b60: 202a 206f 7468 6572 2c20 6b69 6e64 3d6b   * other, kind=k
+00015b70: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
+00015b80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015b90: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00015ba0: 2069 6620 6b69 6e64 2e65 6e64 7377 6974   if kind.endswit
+00015bb0: 6828 2264 6976 2229 3a0a 2020 2020 2020  h("div"):.      
+00015bc0: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
+00015bd0: 203d 205b 5f4f 704d 756c 7454 6572 6d2e   = [_OpMultTerm.
+00015be0: 6e65 775f 6469 765f 6469 6d28 7365 6c66  new_div_dim(self
+00015bf0: 2e61 735f 6469 6d28 292c 206f 7468 6572  .as_dim(), other
+00015c00: 2c20 6b69 6e64 3d6b 696e 642c 2072 6967  , kind=kind, rig
+00015c10: 6874 3d72 6967 6874 295d 0a20 2020 2020  ht=right)].     
+00015c20: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00015c30: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
+00015c40: 2022 6d75 6c22 3a0a 2020 2020 2020 2020   "mul":.        
+00015c50: 2020 2020 6966 2072 6967 6874 3a0a 2020      if right:.  
+00015c60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015c70: 6c66 2e74 6572 6d73 2e61 7070 656e 6428  lf.terms.append(
+00015c80: 6f74 6865 7229 0a20 2020 2020 2020 2020  other).         
+00015c90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00015ca0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00015cb0: 726d 732e 696e 7365 7274 2830 2c20 6f74  rms.insert(0, ot
+00015cc0: 6865 7229 0a20 2020 2020 2020 2020 2020  her).           
+00015cd0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00015ce0: 6173 7365 7274 2046 616c 7365 0a0a 2020  assert False..  
+00015cf0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00015d00: 2020 2064 6566 206e 6577 5f64 6976 5f64     def new_div_d
+00015d10: 696d 2863 6c73 2c20 6e75 6d65 7261 746f  im(cls, numerato
+00015d20: 722c 2064 656e 6f6d 696e 6174 6f72 2c20  r, denominator, 
+00015d30: 6b69 6e64 2c20 7269 6768 7429 3a0a 2020  kind, right):.  
+00015d40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015d50: 2020 3a70 6172 616d 2044 696d 206e 756d    :param Dim num
+00015d60: 6572 6174 6f72 3a0a 2020 2020 2020 2020  erator:.        
+00015d70: 3a70 6172 616d 2044 696d 2064 656e 6f6d  :param Dim denom
+00015d80: 696e 6174 6f72 3a0a 2020 2020 2020 2020  inator:.        
+00015d90: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
+00015da0: 2022 666c 6f6f 7264 6976 2220 6f72 2022   "floordiv" or "
+00015db0: 6365 696c 6469 7622 206f 7220 2274 7275  ceildiv" or "tru
+00015dc0: 6564 6976 220a 2020 2020 2020 2020 3a70  ediv".        :p
+00015dd0: 6172 616d 2062 6f6f 6c20 7269 6768 743a  aram bool right:
+00015de0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00015df0: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00015e00: 0a20 2020 2020 2020 2064 696d 5f76 616c  .        dim_val
+00015e10: 7565 203d 204e 6f6e 650a 2020 2020 2020  ue = None.      
+00015e20: 2020 6120 3d20 6e75 6d65 7261 746f 722e    a = numerator.
+00015e30: 6469 6d65 6e73 696f 6e0a 2020 2020 2020  dimension.      
+00015e40: 2020 6220 3d20 6465 6e6f 6d69 6e61 746f    b = denominato
+00015e50: 722e 6469 6d65 6e73 696f 6e0a 2020 2020  r.dimension.    
+00015e60: 2020 2020 6966 2061 2069 7320 6e6f 7420      if a is not 
+00015e70: 4e6f 6e65 2061 6e64 2062 2069 7320 6e6f  None and b is no
+00015e80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00015e90: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
+00015ea0: 666c 6f6f 7264 6976 223a 0a20 2020 2020  floordiv":.     
+00015eb0: 2020 2020 2020 2020 2020 2064 696d 5f76             dim_v
+00015ec0: 616c 7565 203d 2061 202f 2f20 620a 2020  alue = a // b.  
+00015ed0: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
+00015ee0: 696e 6420 3d3d 2022 6365 696c 6469 7622  ind == "ceildiv"
+00015ef0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015f00: 2020 6469 6d5f 7661 6c75 6520 3d20 2d28    dim_value = -(
+00015f10: 2d61 202f 2f20 6229 0a20 2020 2020 2020  -a // b).       
+00015f20: 2020 2020 2020 2020 2069 6620 6120 2520           if a % 
+00015f30: 6220 3d3d 2030 2061 6e64 2072 6967 6874  b == 0 and right
+00015f40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015f50: 2020 2020 2020 6b69 6e64 203d 2022 666c        kind = "fl
+00015f60: 6f6f 7264 6976 2220 2023 2066 6f72 206e  oordiv"  # for n
+00015f70: 6963 6572 2064 6573 6372 6970 7469 6f6e  icer description
+00015f80: 2c20 616e 6420 646f 6573 206e 6f74 206d  , and does not m
+00015f90: 6174 7465 720a 2020 2020 2020 2020 2020  atter.          
+00015fa0: 2020 656c 6966 206b 696e 6420 3d3d 2022    elif kind == "
+00015fb0: 7472 7565 6469 7622 3a0a 2020 2020 2020  truediv":.      
+00015fc0: 2020 2020 2020 2020 2020 6966 2061 2025            if a %
+00015fd0: 2062 2021 3d20 303a 0a20 2020 2020 2020   b != 0:.       
+00015fe0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00015ff0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00016000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016010: 2020 2020 2020 2022 2573 2074 7275 6564         "%s trued
+00016020: 6976 2025 7320 6f6e 6c79 2061 6c6c 6f77  iv %s only allow
+00016030: 6564 2069 6620 7468 6520 7265 7375 6c74  ed if the result
+00016040: 2069 7320 616e 2069 6e74 6567 6572 2220   is an integer" 
+00016050: 2520 286e 756d 6572 6174 6f72 2c20 6465  % (numerator, de
+00016060: 6e6f 6d69 6e61 746f 7229 0a20 2020 2020  nominator).     
+00016070: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00016080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016090: 2064 696d 5f76 616c 7565 203d 2061 202f   dim_value = a /
+000160a0: 2f20 620a 2020 2020 2020 2020 2020 2020  / b.            
+000160b0: 2020 2020 6966 2072 6967 6874 3a0a 2020      if right:.  
+000160c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160d0: 2020 6b69 6e64 203d 2022 666c 6f6f 7264    kind = "floord
+000160e0: 6976 2220 2023 2066 6f72 206e 6963 6572  iv"  # for nicer
+000160f0: 2064 6573 6372 6970 7469 6f6e 2c20 616e   description, an
+00016100: 6420 646f 6573 206e 6f74 206d 6174 7465  d does not matte
+00016110: 720a 2020 2020 2020 2020 2020 2020 656c  r.            el
+00016120: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00016130: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00016140: 7272 6f72 2822 696e 7661 6c69 6420 6b69  rror("invalid ki
+00016150: 6e64 2025 7222 2025 2028 6b69 6e64 2c29  nd %r" % (kind,)
+00016160: 290a 2020 2020 2020 2020 6966 206b 696e  ).        if kin
+00016170: 6420 3d3d 2022 666c 6f6f 7264 6976 2220  d == "floordiv" 
+00016180: 616e 6420 7269 6768 743a 0a20 2020 2020  and right:.     
+00016190: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+000161a0: 6f6e 203d 2022 2573 2f2f 2573 2220 2520  on = "%s//%s" % 
+000161b0: 285f 6765 745f 6465 7363 7269 7074 696f  (_get_descriptio
+000161c0: 6e28 6e75 6d65 7261 746f 7229 2c20 5f67  n(numerator), _g
+000161d0: 6574 5f64 6573 6372 6970 7469 6f6e 2864  et_description(d
+000161e0: 656e 6f6d 696e 6174 6f72 2929 0a20 2020  enominator)).   
+000161f0: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
+00016200: 3d20 2263 6569 6c64 6976 2220 616e 6420  = "ceildiv" and 
+00016210: 7269 6768 743a 0a20 2020 2020 2020 2020  right:.         
+00016220: 2020 2064 6573 6372 6970 7469 6f6e 203d     description =
+00016230: 2022 e28c 8825 732f 2573 e28c 8922 2025   "...%s/%s..." %
+00016240: 2028 5f67 6574 5f64 6573 6372 6970 7469   (_get_descripti
+00016250: 6f6e 286e 756d 6572 6174 6f72 292c 205f  on(numerator), _
+00016260: 6765 745f 6465 7363 7269 7074 696f 6e28  get_description(
+00016270: 6465 6e6f 6d69 6e61 746f 7229 290a 2020  denominator)).  
+00016280: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00016290: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+000162a0: 696f 6e20 3d20 2225 735f 2573 2825 732c  ion = "%s_%s(%s,
+000162b0: 2025 7329 2220 2520 280a 2020 2020 2020   %s)" % (.      
+000162c0: 2020 2020 2020 2020 2020 6b69 6e64 2c0a            kind,.
+000162d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162e0: 2272 6967 6874 2220 6966 2072 6967 6874  "right" if right
+000162f0: 2065 6c73 6520 226c 6566 7422 2c0a 2020   else "left",.  
+00016300: 2020 2020 2020 2020 2020 2020 2020 5f67                _g
+00016310: 6574 5f64 6573 6372 6970 7469 6f6e 286e  et_description(n
+00016320: 756d 6572 6174 6f72 2c20 6272 6163 6b65  umerator, bracke
+00016330: 7473 3d46 616c 7365 292c 0a20 2020 2020  ts=False),.     
+00016340: 2020 2020 2020 2020 2020 205f 6765 745f             _get_
+00016350: 6465 7363 7269 7074 696f 6e28 6465 6e6f  description(deno
+00016360: 6d69 6e61 746f 722c 2062 7261 636b 6574  minator, bracket
+00016370: 733d 4661 6c73 6529 2c0a 2020 2020 2020  s=False),.      
+00016380: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00016390: 6f70 5f6b 696e 6420 3d20 6b69 6e64 0a20  op_kind = kind. 
+000163a0: 2020 2020 2020 2069 6620 6120 6973 206e         if a is n
+000163b0: 6f74 204e 6f6e 6520 616e 6420 6220 6973  ot None and b is
+000163c0: 206e 6f74 204e 6f6e 6520 616e 6420 6120   not None and a 
+000163d0: 2520 6220 3d3d 2030 3a0a 2020 2020 2020  % b == 0:.      
+000163e0: 2020 2020 2020 6f70 5f6b 696e 6420 3d20        op_kind = 
+000163f0: 2274 7275 6564 6976 2220 2023 206d 616b  "truediv"  # mak
+00016400: 6573 2073 6f6d 6520 6f74 6865 7220 6368  es some other ch
+00016410: 6563 6b73 2073 696d 706c 6572 0a20 2020  ecks simpler.   
+00016420: 2020 2020 206f 705f 6b69 6e64 202b 3d20       op_kind += 
+00016430: 225f 2220 2b20 2822 7269 6768 7422 2069  "_" + ("right" i
+00016440: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
+00016450: 6674 2229 0a20 2020 2020 2020 2072 6574  ft").        ret
+00016460: 7572 6e20 5f64 2e44 696d 280a 2020 2020  urn _d.Dim(.    
+00016470: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00016480: 696f 6e3d 6465 7363 7269 7074 696f 6e2c  ion=description,
+00016490: 0a20 2020 2020 2020 2020 2020 206b 696e  .            kin
+000164a0: 643d 6e75 6d65 7261 746f 722e 6b69 6e64  d=numerator.kind
+000164b0: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+000164c0: 6d65 6e73 696f 6e3d 6469 6d5f 7661 6c75  mension=dim_valu
+000164d0: 652c 0a20 2020 2020 2020 2020 2020 2064  e,.            d
+000164e0: 6572 6976 6564 5f66 726f 6d5f 6f70 3d4f  erived_from_op=O
+000164f0: 7028 6b69 6e64 3d6f 705f 6b69 6e64 2c20  p(kind=op_kind, 
+00016500: 696e 7075 7473 3d5b 6e75 6d65 7261 746f  inputs=[numerato
+00016510: 722c 2064 656e 6f6d 696e 6174 6f72 5d29  r, denominator])
+00016520: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00016530: 7269 7665 645f 6672 6f6d 5f74 6167 3d6e  rived_from_tag=n
+00016540: 756d 6572 6174 6f72 2c0a 2020 2020 2020  umerator,.      
+00016550: 2020 290a 0a20 2020 2064 6566 2061 735f    )..    def as_
+00016560: 6469 6d28 7365 6c66 293a 0a20 2020 2020  dim(self):.     
+00016570: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00016580: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
+00016590: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000165a0: 6620 7365 6c66 2e69 735f 6f6e 6528 293a  f self.is_one():
+000165b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000165c0: 7572 6e20 5f6d 616b 655f 636f 6e73 7461  urn _make_consta
+000165d0: 6e74 5f73 7461 7469 635f 6469 6d28 3129  nt_static_dim(1)
+000165e0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+000165f0: 7365 6c66 2e74 6572 6d73 2920 3d3d 2031  self.terms) == 1
+00016600: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00016610: 7475 726e 2073 656c 662e 7465 726d 735b  turn self.terms[
+00016620: 305d 0a20 2020 2020 2020 2064 696d 5f6b  0].        dim_k
+00016630: 696e 6420 3d20 5f67 6574 5f6d 6572 6765  ind = _get_merge
+00016640: 645f 6469 6d5f 6b69 6e64 2873 656c 662e  d_dim_kind(self.
+00016650: 7465 726d 7329 0a20 2020 2020 2020 2072  terms).        r
+00016660: 6574 7572 6e20 5f64 2e44 696d 280a 2020  eturn _d.Dim(.  
+00016670: 2020 2020 2020 2020 2020 6b69 6e64 3d64            kind=d
+00016680: 696d 5f6b 696e 642c 0a20 2020 2020 2020  im_kind,.       
+00016690: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+000166a0: 3d22 2a22 2e6a 6f69 6e28 6d61 7028 5f67  ="*".join(map(_g
+000166b0: 6574 5f64 6573 6372 6970 7469 6f6e 2c20  et_description, 
+000166c0: 7365 6c66 2e74 6572 6d73 2929 2c0a 2020  self.terms)),.  
+000166d0: 2020 2020 2020 2020 2020 6469 6d65 6e73            dimens
+000166e0: 696f 6e3d 7365 6c66 2e64 696d 656e 7369  ion=self.dimensi
+000166f0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00016700: 6465 7269 7665 645f 6672 6f6d 5f6f 703d  derived_from_op=
+00016710: 4f70 286b 696e 643d 226d 756c 222c 2069  Op(kind="mul", i
+00016720: 6e70 7574 733d 6c69 7374 2873 656c 662e  nputs=list(self.
+00016730: 7465 726d 7329 292c 0a20 2020 2020 2020  terms)),.       
+00016740: 2020 2020 2064 6572 6976 6564 5f66 726f       derived_fro
+00016750: 6d5f 7461 673d 7365 6c66 2e72 6570 7265  m_tag=self.repre
+00016760: 7365 6e74 6174 6976 655f 7461 6728 292c  sentative_tag(),
+00016770: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00016780: 6465 6620 7265 7072 6573 656e 7461 7469  def representati
+00016790: 7665 5f74 6167 2873 656c 6629 3a0a 2020  ve_tag(self):.  
+000167a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000167b0: 2020 3a72 7479 7065 3a20 4469 6d7c 4e6f    :rtype: Dim|No
+000167c0: 6e65 0a20 2020 2020 2020 2022 2222 0a20  ne.        """. 
+000167d0: 2020 2020 2020 2023 2041 6c73 6f20 7365         # Also se
+000167e0: 6520 4469 6d2e 5f4f 704c 696e 6561 7254  e Dim._OpLinearT
+000167f0: 6572 6d2e 7265 7072 6573 656e 7461 7469  erm.representati
+00016800: 7665 5f74 6167 2829 2e0a 2020 2020 2020  ve_tag()..      
+00016810: 2020 2320 4669 7273 7420 6669 6e64 2061    # First find a
+00016820: 6e79 2064 796e 616d 6963 2e0a 2020 2020  ny dynamic..    
+00016830: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
+00016840: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
+00016850: 2020 2020 2020 2020 2069 6620 7465 726d           if term
+00016860: 5f2e 6973 5f64 796e 616d 6963 2829 3a0a  _.is_dynamic():.
+00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016880: 7265 7475 726e 2074 6572 6d5f 0a20 2020  return term_.   
+00016890: 2020 2020 2023 204e 6f77 2066 696e 6420       # Now find 
+000168a0: 6e6f 6e2d 756e 7370 6563 6966 6965 642e  non-unspecified.
+000168b0: 0a20 2020 2020 2020 2066 6f72 2074 6572  .        for ter
+000168c0: 6d5f 2069 6e20 7365 6c66 2e74 6572 6d73  m_ in self.terms
+000168d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000168e0: 2074 6572 6d5f 2e6b 696e 6420 213d 2044   term_.kind != D
+000168f0: 696d 5479 7065 732e 556e 7370 6563 6966  imTypes.Unspecif
+00016900: 6965 643a 0a20 2020 2020 2020 2020 2020  ied:.           
+00016910: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
+00016920: 5f0a 2020 2020 2020 2020 2320 4e6f 7720  _.        # Now 
+00016930: 6669 6e64 2061 6e79 2e0a 2020 2020 2020  find any..      
+00016940: 2020 666f 7220 7465 726d 5f20 696e 2073    for term_ in s
+00016950: 656c 662e 7465 726d 733a 0a20 2020 2020  elf.terms:.     
+00016960: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+00016970: 726d 5f0a 2020 2020 2020 2020 7265 7475  rm_.        retu
+00016980: 726e 204e 6f6e 650a 0a0a 636c 6173 7320  rn None...class 
+00016990: 5f4f 704c 696e 6561 7254 6572 6d3a 0a20  _OpLinearTerm:. 
+000169a0: 2020 2022 2222 0a20 2020 2072 6570 7265     """.    repre
+000169b0: 7365 6e74 7320 7374 6820 6c69 6b65 2061  sents sth like a
+000169c0: 202a 2062 202b 2063 0a20 2020 2022 2222   * b + c.    """
+000169d0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+000169e0: 6f64 0a20 2020 2064 6566 2066 726f 6d5f  od.    def from_
+000169f0: 6469 6d28 636c 732c 2064 696d 293a 0a20  dim(cls, dim):. 
+00016a00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016a10: 2020 203a 7061 7261 6d20 4469 6d20 6469     :param Dim di
+00016a20: 6d3a 0a20 2020 2020 2020 203a 7274 7970  m:.        :rtyp
+00016a30: 653a 2044 696d 2e5f 4f70 4c69 6e65 6172  e: Dim._OpLinear
+00016a40: 5465 726d 0a20 2020 2020 2020 2022 2222  Term.        """
+00016a50: 0a20 2020 2020 2020 2072 6573 203d 2063  .        res = c
+00016a60: 6c73 2e7a 6572 6f28 290a 2020 2020 2020  ls.zero().      
+00016a70: 2020 7265 732e 6578 7465 6e64 5f61 6464    res.extend_add
+00016a80: 5f73 7562 5f28 6469 6d2c 206b 696e 643d  _sub_(dim, kind=
+00016a90: 2261 6464 222c 2072 6967 6874 3d54 7275  "add", right=Tru
+00016aa0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+00016ab0: 6e20 7265 730a 0a20 2020 2040 636c 6173  n res..    @clas
+00016ac0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00016ad0: 7a65 726f 2863 6c73 293a 0a20 2020 2020  zero(cls):.     
+00016ae0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00016af0: 7274 7970 653a 2044 696d 2e5f 4f70 4c69  rtype: Dim._OpLi
+00016b00: 6e65 6172 5465 726d 0a20 2020 2020 2020  nearTerm.       
+00016b10: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00016b20: 7572 6e20 5f4f 704c 696e 6561 7254 6572  urn _OpLinearTer
+00016b30: 6d28 5b5d 290a 0a20 2020 2064 6566 205f  m([])..    def _
+00016b40: 5f69 6e69 745f 5f28 7365 6c66 2c20 7465  _init__(self, te
+00016b50: 726d 7329 3a0a 2020 2020 2020 2020 2222  rms):.        ""
+00016b60: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00016b70: 206c 6973 745b 4469 6d2e 5f4f 704d 756c   list[Dim._OpMul
+00016b80: 7454 6572 6d5d 2074 6572 6d73 3a0a 2020  tTerm] terms:.  
+00016b90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00016ba0: 2020 7365 6c66 2e74 6572 6d73 203d 2074    self.terms = t
+00016bb0: 6572 6d73 0a0a 2020 2020 6465 6620 5f5f  erms..    def __
+00016bc0: 6861 7368 5f5f 2873 656c 6629 3a0a 2020  hash__(self):.  
+00016bd0: 2020 2020 2020 7265 7475 726e 2068 6173        return has
+00016be0: 6828 7475 706c 6528 7365 6c66 2e74 6572  h(tuple(self.ter
+00016bf0: 6d73 2929 0a0a 2020 2020 6465 6620 5f5f  ms))..    def __
+00016c00: 6571 5f5f 2873 656c 662c 206f 7468 6572  eq__(self, other
+00016c10: 293a 0a20 2020 2020 2020 2069 6620 6973  ):.        if is
+00016c20: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
+00016c30: 5f4f 704c 696e 6561 7254 6572 6d29 3a0a  _OpLinearTerm):.
+00016c40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00016c50: 726e 2073 656c 662e 7465 726d 7320 3d3d  rn self.terms ==
+00016c60: 206f 7468 6572 2e74 6572 6d73 0a20 2020   other.terms.   
+00016c70: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00016c80: 650a 0a20 2020 2064 6566 205f 5f6e 655f  e..    def __ne_
+00016c90: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+00016ca0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00016cb0: 6f74 2073 656c 662e 5f5f 6571 5f5f 286f  ot self.__eq__(o
+00016cc0: 7468 6572 290a 0a20 2020 2064 6566 2061  ther)..    def a
+00016cd0: 735f 6469 6d28 7365 6c66 293a 0a20 2020  s_dim(self):.   
+00016ce0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016cf0: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
+00016d00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016d10: 2069 6620 7365 6c66 2e69 735f 7a65 726f   if self.is_zero
+00016d20: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00016d30: 7265 7475 726e 205f 6d61 6b65 5f63 6f6e  return _make_con
+00016d40: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
+00016d50: 2830 290a 2020 2020 2020 2020 6966 206c  (0).        if l
+00016d60: 656e 2873 656c 662e 7465 726d 7329 203d  en(self.terms) =
+00016d70: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00016d80: 2072 6574 7572 6e20 7365 6c66 2e74 6572   return self.ter
+00016d90: 6d73 5b30 5d2e 6173 5f64 696d 2829 0a20  ms[0].as_dim(). 
+00016da0: 2020 2020 2020 2061 6464 5f70 6172 7473         add_parts
+00016db0: 203d 205b 5d0a 2020 2020 2020 2020 6465   = [].        de
+00016dc0: 7363 5f70 6172 7473 203d 205b 5d0a 2020  sc_parts = [].  
+00016dd0: 2020 2020 2020 6469 6d20 3d20 300a 2020        dim = 0.  
+00016de0: 2020 2020 2020 666f 7220 7465 726d 2069        for term i
+00016df0: 6e20 7365 6c66 2e74 6572 6d73 3a0a 2020  n self.terms:.  
+00016e00: 2020 2020 2020 2020 2020 7320 3d20 7465            s = te
+00016e10: 726d 2e61 735f 6469 6d28 290a 2020 2020  rm.as_dim().    
+00016e20: 2020 2020 2020 2020 6164 645f 7061 7274          add_part
+00016e30: 732e 6170 7065 6e64 2873 290a 2020 2020  s.append(s).    
+00016e40: 2020 2020 2020 2020 6465 7363 5f70 6172          desc_par
+00016e50: 7473 2e61 7070 656e 6428 5f67 6574 5f64  ts.append(_get_d
+00016e60: 6573 6372 6970 7469 6f6e 2873 2929 0a20  escription(s)). 
+00016e70: 2020 2020 2020 2020 2020 2069 6620 6469             if di
+00016e80: 6d20 6973 206e 6f74 204e 6f6e 6520 616e  m is not None an
+00016e90: 6420 732e 6469 6d65 6e73 696f 6e20 6973  d s.dimension is
+00016ea0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00016eb0: 2020 2020 2020 2020 2020 2064 696d 202b             dim +
+00016ec0: 3d20 732e 6469 6d65 6e73 696f 6e0a 2020  = s.dimension.  
+00016ed0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00016ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ef0: 6469 6d20 3d20 4e6f 6e65 0a20 2020 2020  dim = None.     
+00016f00: 2020 2069 6620 6c65 6e28 6164 645f 7061     if len(add_pa
+00016f10: 7274 7329 203d 3d20 313a 0a20 2020 2020  rts) == 1:.     
+00016f20: 2020 2020 2020 2072 6574 7572 6e20 6164         return ad
+00016f30: 645f 7061 7274 735b 305d 0a20 2020 2020  d_parts[0].     
+00016f40: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
+00016f50: 280a 2020 2020 2020 2020 2020 2020 6b69  (.            ki
+00016f60: 6e64 3d5f 6765 745f 6d65 7267 6564 5f64  nd=_get_merged_d
+00016f70: 696d 5f6b 696e 6428 6164 645f 7061 7274  im_kind(add_part
+00016f80: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
+00016f90: 6465 7363 7269 7074 696f 6e3d 222b 222e  description="+".
+00016fa0: 6a6f 696e 2864 6573 635f 7061 7274 7329  join(desc_parts)
+00016fb0: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+00016fc0: 6d65 6e73 696f 6e3d 6469 6d2c 0a20 2020  mension=dim,.   
+00016fd0: 2020 2020 2020 2020 2064 6572 6976 6564           derived
+00016fe0: 5f66 726f 6d5f 6f70 3d4f 7028 6b69 6e64  _from_op=Op(kind
+00016ff0: 3d22 6164 6422 2c20 696e 7075 7473 3d61  ="add", inputs=a
+00017000: 6464 5f70 6172 7473 292c 0a20 2020 2020  dd_parts),.     
+00017010: 2020 2020 2020 2064 6572 6976 6564 5f66         derived_f
+00017020: 726f 6d5f 7461 673d 7365 6c66 2e72 6570  rom_tag=self.rep
+00017030: 7265 7365 6e74 6174 6976 655f 7461 6728  resentative_tag(
+00017040: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00017050: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
+00017060: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00017070: 7475 726e 2022 4469 6d2e 5f4f 704c 696e  turn "Dim._OpLin
+00017080: 6561 7254 6572 6d28 2572 2922 2025 2028  earTerm(%r)" % (
+00017090: 7365 6c66 2e74 6572 6d73 2c29 0a0a 2020  self.terms,)..  
+000170a0: 2020 6465 6620 6973 5f7a 6572 6f28 7365    def is_zero(se
+000170b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000170c0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000170d0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
+000170e0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000170f0: 206e 6f74 2073 656c 662e 7465 726d 730a   not self.terms.
+00017100: 0a20 2020 2064 6566 2065 7874 656e 645f  .    def extend_
+00017110: 6164 645f 7375 625f 2873 656c 662c 206f  add_sub_(self, o
+00017120: 7468 6572 2c20 6b69 6e64 2c20 7269 6768  ther, kind, righ
+00017130: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
+00017140: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
+00017150: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
+00017160: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+00017170: 206b 696e 643a 2022 6164 6422 206f 7220   kind: "add" or 
+00017180: 2273 7562 220a 2020 2020 2020 2020 3a70  "sub".        :p
+00017190: 6172 616d 2062 6f6f 6c20 7269 6768 743a  aram bool right:
+000171a0: 206f 7220 6c65 6674 2e20 7269 6768 7420   or left. right 
+000171b0: 6d65 616e 7320 7365 6c66 202b 206f 7468  means self + oth
+000171c0: 6572 2c20 6c65 6674 206d 6561 6e73 206f  er, left means o
+000171d0: 7468 6572 202b 2073 656c 660a 2020 2020  ther + self.    
+000171e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000171f0: 6173 7365 7274 206b 696e 6420 696e 207b  assert kind in {
+00017200: 2261 6464 222c 2022 7375 6222 7d0a 2020  "add", "sub"}.  
+00017210: 2020 2020 2020 6f74 6865 7220 3d20 7365        other = se
+00017220: 6c66 2e5f 6d61 6b65 5f64 696d 286f 7468  lf._make_dim(oth
+00017230: 6572 2c20 6b69 6e64 3d6b 696e 6429 0a20  er, kind=kind). 
+00017240: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
+00017250: 6973 5f63 6f6e 7374 616e 745f 7374 6174  is_constant_stat
+00017260: 6963 5f64 696d 2829 2061 6e64 206f 7468  ic_dim() and oth
+00017270: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
+00017280: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00017290: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+000172a0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
+000172b0: 726f 6d5f 6f70 2061 6e64 206f 7468 6572  rom_op and other
+000172c0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+000172d0: 2e6b 696e 6420 3d3d 2022 6164 6422 3a0a  .kind == "add":.
+000172e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000172f0: 6f74 6865 725f 2069 6e20 6f74 6865 722e  other_ in other.
+00017300: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00017310: 696e 7075 7473 2069 6620 7269 6768 7420  inputs if right 
+00017320: 656c 7365 2072 6576 6572 7365 6428 6f74  else reversed(ot
+00017330: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+00017340: 5f6f 702e 696e 7075 7473 293a 0a20 2020  _op.inputs):.   
+00017350: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017360: 662e 6578 7465 6e64 5f61 6464 5f73 7562  f.extend_add_sub
+00017370: 5f28 6f74 6865 725f 2c20 6b69 6e64 3d6b  _(other_, kind=k
+00017380: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
+00017390: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000173a0: 7475 726e 0a20 2020 2020 2020 2074 6572  turn.        ter
+000173b0: 6d20 3d20 5f4f 704d 756c 7454 6572 6d2e  m = _OpMultTerm.
+000173c0: 6672 6f6d 5f64 696d 286f 7468 6572 290a  from_dim(other).
+000173d0: 2020 2020 2020 2020 6e65 675f 7465 726d          neg_term
+000173e0: 203d 2074 6572 6d2e 6e65 6761 7469 7665   = term.negative
+000173f0: 2829 0a20 2020 2020 2020 2069 6620 6b69  ().        if ki
+00017400: 6e64 203d 3d20 2273 7562 223a 0a20 2020  nd == "sub":.   
+00017410: 2020 2020 2020 2020 2074 6572 6d2c 206e           term, n
+00017420: 6567 5f74 6572 6d20 3d20 6e65 675f 7465  eg_term = neg_te
+00017430: 726d 2c20 7465 726d 0a20 2020 2020 2020  rm, term.       
+00017440: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
+00017450: 6d20 3d20 7365 6c66 2e74 6572 6d73 5b2d  m = self.terms[-
+00017460: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
+00017470: 305d 2069 6620 7365 6c66 2e74 6572 6d73  0] if self.terms
+00017480: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+00017490: 2020 2069 6620 6d6f 7374 5f72 6563 656e     if most_recen
+000174a0: 745f 7465 726d 3a0a 2020 2020 2020 2020  t_term:.        
+000174b0: 2020 2020 6966 206d 6f73 745f 7265 6365      if most_rece
+000174c0: 6e74 5f74 6572 6d20 3d3d 206e 6567 5f74  nt_term == neg_t
+000174d0: 6572 6d3a 0a20 2020 2020 2020 2020 2020  erm:.           
+000174e0: 2020 2020 2073 656c 662e 7465 726d 732e       self.terms.
+000174f0: 706f 7028 2d31 2069 6620 7269 6768 7420  pop(-1 if right 
+00017500: 656c 7365 2030 290a 2020 2020 2020 2020  else 0).        
+00017510: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00017520: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+00017530: 7374 5f72 6563 656e 745f 7465 726d 2e69  st_recent_term.i
+00017540: 735f 636f 6e73 7461 6e74 5f73 7461 7469  s_constant_stati
+00017550: 635f 6469 6d28 2920 616e 6420 7465 726d  c_dim() and term
+00017560: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
+00017570: 7469 635f 6469 6d28 293a 0a20 2020 2020  tic_dim():.     
+00017580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017590: 7465 726d 735b 2d31 2069 6620 7269 6768  terms[-1 if righ
+000175a0: 7420 656c 7365 2030 5d20 3d20 5f4f 704d  t else 0] = _OpM
+000175b0: 756c 7454 6572 6d2e 6672 6f6d 5f64 696d  ultTerm.from_dim
+000175c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000175d0: 2020 2020 2020 5f6d 616b 655f 636f 6e73        _make_cons
+000175e0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
+000175f0: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
+00017600: 2e64 696d 656e 7369 6f6e 202b 2074 6572  .dimension + ter
+00017610: 6d2e 6469 6d65 6e73 696f 6e2c 206b 696e  m.dimension, kin
+00017620: 643d 6f74 6865 722e 6b69 6e64 290a 2020  d=other.kind).  
+00017630: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017650: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00017660: 2020 2069 6620 6d6f 7374 5f72 6563 656e     if most_recen
+00017670: 745f 7465 726d 2e74 6572 6d73 2061 6e64  t_term.terms and
+00017680: 2074 6572 6d2e 7465 726d 7320 616e 6420   term.terms and 
+00017690: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
+000176a0: 2e74 6572 6d73 5b2d 315d 203d 3d20 7465  .terms[-1] == te
+000176b0: 726d 2e74 6572 6d73 5b2d 315d 3a0a 2020  rm.terms[-1]:.  
+000176c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000176d0: 4d65 7267 6520 7465 726d 730a 2020 2020  Merge terms.    
+000176e0: 2020 2020 2020 2020 2020 2020 6120 3d20              a = 
+000176f0: 5f4f 704d 756c 7454 6572 6d2e 6672 6f6d  _OpMultTerm.from
+00017700: 5f64 696d 5f66 6163 746f 7273 286d 6f73  _dim_factors(mos
+00017710: 745f 7265 6365 6e74 5f74 6572 6d2e 7465  t_recent_term.te
+00017720: 726d 735b 3a2d 315d 292e 6173 5f64 696d  rms[:-1]).as_dim
+00017730: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00017740: 2020 2062 203d 205f 4f70 4d75 6c74 5465     b = _OpMultTe
+00017750: 726d 2e66 726f 6d5f 6469 6d5f 6661 6374  rm.from_dim_fact
+00017760: 6f72 7328 7465 726d 2e74 6572 6d73 5b3a  ors(term.terms[:
+00017770: 2d31 5d29 2e61 735f 6469 6d28 290a 2020  -1]).as_dim().  
+00017780: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00017790: 7320 3d20 5f4f 704d 756c 7454 6572 6d2e  s = _OpMultTerm.
+000177a0: 6672 6f6d 5f64 696d 2828 6120 2b20 6229  from_dim((a + b)
+000177b0: 2069 6620 7269 6768 7420 656c 7365 2028   if right else (
+000177c0: 6220 2b20 6129 290a 2020 2020 2020 2020  b + a)).        
+000177d0: 2020 2020 2020 2020 7265 732e 6578 7465          res.exte
+000177e0: 6e64 5f6d 756c 5f64 6976 5f28 7465 726d  nd_mul_div_(term
+000177f0: 2e74 6572 6d73 5b2d 315d 2c20 6b69 6e64  .terms[-1], kind
+00017800: 3d22 6d75 6c22 2c20 7269 6768 743d 5472  ="mul", right=Tr
+00017810: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00017820: 2020 2020 7365 6c66 2e74 6572 6d73 5b2d      self.terms[-
+00017830: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
+00017840: 305d 203d 2072 6573 0a20 2020 2020 2020  0] = res.       
+00017850: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00017860: 2020 2020 2020 2020 6966 2072 6967 6874          if right
+00017870: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00017880: 6c66 2e74 6572 6d73 2e61 7070 656e 6428  lf.terms.append(
+00017890: 7465 726d 290a 2020 2020 2020 2020 656c  term).        el
+000178a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000178b0: 7365 6c66 2e74 6572 6d73 2e69 6e73 6572  self.terms.inser
+000178c0: 7428 302c 2074 6572 6d29 0a0a 2020 2020  t(0, term)..    
+000178d0: 6465 6620 6578 7465 6e64 5f6d 756c 5f64  def extend_mul_d
+000178e0: 6976 5f28 7365 6c66 2c20 6f74 6865 722c  iv_(self, other,
+000178f0: 206b 696e 642c 2072 6967 6874 293a 0a20   kind, right):. 
+00017900: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00017910: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
+00017920: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
+00017930: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
+00017940: 3a20 226d 756c 2220 6f72 2022 6365 696c  : "mul" or "ceil
+00017950: 6469 7622 0a20 2020 2020 2020 203a 7061  div".        :pa
+00017960: 7261 6d20 626f 6f6c 2072 6967 6874 3a20  ram bool right: 
+00017970: 6f72 206c 6566 742e 2072 6967 6874 206d  or left. right m
+00017980: 6561 6e73 2073 656c 6620 2a20 6f74 6865  eans self * othe
+00017990: 722c 206c 6566 7420 6d65 616e 7320 6f74  r, left means ot
+000179a0: 6865 7220 2a20 7365 6c66 0a20 2020 2020  her * self.     
+000179b0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+000179c0: 7373 6572 7420 6b69 6e64 2069 6e20 7b22  ssert kind in {"
+000179d0: 6d75 6c22 2c20 2266 6c6f 6f72 6469 7622  mul", "floordiv"
+000179e0: 2c20 2274 7275 6564 6976 222c 2022 6365  , "truediv", "ce
+000179f0: 696c 6469 7622 7d0a 2020 2020 2020 2020  ildiv"}.        
+00017a00: 6f74 6865 7220 3d20 7365 6c66 2e5f 6d61  other = self._ma
+00017a10: 6b65 5f64 696d 286f 7468 6572 2c20 6b69  ke_dim(other, ki
+00017a20: 6e64 3d6b 696e 6429 0a20 2020 2020 2020  nd=kind).       
+00017a30: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
+00017a40: 2220 616e 6420 7269 6768 743a 0a20 2020  " and right:.   
+00017a50: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00017a60: 616c 6c28 7465 726d 2e63 616e 5f73 696d  all(term.can_sim
+00017a70: 706c 6966 7928 6f74 6865 722c 206b 696e  plify(other, kin
+00017a80: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
+00017a90: 6768 7429 2066 6f72 2074 6572 6d20 696e  ght) for term in
+00017aa0: 2073 656c 662e 7465 726d 7329 3a0a 2020   self.terms):.  
+00017ab0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00017ac0: 446f 2069 7420 7468 6520 6f74 6865 7220  Do it the other 
+00017ad0: 7761 7920 6172 6f75 6e64 0a20 2020 2020  way around.     
+00017ae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017af0: 7465 726d 732c 206f 7468 6572 203d 205f  terms, other = _
+00017b00: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
+00017b10: 6d5f 6469 6d28 6f74 6865 7229 2e74 6572  m_dim(other).ter
+00017b20: 6d73 2c20 7365 6c66 2e61 735f 6469 6d28  ms, self.as_dim(
+00017b30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017b40: 2020 7269 6768 7420 3d20 4661 6c73 650a    right = False.
+00017b50: 2020 2020 2020 2020 6966 206f 7468 6572          if other
+00017b60: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
+00017b70: 7469 635f 6469 6d28 2920 616e 6420 6f74  tic_dim() and ot
+00017b80: 6865 722e 6469 6d65 6e73 696f 6e20 3d3d  her.dimension ==
+00017b90: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00017ba0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+00017bb0: 6620 6b69 6e64 2e65 6e64 7377 6974 6828  f kind.endswith(
+00017bc0: 2264 6976 2229 2061 6e64 206c 656e 2873  "div") and len(s
+00017bd0: 656c 662e 7465 726d 7329 203e 3d20 323a  elf.terms) >= 2:
+00017be0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017bf0: 616e 7928 6e6f 7420 7465 726d 2e64 6976  any(not term.div
+00017c00: 6973 6962 6c65 286f 7468 6572 2c20 7269  isible(other, ri
+00017c10: 6768 743d 7269 6768 7429 2066 6f72 2074  ght=right) for t
+00017c20: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
+00017c30: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00017c40: 2020 2020 7365 6c66 2e74 6572 6d73 203d      self.terms =
+00017c50: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00017c60: 2020 2020 2020 205f 4f70 4d75 6c74 5465         _OpMultTe
+00017c70: 726d 2e66 726f 6d5f 6469 6d28 5f4f 704d  rm.from_dim(_OpM
+00017c80: 756c 7454 6572 6d2e 6e65 775f 6469 765f  ultTerm.new_div_
+00017c90: 6469 6d28 7365 6c66 2e61 735f 6469 6d28  dim(self.as_dim(
+00017ca0: 292c 206f 7468 6572 2c20 6b69 6e64 3d6b  ), other, kind=k
+00017cb0: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
+00017cc0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00017cd0: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00017ce0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00017cf0: 2020 2020 666f 7220 7465 726d 2069 6e20      for term in 
+00017d00: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
+00017d10: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
+00017d20: 656e 645f 6d75 6c5f 6469 765f 286f 7468  end_mul_div_(oth
+00017d30: 6572 2c20 6b69 6e64 3d6b 696e 642c 2072  er, kind=kind, r
+00017d40: 6967 6874 3d72 6967 6874 290a 0a20 2020  ight=right)..   
+00017d50: 2064 6566 205f 6d61 6b65 5f64 696d 2873   def _make_dim(s
+00017d60: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
+00017d70: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00017d80: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00017d90: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+00017da0: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
+00017db0: 6b69 6e64 3a0a 2020 2020 2020 2020 3a72  kind:.        :r
+00017dc0: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+00017dd0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00017de0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+00017df0: 722c 2069 6e74 293a 0a20 2020 2020 2020  r, int):.       
+00017e00: 2020 2020 2062 6173 655f 7461 6720 3d20       base_tag = 
+00017e10: 7365 6c66 2e72 6570 7265 7365 6e74 6174  self.representat
+00017e20: 6976 655f 7461 6728 290a 2020 2020 2020  ive_tag().      
+00017e30: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00017e40: 6b65 5f63 6f6e 7374 616e 745f 7374 6174  ke_constant_stat
+00017e50: 6963 5f64 696d 286f 7468 6572 2c20 6b69  ic_dim(other, ki
+00017e60: 6e64 3d62 6173 655f 7461 672e 6b69 6e64  nd=base_tag.kind
+00017e70: 2069 6620 6261 7365 5f74 6167 2065 6c73   if base_tag els
+00017e80: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
+00017e90: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00017ea0: 6f74 6865 722c 205f 642e 4469 6d29 3a0a  other, _d.Dim):.
+00017eb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017ec0: 726e 206f 7468 6572 2e67 6574 5f73 616d  rn other.get_sam
+00017ed0: 655f 6261 7365 2829 0a20 2020 2020 2020  e_base().       
+00017ee0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00017ef0: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00017f00: 6f72 2822 2573 2025 7320 2573 2069 6e76  or("%s %s %s inv
+00017f10: 616c 6964 2066 6f72 2074 7970 6520 2573  alid for type %s
+00017f20: 2220 2520 2873 656c 662c 206b 696e 642c  " % (self, kind,
+00017f30: 206f 7468 6572 2c20 7479 7065 286f 7468   other, type(oth
+00017f40: 6572 2929 290a 0a20 2020 2064 6566 2072  er)))..    def r
+00017f50: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
+00017f60: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+00017f70: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+00017f80: 7970 653a 2044 696d 7c4e 6f6e 650a 2020  ype: Dim|None.  
+00017f90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00017fa0: 2020 2320 4669 7273 7420 6669 6e64 2061    # First find a
+00017fb0: 6e79 2064 796e 616d 6963 2e0a 2020 2020  ny dynamic..    
+00017fc0: 2020 2020 666f 7220 7465 726d 2069 6e20      for term in 
+00017fd0: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
+00017fe0: 2020 2020 2020 2020 666f 7220 7465 726d          for term
+00017ff0: 5f20 696e 2074 6572 6d2e 7465 726d 733a  _ in term.terms:
+00018000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018010: 2069 6620 7465 726d 5f2e 6973 5f64 796e   if term_.is_dyn
+00018020: 616d 6963 2829 3a0a 2020 2020 2020 2020  amic():.        
 00018030: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00018040: 726e 205f 6d61 6b65 5f63 6f6e 7374 616e  rn _make_constan
-00018050: 745f 7374 6174 6963 5f64 696d 286f 7468  t_static_dim(oth
-00018060: 6572 2c20 6b69 6e64 3d62 6173 655f 7461  er, kind=base_ta
-00018070: 672e 6b69 6e64 2069 6620 6261 7365 5f74  g.kind if base_t
-00018080: 6167 2065 6c73 6520 4e6f 6e65 290a 2020  ag else None).  
-00018090: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-000180a0: 7461 6e63 6528 6f74 6865 722c 205f 642e  tance(other, _d.
-000180b0: 4469 6d29 3a0a 2020 2020 2020 2020 2020  Dim):.          
-000180c0: 2020 7265 7475 726e 206f 7468 6572 2e67    return other.g
-000180d0: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
-000180e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000180f0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00018100: 7970 6545 7272 6f72 2822 2573 2025 7320  ypeError("%s %s 
-00018110: 2573 2069 6e76 616c 6964 2066 6f72 2074  %s invalid for t
-00018120: 7970 6520 2573 2220 2520 2873 656c 662c  ype %s" % (self,
-00018130: 206b 696e 642c 206f 7468 6572 2c20 7479   kind, other, ty
-00018140: 7065 286f 7468 6572 2929 290a 0a20 2020  pe(other)))..   
-00018150: 2064 6566 2072 6570 7265 7365 6e74 6174   def representat
-00018160: 6976 655f 7461 6728 7365 6c66 293a 0a20  ive_tag(self):. 
-00018170: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00018180: 2020 203a 7274 7970 653a 2044 696d 7c4e     :rtype: Dim|N
-00018190: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
-000181a0: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
-000181b0: 6669 6e64 2061 6e79 2064 796e 616d 6963  find any dynamic
-000181c0: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
-000181d0: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
-000181e0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-000181f0: 7220 7465 726d 5f20 696e 2074 6572 6d2e  r term_ in term.
-00018200: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
-00018210: 2020 2020 2020 2069 6620 7465 726d 5f2e         if term_.
-00018220: 6973 5f64 796e 616d 6963 2829 3a0a 2020  is_dynamic():.  
-00018230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018240: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
-00018250: 2020 2020 2020 2023 204e 6f77 2066 696e         # Now fin
-00018260: 6420 6e6f 6e2d 756e 7370 6563 6966 6965  d non-unspecifie
-00018270: 642e 0a20 2020 2020 2020 2066 6f72 2074  d..        for t
-00018280: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
-00018290: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-000182a0: 6f72 2074 6572 6d5f 2069 6e20 7465 726d  or term_ in term
-000182b0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-000182c0: 2020 2020 2020 2020 6966 2074 6572 6d5f          if term_
-000182d0: 2e6b 696e 6420 213d 2044 696d 5479 7065  .kind != DimType
-000182e0: 732e 556e 7370 6563 6966 6965 643a 0a20  s.Unspecified:. 
-000182f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018300: 2020 2072 6574 7572 6e20 7465 726d 5f0a     return term_.
-00018310: 2020 2020 2020 2020 2320 4e6f 7720 6669          # Now fi
-00018320: 6e64 2061 6e79 2e0a 2020 2020 2020 2020  nd any..        
-00018330: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
-00018340: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00018350: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
-00018360: 2074 6572 6d2e 7465 726d 733a 0a20 2020   term.terms:.   
-00018370: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00018380: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
-00018390: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
-000183a0: 6465 6620 5f67 6574 5f6d 6572 6765 645f  def _get_merged_
-000183b0: 6469 6d5f 6b69 6e64 2864 696d 5f74 6167  dim_kind(dim_tag
-000183c0: 7329 3a0a 2020 2020 2222 220a 2020 2020  s):.    """.    
-000183d0: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
-000183e0: 7c74 7570 6c65 5b44 696d 5d20 6469 6d5f  |tuple[Dim] dim_
-000183f0: 7461 6773 3a0a 2020 2020 3a72 6574 7572  tags:.    :retur
-00018400: 6e3a 2064 696d 206b 696e 640a 2020 2020  n: dim kind.    
-00018410: 3a72 7479 7065 3a20 456e 7469 7479 0a20  :rtype: Entity. 
-00018420: 2020 2022 2222 0a20 2020 2069 6620 616e     """.    if an
-00018430: 7928 7461 672e 6973 5f62 6174 6368 5f64  y(tag.is_batch_d
-00018440: 696d 2829 2066 6f72 2074 6167 2069 6e20  im() for tag in 
-00018450: 6469 6d5f 7461 6773 293a 0a20 2020 2020  dim_tags):.     
-00018460: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
-00018470: 6573 2e42 6174 6368 0a20 2020 2065 6c69  es.Batch.    eli
-00018480: 6620 616e 7928 7461 672e 6973 5f66 6561  f any(tag.is_fea
-00018490: 7475 7265 5f64 696d 2829 2066 6f72 2074  ture_dim() for t
-000184a0: 6167 2069 6e20 6469 6d5f 7461 6773 293a  ag in dim_tags):
-000184b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000184c0: 4469 6d54 7970 6573 2e46 6561 7475 7265  DimTypes.Feature
-000184d0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000184e0: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
-000184f0: 6573 2e53 7061 7469 616c 0a0a 0a64 6566  es.Spatial...def
-00018500: 2064 696d 5f63 6d70 5f76 616c 7565 286f   dim_cmp_value(o
-00018510: 626a 293a 0a20 2020 2022 2222 0a20 2020  bj):.    """.   
-00018520: 203a 7061 7261 6d20 4469 6d7c 5f4d 6172   :param Dim|_Mar
-00018530: 6b65 6444 696d 206f 626a 3a0a 2020 2020  kedDim obj:.    
-00018540: 3a72 6574 7572 6e3a 2061 6e79 7468 696e  :return: anythin
-00018550: 6720 7768 6963 6820 6361 6e20 6265 2063  g which can be c
-00018560: 6f6d 7061 7265 640a 2020 2020 2222 220a  ompared.    """.
-00018570: 2020 2020 2320 4d61 6b65 2044 696d 2061      # Make Dim a
-00018580: 6e64 205f 4d61 726b 6564 4469 6d20 636f  nd _MarkedDim co
-00018590: 6d70 6172 6162 6c65 2074 6f20 6561 6368  mparable to each
-000185a0: 206f 7468 6572 2e0a 2020 2020 2320 4e6f   other..    # No
-000185b0: 7465 2074 6861 7420 7468 6520 6f72 6465  te that the orde
-000185c0: 7220 6973 2072 6561 6c6c 7920 6172 6269  r is really arbi
-000185d0: 7472 6172 7920 616e 6420 646f 6573 206e  trary and does n
-000185e0: 6f74 206d 6174 7465 722e 0a20 2020 2069  ot matter..    i
-000185f0: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
-00018600: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
-00018610: 2020 206f 626a 203d 206f 626a 2e67 6574     obj = obj.get
-00018620: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
-00018630: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
-00018640: 2020 2020 2020 2020 2020 2222 2c0a 2020            "",.  
-00018650: 2020 2020 2020 2020 2020 6f62 6a2e 6465            obj.de
-00018660: 7363 7269 7074 696f 6e2c 0a20 2020 2020  scription,.     
-00018670: 2020 2020 2020 206f 626a 2e6b 696e 642c         obj.kind,
-00018680: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
-00018690: 2e64 696d 656e 7369 6f6e 2c0a 2020 2020  .dimension,.    
-000186a0: 2020 2020 2020 2020 6f62 6a2e 6479 6e5f          obj.dyn_
-000186b0: 7369 7a65 5f65 7874 2e64 696d 7320 6966  size_ext.dims if
-000186c0: 206f 626a 2e64 796e 5f73 697a 655f 6578   obj.dyn_size_ex
-000186d0: 7420 6973 206e 6f74 204e 6f6e 6520 656c  t is not None el
-000186e0: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
-000186f0: 2029 0a20 2020 2069 6620 6973 696e 7374   ).    if isinst
-00018700: 616e 6365 286f 626a 2c20 5f6d 2e4d 6172  ance(obj, _m.Mar
-00018710: 6b65 6444 696d 293a 0a20 2020 2020 2020  kedDim):.       
-00018720: 2072 6574 7572 6e20 6f62 6a2e 5f5f 636c   return obj.__cl
-00018730: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20  ass__.__name__, 
-00018740: 6f62 6a2e 7461 670a 2020 2020 7265 7475  obj.tag.    retu
-00018750: 726e 206f 626a 0a                        rn obj.
+00018040: 726e 2074 6572 6d5f 0a20 2020 2020 2020  rn term_.       
+00018050: 2023 204e 6f77 2066 696e 6420 6e6f 6e2d   # Now find non-
+00018060: 756e 7370 6563 6966 6965 642e 0a20 2020  unspecified..   
+00018070: 2020 2020 2066 6f72 2074 6572 6d20 696e       for term in
+00018080: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
+00018090: 2020 2020 2020 2020 2066 6f72 2074 6572           for ter
+000180a0: 6d5f 2069 6e20 7465 726d 2e74 6572 6d73  m_ in term.terms
+000180b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000180c0: 2020 6966 2074 6572 6d5f 2e6b 696e 6420    if term_.kind 
+000180d0: 213d 2044 696d 5479 7065 732e 556e 7370  != DimTypes.Unsp
+000180e0: 6563 6966 6965 643a 0a20 2020 2020 2020  ecified:.       
+000180f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00018100: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
+00018110: 2020 2320 4e6f 7720 6669 6e64 2061 6e79    # Now find any
+00018120: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
+00018130: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
+00018140: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00018150: 7220 7465 726d 5f20 696e 2074 6572 6d2e  r term_ in term.
+00018160: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+00018170: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+00018180: 726d 5f0a 2020 2020 2020 2020 7265 7475  rm_.        retu
+00018190: 726e 204e 6f6e 650a 0a0a 6465 6620 5f67  rn None...def _g
+000181a0: 6574 5f6d 6572 6765 645f 6469 6d5f 6b69  et_merged_dim_ki
+000181b0: 6e64 2864 696d 5f74 6167 7329 3a0a 2020  nd(dim_tags):.  
+000181c0: 2020 2222 220a 2020 2020 3a70 6172 616d    """.    :param
+000181d0: 206c 6973 745b 4469 6d5d 7c74 7570 6c65   list[Dim]|tuple
+000181e0: 5b44 696d 5d20 6469 6d5f 7461 6773 3a0a  [Dim] dim_tags:.
+000181f0: 2020 2020 3a72 6574 7572 6e3a 2064 696d      :return: dim
+00018200: 206b 696e 640a 2020 2020 3a72 7479 7065   kind.    :rtype
+00018210: 3a20 456e 7469 7479 0a20 2020 2022 2222  : Entity.    """
+00018220: 0a20 2020 2069 6620 616e 7928 7461 672e  .    if any(tag.
+00018230: 6973 5f62 6174 6368 5f64 696d 2829 2066  is_batch_dim() f
+00018240: 6f72 2074 6167 2069 6e20 6469 6d5f 7461  or tag in dim_ta
+00018250: 6773 293a 0a20 2020 2020 2020 2072 6574  gs):.        ret
+00018260: 7572 6e20 4469 6d54 7970 6573 2e42 6174  urn DimTypes.Bat
+00018270: 6368 0a20 2020 2065 6c69 6620 616e 7928  ch.    elif any(
+00018280: 7461 672e 6973 5f66 6561 7475 7265 5f64  tag.is_feature_d
+00018290: 696d 2829 2066 6f72 2074 6167 2069 6e20  im() for tag in 
+000182a0: 6469 6d5f 7461 6773 293a 0a20 2020 2020  dim_tags):.     
+000182b0: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
+000182c0: 6573 2e46 6561 7475 7265 0a20 2020 2065  es.Feature.    e
+000182d0: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
+000182e0: 7572 6e20 4469 6d54 7970 6573 2e53 7061  urn DimTypes.Spa
+000182f0: 7469 616c 0a0a 0a64 6566 2064 696d 5f63  tial...def dim_c
+00018300: 6d70 5f76 616c 7565 286f 626a 293a 0a20  mp_value(obj):. 
+00018310: 2020 2022 2222 0a20 2020 203a 7061 7261     """.    :para
+00018320: 6d20 4469 6d7c 5f4d 6172 6b65 6444 696d  m Dim|_MarkedDim
+00018330: 206f 626a 3a0a 2020 2020 3a72 6574 7572   obj:.    :retur
+00018340: 6e3a 2061 6e79 7468 696e 6720 7768 6963  n: anything whic
+00018350: 6820 6361 6e20 6265 2063 6f6d 7061 7265  h can be compare
+00018360: 640a 2020 2020 2222 220a 2020 2020 2320  d.    """.    # 
+00018370: 4d61 6b65 2044 696d 2061 6e64 205f 4d61  Make Dim and _Ma
+00018380: 726b 6564 4469 6d20 636f 6d70 6172 6162  rkedDim comparab
+00018390: 6c65 2074 6f20 6561 6368 206f 7468 6572  le to each other
+000183a0: 2e0a 2020 2020 2320 4e6f 7465 2074 6861  ..    # Note tha
+000183b0: 7420 7468 6520 6f72 6465 7220 6973 2072  t the order is r
+000183c0: 6561 6c6c 7920 6172 6269 7472 6172 7920  eally arbitrary 
+000183d0: 616e 6420 646f 6573 206e 6f74 206d 6174  and does not mat
+000183e0: 7465 722e 0a20 2020 2069 6620 6973 696e  ter..    if isin
+000183f0: 7374 616e 6365 286f 626a 2c20 5f64 2e44  stance(obj, _d.D
+00018400: 696d 293a 0a20 2020 2020 2020 206f 626a  im):.        obj
+00018410: 203d 206f 626a 2e67 6574 5f73 616d 655f   = obj.get_same_
+00018420: 6261 7365 2829 0a20 2020 2020 2020 2072  base().        r
+00018430: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
+00018440: 2020 2020 2222 2c0a 2020 2020 2020 2020      "",.        
+00018450: 2020 2020 6f62 6a2e 6465 7363 7269 7074      obj.descript
+00018460: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00018470: 206f 626a 2e6b 696e 642c 0a20 2020 2020   obj.kind,.     
+00018480: 2020 2020 2020 206f 626a 2e64 696d 656e         obj.dimen
+00018490: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+000184a0: 2020 6f62 6a2e 6479 6e5f 7369 7a65 5f65    obj.dyn_size_e
+000184b0: 7874 2e64 696d 7320 6966 206f 626a 2e64  xt.dims if obj.d
+000184c0: 796e 5f73 697a 655f 6578 7420 6973 206e  yn_size_ext is n
+000184d0: 6f74 204e 6f6e 6520 656c 7365 204e 6f6e  ot None else Non
+000184e0: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
+000184f0: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
+00018500: 626a 2c20 5f6d 2e4d 6172 6b65 6444 696d  bj, _m.MarkedDim
+00018510: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00018520: 6e20 6f62 6a2e 5f5f 636c 6173 735f 5f2e  n obj.__class__.
+00018530: 5f5f 6e61 6d65 5f5f 2c20 6f62 6a2e 7461  __name__, obj.ta
+00018540: 670a 2020 2020 7265 7475 726e 206f 626a  g.    return obj
+00018550: 0a                                       .
```

### Comparing `returnn-1.20230630.233220/returnn/tensor/_tensor_extra.py` & `returnn-1.20230630.93532/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230630.93532/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230630.93532/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230630.93532/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/dim.py` & `returnn-1.20230630.93532/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/marked_dim.py` & `returnn-1.20230630.93532/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/tensor.py` & `returnn-1.20230630.93532/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/tensor_dict.py` & `returnn-1.20230630.93532/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tensor/utils.py` & `returnn-1.20230630.93532/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/compat.py` & `returnn-1.20230630.93532/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/data_pipeline.py` & `returnn-1.20230630.93532/returnn/tf/data_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,39 +219,45 @@
     This class will fill all the placeholders used for training or forwarding or evaluation etc.
     of a :class:`returnn.tf.network.TFNetwork`.
     It will run a background thread which reads the data from a dataset and puts it into a queue.
     """
 
     def __init__(
         self,
-        *,
+        tf_session,
         dataset,
         batches,
         enforce_min_len1=False,
         capacity=10,
+        tf_queue=None,
         batch_slice=None,
         **kwargs,
     ):
         """
+        :param tf.compat.v1.Session|tf.compat.v1.InteractiveSession tf_session:
         :param Dataset dataset:
         :param BatchSetGenerator batches:
         :param bool enforce_min_len1:
         :param ExternData extern_data:
         :param set(str)|None data_keys:
         :param int capacity:
+        :param TFDataQueues|None tf_queue:
         :param slice|None batch_slice: select a subset of the batches
         """
         super(FeedDictDataProvider, self).__init__(**kwargs)
+        self.tf_session = tf_session
         self.dataset = dataset
         self.batches = batches
         self.enforce_min_len1 = enforce_min_len1
         self.batch_slice = batch_slice
         self.state_change_cond = Condition()
         self.queue = None  # type: typing.Optional[Queue]
-        self.queue = Queue(maxsize=capacity)
+        self.tf_queue = tf_queue
+        if not self.tf_queue:
+            self.queue = Queue(maxsize=capacity)
         self.thread = None  # type: typing.Optional[Thread]
         self.thread_finished = False
         self.cur_batch_idx = 0
         self.reached_end = False
 
     def start_threads(self, session):
         """
@@ -376,15 +382,18 @@
             from returnn.util import better_exchook
 
             better_exchook.install()
 
             while self.batches.has_more() and not self.coord.should_stop():
                 enqueue_args = self.get_next_batch(consider_batch_slice=True)
                 if enqueue_args is not None:
-                    self.queue.put(enqueue_args)
+                    if self.queue:
+                        self.queue.put(enqueue_args)
+                    else:
+                        self.tf_queue.enqueue(tf_session=self.tf_session, data=enqueue_args)
                 with self.state_change_cond:
                     self.state_change_cond.notifyAll()
                 self.batches.advance(1)
 
             self.reached_end = not self.batches.has_more()
 
         except Exception as exc:
@@ -405,14 +414,16 @@
         Threading safety: This assumes that there is no other consumer thread for the queue.
         """
         with self.state_change_cond:
             while True:
                 # First check if there is still data in the queue to be processed.
                 if self.queue and not self.queue.empty():
                     return True
+                if self.tf_queue and self.tf_queue.have_more(self.tf_session):
+                    return True
                 if self.thread_finished:
                     return False
                 if not self.thread.is_alive:
                     return False
                 # The thread is alive and working. Wait for a change.
                 self.state_change_cond.wait()
 
@@ -434,14 +445,16 @@
         The queue gets filled by the other thread, via self.thread_main().
 
         :param bool single_threaded: whether to not use the queue
         :returns: we dequeue one batch from the queue and provide it for all placeholders of our external data,
           and additionally return some meta information.
         :rtype: (dict[tf.Tensor,numpy.ndarray],dict[str])
         """
+        if self.tf_queue:
+            return {}  # not needed to feed anything, it gets it via the queues
         if single_threaded:
             assert self.batches.has_more()
             assert self.batch_slice is None
             output = self.get_next_batch(consider_batch_slice=False)
             self.batches.advance(1)
         else:
             output = self.queue.get()
```

### Comparing `returnn-1.20230630.233220/returnn/tf/distributed.py` & `returnn-1.20230630.93532/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/engine.py` & `returnn-1.20230630.93532/returnn/tf/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -2287,14 +2287,15 @@
         else:
             if self.dataset_provider and feed_dict is not False:
                 print("WARNING: dataset_provider is set (via dataset_pipeline) but not used", file=log.v2)
             batch_slice = None
             if tf_horovod.get_ctx() and tf_horovod.get_ctx().is_dataset_distribution_shard():
                 batch_slice = tf_horovod.get_ctx().get_dataset_shard_batch_slice()
             data_provider = FeedDictDataProvider(
+                tf_session=self.tf_session,
                 extern_data=self.network.extern_data,
                 data_keys=self.network.get_used_data_keys(),
                 dataset=dataset,
                 batches=batches,
                 batch_slice=batch_slice,
                 enforce_min_len1=self.config.is_true("enforce_min_len1", False),
             )
```

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230630.93532/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230630.93532/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/horovod.py` & `returnn-1.20230630.93532/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230630.93532/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/layers/base.py` & `returnn-1.20230630.93532/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/layers/basic.py` & `returnn-1.20230630.93532/returnn/tf/layers/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -8440,15 +8440,17 @@
         :rtype: (list[int], list[int])
         """
         from returnn.util import BehaviorVersion
 
         if BehaviorVersion.get() >= 14:
             is_equal_opts = {}
         else:
-            is_equal_opts = dict(treat_feature_as_spatial=True, allow_same_spatial_dim=True, undefined_matches=True)
+            is_equal_opts = dict(
+                treat_feature_as_spatial=True, allow_same_spatial_dim=True, undefined_matches=True, derived_matches=True
+            )
         tags1 = [None if i in red1 else tag for (i, tag) in enumerate(source1.dim_tags)]
         tags2 = [None if i in red2 else tag for (i, tag) in enumerate(source2.dim_tags)]
         var1 = [
             i
             for i, tag in enumerate(tags1)
             if tag and not any(other and tag.is_equal(other, **is_equal_opts) for other in tags2)
         ]
```

### Comparing `returnn-1.20230630.233220/returnn/tf/layers/rec.py` & `returnn-1.20230630.93532/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/layers/segmental_model.py` & `returnn-1.20230630.93532/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/layers/signal_processing.py` & `returnn-1.20230630.93532/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/layers/variable.py` & `returnn-1.20230630.93532/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/native_op.py` & `returnn-1.20230630.93532/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/network.py` & `returnn-1.20230630.93532/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/sprint.py` & `returnn-1.20230630.93532/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/updater.py` & `returnn-1.20230630.93532/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/util/basic.py` & `returnn-1.20230630.93532/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/util/data.py` & `returnn-1.20230630.93532/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/util/gradient_checkpoint.py` & `returnn-1.20230630.93532/returnn/tf/util/gradient_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/util/ken_lm.py` & `returnn-1.20230630.93532/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/tf/util/open_fst.py` & `returnn-1.20230630.93532/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/data/pipeline.py` & `returnn-1.20230630.93532/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230630.93532/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/data/tensor_utils.py` & `returnn-1.20230630.93532/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/distributed.py` & `returnn-1.20230630.93532/returnn/torch/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/engine.py` & `returnn-1.20230630.93532/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/frontend/_backend.py` & `returnn-1.20230630.93532/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/frontend/_rand.py` & `returnn-1.20230630.93532/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/frontend/bridge.py` & `returnn-1.20230630.93532/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/torch/updater.py` & `returnn-1.20230630.93532/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/basic.py` & `returnn-1.20230630.93532/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/better_exchook.py` & `returnn-1.20230630.93532/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/bpe.py` & `returnn-1.20230630.93532/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/debug.py` & `returnn-1.20230630.93532/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/debug_helpers.py` & `returnn-1.20230630.93532/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/fsa.py` & `returnn-1.20230630.93532/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230630.93532/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/pprint.py` & `returnn-1.20230630.93532/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/py-to-pickle.cpp` & `returnn-1.20230630.93532/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/sig_proc.py` & `returnn-1.20230630.93532/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn/util/task_system.py` & `returnn-1.20230630.93532/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/returnn.egg-info/PKG-INFO` & `returnn-1.20230630.93532/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230630.233220
+Version: 1.20230630.93532
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230630.233220/returnn.egg-info/SOURCES.txt` & `returnn-1.20230630.93532/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/setup.py` & `returnn-1.20230630.93532/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/DummySprintExec.py` & `returnn-1.20230630.93532/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230630.93532/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230630.93532/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230630.93532/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/_set_num_threads1.py` & `returnn-1.20230630.93532/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/_setup_test_env.py` & `returnn-1.20230630.93532/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/bpe-unicode-demo.codes` & `returnn-1.20230630.93532/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/bpe-unicode-demo.vocab` & `returnn-1.20230630.93532/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/lexicon_opt.isyms` & `returnn-1.20230630.93532/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/lexicon_opt.jpg` & `returnn-1.20230630.93532/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/lint_common.py` & `returnn-1.20230630.93532/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/pycharm-inspect.py` & `returnn-1.20230630.93532/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/pylint.py` & `returnn-1.20230630.93532/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/returnn-as-framework.py` & `returnn-1.20230630.93532/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/rf_utils.py` & `returnn-1.20230630.93532/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/spelling.dic` & `returnn-1.20230630.93532/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_Config.py` & `returnn-1.20230630.93532/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_Dataset.py` & `returnn-1.20230630.93532/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_Fsa.py` & `returnn-1.20230630.93532/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_GeneratingDataset.py` & `returnn-1.20230630.93532/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_HDFDataset.py` & `returnn-1.20230630.93532/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_LearningRateControl.py` & `returnn-1.20230630.93532/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_Log.py` & `returnn-1.20230630.93532/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_MultiProcDataset.py` & `returnn-1.20230630.93532/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_PTDataset.py` & `returnn-1.20230630.93532/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_Pretrain.py` & `returnn-1.20230630.93532/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_ResNet.py` & `returnn-1.20230630.93532/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_SprintDataset.py` & `returnn-1.20230630.93532/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_SprintInterface.py` & `returnn-1.20230630.93532/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_TFEngine.py` & `returnn-1.20230630.93532/tests/test_TFEngine.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         batch.add_frames(seq_idx=seq_idx, seq_start_frame=0, length=dataset.get_seq_length(seq_idx))
         input_batches.append(batch)
     batch_generator = iter(input_batches)
     batches = BatchSetGenerator(dataset, generator=batch_generator)
     from returnn.tf.data_pipeline import FeedDictDataProvider
 
     data_provider = FeedDictDataProvider(
-        extern_data=extern_data, data_keys=["data", "classes"], dataset=dataset, batches=batches
+        tf_session=session, extern_data=extern_data, data_keys=["data", "classes"], dataset=dataset, batches=batches
     )
 
     # The values that happen to be produced by DummyDataset for the two sequences.
     expected_first_data = [[-0.5, -0.4], [-0.4, -0.3]]
     expected_last_data = [[0.3, 0.4], [0.4, -0.5]]
     expected_classes = [[1, 2, 0, 1, 2], [2, 0, 1, 2, 0]]
```

### Comparing `returnn-1.20230630.233220/tests/test_TFNativeOp.py` & `returnn-1.20230630.93532/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_TFNetworkLayer.py` & `returnn-1.20230630.93532/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230630.93532/tests/test_TFNetworkRecLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2729,15 +2729,15 @@
         net = TFNetwork(extern_data=extern_data, search_flag=True, train_flag=False, config=config)
         net.construct_from_dict(net_dict)
 
         out_layer = net.layers["output"]
         assert isinstance(out_layer, RecLayer)
         net.initialize_params(session)
         data_provider = FeedDictDataProvider(
-            extern_data=extern_data, data_keys=["data"], dataset=dataset, batches=batches
+            tf_session=session, extern_data=extern_data, data_keys=["data"], dataset=dataset, batches=batches
         )
         feed_dict, meta_step_info = data_provider.get_feed_dict(single_threaded=True)
         try:
             print("Output:")
             out = session.run(out_layer.output.placeholder, feed_dict=feed_dict)
             pprint(out)
         except Exception as exc:
@@ -3436,14 +3436,15 @@
         out_layer = net.layers["output"]
         assert isinstance(out_layer, RecLayer)
         assert isinstance(out_layer.cell, _SubnetworkRecCell)
 
         with tf_compat.v1.Session() as session:
             net.initialize_params(session)
             data_provider = FeedDictDataProvider(
+                tf_session=session,
                 extern_data=extern_data,
                 data_keys=["data", "classes"],
                 dataset=dataset,
                 batches=batches,
             )
             feed_dict, meta_step_info = data_provider.get_feed_dict(single_threaded=True)
             if isinstance(net.train_flag, tf.Tensor):
@@ -3919,14 +3920,15 @@
         batches = BatchSetGenerator(dataset, generator=batch_generator)
         out_layer = net.layers["output"]
         assert isinstance(out_layer, RecLayer)
         assert isinstance(out_layer.cell, _SubnetworkRecCell)
 
         net.initialize_params(session)
         data_provider = FeedDictDataProvider(
+            tf_session=session,
             extern_data=extern_data,
             data_keys=["data", "classes", "att_weights", "att_weights_sizes"],
             dataset=dataset,
             batches=batches,
         )
         feed_dict, meta_step_info = data_provider.get_feed_dict(single_threaded=True)
         if isinstance(net.train_flag, tf.Tensor):
@@ -4247,14 +4249,15 @@
             net.construct_from_dict(net_dict)
 
             out_layer = net.layers["output"]
             assert isinstance(out_layer, RecLayer)
             assert isinstance(out_layer.cell, _SubnetworkRecCell)
             net.initialize_params(session)
             data_provider = FeedDictDataProvider(
+                tf_session=session,
                 extern_data=extern_data,
                 data_keys=["data", "classes"] if train_flag else ["data"],
                 dataset=dataset,
                 batches=batches,
             )
             feed_dict, meta_step_info = data_provider.get_feed_dict(single_threaded=True)
             if isinstance(net.train_flag, tf.Tensor):
@@ -4527,14 +4530,15 @@
             net.construct_from_dict(net_dict)
 
             out_layer = net.layers["output"]
             assert isinstance(out_layer, RecLayer)
             assert isinstance(out_layer.cell, _SubnetworkRecCell)
             net.initialize_params(session)
             data_provider = FeedDictDataProvider(
+                tf_session=session,
                 extern_data=extern_data,
                 data_keys=["data", "classes"] if train_flag else ["data"],
                 dataset=dataset,
                 batches=batches,
             )
             feed_dict, meta_step_info = data_provider.get_feed_dict(single_threaded=True)
             if isinstance(net.train_flag, tf.Tensor):
```

### Comparing `returnn-1.20230630.233220/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230630.93532/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_TFUpdater.py` & `returnn-1.20230630.93532/tests/test_TFUpdater.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,15 @@
             recurrent_net=network.recurrent,
             batch_size=100,
             max_seqs=10,
             max_seq_length=sys.maxsize,
             used_data_keys=network.used_data_keys,
         )
         data_provider = FeedDictDataProvider(
+            tf_session=session,
             extern_data=extern_data,
             data_keys=network.used_data_keys,
             dataset=dataset,
             batches=batches,
         )
         feed_dict, _ = data_provider.get_feed_dict(single_threaded=True)
         session.run(updater.get_optim_op(), feed_dict=feed_dict)
@@ -277,14 +278,15 @@
             recurrent_net=network.recurrent,
             batch_size=100,
             max_seqs=10,
             max_seq_length=sys.maxsize,
             used_data_keys=network.used_data_keys,
         )
         data_provider = FeedDictDataProvider(
+            tf_session=session,
             extern_data=extern_data,
             data_keys=network.used_data_keys,
             dataset=dataset,
             batches=batches,
         )
         feed_dict, _ = data_provider.get_feed_dict(single_threaded=True)
         session.run(update_op, feed_dict=feed_dict)
@@ -436,14 +438,15 @@
             recurrent_net=network.recurrent,
             batch_size=100,
             max_seqs=10,
             max_seq_length=sys.maxsize,
             used_data_keys=network.used_data_keys,
         )
         data_provider = FeedDictDataProvider(
+            tf_session=session,
             extern_data=extern_data,
             data_keys=network.used_data_keys,
             dataset=dataset,
             batches=batches,
         )
         feed_dict, _ = data_provider.get_feed_dict(single_threaded=True)
         session.run(optim_op, feed_dict=feed_dict)
@@ -500,14 +503,15 @@
             recurrent_net=network.recurrent,
             batch_size=100,
             max_seqs=10,
             max_seq_length=sys.maxsize,
             used_data_keys=network.used_data_keys,
         )
         data_provider = FeedDictDataProvider(
+            tf_session=session,
             extern_data=extern_data,
             data_keys=network.used_data_keys,
             dataset=dataset,
             batches=batches,
         )
         feed_dict, _ = data_provider.get_feed_dict(single_threaded=True)
         session.run(optim_op, feed_dict=feed_dict)
```

### Comparing `returnn-1.20230630.233220/tests/test_TFUtil.py` & `returnn-1.20230630.93532/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_TF_determinism.py` & `returnn-1.20230630.93532/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_TaskSystem.py` & `returnn-1.20230630.93532/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230630.93532/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_TranslationDataset.py` & `returnn-1.20230630.93532/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_Util.py` & `returnn-1.20230630.93532/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_demos.py` & `returnn-1.20230630.93532/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_fork_exec.py` & `returnn-1.20230630.93532/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_hdf_dump.py` & `returnn-1.20230630.93532/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_array.py` & `returnn-1.20230630.93532/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_attention.py` & `returnn-1.20230630.93532/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_base.py` & `returnn-1.20230630.93532/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_cond.py` & `returnn-1.20230630.93532/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_container.py` & `returnn-1.20230630.93532/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_conv.py` & `returnn-1.20230630.93532/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_encoder_conformer.py` & `returnn-1.20230630.93532/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_loop.py` & `returnn-1.20230630.93532/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_math.py` & `returnn-1.20230630.93532/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_normalization.py` & `returnn-1.20230630.93532/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_rec.py` & `returnn-1.20230630.93532/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_reduce.py` & `returnn-1.20230630.93532/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_rf_signal.py` & `returnn-1.20230630.93532/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_tensor.py` & `returnn-1.20230630.93532/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_tools.py` & `returnn-1.20230630.93532/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_torch_engine.py` & `returnn-1.20230630.93532/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_torch_frontend.py` & `returnn-1.20230630.93532/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tests/test_torch_internal_frontend.py` & `returnn-1.20230630.93532/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/analyze-dataset-batches.py` & `returnn-1.20230630.93532/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/bliss-collect-seq-lens.py` & `returnn-1.20230630.93532/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/bliss-dump-text.py` & `returnn-1.20230630.93532/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/bliss-get-segment-names.py` & `returnn-1.20230630.93532/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/bliss-to-ogg-zip.py` & `returnn-1.20230630.93532/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/bpe-create-lexicon.py` & `returnn-1.20230630.93532/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/calculate-word-error-rate.py` & `returnn-1.20230630.93532/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/cleanup-old-models.py` & `returnn-1.20230630.93532/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/collect-orth-symbols.py` & `returnn-1.20230630.93532/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/collect-words.py` & `returnn-1.20230630.93532/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/compile_native_op.py` & `returnn-1.20230630.93532/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/compile_tf_graph.py` & `returnn-1.20230630.93532/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/debug-dump-search-scores.py` & `returnn-1.20230630.93532/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/debug-plot-search-scores.py` & `returnn-1.20230630.93532/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/dump-dataset-raw-strings.py` & `returnn-1.20230630.93532/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/dump-dataset.py` & `returnn-1.20230630.93532/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/dump-forward-stats.py` & `returnn-1.20230630.93532/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/dump-forward.py` & `returnn-1.20230630.93532/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/dump-network-json.py` & `returnn-1.20230630.93532/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/dump-pickle.py` & `returnn-1.20230630.93532/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230630.93532/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/get-attention-weights.py` & `returnn-1.20230630.93532/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/get-best-model-epoch.py` & `returnn-1.20230630.93532/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/hdf_dump.py` & `returnn-1.20230630.93532/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230630.93532/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/import-blocks-mt-model.py` & `returnn-1.20230630.93532/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/import-t2t-mt-model.py` & `returnn-1.20230630.93532/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/Makefile` & `returnn-1.20230630.93532/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/README.md` & `returnn-1.20230630.93532/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/example/README.md` & `returnn-1.20230630.93532/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230630.93532/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230630.93532/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230630.93532/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/file.h` & `returnn-1.20230630.93532/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230630.93532/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230630.93532/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/main.cc` & `returnn-1.20230630.93532/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230630.93532/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230630.93532/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230630.93532/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/tf_avg_checkpoints.py` & `returnn-1.20230630.93532/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/tf_inspect_checkpoint.py` & `returnn-1.20230630.93532/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/tf_inspect_summary_log.py` & `returnn-1.20230630.93532/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230630.233220/tools/torch_export_to_onnx.py` & `returnn-1.20230630.93532/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

