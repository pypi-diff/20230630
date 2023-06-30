# Comparing `tmp/giskard-2.0.0b8.tar.gz` & `tmp/giskard-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.0.0b8.tar", last modified: Wed Jun 14 18:52:33 2023, max compression
+gzip compressed data, was "giskard-2.0.0b9.tar", last modified: Wed Jun 21 16:41:13 2023, max compression
```

## Comparing `giskard-2.0.0b8.tar` & `giskard-2.0.0b9.tar`

### file list

```diff
@@ -1,220 +1,227 @@
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.256336 giskard-2.0.0b8/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-14 18:52:33.256489 giskard-2.0.0b8/PKG-INFO
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-14 09:16:20.000000 giskard-2.0.0b8/README.md
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.132049 giskard-2.0.0b8/giskard/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1836 2023-06-13 13:04:39.000000 giskard-2.0.0b8/giskard/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/cli.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/cli_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.142868 giskard-2.0.0b8/giskard/client/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/client/dtos.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11481 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/client/giskard_client.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/client/io_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3602 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/client/project.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b8/giskard/client/python_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.144067 giskard-2.0.0b8/giskard/commands/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    16407 2023-06-13 13:05:12.000000 giskard-2.0.0b8/giskard/commands/cli_server.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7604 2023-06-13 13:04:39.000000 giskard-2.0.0b8/giskard/commands/cli_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.147039 giskard-2.0.0b8/giskard/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/core/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11813 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/core.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/dataset_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      886 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/errors.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13213 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/model_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    16026 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/suite.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      560 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/core/validation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.147301 giskard-2.0.0b8/giskard/datasets/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2691 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/datasets/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.147634 giskard-2.0.0b8/giskard/datasets/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26225 2023-06-12 16:43:48.000000 giskard-2.0.0b8/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.150320 giskard-2.0.0b8/giskard/datasets/metadata/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/datasets/metadata/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.152361 giskard-2.0.0b8/giskard/demo/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2922 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/demo/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/demo/titanic.csv
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.156144 giskard-2.0.0b8/giskard/ml_worker/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.159135 giskard-2.0.0b8/giskard/ml_worker/bridge/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/bridge/ml_worker_bridge.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/ml_worker/bridge/service_messages.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.161230 giskard-2.0.0b8/giskard/ml_worker/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/core/log_listener.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5857 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/core/savable.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.162223 giskard-2.0.0b8/giskard/ml_worker/exceptions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/exceptions/IllegalArgumentError.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/exceptions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/exceptions/giskard_exception.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.168126 giskard-2.0.0b8/giskard/ml_worker/generated/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard/ml_worker/generated/ml_worker_pb2.py
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3222 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.169046 giskard-2.0.0b8/giskard/ml_worker/server/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/server/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26239 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/server/ml_worker_service.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.177369 giskard-2.0.0b8/giskard/ml_worker/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b8/giskard/ml_worker/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.178635 giskard-2.0.0b8/giskard/ml_worker/testing/functions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      160 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/functions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3919 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/functions/slicing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6585 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/functions/transformation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.193982 giskard-2.0.0b8/giskard/ml_worker/testing/registry/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1800 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2356 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/decorators_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/giskard_test.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6454 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/slicing_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5376 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/transformation_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1796 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/registry/udf_repository.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/ml_worker/testing/stat_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2634 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/test_result.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/testing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.200281 giskard-2.0.0b8/giskard/ml_worker/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b8/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/ml_worker/utils/file_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/ml_worker/utils/logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1951 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/utils/network.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2502 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/ml_worker/utils/request_interceptor.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.202368 giskard-2.0.0b8/giskard/models/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2191 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/_precooked.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.204402 giskard-2.0.0b8/giskard/models/automodel/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9234 2023-06-13 13:04:39.000000 giskard-2.0.0b8/giskard/models/automodel/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.207871 giskard-2.0.0b8/giskard/models/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.208632 giskard-2.0.0b8/giskard/models/cache/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/cache/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/cache/cache.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.208903 giskard-2.0.0b8/giskard/models/catboost/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/catboost/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.209192 giskard-2.0.0b8/giskard/models/function/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/function/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.209482 giskard-2.0.0b8/giskard/models/huggingface/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/huggingface/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.209772 giskard-2.0.0b8/giskard/models/langchain/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2643 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/langchain/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6343 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/model_explanation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.210061 giskard-2.0.0b8/giskard/models/pytorch/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/pytorch/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.210305 giskard-2.0.0b8/giskard/models/sklearn/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/models/sklearn/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.211218 giskard-2.0.0b8/giskard/models/tensorflow/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1618 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/tensorflow/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      845 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/models/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/path_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.220153 giskard-2.0.0b8/giskard/scanner/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.222996 giskard-2.0.0b8/giskard/scanner/calibration/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-14 17:21:01.000000 giskard-2.0.0b8/giskard/scanner/calibration/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-14 17:21:01.000000 giskard-2.0.0b8/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-14 17:21:01.000000 giskard-2.0.0b8/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.223721 giskard-2.0.0b8/giskard/scanner/common/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/common/examples.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/common/loss_based_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.224017 giskard-2.0.0b8/giskard/scanner/data_leakage/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/scanner/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/issues.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.224459 giskard-2.0.0b8/giskard/scanner/llm/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/llm/toxicity_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/llm/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/logger.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.226231 giskard-2.0.0b8/giskard/scanner/performance/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/scanner/performance/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/performance/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/performance/metrics.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/scanner/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3820 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/result.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.231364 giskard-2.0.0b8/giskard/scanner/robustness/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      964 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/robustness/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1077 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11957 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/scanner.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.231628 giskard-2.0.0b8/giskard/scanner/stochasticity/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.233559 giskard-2.0.0b8/giskard/scanner/templates/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_code_snippet.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.235744 giskard-2.0.0b8/giskard/scanner/templates/_issues/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/data_leakage.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/default.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/llm_toxicity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/overconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/performance.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/robustness.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/stochasticity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues/underconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/_issues_table.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/templates/_main_content.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/templates/_tab_header.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/base.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/scan_results.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.237331 giskard-2.0.0b8/giskard/scanner/templates/static/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/static/external.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-14 09:16:20.000000 giskard-2.0.0b8/giskard/scanner/templates/static/style.css
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.237797 giskard-2.0.0b8/giskard/scanner/visualization/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/scanner/visualization/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/scanner/visualization/custom_jinja.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/settings.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.242349 giskard-2.0.0b8/giskard/slicing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/base.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/category_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/opt_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10349 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/slicing/slice.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11248 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/slicing/stop_words.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/slicing/text_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/slicing/tree_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/slicing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.242689 giskard-2.0.0b8/giskard/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.245022 giskard-2.0.0b8/giskard/testing/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b8/giskard/testing/tests/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33165 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/tests/drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30188 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25824 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/tests/performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10353 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.247262 giskard-2.0.0b8/giskard/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-14 08:04:46.000000 giskard-2.0.0b8/giskard/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7144 2023-06-13 13:04:55.000000 giskard-2.0.0b8/giskard/utils/analytics_collector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/utils/display.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-09 09:22:23.000000 giskard-2.0.0b8/giskard/utils/environment_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.134516 giskard-2.0.0b8/giskard.egg-info/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/PKG-INFO
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/SOURCES.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/dependency_links.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/entry_points.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/requires.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       27 2023-06-14 18:52:33.000000 giskard-2.0.0b8/giskard.egg-info/top_level.txt
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7428 2023-06-14 18:23:36.000000 giskard-2.0.0b8/pyproject.toml
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-14 18:52:33.256888 giskard-2.0.0b8/setup.cfg
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-14 09:21:06.000000 giskard-2.0.0b8/setup.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-14 18:52:33.256101 giskard-2.0.0b8/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1453 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_custom_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14801 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_data_drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6424 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_data_processing_pipeline.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_dataset.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b8/tests/test_logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9561 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_metamorphic_direction.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9533 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_metamorphic_invariance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2402 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2185 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_model_auto_inference.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-07 15:34:18.000000 giskard-2.0.0b8/tests/test_model_explanation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-07 15:34:18.000000 giskard-2.0.0b8/tests/test_model_postprocess.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4573 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_programmatic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4264 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_project_uploads.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4342 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_statistical.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4687 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_upload.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-14 08:04:46.000000 giskard-2.0.0b8/tests/test_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.932316 giskard-2.0.0b9/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-21 16:41:13.932479 giskard-2.0.0b9/PKG-INFO
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-20 09:04:57.000000 giskard-2.0.0b9/README.md
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.887940 giskard-2.0.0b9/giskard/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1836 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/cli.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/cli_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.889672 giskard-2.0.0b9/giskard/client/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/client/dtos.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11481 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/client/giskard_client.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/client/io_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3602 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/client/project.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/client/python_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.890146 giskard-2.0.0b9/giskard/commands/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    17732 2023-06-21 16:24:24.000000 giskard-2.0.0b9/giskard/commands/cli_server.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7604 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/commands/cli_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.894352 giskard-2.0.0b9/giskard/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/core/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11813 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/core/core.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-21 08:57:51.000000 giskard-2.0.0b9/giskard/core/dataset_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      886 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/core/errors.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13248 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/core/model_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    16653 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/core/suite.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      560 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/core/validation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.894490 giskard-2.0.0b9/giskard/datasets/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2691 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/datasets/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.894618 giskard-2.0.0b9/giskard/datasets/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26225 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.895556 giskard-2.0.0b9/giskard/datasets/metadata/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.896179 giskard-2.0.0b9/giskard/demo/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      581 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/demo/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      532 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/demo/linear_regression.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/demo/titanic.csv
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2299 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/demo/titanic_classification.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.896397 giskard-2.0.0b9/giskard/ml_worker/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.897187 giskard-2.0.0b9/giskard/ml_worker/bridge/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/bridge/ml_worker_bridge.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/bridge/service_messages.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.899777 giskard-2.0.0b9/giskard/ml_worker/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/core/log_listener.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5857 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/core/savable.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.901470 giskard-2.0.0b9/giskard/ml_worker/exceptions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/exceptions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/exceptions/giskard_exception.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.901779 giskard-2.0.0b9/giskard/ml_worker/generated/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51532 2023-06-21 16:41:13.000000 giskard-2.0.0b9/giskard/ml_worker/generated/ml_worker_pb2.py
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-21 16:41:13.000000 giskard-2.0.0b9/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3222 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.902016 giskard-2.0.0b9/giskard/ml_worker/server/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/server/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26282 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/ml_worker/server/ml_worker_service.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.902683 giskard-2.0.0b9/giskard/ml_worker/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.909293 giskard-2.0.0b9/giskard/ml_worker/testing/functions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      160 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/testing/functions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3919 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/ml_worker/testing/functions/slicing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6585 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/testing/functions/transformation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.911705 giskard-2.0.0b9/giskard/ml_worker/testing/registry/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:57.000000 giskard-2.0.0b9/giskard/ml_worker/testing/registry/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1800 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/testing/registry/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2356 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/testing/registry/decorators_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/ml_worker/testing/registry/giskard_test.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3944 2023-06-21 08:57:51.000000 giskard-2.0.0b9/giskard/ml_worker/testing/registry/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6454 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/testing/registry/slicing_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5376 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/testing/registry/transformation_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1796 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/testing/registry/udf_repository.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/ml_worker/testing/stat_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2661 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/ml_worker/testing/test_result.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/testing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.912483 giskard-2.0.0b9/giskard/ml_worker/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/ml_worker/utils/file_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/ml_worker/utils/logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1951 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/utils/network.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2502 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/ml_worker/utils/request_interceptor.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.913091 giskard-2.0.0b9/giskard/models/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/models/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2191 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/models/_precooked.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.913313 giskard-2.0.0b9/giskard/models/automodel/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9234 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/models/automodel/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.913447 giskard-2.0.0b9/giskard/models/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/models/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.914011 giskard-2.0.0b9/giskard/models/cache/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/models/cache/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/models/cache/cache.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.914146 giskard-2.0.0b9/giskard/models/catboost/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/models/catboost/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.914281 giskard-2.0.0b9/giskard/models/function/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/models/function/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.914424 giskard-2.0.0b9/giskard/models/huggingface/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/models/huggingface/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.914555 giskard-2.0.0b9/giskard/models/langchain/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2643 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/models/langchain/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6343 2023-06-21 08:59:46.000000 giskard-2.0.0b9/giskard/models/model_explanation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.914682 giskard-2.0.0b9/giskard/models/pytorch/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/models/pytorch/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.914808 giskard-2.0.0b9/giskard/models/sklearn/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/models/sklearn/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.914935 giskard-2.0.0b9/giskard/models/tensorflow/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1618 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/models/tensorflow/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      878 2023-06-21 15:47:42.000000 giskard-2.0.0b9/giskard/models/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/path_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.916173 giskard-2.0.0b9/giskard/scanner/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1645 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.916738 giskard-2.0.0b9/giskard/scanner/calibration/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4857 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/scanner/calibration/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3492 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3653 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.917013 giskard-2.0.0b9/giskard/scanner/common/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2772 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/common/examples.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4230 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/common/loss_based_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.917158 giskard-2.0.0b9/giskard/scanner/correlation/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5267 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/correlation/spurious_correlation_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.917305 giskard-2.0.0b9/giskard/scanner/data_leakage/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/issues.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.917598 giskard-2.0.0b9/giskard/scanner/llm/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/llm/toxicity_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/llm/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/logger.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.918463 giskard-2.0.0b9/giskard/scanner/performance/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-21 14:43:16.000000 giskard-2.0.0b9/giskard/scanner/performance/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-21 14:43:16.000000 giskard-2.0.0b9/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-21 14:43:16.000000 giskard-2.0.0b9/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3992 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/result.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.921106 giskard-2.0.0b9/giskard/scanner/robustness/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      964 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/robustness/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1077 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11957 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/scanner.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.921295 giskard-2.0.0b9/giskard/scanner/stochasticity/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.922315 giskard-2.0.0b9/giskard/scanner/templates/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/_code_snippet.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.923581 giskard-2.0.0b9/giskard/scanner/templates/_issues/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/data_leakage.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/default.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/llm_toxicity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/overconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-21 14:43:16.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/performance.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/robustness.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1623 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/spurious_correlation.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/stochasticity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues/underconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1405 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/templates/_issues_table.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7461 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/templates/_main_content.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3034 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/templates/_tab_header.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/base.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/scan_results.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.924240 giskard-2.0.0b9/giskard/scanner/templates/static/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13030 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/scanner/templates/static/style.css
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.924475 giskard-2.0.0b9/giskard/scanner/visualization/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/visualization/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/scanner/visualization/custom_jinja.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/settings.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.926276 giskard-2.0.0b9/giskard/slicing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/slicing/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/slicing/base.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/slicing/category_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10349 2023-06-21 08:57:51.000000 giskard-2.0.0b9/giskard/slicing/slice.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1509 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/slicing/slice_finder.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11248 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/slicing/stop_words.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7761 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/slicing/text_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3933 2023-06-21 15:49:30.000000 giskard-2.0.0b9/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/slicing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.926498 giskard-2.0.0b9/giskard/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.928176 giskard-2.0.0b9/giskard/testing/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/testing/tests/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6575 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/testing/tests/calibration.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33165 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/testing/tests/drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30188 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25824 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/testing/tests/performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10353 2023-06-21 09:01:08.000000 giskard-2.0.0b9/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.928892 giskard-2.0.0b9/giskard/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-20 09:23:32.000000 giskard-2.0.0b9/giskard/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7565 2023-06-21 16:23:48.000000 giskard-2.0.0b9/giskard/utils/analytics_collector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/utils/display.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-20 09:04:58.000000 giskard-2.0.0b9/giskard/utils/environment_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.888836 giskard-2.0.0b9/giskard.egg-info/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-21 16:41:13.000000 giskard-2.0.0b9/giskard.egg-info/PKG-INFO
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6434 2023-06-21 16:41:13.000000 giskard-2.0.0b9/giskard.egg-info/SOURCES.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-21 16:41:13.000000 giskard-2.0.0b9/giskard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-21 16:41:13.000000 giskard-2.0.0b9/giskard.egg-info/entry_points.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      618 2023-06-21 16:41:13.000000 giskard-2.0.0b9/giskard.egg-info/requires.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        8 2023-06-21 16:41:13.000000 giskard-2.0.0b9/giskard.egg-info/top_level.txt
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7483 2023-06-21 15:48:47.000000 giskard-2.0.0b9/pyproject.toml
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-21 16:41:13.932858 giskard-2.0.0b9/setup.cfg
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-20 09:23:32.000000 giskard-2.0.0b9/setup.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-21 16:41:13.932125 giskard-2.0.0b9/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1453 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_custom_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14801 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_data_drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6424 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_dataset.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-06-20 09:04:58.000000 giskard-2.0.0b9/tests/test_logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9561 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_metamorphic_direction.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9533 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2402 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2185 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_model_auto_inference.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-20 09:04:58.000000 giskard-2.0.0b9/tests/test_model_explanation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-20 09:04:58.000000 giskard-2.0.0b9/tests/test_model_postprocess.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5494 2023-06-21 15:49:30.000000 giskard-2.0.0b9/tests/test_programmatic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4264 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_project_uploads.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4342 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_statistical.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4687 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_upload.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-20 09:23:32.000000 giskard-2.0.0b9/tests/test_utils.py
```

### Comparing `giskard-2.0.0b8/PKG-INFO` & `giskard-2.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b8 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b9 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
```

### Comparing `giskard-2.0.0b8/README.md` & `giskard-2.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/__init__.py` & `giskard-2.0.0b9/giskard/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/cli.py` & `giskard-2.0.0b9/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/cli_utils.py` & `giskard-2.0.0b9/giskard/cli_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/client/giskard_client.py` & `giskard-2.0.0b9/giskard/client/giskard_client.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/client/io_utils.py` & `giskard-2.0.0b9/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/client/project.py` & `giskard-2.0.0b9/giskard/client/project.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/client/python_utils.py` & `giskard-2.0.0b9/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/commands/cli_server.py` & `giskard-2.0.0b9/giskard/commands/cli_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import time
 from pathlib import Path
 from typing import Optional
 from urllib.parse import urlparse
 
 import click
 import docker
 import requests
@@ -36,26 +37,23 @@
 - sudo curl -fsSL https://get.docker.com -o get-docker.sh
 - sudo sh get-docker.sh""",
             e,
         )
         exit(1)
 
 
-@click.group("server", help="Giskard UI management", context_settings={"show_default": True})
+@click.group(
+    "server", help="Giskard UI management", context_settings={"show_default": True}
+)
 def server() -> None:
     """
     Giskard UI management
     """
 
 
-def update_options(fn):
-    fn = click.option("--version", "version", is_flag=False, default="", help="Version to update to.")(fn)
-    return fn
-
-
 def get_version(version=None):
     if version:
         current_settings = _get_settings() or {}
         current_settings["version"] = version
         _write_settings(current_settings)
     else:
         app_settings = _get_settings()
@@ -86,20 +84,49 @@
 
 def get_container(version=None, quit_if_not_exists=True) -> Optional[Container]:
     name = get_container_name(version)
     try:
         return create_docker_client().containers.get(name)
     except NotFound:
         if quit_if_not_exists:
-            logger.error(f"Container {name} could not be found. Run `giskard server start` to create the container")
+            logger.error(
+                f"Container {name} could not be found. Run `giskard server start` to create the container"
+            )
             raise click.Abort()
         else:
             return None
 
 
+def _is_backend_ready(endpoint) -> bool:
+    try:
+        response = requests.get(endpoint)
+        response.raise_for_status()
+        return "UP" == response.json()["status"]
+    except KeyboardInterrupt:
+        raise click.Abort()
+    except BaseException:  # noqa NOSONAR
+        return False
+
+
+def _wait_backend_ready(port: int) -> bool:
+    endpoint = f"http://localhost:{port}/management/health"
+    backoff_time = 2
+    max_duration_second = 3 * 60
+    started_time = time.time()
+    up = False
+
+    while not up and time.time() - started_time <= max_duration_second:
+        time.sleep(backoff_time)
+        up = _is_backend_ready(endpoint)
+        click.echo(".", nl=False)
+
+    click.echo(".")
+    return up
+
+
 def _start(attached=False, version=None):
     logger.info("Starting Giskard Server")
 
     settings = _get_settings() or {}
     port = settings.get("port", 19000)
     ml_worker_port = settings.get("ml_worker_port", 40051)
 
@@ -116,15 +143,26 @@
             get_image_name(version),
             detach=not attached,
             name=get_container_name(version),
             ports={7860: port, 40051: ml_worker_port},
             volumes={home_volume.name: {"bind": "/home/giskard/datadir", "mode": "rw"}},
         )
     container.start()
-    logger.info(f"Giskard Server {version} started. You can access it at http://localhost:{port}")
+
+    up = _wait_backend_ready(port)
+
+    if up:
+        logger.info(
+            f"Giskard Server {version} started. You can access it at http://localhost:{port}"
+        )
+    else:
+        logger.warning(
+            "Giskard backend takes unusually long time to start, "
+            "please check the logs with `giskard server logs backend`"
+        )
 
 
 def _check_downloaded(version: str):
     image = get_image_name(version)
     try:
         create_docker_client().images.get(image)
         logger.debug(f"Docker image exists: {image}")
@@ -148,21 +186,25 @@
 
 
 @retry(wait=wait_exponential(min=0.1, max=5, multiplier=0.1))
 def _fetch_latest_tag() -> str:
     """
     Returns: the latest tag from the Docker Hub API. Format: vX.Y.Z
     """
-    response = requests.get("https://hub.docker.com/v2/namespaces/giskardai/repositories/giskard/tags?page_size=10")
+    response = requests.get(
+        "https://hub.docker.com/v2/namespaces/giskardai/repositories/giskard/tags?page_size=10"
+    )
     response.raise_for_status()
     json_response = response.json()
     latest_tag = "latest"
     latest = next(i for i in json_response["results"] if i["name"] == latest_tag)
     latest_version_image = next(
-        i for i in json_response["results"] if ((i["name"] != latest_tag) and (i["digest"] == latest["digest"]))
+        i
+        for i in json_response["results"]
+        if ((i["name"] != latest_tag) and (i["digest"] == latest["digest"]))
     )
 
     tag = latest_version_image["name"]
     return tag.replace("v", "")
 
 
 def _write_settings(settings):
@@ -190,33 +232,41 @@
     return home_volume
 
 
 def _expose(token):
     container = get_container()
     if container:
         if container.status != "running":
-            print("Error: Giskard server is not running. Please start it using `giskard server start`")
+            print(
+                "Error: Giskard server is not running. Please start it using `giskard server start`"
+            )
             raise click.Abort()
     else:
         raise click.Abort()
     print("Exposing Giskard Server to the internet...")
     from pyngrok import ngrok
     from pyngrok.conf import PyngrokConfig
 
     if token:
         ngrok.set_auth_token(token)
 
-    http_tunnel = ngrok.connect(19000, "http", pyngrok_config=None if token else PyngrokConfig(region="us"))
-    tcp_tunnel = ngrok.connect(40051, "tcp", pyngrok_config=None if token else PyngrokConfig(region="eu"))
+    http_tunnel = ngrok.connect(
+        19000, "http", pyngrok_config=None if token else PyngrokConfig(region="us")
+    )
+    tcp_tunnel = ngrok.connect(
+        40051, "tcp", pyngrok_config=None if token else PyngrokConfig(region="eu")
+    )
 
     # Only split the last ':' in case the URL contains a port
     tcp_addr = urlparse(tcp_tunnel.public_url)
 
     print("Giskard Server is now exposed to the internet.")
-    print("You can now upload objects to the Giskard Server using the following client: \n")
+    print(
+        "You can now upload objects to the Giskard Server using the following client: \n"
+    )
 
     print(
         f"""token=...
 client = giskard.GiskardClient(\"{http_tunnel.public_url}\", token)
 
 # To run your model with the Giskard Server, execute these three lines on Google Colab:
 
@@ -240,15 +290,17 @@
     "--attach",
     "-a",
     "attached",
     is_flag=True,
     default=False,
     help="Starts the server and attaches to it, displaying logs in console.",
 )
-@click.option("--version", "version", required=False, help="Version of Giskard server to start")
+@click.option(
+    "--version", "version", required=False, help="Version of Giskard server to start"
+)
 @common_options
 def start(attached, version):
     """\b
     Start Giskard Server.
 
     By default, the server starts detached and will run in the background.
     You can attach to it by using -a
@@ -278,16 +330,26 @@
         container.stop()
         logger.info("Giskard Server stopped")
     else:
         logger.info(f"Giskard container {container.name} is not running")
 
 
 @server.command("restart")
-@click.argument("service", type=click.Choice(["backend", "frontend", "worker", "db"]), required=False)
-@click.option("--hard", "hard", is_flag=True, default=False, help="Hard restart. Restarts the whole container")
+@click.argument(
+    "service",
+    type=click.Choice(["backend", "frontend", "worker", "db"]),
+    required=False,
+)
+@click.option(
+    "--hard",
+    "hard",
+    is_flag=True,
+    default=False,
+    help="Hard restart. Restarts the whole container",
+)
 @common_options
 def restart(service, hard):
     """\b
     Restart Giskard Server.
 
     Stops any running Giskard server and starts it again.
     """
@@ -307,27 +369,49 @@
             logger.info(f"Restarting {container.name} container")
             container.start()
             container.stop()
             if get_container():
                 logger.info(f"Container {container.name} restarted")
         else:
             if service:
-                logger.info(f"Restarting service {service} in {container.name} container")
-                command = f"supervisorctl -c /opt/giskard/supervisord.conf restart {service}"
+                logger.info(
+                    f"Restarting service {service} in {container.name} container"
+                )
+                command = (
+                    f"supervisorctl -c /opt/giskard/supervisord.conf restart {service}"
+                )
             else:
                 logger.info(f"Restarting all services in {container.name} container")
                 command = "supervisorctl -c /opt/giskard/supervisord.conf restart all"
             for res in container.exec_run(command, stream=True).output:
                 print(res.decode())
 
 
 @server.command("logs")
-@click.argument("service", type=click.Choice(["backend", "frontend", "worker", "db"]), required=False)
-@click.option("--lines", "-l", "nb_lines", default=300, type=click.IntRange(0), help="Number of log lines to show")
-@click.option("--follow", "-f", "follow", is_flag=True, default=False, help="Follow the logs stream")
+@click.argument(
+    "service",
+    type=click.Choice(["backend", "frontend", "worker", "db"]),
+    required=False,
+)
+@click.option(
+    "--lines",
+    "-l",
+    "nb_lines",
+    default=300,
+    type=click.IntRange(0),
+    help="Number of log lines to show",
+)
+@click.option(
+    "--follow",
+    "-f",
+    "follow",
+    is_flag=True,
+    default=False,
+    help="Follow the logs stream",
+)
 @common_options
 def logs(service, nb_lines, follow):
     """\b
     Prints logs of server services
     """
     analytics.track(
         "giskard-server:logs",
@@ -367,34 +451,38 @@
 def diagnose(local_dir):
     """\b
     Save server logs to a local archive (Useful for support).
     """
     analytics.track("giskard-server:diagnose")
     out_dir = Path(local_dir)
     assert out_dir.is_dir(), "'output' should be an existing directory"
-    bits, stat = get_container().get_archive("/home/giskard/datadir/run", encode_stream=True)
+    bits, _ = get_container().get_archive(
+        "/home/giskard/datadir/run", encode_stream=True
+    )
     from datetime import datetime
 
     now = datetime.now().strftime("%Y%m%d_%H%M%S_%f")
-    out_file = out_dir / f"giskard-diagnose-{get_version().replace('.', '_')}-{now}.tar.gz"
+    out_file = (
+        out_dir / f"giskard-diagnose-{get_version().replace('.', '_')}-{now}.tar.gz"
+    )
     with open(out_file, "wb") as f:
         for chunk in bits:
             f.write(chunk)
     logger.info(f"Wrote diagnose info to {out_file}")
 
 
-@server.command("update")
+@server.command("upgrade")
 @common_options
 @click.argument("version", required=False, default=None)
-def update(version):
+def upgrade(version):
     """\b
     Update Giskard Server. Uses the latest available version if not specified.
     """
     analytics.track(
-        "giskard-server:update",
+        "giskard-server:upgrade",
         {
             "version": version,
         },
     )
     latest_version = _fetch_latest_tag()
     if not version:
         version = latest_version
@@ -403,15 +491,15 @@
     if installed_version == version:
         logger.info(f"Giskard server is already running version {version}")
         return
 
     logger.info(f"Updating Giskard Server {installed_version} -> {version}")
     _pull_image(version)
     _write_settings({**_get_settings(), **{"version": version}})
-    logger.info(f"Giskard Server updated to {version}")
+    logger.info(f"Giskard Server upgraded to {version}")
 
 
 def read_version(version_str: str) -> Version:
     try:
         return version.parse(version_str)
     except InvalidVersion:
         return version.NegativeInfinity
@@ -422,15 +510,17 @@
 def status():
     """\b
     Check if server container is running and status of each internal service
     """
     analytics.track("giskard-server:status")
     app_settings = _get_settings()
     if not app_settings:
-        logger.info("Giskard Server is not installed. Install using `giskard server start`")
+        logger.info(
+            "Giskard Server is not installed. Install using `giskard server start`"
+        )
         return
     else:
         version = app_settings["version"]
 
     logger.info(f"Giskard Server version is set to {version}")
 
     latest = _fetch_latest_tag()
@@ -438,21 +528,29 @@
     if read_version(version) < read_version(latest):
         logger.info(f"A new version is available: {latest}")
 
     container = get_container()
     if container:
         if container.status == "running":
             logger.info(f"Container {container.name} status:")
-            print(get_container().exec_run("supervisorctl -c /opt/giskard/supervisord.conf").output.decode())
+            print(
+                get_container()
+                .exec_run("supervisorctl -c /opt/giskard/supervisord.conf")
+                .output.decode()
+            )
         else:
-            logger.info(f"Container {container.name} isn't running ({container.status})")
+            logger.info(
+                f"Container {container.name} isn't running ({container.status})"
+            )
 
 
 @server.command("clean")
-@click.option("--data", "delete_data", is_flag=True, help="Delete user data (giskard-home volume)")
+@click.option(
+    "--data", "delete_data", is_flag=True, help="Delete user data (giskard-home volume)"
+)
 @common_options
 def clean(delete_data):
     """\b
     Delete Docker container, container (and possibly a volume) associated with the current version of Giskard Server
     """
     analytics.track("giskard-server:clean", {"delete_data": delete_data})
     data_deletion_confirmed = delete_data and click.confirm(
```

### Comparing `giskard-2.0.0b8/giskard/commands/cli_worker.py` & `giskard-2.0.0b9/giskard/commands/cli_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/core/core.py` & `giskard-2.0.0b9/giskard/core/core.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/core/dataset_validation.py` & `giskard-2.0.0b9/giskard/core/dataset_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/core/errors.py` & `giskard-2.0.0b9/giskard/core/errors.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/core/model_validation.py` & `giskard-2.0.0b9/giskard/core/model_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             validate_label_with_target(
                 model.meta.name, model.meta.classification_labels, target_values, validate_ds.target
             )
             validate_model_execution(model, validate_ds)
         else:  # Classification with target = None
             validate_model_execution(model, validate_ds)
 
-        if model.meta.model_type == SupportedModelTypes.CLASSIFICATION:
+        if model.meta.model_type == SupportedModelTypes.CLASSIFICATION and validate_ds.target is not None:
             validate_order_classifcation_labels(model, validate_ds)
 
 
 @configured_validate_arguments
 def validate_model_execution(model: BaseModel, dataset: Dataset, deterministic: bool = True) -> None:
     # testing multiple entries
     validation_size = min(len(dataset), 10)
```

### Comparing `giskard-2.0.0b8/giskard/core/suite.py` & `giskard-2.0.0b9/giskard/core/suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import inspect
 import logging
+import traceback
 from dataclasses import dataclass
 from typing import List, Any, Union, Dict, Mapping, Optional
 
 from giskard.client.dtos import TestSuiteDTO, TestInputDTO, SuiteTestDTO
 from giskard.client.giskard_client import GiskardClient
 from giskard.core.core import TestFunctionMeta
 from giskard.datasets.base import Dataset
 from giskard.ml_worker.core.savable import Artifact
 from giskard.ml_worker.testing.registry.giskard_test import GiskardTest, Test, GiskardTestMethod
 from giskard.ml_worker.testing.registry.registry import tests_registry
 from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
-from giskard.ml_worker.testing.test_result import TestResult
+from giskard.ml_worker.testing.test_result import TestResult, TestMessage, TestMessageLevel
 from giskard.models.base import BaseModel
 
 logger = logging.getLogger(__name__)
 
 suite_input_types: List[type] = [Dataset, BaseModel, str, bool, int, float, SlicingFunction, SlicingFunction]
 
 
@@ -220,19 +221,33 @@
         res: List[(str, Union[bool, TestResult])] = list()
         required_params = self.find_required_params()
         undefined_params = {k: v for k, v in required_params.items() if k not in suite_run_args}
         if len(undefined_params):
             raise ValueError(f"Missing {len(undefined_params)} required parameters: {undefined_params}")
 
         for test_partial in self.tests:
-            test_params = self.create_test_params(test_partial, suite_run_args)
-            result = test_partial.giskard_test.get_builder()(**test_params).execute()
-            res.append((test_partial.test_name, result))
-            if verbose:
-                print("""Executed '{0}' with arguments {1}: {2}""".format(test_partial.test_name, test_params, result))
+            try:
+                test_params = self.create_test_params(test_partial, suite_run_args)
+                result = test_partial.giskard_test.get_builder()(**test_params).execute()
+                res.append((test_partial.test_name, result))
+                if verbose:
+                    print(
+                        """Executed '{0}' with arguments {1}: {2}""".format(test_partial.test_name, test_params, result)
+                    )
+            except BaseException:  # noqa NOSONAR
+                error = traceback.format_exc()
+                logging.exception("An error happened during test execution")
+                res.append(
+                    (
+                        test_partial.test_name,
+                        TestResult(
+                            passed=False, is_error=True, messages=[TestMessage(type=TestMessageLevel.ERROR, text=error)]
+                        ),
+                    )
+                )
 
         result = single_binary_result([result for name, result in res])
 
         logger.info(f"Executed test suite '{self.name or 'unnamed'}'")
         logger.info(f"result: {'success' if result else 'failed'}")
         for test_name, r in res:
             logger.info(f"{test_name}: {format_test_result(r)}")
```

### Comparing `giskard-2.0.0b8/giskard/core/validation.py` & `giskard-2.0.0b9/giskard/core/validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/datasets/__init__.py` & `giskard-2.0.0b9/giskard/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/datasets/base/__init__.py` & `giskard-2.0.0b9/giskard/datasets/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/datasets/metadata/indexing.py` & `giskard-2.0.0b9/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/datasets/metadata/registry.py` & `giskard-2.0.0b9/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.0.0b9/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/demo/__init__.py` & `giskard-2.0.0b9/giskard/demo/titanic_classification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import os
-
-import numpy as np
 import pandas as pd
 from sklearn import model_selection
 from sklearn.compose import ColumnTransformer
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.impute import SimpleImputer
-from sklearn.linear_model import LinearRegression
 from sklearn.linear_model import LogisticRegression
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import OneHotEncoder, StandardScaler
 
 
-def titanic_df():
+def get_df():
     df = pd.read_csv(os.path.join(os.path.dirname(__file__), "titanic.csv"))
     df.drop(["Ticket", "Cabin"], axis=1, inplace=True)
     _classification_labels = {0: "no", 1: "yes"}
     df["Survived"] = df["Survived"].apply(lambda x: _classification_labels[x])
     return df
 
 
-def titanic():
-    df = titanic_df()
+def get_model_and_df():
+    df = get_df()
     cat_cols = ["Pclass", "Sex", "SibSp", "Parch", "Embarked"]
     num_cols = ["PassengerId", "Age", "Fare"]
     text_cols = ["Name"]
     target = "Survived"
 
     # tfidf the text column
     text_transformer = Pipeline([("tfidf", TfidfVectorizer(lowercase=False, strip_accents=None))])
@@ -62,46 +59,14 @@
     clf.fit(X_train, Y_train)
 
     test_data = pd.concat([X_test, Y_test], axis=1)
 
     return clf, test_data
 
 
-def titanic_pipeline():
-    clf, _ = titanic()
+def get_pipeline():
+    clf, _ = get_model_and_df()
 
     def preprocessor(df):
         return clf[0].transform(df)
 
     return preprocessor, clf[1]
-
-
-def linear_df():
-    df = pd.DataFrame({"x": np.arange(100), "y": np.arange(100)})
-    return df
-
-
-def linear():
-    df = linear_df()
-
-    reg = LinearRegression()
-    reg.fit(df["x"].to_numpy().reshape(100, 1), df["y"].to_numpy().reshape(100, 1))
-    return reg, df
-
-
-def linear_pipeline():
-    reg, _ = linear()
-
-    def preprocessor(df):
-        return df["x"].to_numpy().reshape(len(df["x"]), 1)
-
-    return preprocessor, reg
-
-
-__all__ = [
-    "titanic_df",
-    "titanic",
-    "titanic_pipeline",
-    "linear_df",
-    "linear",
-    "linear_pipeline",
-]
```

### Comparing `giskard-2.0.0b8/giskard/demo/titanic.csv` & `giskard-2.0.0b9/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.0.0b9/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/bridge/ml_worker_bridge.py` & `giskard-2.0.0b9/giskard/ml_worker/bridge/ml_worker_bridge.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/core/log_listener.py` & `giskard-2.0.0b9/giskard/ml_worker/core/log_listener.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/core/savable.py` & `giskard-2.0.0b9/giskard/ml_worker/core/savable.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/generated/ml_worker_pb2.py` & `giskard-2.0.0b9/giskard/ml_worker/generated/ml_worker_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fml-worker.proto\x12\x06worker\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1bgoogle/protobuf/empty.proto\",\n\x13MLWorkerInfoRequest\x12\x15\n\rlist_packages\x18\x01 \x01(\x08\"\xe6\x02\n\x0cMLWorkerInfo\x12&\n\x08platform\x18\x01 \x01(\x0b\x32\x14.worker.PlatformInfo\x12\x13\n\x0binterpreter\x18\x02 \x01(\t\x12\x1b\n\x13interpreter_version\x18\x03 \x01(\t\x12G\n\x12installed_packages\x18\x04 \x03(\x0b\x32+.worker.MLWorkerInfo.InstalledPackagesEntry\x12\x1d\n\x15internal_grpc_address\x18\x05 \x01(\t\x12\x11\n\tis_remote\x18\x06 \x01(\x08\x12\x0b\n\x03pid\x18\x07 \x01(\r\x12\x1a\n\x12process_start_time\x18\x08 \x01(\x04\x12\x1e\n\x16giskard_client_version\x18\t \x01(\t\x1a\x38\n\x16InstalledPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x0cPlatformInfo\x12\x0f\n\x07machine\x18\x01 \x01(\t\x12\x0c\n\x04node\x18\x02 \x01(\t\x12\x11\n\tprocessor\x18\x03 \x01(\t\x12\x0f\n\x07release\x18\x04 \x01(\t\x12\x0e\n\x06system\x18\x05 \x01(\t\x12\x0f\n\x07version\x18\x06 \x01(\t\"n\n\x11\x46ileUploadRequest\x12.\n\x08metadata\x18\x01 \x01(\x0b\x32\x1a.worker.FileUploadMetadataH\x00\x12\x1e\n\x05\x63hunk\x18\x02 \x01(\x0b\x32\r.worker.ChunkH\x00\x42\t\n\x07request\"h\n\x12\x46ileUploadMetadata\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\tfile_type\x18\x02 \x01(\x0e\x32\x10.worker.FileType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0bproject_key\x18\x04 \x01(\t\"\x16\n\x07\x45\x63hoMsg\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\xc0\x01\n\x0e\x45xplainRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x34\n\x07\x63olumns\x18\x03 \x03(\x0b\x32#.worker.ExplainRequest.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x02\n\x12\x45xplainTextRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\x12\x38\n\x07\x63olumns\x18\x03 \x03(\x0b\x32\'.worker.ExplainTextRequest.ColumnsEntry\x12\x41\n\x0c\x63olumn_types\x18\x04 \x03(\x0b\x32+.worker.ExplainTextRequest.ColumnTypesEntry\x12\x11\n\tn_samples\x18\x05 \x01(\r\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb9\x02\n\x0f\x45xplainResponse\x12?\n\x0c\x65xplanations\x18\x01 \x03(\x0b\x32).worker.ExplainResponse.ExplanationsEntry\x1a\x8a\x01\n\x0b\x45xplanation\x12H\n\x0bper_feature\x18\x01 \x03(\x0b\x32\x33.worker.ExplainResponse.Explanation.PerFeatureEntry\x1a\x31\n\x0fPerFeatureEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1aX\n\x11\x45xplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.worker.ExplainResponse.Explanation:\x02\x38\x01\"\xe4\x01\n\x13\x45xplainTextResponse\x12\r\n\x05words\x18\x01 \x03(\t\x12\x39\n\x07weights\x18\x02 \x03(\x0b\x32(.worker.ExplainTextResponse.WeightsEntry\x1a$\n\x11WeightsPerFeature\x12\x0f\n\x07weights\x18\x01 \x03(\x02\x1a]\n\x0cWeightsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12<\n\x05value\x18\x02 \x01(\x0b\x32-.worker.ExplainTextResponse.WeightsPerFeature:\x02\x38\x01\"\x8d\x01\n\x1cRunModelForDataFrameResponse\x12*\n\x0f\x61ll_predictions\x18\x01 \x01(\x0b\x32\x11.worker.DataFrame\x12\x12\n\nprediction\x18\x02 \x03(\t\x12\x15\n\rprobabilities\x18\x03 \x03(\x02\x12\x16\n\x0eraw_prediction\x18\x04 \x03(\x02\"h\n\x07\x44\x61taRow\x12-\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x1c.worker.DataRow.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"*\n\tDataFrame\x12\x1d\n\x04rows\x18\x01 \x03(\x0b\x32\x0f.worker.DataRow\"\xfa\x02\n\x1bRunModelForDataFrameRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\tdataframe\x18\x02 \x01(\x0b\x32\x11.worker.DataFrame\x12\x0e\n\x06target\x18\x03 \x01(\t\x12J\n\x0c\x63olumn_types\x18\x04 \x03(\x0b\x32\x34.worker.RunModelForDataFrameRequest.ColumnTypesEntry\x12L\n\rcolumn_dtypes\x18\x05 \x03(\x0b\x32\x35.worker.RunModelForDataFrameRequest.ColumnDtypesEntry\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x33\n\x11\x43olumnDtypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x86\x01\n\x0fRunModelRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x14\n\x0cinspectionId\x18\x03 \x01(\x04\x12\x13\n\x0bproject_key\x18\x04 \x01(\t\"?\n\x10RunModelResponse\x12\x13\n\x0bresults_csv\x18\x01 \x01(\t\x12\x16\n\x0e\x63\x61lculated_csv\x18\x02 \x01(\t\"P\n\x13RunAdHocTestRequest\x12\x10\n\x08testUuid\x18\x01 \x01(\t\x12\'\n\targuments\x18\x02 \x03(\x0b\x32\x14.worker.FuncArgument\"v\n\x18\x44\x61tasetProcessingRequest\x12$\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x34\n\tfunctions\x18\x02 \x03(\x0b\x32!.worker.DatasetProcessingFunction\"\xb7\x01\n\x19\x44\x61tasetProcessingFunction\x12.\n\x0fslicingFunction\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x35\n\x16transformationFunction\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\'\n\targuments\x18\x03 \x03(\x0b\x32\x14.worker.FuncArgumentB\n\n\x08\x66unction\"Z\n\x11SuiteTestArgument\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08testUuid\x18\x02 \x01(\t\x12\'\n\targuments\x18\x03 \x03(\x0b\x32\x14.worker.FuncArgument\"n\n\x13RunTestSuiteRequest\x12(\n\x05tests\x18\x01 \x03(\x0b\x32\x19.worker.SuiteTestArgument\x12-\n\x0fglobalArguments\x18\x02 \x03(\x0b\x32\x14.worker.FuncArgument\"\xe0\x02\n\x0c\x46uncArgument\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05model\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12&\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x0f\n\x05\x66loat\x18\x04 \x01(\x02H\x00\x12\r\n\x03int\x18\x05 \x01(\x05H\x00\x12\r\n\x03str\x18\x06 \x01(\tH\x00\x12\x0e\n\x04\x62ool\x18\x07 \x01(\x08H\x00\x12.\n\x0fslicingFunction\x18\x08 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x35\n\x16transformationFunction\x18\t \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x10\n\x06kwargs\x18\n \x01(\tH\x00\x12\"\n\x04\x61rgs\x18\x0b \x03(\x0b\x32\x14.worker.FuncArgument\x12\x0c\n\x04none\x18\x0c \x01(\x08\x42\n\n\x08\x61rgument\"\x1f\n\x0fRunTestResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\"9\n\x19Partial_unexpected_counts\x12\r\n\x05value\x18\x01 \x03(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"S\n\x15NamedSingleTestResult\x12\x10\n\x08testUuid\x18\x01 \x01(\t\x12(\n\x06result\x18\x02 \x01(\x0b\x32\x18.worker.SingleTestResult\"R\n\x1aIdentifierSingleTestResult\x12\n\n\x02id\x18\x01 \x01(\x03\x12(\n\x06result\x18\x02 \x01(\x0b\x32\x18.worker.SingleTestResult\"B\n\x0bTestMessage\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.worker.TestMessageType\x12\x0c\n\x04text\x18\x02 \x01(\t\"\xe6\x04\n\x10SingleTestResult\x12\x0e\n\x06passed\x18\r \x01(\x08\x12%\n\x08messages\x18\x10 \x03(\x0b\x32\x13.worker.TestMessage\x12\x32\n\x05props\x18\x0e \x03(\x0b\x32#.worker.SingleTestResult.PropsEntry\x12\x0e\n\x06metric\x18\x0f \x01(\x02\x12\x15\n\rmissing_count\x18\x02 \x01(\x05\x12\x17\n\x0fmissing_percent\x18\x03 \x01(\x01\x12\x18\n\x10unexpected_count\x18\x04 \x01(\x05\x12\x1a\n\x12unexpected_percent\x18\x05 \x01(\x01\x12 \n\x18unexpected_percent_total\x18\x06 \x01(\x01\x12%\n\x1dunexpected_percent_nonmissing\x18\x07 \x01(\x01\x12%\n\x1dpartial_unexpected_index_list\x18\t \x03(\r\x12\x44\n\x19partial_unexpected_counts\x18\n \x03(\x0b\x32!.worker.Partial_unexpected_counts\x12\x1d\n\x15unexpected_index_list\x18\x0c \x03(\r\x12\x11\n\toutput_df\x18\x12 \x01(\x0c\x12 \n\x18number_of_perturbed_rows\x18\x14 \x01(\r\x12\x1a\n\x12\x61\x63tual_slices_size\x18\x15 \x03(\r\x12\x1d\n\x15reference_slices_size\x18\x16 \x03(\r\x1a,\n\nPropsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"C\n\x11TestResultMessage\x12.\n\x07results\x18\x01 \x03(\x0b\x32\x1d.worker.NamedSingleTestResult\"\x99\x01\n\x1e\x44\x61tasetProcessingResultMessage\x12\x11\n\tdatasetId\x18\x01 \x01(\t\x12\x11\n\ttotalRows\x18\x02 \x01(\r\x12\x14\n\x0c\x66ilteredRows\x18\x03 \x03(\r\x12;\n\rmodifications\x18\x04 \x03(\x0b\x32$.worker.DatasetRowModificationResult\"\xb3\x01\n\x1c\x44\x61tasetRowModificationResult\x12\r\n\x05rowId\x18\x01 \x01(\r\x12N\n\rmodifications\x18\x02 \x03(\x0b\x32\x37.worker.DatasetRowModificationResult.ModificationsEntry\x1a\x34\n\x12ModificationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x16TestSuiteResultMessage\x12\x10\n\x08is_error\x18\x01 \x01(\x08\x12\x0f\n\x07is_pass\x18\x02 \x01(\x08\x12\x33\n\x07results\x18\x03 \x03(\x0b\x32\".worker.IdentifierSingleTestResult\x12\x0c\n\x04logs\x18\x04 \x01(\t\"N\n\x0b\x41rtifactRef\x12\x13\n\x0bproject_key\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\x12\x13\n\x06sample\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\t\n\x07_sample\"\x18\n\x05\x43hunk\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c\"0\n\x0cUploadStatus\x12 \n\x04\x63ode\x18\x01 \x01(\x0e\x32\x12.worker.StatusCode\"1\n\x11MLWorkerErrorInfo\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\r\n\x05stack\x18\x02 \x01(\t\"\xa4\x01\n\nSuiteInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12*\n\nmodel_meta\x18\x03 \x01(\x0b\x32\x11.worker.ModelMetaH\x00\x88\x01\x01\x12.\n\x0c\x64\x61taset_meta\x18\x04 \x01(\x0b\x32\x13.worker.DatasetMetaH\x01\x88\x01\x01\x42\r\n\x0b_model_metaB\x0f\n\r_dataset_meta\"3\n\tModelMeta\x12\x17\n\nmodel_type\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_model_type\"-\n\x0b\x44\x61tasetMeta\x12\x13\n\x06target\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\t\n\x07_target\"S\n\x18GenerateTestSuiteRequest\x12\x13\n\x0bproject_key\x18\x01 \x01(\t\x12\"\n\x06inputs\x18\x02 \x03(\x0b\x32\x12.worker.SuiteInput\"A\n\x19GenerateTestSuiteResponse\x12$\n\x05tests\x18\x01 \x03(\x0b\x32\x15.worker.GeneratedTest\"N\n\rGeneratedTest\x12\x11\n\ttest_uuid\x18\x01 \x01(\t\x12*\n\x06inputs\x18\x02 \x03(\x0b\x32\x1a.worker.GeneratedTestInput\"C\n\x12GeneratedTestInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08is_alias\x18\x03 \x01(\x08\"\xb3\x03\n\x0f\x43\x61talogResponse\x12\x31\n\x05tests\x18\x01 \x03(\x0b\x32\".worker.CatalogResponse.TestsEntry\x12\x33\n\x06slices\x18\x02 \x03(\x0b\x32#.worker.CatalogResponse.SlicesEntry\x12\x45\n\x0ftransformations\x18\x03 \x03(\x0b\x32,.worker.CatalogResponse.TransformationsEntry\x1a\x42\n\nTestsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.worker.FunctionMeta:\x02\x38\x01\x1aQ\n\x0bSlicesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".worker.DatasetProcessFunctionMeta:\x02\x38\x01\x1aZ\n\x14TransformationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".worker.DatasetProcessFunctionMeta:\x02\x38\x01\"\xd6\x01\n\x0c\x46unctionMeta\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x0e\n\x06module\x18\x05 \x01(\t\x12\x0b\n\x03\x64oc\x18\x06 \x01(\t\x12\x11\n\tmoduleDoc\x18\x07 \x01(\t\x12*\n\x04\x61rgs\x18\x08 \x03(\x0b\x32\x1c.worker.TestFunctionArgument\x12\x0c\n\x04tags\x18\t \x03(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\"\xb4\x02\n\x1a\x44\x61tasetProcessFunctionMeta\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x0e\n\x06module\x18\x05 \x01(\t\x12\x0b\n\x03\x64oc\x18\x06 \x01(\t\x12\x11\n\tmoduleDoc\x18\x07 \x01(\t\x12*\n\x04\x61rgs\x18\x08 \x03(\x0b\x32\x1c.worker.TestFunctionArgument\x12\x0c\n\x04tags\x18\t \x03(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x11\n\tcellLevel\x18\x0c \x01(\x08\x12\x17\n\ncolumnType\x18\r \x01(\tH\x00\x88\x01\x01\x12\x13\n\x0bprocessType\x18\x0e \x01(\tB\r\n\x0b_columnType\"g\n\x14TestFunctionArgument\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08optional\x18\x03 \x01(\x08\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x04 \x01(\t\x12\x10\n\x08\x61rgOrder\x18\x05 \x01(\r\"\x8c\x01\n\x10\x43omparisonClause\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12/\n\x0f\x63omparison_type\x18\x02 \x01(\x0e\x32\x16.worker.ComparisonType\x12\x14\n\x0c\x63olumn_dtype\x18\x03 \x01(\t\x12\x12\n\x05value\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_value\"V\n\x1eGenerateQueryBasedSliceRequest\x12\x34\n\x12\x63omparison_clauses\x18\x01 \x03(\x0b\x32\x18.worker.ComparisonClause\"-\n\x1fGenerateQueryBasedSliceResponse\x12\n\n\x02id\x18\x01 \x01(\t*\"\n\x08\x46ileType\x12\t\n\x05MODEL\x10\x00\x12\x0b\n\x07\x44\x41TASET\x10\x01*&\n\x0fTestMessageType\x12\t\n\x05\x45RROR\x10\x00\x12\x08\n\x04INFO\x10\x01*Q\n\nStatusCode\x12\x0b\n\x07Unknown\x10\x00\x12\x06\n\x02Ok\x10\x01\x12\n\n\x06\x46\x61iled\x10\x02\x12\r\n\tCacheMiss\x10\x03\x12\t\n\x05Ready\x10\x04\x12\x08\n\x04Next\x10\x05*\x89\x01\n\x0e\x43omparisonType\x12\x06\n\x02IS\x10\x00\x12\n\n\x06IS_NOT\x10\x01\x12\x0c\n\x08\x43ONTAINS\x10\x02\x12\x15\n\x11\x44OES_NOT_CONTAINS\x10\x03\x12\x0f\n\x0bSTARTS_WITH\x10\x04\x12\r\n\tENDS_WITH\x10\x05\x12\x0c\n\x08IS_EMPTY\x10\x06\x12\x10\n\x0cIS_NOT_EMPTY\x10\x07\x32\xf1\x07\n\x08MLWorker\x12>\n\x07getInfo\x12\x1b.worker.MLWorkerInfoRequest\x1a\x14.worker.MLWorkerInfo\"\x00\x12H\n\x0crunAdHocTest\x12\x1b.worker.RunAdHocTestRequest\x1a\x19.worker.TestResultMessage\"\x00\x12_\n\x11\x64\x61tasetProcessing\x12 .worker.DatasetProcessingRequest\x1a&.worker.DatasetProcessingResultMessage\"\x00\x12M\n\x0crunTestSuite\x12\x1b.worker.RunTestSuiteRequest\x1a\x1e.worker.TestSuiteResultMessage\"\x00\x12=\n\x08runModel\x12\x17.worker.RunModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x63\n\x14runModelForDataFrame\x12#.worker.RunModelForDataFrameRequest\x1a$.worker.RunModelForDataFrameResponse\"\x00\x12<\n\x07\x65xplain\x12\x16.worker.ExplainRequest\x1a\x17.worker.ExplainResponse\"\x00\x12H\n\x0b\x65xplainText\x12\x1a.worker.ExplainTextRequest\x1a\x1b.worker.ExplainTextResponse\"\x00\x12*\n\x04\x65\x63ho\x12\x0f.worker.EchoMsg\x1a\x0f.worker.EchoMsg\"\x00\x12Z\n\x11generateTestSuite\x12 .worker.GenerateTestSuiteRequest\x1a!.worker.GenerateTestSuiteResponse\"\x00\x12>\n\nstopWorker\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\ngetCatalog\x12\x16.google.protobuf.Empty\x1a\x17.worker.CatalogResponse\"\x00\x12v\n!generateQueryBasedSlicingFunction\x12&.worker.GenerateQueryBasedSliceRequest\x1a\'.worker.GenerateQueryBasedSliceResponse\"\x00\x42(\n\x11\x61i.giskard.workerB\x0bWorkerProtoP\x01\xa2\x02\x03WRKb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fml-worker.proto\x12\x06worker\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1bgoogle/protobuf/empty.proto\",\n\x13MLWorkerInfoRequest\x12\x15\n\rlist_packages\x18\x01 \x01(\x08\"\xe6\x02\n\x0cMLWorkerInfo\x12&\n\x08platform\x18\x01 \x01(\x0b\x32\x14.worker.PlatformInfo\x12\x13\n\x0binterpreter\x18\x02 \x01(\t\x12\x1b\n\x13interpreter_version\x18\x03 \x01(\t\x12G\n\x12installed_packages\x18\x04 \x03(\x0b\x32+.worker.MLWorkerInfo.InstalledPackagesEntry\x12\x1d\n\x15internal_grpc_address\x18\x05 \x01(\t\x12\x11\n\tis_remote\x18\x06 \x01(\x08\x12\x0b\n\x03pid\x18\x07 \x01(\r\x12\x1a\n\x12process_start_time\x18\x08 \x01(\x04\x12\x1e\n\x16giskard_client_version\x18\t \x01(\t\x1a\x38\n\x16InstalledPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x0cPlatformInfo\x12\x0f\n\x07machine\x18\x01 \x01(\t\x12\x0c\n\x04node\x18\x02 \x01(\t\x12\x11\n\tprocessor\x18\x03 \x01(\t\x12\x0f\n\x07release\x18\x04 \x01(\t\x12\x0e\n\x06system\x18\x05 \x01(\t\x12\x0f\n\x07version\x18\x06 \x01(\t\"n\n\x11\x46ileUploadRequest\x12.\n\x08metadata\x18\x01 \x01(\x0b\x32\x1a.worker.FileUploadMetadataH\x00\x12\x1e\n\x05\x63hunk\x18\x02 \x01(\x0b\x32\r.worker.ChunkH\x00\x42\t\n\x07request\"h\n\x12\x46ileUploadMetadata\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\tfile_type\x18\x02 \x01(\x0e\x32\x10.worker.FileType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0bproject_key\x18\x04 \x01(\t\"\x16\n\x07\x45\x63hoMsg\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\xc0\x01\n\x0e\x45xplainRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x34\n\x07\x63olumns\x18\x03 \x03(\x0b\x32#.worker.ExplainRequest.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x02\n\x12\x45xplainTextRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\x12\x38\n\x07\x63olumns\x18\x03 \x03(\x0b\x32\'.worker.ExplainTextRequest.ColumnsEntry\x12\x41\n\x0c\x63olumn_types\x18\x04 \x03(\x0b\x32+.worker.ExplainTextRequest.ColumnTypesEntry\x12\x11\n\tn_samples\x18\x05 \x01(\r\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb9\x02\n\x0f\x45xplainResponse\x12?\n\x0c\x65xplanations\x18\x01 \x03(\x0b\x32).worker.ExplainResponse.ExplanationsEntry\x1a\x8a\x01\n\x0b\x45xplanation\x12H\n\x0bper_feature\x18\x01 \x03(\x0b\x32\x33.worker.ExplainResponse.Explanation.PerFeatureEntry\x1a\x31\n\x0fPerFeatureEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1aX\n\x11\x45xplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.worker.ExplainResponse.Explanation:\x02\x38\x01\"\xe4\x01\n\x13\x45xplainTextResponse\x12\r\n\x05words\x18\x01 \x03(\t\x12\x39\n\x07weights\x18\x02 \x03(\x0b\x32(.worker.ExplainTextResponse.WeightsEntry\x1a$\n\x11WeightsPerFeature\x12\x0f\n\x07weights\x18\x01 \x03(\x02\x1a]\n\x0cWeightsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12<\n\x05value\x18\x02 \x01(\x0b\x32-.worker.ExplainTextResponse.WeightsPerFeature:\x02\x38\x01\"\x8d\x01\n\x1cRunModelForDataFrameResponse\x12*\n\x0f\x61ll_predictions\x18\x01 \x01(\x0b\x32\x11.worker.DataFrame\x12\x12\n\nprediction\x18\x02 \x03(\t\x12\x15\n\rprobabilities\x18\x03 \x03(\x02\x12\x16\n\x0eraw_prediction\x18\x04 \x03(\x02\"h\n\x07\x44\x61taRow\x12-\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x1c.worker.DataRow.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"*\n\tDataFrame\x12\x1d\n\x04rows\x18\x01 \x03(\x0b\x32\x0f.worker.DataRow\"\xfa\x02\n\x1bRunModelForDataFrameRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\tdataframe\x18\x02 \x01(\x0b\x32\x11.worker.DataFrame\x12\x0e\n\x06target\x18\x03 \x01(\t\x12J\n\x0c\x63olumn_types\x18\x04 \x03(\x0b\x32\x34.worker.RunModelForDataFrameRequest.ColumnTypesEntry\x12L\n\rcolumn_dtypes\x18\x05 \x03(\x0b\x32\x35.worker.RunModelForDataFrameRequest.ColumnDtypesEntry\x1a\x32\n\x10\x43olumnTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x33\n\x11\x43olumnDtypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x86\x01\n\x0fRunModelRequest\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12$\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x14\n\x0cinspectionId\x18\x03 \x01(\x04\x12\x13\n\x0bproject_key\x18\x04 \x01(\t\"?\n\x10RunModelResponse\x12\x13\n\x0bresults_csv\x18\x01 \x01(\t\x12\x16\n\x0e\x63\x61lculated_csv\x18\x02 \x01(\t\"P\n\x13RunAdHocTestRequest\x12\x10\n\x08testUuid\x18\x01 \x01(\t\x12\'\n\targuments\x18\x02 \x03(\x0b\x32\x14.worker.FuncArgument\"v\n\x18\x44\x61tasetProcessingRequest\x12$\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRef\x12\x34\n\tfunctions\x18\x02 \x03(\x0b\x32!.worker.DatasetProcessingFunction\"\xb7\x01\n\x19\x44\x61tasetProcessingFunction\x12.\n\x0fslicingFunction\x18\x01 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x35\n\x16transformationFunction\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\'\n\targuments\x18\x03 \x03(\x0b\x32\x14.worker.FuncArgumentB\n\n\x08\x66unction\"Z\n\x11SuiteTestArgument\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08testUuid\x18\x02 \x01(\t\x12\'\n\targuments\x18\x03 \x03(\x0b\x32\x14.worker.FuncArgument\"n\n\x13RunTestSuiteRequest\x12(\n\x05tests\x18\x01 \x03(\x0b\x32\x19.worker.SuiteTestArgument\x12-\n\x0fglobalArguments\x18\x02 \x03(\x0b\x32\x14.worker.FuncArgument\"\xe0\x02\n\x0c\x46uncArgument\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05model\x18\x02 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12&\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x0f\n\x05\x66loat\x18\x04 \x01(\x02H\x00\x12\r\n\x03int\x18\x05 \x01(\x05H\x00\x12\r\n\x03str\x18\x06 \x01(\tH\x00\x12\x0e\n\x04\x62ool\x18\x07 \x01(\x08H\x00\x12.\n\x0fslicingFunction\x18\x08 \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x35\n\x16transformationFunction\x18\t \x01(\x0b\x32\x13.worker.ArtifactRefH\x00\x12\x10\n\x06kwargs\x18\n \x01(\tH\x00\x12\"\n\x04\x61rgs\x18\x0b \x03(\x0b\x32\x14.worker.FuncArgument\x12\x0c\n\x04none\x18\x0c \x01(\x08\x42\n\n\x08\x61rgument\"\x1f\n\x0fRunTestResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\"9\n\x19Partial_unexpected_counts\x12\r\n\x05value\x18\x01 \x03(\r\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"S\n\x15NamedSingleTestResult\x12\x10\n\x08testUuid\x18\x01 \x01(\t\x12(\n\x06result\x18\x02 \x01(\x0b\x32\x18.worker.SingleTestResult\"R\n\x1aIdentifierSingleTestResult\x12\n\n\x02id\x18\x01 \x01(\x03\x12(\n\x06result\x18\x02 \x01(\x0b\x32\x18.worker.SingleTestResult\"B\n\x0bTestMessage\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.worker.TestMessageType\x12\x0c\n\x04text\x18\x02 \x01(\t\"\xf8\x04\n\x10SingleTestResult\x12\x0e\n\x06passed\x18\r \x01(\x08\x12\x10\n\x08is_error\x18\x17 \x01(\x08\x12%\n\x08messages\x18\x10 \x03(\x0b\x32\x13.worker.TestMessage\x12\x32\n\x05props\x18\x0e \x03(\x0b\x32#.worker.SingleTestResult.PropsEntry\x12\x0e\n\x06metric\x18\x0f \x01(\x02\x12\x15\n\rmissing_count\x18\x02 \x01(\x05\x12\x17\n\x0fmissing_percent\x18\x03 \x01(\x01\x12\x18\n\x10unexpected_count\x18\x04 \x01(\x05\x12\x1a\n\x12unexpected_percent\x18\x05 \x01(\x01\x12 \n\x18unexpected_percent_total\x18\x06 \x01(\x01\x12%\n\x1dunexpected_percent_nonmissing\x18\x07 \x01(\x01\x12%\n\x1dpartial_unexpected_index_list\x18\t \x03(\r\x12\x44\n\x19partial_unexpected_counts\x18\n \x03(\x0b\x32!.worker.Partial_unexpected_counts\x12\x1d\n\x15unexpected_index_list\x18\x0c \x03(\r\x12\x11\n\toutput_df\x18\x12 \x01(\x0c\x12 \n\x18number_of_perturbed_rows\x18\x14 \x01(\r\x12\x1a\n\x12\x61\x63tual_slices_size\x18\x15 \x03(\r\x12\x1d\n\x15reference_slices_size\x18\x16 \x03(\r\x1a,\n\nPropsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"C\n\x11TestResultMessage\x12.\n\x07results\x18\x01 \x03(\x0b\x32\x1d.worker.NamedSingleTestResult\"\x99\x01\n\x1e\x44\x61tasetProcessingResultMessage\x12\x11\n\tdatasetId\x18\x01 \x01(\t\x12\x11\n\ttotalRows\x18\x02 \x01(\r\x12\x14\n\x0c\x66ilteredRows\x18\x03 \x03(\r\x12;\n\rmodifications\x18\x04 \x03(\x0b\x32$.worker.DatasetRowModificationResult\"\xb3\x01\n\x1c\x44\x61tasetRowModificationResult\x12\r\n\x05rowId\x18\x01 \x01(\r\x12N\n\rmodifications\x18\x02 \x03(\x0b\x32\x37.worker.DatasetRowModificationResult.ModificationsEntry\x1a\x34\n\x12ModificationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x16TestSuiteResultMessage\x12\x10\n\x08is_error\x18\x01 \x01(\x08\x12\x0f\n\x07is_pass\x18\x02 \x01(\x08\x12\x33\n\x07results\x18\x03 \x03(\x0b\x32\".worker.IdentifierSingleTestResult\x12\x0c\n\x04logs\x18\x04 \x01(\t\"N\n\x0b\x41rtifactRef\x12\x13\n\x0bproject_key\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\x12\x13\n\x06sample\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\t\n\x07_sample\"\x18\n\x05\x43hunk\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c\"0\n\x0cUploadStatus\x12 \n\x04\x63ode\x18\x01 \x01(\x0e\x32\x12.worker.StatusCode\"1\n\x11MLWorkerErrorInfo\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\r\n\x05stack\x18\x02 \x01(\t\"\xa4\x01\n\nSuiteInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12*\n\nmodel_meta\x18\x03 \x01(\x0b\x32\x11.worker.ModelMetaH\x00\x88\x01\x01\x12.\n\x0c\x64\x61taset_meta\x18\x04 \x01(\x0b\x32\x13.worker.DatasetMetaH\x01\x88\x01\x01\x42\r\n\x0b_model_metaB\x0f\n\r_dataset_meta\"3\n\tModelMeta\x12\x17\n\nmodel_type\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_model_type\"-\n\x0b\x44\x61tasetMeta\x12\x13\n\x06target\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\t\n\x07_target\"S\n\x18GenerateTestSuiteRequest\x12\x13\n\x0bproject_key\x18\x01 \x01(\t\x12\"\n\x06inputs\x18\x02 \x03(\x0b\x32\x12.worker.SuiteInput\"A\n\x19GenerateTestSuiteResponse\x12$\n\x05tests\x18\x01 \x03(\x0b\x32\x15.worker.GeneratedTest\"N\n\rGeneratedTest\x12\x11\n\ttest_uuid\x18\x01 \x01(\t\x12*\n\x06inputs\x18\x02 \x03(\x0b\x32\x1a.worker.GeneratedTestInput\"C\n\x12GeneratedTestInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08is_alias\x18\x03 \x01(\x08\"\xb3\x03\n\x0f\x43\x61talogResponse\x12\x31\n\x05tests\x18\x01 \x03(\x0b\x32\".worker.CatalogResponse.TestsEntry\x12\x33\n\x06slices\x18\x02 \x03(\x0b\x32#.worker.CatalogResponse.SlicesEntry\x12\x45\n\x0ftransformations\x18\x03 \x03(\x0b\x32,.worker.CatalogResponse.TransformationsEntry\x1a\x42\n\nTestsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.worker.FunctionMeta:\x02\x38\x01\x1aQ\n\x0bSlicesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".worker.DatasetProcessFunctionMeta:\x02\x38\x01\x1aZ\n\x14TransformationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".worker.DatasetProcessFunctionMeta:\x02\x38\x01\"\xd6\x01\n\x0c\x46unctionMeta\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x0e\n\x06module\x18\x05 \x01(\t\x12\x0b\n\x03\x64oc\x18\x06 \x01(\t\x12\x11\n\tmoduleDoc\x18\x07 \x01(\t\x12*\n\x04\x61rgs\x18\x08 \x03(\x0b\x32\x1c.worker.TestFunctionArgument\x12\x0c\n\x04tags\x18\t \x03(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\"\xb4\x02\n\x1a\x44\x61tasetProcessFunctionMeta\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x0e\n\x06module\x18\x05 \x01(\t\x12\x0b\n\x03\x64oc\x18\x06 \x01(\t\x12\x11\n\tmoduleDoc\x18\x07 \x01(\t\x12*\n\x04\x61rgs\x18\x08 \x03(\x0b\x32\x1c.worker.TestFunctionArgument\x12\x0c\n\x04tags\x18\t \x03(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x11\n\tcellLevel\x18\x0c \x01(\x08\x12\x17\n\ncolumnType\x18\r \x01(\tH\x00\x88\x01\x01\x12\x13\n\x0bprocessType\x18\x0e \x01(\tB\r\n\x0b_columnType\"g\n\x14TestFunctionArgument\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08optional\x18\x03 \x01(\x08\x12\x0f\n\x07\x64\x65\x66\x61ult\x18\x04 \x01(\t\x12\x10\n\x08\x61rgOrder\x18\x05 \x01(\r\"\x8c\x01\n\x10\x43omparisonClause\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12/\n\x0f\x63omparison_type\x18\x02 \x01(\x0e\x32\x16.worker.ComparisonType\x12\x14\n\x0c\x63olumn_dtype\x18\x03 \x01(\t\x12\x12\n\x05value\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_value\"V\n\x1eGenerateQueryBasedSliceRequest\x12\x34\n\x12\x63omparison_clauses\x18\x01 \x03(\x0b\x32\x18.worker.ComparisonClause\"-\n\x1fGenerateQueryBasedSliceResponse\x12\n\n\x02id\x18\x01 \x01(\t*\"\n\x08\x46ileType\x12\t\n\x05MODEL\x10\x00\x12\x0b\n\x07\x44\x41TASET\x10\x01*&\n\x0fTestMessageType\x12\t\n\x05\x45RROR\x10\x00\x12\x08\n\x04INFO\x10\x01*Q\n\nStatusCode\x12\x0b\n\x07Unknown\x10\x00\x12\x06\n\x02Ok\x10\x01\x12\n\n\x06\x46\x61iled\x10\x02\x12\r\n\tCacheMiss\x10\x03\x12\t\n\x05Ready\x10\x04\x12\x08\n\x04Next\x10\x05*\x89\x01\n\x0e\x43omparisonType\x12\x06\n\x02IS\x10\x00\x12\n\n\x06IS_NOT\x10\x01\x12\x0c\n\x08\x43ONTAINS\x10\x02\x12\x15\n\x11\x44OES_NOT_CONTAINS\x10\x03\x12\x0f\n\x0bSTARTS_WITH\x10\x04\x12\r\n\tENDS_WITH\x10\x05\x12\x0c\n\x08IS_EMPTY\x10\x06\x12\x10\n\x0cIS_NOT_EMPTY\x10\x07\x32\xf1\x07\n\x08MLWorker\x12>\n\x07getInfo\x12\x1b.worker.MLWorkerInfoRequest\x1a\x14.worker.MLWorkerInfo\"\x00\x12H\n\x0crunAdHocTest\x12\x1b.worker.RunAdHocTestRequest\x1a\x19.worker.TestResultMessage\"\x00\x12_\n\x11\x64\x61tasetProcessing\x12 .worker.DatasetProcessingRequest\x1a&.worker.DatasetProcessingResultMessage\"\x00\x12M\n\x0crunTestSuite\x12\x1b.worker.RunTestSuiteRequest\x1a\x1e.worker.TestSuiteResultMessage\"\x00\x12=\n\x08runModel\x12\x17.worker.RunModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x63\n\x14runModelForDataFrame\x12#.worker.RunModelForDataFrameRequest\x1a$.worker.RunModelForDataFrameResponse\"\x00\x12<\n\x07\x65xplain\x12\x16.worker.ExplainRequest\x1a\x17.worker.ExplainResponse\"\x00\x12H\n\x0b\x65xplainText\x12\x1a.worker.ExplainTextRequest\x1a\x1b.worker.ExplainTextResponse\"\x00\x12*\n\x04\x65\x63ho\x12\x0f.worker.EchoMsg\x1a\x0f.worker.EchoMsg\"\x00\x12Z\n\x11generateTestSuite\x12 .worker.GenerateTestSuiteRequest\x1a!.worker.GenerateTestSuiteResponse\"\x00\x12>\n\nstopWorker\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\ngetCatalog\x12\x16.google.protobuf.Empty\x1a\x17.worker.CatalogResponse\"\x00\x12v\n!generateQueryBasedSlicingFunction\x12&.worker.GenerateQueryBasedSliceRequest\x1a\'.worker.GenerateQueryBasedSliceResponse\"\x00\x42(\n\x11\x61i.giskard.workerB\x0bWorkerProtoP\x01\xa2\x02\x03WRKb\x06proto3')
 
 _FILETYPE = DESCRIPTOR.enum_types_by_name['FileType']
 FileType = enum_type_wrapper.EnumTypeWrapper(_FILETYPE)
 _TESTMESSAGETYPE = DESCRIPTOR.enum_types_by_name['TestMessageType']
 TestMessageType = enum_type_wrapper.EnumTypeWrapper(_TESTMESSAGETYPE)
 _STATUSCODE = DESCRIPTOR.enum_types_by_name['StatusCode']
 StatusCode = enum_type_wrapper.EnumTypeWrapper(_STATUSCODE)
@@ -632,22 +632,22 @@
   _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._serialized_options = b'8\001'
   _CATALOGRESPONSE_TESTSENTRY._options = None
   _CATALOGRESPONSE_TESTSENTRY._serialized_options = b'8\001'
   _CATALOGRESPONSE_SLICESENTRY._options = None
   _CATALOGRESPONSE_SLICESENTRY._serialized_options = b'8\001'
   _CATALOGRESPONSE_TRANSFORMATIONSENTRY._options = None
   _CATALOGRESPONSE_TRANSFORMATIONSENTRY._serialized_options = b'8\001'
-  _FILETYPE._serialized_start=7376
-  _FILETYPE._serialized_end=7410
-  _TESTMESSAGETYPE._serialized_start=7412
-  _TESTMESSAGETYPE._serialized_end=7450
-  _STATUSCODE._serialized_start=7452
-  _STATUSCODE._serialized_end=7533
-  _COMPARISONTYPE._serialized_start=7536
-  _COMPARISONTYPE._serialized_end=7673
+  _FILETYPE._serialized_start=7394
+  _FILETYPE._serialized_end=7428
+  _TESTMESSAGETYPE._serialized_start=7430
+  _TESTMESSAGETYPE._serialized_end=7468
+  _STATUSCODE._serialized_start=7470
+  _STATUSCODE._serialized_end=7551
+  _COMPARISONTYPE._serialized_start=7554
+  _COMPARISONTYPE._serialized_end=7691
   _MLWORKERINFOREQUEST._serialized_start=115
   _MLWORKERINFOREQUEST._serialized_end=159
   _MLWORKERINFO._serialized_start=162
   _MLWORKERINFO._serialized_end=520
   _MLWORKERINFO_INSTALLEDPACKAGESENTRY._serialized_start=464
   _MLWORKERINFO_INSTALLEDPACKAGESENTRY._serialized_end=520
   _PLATFORMINFO._serialized_start=522
@@ -719,65 +719,65 @@
   _NAMEDSINGLETESTRESULT._serialized_start=3863
   _NAMEDSINGLETESTRESULT._serialized_end=3946
   _IDENTIFIERSINGLETESTRESULT._serialized_start=3948
   _IDENTIFIERSINGLETESTRESULT._serialized_end=4030
   _TESTMESSAGE._serialized_start=4032
   _TESTMESSAGE._serialized_end=4098
   _SINGLETESTRESULT._serialized_start=4101
-  _SINGLETESTRESULT._serialized_end=4715
-  _SINGLETESTRESULT_PROPSENTRY._serialized_start=4671
-  _SINGLETESTRESULT_PROPSENTRY._serialized_end=4715
-  _TESTRESULTMESSAGE._serialized_start=4717
-  _TESTRESULTMESSAGE._serialized_end=4784
-  _DATASETPROCESSINGRESULTMESSAGE._serialized_start=4787
-  _DATASETPROCESSINGRESULTMESSAGE._serialized_end=4940
-  _DATASETROWMODIFICATIONRESULT._serialized_start=4943
-  _DATASETROWMODIFICATIONRESULT._serialized_end=5122
-  _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._serialized_start=5070
-  _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._serialized_end=5122
-  _TESTSUITERESULTMESSAGE._serialized_start=5124
-  _TESTSUITERESULTMESSAGE._serialized_end=5250
-  _ARTIFACTREF._serialized_start=5252
-  _ARTIFACTREF._serialized_end=5330
-  _CHUNK._serialized_start=5332
-  _CHUNK._serialized_end=5356
-  _UPLOADSTATUS._serialized_start=5358
-  _UPLOADSTATUS._serialized_end=5406
-  _MLWORKERERRORINFO._serialized_start=5408
-  _MLWORKERERRORINFO._serialized_end=5457
-  _SUITEINPUT._serialized_start=5460
-  _SUITEINPUT._serialized_end=5624
-  _MODELMETA._serialized_start=5626
-  _MODELMETA._serialized_end=5677
-  _DATASETMETA._serialized_start=5679
-  _DATASETMETA._serialized_end=5724
-  _GENERATETESTSUITEREQUEST._serialized_start=5726
-  _GENERATETESTSUITEREQUEST._serialized_end=5809
-  _GENERATETESTSUITERESPONSE._serialized_start=5811
-  _GENERATETESTSUITERESPONSE._serialized_end=5876
-  _GENERATEDTEST._serialized_start=5878
-  _GENERATEDTEST._serialized_end=5956
-  _GENERATEDTESTINPUT._serialized_start=5958
-  _GENERATEDTESTINPUT._serialized_end=6025
-  _CATALOGRESPONSE._serialized_start=6028
-  _CATALOGRESPONSE._serialized_end=6463
-  _CATALOGRESPONSE_TESTSENTRY._serialized_start=6222
-  _CATALOGRESPONSE_TESTSENTRY._serialized_end=6288
-  _CATALOGRESPONSE_SLICESENTRY._serialized_start=6290
-  _CATALOGRESPONSE_SLICESENTRY._serialized_end=6371
-  _CATALOGRESPONSE_TRANSFORMATIONSENTRY._serialized_start=6373
-  _CATALOGRESPONSE_TRANSFORMATIONSENTRY._serialized_end=6463
-  _FUNCTIONMETA._serialized_start=6466
-  _FUNCTIONMETA._serialized_end=6680
-  _DATASETPROCESSFUNCTIONMETA._serialized_start=6683
-  _DATASETPROCESSFUNCTIONMETA._serialized_end=6991
-  _TESTFUNCTIONARGUMENT._serialized_start=6993
-  _TESTFUNCTIONARGUMENT._serialized_end=7096
-  _COMPARISONCLAUSE._serialized_start=7099
-  _COMPARISONCLAUSE._serialized_end=7239
-  _GENERATEQUERYBASEDSLICEREQUEST._serialized_start=7241
-  _GENERATEQUERYBASEDSLICEREQUEST._serialized_end=7327
-  _GENERATEQUERYBASEDSLICERESPONSE._serialized_start=7329
-  _GENERATEQUERYBASEDSLICERESPONSE._serialized_end=7374
-  _MLWORKER._serialized_start=7676
-  _MLWORKER._serialized_end=8685
+  _SINGLETESTRESULT._serialized_end=4733
+  _SINGLETESTRESULT_PROPSENTRY._serialized_start=4689
+  _SINGLETESTRESULT_PROPSENTRY._serialized_end=4733
+  _TESTRESULTMESSAGE._serialized_start=4735
+  _TESTRESULTMESSAGE._serialized_end=4802
+  _DATASETPROCESSINGRESULTMESSAGE._serialized_start=4805
+  _DATASETPROCESSINGRESULTMESSAGE._serialized_end=4958
+  _DATASETROWMODIFICATIONRESULT._serialized_start=4961
+  _DATASETROWMODIFICATIONRESULT._serialized_end=5140
+  _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._serialized_start=5088
+  _DATASETROWMODIFICATIONRESULT_MODIFICATIONSENTRY._serialized_end=5140
+  _TESTSUITERESULTMESSAGE._serialized_start=5142
+  _TESTSUITERESULTMESSAGE._serialized_end=5268
+  _ARTIFACTREF._serialized_start=5270
+  _ARTIFACTREF._serialized_end=5348
+  _CHUNK._serialized_start=5350
+  _CHUNK._serialized_end=5374
+  _UPLOADSTATUS._serialized_start=5376
+  _UPLOADSTATUS._serialized_end=5424
+  _MLWORKERERRORINFO._serialized_start=5426
+  _MLWORKERERRORINFO._serialized_end=5475
+  _SUITEINPUT._serialized_start=5478
+  _SUITEINPUT._serialized_end=5642
+  _MODELMETA._serialized_start=5644
+  _MODELMETA._serialized_end=5695
+  _DATASETMETA._serialized_start=5697
+  _DATASETMETA._serialized_end=5742
+  _GENERATETESTSUITEREQUEST._serialized_start=5744
+  _GENERATETESTSUITEREQUEST._serialized_end=5827
+  _GENERATETESTSUITERESPONSE._serialized_start=5829
+  _GENERATETESTSUITERESPONSE._serialized_end=5894
+  _GENERATEDTEST._serialized_start=5896
+  _GENERATEDTEST._serialized_end=5974
+  _GENERATEDTESTINPUT._serialized_start=5976
+  _GENERATEDTESTINPUT._serialized_end=6043
+  _CATALOGRESPONSE._serialized_start=6046
+  _CATALOGRESPONSE._serialized_end=6481
+  _CATALOGRESPONSE_TESTSENTRY._serialized_start=6240
+  _CATALOGRESPONSE_TESTSENTRY._serialized_end=6306
+  _CATALOGRESPONSE_SLICESENTRY._serialized_start=6308
+  _CATALOGRESPONSE_SLICESENTRY._serialized_end=6389
+  _CATALOGRESPONSE_TRANSFORMATIONSENTRY._serialized_start=6391
+  _CATALOGRESPONSE_TRANSFORMATIONSENTRY._serialized_end=6481
+  _FUNCTIONMETA._serialized_start=6484
+  _FUNCTIONMETA._serialized_end=6698
+  _DATASETPROCESSFUNCTIONMETA._serialized_start=6701
+  _DATASETPROCESSFUNCTIONMETA._serialized_end=7009
+  _TESTFUNCTIONARGUMENT._serialized_start=7011
+  _TESTFUNCTIONARGUMENT._serialized_end=7114
+  _COMPARISONCLAUSE._serialized_start=7117
+  _COMPARISONCLAUSE._serialized_end=7257
+  _GENERATEQUERYBASEDSLICEREQUEST._serialized_start=7259
+  _GENERATEQUERYBASEDSLICEREQUEST._serialized_end=7345
+  _GENERATEQUERYBASEDSLICERESPONSE._serialized_start=7347
+  _GENERATEQUERYBASEDSLICERESPONSE._serialized_end=7392
+  _MLWORKER._serialized_start=7694
+  _MLWORKER._serialized_end=8703
 # @@protoc_insertion_point(module_scope)
```

### Comparing `giskard-2.0.0b8/giskard/ml_worker/generated/ml_worker_pb2_grpc.py` & `giskard-2.0.0b9/giskard/ml_worker/generated/ml_worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/ml_worker.py` & `giskard-2.0.0b9/giskard/ml_worker/ml_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/server/ml_worker_service.py` & `giskard-2.0.0b9/giskard/ml_worker/server/ml_worker_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,15 @@
     def explain(self, request: ml_worker_pb2.ExplainRequest, context) -> ml_worker_pb2.ExplainResponse:
         model = BaseModel.download(self.client, request.model.project_key, request.model.id)
         dataset = Dataset.download(self.client, request.dataset.project_key, request.dataset.id, request.dataset.sample)
         explanations = explain(model, dataset, request.columns)
 
         return ml_worker_pb2.ExplainResponse(
             explanations={
-                k: ml_worker_pb2.ExplainResponse.Explanation(per_feature=v)
+                str(k): ml_worker_pb2.ExplainResponse.Explanation(per_feature=v)
                 for k, v in explanations["explanations"].items()
             }
         )
 
     def explainText(self, request: ml_worker_pb2.ExplainTextRequest, context) -> ml_worker_pb2.ExplainTextResponse:
         n_samples = 500 if request.n_samples <= 0 else request.n_samples
         model = BaseModel.download(self.client, request.model.project_key, request.model.id)
@@ -555,14 +555,15 @@
 
 def map_result_to_single_test_result(result) -> ml_worker_pb2.SingleTestResult:
     if isinstance(result, ml_worker_pb2.SingleTestResult):
         return result
     elif isinstance(result, TestResult):
         return ml_worker_pb2.SingleTestResult(
             passed=result.passed,
+            is_error=result.is_error,
             messages=[
                 ml_worker_pb2.TestMessage(
                     type=ml_worker_pb2.TestMessageType.ERROR
                     if message.type == TestMessageLevel.ERROR
                     else ml_worker_pb2.TestMessageType.INFO,
                     text=message.text,
                 )
```

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/functions/slicing.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/functions/slicing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/functions/transformation.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/functions/transformation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/registry/decorators.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/registry/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/registry/decorators_utils.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/registry/decorators_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/registry/giskard_test.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/registry/giskard_test.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/registry/registry.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/registry/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 class GiskardTestRegistry:
     _tests: Dict[str, SavableMeta] = {}
 
     def register(self, meta: SavableMeta):
         if meta.uuid not in self._tests:
             self.add_func(meta)
             full_name = f"{meta.full_name} ({meta.uuid})" if hasattr(meta, "full_name") else f"{meta.uuid}"
-            logger.info(f"Registered test function: {full_name}")
+            logger.debug(f"Registered test function: {full_name}")
 
     def add_func(self, meta: SavableMeta):
         self._tests[meta.uuid] = meta
 
     def get_all(self):
         return self._tests
```

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/registry/slicing_function.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/registry/slicing_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/registry/transformation_function.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/registry/transformation_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/registry/udf_repository.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/registry/udf_repository.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/stat_utils.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/test_result.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/test_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     unexpected_percent_nonmissing: float = 0
     partial_unexpected_index_list: List[PartialUnexpectedCounts] = field(default_factory=list, repr=False)
     unexpected_index_list: List[int] = field(default_factory=list, repr=False)
     output_df: bytes = None
     number_of_perturbed_rows: int = 0
     actual_slices_size: List[int] = field(default_factory=list, repr=False)
     reference_slices_size: List[int] = field(default_factory=list, repr=False)
+    is_error: bool = False
 
     def _repr_html_(self):
         return """
                <h4><span style="color:{0};">{1}</span> Test {2}</h4>
                <p>Metric: {3}<p>
                <ul>{4}</ul>
                """.format(
```

### Comparing `giskard-2.0.0b8/giskard/ml_worker/testing/utils.py` & `giskard-2.0.0b9/giskard/ml_worker/testing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/utils/logging.py` & `giskard-2.0.0b9/giskard/ml_worker/utils/logging.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/utils/network.py` & `giskard-2.0.0b9/giskard/ml_worker/utils/network.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/ml_worker/utils/request_interceptor.py` & `giskard-2.0.0b9/giskard/ml_worker/utils/request_interceptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/__init__.py` & `giskard-2.0.0b9/giskard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/_precooked.py` & `giskard-2.0.0b9/giskard/models/_precooked.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/automodel/__init__.py` & `giskard-2.0.0b9/giskard/models/automodel/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/base/__init__.py` & `giskard-2.0.0b9/giskard/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/cache/__init__.py` & `giskard-2.0.0b9/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/cache/cache.py` & `giskard-2.0.0b9/giskard/models/cache/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/catboost/__init__.py` & `giskard-2.0.0b9/giskard/models/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/function/__init__.py` & `giskard-2.0.0b9/giskard/models/function/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/huggingface/__init__.py` & `giskard-2.0.0b9/giskard/models/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/langchain/__init__.py` & `giskard-2.0.0b9/giskard/models/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/model_explanation.py` & `giskard-2.0.0b9/giskard/models/model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/pytorch/__init__.py` & `giskard-2.0.0b9/giskard/models/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/sklearn/__init__.py` & `giskard-2.0.0b9/giskard/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/tensorflow/__init__.py` & `giskard-2.0.0b9/giskard/models/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/models/utils.py` & `giskard-2.0.0b9/giskard/models/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,23 +23,22 @@
     return some_list
 
 
 def np_type_to_native(i):
     return i.item() if isinstance(i, np.generic) else i
 
 
-def fix_seed():
-    seed = 1337
-
+def fix_seed(seed=1337):
     random.seed(seed)
     np.random.seed(seed)
     try:
         import torch
 
         torch.manual_seed(seed)
+        torch.cuda.manual_seed_all(seed)
     except ImportError:
         pass
 
 
 @lru_cache(None)
 def warn_once(logger, msg: str):
     logger.warning(msg)
```

### Comparing `giskard-2.0.0b8/giskard/path_utils.py` & `giskard-2.0.0b9/giskard/path_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/__init__.py` & `giskard-2.0.0b9/giskard/scanner/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ".performance.performance_bias_detector",
     ".robustness.text_perturbation_detector",
     ".robustness.ethical_bias_detector",
     ".data_leakage.data_leakage_detector",
     ".stochasticity.stochasticity_detector",
     ".calibration.overconfidence_detector",
     ".calibration.underconfidence_detector",
+    ".correlation.spurious_correlation_detector",
     ".llm.toxicity_detector",
 ]
 
 
 def _register_default_detectors():
     import importlib
```

### Comparing `giskard-2.0.0b8/giskard/scanner/calibration/issues.py` & `giskard-2.0.0b9/giskard/scanner/performance/issues.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,138 @@
-import pandas as pd
-from abc import abstractmethod
 from dataclasses import dataclass
 from functools import lru_cache
 
+from .metrics import PerformanceMetric
 from ..common.examples import ExampleExtractor
-
 from ..issues import Issue
 from ...datasets.base import Dataset
 from ...ml_worker.testing.registry.slicing_function import SlicingFunction
 from ...models.base import BaseModel
 from ...slicing.slice import QueryBasedSliceFunction
 from ...slicing.text_slicer import MetadataSliceFunction
 
 
 @dataclass
-class CalibrationIssueInfo:
+class PerformanceIssueInfo:
+    metric: PerformanceMetric
+    metric_value_reference: float
+    metric_value_slice: float
     slice_fn: SlicingFunction
     slice_size: int
-    metric_value_slice: float
-    metric_value_reference: float
-    loss_values: pd.Series
-    fail_idx: pd.DataFrame
     threshold: float
 
     @property
     def metric_rel_delta(self):
         return (self.metric_value_slice - self.metric_value_reference) / self.metric_value_reference
 
     @property
     def metric_abs_delta(self):
         return self.metric_value_slice - self.metric_value_reference
 
 
-class CalibrationIssue(Issue):
-    group = "Calibration"
+class PerformanceIssue(Issue):
+    """Performance Issue"""
+
+    group = "Performance"
 
-    info: CalibrationIssueInfo
+    info: PerformanceIssueInfo
 
     def __init__(
         self,
         model: BaseModel,
         dataset: Dataset,
         level: str,
-        info: CalibrationIssueInfo,
+        info: PerformanceIssueInfo,
     ):
         super().__init__(model, dataset, level, info)
 
+    def __repr__(self):
+        return f"<PerformanceIssue slice='{self.info.slice_fn}', metric='{self.info.metric.name}', metric_delta={self.info.metric_rel_delta * 100:.2f}%>"
+
     @property
     def domain(self):
         return str(self.info.slice_fn)
 
     @property
-    @abstractmethod
     def metric(self):
-        ...
+        return f"{self.info.metric.name} = {self.info.metric_value_slice:.2f}"
 
     @property
     def deviation(self):
-        return f"{self.info.metric_rel_delta * 100:.2f}% than global"
+        return f"{self.info.metric_rel_delta * 100:+.2f}% than global"
 
     @property
     def description(self):
-        return f"{len(self.info.fail_idx)} out of {self.info.slice_size} samples"
-
-    def _features(self):
-        if isinstance(self.info.slice_fn, QueryBasedSliceFunction):
-            return self.info.slice_fn.query.columns()
-        if isinstance(self.info.slice_fn, MetadataSliceFunction):
-            return [self.info.slice_fn.feature]
-        return self.model.meta.feature_names or self.dataset.columns
-
-    @property
-    def importance(self):
-        return self.info.metric_rel_delta
+        return f"{self.info.slice_size} samples ({self.info.slice_size / len(self.dataset) * 100:.2f}%)"
 
     @property
     def features(self):
         if isinstance(self.info.slice_fn, QueryBasedSliceFunction):
             return self.info.slice_fn.query.columns()
         if isinstance(self.info.slice_fn, MetadataSliceFunction):
             return [self.info.slice_fn.feature]
         return self.model.meta.feature_names or self.dataset.columns
 
     @lru_cache
     def examples(self, n=3):
         def filter_examples(issue, dataset):
-            bad_pred_mask = dataset.df.index.isin(self.info.fail_idx)
+            pred = issue.model.predict(dataset)
+            bad_pred_mask = dataset.df[dataset.target] != pred.prediction
 
             return dataset.slice(lambda df: df.loc[bad_pred_mask], row_level=False)
 
-        def sort_examples(issue, examples):
-            idx = self.info.loss_values.loc[examples.index].sort_values(ascending=False).index
-            return examples.loc[idx]
-
-        extractor = ExampleExtractor(self, filter_examples, sort_examples)
-        return extractor.get_examples_dataframe(n, with_prediction=2)
-
-    def generate_tests(self, with_names=False) -> list:
-        return []
-
-
-class OverconfidenceIssue(CalibrationIssue):
-    group = "Overconfidence"
+        extractor = ExampleExtractor(self, filter_examples)
+        return extractor.get_examples_dataframe(n, with_prediction=1)
 
     @property
-    def metric(self) -> str:
-        return "Overconfidence rate"
+    def importance(self):
+        if self.info.metric.greater_is_better:
+            return -self.info.metric_rel_delta
 
+        return self.info.metric_rel_delta
 
-class UnderconfidenceIssue(CalibrationIssue):
-    group = "Underconfidence"
+    @property
+    def slicing_fn(self):
+        return self.info.slice_fn
 
-    _num_labels_display = 2
+    def generate_tests(self, with_names=False) -> list:
+        test_fn = _metric_to_test_object(self.info.metric)
 
-    @property
-    def metric(self) -> str:
-        return "Underconfidence rate"
+        if test_fn is None:
+            return []
 
-    @property
-    def deviation(self):
-        return f"{self.info.metric_rel_delta * 100:.2f}% than global"
+        # Convert the relative threshold to an absolute one.
+        delta = (self.info.metric.greater_is_better * 2 - 1) * self.info.threshold * self.info.metric_value_reference
+        abs_threshold = self.info.metric_value_reference - delta
+
+        tests = [
+            test_fn(
+                model=self.model, dataset=self.dataset, slicing_function=self.info.slice_fn, threshold=abs_threshold
+            )
+        ]
+
+        if with_names:
+            names = [f"{self.info.metric.name} on data slice “{self.info.slice_fn}”"]
+            return list(zip(tests, names))
+
+        return tests
+
+
+_metric_test_mapping = {
+    "F1Score": "test_f1",
+    "Precision": "test_precision",
+    "Accuracy": "test_accuracy",
+    "Recall": "test_recall",
+    "AUC": "test_auc",
+    "MeanSquaredError": "test_mse",
+    "MeanAbsoluteError": "test_mae",
+}
+
+
+def _metric_to_test_object(metric: PerformanceMetric):
+    from ...testing.tests import performance as performance_tests
+
+    try:
+        test_name = _metric_test_mapping[metric.__class__.__name__]
+        return getattr(performance_tests, test_name)
+    except (KeyError, AttributeError):
+        return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `giskard-2.0.0b8/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.0.0b9/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 from typing import Sequence
-import numpy as np
 import pandas as pd
 
+from ...testing.tests.calibration import _calculate_underconfidence_score
+
 from ...ml_worker.testing.registry.slicing_function import SlicingFunction
 from ...models.base import BaseModel
 from ...datasets import Dataset
 from ..decorators import detector
 from ..common.loss_based_detector import LossBasedDetector
-from .issues import CalibrationIssue, CalibrationIssueInfo, OverconfidenceIssue
+from .issues import CalibrationIssue, CalibrationIssueInfo, UnderconfidenceIssue
 from ..logger import logger
 
 
-@detector(name="overconfidence", tags=["overconfidence", "classification"])
-class OverconfidenceDetector(LossBasedDetector):
-    def __init__(self, threshold=0.10, p_threshold=None, method="tree"):
+@detector(name="underconfidence", tags=["underconfidence", "classification"])
+class UnderconfidenceDetector(LossBasedDetector):
+    _needs_target = False
+
+    def __init__(self, threshold=0.1, p_threshold=0.95, method="tree"):
         self.threshold = threshold
         self.p_threshold = p_threshold
         self.method = method
 
     @property
     def _numerical_slicer_method(self):
         return self.method
 
     def run(self, model: BaseModel, dataset: Dataset):
         if not model.is_classification:
-            raise ValueError("Overconfidence bias detector only works for classification models.")
+            raise ValueError("Underconfidence detector only works for classification models.")
 
         return super().run(model, dataset)
 
     def _calculate_loss(self, model: BaseModel, dataset: Dataset) -> pd.DataFrame:
-        true_target = dataset.df.loc[:, dataset.target].values
-        pred = model.predict(dataset)
-        label2id = {label: n for n, label in enumerate(model.meta.classification_labels)}
-
-        # Empirical cost associated to overconfidence
-        p_max = pred.probabilities
-        p_true_label = np.array([pred.raw[n, label2id[label]] for n, label in enumerate(true_target)])
-
-        loss_values = p_max - p_true_label
-        mask = loss_values > 0
-
-        return pd.DataFrame({self.LOSS_COLUMN_NAME: loss_values[mask]}, index=dataset.df.index[mask])
+        return _calculate_underconfidence_score(model, dataset).to_frame(self.LOSS_COLUMN_NAME)
 
     def _find_issues(
         self,
         slices: Sequence[SlicingFunction],
         model: BaseModel,
         dataset: Dataset,
         meta: pd.DataFrame,
@@ -54,45 +46,48 @@
             dataset.df.join(meta, how="left"),
             target=dataset.target,
             column_types=dataset.column_types,
         )
         # For performance
         dataset_with_meta.load_metadata_from_instance(dataset.column_meta)
 
-        p_threshold = self.p_threshold or _default_overconfidence_threshold(model)
-        logger.info(f"{self.__class__.__name__}: Using overconfidence threshold = {p_threshold}")
-
-        reference_rate = (dataset_with_meta.df[self.LOSS_COLUMN_NAME].dropna() > p_threshold).mean()
+        reference_rate = (dataset_with_meta.df[self.LOSS_COLUMN_NAME].dropna() > self.p_threshold).mean()
 
         issues = []
         for slice_fn in slices:
             sliced_dataset = dataset_with_meta.slice(slice_fn)
 
-            slice_rate = (sliced_dataset.df[self.LOSS_COLUMN_NAME].dropna() > p_threshold).mean()
-            fail_idx = sliced_dataset.df[(sliced_dataset.df[self.LOSS_COLUMN_NAME] > p_threshold)].index
+            slice_rate = (sliced_dataset.df[self.LOSS_COLUMN_NAME].dropna() > self.p_threshold).mean()
+            fail_idx = sliced_dataset.df[(sliced_dataset.df[self.LOSS_COLUMN_NAME] > self.p_threshold)].index
+
+            # Skip non representative slices
+            # @TODO: do this with a statistical test instead of filtering by count only (GSK-1279)
+            if len(fail_idx) < 20:
+                continue
+
             relative_delta = (slice_rate - reference_rate) / reference_rate
 
+            logger.info(
+                f"{self.__class__.__name__}: Testing slice {slice_fn}\tUnderconfidence rate (slice) = {slice_rate:.3f} (global {reference_rate:.3f}) Δm = {relative_delta:.3f}"
+            )
+
             if relative_delta > self.threshold:
                 level = "major" if relative_delta > 2 * self.threshold else "medium"
                 issues.append(
-                    OverconfidenceIssue(
+                    UnderconfidenceIssue(
                         model,
                         dataset,
                         level,
                         CalibrationIssueInfo(
                             slice_fn=slice_fn,
                             slice_size=len(sliced_dataset),
                             metric_value_slice=slice_rate,
                             metric_value_reference=reference_rate,
                             loss_values=meta[self.LOSS_COLUMN_NAME],
                             fail_idx=fail_idx,
                             threshold=self.threshold,
+                            p_threshold=self.p_threshold,
                         ),
                     )
                 )
 
         return issues
-
-
-def _default_overconfidence_threshold(model: BaseModel) -> float:
-    n = len(model.meta.classification_labels)
-    return 1 / (3e-1 * (n - 2) + 2 - 1e-3 * (n - 2) ** 2)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `giskard-2.0.0b8/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.0.0b9/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from typing import Sequence
-import numpy as np
 import pandas as pd
 
+from ...testing.tests.calibration import _default_overconfidence_threshold
+
+from ...testing.tests.calibration import _calculate_overconfidence_score
+
 from ...ml_worker.testing.registry.slicing_function import SlicingFunction
 from ...models.base import BaseModel
 from ...datasets import Dataset
 from ..decorators import detector
 from ..common.loss_based_detector import LossBasedDetector
-from .issues import CalibrationIssue, CalibrationIssueInfo, UnderconfidenceIssue
+from .issues import CalibrationIssue, CalibrationIssueInfo, OverconfidenceIssue
 from ..logger import logger
 
 
-@detector(name="underconfidence", tags=["underconfidence", "classification"])
-class UnderconfidenceDetector(LossBasedDetector):
-    def __init__(self, threshold=0.1, p_threshold=0.95, method="tree"):
+@detector(name="overconfidence", tags=["overconfidence", "classification"])
+class OverconfidenceDetector(LossBasedDetector):
+    def __init__(self, threshold=0.10, p_threshold=None, method="tree"):
         self.threshold = threshold
         self.p_threshold = p_threshold
         self.method = method
 
     @property
     def _numerical_slicer_method(self):
         return self.method
 
     def run(self, model: BaseModel, dataset: Dataset):
         if not model.is_classification:
-            raise ValueError("Underconfidence detector only works for classification models.")
+            raise ValueError("Overconfidence bias detector only works for classification models.")
 
         return super().run(model, dataset)
 
     def _calculate_loss(self, model: BaseModel, dataset: Dataset) -> pd.DataFrame:
-        # Empirical cost associated to underconfidence: difference between
-        # the two most probable classes.
-        ps = model.predict(dataset).raw
-
-        # Relative difference
-        ps_2 = -np.partition(-ps, 1, axis=-1)[:, :2]
-        loss_values = ps_2.min(axis=-1) / ps_2.max(axis=-1)
-
-        return pd.DataFrame({self.LOSS_COLUMN_NAME: loss_values}, index=dataset.df.index)
+        loss = _calculate_overconfidence_score(model, dataset).to_frame(self.LOSS_COLUMN_NAME)
+        return loss[loss[self.LOSS_COLUMN_NAME] > 0]
 
     def _find_issues(
         self,
         slices: Sequence[SlicingFunction],
         model: BaseModel,
         dataset: Dataset,
         meta: pd.DataFrame,
@@ -51,46 +47,41 @@
             dataset.df.join(meta, how="left"),
             target=dataset.target,
             column_types=dataset.column_types,
         )
         # For performance
         dataset_with_meta.load_metadata_from_instance(dataset.column_meta)
 
-        reference_rate = (dataset_with_meta.df[self.LOSS_COLUMN_NAME].dropna() > self.p_threshold).mean()
+        p_threshold = self.p_threshold or _default_overconfidence_threshold(model)
+        logger.info(f"{self.__class__.__name__}: Using overconfidence threshold = {p_threshold}")
+
+        reference_rate = (dataset_with_meta.df[self.LOSS_COLUMN_NAME].dropna() > p_threshold).mean()
 
         issues = []
         for slice_fn in slices:
             sliced_dataset = dataset_with_meta.slice(slice_fn)
 
-            slice_rate = (sliced_dataset.df[self.LOSS_COLUMN_NAME].dropna() > self.p_threshold).mean()
-            fail_idx = sliced_dataset.df[(sliced_dataset.df[self.LOSS_COLUMN_NAME] > self.p_threshold)].index
-
-            # Skip non representative slices
-            if len(fail_idx) < 20:
-                continue
-
+            slice_rate = (sliced_dataset.df[self.LOSS_COLUMN_NAME].dropna() > p_threshold).mean()
+            fail_idx = sliced_dataset.df[(sliced_dataset.df[self.LOSS_COLUMN_NAME] > p_threshold)].index
             relative_delta = (slice_rate - reference_rate) / reference_rate
 
-            logger.info(
-                f"{self.__class__.__name__}: Testing slice {slice_fn}\tUnderconfidence rate (slice) = {slice_rate:.3f} (global {reference_rate:.3f}) Δm = {relative_delta:.3f}"
-            )
-
             if relative_delta > self.threshold:
                 level = "major" if relative_delta > 2 * self.threshold else "medium"
                 issues.append(
-                    UnderconfidenceIssue(
+                    OverconfidenceIssue(
                         model,
                         dataset,
                         level,
                         CalibrationIssueInfo(
                             slice_fn=slice_fn,
                             slice_size=len(sliced_dataset),
                             metric_value_slice=slice_rate,
                             metric_value_reference=reference_rate,
                             loss_values=meta[self.LOSS_COLUMN_NAME],
                             fail_idx=fail_idx,
                             threshold=self.threshold,
+                            p_threshold=p_threshold,
                         ),
                     )
                 )
 
         return issues
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `giskard-2.0.0b8/giskard/scanner/common/examples.py` & `giskard-2.0.0b9/giskard/scanner/common/examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,17 @@
         # Filter if needed
         if self.filter_fn:
             dataset = self.filter_fn(issue, dataset)
 
         examples = dataset.df.copy()
 
         # Keep only interesting columns
-        cols_to_show = issue.features + [issue.dataset.target]
+        cols_to_show = issue.features
+        if issue.dataset.target is not None:
+            cols_to_show += [issue.dataset.target]
         examples = examples.loc[:, cols_to_show]
 
         # If metadata slice, add the metadata column
         if isinstance(issue.slicing_fn, MetadataSliceFunction):
             for col in issue.features:
                 meta_cols = issue.slicing_fn.query.columns()
                 provider = issue.slicing_fn.provider
@@ -50,15 +52,18 @@
                     label_idx = np.argsort(-ps)[:num_labels_to_print]
                     pred_examples.append(
                         "\n".join([f"{issue.model.meta.classification_labels[i]} (p = {ps[i]:.2f})" for i in label_idx])
                     )
             else:
                 pred_examples = model_pred.prediction
 
-            examples[f"Predicted `{issue.dataset.target}`"] = pred_examples
+            predicted_label = "Predicted"
+            if issue.dataset.target is not None:
+                predicted_label += f" `{issue.dataset.target}`"
+            examples[predicted_label] = pred_examples
 
         n = min(len(examples), n)
         if n > 0:
             if self.sorting_fn:
                 return self.sorting_fn(issue, examples).head(n)
 
             return examples.sample(n, random_state=142)
```

### Comparing `giskard-2.0.0b8/giskard/scanner/common/loss_based_detector.py` & `giskard-2.0.0b9/giskard/scanner/common/loss_based_detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import datetime
 from time import perf_counter
 import pandas as pd
 from typing import Sequence
 from abc import abstractmethod
 
+from ...slicing.slice_finder import SliceFinder
+
 from ..registry import Detector
 
 from ...models.base import BaseModel
 from ...datasets.base import Dataset
-from ...slicing.utils import get_slicer
-from ...slicing.text_slicer import TextSlicer
-from ...slicing.category_slicer import CategorySlicer
 from ...ml_worker.testing.registry.slicing_function import SlicingFunction
 from ..logger import logger
 from ..issues import Issue
 
 
 class LossBasedDetector(Detector):
     MIN_DATASET_LENGTH = 100
     MAX_DATASET_SIZE = 10_000_000
     LOSS_COLUMN_NAME = "__gsk__loss"
 
+    _needs_target = True
+
     def run(self, model: BaseModel, dataset: Dataset):
+        if self._needs_target and dataset.target is None:
+            logger.info(f"{self.__class__.__name__}: Skipping detection because the dataset has no target column.")
+            return []
+
         logger.info(f"{self.__class__.__name__}: Running")
 
         # Check if we have enough data to run the scan
         if len(dataset) < self.MIN_DATASET_LENGTH:
             logger.warning(
                 f"{self.__class__.__name__}: Skipping scan because the dataset is too small"
                 f" (< {self.MIN_DATASET_LENGTH} samples)."
@@ -44,16 +49,15 @@
         meta = self._calculate_loss(model, dataset)
         elapsed = perf_counter() - start
         logger.info(f"{self.__class__.__name__}: Loss calculated (took {datetime.timedelta(seconds=elapsed)})")
 
         # Find slices
         logger.info(f"{self.__class__.__name__}: Finding data slices")
         start = perf_counter()
-        dataset_to_slice = dataset.select_columns(model.meta.feature_names) if model.meta.feature_names else dataset
-        slices = self._find_slices(dataset_to_slice, meta)
+        slices = self._find_slices(model, dataset, meta)
         elapsed = perf_counter() - start
         logger.info(
             f"{self.__class__.__name__}: {len(slices)} slices found (took {datetime.timedelta(seconds=elapsed)})"
         )
 
         # Create issues from the slices
         logger.info(f"{self.__class__.__name__}: Analyzing issues")
@@ -66,51 +70,35 @@
 
         return issues
 
     @property
     def _numerical_slicer_method(self):
         return "tree"
 
-    def _find_slices(self, dataset: Dataset, meta: pd.DataFrame):
+    def _find_slices(self, model: BaseModel, dataset: Dataset, meta: pd.DataFrame):
+        features = model.meta.feature_names or dataset.columns.drop(dataset.target, errors="ignore")
+
         df_with_meta = dataset.df.join(meta, how="right")
 
         column_types = dataset.column_types.copy()
         column_types[self.LOSS_COLUMN_NAME] = "numeric"
         dataset_with_meta = Dataset(
             df_with_meta,
             target=dataset.target,
             column_types=column_types,
             validation=False,
         )
 
         # For performance
         dataset_with_meta.load_metadata_from_instance(dataset.column_meta)
 
-        # Columns by type
-        cols_by_type = {
-            type_val: [col for col, col_type in dataset.column_types.items() if col_type == type_val]
-            for type_val in ["numeric", "category", "text"]
-        }
-
-        # Numerical features
-        slicer = get_slicer(self._numerical_slicer_method, dataset_with_meta, self.LOSS_COLUMN_NAME)
-
-        slices = []
-        for col in cols_by_type["numeric"]:
-            slices.extend(slicer.find_slices([col]))
-
-        # Categorical features
-        slicer = CategorySlicer(dataset_with_meta, target=self.LOSS_COLUMN_NAME)
-        for col in cols_by_type["category"]:
-            slices.extend(slicer.find_slices([col]))
-
-        # Text features
-        slicer = TextSlicer(dataset_with_meta, target=self.LOSS_COLUMN_NAME, slicer=self._numerical_slicer_method)
-        for col in cols_by_type["text"]:
-            slices.extend(slicer.find_slices([col]))
+        # Find slices
+        sf = SliceFinder(numerical_slicer=self._numerical_slicer_method)
+        sliced = sf.run(dataset_with_meta, features, target=self.LOSS_COLUMN_NAME)
+        slices = sum(sliced.values(), start=[])
 
         # Keep only slices of size at least 5% of the dataset or 20 samples (whatever is larger)
         slices = [s for s in slices if max(0.05 * len(dataset), 20) <= len(dataset_with_meta.slice(s))]
 
         return slices
 
     @abstractmethod
```

### Comparing `giskard-2.0.0b8/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.0.0b9/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/decorators.py` & `giskard-2.0.0b9/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/issues.py` & `giskard-2.0.0b9/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/llm/toxicity_detector.py` & `giskard-2.0.0b9/giskard/scanner/llm/toxicity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/llm/utils.py` & `giskard-2.0.0b9/giskard/scanner/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/performance/issues.py` & `giskard-2.0.0b9/giskard/scanner/calibration/issues.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,138 +1,167 @@
+import pandas as pd
+from abc import abstractmethod
 from dataclasses import dataclass
 from functools import lru_cache
 
-from .metrics import PerformanceMetric
+from ...testing.tests.calibration import test_underconfidence_rate
+
+from ...testing.tests.calibration import test_overconfidence_rate
+
 from ..common.examples import ExampleExtractor
+
 from ..issues import Issue
 from ...datasets.base import Dataset
 from ...ml_worker.testing.registry.slicing_function import SlicingFunction
 from ...models.base import BaseModel
 from ...slicing.slice import QueryBasedSliceFunction
 from ...slicing.text_slicer import MetadataSliceFunction
 
 
 @dataclass
-class PerformanceIssueInfo:
-    metric: PerformanceMetric
-    metric_value_reference: float
-    metric_value_slice: float
+class CalibrationIssueInfo:
     slice_fn: SlicingFunction
     slice_size: int
+    metric_value_slice: float
+    metric_value_reference: float
+    loss_values: pd.Series
+    fail_idx: pd.DataFrame
     threshold: float
+    p_threshold: float
 
     @property
     def metric_rel_delta(self):
         return (self.metric_value_slice - self.metric_value_reference) / self.metric_value_reference
 
     @property
     def metric_abs_delta(self):
         return self.metric_value_slice - self.metric_value_reference
 
 
-class PerformanceIssue(Issue):
-    """Performance Issue"""
-
-    group = "Performance"
+class CalibrationIssue(Issue):
+    group = "Calibration"
 
-    info: PerformanceIssueInfo
+    info: CalibrationIssueInfo
 
     def __init__(
         self,
         model: BaseModel,
         dataset: Dataset,
         level: str,
-        info: PerformanceIssueInfo,
+        info: CalibrationIssueInfo,
     ):
         super().__init__(model, dataset, level, info)
 
-    def __repr__(self):
-        return f"<PerformanceIssue slice='{self.info.slice_fn}', metric='{self.info.metric.name}', metric_delta={self.info.metric_rel_delta * 100:.2f}%>"
-
     @property
     def domain(self):
         return str(self.info.slice_fn)
 
     @property
+    @abstractmethod
     def metric(self):
-        return f"{self.info.metric.name} = {self.info.metric_value_slice:.2f}"
+        ...
 
     @property
     def deviation(self):
-        return f"{self.info.metric_rel_delta * 100:+.2f}% than global"
+        return f"{self.info.metric_rel_delta * 100:.2f}% than global"
 
     @property
     def description(self):
-        return f"{self.info.slice_size} samples ({self.info.slice_size / len(self.dataset) * 100:.2f}%)"
+        return f"{len(self.info.fail_idx)} out of {self.info.slice_size} samples"
+
+    def _features(self):
+        if isinstance(self.info.slice_fn, QueryBasedSliceFunction):
+            return self.info.slice_fn.query.columns()
+        if isinstance(self.info.slice_fn, MetadataSliceFunction):
+            return [self.info.slice_fn.feature]
+        return self.model.meta.feature_names or self.dataset.columns
+
+    @property
+    def importance(self):
+        return self.info.metric_rel_delta
 
     @property
     def features(self):
         if isinstance(self.info.slice_fn, QueryBasedSliceFunction):
             return self.info.slice_fn.query.columns()
         if isinstance(self.info.slice_fn, MetadataSliceFunction):
             return [self.info.slice_fn.feature]
         return self.model.meta.feature_names or self.dataset.columns
 
     @lru_cache
     def examples(self, n=3):
         def filter_examples(issue, dataset):
-            pred = issue.model.predict(dataset)
-            bad_pred_mask = dataset.df[dataset.target] != pred.prediction
+            bad_pred_mask = dataset.df.index.isin(self.info.fail_idx)
 
             return dataset.slice(lambda df: df.loc[bad_pred_mask], row_level=False)
 
-        extractor = ExampleExtractor(self, filter_examples)
-        return extractor.get_examples_dataframe(n, with_prediction=1)
+        def sort_examples(issue, examples):
+            idx = self.info.loss_values.loc[examples.index].sort_values(ascending=False).index
+            return examples.loc[idx]
 
-    @property
-    def importance(self):
-        if self.info.metric.greater_is_better:
-            return -self.info.metric_rel_delta
+        extractor = ExampleExtractor(self, filter_examples, sort_examples)
+        return extractor.get_examples_dataframe(n, with_prediction=2)
 
-        return self.info.metric_rel_delta
+    def generate_tests(self, with_names=False) -> list:
+        return []
 
-    @property
-    def slicing_fn(self):
-        return self.info.slice_fn
 
-    def generate_tests(self, with_names=False) -> list:
-        test_fn = _metric_to_test_object(self.info.metric)
+class OverconfidenceIssue(CalibrationIssue):
+    group = "Overconfidence"
 
-        if test_fn is None:
-            return []
+    @property
+    def metric(self) -> str:
+        return "Overconfidence rate"
 
-        # Convert the relative threshold to an absolute one.
-        delta = (self.info.metric.greater_is_better * 2 - 1) * self.info.threshold * self.info.metric_value_reference
-        abs_threshold = self.info.metric_value_reference - delta
+    def generate_tests(self, with_names=False) -> list:
+        abs_threshold = self.info.metric_value_reference * (1 + self.info.threshold)
 
         tests = [
-            test_fn(
-                model=self.model, dataset=self.dataset, slicing_function=self.info.slice_fn, threshold=abs_threshold
+            test_overconfidence_rate(
+                model=self.model,
+                dataset=self.dataset,
+                slicing_function=self.info.slice_fn,
+                threshold=abs_threshold,
+                p_threshold=self.info.p_threshold,
             )
         ]
 
         if with_names:
-            names = [f"{self.info.metric.name} on data slice “{self.info.slice_fn}”"]
+            names = [f"Overconfidence on data slice “{self.info.slice_fn}”"]
+
             return list(zip(tests, names))
 
         return tests
 
 
-_metric_test_mapping = {
-    "F1Score": "test_f1",
-    "Precision": "test_precision",
-    "Accuracy": "test_accuracy",
-    "Recall": "test_recall",
-    "AUC": "test_auc",
-    "MeanSquaredError": "test_mse",
-    "MeanAbsoluteError": "test_mae",
-}
-
-
-def _metric_to_test_object(metric: PerformanceMetric):
-    from ...testing.tests import performance as performance_tests
-
-    try:
-        test_name = _metric_test_mapping[metric.__class__.__name__]
-        return getattr(performance_tests, test_name)
-    except (KeyError, AttributeError):
-        return None
+class UnderconfidenceIssue(CalibrationIssue):
+    group = "Underconfidence"
+
+    _num_labels_display = 2
+
+    @property
+    def metric(self) -> str:
+        return "Underconfidence rate"
+
+    @property
+    def deviation(self):
+        return f"{self.info.metric_rel_delta * 100:.2f}% than global"
+
+    def generate_tests(self, with_names=False) -> list:
+        abs_threshold = self.info.metric_value_reference * (1 + self.info.threshold)
+
+        tests = [
+            test_underconfidence_rate(
+                model=self.model,
+                dataset=self.dataset,
+                slicing_function=self.info.slice_fn,
+                threshold=abs_threshold,
+                p_threshold=self.info.p_threshold,
+            )
+        ]
+
+        if with_names:
+            names = [f"Underconfidence on data slice “{self.info.slice_fn}”"]
+
+            return list(zip(tests, names))
+
+        return tests
```

### Comparing `giskard-2.0.0b8/giskard/scanner/performance/metrics.py` & `giskard-2.0.0b9/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.0.0b9/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/registry.py` & `giskard-2.0.0b9/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/result.py` & `giskard-2.0.0b9/giskard/scanner/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,18 +42,21 @@
         for issue in self.issues:
             issues_by_group[issue.group].append(issue)
 
         html = tpl.render(
             issues=self.issues,
             issues_by_group=issues_by_group,
             num_major_issues={
-                group: len([i for i in issues if i.is_major]) for group, issues in issues_by_group.items()
+                group: len([i for i in issues if i.level == "major"]) for group, issues in issues_by_group.items()
             },
             num_medium_issues={
-                group: len([i for i in issues if not i.is_major]) for group, issues in issues_by_group.items()
+                group: len([i for i in issues if i.level == "medium"]) for group, issues in issues_by_group.items()
+            },
+            num_info_issues={
+                group: len([i for i in issues if i.level == "info"]) for group, issues in issues_by_group.items()
             },
         )
 
         escaped = escape(html)
         uid = id(self)
 
         from pathlib import Path
```

### Comparing `giskard-2.0.0b8/giskard/scanner/robustness/base_detector.py` & `giskard-2.0.0b9/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/robustness/entity_swap.py` & `giskard-2.0.0b9/giskard/scanner/robustness/entity_swap.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.0.0b9/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/robustness/issues.py` & `giskard-2.0.0b9/giskard/scanner/robustness/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/robustness/nationalities.json` & `giskard-2.0.0b9/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.0.0b9/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/robustness/text_transformations.py` & `giskard-2.0.0b9/giskard/scanner/robustness/text_transformations.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/scanner.py` & `giskard-2.0.0b9/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.0.0b9/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_code_snippet.html` & `giskard-2.0.0b9/giskard/scanner/templates/_code_snippet.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues/data_leakage.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues/data_leakage.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues/default.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues/default.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues/llm_toxicity.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues/llm_toxicity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues/overconfidence.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues/overconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues/performance.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues/performance.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues/robustness.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues/robustness.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues/stochasticity.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues/stochasticity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues/underconfidence.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues/underconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_issues_table.html` & `giskard-2.0.0b9/giskard/scanner/templates/_issues_table.html`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
                 {% include "_issues/underconfidence.html" %}
             {% elif issue.__class__.__name__ == 'DataLeakageIssue' %}
                 {% include "_issues/data_leakage.html" %}
             {% elif issue.__class__.__name__ == 'StochasticityIssue' %}
                 {% include "_issues/stochasticity.html" %}
             {% elif issue.__class__.__name__ == 'LLMToxicityIssue' %}
                 {% include "_issues/llm_toxicity.html" %}
+            {% elif issue.__class__.__name__ == 'SpuriousCorrelationIssue' %}
+                {% include "_issues/spurious_correlation.html" %}
             {% else %}
                 {% include "_issues/default.html" %}
             {% endif %}
         </tbody>
         {% endfor %}
     </table>
 </div>
```

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_main_content.html` & `giskard-2.0.0b9/giskard/scanner/templates/_main_content.html`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,20 @@
                 execution. This may happen when some stochastic training process is included in the prediction pipeline.
             </p>
             {% elif issues[0].__class__.__name__ == "LLMToxicityIssue" %}
             <p>
                 Your model seems to exhibit offensive behaviour when we use adversarial “Do Anything Now” (DAN)
                 prompts.
             </p>
+            {% elif issues[0].__class__.__name__ == "SpuriousCorrelationIssue" %}
+            <p>
+                We found potential spurious correlations between your data and the model predictions. Spurious
+                correlations may occur when the model overfits on relations that are not causal. We recommend that you
+                verify the causal relationship between the detected data slices and the target variable.
+            </p>
             {% else %}
             <p>Found issues for {{ issues[0].group }}</p>
             {% endif %}
         </div>
     </div>
 
     <div class="flex items-center space-x-1">
@@ -97,14 +103,18 @@
         <span class="text-xs border rounded px-1 uppercase text-red-400 border-red-400">{{num_major_issues[group]}}
             major</span>
         {% endif %}
         {% if num_medium_issues[group] > 0 %}
         <span class="text-xs border rounded px-1 uppercase text-amber-200 border-amber-200">{{num_medium_issues[group]}}
             medium</span>
         {% endif %}
+        {% if num_info_issues[group] > 0 %}
+        <span class="text-xs border rounded px-1 uppercase text-blue-200 border-blue-200">{{num_info_issues[group]}}
+            info</span>
+        {% endif %}
     </div>
 
     {% include "_issues_table.html" %}
 </div>
 {% endfor %}
 
 {% if issues|length == 0 %}
```

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/_tab_header.html` & `giskard-2.0.0b9/giskard/scanner/templates/_tab_header.html`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,24 @@
     {% for group, issues in issues_by_group.items() %}
     <div data-tab-target="{{ group | replace(' ', '_') }}"
         class="cursor-pointer group{% if loop.index == 1 %} active{% endif %}">
         <div
             class="group-[.active]:bg-zinc-800 group-[.active]:border-b-zinc-800 group-[.active]:border-gray-500 border-l px-3 py-2 border-r border-t border-b border-gray-600 border-b-gray-500 h-11">
             {{ group}}
             {% if issues | length > 0 %}
-            {% if num_major_issues[group] > 0 %}
-            <span class="ml-1 rounded-full text-xs min-w-4 min-h-4 px-1 py-0.5 inline-block text-center bg-red-400">
+                {% if num_major_issues[group] > 0 %}
+                <span class="ml-1 rounded-full text-xs min-w-4 min-h-4 px-1 py-0.5 inline-block text-center bg-red-400">
+                {% elif num_medium_issues[group] > 0 %}
+                <span class="ml-1 rounded-full text-xs min-w-4 min-h-4 px-1 py-0.5 inline-block text-center bg-amber-200 text-amber-900">
                 {% else %}
-                <span
-                    class="ml-1 rounded-full text-xs min-w-4 min-h-4 px-1 py-0.5 inline-block text-center bg-amber-200 text-amber-900">
-                    {% endif %}
+                <span class="ml-1 rounded-full text-xs min-w-4 min-h-4 px-1 py-0.5 inline-block text-center bg-blue-300 text-blue-900">
+                {% endif %}
                     {{ issues | length }}
                 </span>
-                {% endif %}
+            {% endif %}
         </div>
     </div>
     {% endfor %}
 
     {# Spacer #}
     <div class="flex-grow border-b border-gray-500 h-11"></div>
 </div>
```

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/scan_results.html` & `giskard-2.0.0b9/giskard/scanner/templates/scan_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/static/external.js` & `giskard-2.0.0b9/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/static/internal.js` & `giskard-2.0.0b9/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/scanner/templates/static/style.css` & `giskard-2.0.0b9/giskard/scanner/templates/static/style.css`

 * *Files 5% similar despite different names*

```diff
@@ -5,8 +5,8 @@
   Author: github.com
   Maintainer: @Hirse
   Updated: 2021-05-15
 
   Outdated base version: https://github.com/primer/github-syntax-dark
   Current colors taken from GitHub's CSS
 */.hljs{background:#0d1117;color:#c9d1d9}.hljs-doctag,.hljs-keyword,.hljs-meta .hljs-keyword,.hljs-template-tag,.hljs-template-variable,.hljs-type,.hljs-variable.language_{color:#ff7b72}.hljs-title,.hljs-title.class_,.hljs-title.class_.inherited__,.hljs-title.function_{color:#d2a8ff}.hljs-attr,.hljs-attribute,.hljs-literal,.hljs-meta,.hljs-number,.hljs-operator,.hljs-selector-attr,.hljs-selector-class,.hljs-selector-id,.hljs-variable{color:#79c0ff}.hljs-meta .hljs-string,.hljs-regexp,.hljs-string{color:#a5d6ff}.hljs-built_in,.hljs-symbol{color:#ffa657}.hljs-code,.hljs-comment,.hljs-formula{color:#8b949e}.hljs-name,.hljs-quote,.hljs-selector-pseudo,.hljs-selector-tag{color:#7ee787}.hljs-subst{color:#c9d1d9}.hljs-section{color:#1f6feb;font-weight:700}.hljs-bullet{color:#f2cc60}.hljs-emphasis{color:#c9d1d9;font-style:italic}.hljs-strong{color:#c9d1d9;font-weight:700}.hljs-addition{background-color:#033a16;color:#aff5b4}.hljs-deletion{background-color:#67060c;color:#ffdcd7}.hljs-copy-wrapper{overflow:hidden;position:relative}.hljs-copy-button:focus,.hljs-copy-wrapper:hover .hljs-copy-button{transform:translateX(0)}.hljs-copy-button{background-color:#2d2b57;background-color:var(--hljs-theme-background);background-image:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="none" viewBox="0 0 24 24"><path fill="%23fff" fill-rule="evenodd" d="M6 5a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1V6a1 1 0 0 0-1-1h-2a1 1 0 1 1 0-2h2a3 3 0 0 1 3 3v14a3 3 0 0 1-3 3H6a3 3 0 0 1-3-3V6a3 3 0 0 1 3-3h2a1 1 0 0 1 0 2H6Z" clip-rule="evenodd"/><path fill="%23fff" fill-rule="evenodd" d="M7 3a2 2 0 0 1 2-2h6a2 2 0 0 1 2 2v2a2 2 0 0 1-2 2H9a2 2 0 0 1-2-2V3Zm8 0H9v2h6V3Z" clip-rule="evenodd"/></svg>');background-position:50%;background-repeat:no-repeat;border:1px solid #ffffff22;border-radius:.25rem;color:#fff;height:2rem;position:absolute;right:1em;text-indent:-9999px;top:1em;transition:background-color .2s ease,transform .2s ease-out;width:2rem}.hljs-copy-button:hover{border-color:#ffffff44}.hljs-copy-button:active{border-color:#ffffff66}.hljs-copy-button[data-copied=true]{background-image:none;text-indent:0;width:auto}@media (prefers-reduced-motion){.hljs-copy-button{transition:none}}.hljs-copy-alert{clip:rect(0 0 0 0);-webkit-clip-path:inset(50%);clip-path:inset(50%);height:1px;overflow:hidden;position:absolute;white-space:nowrap;width:1px}
-/*! tailwindcss v3.3.2 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.collapse{visibility:collapse}.m-4{margin:1rem}.my-1{margin-bottom:.25rem;margin-top:.25rem}.my-2{margin-bottom:.5rem;margin-top:.5rem}.my-4{margin-top:1rem}.mb-4,.my-4{margin-bottom:1rem}.ml-1{margin-left:.25rem}.ml-2{margin-left:.5rem}.ml-4{margin-left:1rem}.mr-2{margin-right:.5rem}.mt-1{margin-top:.25rem}.mt-1\.5{margin-top:.375rem}.mt-4{margin-top:1rem}.block{display:block}.inline-block{display:inline-block}.flex{display:flex}.table{display:table}.hidden{display:none}.h-11{height:2.75rem}.h-6{height:1.5rem}.w-6{width:1.5rem}.w-full{width:100%}.max-w-xl{max-width:36rem}.flex-grow{flex-grow:1}.table-auto{table-layout:auto}.cursor-pointer{cursor:pointer}.resize{resize:both}.list-disc{list-style-type:disc}.items-center{align-items:center}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:calc(.25rem*(1 - var(--tw-space-x-reverse)));margin-right:calc(.25rem*var(--tw-space-x-reverse))}.overflow-scroll{overflow:scroll}.rounded{border-radius:.25rem}.rounded-full{border-radius:9999px}.rounded-sm{border-radius:.125rem}.rounded-t{border-top-left-radius:.25rem;border-top-right-radius:.25rem}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-l{border-left-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-amber-200{--tw-border-opacity:1;border-color:rgb(253 230 138/var(--tw-border-opacity))}.border-gray-500{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.border-gray-600{--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}.border-red-400{--tw-border-opacity:1;border-color:rgb(248 113 113/var(--tw-border-opacity))}.border-zinc-100\/50{border-color:hsla(240,5%,96%,.5)}.border-zinc-500{--tw-border-opacity:1;border-color:rgb(113 113 122/var(--tw-border-opacity))}.border-b-gray-500{--tw-border-opacity:1;border-bottom-color:rgb(107 114 128/var(--tw-border-opacity))}.bg-amber-100\/40{background-color:hsla(48,96%,89%,.4)}.bg-amber-200{--tw-bg-opacity:1;background-color:rgb(253 230 138/var(--tw-bg-opacity))}.bg-green-100\/40{background-color:rgba(220,252,231,.4)}.bg-red-400{--tw-bg-opacity:1;background-color:rgb(248 113 113/var(--tw-bg-opacity))}.bg-zinc-500{--tw-bg-opacity:1;background-color:rgb(113 113 122/var(--tw-bg-opacity))}.bg-zinc-700{--tw-bg-opacity:1;background-color:rgb(63 63 70/var(--tw-bg-opacity))}.p-3{padding:.75rem}.p-4{padding:1rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-3{padding-left:.75rem;padding-right:.75rem}.px-4{padding-left:1rem;padding-right:1rem}.py-0{padding-bottom:0;padding-top:0}.py-0\.5{padding-bottom:.125rem;padding-top:.125rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.pt-1{padding-top:.25rem}.text-left{text-align:left}.text-center{text-align:center}.text-right{text-align:right}.align-middle{vertical-align:middle}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.uppercase{text-transform:uppercase}.lowercase{text-transform:lowercase}.text-amber-100{--tw-text-opacity:1;color:rgb(254 243 199/var(--tw-text-opacity))}.text-amber-200{--tw-text-opacity:1;color:rgb(253 230 138/var(--tw-text-opacity))}.text-amber-900{--tw-text-opacity:1;color:rgb(120 53 15/var(--tw-text-opacity))}.text-blue-300{--tw-text-opacity:1;color:rgb(147 197 253/var(--tw-text-opacity))}.text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.text-green-50{--tw-text-opacity:1;color:rgb(240 253 244/var(--tw-text-opacity))}.text-red-400{--tw-text-opacity:1;color:rgb(248 113 113/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.text-zinc-100\/90{color:hsla(240,5%,96%,.9)}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}table.dataframe{max-width:100%;overflow:auto;width:100%}.dataframe tr{border-bottom:1px solid #555}.dataframe td,.dataframe th{padding:.5rem}.dataframe th{text-align:left!important}.first\:border-t:first-child{border-top-width:1px}.hover\:border-zinc-500:hover{--tw-border-opacity:1;border-color:rgb(113 113 122/var(--tw-border-opacity))}.hover\:bg-zinc-400:hover{--tw-bg-opacity:1;background-color:rgb(161 161 170/var(--tw-bg-opacity))}.hover\:bg-zinc-500:hover{--tw-bg-opacity:1;background-color:rgb(113 113 122/var(--tw-bg-opacity))}.hover\:bg-zinc-700:hover{--tw-bg-opacity:1;background-color:rgb(63 63 70/var(--tw-bg-opacity))}.hover\:text-white:hover{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.group.open .group-\[\.open\]\:inline-block{display:inline-block}.group.open .group-\[\.open\]\:hidden{display:none}.group.active .group-\[\.active\]\:border-gray-500{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.group.active .group-\[\.active\]\:border-b-zinc-800{--tw-border-opacity:1;border-bottom-color:rgb(39 39 42/var(--tw-border-opacity))}.group.active .group-\[\.active\]\:bg-zinc-800{--tw-bg-opacity:1;background-color:rgb(39 39 42/var(--tw-bg-opacity))}.peer.open~.peer-\[\.open\]\:visible{visibility:visible}:is(.dark .dark\:bg-zinc-800){--tw-bg-opacity:1;background-color:rgb(39 39 42/var(--tw-bg-opacity))}:is(.dark .dark\:bg-zinc-900){--tw-bg-opacity:1;background-color:rgb(24 24 27/var(--tw-bg-opacity))}:is(.dark .dark\:fill-white){fill:#fff}:is(.dark .dark\:text-white){--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}
+/*! tailwindcss v3.3.2 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.collapse{visibility:collapse}.m-4{margin:1rem}.my-1{margin-bottom:.25rem;margin-top:.25rem}.my-2{margin-bottom:.5rem;margin-top:.5rem}.my-4{margin-top:1rem}.mb-4,.my-4{margin-bottom:1rem}.ml-1{margin-left:.25rem}.ml-2{margin-left:.5rem}.ml-4{margin-left:1rem}.mr-2{margin-right:.5rem}.mt-1{margin-top:.25rem}.mt-1\.5{margin-top:.375rem}.mt-4{margin-top:1rem}.block{display:block}.inline-block{display:inline-block}.flex{display:flex}.table{display:table}.hidden{display:none}.h-11{height:2.75rem}.h-6{height:1.5rem}.w-6{width:1.5rem}.w-full{width:100%}.max-w-xl{max-width:36rem}.flex-grow{flex-grow:1}.table-auto{table-layout:auto}.cursor-pointer{cursor:pointer}.resize{resize:both}.list-disc{list-style-type:disc}.items-center{align-items:center}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:calc(.25rem*(1 - var(--tw-space-x-reverse)));margin-right:calc(.25rem*var(--tw-space-x-reverse))}.overflow-scroll{overflow:scroll}.rounded{border-radius:.25rem}.rounded-full{border-radius:9999px}.rounded-sm{border-radius:.125rem}.rounded-t{border-top-left-radius:.25rem;border-top-right-radius:.25rem}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-l{border-left-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-amber-200{--tw-border-opacity:1;border-color:rgb(253 230 138/var(--tw-border-opacity))}.border-blue-200{--tw-border-opacity:1;border-color:rgb(191 219 254/var(--tw-border-opacity))}.border-gray-500{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.border-gray-600{--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}.border-red-400{--tw-border-opacity:1;border-color:rgb(248 113 113/var(--tw-border-opacity))}.border-zinc-100\/50{border-color:hsla(240,5%,96%,.5)}.border-zinc-500{--tw-border-opacity:1;border-color:rgb(113 113 122/var(--tw-border-opacity))}.border-b-gray-500{--tw-border-opacity:1;border-bottom-color:rgb(107 114 128/var(--tw-border-opacity))}.bg-amber-100\/40{background-color:hsla(48,96%,89%,.4)}.bg-amber-200{--tw-bg-opacity:1;background-color:rgb(253 230 138/var(--tw-bg-opacity))}.bg-blue-300{--tw-bg-opacity:1;background-color:rgb(147 197 253/var(--tw-bg-opacity))}.bg-green-100\/40{background-color:rgba(220,252,231,.4)}.bg-red-400{--tw-bg-opacity:1;background-color:rgb(248 113 113/var(--tw-bg-opacity))}.bg-zinc-500{--tw-bg-opacity:1;background-color:rgb(113 113 122/var(--tw-bg-opacity))}.bg-zinc-700{--tw-bg-opacity:1;background-color:rgb(63 63 70/var(--tw-bg-opacity))}.p-3{padding:.75rem}.p-4{padding:1rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-3{padding-left:.75rem;padding-right:.75rem}.px-4{padding-left:1rem;padding-right:1rem}.py-0{padding-bottom:0;padding-top:0}.py-0\.5{padding-bottom:.125rem;padding-top:.125rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.pt-1{padding-top:.25rem}.text-left{text-align:left}.text-center{text-align:center}.text-right{text-align:right}.align-middle{vertical-align:middle}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.uppercase{text-transform:uppercase}.lowercase{text-transform:lowercase}.text-amber-100{--tw-text-opacity:1;color:rgb(254 243 199/var(--tw-text-opacity))}.text-amber-200{--tw-text-opacity:1;color:rgb(253 230 138/var(--tw-text-opacity))}.text-amber-900{--tw-text-opacity:1;color:rgb(120 53 15/var(--tw-text-opacity))}.text-blue-200{--tw-text-opacity:1;color:rgb(191 219 254/var(--tw-text-opacity))}.text-blue-300{--tw-text-opacity:1;color:rgb(147 197 253/var(--tw-text-opacity))}.text-blue-900{--tw-text-opacity:1;color:rgb(30 58 138/var(--tw-text-opacity))}.text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.text-green-50{--tw-text-opacity:1;color:rgb(240 253 244/var(--tw-text-opacity))}.text-red-400{--tw-text-opacity:1;color:rgb(248 113 113/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.text-zinc-100\/90{color:hsla(240,5%,96%,.9)}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}table.dataframe{max-width:100%;overflow:auto;width:100%}.dataframe tr{border-bottom:1px solid #555}.dataframe td,.dataframe th{padding:.5rem}.dataframe th{text-align:left!important}.first\:border-t:first-child{border-top-width:1px}.hover\:border-zinc-500:hover{--tw-border-opacity:1;border-color:rgb(113 113 122/var(--tw-border-opacity))}.hover\:bg-zinc-400:hover{--tw-bg-opacity:1;background-color:rgb(161 161 170/var(--tw-bg-opacity))}.hover\:bg-zinc-500:hover{--tw-bg-opacity:1;background-color:rgb(113 113 122/var(--tw-bg-opacity))}.hover\:bg-zinc-700:hover{--tw-bg-opacity:1;background-color:rgb(63 63 70/var(--tw-bg-opacity))}.hover\:text-white:hover{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.group.open .group-\[\.open\]\:inline-block{display:inline-block}.group.open .group-\[\.open\]\:hidden{display:none}.group.active .group-\[\.active\]\:border-gray-500{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.group.active .group-\[\.active\]\:border-b-zinc-800{--tw-border-opacity:1;border-bottom-color:rgb(39 39 42/var(--tw-border-opacity))}.group.active .group-\[\.active\]\:bg-zinc-800{--tw-bg-opacity:1;background-color:rgb(39 39 42/var(--tw-bg-opacity))}.peer.open~.peer-\[\.open\]\:visible{visibility:visible}:is(.dark .dark\:bg-zinc-800){--tw-bg-opacity:1;background-color:rgb(39 39 42/var(--tw-bg-opacity))}:is(.dark .dark\:bg-zinc-900){--tw-bg-opacity:1;background-color:rgb(24 24 27/var(--tw-bg-opacity))}:is(.dark .dark\:fill-white){fill:#fff}:is(.dark .dark\:text-white){--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}
```

### Comparing `giskard-2.0.0b8/giskard/scanner/visualization/custom_jinja.py` & `giskard-2.0.0b9/giskard/scanner/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/settings.py` & `giskard-2.0.0b9/giskard/settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/slicing/base.py` & `giskard-2.0.0b9/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/slicing/bruteforce_slicer.py` & `giskard-2.0.0b9/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/slicing/category_slicer.py` & `giskard-2.0.0b9/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/slicing/multiscale_slicer.py` & `giskard-2.0.0b9/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/slicing/opt_slicer.py` & `giskard-2.0.0b9/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/slicing/slice.py` & `giskard-2.0.0b9/giskard/slicing/slice.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/slicing/stop_words.py` & `giskard-2.0.0b9/giskard/slicing/stop_words.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/slicing/text_slicer.py` & `giskard-2.0.0b9/giskard/slicing/text_slicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,20 +73,22 @@
 
         # Convert slices from metadata to original dataset
         slices = [MetadataSliceFunction(s.query, feature, "text") for s in slices]
 
         return slices
 
     def find_token_based_slices(self, feature, target):
+        target_is_numeric = pd.api.types.is_numeric_dtype(self.dataset.df[target])
         try:
-            tokens = set(
-                self._get_high_loss_tokens(feature, target)
-                + self._get_deviant_tokens(feature, target)
-                + self._get_top_tokens(feature, target)
-            )
+            tokens = self._get_top_tokens(feature, target)
+
+            if target_is_numeric:
+                tokens += self._get_high_loss_tokens(feature, target) + self._get_deviant_tokens(feature, target)
+
+            tokens = set(tokens)
         except VectorizerError:
             # Could not get meaningful tokens (e.g. all stop words)
             warning(f"Could not get meaningful tokens for textual feature `{feature}`. Are you sure this is text?")
             return []
 
         return [QueryBasedSliceFunction(Query([ContainsWord(feature, token)])) for token in tokens]
```

### Comparing `giskard-2.0.0b8/giskard/slicing/tree_slicer.py` & `giskard-2.0.0b9/giskard/slicing/tree_slicer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import logging
 import numpy as np
+import pandas as pd
 from scipy import stats
 from typing import Optional, Sequence
-from sklearn.tree import DecisionTreeRegressor
+from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.tree._tree import Tree as SklearnTree
 from sklearn.model_selection import GridSearchCV
 
 from .base import BaseSlicer
 from .slice import Query, LowerThan, GreaterThan, QueryBasedSliceFunction
 
 
+logger = logging.getLogger(__name__)
+
+
 def make_slices_from_tree(tree: SklearnTree, feature_names: Optional[Sequence] = None):
     """Builds data slices from a decision tree."""
     node_clauses = np.empty(tree.node_count, dtype=list)
     node_clauses[0] = []
 
     queue = [0]
     while queue:
@@ -50,45 +54,52 @@
         data = data.loc[:, features + [target]].dropna()
 
         min_samples = max(int(0.01 * len(data)), 30)  # min 1% of the data or 30 samples
 
         if len(data) < min_samples:
             return []
 
-        criterion = self._choose_tree_criterion(data.loc[:, target].values)
-
-        logging.debug(f"Using `{criterion}` criterion")
+        if pd.api.types.is_numeric_dtype(data[target]):
+            logger.debug("Target is numeric, using regression tree.")
+            criterion = self._choose_tree_criterion(data.loc[:, target].values)
+            logger.debug(f"Using `{criterion}` criterion.")
+
+            data_var = data.loc[:, target].var()
+
+            dt = DecisionTreeRegressor(
+                criterion=criterion,
+                splitter="best",
+                min_samples_leaf=min_samples,
+                max_leaf_nodes=20,
+            )
+            gs = GridSearchCV(
+                dt,
+                {
+                    # impurity in this case refers to the regression criterion
+                    "min_impurity_decrease": np.linspace(data_var / 100, data_var / 10, 10)
+                },
+            )
+        else:
+            logger.debug("Target is not numeric, using a classification tree.")
+            dt = DecisionTreeClassifier(
+                criterion="gini",
+                splitter="best",
+                min_samples_leaf=min_samples,
+                max_leaf_nodes=20,
+            )
+            gs = GridSearchCV(dt, {"min_impurity_decrease": np.linspace(0.001, 0.1, 10)})
 
-        data_var = data.loc[:, target].var()
-
-        dt = DecisionTreeRegressor(
-            criterion=criterion,
-            splitter="best",
-            min_samples_leaf=min_samples,
-            max_leaf_nodes=20,
-        )
-        gs = GridSearchCV(
-            dt,
-            {
-                # impurity in this case refers to the regression criterion
-                "min_impurity_decrease": np.linspace(data_var / 100, data_var / 10, 10)
-            },
-        )
         gs.fit(data.loc[:, features], data.loc[:, target])
         dt = gs.best_estimator_
 
         # Need at least a split, otherwise return now.
         if dt.tree_.node_count < 2:
-            logging.debug("No split found, stopping now.")
+            logger.debug("No split found, stopping now.")
             return []
 
-        # Debugging info
-        corr = stats.pearsonr(data.loc[:, target], dt.predict(data.loc[:, features]))[0]
-        logging.debug(f"Decision tree target correlation: {corr:.2f}")
-
         # Make test slices
         slice_candidates = make_slices_from_tree(dt.tree_, features)
 
         return slice_candidates
 
     def _choose_tree_criterion(self, target_samples: np.ndarray):
         norm_ks_stat = stats.kstest(target_samples, "norm").statistic
```

### Comparing `giskard-2.0.0b8/giskard/slicing/utils.py` & `giskard-2.0.0b9/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/testing/__init__.py` & `giskard-2.0.0b9/giskard/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/testing/tests/drift.py` & `giskard-2.0.0b9/giskard/testing/tests/drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/testing/tests/metamorphic.py` & `giskard-2.0.0b9/giskard/testing/tests/metamorphic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/testing/tests/performance.py` & `giskard-2.0.0b9/giskard/testing/tests/performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/testing/tests/statistic.py` & `giskard-2.0.0b9/giskard/testing/tests/statistic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard/utils/analytics_collector.py` & `giskard-2.0.0b9/giskard/utils/analytics_collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,31 +48,41 @@
 
 def get_model_properties(model):
     from ..models.base import WrapperModel
 
     if model is None:
         return {}
 
-    inner_model_class = fullname(model.model) if isinstance(model, WrapperModel) else None
-    feature_names = [anonymize(n) for n in model.meta.feature_names]
+    inner_model_class = (
+        fullname(model.model) if isinstance(model, WrapperModel) else None
+    )
+    feature_names = (
+        [anonymize(n) for n in model.meta.feature_names]
+        if model.meta.feature_names
+        else None
+    )
 
     return {
         "model_id": str(model.id),
         "model_type": model.meta.model_type.value,
         "model_class": fullname(model),
         "model_inner_class": inner_model_class,
         "model_feature_names": feature_names,
     }
 
 
 def get_dataset_properties(dataset):
     if dataset is None:
         return {}
 
-    column_types = {anonymize(k): v for k, v in dataset.column_types.items()} if dataset.column_types else {}
+    column_types = (
+        {anonymize(k): v for k, v in dataset.column_types.items()}
+        if dataset.column_types
+        else {}
+    )
     column_dtypes = {anonymize(k): v for k, v in dataset.column_dtypes.items()}
 
     return {
         "dataset_id": str(dataset.id) if dataset is not None else "none",
         "dataset_rows": dataset.df.shape[0],
         "dataset_cols": dataset.df.shape[1],
         "dataset_column_types": column_types,
@@ -117,15 +127,19 @@
         if self.is_enabled:
             self.mp = self.configure_mixpanel()
             self.distinct_user_id = GiskardAnalyticsCollector.machine_based_user_id()
 
     @staticmethod
     @analytics_method
     def configure_mixpanel() -> Mixpanel:
-        is_dev_mode = os.environ.get("GISKARD_DEV_MODE", "n").lower() in ["yes", "true", "1"]
+        is_dev_mode = os.environ.get("GISKARD_DEV_MODE", "n").lower() in [
+            "yes",
+            "true",
+            "1",
+        ]
 
         return Mixpanel(
             GiskardAnalyticsCollector.dev_mp_project_key
             if is_dev_mode
             else GiskardAnalyticsCollector.prod_mp_project_key
         )
 
@@ -154,15 +168,18 @@
             }
             if properties is not None:
                 merged_props = {**merged_props, **properties}
             if self.server_info is not None:
                 merged_props = {**merged_props, **self.server_info}
 
             self.mp.track(
-                distinct_id=self.distinct_user_id, event_name=event_name, properties=dict(merged_props), meta=meta
+                distinct_id=self.distinct_user_id,
+                event_name=event_name,
+                properties=dict(merged_props),
+                meta=meta,
             )
 
     def initialize_giskard_version(self):
         if not self.giskard_version:
             import giskard
 
             self.giskard_version = giskard.get_version()
@@ -197,15 +214,22 @@
         IP address itself **isn't stored** by in the telemetry data, see:
         https://docs.mixpanel.com/docs/tracking/how-tos/effective-server#tracking-geolocation
         """
         with GiskardAnalyticsCollector.lock:
             if self.ip:
                 return
             try:
-                self.ip = requests.get("https://api64.ipify.org/?format=json").json().get("ip", "unknown")
+                self.ip = (
+                    requests.get(
+                        "http://ip-api.com/json",  # noqa NOSONAR - we don't care about security here
+                        timeout=(2, 2),
+                    )
+                    .json()
+                    .get("ip", "unknown")
+                )
             except:  # noqa NOSONAR
                 self.ip = "unknown"
 
 
 def add_exception_hook(original_hook=None):
     def _exception_hook(type, value, traceback):
         try:
```

### Comparing `giskard-2.0.0b8/giskard/utils/environment_detector.py` & `giskard-2.0.0b9/giskard/utils/environment_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/giskard.egg-info/PKG-INFO` & `giskard-2.0.0b9/giskard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b8 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b9 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
```

### Comparing `giskard-2.0.0b8/giskard.egg-info/SOURCES.txt` & `giskard-2.0.0b9/giskard.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 giskard/datasets/__init__.py
 giskard/datasets/base/__init__.py
 giskard/datasets/metadata/__init__.py
 giskard/datasets/metadata/indexing.py
 giskard/datasets/metadata/registry.py
 giskard/datasets/metadata/text_metadata_provider.py
 giskard/demo/__init__.py
+giskard/demo/linear_regression.py
 giskard/demo/titanic.csv
+giskard/demo/titanic_classification.py
 giskard/ml_worker/__init__.py
 giskard/ml_worker/ml_worker.py
 giskard/ml_worker/bridge/data_encryptor.py
 giskard/ml_worker/bridge/error.py
 giskard/ml_worker/bridge/ml_worker_bridge.py
 giskard/ml_worker/bridge/service_messages.py
 giskard/ml_worker/core/log_listener.py
@@ -93,14 +95,15 @@
 giskard/scanner/result.py
 giskard/scanner/scanner.py
 giskard/scanner/calibration/issues.py
 giskard/scanner/calibration/overconfidence_detector.py
 giskard/scanner/calibration/underconfidence_detector.py
 giskard/scanner/common/examples.py
 giskard/scanner/common/loss_based_detector.py
+giskard/scanner/correlation/spurious_correlation_detector.py
 giskard/scanner/data_leakage/data_leakage_detector.py
 giskard/scanner/llm/toxicity_detector.py
 giskard/scanner/llm/utils.py
 giskard/scanner/performance/__init__.py
 giskard/scanner/performance/issues.py
 giskard/scanner/performance/metrics.py
 giskard/scanner/performance/performance_bias_detector.py
@@ -120,34 +123,37 @@
 giskard/scanner/templates/scan_results.html
 giskard/scanner/templates/_issues/data_leakage.html
 giskard/scanner/templates/_issues/default.html
 giskard/scanner/templates/_issues/llm_toxicity.html
 giskard/scanner/templates/_issues/overconfidence.html
 giskard/scanner/templates/_issues/performance.html
 giskard/scanner/templates/_issues/robustness.html
+giskard/scanner/templates/_issues/spurious_correlation.html
 giskard/scanner/templates/_issues/stochasticity.html
 giskard/scanner/templates/_issues/underconfidence.html
 giskard/scanner/templates/static/external.js
 giskard/scanner/templates/static/internal.js
 giskard/scanner/templates/static/style.css
 giskard/scanner/visualization/__init__.py
 giskard/scanner/visualization/custom_jinja.py
 giskard/slicing/__init__.py
 giskard/slicing/base.py
 giskard/slicing/bruteforce_slicer.py
 giskard/slicing/category_slicer.py
 giskard/slicing/multiscale_slicer.py
 giskard/slicing/opt_slicer.py
 giskard/slicing/slice.py
+giskard/slicing/slice_finder.py
 giskard/slicing/stop_words.py
 giskard/slicing/text_slicer.py
 giskard/slicing/tree_slicer.py
 giskard/slicing/utils.py
 giskard/testing/__init__.py
 giskard/testing/tests/__init__.py
+giskard/testing/tests/calibration.py
 giskard/testing/tests/drift.py
 giskard/testing/tests/metamorphic.py
 giskard/testing/tests/performance.py
 giskard/testing/tests/statistic.py
 giskard/utils/__init__.py
 giskard/utils/analytics_collector.py
 giskard/utils/display.py
```

### Comparing `giskard-2.0.0b8/giskard.egg-info/requires.txt` & `giskard-2.0.0b9/giskard.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 jinja2>=3
 requests-toolbelt>=0.9.1
 
 [llm]
 transformers
 torch
 langchain
-datasets
 evaluate
-bert_score
+datasets>=2.13.0
+bert-score>=0.3.13
 
 [server]
 tenacity>=4.11.0
 psutil>=5.4.6
 click>=7.0
 docker>=6.0.0
 shap>=0.41.0
```

### Comparing `giskard-2.0.0b8/pyproject.toml` & `giskard-2.0.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     "sphinx-autoapi>=2.1.0",
     "sphinx-rtd-theme>=1.2.0",
     "sphinx-tabs>=3.4.1",
     "sphinx-design>=0.4.1",
     "sphinx-copybutton>=0.5.2",
     "sphinx-click>=4.4.0",
     "nbsphinx>=0.9.2",
-    "sphinx-favicon>=1.0.1",
 ]
 
 [tool.setuptools.packages.find]
 include = ["giskard*"]
 exclude = ["docs*", "tests*"]
 
 [tool.setuptools.package-data]
@@ -104,15 +103,15 @@
 "Twitter" = "https://twitter.com/giskard_ai"
 
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.0.0b8"
+version = "2.0.0b9"
 description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [
     { name = "Giskard AI", email = "hello@giskard.ai" },
 ]
 keywords = [
     "Artificial Intelligence",
     "Machine Learning",
@@ -155,17 +154,18 @@
 ]
 
 [project.optional-dependencies]
 llm = [
     "transformers",
     "torch",
     "langchain",
-    "datasets",
     "evaluate",
-    "bert_score",
+#    pdm lock -G:all doesn't work without fixing these two versions
+    "datasets>=2.13.0",
+    "bert-score>=0.3.13",
 ]
 server = [
     "tenacity>=4.11.0",
     "psutil>=5.4.6",
     "click>=7.0",
     "docker>=6.0.0",
     "shap>=0.41.0",
```

### Comparing `giskard-2.0.0b8/setup.py` & `giskard-2.0.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_custom_model.py` & `giskard-2.0.0b9/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_data_drift.py` & `giskard-2.0.0b9/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_data_processing_pipeline.py` & `giskard-2.0.0b9/tests/test_data_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_dataset.py` & `giskard-2.0.0b9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_metamorphic_direction.py` & `giskard-2.0.0b9/tests/test_metamorphic_direction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_metamorphic_invariance.py` & `giskard-2.0.0b9/tests/test_metamorphic_invariance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_model.py` & `giskard-2.0.0b9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_model_auto_inference.py` & `giskard-2.0.0b9/tests/test_model_auto_inference.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_model_explanation.py` & `giskard-2.0.0b9/tests/test_model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_model_postprocess.py` & `giskard-2.0.0b9/tests/test_model_postprocess.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_performance.py` & `giskard-2.0.0b9/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_programmatic.py` & `giskard-2.0.0b9/tests/test_programmatic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 
 from giskard import test, scan
 from giskard.core.suite import Suite, SuiteInput
 from giskard.datasets.base import Dataset
-from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
+from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction, slicing_function
+from giskard.ml_worker.testing.test_result import TestMessageLevel
 from giskard.models.base import BaseModel
 from giskard.testing.tests.performance import test_auc, test_f1, test_diff_f1
 
 
 @test()
 def _test_a_greater_b(a: int, b: int):
     return a > b
@@ -105,14 +106,34 @@
     assert (
         Suite()
         .add_test(test_auc(dataset=shared_input, threshold=0.2))
         .run(model=german_credit_model, dataset=german_credit_data)[0]
     )
 
 
+def test_execution_error(german_credit_data: Dataset, german_credit_model: BaseModel):
+    shared_input = SuiteInput("dataset", Dataset)
+
+    @slicing_function(row_level=False)
+    def empty_slice(x):
+        return x.iloc[[]]
+
+    result = Suite().add_test(test_f1(dataset=shared_input, threshold=0.2, slicing_function=empty_slice)) \
+        .add_test(test_f1(dataset=shared_input, threshold=0.2)) \
+        .run(model=german_credit_model, dataset=german_credit_data)
+
+    assert result[0] is False
+    assert result[1][0][1].passed is False
+    assert result[1][0][1].is_error is True
+    assert result[1][0][1].messages[0].type is TestMessageLevel.ERROR
+    assert 'The sliced dataset in test_f1 is empty.' in result[1][0][1].messages[0].text
+    assert result[1][1][1].passed is True
+    assert result[1][1][1].is_error is False
+
+
 def test_save_suite(german_credit_data: Dataset, german_credit_model: BaseModel):
     # with MockedClient() as (client, mr):
     #     Suite().add_test(test_auc(threshold=0.2, dataset=german_credit_data)).add_test(
     #         test_f1(threshold=0.2, dataset=german_credit_data)
     #     ).upload(client, "test_project_key")
     scan(german_credit_model, german_credit_data)
```

### Comparing `giskard-2.0.0b8/tests/test_project_uploads.py` & `giskard-2.0.0b9/tests/test_project_uploads.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_statistical.py` & `giskard-2.0.0b9/tests/test_statistical.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b8/tests/test_upload.py` & `giskard-2.0.0b9/tests/test_upload.py`

 * *Files identical despite different names*

