# Comparing `tmp/jittor-1.3.8.4.tar.gz` & `tmp/jittor-1.3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jittor-1.3.8.4.tar", last modified: Tue Jun 27 14:24:25 2023, max compression
+gzip compressed data, was "jittor-1.3.8.5.tar", last modified: Fri Jun 30 15:33:00 2023, max compression
```

## Comparing `jittor-1.3.8.4.tar` & `jittor-1.3.8.5.tar`

### file list

```diff
@@ -1,795 +1,795 @@
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.095244 jittor-1.3.8.4/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11613 2023-05-01 08:04:48.000000 jittor-1.3.8.4/LICENSE.txt
--rw-rw-r--   0 cjld      (1000) cjld      (1000)       88 2021-07-31 06:19:50.000000 jittor-1.3.8.4/MANIFEST.in
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11712 2023-06-27 14:24:25.095244 jittor-1.3.8.4/PKG-INFO
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11809 2023-03-31 13:28:11.000000 jittor-1.3.8.4/README.md
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.954411 jittor-1.3.8.4/python/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    67082 2023-06-27 14:21:54.000000 jittor-1.3.8.4/python/jittor/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   244353 2022-09-15 16:59:59.000000 jittor-1.3.8.4/python/jittor/__init__.pyi
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6545 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/attention.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/ccl/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)       86 2022-12-02 14:36:01.000000 jittor-1.3.8.4/python/jittor/ccl/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8866 2022-12-02 14:36:01.000000 jittor-1.3.8.4/python/jittor/ccl/ccl_2d.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10077 2022-12-02 14:36:01.000000 jittor-1.3.8.4/python/jittor/ccl/ccl_3d.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11051 2022-12-02 14:36:01.000000 jittor-1.3.8.4/python/jittor/ccl/ccl_link.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    24872 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/compile_extern.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    54031 2023-05-13 22:54:20.000000 jittor-1.3.8.4/python/jittor/compiler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9039 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/contrib.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/dataset/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      201 2023-01-07 09:03:52.000000 jittor-1.3.8.4/python/jittor/dataset/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6439 2021-06-16 12:20:56.000000 jittor-1.3.8.4/python/jittor/dataset/cifar.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    27453 2023-06-09 18:33:24.000000 jittor-1.3.8.4/python/jittor/dataset/dataset.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8320 2021-09-04 06:27:26.000000 jittor-1.3.8.4/python/jittor/dataset/mnist.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3323 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/dataset/sampler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2326 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/dataset/utils.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2410 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/dataset/voc.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/demo/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3591 2022-04-04 06:54:03.000000 jittor-1.3.8.4/python/jittor/demo/simple_cgan.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    15663 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/depthwise_conv.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6546 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/distributions.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/einops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      262 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8494 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/_backends.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    33864 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/einops.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/einops/experimental/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)        0 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/experimental/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15167 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/experimental/indexing.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/einops/layers/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2933 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/layers/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8720 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/layers/_einmix.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2057 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/layers/jittor.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6848 2022-11-07 04:02:17.000000 jittor-1.3.8.4/python/jittor/einops/parsing.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.954411 jittor-1.3.8.4/python/jittor/extern/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/extern/acl/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2379 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/acl/acl_compiler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    14964 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/acl/acl_error_code.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11204 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/acl/acl_jittor.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      644 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/acl/acl_jittor.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/extern/corex/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3816 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/corex/corex_compiler.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.954411 jittor-1.3.8.4/python/jittor/extern/cuda/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.943577 jittor-1.3.8.4/python/jittor/extern/cuda/cub/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/extern/cuda/cub/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     9072 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/inc/cub_test.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3918 2023-06-06 14:46:30.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      911 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3424 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_argsort_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      931 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_argsort_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4891 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      809 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1144 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_test_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      624 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_test_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3679 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_where_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1146 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_where_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.943577 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/inc/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      973 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/inc/cublas_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4418 2023-05-16 15:04:55.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      905 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5778 2023-05-13 23:06:10.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      953 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4383 2023-06-27 14:08:09.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      771 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      879 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_test_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      639 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12200 2021-07-26 07:27:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/src/cublas_matmul_test.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      990 2023-06-18 12:13:08.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/src/cublas_wrapper.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1606 2020-12-03 05:10:19.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cublas/src/helper_cublas.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.943577 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/inc/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4906 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/inc/cudnn_rnn_descriptor.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      842 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/inc/cudnn_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11561 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1143 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11327 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1151 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11535 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1029 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12570 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1116 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12027 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1121 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12423 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1061 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8286 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1470 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9384 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1375 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1093 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      628 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    39400 2021-12-30 07:13:56.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/src/cudnn_conv_test.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2914 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/src/cudnn_rnn_descriptor.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1070 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/src/cudnn_wrapper.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      161 2021-07-26 07:24:52.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/src/helper_cudnn.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.943577 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6280 2022-03-30 06:36:09.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/inc/cufft_utils.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      717 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/inc/cufft_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/ops/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3201 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      821 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/src/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1002 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cufft/src/cufft_wrapper.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.943577 jittor-1.3.8.4/python/jittor/extern/cuda/curand/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/curand/inc/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      632 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/curand/inc/curand_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/curand/ops/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1632 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/curand/ops/curand_random_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      759 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/curand/ops/curand_random_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/curand/src/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1078 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/curand/src/curand_wrapper.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1933 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/curand/src/helper_curand.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.954411 jittor-1.3.8.4/python/jittor/extern/cuda/cutt/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1052 2022-05-26 06:57:29.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_test_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      629 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_test_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3868 2023-05-16 06:12:13.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      775 2021-04-15 10:38:17.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      888 2021-11-01 03:42:19.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      559 2021-07-26 07:18:24.000000 jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/inc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      588 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/extern/cuda/inc/fp16_dev.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5639 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/extern/cuda/inc/fp16_emu.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12641 2022-10-25 03:25:21.000000 jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_cuda.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1173 2023-04-08 05:52:12.000000 jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_functions.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    27554 2023-04-08 05:52:07.000000 jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_image.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    33798 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_string.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    14855 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_timer.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.954411 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/inc/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      656 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/inc/nccl_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2033 2023-06-21 07:07:38.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_all_gather_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      782 2023-06-21 06:59:59.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_all_gather_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1866 2023-06-21 06:59:07.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      782 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1886 2023-06-21 06:59:10.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      808 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1972 2023-06-21 06:59:31.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      799 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3785 2022-05-26 06:57:29.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_test_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      644 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/src/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1923 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/cuda/nccl/src/nccl_wrapper.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/cuda/src/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1323 2021-07-26 07:15:57.000000 jittor-1.3.8.4/python/jittor/extern/cuda/src/fp16_dev.cu
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5303 2022-07-04 16:11:21.000000 jittor-1.3.8.4/python/jittor/extern/cuda/src/fp16_emu.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11787 2021-07-26 07:13:54.000000 jittor-1.3.8.4/python/jittor/extern/cuda/src/helper_cuda.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/llvm/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15734 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/extern/llvm/jt_alignment_from_assumptions.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.954411 jittor-1.3.8.4/python/jittor/extern/mkl/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/mkl/ops/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    36034 2022-03-22 14:48:20.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/cpu_cnn_inference_f32.cpp
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8788 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1043 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8850 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1048 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7552 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1035 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2210 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_matmul_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      762 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_matmul_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      810 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_test_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      595 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.954411 jittor-1.3.8.4/python/jittor/extern/mpi/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/mpi/inc/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2014 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/inc/mpi_wrapper.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.986911 jittor-1.3.8.4/python/jittor/extern/mpi/ops/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2899 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_all_reduce_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1110 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_all_reduce_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2222 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_broadcast_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1028 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_broadcast_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2989 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_reduce_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1171 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_reduce_op.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1102 2022-05-26 06:57:29.000000 jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_test_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      641 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_test_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.997744 jittor-1.3.8.4/python/jittor/extern/mpi/src/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3452 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/extern/mpi/src/mpi_wrapper.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.997744 jittor-1.3.8.4/python/jittor/extern/rocm/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   115033 2022-08-09 11:21:18.000000 jittor-1.3.8.4/python/jittor/extern/rocm/rocm_cache.tar.gz
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6235 2022-10-26 06:26:28.000000 jittor-1.3.8.4/python/jittor/extern/rocm/rocm_compiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1712 2022-08-09 11:21:18.000000 jittor-1.3.8.4/python/jittor/extern/rocm/rocm_config.cc
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      497 2022-08-09 11:21:18.000000 jittor-1.3.8.4/python/jittor/extern/rocm/rocm_config.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      538 2022-07-04 16:11:21.000000 jittor-1.3.8.4/python/jittor/extern/rocm/rocm_jittor.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6598 2022-08-09 11:21:18.000000 jittor-1.3.8.4/python/jittor/extern/rocm/rocm_wrapper.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    23687 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/init.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1715 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/init_cupy.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    16949 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/linalg.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.997744 jittor-1.3.8.4/python/jittor/loss3d/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      105 2021-06-30 08:15:49.000000 jittor-1.3.8.4/python/jittor/loss3d/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5553 2021-06-30 08:15:49.000000 jittor-1.3.8.4/python/jittor/loss3d/chamfer.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    16008 2021-06-30 08:15:49.000000 jittor-1.3.8.4/python/jittor/loss3d/emd.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7936 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/lr_scheduler.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.997744 jittor-1.3.8.4/python/jittor/math_util/
--rw-r--r--   0 cjld      (1000) cjld      (1000)       64 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/math_util/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    15722 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/math_util/gamma.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      671 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/math_util/igamma.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.997744 jittor-1.3.8.4/python/jittor/math_util/src/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5520 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/math_util/src/gamma_grad.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    29181 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/math_util/src/igamma.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    76767 2023-06-06 14:33:24.000000 jittor-1.3.8.4/python/jittor/misc.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.997744 jittor-1.3.8.4/python/jittor/models/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      513 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/models/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2246 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/alexnet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6745 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/densenet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6328 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/googlenet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    11821 2022-04-04 06:54:03.000000 jittor-1.3.8.4/python/jittor/models/inception.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4821 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/mnasnet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4602 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/mobilenet.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8032 2021-10-19 11:51:01.000000 jittor-1.3.8.4/python/jittor/models/res2net.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9657 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/resnet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5575 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/shufflenetv2.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4028 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/squeezenet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3711 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/models/vgg.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)   122453 2023-06-09 17:01:30.000000 jittor-1.3.8.4/python/jittor/nn.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.008577 jittor-1.3.8.4/python/jittor/notebook/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.019411 jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      297 2021-07-14 13:51:52.000000 jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/README.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   243006 2021-07-14 13:51:52.000000 jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/mnist.png
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     5047 2021-07-14 13:51:52.000000 jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 0 --- 介绍与安装.ipynb
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    29117 2021-07-14 13:51:52.000000 jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 1 --- 基本概念.ipynb
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    62291 2022-03-15 13:17:00.000000 jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 2 --- 如何训练一个简单线性回归.ipynb
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   136962 2022-03-15 13:17:00.000000 jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 3 --- 尝试解决一个实际问题.ipynb
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6314 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/ConditionGAN.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3487 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/ConditionGAN.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6752 2022-04-04 06:54:03.000000 jittor-1.3.8.4/python/jittor/notebook/ConditionGAN.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10677 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/LSGAN.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7897 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/LSGAN.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10677 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/notebook/LSGAN.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      238 2022-03-15 13:17:00.000000 jittor-1.3.8.4/python/jittor/notebook/__main__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1243 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/basics.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1250 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/basics.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2111 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/notebook/basics.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2232 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/custom_op.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2249 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/custom_op.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2760 2021-07-16 06:09:15.000000 jittor-1.3.8.4/python/jittor/notebook/custom_op.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1996 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/example.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2152 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/example.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3099 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/notebook/example.src.md
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.019411 jittor-1.3.8.4/python/jittor/notebook/figs/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    41082 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/notebook/figs/mop.svg
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2203 2022-03-22 14:48:20.000000 jittor-1.3.8.4/python/jittor/notebook/md_to_ipynb.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     7817 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/meta_op.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8068 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/meta_op.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    10843 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/notebook/meta_op.src.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      235 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/profiler.cn.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      264 2021-10-11 05:54:17.000000 jittor-1.3.8.4/python/jittor/notebook/profiler.md
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      459 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/notebook/profiler.src.md
--rw-r--r--   0 cjld      (1000) cjld      (1000)    23255 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/optim.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.019411 jittor-1.3.8.4/python/jittor/other/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4777 2023-06-21 04:30:04.000000 jittor-1.3.8.4/python/jittor/other/code_softmax.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    29598 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/pool.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    35074 2023-05-13 04:29:28.000000 jittor-1.3.8.4/python/jittor/pyjt_compiler.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.019411 jittor-1.3.8.4/python/jittor/script/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1464 2021-05-12 08:13:24.000000 jittor-1.3.8.4/python/jittor/script/Dockerfile_cuda11
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      890 2021-06-19 09:21:11.000000 jittor-1.3.8.4/python/jittor/script/build_aarch64_mkl.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      893 2021-05-04 00:57:17.000000 jittor-1.3.8.4/python/jittor/script/converter_server.sh
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4134 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/script/inference_perf.py
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)     2265 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/script/install.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2543 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/script/install_llvm.sh
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)      632 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/script/install_mkl.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1569 2022-03-15 13:17:00.000000 jittor-1.3.8.4/python/jittor/script/make_doc.py
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)     4359 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/script/tmpi
--rwxrwxr-x   0 cjld      (1000) cjld      (1000)      144 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/script/update.sh
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1759 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/sparse.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.030244 jittor-1.3.8.4/python/jittor/src/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1326 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/common.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1056 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/core.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1573 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/event_queue.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2392 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/event_queue.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    26917 2023-06-23 10:06:02.000000 jittor-1.3.8.4/python/jittor/src/executor.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1043 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/executor.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8249 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/fused_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1936 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/fused_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      643 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/fuser.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    10134 2023-05-22 01:02:36.000000 jittor-1.3.8.4/python/jittor/src/grad.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      712 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/grad.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5885 2023-05-16 07:23:39.000000 jittor-1.3.8.4/python/jittor/src/graph.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4724 2023-05-16 07:23:32.000000 jittor-1.3.8.4/python/jittor/src/graph.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2730 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/init.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1091 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/init.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9383 2023-06-04 21:24:53.000000 jittor-1.3.8.4/python/jittor/src/jit_compiler.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      652 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/jit_compiler.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3262 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/jit_key.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7600 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/jit_key.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2031 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/lock.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      864 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/lock.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.030244 jittor-1.3.8.4/python/jittor/src/mem/
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.030244 jittor-1.3.8.4/python/jittor/src/mem/allocator/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1188 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/aligned_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      779 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/aligned_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1407 2023-06-21 06:37:27.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_device_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      805 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_device_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1107 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_dual_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4172 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_dual_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1087 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_host_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      802 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_host_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1190 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_managed_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      856 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_managed_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1501 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/foreign_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      948 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/foreign_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1127 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/nfef_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1000 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/nfef_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9259 2023-06-21 06:33:15.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/sfrl_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3883 2023-06-04 16:31:06.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/sfrl_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1781 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/stat_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1071 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/stat_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3765 2023-06-21 06:30:33.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/temp_allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2234 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator/temp_allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5428 2023-06-18 12:30:56.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2237 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/allocator.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11462 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/mem_info.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1019 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/mem_info.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8807 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/swap.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2427 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/mem/swap.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6373 2023-05-22 03:19:52.000000 jittor-1.3.8.4/python/jittor/src/memory_profiler.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1429 2023-05-22 03:29:05.000000 jittor-1.3.8.4/python/jittor/src/memory_profiler.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.041077 jittor-1.3.8.4/python/jittor/src/misc/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      485 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/cpu_atomic.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1820 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/cpu_atomic.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2362 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/cpu_math.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      490 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/cpu_math.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1570 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/cstr.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7264 2023-05-13 08:27:34.000000 jittor-1.3.8.4/python/jittor/src/misc/cuda_atomic.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2954 2023-06-18 09:27:45.000000 jittor-1.3.8.4/python/jittor/src/misc/cuda_flags.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1061 2023-06-18 09:24:17.000000 jittor-1.3.8.4/python/jittor/src/misc/cuda_flags.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2191 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/cuda_limits.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      662 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/deleter.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2538 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/fast_shared_ptr.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1000 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/hash.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      864 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/intrin.h
--rwxr-xr-x   0 cjld      (1000) cjld      (1000)   326707 2023-03-30 05:25:05.000000 jittor-1.3.8.4/python/jittor/src/misc/miniz.cc
--rwxr-xr-x   0 cjld      (1000) cjld      (1000)    70346 2023-06-23 10:26:15.000000 jittor-1.3.8.4/python/jittor/src/misc/miniz.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2519 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/nan_checker.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3046 2023-05-13 12:40:54.000000 jittor-1.3.8.4/python/jittor/src/misc/nan_checker.cu
--rw-r--r--   0 cjld      (1000) cjld      (1000)      403 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/nan_checker.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5953 2023-05-16 04:56:35.000000 jittor-1.3.8.4/python/jittor/src/misc/nano_string.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7634 2023-05-13 20:28:36.000000 jittor-1.3.8.4/python/jittor/src/misc/nano_string.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9048 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/nano_vector.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3368 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/ring_buffer.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6868 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/ring_buffer.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1801 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/stack_vector.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1503 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/misc/string_view_map.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7512 2023-05-16 14:49:25.000000 jittor-1.3.8.4/python/jittor/src/node.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1902 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/numpy_func.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9475 2023-05-19 23:16:17.000000 jittor-1.3.8.4/python/jittor/src/op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2828 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    43093 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/op_compiler.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1766 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/op_compiler.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.051911 jittor-1.3.8.4/python/jittor/src/ops/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7467 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/arg_reduce_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1761 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/arg_reduce_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6273 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/argsort_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2167 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/argsort_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4035 2023-06-04 21:24:23.000000 jittor-1.3.8.4/python/jittor/src/ops/array_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1098 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/array_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    15124 2023-05-16 05:07:55.000000 jittor-1.3.8.4/python/jittor/src/ops/binary_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      727 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/binary_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6900 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/broadcast_to_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2794 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/broadcast_to_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3650 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/candidate_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1945 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/candidate_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1211 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/clone_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      715 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/clone_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8685 2023-05-13 17:11:35.000000 jittor-1.3.8.4/python/jittor/src/ops/code_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)    10232 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/code_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1425 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/copy_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      694 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/copy_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      685 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/empty_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      607 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/empty_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5104 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/fetch_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2540 2023-06-04 20:08:00.000000 jittor-1.3.8.4/python/jittor/src/ops/fetch_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3766 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/fuse_transpose_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      774 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/fuse_transpose_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    19861 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/getitem_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1555 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/getitem_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2724 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/index_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1986 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/index_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5542 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/numpy_code_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3394 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/numpy_code_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1508 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/op_register.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1544 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/op_register.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1577 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/op_utils.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2072 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/random_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      686 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/random_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12858 2023-05-16 14:58:04.000000 jittor-1.3.8.4/python/jittor/src/ops/reduce_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1019 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/reduce_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5836 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/reindex_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4093 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/reindex_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5603 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/reindex_reduce_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3610 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/reindex_reduce_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2069 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/reshape_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1536 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/reshape_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1615 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/safe_clip_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1008 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/safe_clip_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12583 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/setitem_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1130 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/setitem_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3004 2023-05-13 19:25:10.000000 jittor-1.3.8.4/python/jittor/src/ops/tape_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1897 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/tape_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3745 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/ternary_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      735 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/ternary_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3808 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/transpose_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      761 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/transpose_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    26784 2023-05-13 12:41:11.000000 jittor-1.3.8.4/python/jittor/src/ops/unary_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      742 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/unary_op.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8196 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/where_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1232 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/ops/where_op.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.051911 jittor-1.3.8.4/python/jittor/src/opt/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    38841 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/expr.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5751 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/expr.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.051911 jittor-1.3.8.4/python/jittor/src/opt/gopt/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5549 2023-06-19 04:36:41.000000 jittor-1.3.8.4/python/jittor/src/opt/gopt/setitem_gopt.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3084 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/jit_searcher.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      748 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/jit_searcher.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    35269 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/kernel_ir.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8192 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/kernel_ir.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.062744 jittor-1.3.8.4/python/jittor/src/opt/pass/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2071 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/assume_aligned_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      572 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/assume_aligned_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      613 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/atomic_tuner_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6886 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/check_cache_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      613 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/check_cache_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1494 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/compile_shapes_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      572 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/compile_shapes_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1644 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/const_var_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      562 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/const_var_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1391 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/expand_empty_block_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      582 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/expand_empty_block_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6960 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/fake_main_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      557 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/fake_main_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3545 2023-05-11 12:13:21.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/float_atomic_fix_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      590 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/float_atomic_fix_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1480 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/insert_profile_loop_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      585 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/insert_profile_loop_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4427 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/loop_to_func_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      564 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/loop_to_func_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12889 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/loop_var_analyze_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      662 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/loop_var_analyze_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1246 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/mark_raw_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      554 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/mark_raw_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2283 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/merge_loop_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      560 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/merge_loop_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6195 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/merge_loop_var_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      570 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/merge_loop_var_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      556 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/parallel_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      680 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      732 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1490 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/remove_intermediate_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      587 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/remove_intermediate_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      897 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/remove_loop_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      620 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/remove_loop_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      633 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/rename_loop_index_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      579 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/rename_loop_index_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2306 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/reorder_loop_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      610 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/reorder_loop_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3452 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/replace_for_num_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      868 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/replace_for_num_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5910 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/restride_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      556 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/restride_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      574 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/shared_reduce_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      604 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/solve_conflict_define_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      591 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/solve_conflict_define_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1362 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/split_loop_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      634 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/split_loop_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3719 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/unroll_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      562 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/unroll_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      944 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/use_movnt_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      610 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/use_movnt_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3411 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/vectorize_pass.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      559 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass/vectorize_pass.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4356 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass_manager.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1954 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/pass_manager.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.062744 jittor-1.3.8.4/python/jittor/src/opt/tuner/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2242 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/broadcast_tuner.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      670 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/broadcast_tuner.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    16851 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/conv_tuner.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      692 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/conv_tuner.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4058 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/matmul_tuner.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      622 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/matmul_tuner.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2601 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/reduce_tuner.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      689 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/reduce_tuner.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1139 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/reorder_tuner.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      593 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/reorder_tuner.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      655 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/tuner.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      709 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner/tuner.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2310 2023-06-04 21:11:55.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner_manager.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      797 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/tuner_manager.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7246 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/var_relay.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1733 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/opt/var_relay.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12891 2023-06-24 14:29:55.000000 jittor-1.3.8.4/python/jittor/src/parallel_compiler.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      610 2023-06-24 14:28:20.000000 jittor-1.3.8.4/python/jittor/src/parallel_compiler.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.062744 jittor-1.3.8.4/python/jittor/src/profiler/
--rw-r--r--   0 cjld      (1000) cjld      (1000)      913 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/cache_info.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      717 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/cache_info.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1882 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/memory_checker.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1080 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/memory_checker.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    21999 2023-05-16 04:35:30.000000 jittor-1.3.8.4/python/jittor/src/profiler/profiler.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2317 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/profiler.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1914 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/profiler_guard.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2224 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/replacement.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1311 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/replacement.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3423 2023-06-17 04:52:49.000000 jittor-1.3.8.4/python/jittor/src/profiler/simple_profiler.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2609 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/profiler/vtop.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.062744 jittor-1.3.8.4/python/jittor/src/pybind/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1313 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pybind/core.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)    16013 2023-05-16 04:35:32.000000 jittor-1.3.8.4/python/jittor/src/pybind/py_var_tracer.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1950 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pybind/py_var_tracer.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)      558 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pybind/py_var_tracer_interface.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.062744 jittor-1.3.8.4/python/jittor/src/pyjt/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2688 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/numpy.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4020 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/numpy.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2093 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_arg_printer.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1044 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_arg_printer.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6571 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_array_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1116 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_caller.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      551 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_caller.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    27629 2023-06-25 14:57:53.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_converter.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2248 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_obj_holder.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8751 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_ring_buffer.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1709 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/py_ring_buffer.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    15153 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/pyjt/pyjt_console.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.062744 jittor-1.3.8.4/python/jittor/src/test/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8024 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_expr.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      832 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_fast_shared_ptr.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2266 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_jit_key.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11949 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_kernel_ir.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2208 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_nano_vector.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      820 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_op_compiler.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3937 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_op_relay.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2040 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_setitem_op.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4738 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/test/test_sfrl_allocator.cc
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.073578 jittor-1.3.8.4/python/jittor/src/type/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6593 2023-05-13 22:53:57.000000 jittor-1.3.8.4/python/jittor/src/type/common_op_type.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6265 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/type/fp16_compute.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7484 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/type/fp16_op_type.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6873 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/types.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.073578 jittor-1.3.8.4/python/jittor/src/utils/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    15087 2023-05-13 08:17:57.000000 jittor-1.3.8.4/python/jittor/src/utils/cache_compile.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      746 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/cache_compile.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1706 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/cross_platform.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1286 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/flags.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      408 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/flags.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    20979 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/jit_utils.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)    21467 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/log.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9277 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/log.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1490 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/mwsr_list.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4766 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/mwsr_list.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     6721 2021-10-01 11:48:38.000000 jittor-1.3.8.4/python/jittor/src/utils/seh.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7262 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/str_utils.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1522 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/str_utils.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7975 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/tracer.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)      485 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/utils/tracer.h
--rw-rw-r--   0 cjld      (1000) cjld      (1000)       15 2021-10-01 11:48:38.000000 jittor-1.3.8.4/python/jittor/src/utils/vdp
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5563 2023-06-04 18:38:09.000000 jittor-1.3.8.4/python/jittor/src/var.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3286 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/var.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)    10521 2023-06-23 17:25:11.000000 jittor-1.3.8.4/python/jittor/src/var_holder.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)    10797 2023-06-23 15:08:13.000000 jittor-1.3.8.4/python/jittor/src/var_holder.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1202 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/var_slices.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2993 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/src/var_slices.h
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.084411 jittor-1.3.8.4/python/jittor/test/
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2927 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/__main__.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.084411 jittor-1.3.8.4/python/jittor/test/misc/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15224 2022-03-14 07:47:44.000000 jittor-1.3.8.4/python/jittor/test/misc/superglue.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.084411 jittor-1.3.8.4/python/jittor/test/perf/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     8216 2022-03-22 14:48:20.000000 jittor-1.3.8.4/python/jittor/test/perf/perf.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.084411 jittor-1.3.8.4/python/jittor/test/system/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      358 2020-12-07 05:07:32.000000 jittor-1.3.8.4/python/jittor/test/system/test_all.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:52.000000 jittor-1.3.8.4/python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:48.000000 jittor-1.3.8.4/python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:44.000000 jittor-1.3.8.4/python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:39.000000 jittor-1.3.8.4/python/jittor/test/system/test_cuda11.1_ubuntu18.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1844 2020-12-09 09:06:33.000000 jittor-1.3.8.4/python/jittor/test/system/test_cuda11.1_ubuntu20.04.sh
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1535 2020-12-09 09:06:26.000000 jittor-1.3.8.4/python/jittor/test/system/test_nocuda_ubuntu18.04.sh
--rw-r--r--   0 cjld      (1000) cjld      (1000)      661 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5310 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_acl.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3269 2022-09-01 03:11:16.000000 jittor-1.3.8.4/python/jittor/test/test_adamw.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3007 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_affine_grid.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1453 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_allocator.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1573 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_allocator2.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    12385 2021-08-04 11:28:54.000000 jittor-1.3.8.4/python/jittor/test/test_arg_pool_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5539 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_arg_reduce_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4327 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_argsort_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6742 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_array.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4192 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_asm_tuner.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2882 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_atomic_tuner.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2258 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_attention.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2134 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_auto_diff.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5576 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_batchnorm.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12199 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_benchmark.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2177 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_bicubic.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7256 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_binary_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1591 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_bmm.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4661 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_broadcast_to_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1819 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_broadcast_tuner.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4566 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_cache.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2662 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_candidate.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1143 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_clone.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    14087 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_code_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1137 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_compile_options.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6570 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_concat_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      963 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_console.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2464 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_contrib.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4874 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_conv_transpose.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6831 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_conv_tuner.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11127 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_core.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3460 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_cub_cumsum.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1538 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_cublas_test_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3801 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_cuda.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9134 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_cudnn_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1570 2022-04-23 08:12:38.000000 jittor-1.3.8.4/python/jittor/test/test_cumprod_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2986 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_custom_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      869 2020-09-16 07:12:03.000000 jittor-1.3.8.4/python/jittor/test/test_cutt.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     4068 2022-09-15 16:59:59.000000 jittor-1.3.8.4/python/jittor/test/test_cutt_transpose_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    10487 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_dataset.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1455 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_default_var.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4289 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_densenet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3130 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_depthwise_conv.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1571 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_digamma.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7920 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_distributions.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    28179 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_einops.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4462 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_einsum.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1138 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_emnist.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2195 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_error_msg.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2732 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_example.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3130 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_example_accumulate_grad.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1156 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_fetcher.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9165 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_fft_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1006 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_flags.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1958 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_fold.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12961 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_fp16.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9481 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_function.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    13063 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_fused_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1447 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_fuser.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1730 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_gamma_distribution.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6053 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_grad.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5585 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_group_conv_tuner.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1556 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_histc.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2239 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_hook.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2686 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_image_folder.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5361 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_inception.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2312 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_index_op.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3247 2021-10-22 06:53:31.000000 jittor-1.3.8.4/python/jittor/test/test_init.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1216 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_interpolation.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1002 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_jit_tests.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1867 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_jtune.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1889 2022-05-06 04:57:57.000000 jittor-1.3.8.4/python/jittor/test/test_knn.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1364 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_lazy_execution.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11030 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_linalg.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2211 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_load_pth.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1089 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_lock.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1813 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_log.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2073 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_longest_dis_fuse.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9002 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_loss.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3392 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_loss3d.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1702 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_lr_scheduler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3814 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_lstm.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    13954 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_matmul.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1648 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_matmul_tuner.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1263 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_mem.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3818 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_memory_profiler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2302 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_merge_loop_var_pass.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4523 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_merge_single_array_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6544 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_misc_issue.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    16899 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_misc_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8278 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_mkl_conv_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      648 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_mkl_test_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4056 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_models.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3220 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_mpi.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4369 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_mpi_batchnorm.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1879 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_mpi_in_py.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2374 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_mpi_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2615 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_nano_string.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1581 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_nano_vector.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      703 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_nccl.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5181 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_nccl_ops.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1495 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_new_fused_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5550 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_node.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1630 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_notebooks.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6193 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_numpy_code_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6353 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_op_compiler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1520 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_opt_state_dict.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1570 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_optimizer.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1883 2023-03-22 11:47:26.000000 jittor-1.3.8.4/python/jittor/test/test_optimizer_save_load.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3904 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_pad.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     7853 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_parallel_pass.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1196 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_param_list.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1462 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_profiler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8588 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_pytorch_converter.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3728 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_random_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4642 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_reduce_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1760 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_reduce_tuner.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11179 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_reindex_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3620 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_reindex_reduce_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3801 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_relu.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3383 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_reorder_tuner.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1670 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_repeat.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3237 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_reshape.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5310 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_resize_and_crop.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6181 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_resnet.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2217 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_ring_buffer.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3721 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_ring_buffer2.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    26660 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_rnn.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15920 2022-08-09 11:21:18.000000 jittor-1.3.8.4/python/jittor/test/test_rocm.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1721 2021-03-23 11:08:33.000000 jittor-1.3.8.4/python/jittor/test/test_sampler.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2368 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_search_sorted.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1549 2021-06-22 07:08:32.000000 jittor-1.3.8.4/python/jittor/test/test_searchsorted_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    15402 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_setitem.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1481 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_single_process_scope.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6304 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_slice.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1371 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_sparse.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1732 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_stop_fuse.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3872 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_superglue.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2088 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_ternary_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6552 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_trace_var.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1439 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_tracer.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    40470 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_transform.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5469 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_transpose_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4342 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_unary_op.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1869 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_unique.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2230 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_utils.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2074 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_var.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     3731 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_vgg.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2202 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_weightnorm.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2790 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/test/test_where_op.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.084411 jittor-1.3.8.4/python/jittor/transform/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    54004 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/transform/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    23971 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/transform/function_pil.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.084411 jittor-1.3.8.4/python/jittor/utils/
--rwxr-xr-x   0 cjld      (1000) cjld      (1000)     5419 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/asm_tuner.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      352 2022-12-01 04:53:11.000000 jittor-1.3.8.4/python/jittor/utils/bench_klo.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      685 2020-12-13 14:03:17.000000 jittor-1.3.8.4/python/jittor/utils/converter_server.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)   437003 2023-04-03 01:38:42.000000 jittor-1.3.8.4/python/jittor/utils/data.gz
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      662 2022-06-23 13:14:46.000000 jittor-1.3.8.4/python/jittor/utils/dlink_compiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1276 2022-03-15 13:17:00.000000 jittor-1.3.8.4/python/jittor/utils/dumpdef.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     9761 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/gen_pyi.py
--rwxr-xr-x   0 cjld      (1000) cjld      (1000)     1926 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/jtune.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2190 2021-10-01 11:48:38.000000 jittor-1.3.8.4/python/jittor/utils/local_doc_builder.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1214 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/nvtx.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     4895 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/polish.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2484 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/polish_centos.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1834 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/publish.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    28291 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/pytorch_converter.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)      837 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor/utils/tracer.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.095244 jittor-1.3.8.4/python/jittor/vcompiler/
--rw-r--r--   0 cjld      (1000) cjld      (1000)       24 2023-06-25 14:33:06.000000 jittor-1.3.8.4/python/jittor/vcompiler/__init__.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    35521 2023-06-25 14:33:37.000000 jittor-1.3.8.4/python/jittor/vcompiler/vcompiler.cc
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2371 2023-06-25 14:33:46.000000 jittor-1.3.8.4/python/jittor/vcompiler/vcompiler.h
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5028 2023-06-25 14:33:27.000000 jittor-1.3.8.4/python/jittor/vcompiler/vcompiler.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)       41 2021-06-18 14:24:21.000000 jittor-1.3.8.4/python/jittor/version
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2878 2023-04-04 18:16:13.000000 jittor-1.3.8.4/python/jittor/weightnorm.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:24.976077 jittor-1.3.8.4/python/jittor.egg-info/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    11712 2023-06-27 14:24:24.000000 jittor-1.3.8.4/python/jittor.egg-info/PKG-INFO
--rw-r--r--   0 cjld      (1000) cjld      (1000)    28436 2023-06-27 14:24:24.000000 jittor-1.3.8.4/python/jittor.egg-info/SOURCES.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)        1 2023-06-27 14:24:24.000000 jittor-1.3.8.4/python/jittor.egg-info/dependency_links.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       75 2023-06-27 14:24:24.000000 jittor-1.3.8.4/python/jittor.egg-info/requires.txt
--rw-r--r--   0 cjld      (1000) cjld      (1000)       20 2023-06-27 14:24:24.000000 jittor-1.3.8.4/python/jittor.egg-info/top_level.txt
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.095244 jittor-1.3.8.4/python/jittor_utils/
--rw-r--r--   0 cjld      (1000) cjld      (1000)    25368 2023-06-18 09:11:20.000000 jittor-1.3.8.4/python/jittor_utils/__init__.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)    15503 2022-03-22 14:48:20.000000 jittor-1.3.8.4/python/jittor_utils/auto_diff.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     1290 2022-05-08 11:48:51.000000 jittor-1.3.8.4/python/jittor_utils/auto_git_tag.py
-drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-27 14:24:25.095244 jittor-1.3.8.4/python/jittor_utils/class/
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      993 2021-10-12 06:29:13.000000 jittor-1.3.8.4/python/jittor_utils/class/motd
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      472 2021-10-12 06:29:13.000000 jittor-1.3.8.4/python/jittor_utils/class/setup.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5595 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor_utils/class/setup_env.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     1634 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor_utils/clean_cache.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3812 2021-10-01 11:48:38.000000 jittor-1.3.8.4/python/jittor_utils/config.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      710 2022-05-08 11:48:51.000000 jittor-1.3.8.4/python/jittor_utils/github_release.sh
--rw-r--r--   0 cjld      (1000) cjld      (1000)     6105 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor_utils/install_cuda.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      504 2021-10-01 11:48:38.000000 jittor-1.3.8.4/python/jittor_utils/install_msvc.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    12389 2023-06-23 09:31:05.000000 jittor-1.3.8.4/python/jittor_utils/load_pytorch.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)    10438 2023-03-30 09:43:29.000000 jittor-1.3.8.4/python/jittor_utils/load_pytorch_old.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2608 2022-04-22 13:37:44.000000 jittor-1.3.8.4/python/jittor_utils/lock.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     5441 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor_utils/misc.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     3093 2022-07-06 05:24:42.000000 jittor-1.3.8.4/python/jittor_utils/pack_offline.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      799 2021-10-12 06:29:13.000000 jittor-1.3.8.4/python/jittor_utils/pip_publish.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)      852 2021-10-13 11:17:19.000000 jittor-1.3.8.4/python/jittor_utils/query_cuda_cc.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     8822 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor_utils/ring_buffer.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)     2168 2023-05-01 08:04:48.000000 jittor-1.3.8.4/python/jittor_utils/student_queue.py
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2844 2022-09-15 16:59:59.000000 jittor-1.3.8.4/python/jittor_utils/translator.py
--rw-r--r--   0 cjld      (1000) cjld      (1000)       38 2023-06-27 14:24:25.095244 jittor-1.3.8.4/setup.cfg
--rw-rw-r--   0 cjld      (1000) cjld      (1000)     2464 2021-10-12 06:29:13.000000 jittor-1.3.8.4/setup.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.806691 jittor-1.3.8.5/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11613 2023-05-01 08:04:48.000000 jittor-1.3.8.5/LICENSE.txt
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)       88 2021-07-31 06:19:50.000000 jittor-1.3.8.5/MANIFEST.in
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11712 2023-06-30 15:33:00.806691 jittor-1.3.8.5/PKG-INFO
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11809 2023-03-31 13:28:11.000000 jittor-1.3.8.5/README.md
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.655024 jittor-1.3.8.5/python/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    67082 2023-06-30 15:31:25.000000 jittor-1.3.8.5/python/jittor/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   244353 2022-09-15 16:59:59.000000 jittor-1.3.8.5/python/jittor/__init__.pyi
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6545 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/attention.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/ccl/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)       86 2022-12-02 14:36:01.000000 jittor-1.3.8.5/python/jittor/ccl/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8866 2022-12-02 14:36:01.000000 jittor-1.3.8.5/python/jittor/ccl/ccl_2d.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    10077 2022-12-02 14:36:01.000000 jittor-1.3.8.5/python/jittor/ccl/ccl_3d.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    11051 2022-12-02 14:36:01.000000 jittor-1.3.8.5/python/jittor/ccl/ccl_link.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    24872 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/compile_extern.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    54090 2023-06-30 13:48:50.000000 jittor-1.3.8.5/python/jittor/compiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9039 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/contrib.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/dataset/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      201 2023-01-07 09:03:52.000000 jittor-1.3.8.5/python/jittor/dataset/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6439 2021-06-16 12:20:56.000000 jittor-1.3.8.5/python/jittor/dataset/cifar.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    27453 2023-06-09 18:33:24.000000 jittor-1.3.8.5/python/jittor/dataset/dataset.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8320 2021-09-04 06:27:26.000000 jittor-1.3.8.5/python/jittor/dataset/mnist.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3323 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/dataset/sampler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2326 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/dataset/utils.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2410 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/dataset/voc.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/demo/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3591 2022-04-04 06:54:03.000000 jittor-1.3.8.5/python/jittor/demo/simple_cgan.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15663 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/depthwise_conv.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6546 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/distributions.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/einops/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      262 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8494 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/_backends.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    33864 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/einops.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/einops/experimental/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)        0 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/experimental/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15167 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/experimental/indexing.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/einops/layers/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2933 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/layers/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8720 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/layers/_einmix.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2057 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/layers/jittor.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6848 2022-11-07 04:02:17.000000 jittor-1.3.8.5/python/jittor/einops/parsing.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/extern/acl/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3193 2023-06-30 14:46:51.000000 jittor-1.3.8.5/python/jittor/extern/acl/acl_compiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    14964 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/acl/acl_error_code.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11567 2023-06-30 14:39:28.000000 jittor-1.3.8.5/python/jittor/extern/acl/acl_jittor.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      644 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/acl/acl_jittor.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/extern/corex/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3816 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/corex/corex_compiler.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/cuda/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.633358 jittor-1.3.8.5/python/jittor/extern/cuda/cub/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/extern/cuda/cub/inc/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     9072 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/inc/cub_test.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3918 2023-06-06 14:46:30.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      911 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3424 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_argsort_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      931 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_argsort_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4891 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      809 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1144 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      624 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_test_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3679 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_where_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1146 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_where_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.633358 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      973 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/inc/cublas_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4418 2023-05-16 15:04:55.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      905 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5778 2023-05-13 23:06:10.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      953 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4383 2023-06-28 12:40:15.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      771 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      879 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      639 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/src/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    12200 2021-07-26 07:27:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/src/cublas_matmul_test.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      990 2023-06-18 12:13:08.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/src/cublas_wrapper.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1606 2020-12-03 05:10:19.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cublas/src/helper_cublas.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4906 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/inc/cudnn_rnn_descriptor.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      842 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/inc/cudnn_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11561 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1143 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11327 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1151 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11535 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1029 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12570 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1116 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12027 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1121 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12423 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1061 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8286 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1470 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9384 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1375 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1093 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      628 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/src/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    39400 2021-12-30 07:13:56.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/src/cudnn_conv_test.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2914 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/src/cudnn_rnn_descriptor.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1070 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/src/cudnn_wrapper.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      161 2021-07-26 07:24:52.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/src/helper_cudnn.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/inc/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6280 2022-03-30 06:36:09.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/inc/cufft_utils.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      717 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/inc/cufft_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3201 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      821 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1002 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cufft/src/cufft_wrapper.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/cuda/curand/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/curand/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      632 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/curand/inc/curand_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/curand/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1632 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/curand/ops/curand_random_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      759 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/curand/ops/curand_random_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/curand/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1078 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/curand/src/curand_wrapper.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1933 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/curand/src/helper_curand.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/cuda/cutt/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.676691 jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1052 2022-05-26 06:57:29.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_test_op.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      629 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_test_op.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3868 2023-05-16 06:12:13.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      775 2021-04-15 10:38:17.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      888 2021-11-01 03:42:19.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      559 2021-07-26 07:18:24.000000 jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/cuda/inc/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      588 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/extern/cuda/inc/fp16_dev.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     5639 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/extern/cuda/inc/fp16_emu.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    12641 2022-10-25 03:25:21.000000 jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_cuda.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1173 2023-04-08 05:52:12.000000 jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_functions.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    27554 2023-04-08 05:52:07.000000 jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_image.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    33798 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_string.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    14855 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_timer.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      656 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/inc/nccl_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2033 2023-06-21 07:07:38.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_all_gather_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      782 2023-06-21 06:59:59.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_all_gather_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1866 2023-06-21 06:59:07.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      782 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1886 2023-06-21 06:59:10.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      808 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1972 2023-06-21 06:59:31.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      799 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3785 2022-05-26 06:57:29.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      644 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1923 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/cuda/nccl/src/nccl_wrapper.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/cuda/src/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1323 2021-07-26 07:15:57.000000 jittor-1.3.8.5/python/jittor/extern/cuda/src/fp16_dev.cu
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     5303 2022-07-04 16:11:21.000000 jittor-1.3.8.5/python/jittor/extern/cuda/src/fp16_emu.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    11787 2021-07-26 07:13:54.000000 jittor-1.3.8.5/python/jittor/extern/cuda/src/helper_cuda.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/llvm/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15734 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/extern/llvm/jt_alignment_from_assumptions.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/mkl/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/mkl/ops/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    36034 2022-03-22 14:48:20.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/cpu_cnn_inference_f32.cpp
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8788 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1043 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8850 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1048 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7552 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1035 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2210 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_matmul_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      762 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_matmul_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      810 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      595 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.644191 jittor-1.3.8.5/python/jittor/extern/mpi/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/mpi/inc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2014 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/inc/mpi_wrapper.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/mpi/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2899 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_all_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1110 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_all_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2222 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_broadcast_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1028 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_broadcast_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2989 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1171 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_reduce_op.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1102 2022-05-26 06:57:29.000000 jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_test_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      641 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_test_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.687524 jittor-1.3.8.5/python/jittor/extern/mpi/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3452 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/extern/mpi/src/mpi_wrapper.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.698357 jittor-1.3.8.5/python/jittor/extern/rocm/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   115033 2022-08-09 11:21:18.000000 jittor-1.3.8.5/python/jittor/extern/rocm/rocm_cache.tar.gz
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6235 2022-10-26 06:26:28.000000 jittor-1.3.8.5/python/jittor/extern/rocm/rocm_compiler.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1712 2022-08-09 11:21:18.000000 jittor-1.3.8.5/python/jittor/extern/rocm/rocm_config.cc
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      497 2022-08-09 11:21:18.000000 jittor-1.3.8.5/python/jittor/extern/rocm/rocm_config.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      538 2022-07-04 16:11:21.000000 jittor-1.3.8.5/python/jittor/extern/rocm/rocm_jittor.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6598 2022-08-09 11:21:18.000000 jittor-1.3.8.5/python/jittor/extern/rocm/rocm_wrapper.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    23687 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/init.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1715 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/init_cupy.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    16949 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/linalg.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.698357 jittor-1.3.8.5/python/jittor/loss3d/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      105 2021-06-30 08:15:49.000000 jittor-1.3.8.5/python/jittor/loss3d/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     5553 2021-06-30 08:15:49.000000 jittor-1.3.8.5/python/jittor/loss3d/chamfer.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    16008 2021-06-30 08:15:49.000000 jittor-1.3.8.5/python/jittor/loss3d/emd.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7936 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/lr_scheduler.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.698357 jittor-1.3.8.5/python/jittor/math_util/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       64 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/math_util/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15722 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/math_util/gamma.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      671 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/math_util/igamma.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.698357 jittor-1.3.8.5/python/jittor/math_util/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5520 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/math_util/src/gamma_grad.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    29181 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/math_util/src/igamma.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    76767 2023-06-06 14:33:24.000000 jittor-1.3.8.5/python/jittor/misc.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.698357 jittor-1.3.8.5/python/jittor/models/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      513 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/models/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2246 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/alexnet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6745 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/densenet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6328 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/googlenet.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    11821 2022-04-04 06:54:03.000000 jittor-1.3.8.5/python/jittor/models/inception.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4821 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/mnasnet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4602 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/mobilenet.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8032 2021-10-19 11:51:01.000000 jittor-1.3.8.5/python/jittor/models/res2net.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9657 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/resnet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5575 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/shufflenetv2.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4028 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/squeezenet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3711 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/models/vgg.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)   122453 2023-06-09 17:01:30.000000 jittor-1.3.8.5/python/jittor/nn.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.709191 jittor-1.3.8.5/python/jittor/notebook/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.709191 jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      297 2021-07-14 13:51:52.000000 jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/README.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   243006 2021-07-14 13:51:52.000000 jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/mnist.png
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     5047 2021-07-14 13:51:52.000000 jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 0 --- 介绍与安装.ipynb
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    29117 2021-07-14 13:51:52.000000 jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 1 --- 基本概念.ipynb
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    62291 2022-03-15 13:17:00.000000 jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 2 --- 如何训练一个简单线性回归.ipynb
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   136962 2022-03-15 13:17:00.000000 jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 3 --- 尝试解决一个实际问题.ipynb
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6314 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/ConditionGAN.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3487 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/ConditionGAN.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6752 2022-04-04 06:54:03.000000 jittor-1.3.8.5/python/jittor/notebook/ConditionGAN.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    10677 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/LSGAN.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     7897 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/LSGAN.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    10677 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/notebook/LSGAN.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      238 2022-03-15 13:17:00.000000 jittor-1.3.8.5/python/jittor/notebook/__main__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1243 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/basics.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1250 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/basics.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2111 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/notebook/basics.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2232 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/custom_op.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2249 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/custom_op.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2760 2021-07-16 06:09:15.000000 jittor-1.3.8.5/python/jittor/notebook/custom_op.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1996 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/example.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2152 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/example.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3099 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/notebook/example.src.md
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.709191 jittor-1.3.8.5/python/jittor/notebook/figs/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    41082 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/notebook/figs/mop.svg
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2203 2022-03-22 14:48:20.000000 jittor-1.3.8.5/python/jittor/notebook/md_to_ipynb.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     7817 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/meta_op.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8068 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/meta_op.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    10843 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/notebook/meta_op.src.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      235 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/profiler.cn.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      264 2021-10-11 05:54:17.000000 jittor-1.3.8.5/python/jittor/notebook/profiler.md
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      459 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/notebook/profiler.src.md
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    23255 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/optim.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.709191 jittor-1.3.8.5/python/jittor/other/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     4777 2023-06-21 04:30:04.000000 jittor-1.3.8.5/python/jittor/other/code_softmax.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    29598 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/pool.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    35074 2023-05-13 04:29:28.000000 jittor-1.3.8.5/python/jittor/pyjt_compiler.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.720024 jittor-1.3.8.5/python/jittor/script/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1464 2021-05-12 08:13:24.000000 jittor-1.3.8.5/python/jittor/script/Dockerfile_cuda11
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      890 2021-06-19 09:21:11.000000 jittor-1.3.8.5/python/jittor/script/build_aarch64_mkl.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      893 2021-05-04 00:57:17.000000 jittor-1.3.8.5/python/jittor/script/converter_server.sh
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4134 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/script/inference_perf.py
+-rwxrwxr-x   0 cjld      (1000) cjld      (1000)     2265 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/script/install.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2543 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/script/install_llvm.sh
+-rwxrwxr-x   0 cjld      (1000) cjld      (1000)      632 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/script/install_mkl.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1569 2022-03-15 13:17:00.000000 jittor-1.3.8.5/python/jittor/script/make_doc.py
+-rwxrwxr-x   0 cjld      (1000) cjld      (1000)     4359 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/script/tmpi
+-rwxrwxr-x   0 cjld      (1000) cjld      (1000)      144 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/script/update.sh
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1759 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/sparse.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.720024 jittor-1.3.8.5/python/jittor/src/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1326 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/common.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1056 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/core.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1573 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/event_queue.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2392 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/event_queue.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    26917 2023-06-23 10:06:02.000000 jittor-1.3.8.5/python/jittor/src/executor.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1043 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/executor.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8249 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/fused_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1936 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/fused_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      643 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/fuser.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10134 2023-05-22 01:02:36.000000 jittor-1.3.8.5/python/jittor/src/grad.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      712 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/grad.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5885 2023-05-16 07:23:39.000000 jittor-1.3.8.5/python/jittor/src/graph.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4724 2023-05-16 07:23:32.000000 jittor-1.3.8.5/python/jittor/src/graph.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2730 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/init.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1091 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/init.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9383 2023-06-04 21:24:53.000000 jittor-1.3.8.5/python/jittor/src/jit_compiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      652 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/jit_compiler.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3262 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/jit_key.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7600 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/jit_key.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2031 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/lock.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      864 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/lock.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.730857 jittor-1.3.8.5/python/jittor/src/mem/
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.730857 jittor-1.3.8.5/python/jittor/src/mem/allocator/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1188 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/aligned_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      779 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/aligned_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1407 2023-06-21 06:37:27.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_device_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      805 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_device_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1107 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_dual_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4172 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_dual_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1087 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_host_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      802 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_host_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1190 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_managed_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      856 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_managed_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1501 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/foreign_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      948 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/foreign_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1127 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/nfef_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1000 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/nfef_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9259 2023-06-21 06:33:15.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/sfrl_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3883 2023-06-04 16:31:06.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/sfrl_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1781 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/stat_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1071 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/stat_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3765 2023-06-21 06:30:33.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/temp_allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2234 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator/temp_allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5428 2023-06-18 12:30:56.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2237 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/allocator.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11462 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/mem_info.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1019 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/mem_info.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8807 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/swap.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2427 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/mem/swap.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6373 2023-05-22 03:19:52.000000 jittor-1.3.8.5/python/jittor/src/memory_profiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1429 2023-05-22 03:29:05.000000 jittor-1.3.8.5/python/jittor/src/memory_profiler.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.741691 jittor-1.3.8.5/python/jittor/src/misc/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      485 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/cpu_atomic.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1820 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/cpu_atomic.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2362 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/cpu_math.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      490 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/cpu_math.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1570 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/cstr.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7264 2023-05-13 08:27:34.000000 jittor-1.3.8.5/python/jittor/src/misc/cuda_atomic.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2954 2023-06-18 09:27:45.000000 jittor-1.3.8.5/python/jittor/src/misc/cuda_flags.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1061 2023-06-18 09:24:17.000000 jittor-1.3.8.5/python/jittor/src/misc/cuda_flags.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2191 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/cuda_limits.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      662 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/deleter.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2538 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/fast_shared_ptr.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1000 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/hash.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      864 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/intrin.h
+-rwxr-xr-x   0 cjld      (1000) cjld      (1000)   326707 2023-03-30 05:25:05.000000 jittor-1.3.8.5/python/jittor/src/misc/miniz.cc
+-rwxr-xr-x   0 cjld      (1000) cjld      (1000)    70346 2023-06-23 10:26:15.000000 jittor-1.3.8.5/python/jittor/src/misc/miniz.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2518 2023-06-29 05:48:45.000000 jittor-1.3.8.5/python/jittor/src/misc/nan_checker.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3046 2023-05-13 12:40:54.000000 jittor-1.3.8.5/python/jittor/src/misc/nan_checker.cu
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      403 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/nan_checker.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5953 2023-05-16 04:56:35.000000 jittor-1.3.8.5/python/jittor/src/misc/nano_string.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7634 2023-05-13 20:28:36.000000 jittor-1.3.8.5/python/jittor/src/misc/nano_string.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9048 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/nano_vector.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3368 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/ring_buffer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6868 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/ring_buffer.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1801 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/stack_vector.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1503 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/misc/string_view_map.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7512 2023-05-16 14:49:25.000000 jittor-1.3.8.5/python/jittor/src/node.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1902 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/numpy_func.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9475 2023-05-19 23:16:17.000000 jittor-1.3.8.5/python/jittor/src/op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2828 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    43093 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/op_compiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1766 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/op_compiler.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.752524 jittor-1.3.8.5/python/jittor/src/ops/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7467 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/arg_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1761 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/arg_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6273 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/argsort_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2167 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/argsort_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4035 2023-06-04 21:24:23.000000 jittor-1.3.8.5/python/jittor/src/ops/array_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1098 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/array_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15124 2023-05-16 05:07:55.000000 jittor-1.3.8.5/python/jittor/src/ops/binary_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      727 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/binary_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6900 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/broadcast_to_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2794 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/broadcast_to_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3650 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/candidate_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1945 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/candidate_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1211 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/clone_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      715 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/clone_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8685 2023-05-13 17:11:35.000000 jittor-1.3.8.5/python/jittor/src/ops/code_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10232 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/code_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1425 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/copy_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      694 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/copy_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      685 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/empty_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      607 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/empty_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5104 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/fetch_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2540 2023-06-04 20:08:00.000000 jittor-1.3.8.5/python/jittor/src/ops/fetch_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3766 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/fuse_transpose_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      774 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/fuse_transpose_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    19861 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/getitem_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1555 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/getitem_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2724 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/index_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1986 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/index_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5542 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/numpy_code_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3394 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/numpy_code_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1508 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/op_register.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1544 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/op_register.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1577 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/op_utils.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2072 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/random_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      686 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/random_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12858 2023-05-16 14:58:04.000000 jittor-1.3.8.5/python/jittor/src/ops/reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1019 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5836 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/reindex_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4093 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/reindex_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5603 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/reindex_reduce_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3610 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/reindex_reduce_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2069 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/reshape_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1536 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/reshape_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1615 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/safe_clip_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1008 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/safe_clip_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12583 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/setitem_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1130 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/setitem_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3004 2023-05-13 19:25:10.000000 jittor-1.3.8.5/python/jittor/src/ops/tape_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1897 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/tape_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3745 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/ternary_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      735 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/ternary_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3808 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/transpose_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      761 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/transpose_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    26784 2023-05-13 12:41:11.000000 jittor-1.3.8.5/python/jittor/src/ops/unary_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      742 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/unary_op.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8196 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/where_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1232 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/ops/where_op.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.752524 jittor-1.3.8.5/python/jittor/src/opt/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    38841 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/expr.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5751 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/expr.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.752524 jittor-1.3.8.5/python/jittor/src/opt/gopt/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5549 2023-06-19 04:36:41.000000 jittor-1.3.8.5/python/jittor/src/opt/gopt/setitem_gopt.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3084 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/jit_searcher.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      748 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/jit_searcher.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    35269 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/kernel_ir.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8192 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/kernel_ir.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.763357 jittor-1.3.8.5/python/jittor/src/opt/pass/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2071 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/assume_aligned_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      572 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/assume_aligned_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      613 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/atomic_tuner_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6886 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/check_cache_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      613 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/check_cache_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1494 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/compile_shapes_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      572 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/compile_shapes_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1644 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/const_var_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      562 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/const_var_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1391 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/expand_empty_block_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      582 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/expand_empty_block_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6960 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/fake_main_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      557 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/fake_main_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3545 2023-05-11 12:13:21.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/float_atomic_fix_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      590 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/float_atomic_fix_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1480 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/insert_profile_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      585 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/insert_profile_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4427 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/loop_to_func_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      564 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/loop_to_func_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12889 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/loop_var_analyze_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      662 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/loop_var_analyze_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1246 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/mark_raw_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      554 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/mark_raw_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2283 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/merge_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      560 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/merge_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6195 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/merge_loop_var_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      570 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/merge_loop_var_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      556 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/parallel_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      680 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      732 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1490 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/remove_intermediate_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      587 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/remove_intermediate_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      897 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/remove_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      620 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/remove_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      633 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/rename_loop_index_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      579 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/rename_loop_index_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2306 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/reorder_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      610 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/reorder_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3452 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/replace_for_num_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      868 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/replace_for_num_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5910 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/restride_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      556 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/restride_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      574 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/shared_reduce_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      604 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/solve_conflict_define_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      591 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/solve_conflict_define_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1362 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/split_loop_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      634 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/split_loop_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3719 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/unroll_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      562 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/unroll_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      944 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/use_movnt_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      610 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/use_movnt_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3411 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/vectorize_pass.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      559 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass/vectorize_pass.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4356 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass_manager.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1954 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/pass_manager.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.763357 jittor-1.3.8.5/python/jittor/src/opt/tuner/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2242 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/broadcast_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      670 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/broadcast_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    16851 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/conv_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      692 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/conv_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4058 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/matmul_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      622 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/matmul_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2601 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/reduce_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      689 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/reduce_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1139 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/reorder_tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      593 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/reorder_tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      655 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/tuner.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      709 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner/tuner.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2310 2023-06-04 21:11:55.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner_manager.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      797 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/tuner_manager.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7246 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/var_relay.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1733 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/opt/var_relay.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12891 2023-06-24 14:29:55.000000 jittor-1.3.8.5/python/jittor/src/parallel_compiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      610 2023-06-24 14:28:20.000000 jittor-1.3.8.5/python/jittor/src/parallel_compiler.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.763357 jittor-1.3.8.5/python/jittor/src/profiler/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      913 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/cache_info.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      717 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/cache_info.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1882 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/memory_checker.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1080 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/memory_checker.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    21999 2023-05-16 04:35:30.000000 jittor-1.3.8.5/python/jittor/src/profiler/profiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2317 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/profiler.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1914 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/profiler_guard.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2224 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/replacement.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1311 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/replacement.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3423 2023-06-17 04:52:49.000000 jittor-1.3.8.5/python/jittor/src/profiler/simple_profiler.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2609 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/profiler/vtop.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.763357 jittor-1.3.8.5/python/jittor/src/pybind/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1313 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pybind/core.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    16013 2023-05-16 04:35:32.000000 jittor-1.3.8.5/python/jittor/src/pybind/py_var_tracer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1950 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pybind/py_var_tracer.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      558 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pybind/py_var_tracer_interface.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.774191 jittor-1.3.8.5/python/jittor/src/pyjt/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2688 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/numpy.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4020 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/numpy.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2093 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_arg_printer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1044 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_arg_printer.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6571 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_array_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1116 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_caller.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      551 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_caller.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    27629 2023-06-25 14:57:53.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_converter.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2248 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_obj_holder.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8751 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_ring_buffer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1709 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/py_ring_buffer.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15153 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/pyjt/pyjt_console.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.774191 jittor-1.3.8.5/python/jittor/src/test/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8024 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_expr.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      832 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_fast_shared_ptr.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2266 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_jit_key.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11949 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_kernel_ir.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2208 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_nano_vector.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      820 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_op_compiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3937 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_op_relay.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2040 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_setitem_op.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4738 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/test/test_sfrl_allocator.cc
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.774191 jittor-1.3.8.5/python/jittor/src/type/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6593 2023-05-13 22:53:57.000000 jittor-1.3.8.5/python/jittor/src/type/common_op_type.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6291 2023-06-30 12:33:45.000000 jittor-1.3.8.5/python/jittor/src/type/fp16_compute.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7484 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/type/fp16_op_type.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6873 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/types.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.774191 jittor-1.3.8.5/python/jittor/src/utils/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15087 2023-05-13 08:17:57.000000 jittor-1.3.8.5/python/jittor/src/utils/cache_compile.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      746 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/cache_compile.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1706 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/cross_platform.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1286 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/flags.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      408 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/flags.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    20979 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/jit_utils.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    21467 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/log.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9277 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/log.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1490 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/mwsr_list.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4766 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/mwsr_list.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     6721 2021-10-01 11:48:38.000000 jittor-1.3.8.5/python/jittor/src/utils/seh.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7262 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/str_utils.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1522 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/str_utils.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7975 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/tracer.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      485 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/utils/tracer.h
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)       15 2021-10-01 11:48:38.000000 jittor-1.3.8.5/python/jittor/src/utils/vdp
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5563 2023-06-04 18:38:09.000000 jittor-1.3.8.5/python/jittor/src/var.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3286 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/var.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10521 2023-06-23 17:25:11.000000 jittor-1.3.8.5/python/jittor/src/var_holder.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10797 2023-06-23 15:08:13.000000 jittor-1.3.8.5/python/jittor/src/var_holder.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1202 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/var_slices.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2993 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/src/var_slices.h
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.795858 jittor-1.3.8.5/python/jittor/test/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2927 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/__main__.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.795858 jittor-1.3.8.5/python/jittor/test/misc/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15224 2022-03-14 07:47:44.000000 jittor-1.3.8.5/python/jittor/test/misc/superglue.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.795858 jittor-1.3.8.5/python/jittor/test/perf/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     8216 2022-03-22 14:48:20.000000 jittor-1.3.8.5/python/jittor/test/perf/perf.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.795858 jittor-1.3.8.5/python/jittor/test/system/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      358 2020-12-07 05:07:32.000000 jittor-1.3.8.5/python/jittor/test/system/test_all.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:52.000000 jittor-1.3.8.5/python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:48.000000 jittor-1.3.8.5/python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:44.000000 jittor-1.3.8.5/python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1652 2020-12-09 09:06:39.000000 jittor-1.3.8.5/python/jittor/test/system/test_cuda11.1_ubuntu18.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1844 2020-12-09 09:06:33.000000 jittor-1.3.8.5/python/jittor/test/system/test_cuda11.1_ubuntu20.04.sh
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1535 2020-12-09 09:06:26.000000 jittor-1.3.8.5/python/jittor/test/system/test_nocuda_ubuntu18.04.sh
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      661 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5310 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_acl.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3269 2022-09-01 03:11:16.000000 jittor-1.3.8.5/python/jittor/test/test_adamw.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3007 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_affine_grid.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1453 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_allocator.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1573 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_allocator2.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    12385 2021-08-04 11:28:54.000000 jittor-1.3.8.5/python/jittor/test/test_arg_pool_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5539 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_arg_reduce_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4327 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_argsort_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6742 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_array.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4192 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_asm_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2882 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_atomic_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2258 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_attention.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2134 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_auto_diff.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5576 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_batchnorm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12199 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_benchmark.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2177 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_bicubic.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7256 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_binary_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1591 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_bmm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4661 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_broadcast_to_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1819 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_broadcast_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4566 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_cache.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2662 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_candidate.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1143 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_clone.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    14087 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_code_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1137 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_compile_options.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6570 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_concat_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      963 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_console.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2464 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_contrib.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4874 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_conv_transpose.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6831 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_conv_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11127 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_core.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3460 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_cub_cumsum.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1538 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_cublas_test_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3801 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_cuda.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9134 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_cudnn_op.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1570 2022-04-23 08:12:38.000000 jittor-1.3.8.5/python/jittor/test/test_cumprod_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2986 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_custom_op.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      869 2020-09-16 07:12:03.000000 jittor-1.3.8.5/python/jittor/test/test_cutt.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     4068 2022-09-15 16:59:59.000000 jittor-1.3.8.5/python/jittor/test/test_cutt_transpose_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10487 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_dataset.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1455 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_default_var.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4289 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_densenet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3130 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_depthwise_conv.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1571 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_digamma.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7920 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_distributions.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    28179 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_einops.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4462 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_einsum.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1138 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_emnist.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2195 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_error_msg.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2732 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_example.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3130 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_example_accumulate_grad.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1156 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_fetcher.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9165 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_fft_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1006 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_flags.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1958 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_fold.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12961 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_fp16.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9481 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_function.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    13063 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_fused_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1447 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_fuser.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1730 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_gamma_distribution.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6053 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_grad.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5585 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_group_conv_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1556 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_histc.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2239 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_hook.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2686 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_image_folder.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5361 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_inception.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2312 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_index_op.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3247 2021-10-22 06:53:31.000000 jittor-1.3.8.5/python/jittor/test/test_init.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1216 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_interpolation.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1002 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_jit_tests.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1867 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_jtune.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1889 2022-05-06 04:57:57.000000 jittor-1.3.8.5/python/jittor/test/test_knn.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1364 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_lazy_execution.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11030 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_linalg.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2211 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_load_pth.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1089 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_lock.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1813 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_log.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2073 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_longest_dis_fuse.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9002 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_loss.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3392 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_loss3d.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1702 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_lr_scheduler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3814 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_lstm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    13954 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_matmul.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1648 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_matmul_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1263 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_mem.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3818 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_memory_profiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2302 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_merge_loop_var_pass.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4523 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_merge_single_array_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6544 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_misc_issue.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    16899 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_misc_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8278 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_mkl_conv_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      648 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_mkl_test_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4056 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_models.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3220 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_mpi.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4369 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_mpi_batchnorm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1879 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_mpi_in_py.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2374 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_mpi_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2615 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_nano_string.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1581 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_nano_vector.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      703 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_nccl.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5181 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_nccl_ops.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1495 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_new_fused_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5550 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_node.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1630 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_notebooks.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6193 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_numpy_code_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6353 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_op_compiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1520 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_opt_state_dict.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1570 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_optimizer.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1883 2023-03-22 11:47:26.000000 jittor-1.3.8.5/python/jittor/test/test_optimizer_save_load.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3904 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_pad.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     7853 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_parallel_pass.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1196 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_param_list.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1462 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_profiler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8588 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_pytorch_converter.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3728 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_random_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4642 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_reduce_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1760 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_reduce_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11179 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_reindex_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3620 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_reindex_reduce_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3801 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_relu.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3383 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_reorder_tuner.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1670 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_repeat.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3237 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_reshape.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5310 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_resize_and_crop.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6181 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_resnet.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2217 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_ring_buffer.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3721 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_ring_buffer2.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    26660 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_rnn.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15920 2022-08-09 11:21:18.000000 jittor-1.3.8.5/python/jittor/test/test_rocm.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1721 2021-03-23 11:08:33.000000 jittor-1.3.8.5/python/jittor/test/test_sampler.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2368 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_search_sorted.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1549 2021-06-22 07:08:32.000000 jittor-1.3.8.5/python/jittor/test/test_searchsorted_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    15402 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_setitem.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1481 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_single_process_scope.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6304 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_slice.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1371 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_sparse.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1732 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_stop_fuse.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3872 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_superglue.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2088 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_ternary_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6552 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_trace_var.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1439 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_tracer.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    40470 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_transform.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5469 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_transpose_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4342 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_unary_op.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1869 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_unique.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2230 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_utils.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2074 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_var.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     3731 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_vgg.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2202 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_weightnorm.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2790 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/test/test_where_op.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.795858 jittor-1.3.8.5/python/jittor/transform/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    54004 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/transform/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    23971 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/transform/function_pil.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.795858 jittor-1.3.8.5/python/jittor/utils/
+-rwxr-xr-x   0 cjld      (1000) cjld      (1000)     5419 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/asm_tuner.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      352 2022-12-01 04:53:11.000000 jittor-1.3.8.5/python/jittor/utils/bench_klo.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      685 2020-12-13 14:03:17.000000 jittor-1.3.8.5/python/jittor/utils/converter_server.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)   437003 2023-04-03 01:38:42.000000 jittor-1.3.8.5/python/jittor/utils/data.gz
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      662 2022-06-23 13:14:46.000000 jittor-1.3.8.5/python/jittor/utils/dlink_compiler.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1276 2022-03-15 13:17:00.000000 jittor-1.3.8.5/python/jittor/utils/dumpdef.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     9761 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/gen_pyi.py
+-rwxr-xr-x   0 cjld      (1000) cjld      (1000)     1926 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/jtune.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2190 2021-10-01 11:48:38.000000 jittor-1.3.8.5/python/jittor/utils/local_doc_builder.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1214 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/nvtx.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     4895 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/polish.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2484 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/polish_centos.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1834 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/publish.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    28291 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/pytorch_converter.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)      837 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor/utils/tracer.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.795858 jittor-1.3.8.5/python/jittor/vcompiler/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       24 2023-06-25 14:33:06.000000 jittor-1.3.8.5/python/jittor/vcompiler/__init__.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    35521 2023-06-25 14:33:37.000000 jittor-1.3.8.5/python/jittor/vcompiler/vcompiler.cc
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2371 2023-06-25 14:33:46.000000 jittor-1.3.8.5/python/jittor/vcompiler/vcompiler.h
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5028 2023-06-25 14:33:27.000000 jittor-1.3.8.5/python/jittor/vcompiler/vcompiler.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)       41 2021-06-18 14:24:21.000000 jittor-1.3.8.5/python/jittor/version
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2878 2023-04-04 18:16:13.000000 jittor-1.3.8.5/python/jittor/weightnorm.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.665857 jittor-1.3.8.5/python/jittor.egg-info/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    11712 2023-06-30 15:33:00.000000 jittor-1.3.8.5/python/jittor.egg-info/PKG-INFO
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    28436 2023-06-30 15:33:00.000000 jittor-1.3.8.5/python/jittor.egg-info/SOURCES.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)        1 2023-06-30 15:33:00.000000 jittor-1.3.8.5/python/jittor.egg-info/dependency_links.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       75 2023-06-30 15:33:00.000000 jittor-1.3.8.5/python/jittor.egg-info/requires.txt
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       20 2023-06-30 15:33:00.000000 jittor-1.3.8.5/python/jittor.egg-info/top_level.txt
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.806691 jittor-1.3.8.5/python/jittor_utils/
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    25368 2023-06-18 09:11:20.000000 jittor-1.3.8.5/python/jittor_utils/__init__.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)    15503 2022-03-22 14:48:20.000000 jittor-1.3.8.5/python/jittor_utils/auto_diff.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     1290 2022-05-08 11:48:51.000000 jittor-1.3.8.5/python/jittor_utils/auto_git_tag.py
+drwxr-xr-x   0 cjld      (1000) cjld      (1000)        0 2023-06-30 15:33:00.806691 jittor-1.3.8.5/python/jittor_utils/class/
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      993 2021-10-12 06:29:13.000000 jittor-1.3.8.5/python/jittor_utils/class/motd
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      472 2021-10-12 06:29:13.000000 jittor-1.3.8.5/python/jittor_utils/class/setup.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5595 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor_utils/class/setup_env.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     1634 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor_utils/clean_cache.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3812 2021-10-01 11:48:38.000000 jittor-1.3.8.5/python/jittor_utils/config.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      710 2022-05-08 11:48:51.000000 jittor-1.3.8.5/python/jittor_utils/github_release.sh
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     6105 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor_utils/install_cuda.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      504 2021-10-01 11:48:38.000000 jittor-1.3.8.5/python/jittor_utils/install_msvc.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    12389 2023-06-23 09:31:05.000000 jittor-1.3.8.5/python/jittor_utils/load_pytorch.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)    10438 2023-03-30 09:43:29.000000 jittor-1.3.8.5/python/jittor_utils/load_pytorch_old.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2608 2022-04-22 13:37:44.000000 jittor-1.3.8.5/python/jittor_utils/lock.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     5441 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor_utils/misc.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     3093 2022-07-06 05:24:42.000000 jittor-1.3.8.5/python/jittor_utils/pack_offline.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      799 2021-10-12 06:29:13.000000 jittor-1.3.8.5/python/jittor_utils/pip_publish.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)      852 2021-10-13 11:17:19.000000 jittor-1.3.8.5/python/jittor_utils/query_cuda_cc.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     8822 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor_utils/ring_buffer.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)     2168 2023-05-01 08:04:48.000000 jittor-1.3.8.5/python/jittor_utils/student_queue.py
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2844 2022-09-15 16:59:59.000000 jittor-1.3.8.5/python/jittor_utils/translator.py
+-rw-r--r--   0 cjld      (1000) cjld      (1000)       38 2023-06-30 15:33:00.806691 jittor-1.3.8.5/setup.cfg
+-rw-rw-r--   0 cjld      (1000) cjld      (1000)     2464 2021-10-12 06:29:13.000000 jittor-1.3.8.5/setup.py
```

### Comparing `jittor-1.3.8.4/LICENSE.txt` & `jittor-1.3.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/PKG-INFO` & `jittor-1.3.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jittor
-Version: 1.3.8.4
+Version: 1.3.8.5
 Summary: a Just-in-time(JIT) deep learning framework
 Home-page: http://jittor.org
 Author: Jittor Group
 Author-email: ran.donglang@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `jittor-1.3.8.4/README.md` & `jittor-1.3.8.5/README.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/__init__.py` & `jittor-1.3.8.5/python/jittor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #   Meng-Hao Guo <guomenghao1997@gmail.com>
 #
 # 
 # This file is subject to the terms and conditions defined in
 # file 'LICENSE.txt', which is part of this source code package.
 # ***************************************************************
 
-__version__ = '1.3.8.4'
+__version__ = '1.3.8.5'
 from jittor_utils import lock
 with lock.lock_scope():
     ori_int = int
     ori_float = float
     ori_bool = bool
     from . import compiler
     from .compiler import LOG, has_cuda
```

### Comparing `jittor-1.3.8.4/python/jittor/__init__.pyi` & `jittor-1.3.8.5/python/jittor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/attention.py` & `jittor-1.3.8.5/python/jittor/attention.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/ccl/ccl_2d.py` & `jittor-1.3.8.5/python/jittor/ccl/ccl_2d.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/ccl/ccl_3d.py` & `jittor-1.3.8.5/python/jittor/ccl/ccl_3d.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/ccl/ccl_link.py` & `jittor-1.3.8.5/python/jittor/ccl/ccl_link.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/compile_extern.py` & `jittor-1.3.8.5/python/jittor/compile_extern.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/compiler.py` & `jittor-1.3.8.5/python/jittor/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,16 @@
             src = f.read().decode("utf8")
         defs = re_def.findall(src)
         for _, args in defs:
             args = args.split(",")
             type = args[0].strip()
             name = args[1].strip()
             if not has_cuda and "cuda" in name and name!="use_cuda":
-                continue
+                if name != "use_cuda_host_allocator":
+                    continue
             default = args[2].strip()
             doc = ",".join(args[3:])
             doc = eval(f"({doc})")
             LOG.vv(f"Find define {name} from {src_name}")
             if name in visit:
                 continue
             visit[name] = 1
```

### Comparing `jittor-1.3.8.4/python/jittor/contrib.py` & `jittor-1.3.8.5/python/jittor/contrib.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/dataset/cifar.py` & `jittor-1.3.8.5/python/jittor/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/dataset/dataset.py` & `jittor-1.3.8.5/python/jittor/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/dataset/mnist.py` & `jittor-1.3.8.5/python/jittor/dataset/mnist.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/dataset/sampler.py` & `jittor-1.3.8.5/python/jittor/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/dataset/utils.py` & `jittor-1.3.8.5/python/jittor/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/dataset/voc.py` & `jittor-1.3.8.5/python/jittor/dataset/voc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/demo/simple_cgan.py` & `jittor-1.3.8.5/python/jittor/demo/simple_cgan.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/depthwise_conv.py` & `jittor-1.3.8.5/python/jittor/depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/distributions.py` & `jittor-1.3.8.5/python/jittor/distributions.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/einops/_backends.py` & `jittor-1.3.8.5/python/jittor/einops/_backends.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/einops/einops.py` & `jittor-1.3.8.5/python/jittor/einops/einops.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/einops/experimental/indexing.py` & `jittor-1.3.8.5/python/jittor/einops/experimental/indexing.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/einops/layers/__init__.py` & `jittor-1.3.8.5/python/jittor/einops/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/einops/layers/_einmix.py` & `jittor-1.3.8.5/python/jittor/einops/layers/_einmix.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/einops/layers/jittor.py` & `jittor-1.3.8.5/python/jittor/einops/layers/jittor.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/einops/parsing.py` & `jittor-1.3.8.5/python/jittor/einops/parsing.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/acl/acl_error_code.cc` & `jittor-1.3.8.5/python/jittor/extern/acl/acl_error_code.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/acl/acl_jittor.cc` & `jittor-1.3.8.5/python/jittor/extern/acl/acl_jittor.cc`

 * *Files 5% similar despite different names*

```diff
@@ -70,14 +70,17 @@
     CHECK_ACL(aclrtDestroyContext(acl_jittor_context));
     CHECK_ACL(aclFinalize());
 }
 
 } _acl_jittor_initer;
 
 string process_acl(const string& src, const string& name, const map<string,string>& kargs) {
+    if (endswith(name, "_jittor.cc"))
+        return src;
+    try {
     auto tokens = token_split(src);
     int edit = 0;
     for (int i=0; i<tokens.size(); i++) {
         auto& token = tokens[i];
         if (token == "cuda_runtime") token = "acl_jittor", edit ++; else
         if (token == "CUDA") token = "ACL", edit ++; else
         if (startswith(token, "cuda")) {
@@ -159,35 +162,44 @@
     }
     if (!edit) return src;
     string new_src = join(tokens, "");
     if (name == "executor.cc") {
         new_src = "#include <Python.h>\n#include <pystate.h>\n"+
         replace(new_src, "op->do_run_after_prepare(jkl);", 
         R"({
-            Py_BEGIN_ALLOW_THREADS
-            op->do_run_after_prepare(jkl);
-            Py_END_ALLOW_THREADS
+            if (!PyGILState_Check()) {
+                op->do_run_after_prepare(jkl);
+            } else {
+                Py_BEGIN_ALLOW_THREADS
+                op->do_run_after_prepare(jkl);
+                Py_END_ALLOW_THREADS
+            }
         })");
     }
     if (name == "profiler.cc") {
         new_src = token_replace_all(new_src, ".cc", ".tikcc");
     }
     // LOGir << name << (name == "pass_manager.cc");
     if (name == "pass_manager.cc") {
         LOGir << "replace" << name;
         new_src = token_replace_all(new_src, "run_pass<FloatAtomicFixPass>();", "WTF");
     }
     // ????????
     return new_src;
+    } catch (const std::exception& e) {
+        LOGe << "process acl error:" << e.what();
+        LOGe << "name:" << name;
+        throw;
+    }
 }
 
 void acl_jittor_op_compiler(string& filename, string& src, bool is_acl, string& extra_flags) {
     if (!is_acl) return;
-    extra_flags += " --tik-soc-version=Ascend910 ";
-    filename = replace(filename, ".cc", ".tikcc");
+    // extra_flags += " --tik-soc-version=Ascend910 ";
+    // filename = replace(filename, ".cc", ".tikcc");
     // LOGir << filename;
     string new_src = process_acl(src, "", {});
     new_src = replace(new_src, R"(#include "misc/cuda_atomic.h")", "");
     new_src = replace(new_src, R"(#include "misc/cuda_limits.h")", "");
     new_src = replace(new_src, "__global__", "__ai_device_entry__");
     new_src = token_replace_all(new_src, "__launch_bounds__($1)", "");
     new_src = token_replace_all(new_src, "int thread_num = $1;", "int thread_num = 1;");
```

### Comparing `jittor-1.3.8.4/python/jittor/extern/acl/acl_jittor.h` & `jittor-1.3.8.5/python/jittor/extern/acl/acl_jittor.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/corex/corex_compiler.py` & `jittor-1.3.8.5/python/jittor/extern/corex/corex_compiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/inc/cub_test.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/inc/cub_test.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_arg_reduce_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_argsort_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_argsort_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_argsort_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_argsort_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_cumsum_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_test_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_test_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_test_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_where_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_where_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cub/ops/cub_where_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cub/ops/cub_where_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/inc/cublas_wrapper.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/inc/cublas_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_acc_matmul_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_batched_matmul_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_matmul_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_test_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/ops/cublas_test_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/ops/cublas_test_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/src/cublas_matmul_test.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/src/cublas_matmul_test.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/src/cublas_wrapper.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/src/cublas_wrapper.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cublas/src/helper_cublas.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cublas/src/helper_cublas.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/inc/cudnn_rnn_descriptor.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/inc/cudnn_rnn_descriptor.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/inc/cudnn_wrapper.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/inc/cudnn_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_w_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_backward_x_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv3d_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_w_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_backward_x_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_conv_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_backward_x_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_rnn_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/ops/cudnn_test_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/src/cudnn_conv_test.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/src/cudnn_conv_test.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/src/cudnn_rnn_descriptor.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/src/cudnn_rnn_descriptor.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cudnn/src/cudnn_wrapper.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cudnn/src/cudnn_wrapper.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cufft/inc/cufft_utils.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cufft/inc/cufft_utils.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cufft/inc/cufft_wrapper.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cufft/inc/cufft_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cufft/ops/cufft_fft_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cufft/src/cufft_wrapper.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cufft/src/cufft_wrapper.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/curand/inc/curand_wrapper.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/curand/inc/curand_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/curand/ops/curand_random_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/curand/ops/curand_random_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/curand/ops/curand_random_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/curand/ops/curand_random_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/curand/src/curand_wrapper.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/curand/src/curand_wrapper.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/curand/src/helper_curand.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/curand/src/helper_curand.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_test_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_test_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_test_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_transpose_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/cutt/ops/cutt_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/inc/fp16_dev.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/inc/fp16_dev.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/inc/fp16_emu.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/inc/fp16_emu.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_cuda.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_cuda.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_functions.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_functions.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_image.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_image.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_string.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_string.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/inc/helper_timer.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/inc/helper_timer.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/inc/nccl_wrapper.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/inc/nccl_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_all_gather_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_all_gather_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_all_gather_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_all_gather_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_all_reduce_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_broadcast_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_reduce_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_test_op.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/ops/nccl_test_op.h` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/ops/nccl_test_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/nccl/src/nccl_wrapper.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/nccl/src/nccl_wrapper.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/src/fp16_dev.cu` & `jittor-1.3.8.5/python/jittor/extern/cuda/src/fp16_dev.cu`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/src/fp16_emu.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/src/fp16_emu.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/cuda/src/helper_cuda.cc` & `jittor-1.3.8.5/python/jittor/extern/cuda/src/helper_cuda.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/llvm/jt_alignment_from_assumptions.cc` & `jittor-1.3.8.5/python/jittor/extern/llvm/jt_alignment_from_assumptions.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/cpu_cnn_inference_f32.cpp` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/cpu_cnn_inference_f32.cpp`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.h` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_backward_w_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.h` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_backward_x_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_conv_op.h` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_conv_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_matmul_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_matmul_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_matmul_op.h` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_matmul_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_test_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mkl/ops/mkl_test_op.h` & `jittor-1.3.8.5/python/jittor/extern/mkl/ops/mkl_test_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/inc/mpi_wrapper.h` & `jittor-1.3.8.5/python/jittor/extern/mpi/inc/mpi_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_all_reduce_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_all_reduce_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_all_reduce_op.h` & `jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_all_reduce_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_broadcast_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_broadcast_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_broadcast_op.h` & `jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_broadcast_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_reduce_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_reduce_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_reduce_op.h` & `jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_reduce_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_test_op.cc` & `jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_test_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/ops/mpi_test_op.h` & `jittor-1.3.8.5/python/jittor/extern/mpi/ops/mpi_test_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/mpi/src/mpi_wrapper.cc` & `jittor-1.3.8.5/python/jittor/extern/mpi/src/mpi_wrapper.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/rocm/rocm_cache.tar.gz` & `jittor-1.3.8.5/python/jittor/extern/rocm/rocm_cache.tar.gz`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/rocm/rocm_compiler.py` & `jittor-1.3.8.5/python/jittor/extern/rocm/rocm_compiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/rocm/rocm_config.cc` & `jittor-1.3.8.5/python/jittor/extern/rocm/rocm_config.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/rocm/rocm_jittor.h` & `jittor-1.3.8.5/python/jittor/extern/rocm/rocm_jittor.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/extern/rocm/rocm_wrapper.h` & `jittor-1.3.8.5/python/jittor/extern/rocm/rocm_wrapper.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/init.py` & `jittor-1.3.8.5/python/jittor/init.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/init_cupy.py` & `jittor-1.3.8.5/python/jittor/init_cupy.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/linalg.py` & `jittor-1.3.8.5/python/jittor/linalg.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/loss3d/chamfer.py` & `jittor-1.3.8.5/python/jittor/loss3d/chamfer.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/loss3d/emd.py` & `jittor-1.3.8.5/python/jittor/loss3d/emd.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/lr_scheduler.py` & `jittor-1.3.8.5/python/jittor/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/math_util/gamma.py` & `jittor-1.3.8.5/python/jittor/math_util/gamma.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/math_util/igamma.py` & `jittor-1.3.8.5/python/jittor/math_util/igamma.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/math_util/src/gamma_grad.h` & `jittor-1.3.8.5/python/jittor/math_util/src/gamma_grad.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/math_util/src/igamma.h` & `jittor-1.3.8.5/python/jittor/math_util/src/igamma.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/misc.py` & `jittor-1.3.8.5/python/jittor/misc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/__init__.py` & `jittor-1.3.8.5/python/jittor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/alexnet.py` & `jittor-1.3.8.5/python/jittor/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/densenet.py` & `jittor-1.3.8.5/python/jittor/models/densenet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/googlenet.py` & `jittor-1.3.8.5/python/jittor/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/inception.py` & `jittor-1.3.8.5/python/jittor/models/inception.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/mnasnet.py` & `jittor-1.3.8.5/python/jittor/models/mnasnet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/mobilenet.py` & `jittor-1.3.8.5/python/jittor/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/res2net.py` & `jittor-1.3.8.5/python/jittor/models/res2net.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/resnet.py` & `jittor-1.3.8.5/python/jittor/models/resnet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/shufflenetv2.py` & `jittor-1.3.8.5/python/jittor/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/squeezenet.py` & `jittor-1.3.8.5/python/jittor/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/models/vgg.py` & `jittor-1.3.8.5/python/jittor/models/vgg.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/nn.py` & `jittor-1.3.8.5/python/jittor/nn.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/mnist.png` & `jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/mnist.png`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 0 --- 介绍与安装.ipynb` & `jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 0 --- 介绍与安装.ipynb`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 1 --- 基本概念.ipynb` & `jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 1 --- 基本概念.ipynb`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 2 --- 如何训练一个简单线性回归.ipynb` & `jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 2 --- 如何训练一个简单线性回归.ipynb`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 3 --- 尝试解决一个实际问题.ipynb` & `jittor-1.3.8.5/python/jittor/notebook/60分钟快速入门Jittor/计图入门教程 3 --- 尝试解决一个实际问题.ipynb`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/ConditionGAN.cn.md` & `jittor-1.3.8.5/python/jittor/notebook/ConditionGAN.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/ConditionGAN.md` & `jittor-1.3.8.5/python/jittor/notebook/ConditionGAN.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/ConditionGAN.src.md` & `jittor-1.3.8.5/python/jittor/notebook/ConditionGAN.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/LSGAN.cn.md` & `jittor-1.3.8.5/python/jittor/notebook/LSGAN.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/LSGAN.md` & `jittor-1.3.8.5/python/jittor/notebook/LSGAN.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/LSGAN.src.md` & `jittor-1.3.8.5/python/jittor/notebook/LSGAN.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/basics.cn.md` & `jittor-1.3.8.5/python/jittor/notebook/basics.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/basics.md` & `jittor-1.3.8.5/python/jittor/notebook/basics.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/basics.src.md` & `jittor-1.3.8.5/python/jittor/notebook/basics.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/custom_op.cn.md` & `jittor-1.3.8.5/python/jittor/notebook/custom_op.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/custom_op.md` & `jittor-1.3.8.5/python/jittor/notebook/custom_op.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/custom_op.src.md` & `jittor-1.3.8.5/python/jittor/notebook/custom_op.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/example.cn.md` & `jittor-1.3.8.5/python/jittor/notebook/example.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/example.md` & `jittor-1.3.8.5/python/jittor/notebook/example.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/example.src.md` & `jittor-1.3.8.5/python/jittor/notebook/example.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/figs/mop.svg` & `jittor-1.3.8.5/python/jittor/notebook/figs/mop.svg`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/md_to_ipynb.py` & `jittor-1.3.8.5/python/jittor/notebook/md_to_ipynb.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/meta_op.cn.md` & `jittor-1.3.8.5/python/jittor/notebook/meta_op.cn.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/meta_op.md` & `jittor-1.3.8.5/python/jittor/notebook/meta_op.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/notebook/meta_op.src.md` & `jittor-1.3.8.5/python/jittor/notebook/meta_op.src.md`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/optim.py` & `jittor-1.3.8.5/python/jittor/optim.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/other/code_softmax.py` & `jittor-1.3.8.5/python/jittor/other/code_softmax.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/pool.py` & `jittor-1.3.8.5/python/jittor/pool.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/pyjt_compiler.py` & `jittor-1.3.8.5/python/jittor/pyjt_compiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/Dockerfile_cuda11` & `jittor-1.3.8.5/python/jittor/script/Dockerfile_cuda11`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/build_aarch64_mkl.sh` & `jittor-1.3.8.5/python/jittor/script/build_aarch64_mkl.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/converter_server.sh` & `jittor-1.3.8.5/python/jittor/script/converter_server.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/inference_perf.py` & `jittor-1.3.8.5/python/jittor/script/inference_perf.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/install.sh` & `jittor-1.3.8.5/python/jittor/script/install.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/install_llvm.sh` & `jittor-1.3.8.5/python/jittor/script/install_llvm.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/install_mkl.sh` & `jittor-1.3.8.5/python/jittor/script/install_mkl.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/make_doc.py` & `jittor-1.3.8.5/python/jittor/script/make_doc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/script/tmpi` & `jittor-1.3.8.5/python/jittor/script/tmpi`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/sparse.py` & `jittor-1.3.8.5/python/jittor/sparse.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/common.h` & `jittor-1.3.8.5/python/jittor/src/common.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/core.h` & `jittor-1.3.8.5/python/jittor/src/core.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/event_queue.cc` & `jittor-1.3.8.5/python/jittor/src/event_queue.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/event_queue.h` & `jittor-1.3.8.5/python/jittor/src/event_queue.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/executor.cc` & `jittor-1.3.8.5/python/jittor/src/executor.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/executor.h` & `jittor-1.3.8.5/python/jittor/src/executor.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/fused_op.cc` & `jittor-1.3.8.5/python/jittor/src/fused_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/fused_op.h` & `jittor-1.3.8.5/python/jittor/src/fused_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/fuser.h` & `jittor-1.3.8.5/python/jittor/src/fuser.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/grad.cc` & `jittor-1.3.8.5/python/jittor/src/grad.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/grad.h` & `jittor-1.3.8.5/python/jittor/src/grad.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/graph.cc` & `jittor-1.3.8.5/python/jittor/src/graph.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/graph.h` & `jittor-1.3.8.5/python/jittor/src/graph.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/init.cc` & `jittor-1.3.8.5/python/jittor/src/init.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/init.h` & `jittor-1.3.8.5/python/jittor/src/init.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/jit_compiler.cc` & `jittor-1.3.8.5/python/jittor/src/jit_compiler.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/jit_compiler.h` & `jittor-1.3.8.5/python/jittor/src/jit_compiler.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/jit_key.cc` & `jittor-1.3.8.5/python/jittor/src/jit_key.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/jit_key.h` & `jittor-1.3.8.5/python/jittor/src/jit_key.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/lock.cc` & `jittor-1.3.8.5/python/jittor/src/lock.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/lock.h` & `jittor-1.3.8.5/python/jittor/src/lock.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/aligned_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/aligned_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/aligned_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/aligned_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_device_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_device_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_device_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_device_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_dual_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_dual_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_dual_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_dual_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_host_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_host_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_host_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_host_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_managed_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_managed_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/cuda_managed_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/cuda_managed_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/foreign_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/foreign_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/foreign_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/foreign_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/nfef_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/nfef_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/nfef_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/nfef_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/sfrl_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/sfrl_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/sfrl_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/sfrl_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/stat_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/stat_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/stat_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/stat_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/temp_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/temp_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator/temp_allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator/temp_allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator.cc` & `jittor-1.3.8.5/python/jittor/src/mem/allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/allocator.h` & `jittor-1.3.8.5/python/jittor/src/mem/allocator.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/mem_info.cc` & `jittor-1.3.8.5/python/jittor/src/mem/mem_info.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/mem_info.h` & `jittor-1.3.8.5/python/jittor/src/mem/mem_info.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/swap.cc` & `jittor-1.3.8.5/python/jittor/src/mem/swap.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/mem/swap.h` & `jittor-1.3.8.5/python/jittor/src/mem/swap.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/memory_profiler.cc` & `jittor-1.3.8.5/python/jittor/src/memory_profiler.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/memory_profiler.h` & `jittor-1.3.8.5/python/jittor/src/memory_profiler.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/cpu_atomic.h` & `jittor-1.3.8.5/python/jittor/src/misc/cpu_atomic.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/cpu_math.cc` & `jittor-1.3.8.5/python/jittor/src/misc/cpu_math.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/cstr.h` & `jittor-1.3.8.5/python/jittor/src/misc/cstr.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/cuda_atomic.h` & `jittor-1.3.8.5/python/jittor/src/misc/cuda_atomic.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/cuda_flags.cc` & `jittor-1.3.8.5/python/jittor/src/misc/cuda_flags.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/cuda_flags.h` & `jittor-1.3.8.5/python/jittor/src/misc/cuda_flags.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/cuda_limits.h` & `jittor-1.3.8.5/python/jittor/src/misc/cuda_limits.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/deleter.h` & `jittor-1.3.8.5/python/jittor/src/misc/deleter.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/fast_shared_ptr.h` & `jittor-1.3.8.5/python/jittor/src/misc/fast_shared_ptr.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/hash.h` & `jittor-1.3.8.5/python/jittor/src/misc/hash.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/intrin.h` & `jittor-1.3.8.5/python/jittor/src/misc/intrin.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/miniz.cc` & `jittor-1.3.8.5/python/jittor/src/misc/miniz.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/miniz.h` & `jittor-1.3.8.5/python/jittor/src/misc/miniz.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/nan_checker.cc` & `jittor-1.3.8.5/python/jittor/src/misc/nan_checker.cc`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 // Copyright (c) 2023 Jittor. All Rights Reserved.
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #include <cfloat>
 #include <cmath>
 #include "misc/nan_checker.h"
-#ifdef HAS_CUDA
+#ifdef IS_CUDA
 #include "misc/cuda_flags.h"
 #include <cuda_runtime.h>
 #include <cuda_fp16.h>
 #include "helper_cuda.h"
 #endif
 #include "mem/allocator.h"
 #include "op.h"
```

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/nan_checker.cu` & `jittor-1.3.8.5/python/jittor/src/misc/nan_checker.cu`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/nano_string.cc` & `jittor-1.3.8.5/python/jittor/src/misc/nano_string.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/nano_string.h` & `jittor-1.3.8.5/python/jittor/src/misc/nano_string.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/nano_vector.h` & `jittor-1.3.8.5/python/jittor/src/misc/nano_vector.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/ring_buffer.cc` & `jittor-1.3.8.5/python/jittor/src/misc/ring_buffer.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/ring_buffer.h` & `jittor-1.3.8.5/python/jittor/src/misc/ring_buffer.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/stack_vector.h` & `jittor-1.3.8.5/python/jittor/src/misc/stack_vector.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/misc/string_view_map.h` & `jittor-1.3.8.5/python/jittor/src/misc/string_view_map.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/node.h` & `jittor-1.3.8.5/python/jittor/src/node.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/numpy_func.h` & `jittor-1.3.8.5/python/jittor/src/numpy_func.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/op.cc` & `jittor-1.3.8.5/python/jittor/src/op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/op.h` & `jittor-1.3.8.5/python/jittor/src/op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/op_compiler.cc` & `jittor-1.3.8.5/python/jittor/src/op_compiler.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/op_compiler.h` & `jittor-1.3.8.5/python/jittor/src/op_compiler.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/arg_reduce_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/arg_reduce_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/arg_reduce_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/arg_reduce_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/argsort_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/argsort_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/argsort_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/argsort_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/array_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/array_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/array_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/array_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/binary_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/binary_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/binary_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/binary_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/broadcast_to_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/broadcast_to_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/broadcast_to_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/broadcast_to_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/candidate_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/candidate_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/candidate_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/candidate_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/clone_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/clone_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/clone_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/clone_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/code_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/code_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/code_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/code_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/copy_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/copy_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/copy_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/copy_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/empty_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/empty_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/empty_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/empty_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/fetch_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/fetch_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/fetch_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/fetch_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/fuse_transpose_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/fuse_transpose_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/fuse_transpose_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/fuse_transpose_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/getitem_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/getitem_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/getitem_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/getitem_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/index_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/index_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/index_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/index_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/numpy_code_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/numpy_code_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/numpy_code_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/numpy_code_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/op_register.cc` & `jittor-1.3.8.5/python/jittor/src/ops/op_register.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/op_register.h` & `jittor-1.3.8.5/python/jittor/src/ops/op_register.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/op_utils.cc` & `jittor-1.3.8.5/python/jittor/src/ops/op_utils.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/random_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/random_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/random_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/random_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/reduce_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/reduce_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/reduce_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/reduce_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/reindex_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/reindex_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/reindex_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/reindex_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/reindex_reduce_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/reindex_reduce_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/reindex_reduce_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/reindex_reduce_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/reshape_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/reshape_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/reshape_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/reshape_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/safe_clip_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/safe_clip_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/safe_clip_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/safe_clip_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/setitem_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/setitem_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/setitem_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/setitem_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/tape_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/tape_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/tape_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/tape_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/ternary_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/ternary_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/ternary_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/ternary_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/transpose_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/transpose_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/transpose_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/transpose_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/unary_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/unary_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/unary_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/unary_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/where_op.cc` & `jittor-1.3.8.5/python/jittor/src/ops/where_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/ops/where_op.h` & `jittor-1.3.8.5/python/jittor/src/ops/where_op.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/expr.cc` & `jittor-1.3.8.5/python/jittor/src/opt/expr.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/expr.h` & `jittor-1.3.8.5/python/jittor/src/opt/expr.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/gopt/setitem_gopt.cc` & `jittor-1.3.8.5/python/jittor/src/opt/gopt/setitem_gopt.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/jit_searcher.cc` & `jittor-1.3.8.5/python/jittor/src/opt/jit_searcher.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/jit_searcher.h` & `jittor-1.3.8.5/python/jittor/src/opt/jit_searcher.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/kernel_ir.cc` & `jittor-1.3.8.5/python/jittor/src/opt/kernel_ir.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/kernel_ir.h` & `jittor-1.3.8.5/python/jittor/src/opt/kernel_ir.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/assume_aligned_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/assume_aligned_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/assume_aligned_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/assume_aligned_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/atomic_tuner_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/atomic_tuner_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/check_cache_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/check_cache_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/check_cache_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/check_cache_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/compile_shapes_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/compile_shapes_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/compile_shapes_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/compile_shapes_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/const_var_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/const_var_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/const_var_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/const_var_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/expand_empty_block_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/expand_empty_block_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/expand_empty_block_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/expand_empty_block_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/fake_main_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/fake_main_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/fake_main_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/fake_main_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/float_atomic_fix_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/float_atomic_fix_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/float_atomic_fix_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/float_atomic_fix_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/insert_profile_loop_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/insert_profile_loop_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/insert_profile_loop_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/insert_profile_loop_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/loop_to_func_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/loop_to_func_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/loop_to_func_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/loop_to_func_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/loop_var_analyze_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/loop_var_analyze_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/loop_var_analyze_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/loop_var_analyze_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/mark_raw_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/mark_raw_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/mark_raw_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/mark_raw_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/merge_loop_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/merge_loop_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/merge_loop_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/merge_loop_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/merge_loop_var_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/merge_loop_var_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/merge_loop_var_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/merge_loop_var_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/parallel_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/parallel_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/remove_intermediate_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/remove_intermediate_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/remove_intermediate_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/remove_intermediate_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/remove_loop_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/remove_loop_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/remove_loop_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/remove_loop_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/rename_loop_index_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/rename_loop_index_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/rename_loop_index_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/rename_loop_index_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/reorder_loop_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/reorder_loop_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/reorder_loop_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/reorder_loop_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/replace_for_num_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/replace_for_num_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/replace_for_num_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/replace_for_num_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/restride_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/restride_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/restride_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/restride_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/shared_reduce_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/shared_reduce_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/solve_conflict_define_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/solve_conflict_define_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/solve_conflict_define_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/solve_conflict_define_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/split_loop_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/split_loop_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/split_loop_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/split_loop_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/unroll_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/unroll_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/unroll_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/unroll_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/use_movnt_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/use_movnt_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/use_movnt_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/use_movnt_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/vectorize_pass.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass/vectorize_pass.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass/vectorize_pass.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass/vectorize_pass.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass_manager.cc` & `jittor-1.3.8.5/python/jittor/src/opt/pass_manager.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/pass_manager.h` & `jittor-1.3.8.5/python/jittor/src/opt/pass_manager.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/broadcast_tuner.cc` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/broadcast_tuner.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/broadcast_tuner.h` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/broadcast_tuner.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/conv_tuner.cc` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/conv_tuner.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/conv_tuner.h` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/conv_tuner.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/matmul_tuner.cc` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/matmul_tuner.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/matmul_tuner.h` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/matmul_tuner.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/reduce_tuner.cc` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/reduce_tuner.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/reduce_tuner.h` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/reduce_tuner.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/reorder_tuner.cc` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/reorder_tuner.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/reorder_tuner.h` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/reorder_tuner.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/tuner.cc` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/tuner.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner/tuner.h` & `jittor-1.3.8.5/python/jittor/src/opt/tuner/tuner.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner_manager.cc` & `jittor-1.3.8.5/python/jittor/src/opt/tuner_manager.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/tuner_manager.h` & `jittor-1.3.8.5/python/jittor/src/opt/tuner_manager.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/var_relay.cc` & `jittor-1.3.8.5/python/jittor/src/opt/var_relay.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/opt/var_relay.h` & `jittor-1.3.8.5/python/jittor/src/opt/var_relay.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/parallel_compiler.cc` & `jittor-1.3.8.5/python/jittor/src/parallel_compiler.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/parallel_compiler.h` & `jittor-1.3.8.5/python/jittor/src/parallel_compiler.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/cache_info.cc` & `jittor-1.3.8.5/python/jittor/src/profiler/cache_info.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/cache_info.h` & `jittor-1.3.8.5/python/jittor/src/profiler/cache_info.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/memory_checker.cc` & `jittor-1.3.8.5/python/jittor/src/profiler/memory_checker.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/memory_checker.h` & `jittor-1.3.8.5/python/jittor/src/profiler/memory_checker.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/profiler.cc` & `jittor-1.3.8.5/python/jittor/src/profiler/profiler.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/profiler.h` & `jittor-1.3.8.5/python/jittor/src/profiler/profiler.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/profiler_guard.h` & `jittor-1.3.8.5/python/jittor/src/profiler/profiler_guard.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/replacement.cc` & `jittor-1.3.8.5/python/jittor/src/profiler/replacement.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/replacement.h` & `jittor-1.3.8.5/python/jittor/src/profiler/replacement.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/simple_profiler.h` & `jittor-1.3.8.5/python/jittor/src/profiler/simple_profiler.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/profiler/vtop.cc` & `jittor-1.3.8.5/python/jittor/src/profiler/vtop.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pybind/core.cc` & `jittor-1.3.8.5/python/jittor/src/pybind/core.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pybind/py_var_tracer.cc` & `jittor-1.3.8.5/python/jittor/src/pybind/py_var_tracer.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pybind/py_var_tracer.h` & `jittor-1.3.8.5/python/jittor/src/pybind/py_var_tracer.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pybind/py_var_tracer_interface.h` & `jittor-1.3.8.5/python/jittor/src/pybind/py_var_tracer_interface.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/numpy.cc` & `jittor-1.3.8.5/python/jittor/src/pyjt/numpy.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/numpy.h` & `jittor-1.3.8.5/python/jittor/src/pyjt/numpy.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_arg_printer.cc` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_arg_printer.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_arg_printer.h` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_arg_printer.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_array_op.cc` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_array_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_caller.cc` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_caller.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_caller.h` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_caller.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_converter.h` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_converter.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_obj_holder.h` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_obj_holder.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_ring_buffer.cc` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_ring_buffer.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/py_ring_buffer.h` & `jittor-1.3.8.5/python/jittor/src/pyjt/py_ring_buffer.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/pyjt/pyjt_console.h` & `jittor-1.3.8.5/python/jittor/src/pyjt/pyjt_console.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_expr.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_expr.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_fast_shared_ptr.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_fast_shared_ptr.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_jit_key.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_jit_key.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_kernel_ir.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_kernel_ir.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_nano_vector.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_nano_vector.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_op_compiler.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_op_compiler.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_op_relay.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_op_relay.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_setitem_op.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_setitem_op.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/test/test_sfrl_allocator.cc` & `jittor-1.3.8.5/python/jittor/src/test/test_sfrl_allocator.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/type/common_op_type.cc` & `jittor-1.3.8.5/python/jittor/src/type/common_op_type.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/type/fp16_compute.h` & `jittor-1.3.8.5/python/jittor/src/type/fp16_compute.h`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 // Maintainers: Dun Liang <randonlang@gmail.com>. 
 // This file is subject to the terms and conditions defined in
 // file 'LICENSE.txt', which is part of this source code package.
 // ***************************************************************
 #pragma once
 #include "common.h"
 
-#ifdef JIT_cuda
+#if defined(JIT_cuda) && !defined(IS_ACL)
 
 #include <driver_types.h>
 #include <cuda_fp16.h>
 
 namespace jittor {
 
 typedef __half float16;
```

### Comparing `jittor-1.3.8.4/python/jittor/src/type/fp16_op_type.cc` & `jittor-1.3.8.5/python/jittor/src/type/fp16_op_type.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/types.h` & `jittor-1.3.8.5/python/jittor/src/types.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/cache_compile.cc` & `jittor-1.3.8.5/python/jittor/src/utils/cache_compile.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/cache_compile.h` & `jittor-1.3.8.5/python/jittor/src/utils/cache_compile.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/cross_platform.h` & `jittor-1.3.8.5/python/jittor/src/utils/cross_platform.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/flags.cc` & `jittor-1.3.8.5/python/jittor/src/utils/flags.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/jit_utils.cc` & `jittor-1.3.8.5/python/jittor/src/utils/jit_utils.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/log.cc` & `jittor-1.3.8.5/python/jittor/src/utils/log.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/log.h` & `jittor-1.3.8.5/python/jittor/src/utils/log.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/mwsr_list.cc` & `jittor-1.3.8.5/python/jittor/src/utils/mwsr_list.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/mwsr_list.h` & `jittor-1.3.8.5/python/jittor/src/utils/mwsr_list.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/seh.h` & `jittor-1.3.8.5/python/jittor/src/utils/seh.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/str_utils.cc` & `jittor-1.3.8.5/python/jittor/src/utils/str_utils.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/str_utils.h` & `jittor-1.3.8.5/python/jittor/src/utils/str_utils.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/utils/tracer.cc` & `jittor-1.3.8.5/python/jittor/src/utils/tracer.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/var.cc` & `jittor-1.3.8.5/python/jittor/src/var.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/var.h` & `jittor-1.3.8.5/python/jittor/src/var.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/var_holder.cc` & `jittor-1.3.8.5/python/jittor/src/var_holder.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/var_holder.h` & `jittor-1.3.8.5/python/jittor/src/var_holder.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/var_slices.cc` & `jittor-1.3.8.5/python/jittor/src/var_slices.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/src/var_slices.h` & `jittor-1.3.8.5/python/jittor/src/var_slices.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/__main__.py` & `jittor-1.3.8.5/python/jittor/test/__main__.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/misc/superglue.py` & `jittor-1.3.8.5/python/jittor/test/misc/superglue.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/perf/perf.py` & `jittor-1.3.8.5/python/jittor/test/perf/perf.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh` & `jittor-1.3.8.5/python/jittor/test/system/test_cuda10.0_ubuntu16.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh` & `jittor-1.3.8.5/python/jittor/test/system/test_cuda10.0_ubuntu18.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh` & `jittor-1.3.8.5/python/jittor/test/system/test_cuda11.1_ubuntu16.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/system/test_cuda11.1_ubuntu18.04.sh` & `jittor-1.3.8.5/python/jittor/test/system/test_cuda11.1_ubuntu18.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/system/test_cuda11.1_ubuntu20.04.sh` & `jittor-1.3.8.5/python/jittor/test/system/test_cuda11.1_ubuntu20.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/system/test_nocuda_ubuntu18.04.sh` & `jittor-1.3.8.5/python/jittor/test/system/test_nocuda_ubuntu18.04.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test.h` & `jittor-1.3.8.5/python/jittor/test/test.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_acl.py` & `jittor-1.3.8.5/python/jittor/test/test_acl.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_adamw.py` & `jittor-1.3.8.5/python/jittor/test/test_adamw.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_affine_grid.py` & `jittor-1.3.8.5/python/jittor/test/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_allocator.py` & `jittor-1.3.8.5/python/jittor/test/test_allocator.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_allocator2.py` & `jittor-1.3.8.5/python/jittor/test/test_allocator2.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_arg_pool_op.py` & `jittor-1.3.8.5/python/jittor/test/test_arg_pool_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_arg_reduce_op.py` & `jittor-1.3.8.5/python/jittor/test/test_arg_reduce_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_argsort_op.py` & `jittor-1.3.8.5/python/jittor/test/test_argsort_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_array.py` & `jittor-1.3.8.5/python/jittor/test/test_array.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_asm_tuner.py` & `jittor-1.3.8.5/python/jittor/test/test_asm_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_atomic_tuner.py` & `jittor-1.3.8.5/python/jittor/test/test_atomic_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_attention.py` & `jittor-1.3.8.5/python/jittor/test/test_attention.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_auto_diff.py` & `jittor-1.3.8.5/python/jittor/test/test_auto_diff.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_batchnorm.py` & `jittor-1.3.8.5/python/jittor/test/test_batchnorm.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_benchmark.py` & `jittor-1.3.8.5/python/jittor/test/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_bicubic.py` & `jittor-1.3.8.5/python/jittor/test/test_bicubic.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_binary_op.py` & `jittor-1.3.8.5/python/jittor/test/test_binary_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_bmm.py` & `jittor-1.3.8.5/python/jittor/test/test_bmm.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_broadcast_to_op.py` & `jittor-1.3.8.5/python/jittor/test/test_broadcast_to_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_broadcast_tuner.py` & `jittor-1.3.8.5/python/jittor/test/test_broadcast_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_cache.py` & `jittor-1.3.8.5/python/jittor/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_candidate.py` & `jittor-1.3.8.5/python/jittor/test/test_candidate.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_clone.py` & `jittor-1.3.8.5/python/jittor/test/test_clone.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_code_op.py` & `jittor-1.3.8.5/python/jittor/test/test_code_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_compile_options.py` & `jittor-1.3.8.5/python/jittor/test/test_compile_options.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_concat_op.py` & `jittor-1.3.8.5/python/jittor/test/test_concat_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_console.py` & `jittor-1.3.8.5/python/jittor/test/test_console.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_contrib.py` & `jittor-1.3.8.5/python/jittor/test/test_contrib.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_conv_transpose.py` & `jittor-1.3.8.5/python/jittor/test/test_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_conv_tuner.py` & `jittor-1.3.8.5/python/jittor/test/test_conv_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_core.py` & `jittor-1.3.8.5/python/jittor/test/test_core.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_cub_cumsum.py` & `jittor-1.3.8.5/python/jittor/test/test_cub_cumsum.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_cublas_test_op.py` & `jittor-1.3.8.5/python/jittor/test/test_cublas_test_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_cuda.py` & `jittor-1.3.8.5/python/jittor/test/test_cuda.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_cudnn_op.py` & `jittor-1.3.8.5/python/jittor/test/test_cudnn_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_cumprod_op.py` & `jittor-1.3.8.5/python/jittor/test/test_cumprod_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_custom_op.py` & `jittor-1.3.8.5/python/jittor/test/test_custom_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_cutt.py` & `jittor-1.3.8.5/python/jittor/test/test_cutt.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_cutt_transpose_op.py` & `jittor-1.3.8.5/python/jittor/test/test_cutt_transpose_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_dataset.py` & `jittor-1.3.8.5/python/jittor/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_default_var.py` & `jittor-1.3.8.5/python/jittor/test/test_default_var.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_densenet.py` & `jittor-1.3.8.5/python/jittor/test/test_densenet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_depthwise_conv.py` & `jittor-1.3.8.5/python/jittor/test/test_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_digamma.py` & `jittor-1.3.8.5/python/jittor/test/test_digamma.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_distributions.py` & `jittor-1.3.8.5/python/jittor/test/test_distributions.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_einops.py` & `jittor-1.3.8.5/python/jittor/test/test_einops.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_einsum.py` & `jittor-1.3.8.5/python/jittor/test/test_einsum.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_emnist.py` & `jittor-1.3.8.5/python/jittor/test/test_emnist.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_error_msg.py` & `jittor-1.3.8.5/python/jittor/test/test_error_msg.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_example.py` & `jittor-1.3.8.5/python/jittor/test/test_example.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_example_accumulate_grad.py` & `jittor-1.3.8.5/python/jittor/test/test_example_accumulate_grad.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_fetcher.py` & `jittor-1.3.8.5/python/jittor/test/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_fft_op.py` & `jittor-1.3.8.5/python/jittor/test/test_fft_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_flags.py` & `jittor-1.3.8.5/python/jittor/test/test_flags.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_fold.py` & `jittor-1.3.8.5/python/jittor/test/test_fold.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_fp16.py` & `jittor-1.3.8.5/python/jittor/test/test_fp16.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_function.py` & `jittor-1.3.8.5/python/jittor/test/test_function.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_fused_op.py` & `jittor-1.3.8.5/python/jittor/test/test_fused_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_fuser.py` & `jittor-1.3.8.5/python/jittor/test/test_fuser.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_gamma_distribution.py` & `jittor-1.3.8.5/python/jittor/test/test_gamma_distribution.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_grad.py` & `jittor-1.3.8.5/python/jittor/test/test_grad.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_group_conv_tuner.py` & `jittor-1.3.8.5/python/jittor/test/test_group_conv_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_histc.py` & `jittor-1.3.8.5/python/jittor/test/test_histc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_hook.py` & `jittor-1.3.8.5/python/jittor/test/test_hook.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_image_folder.py` & `jittor-1.3.8.5/python/jittor/test/test_image_folder.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_inception.py` & `jittor-1.3.8.5/python/jittor/test/test_inception.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_index_op.py` & `jittor-1.3.8.5/python/jittor/test/test_index_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_init.py` & `jittor-1.3.8.5/python/jittor/test/test_init.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_interpolation.py` & `jittor-1.3.8.5/python/jittor/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_jit_tests.py` & `jittor-1.3.8.5/python/jittor/test/test_jit_tests.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_jtune.py` & `jittor-1.3.8.5/python/jittor/test/test_jtune.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_knn.py` & `jittor-1.3.8.5/python/jittor/test/test_knn.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_lazy_execution.py` & `jittor-1.3.8.5/python/jittor/test/test_lazy_execution.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_linalg.py` & `jittor-1.3.8.5/python/jittor/test/test_linalg.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_load_pth.py` & `jittor-1.3.8.5/python/jittor/test/test_load_pth.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_lock.py` & `jittor-1.3.8.5/python/jittor/test/test_lock.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_log.py` & `jittor-1.3.8.5/python/jittor/test/test_log.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_longest_dis_fuse.py` & `jittor-1.3.8.5/python/jittor/test/test_longest_dis_fuse.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_loss.py` & `jittor-1.3.8.5/python/jittor/test/test_loss.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_loss3d.py` & `jittor-1.3.8.5/python/jittor/test/test_loss3d.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_lr_scheduler.py` & `jittor-1.3.8.5/python/jittor/test/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_lstm.py` & `jittor-1.3.8.5/python/jittor/test/test_lstm.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_matmul.py` & `jittor-1.3.8.5/python/jittor/test/test_matmul.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_matmul_tuner.py` & `jittor-1.3.8.5/python/jittor/test/test_matmul_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_mem.py` & `jittor-1.3.8.5/python/jittor/test/test_mem.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_memory_profiler.py` & `jittor-1.3.8.5/python/jittor/test/test_memory_profiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_merge_loop_var_pass.py` & `jittor-1.3.8.5/python/jittor/test/test_merge_loop_var_pass.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_merge_single_array_op.py` & `jittor-1.3.8.5/python/jittor/test/test_merge_single_array_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_misc_issue.py` & `jittor-1.3.8.5/python/jittor/test/test_misc_issue.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_misc_op.py` & `jittor-1.3.8.5/python/jittor/test/test_misc_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_mkl_conv_op.py` & `jittor-1.3.8.5/python/jittor/test/test_mkl_conv_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_mkl_test_op.py` & `jittor-1.3.8.5/python/jittor/test/test_mkl_test_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_models.py` & `jittor-1.3.8.5/python/jittor/test/test_models.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_mpi.py` & `jittor-1.3.8.5/python/jittor/test/test_mpi.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_mpi_batchnorm.py` & `jittor-1.3.8.5/python/jittor/test/test_mpi_batchnorm.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_mpi_in_py.py` & `jittor-1.3.8.5/python/jittor/test/test_mpi_in_py.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_mpi_op.py` & `jittor-1.3.8.5/python/jittor/test/test_mpi_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_nano_string.py` & `jittor-1.3.8.5/python/jittor/test/test_nano_string.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_nano_vector.py` & `jittor-1.3.8.5/python/jittor/test/test_nano_vector.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_nccl.py` & `jittor-1.3.8.5/python/jittor/test/test_nccl.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_nccl_ops.py` & `jittor-1.3.8.5/python/jittor/test/test_nccl_ops.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_new_fused_op.py` & `jittor-1.3.8.5/python/jittor/test/test_new_fused_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_node.py` & `jittor-1.3.8.5/python/jittor/test/test_node.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_notebooks.py` & `jittor-1.3.8.5/python/jittor/test/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_numpy_code_op.py` & `jittor-1.3.8.5/python/jittor/test/test_numpy_code_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_op_compiler.py` & `jittor-1.3.8.5/python/jittor/test/test_op_compiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_opt_state_dict.py` & `jittor-1.3.8.5/python/jittor/test/test_opt_state_dict.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_optimizer.py` & `jittor-1.3.8.5/python/jittor/test/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_optimizer_save_load.py` & `jittor-1.3.8.5/python/jittor/test/test_optimizer_save_load.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_pad.py` & `jittor-1.3.8.5/python/jittor/test/test_pad.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_parallel_pass.py` & `jittor-1.3.8.5/python/jittor/test/test_parallel_pass.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_param_list.py` & `jittor-1.3.8.5/python/jittor/test/test_param_list.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_profiler.py` & `jittor-1.3.8.5/python/jittor/test/test_profiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_pytorch_converter.py` & `jittor-1.3.8.5/python/jittor/test/test_pytorch_converter.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_random_op.py` & `jittor-1.3.8.5/python/jittor/test/test_random_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_reduce_op.py` & `jittor-1.3.8.5/python/jittor/test/test_reduce_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_reduce_tuner.py` & `jittor-1.3.8.5/python/jittor/test/test_reduce_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_reindex_op.py` & `jittor-1.3.8.5/python/jittor/test/test_reindex_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_reindex_reduce_op.py` & `jittor-1.3.8.5/python/jittor/test/test_reindex_reduce_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_relu.py` & `jittor-1.3.8.5/python/jittor/test/test_relu.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_reorder_tuner.py` & `jittor-1.3.8.5/python/jittor/test/test_reorder_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_repeat.py` & `jittor-1.3.8.5/python/jittor/test/test_repeat.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_reshape.py` & `jittor-1.3.8.5/python/jittor/test/test_reshape.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_resize_and_crop.py` & `jittor-1.3.8.5/python/jittor/test/test_resize_and_crop.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_resnet.py` & `jittor-1.3.8.5/python/jittor/test/test_resnet.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_ring_buffer.py` & `jittor-1.3.8.5/python/jittor/test/test_ring_buffer.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_ring_buffer2.py` & `jittor-1.3.8.5/python/jittor/test/test_ring_buffer2.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_rnn.py` & `jittor-1.3.8.5/python/jittor/test/test_rnn.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_rocm.py` & `jittor-1.3.8.5/python/jittor/test/test_rocm.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_sampler.py` & `jittor-1.3.8.5/python/jittor/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_search_sorted.py` & `jittor-1.3.8.5/python/jittor/test/test_search_sorted.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_searchsorted_op.py` & `jittor-1.3.8.5/python/jittor/test/test_searchsorted_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_setitem.py` & `jittor-1.3.8.5/python/jittor/test/test_setitem.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_single_process_scope.py` & `jittor-1.3.8.5/python/jittor/test/test_single_process_scope.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_slice.py` & `jittor-1.3.8.5/python/jittor/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_sparse.py` & `jittor-1.3.8.5/python/jittor/test/test_sparse.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_stop_fuse.py` & `jittor-1.3.8.5/python/jittor/test/test_stop_fuse.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_superglue.py` & `jittor-1.3.8.5/python/jittor/test/test_superglue.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_ternary_op.py` & `jittor-1.3.8.5/python/jittor/test/test_ternary_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_trace_var.py` & `jittor-1.3.8.5/python/jittor/test/test_trace_var.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_tracer.py` & `jittor-1.3.8.5/python/jittor/test/test_tracer.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_transform.py` & `jittor-1.3.8.5/python/jittor/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_transpose_op.py` & `jittor-1.3.8.5/python/jittor/test/test_transpose_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_unary_op.py` & `jittor-1.3.8.5/python/jittor/test/test_unary_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_unique.py` & `jittor-1.3.8.5/python/jittor/test/test_unique.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_utils.py` & `jittor-1.3.8.5/python/jittor/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_var.py` & `jittor-1.3.8.5/python/jittor/test/test_var.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_vgg.py` & `jittor-1.3.8.5/python/jittor/test/test_vgg.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_weightnorm.py` & `jittor-1.3.8.5/python/jittor/test/test_weightnorm.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/test/test_where_op.py` & `jittor-1.3.8.5/python/jittor/test/test_where_op.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/transform/__init__.py` & `jittor-1.3.8.5/python/jittor/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/transform/function_pil.py` & `jittor-1.3.8.5/python/jittor/transform/function_pil.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/asm_tuner.py` & `jittor-1.3.8.5/python/jittor/utils/asm_tuner.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/converter_server.py` & `jittor-1.3.8.5/python/jittor/utils/converter_server.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/data.gz` & `jittor-1.3.8.5/python/jittor/utils/data.gz`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/dlink_compiler.py` & `jittor-1.3.8.5/python/jittor/utils/dlink_compiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/dumpdef.py` & `jittor-1.3.8.5/python/jittor/utils/dumpdef.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/gen_pyi.py` & `jittor-1.3.8.5/python/jittor/utils/gen_pyi.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/jtune.py` & `jittor-1.3.8.5/python/jittor/utils/jtune.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/local_doc_builder.py` & `jittor-1.3.8.5/python/jittor/utils/local_doc_builder.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/nvtx.py` & `jittor-1.3.8.5/python/jittor/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/polish.py` & `jittor-1.3.8.5/python/jittor/utils/polish.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/polish_centos.py` & `jittor-1.3.8.5/python/jittor/utils/polish_centos.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/publish.py` & `jittor-1.3.8.5/python/jittor/utils/publish.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/pytorch_converter.py` & `jittor-1.3.8.5/python/jittor/utils/pytorch_converter.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/utils/tracer.py` & `jittor-1.3.8.5/python/jittor/utils/tracer.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/vcompiler/vcompiler.cc` & `jittor-1.3.8.5/python/jittor/vcompiler/vcompiler.cc`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/vcompiler/vcompiler.h` & `jittor-1.3.8.5/python/jittor/vcompiler/vcompiler.h`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/vcompiler/vcompiler.py` & `jittor-1.3.8.5/python/jittor/vcompiler/vcompiler.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor/weightnorm.py` & `jittor-1.3.8.5/python/jittor/weightnorm.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor.egg-info/PKG-INFO` & `jittor-1.3.8.5/python/jittor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jittor
-Version: 1.3.8.4
+Version: 1.3.8.5
 Summary: a Just-in-time(JIT) deep learning framework
 Home-page: http://jittor.org
 Author: Jittor Group
 Author-email: ran.donglang@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `jittor-1.3.8.4/python/jittor.egg-info/SOURCES.txt` & `jittor-1.3.8.5/python/jittor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/__init__.py` & `jittor-1.3.8.5/python/jittor_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/auto_diff.py` & `jittor-1.3.8.5/python/jittor_utils/auto_diff.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/auto_git_tag.py` & `jittor-1.3.8.5/python/jittor_utils/auto_git_tag.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/class/motd` & `jittor-1.3.8.5/python/jittor_utils/class/motd`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/class/setup_env.py` & `jittor-1.3.8.5/python/jittor_utils/class/setup_env.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/clean_cache.py` & `jittor-1.3.8.5/python/jittor_utils/clean_cache.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/config.py` & `jittor-1.3.8.5/python/jittor_utils/config.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/github_release.sh` & `jittor-1.3.8.5/python/jittor_utils/github_release.sh`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/install_cuda.py` & `jittor-1.3.8.5/python/jittor_utils/install_cuda.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/load_pytorch.py` & `jittor-1.3.8.5/python/jittor_utils/load_pytorch.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/load_pytorch_old.py` & `jittor-1.3.8.5/python/jittor_utils/load_pytorch_old.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/lock.py` & `jittor-1.3.8.5/python/jittor_utils/lock.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/misc.py` & `jittor-1.3.8.5/python/jittor_utils/misc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/pack_offline.py` & `jittor-1.3.8.5/python/jittor_utils/pack_offline.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/pip_publish.py` & `jittor-1.3.8.5/python/jittor_utils/pip_publish.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/query_cuda_cc.py` & `jittor-1.3.8.5/python/jittor_utils/query_cuda_cc.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/ring_buffer.py` & `jittor-1.3.8.5/python/jittor_utils/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/student_queue.py` & `jittor-1.3.8.5/python/jittor_utils/student_queue.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/python/jittor_utils/translator.py` & `jittor-1.3.8.5/python/jittor_utils/translator.py`

 * *Files identical despite different names*

### Comparing `jittor-1.3.8.4/setup.py` & `jittor-1.3.8.5/setup.py`

 * *Files identical despite different names*

