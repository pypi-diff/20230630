# Comparing `tmp/triton_model_navigator-0.5.6-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,135 +1,147 @@
-Zip file size: 234262 bytes, number of entries: 133
--rw-r--r--  2.0 unx      881 b- defN 23-Jun-22 17:26 model_navigator/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-Jun-23 10:40 model_navigator/__version__.py
--rw-r--r--  2.0 unx     3668 b- defN 23-Jun-23 01:05 model_navigator/exceptions.py
--rw-r--r--  2.0 unx     9474 b- defN 23-Jun-23 01:05 model_navigator/execution_context.py
--rw-r--r--  2.0 unx     4790 b- defN 23-Jun-23 01:05 model_navigator/logger.py
--rw-rw-rw-  2.0 unx     1716 b- defN 23-Jun-23 10:40 model_navigator/api/__init__.py
--rw-rw-rw-  2.0 unx    24304 b- defN 23-Jun-23 10:40 model_navigator/api/config.py
--rw-rw-rw-  2.0 unx     6425 b- defN 23-Jun-23 10:40 model_navigator/api/jax.py
--rw-rw-rw-  2.0 unx     5423 b- defN 23-Jun-23 10:40 model_navigator/api/onnx.py
--rw-rw-rw-  2.0 unx    11860 b- defN 23-Jun-23 10:40 model_navigator/api/package.py
--rw-rw-rw-  2.0 unx     4906 b- defN 23-Jun-23 10:40 model_navigator/api/python.py
--rw-rw-rw-  2.0 unx     7748 b- defN 23-Jun-23 01:05 model_navigator/api/pytriton.py
--rw-rw-rw-  2.0 unx     6519 b- defN 23-Jun-23 10:40 model_navigator/api/tensorflow.py
--rw-rw-rw-  2.0 unx     6325 b- defN 23-Jun-23 10:40 model_navigator/api/torch.py
--rw-r--r--  2.0 unx     1553 b- defN 23-Jun-22 17:26 model_navigator/api/triton.py
--rw-r--r--  2.0 unx     1811 b- defN 23-Jun-22 17:26 model_navigator/api/utilities.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/__init__.py
--rw-rw-rw-  2.0 unx     4938 b- defN 23-Jun-23 01:05 model_navigator/commands/base.py
--rw-rw-rw-  2.0 unx    10065 b- defN 23-Jun-23 10:40 model_navigator/commands/infer_metadata.py
--rw-rw-rw-  2.0 unx     3289 b- defN 23-Jun-23 01:05 model_navigator/commands/load.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/__init__.py
--rw-rw-rw-  2.0 unx     9863 b- defN 23-Jun-23 01:05 model_navigator/commands/convert/base.py
--rw-rw-rw-  2.0 unx     7489 b- defN 23-Jun-23 10:40 model_navigator/commands/convert/tf.py
--rw-rw-rw-  2.0 unx     9879 b- defN 23-Jun-23 10:40 model_navigator/commands/convert/torch.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/converters/__init__.py
--rw-r--r--  2.0 unx     3418 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/converters/ts2onnx.py
--rw-r--r--  2.0 unx     4992 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-r--r--  2.0 unx      680 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/onnx/__init__.py
--rw-r--r--  2.0 unx     1727 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-rw-rw-  2.0 unx    10643 b- defN 23-Jun-23 10:40 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-r--r--  2.0 unx     2235 b- defN 23-Jun-22 17:26 model_navigator/commands/convert/onnx/trt_load_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/copy/__init__.py
--rw-rw-rw-  2.0 unx     1729 b- defN 23-Jun-23 01:05 model_navigator/commands/copy/onnx.py
--rw-r--r--  2.0 unx      678 b- defN 23-Jun-22 17:26 model_navigator/commands/correctness/__init__.py
--rw-rw-rw-  2.0 unx     5594 b- defN 23-Jun-23 01:05 model_navigator/commands/correctness/correctness.py
--rw-rw-rw-  2.0 unx     4550 b- defN 23-Jun-23 01:05 model_navigator/commands/correctness/correctness_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/data_dump/__init__.py
--rw-rw-rw-  2.0 unx    11162 b- defN 23-Jun-23 10:40 model_navigator/commands/data_dump/samples.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/export/__init__.py
--rw-rw-rw-  2.0 unx     3531 b- defN 23-Jun-23 01:05 model_navigator/commands/export/jax.py
--rw-rw-rw-  2.0 unx     5485 b- defN 23-Jun-23 01:05 model_navigator/commands/export/tf.py
--rw-rw-rw-  2.0 unx     9043 b- defN 23-Jun-23 01:05 model_navigator/commands/export/torch.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/__init__.py
--rw-r--r--  2.0 unx     3945 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-r--r--  2.0 unx     3171 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-r--r--  2.0 unx     3122 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/torch2onnx.py
--rw-r--r--  2.0 unx     2728 b- defN 23-Jun-22 17:26 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-r--r--  2.0 unx      715 b- defN 23-Jun-22 17:26 model_navigator/commands/find_max_batch_size/__init__.py
--rw-rw-rw-  2.0 unx     6396 b- defN 23-Jun-23 10:40 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-rw-rw-  2.0 unx     2984 b- defN 23-Jun-23 10:40 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-rw-rw-  2.0 unx      688 b- defN 23-Jun-23 01:05 model_navigator/commands/performance/__init__.py
--rw-rw-rw-  2.0 unx    15770 b- defN 23-Jun-23 10:40 model_navigator/commands/performance/performance.py
--rw-rw-rw-  2.0 unx     3037 b- defN 23-Jun-23 10:40 model_navigator/commands/performance/performance_script.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/commands/verification/__init__.py
--rw-rw-rw-  2.0 unx     5441 b- defN 23-Jun-23 01:05 model_navigator/commands/verification/verify.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/configuration/__init__.py
--rw-rw-rw-  2.0 unx     2473 b- defN 23-Jun-23 10:40 model_navigator/configuration/common_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/configuration/model/__init__.py
--rw-rw-rw-  2.0 unx    15623 b- defN 23-Jun-23 01:05 model_navigator/configuration/model/model_config.py
--rw-r--r--  2.0 unx    13677 b- defN 23-Jun-22 17:26 model_navigator/configuration/model/model_config_builder.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/core/__init__.py
--rw-rw-rw-  2.0 unx     1326 b- defN 23-Jun-23 10:40 model_navigator/core/constants.py
--rw-rw-rw-  2.0 unx    20111 b- defN 23-Jun-23 10:40 model_navigator/core/package.py
--rw-rw-rw-  2.0 unx    20337 b- defN 23-Jun-23 10:40 model_navigator/core/status.py
--rw-rw-rw-  2.0 unx     8052 b- defN 23-Jun-23 10:40 model_navigator/core/tensor.py
--rw-r--r--  2.0 unx     2817 b- defN 23-Jun-22 17:26 model_navigator/frameworks/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-Jun-22 17:26 model_navigator/frameworks/jax/__init__.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jun-22 17:26 model_navigator/frameworks/jax/model.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/frameworks/onnx/__init__.py
--rw-r--r--  2.0 unx     1085 b- defN 23-Jun-22 17:26 model_navigator/frameworks/onnx/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/frameworks/tensorrt/__init__.py
--rw-rw-rw-  2.0 unx    26575 b- defN 23-Jun-23 10:40 model_navigator/frameworks/tensorrt/cuda.py
--rw-rw-rw-  2.0 unx     9874 b- defN 23-Jun-23 10:40 model_navigator/frameworks/tensorrt/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/frameworks/torch/__init__.py
--rw-rw-rw-  2.0 unx     1508 b- defN 23-Jun-23 01:05 model_navigator/frameworks/torch/utils.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/pipelines/__init__.py
--rw-rw-rw-  2.0 unx     5685 b- defN 23-Jun-23 01:05 model_navigator/pipelines/pipeline.py
--rw-rw-rw-  2.0 unx     7333 b- defN 23-Jun-23 01:05 model_navigator/pipelines/pipeline_manager.py
--rw-rw-rw-  2.0 unx     9805 b- defN 23-Jun-23 10:40 model_navigator/pipelines/validation.py
--rw-rw-rw-  2.0 unx     1879 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/__init__.py
--rw-rw-rw-  2.0 unx     2036 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/correctness.py
--rw-rw-rw-  2.0 unx     5703 b- defN 23-Jun-23 10:40 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-rw-rw-  2.0 unx     1647 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/jax.py
--rw-rw-rw-  2.0 unx     2483 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/onnx.py
--rw-rw-rw-  2.0 unx     2365 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/preprocessing.py
--rw-rw-rw-  2.0 unx     2685 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/profiling.py
--rw-rw-rw-  2.0 unx     2869 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/tensorflow.py
--rw-rw-rw-  2.0 unx     3261 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/torch.py
--rw-rw-rw-  2.0 unx     2042 b- defN 23-Jun-23 01:05 model_navigator/pipelines/builders/verify.py
--rw-r--r--  2.0 unx     1584 b- defN 23-Jun-22 17:26 model_navigator/runners/__init__.py
--rw-rw-rw-  2.0 unx    11369 b- defN 23-Jun-23 10:40 model_navigator/runners/base.py
--rw-r--r--  2.0 unx     2620 b- defN 23-Jun-22 17:26 model_navigator/runners/jax.py
--rw-rw-rw-  2.0 unx     7302 b- defN 23-Jun-23 10:40 model_navigator/runners/onnx.py
--rw-r--r--  2.0 unx     2267 b- defN 23-Jun-22 17:26 model_navigator/runners/python.py
--rw-rw-rw-  2.0 unx     2285 b- defN 23-Jun-23 01:05 model_navigator/runners/registry.py
--rw-r--r--  2.0 unx     7976 b- defN 23-Jun-22 17:26 model_navigator/runners/tensorflow.py
--rw-rw-rw-  2.0 unx    25301 b- defN 23-Jun-23 10:40 model_navigator/runners/tensorrt.py
--rw-rw-rw-  2.0 unx     7699 b- defN 23-Jun-23 10:40 model_navigator/runners/torch.py
--rw-rw-rw-  2.0 unx     3554 b- defN 23-Jun-23 01:05 model_navigator/runners/utils.py
--rw-r--r--  2.0 unx      937 b- defN 23-Jun-22 17:26 model_navigator/runtime_analyzer/__init__.py
--rw-rw-rw-  2.0 unx    11706 b- defN 23-Jun-23 01:05 model_navigator/runtime_analyzer/analyzer.py
--rw-r--r--  2.0 unx     2304 b- defN 23-Jun-22 17:26 model_navigator/runtime_analyzer/strategy.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/triton/__init__.py
--rw-r--r--  2.0 unx     3180 b- defN 23-Jun-22 17:26 model_navigator/triton/model_config.py
--rw-r--r--  2.0 unx     5218 b- defN 23-Jun-22 17:26 model_navigator/triton/model_config_builder.py
--rw-r--r--  2.0 unx    23090 b- defN 23-Jun-22 17:26 model_navigator/triton/model_config_generator.py
--rw-rw-rw-  2.0 unx    15245 b- defN 23-Jun-23 10:40 model_navigator/triton/model_repository.py
--rw-r--r--  2.0 unx     2081 b- defN 23-Jun-22 17:26 model_navigator/triton/utils.py
--rw-r--r--  2.0 unx      944 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/__init__.py
--rw-r--r--  2.0 unx     2872 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/base_model_config.py
--rw-r--r--  2.0 unx    22326 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/common.py
--rw-r--r--  2.0 unx     2229 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/internal.py
--rw-r--r--  2.0 unx     2685 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-r--r--  2.0 unx     1785 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/python_model_config.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-r--r--  2.0 unx     3162 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Jun-22 17:26 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-22 17:26 model_navigator/utils/__init__.py
--rw-rw-rw-  2.0 unx    14113 b- defN 23-Jun-23 10:40 model_navigator/utils/common.py
--rw-rw-rw-  2.0 unx     8004 b- defN 23-Jun-23 10:40 model_navigator/utils/dataloader.py
--rw-r--r--  2.0 unx     3902 b- defN 23-Jun-22 17:26 model_navigator/utils/devices.py
--rw-r--r--  2.0 unx     1308 b- defN 23-Jun-22 17:26 model_navigator/utils/enums.py
--rw-r--r--  2.0 unx     6163 b- defN 23-Jun-22 17:26 model_navigator/utils/environment.py
--rw-rw-rw-  2.0 unx     3528 b- defN 23-Jun-23 01:05 model_navigator/utils/format_helpers.py
--rw-rw-rw-  2.0 unx     2325 b- defN 23-Jun-23 01:05 model_navigator/utils/module.py
--rw-rw-rw-  2.0 unx     3233 b- defN 23-Jun-23 01:05 model_navigator/utils/package.py
--rw-r--r--  2.0 unx    10140 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    12074 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    13271 b- defN 23-Jun-23 12:25 triton_model_navigator-0.5.6.dist-info/RECORD
-133 files, 704952 bytes uncompressed, 212626 bytes compressed:  69.8%
+Zip file size: 254299 bytes, number of entries: 145
+-rw-r--r--  2.0 unx      881 b- defN 23-Jun-28 12:15 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-Jun-28 12:15 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     3915 b- defN 23-Jun-28 12:15 model_navigator/exceptions.py
+-rw-rw-rw-  2.0 unx     1716 b- defN 23-Jun-28 12:15 model_navigator/api/__init__.py
+-rw-rw-rw-  2.0 unx    24220 b- defN 23-Jun-30 11:34 model_navigator/api/config.py
+-rw-rw-rw-  2.0 unx     6263 b- defN 23-Jun-30 11:34 model_navigator/api/jax.py
+-rw-rw-rw-  2.0 unx     5268 b- defN 23-Jun-30 11:34 model_navigator/api/onnx.py
+-rw-rw-rw-  2.0 unx    16279 b- defN 23-Jun-30 11:34 model_navigator/api/package.py
+-rw-rw-rw-  2.0 unx     4795 b- defN 23-Jun-28 12:15 model_navigator/api/python.py
+-rw-rw-rw-  2.0 unx     7751 b- defN 23-Jun-28 12:15 model_navigator/api/pytriton.py
+-rw-rw-rw-  2.0 unx     6350 b- defN 23-Jun-30 11:34 model_navigator/api/tensorflow.py
+-rw-rw-rw-  2.0 unx     6158 b- defN 23-Jun-30 11:34 model_navigator/api/torch.py
+-rw-rw-rw-  2.0 unx     1553 b- defN 23-Jun-28 12:15 model_navigator/api/triton.py
+-rw-rw-rw-  2.0 unx     1811 b- defN 23-Jun-28 12:15 model_navigator/api/utilities.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/__init__.py
+-rw-rw-rw-  2.0 unx     5542 b- defN 23-Jun-28 12:15 model_navigator/commands/base.py
+-rw-rw-rw-  2.0 unx     9486 b- defN 23-Jun-28 12:15 model_navigator/commands/execution_context.py
+-rw-rw-rw-  2.0 unx    12793 b- defN 23-Jun-28 12:15 model_navigator/commands/infer_metadata.py
+-rw-rw-rw-  2.0 unx     3325 b- defN 23-Jun-28 12:15 model_navigator/commands/load.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/__init__.py
+-rw-rw-rw-  2.0 unx     9868 b- defN 23-Jun-30 11:34 model_navigator/commands/convert/base.py
+-rw-rw-rw-  2.0 unx     7633 b- defN 23-Jun-30 11:34 model_navigator/commands/convert/tf.py
+-rw-rw-rw-  2.0 unx    10029 b- defN 23-Jun-30 11:34 model_navigator/commands/convert/torch.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/converters/__init__.py
+-rw-rw-rw-  2.0 unx     3418 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-rw-rw-  2.0 unx     3105 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-rw-rw-  2.0 unx     4992 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-rw-rw-  2.0 unx      680 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/onnx/__init__.py
+-rw-rw-rw-  2.0 unx     1727 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-rw-rw-  2.0 unx    10733 b- defN 23-Jun-30 11:34 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-rw-rw-  2.0 unx     2235 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/onnx/trt_load_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/copy/__init__.py
+-rw-rw-rw-  2.0 unx     1798 b- defN 23-Jun-28 12:15 model_navigator/commands/copy/onnx.py
+-rw-rw-rw-  2.0 unx      678 b- defN 23-Jun-28 12:15 model_navigator/commands/correctness/__init__.py
+-rw-rw-rw-  2.0 unx     5674 b- defN 23-Jun-28 12:15 model_navigator/commands/correctness/correctness.py
+-rw-rw-rw-  2.0 unx     4733 b- defN 23-Jun-28 15:05 model_navigator/commands/correctness/correctness_script.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/data_dump/__init__.py
+-rw-rw-rw-  2.0 unx    10740 b- defN 23-Jun-28 12:15 model_navigator/commands/data_dump/samples.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/export/__init__.py
+-rw-rw-rw-  2.0 unx     3611 b- defN 23-Jun-28 12:15 model_navigator/commands/export/jax.py
+-rw-rw-rw-  2.0 unx     5598 b- defN 23-Jun-28 12:15 model_navigator/commands/export/tf.py
+-rw-rw-rw-  2.0 unx     9156 b- defN 23-Jun-28 12:15 model_navigator/commands/export/torch.py
+-rw-rw-rw-  2.0 unx     1056 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/__init__.py
+-rw-rw-rw-  2.0 unx     3945 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-rw-rw-  2.0 unx     3171 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-rw-rw-  2.0 unx     3122 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-rw-rw-  2.0 unx     3077 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-rw-rw-  2.0 unx     2728 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-rw-rw-  2.0 unx      715 b- defN 23-Jun-28 12:15 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-rw-rw-  2.0 unx     7156 b- defN 23-Jun-28 12:15 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-rw-rw-  2.0 unx     3075 b- defN 23-Jun-28 12:15 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-rw-rw-  2.0 unx      784 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/__init__.py
+-rw-rw-rw-  2.0 unx     5260 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/performance.py
+-rw-rw-rw-  2.0 unx     6964 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/profile.py
+-rw-rw-rw-  2.0 unx     3104 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/profile_script.py
+-rw-rw-rw-  2.0 unx     7269 b- defN 23-Jun-28 15:05 model_navigator/commands/performance/profiler.py
+-rw-rw-rw-  2.0 unx     5476 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/results.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/verification/__init__.py
+-rw-rw-rw-  2.0 unx     4657 b- defN 23-Jun-28 12:15 model_navigator/commands/verification/verify.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/configuration/__init__.py
+-rw-rw-rw-  2.0 unx     2002 b- defN 23-Jun-28 12:15 model_navigator/configuration/common_config.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/configuration/model/__init__.py
+-rw-rw-rw-  2.0 unx    15653 b- defN 23-Jun-30 11:34 model_navigator/configuration/model/model_config.py
+-rw-rw-rw-  2.0 unx    13677 b- defN 23-Jun-30 11:34 model_navigator/configuration/model/model_config_builder.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/core/__init__.py
+-rw-rw-rw-  2.0 unx     1389 b- defN 23-Jun-30 11:34 model_navigator/core/constants.py
+-rw-rw-rw-  2.0 unx     5299 b- defN 23-Jun-28 12:15 model_navigator/core/logger.py
+-rw-rw-rw-  2.0 unx     9941 b- defN 23-Jun-28 12:15 model_navigator/core/tensor.py
+-rw-rw-rw-  2.0 unx     2147 b- defN 23-Jun-28 12:15 model_navigator/core/workspace.py
+-rw-rw-rw-  2.0 unx     2817 b- defN 23-Jun-28 12:15 model_navigator/frameworks/__init__.py
+-rw-rw-rw-  2.0 unx      669 b- defN 23-Jun-28 12:15 model_navigator/frameworks/jax/__init__.py
+-rw-rw-rw-  2.0 unx     1554 b- defN 23-Jun-28 12:15 model_navigator/frameworks/jax/model.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/frameworks/onnx/__init__.py
+-rw-rw-rw-  2.0 unx     1085 b- defN 23-Jun-28 12:15 model_navigator/frameworks/onnx/utils.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/frameworks/tensorrt/__init__.py
+-rw-rw-rw-  2.0 unx    27191 b- defN 23-Jun-28 12:15 model_navigator/frameworks/tensorrt/cuda.py
+-rw-rw-rw-  2.0 unx    10627 b- defN 23-Jun-30 11:34 model_navigator/frameworks/tensorrt/utils.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/frameworks/torch/__init__.py
+-rw-rw-rw-  2.0 unx     1513 b- defN 23-Jun-28 12:15 model_navigator/frameworks/torch/utils.py
+-rw-rw-rw-  2.0 unx      622 b- defN 23-Jun-28 12:15 model_navigator/package/__init__.py
+-rw-rw-rw-  2.0 unx    12176 b- defN 23-Jun-28 13:04 model_navigator/package/builder.py
+-rw-rw-rw-  2.0 unx     4651 b- defN 23-Jun-28 12:15 model_navigator/package/loader.py
+-rw-rw-rw-  2.0 unx    11755 b- defN 23-Jun-28 15:05 model_navigator/package/package.py
+-rw-rw-rw-  2.0 unx     2819 b- defN 23-Jun-28 12:15 model_navigator/package/profiling_results.py
+-rw-rw-rw-  2.0 unx    21135 b- defN 23-Jun-30 11:34 model_navigator/package/status.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/pipelines/__init__.py
+-rw-rw-rw-  2.0 unx     5232 b- defN 23-Jun-28 12:15 model_navigator/pipelines/pipeline.py
+-rw-rw-rw-  2.0 unx    14762 b- defN 23-Jun-28 12:15 model_navigator/pipelines/pipeline_context.py
+-rw-rw-rw-  2.0 unx     3832 b- defN 23-Jun-28 12:15 model_navigator/pipelines/pipeline_manager.py
+-rw-rw-rw-  2.0 unx     9693 b- defN 23-Jun-30 11:34 model_navigator/pipelines/validation.py
+-rw-rw-rw-  2.0 unx     1883 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/__init__.py
+-rw-rw-rw-  2.0 unx     2106 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/correctness.py
+-rw-rw-rw-  2.0 unx     5682 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-rw-rw-  2.0 unx     1660 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/jax.py
+-rw-rw-rw-  2.0 unx     2509 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/onnx.py
+-rw-rw-rw-  2.0 unx     2516 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/performance.py
+-rw-rw-rw-  2.0 unx     2239 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/preprocessing.py
+-rw-rw-rw-  2.0 unx     2504 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/profiling.py
+-rw-rw-rw-  2.0 unx     2921 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/tensorflow.py
+-rw-rw-rw-  2.0 unx     3326 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/torch.py
+-rw-rw-rw-  2.0 unx     2112 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/verify.py
+-rw-rw-rw-  2.0 unx      622 b- defN 23-Jun-28 12:15 model_navigator/pipelines/wrappers/__init__.py
+-rw-rw-rw-  2.0 unx     2747 b- defN 23-Jun-28 12:15 model_navigator/pipelines/wrappers/optimize.py
+-rw-rw-rw-  2.0 unx     4881 b- defN 23-Jun-28 12:15 model_navigator/pipelines/wrappers/profile.py
+-rw-rw-rw-  2.0 unx     1584 b- defN 23-Jun-28 12:15 model_navigator/runners/__init__.py
+-rw-rw-rw-  2.0 unx    13796 b- defN 23-Jun-28 12:15 model_navigator/runners/base.py
+-rw-rw-rw-  2.0 unx     2620 b- defN 23-Jun-28 12:15 model_navigator/runners/jax.py
+-rw-rw-rw-  2.0 unx     9999 b- defN 23-Jun-28 12:15 model_navigator/runners/onnx.py
+-rw-rw-rw-  2.0 unx     2267 b- defN 23-Jun-28 12:15 model_navigator/runners/python.py
+-rw-rw-rw-  2.0 unx     2290 b- defN 23-Jun-28 12:15 model_navigator/runners/registry.py
+-rw-rw-rw-  2.0 unx     7976 b- defN 23-Jun-28 12:15 model_navigator/runners/tensorflow.py
+-rw-rw-rw-  2.0 unx    26748 b- defN 23-Jun-28 14:25 model_navigator/runners/tensorrt.py
+-rw-rw-rw-  2.0 unx    10041 b- defN 23-Jun-29 08:01 model_navigator/runners/torch.py
+-rw-rw-rw-  2.0 unx     3559 b- defN 23-Jun-28 12:15 model_navigator/runners/utils.py
+-rw-rw-rw-  2.0 unx      937 b- defN 23-Jun-28 12:15 model_navigator/runtime_analyzer/__init__.py
+-rw-rw-rw-  2.0 unx    11714 b- defN 23-Jun-28 12:15 model_navigator/runtime_analyzer/analyzer.py
+-rw-rw-rw-  2.0 unx     2304 b- defN 23-Jun-28 12:15 model_navigator/runtime_analyzer/strategy.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/triton/__init__.py
+-rw-rw-rw-  2.0 unx     3180 b- defN 23-Jun-28 12:15 model_navigator/triton/model_config.py
+-rw-rw-rw-  2.0 unx     5218 b- defN 23-Jun-28 12:15 model_navigator/triton/model_config_builder.py
+-rw-rw-rw-  2.0 unx    23090 b- defN 23-Jun-28 12:15 model_navigator/triton/model_config_generator.py
+-rw-rw-rw-  2.0 unx    15243 b- defN 23-Jun-30 11:34 model_navigator/triton/model_repository.py
+-rw-rw-rw-  2.0 unx     2081 b- defN 23-Jun-28 12:15 model_navigator/triton/utils.py
+-rw-rw-rw-  2.0 unx      944 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/__init__.py
+-rw-rw-rw-  2.0 unx     2872 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-rw-rw-  2.0 unx    22326 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/common.py
+-rw-rw-rw-  2.0 unx     2229 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/internal.py
+-rw-rw-rw-  2.0 unx     2685 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-rw-rw-  2.0 unx     1785 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-rw-rw-  2.0 unx     2239 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-rw-rw-  2.0 unx     3162 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-rw-rw-  2.0 unx     3040 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/utils/__init__.py
+-rw-rw-rw-  2.0 unx    14528 b- defN 23-Jun-30 12:44 model_navigator/utils/common.py
+-rw-rw-rw-  2.0 unx     8132 b- defN 23-Jun-28 12:15 model_navigator/utils/dataloader.py
+-rw-rw-rw-  2.0 unx     3902 b- defN 23-Jun-28 12:15 model_navigator/utils/devices.py
+-rw-rw-rw-  2.0 unx     1308 b- defN 23-Jun-28 12:15 model_navigator/utils/enums.py
+-rw-rw-rw-  2.0 unx     6163 b- defN 23-Jun-28 12:15 model_navigator/utils/environment.py
+-rw-rw-rw-  2.0 unx     4096 b- defN 23-Jun-28 12:15 model_navigator/utils/format_helpers.py
+-rw-rw-rw-  2.0 unx     2330 b- defN 23-Jun-28 12:15 model_navigator/utils/module.py
+-rw-rw-rw-  2.0 unx    10140 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10798 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    14493 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/RECORD
+145 files, 768630 bytes uncompressed, 230679 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -3,20 +3,14 @@
 
 Filename: model_navigator/__version__.py
 Comment: 
 
 Filename: model_navigator/exceptions.py
 Comment: 
 
-Filename: model_navigator/execution_context.py
-Comment: 
-
-Filename: model_navigator/logger.py
-Comment: 
-
 Filename: model_navigator/api/__init__.py
 Comment: 
 
 Filename: model_navigator/api/config.py
 Comment: 
 
 Filename: model_navigator/api/jax.py
@@ -48,14 +42,17 @@
 
 Filename: model_navigator/commands/__init__.py
 Comment: 
 
 Filename: model_navigator/commands/base.py
 Comment: 
 
+Filename: model_navigator/commands/execution_context.py
+Comment: 
+
 Filename: model_navigator/commands/infer_metadata.py
 Comment: 
 
 Filename: model_navigator/commands/load.py
 Comment: 
 
 Filename: model_navigator/commands/convert/__init__.py
@@ -156,15 +153,24 @@
 
 Filename: model_navigator/commands/performance/__init__.py
 Comment: 
 
 Filename: model_navigator/commands/performance/performance.py
 Comment: 
 
-Filename: model_navigator/commands/performance/performance_script.py
+Filename: model_navigator/commands/performance/profile.py
+Comment: 
+
+Filename: model_navigator/commands/performance/profile_script.py
+Comment: 
+
+Filename: model_navigator/commands/performance/profiler.py
+Comment: 
+
+Filename: model_navigator/commands/performance/results.py
 Comment: 
 
 Filename: model_navigator/commands/verification/__init__.py
 Comment: 
 
 Filename: model_navigator/commands/verification/verify.py
 Comment: 
@@ -186,21 +192,21 @@
 
 Filename: model_navigator/core/__init__.py
 Comment: 
 
 Filename: model_navigator/core/constants.py
 Comment: 
 
-Filename: model_navigator/core/package.py
+Filename: model_navigator/core/logger.py
 Comment: 
 
-Filename: model_navigator/core/status.py
+Filename: model_navigator/core/tensor.py
 Comment: 
 
-Filename: model_navigator/core/tensor.py
+Filename: model_navigator/core/workspace.py
 Comment: 
 
 Filename: model_navigator/frameworks/__init__.py
 Comment: 
 
 Filename: model_navigator/frameworks/jax/__init__.py
 Comment: 
@@ -225,20 +231,41 @@
 
 Filename: model_navigator/frameworks/torch/__init__.py
 Comment: 
 
 Filename: model_navigator/frameworks/torch/utils.py
 Comment: 
 
+Filename: model_navigator/package/__init__.py
+Comment: 
+
+Filename: model_navigator/package/builder.py
+Comment: 
+
+Filename: model_navigator/package/loader.py
+Comment: 
+
+Filename: model_navigator/package/package.py
+Comment: 
+
+Filename: model_navigator/package/profiling_results.py
+Comment: 
+
+Filename: model_navigator/package/status.py
+Comment: 
+
 Filename: model_navigator/pipelines/__init__.py
 Comment: 
 
 Filename: model_navigator/pipelines/pipeline.py
 Comment: 
 
+Filename: model_navigator/pipelines/pipeline_context.py
+Comment: 
+
 Filename: model_navigator/pipelines/pipeline_manager.py
 Comment: 
 
 Filename: model_navigator/pipelines/validation.py
 Comment: 
 
 Filename: model_navigator/pipelines/builders/__init__.py
@@ -252,14 +279,17 @@
 
 Filename: model_navigator/pipelines/builders/jax.py
 Comment: 
 
 Filename: model_navigator/pipelines/builders/onnx.py
 Comment: 
 
+Filename: model_navigator/pipelines/builders/performance.py
+Comment: 
+
 Filename: model_navigator/pipelines/builders/preprocessing.py
 Comment: 
 
 Filename: model_navigator/pipelines/builders/profiling.py
 Comment: 
 
 Filename: model_navigator/pipelines/builders/tensorflow.py
@@ -267,14 +297,23 @@
 
 Filename: model_navigator/pipelines/builders/torch.py
 Comment: 
 
 Filename: model_navigator/pipelines/builders/verify.py
 Comment: 
 
+Filename: model_navigator/pipelines/wrappers/__init__.py
+Comment: 
+
+Filename: model_navigator/pipelines/wrappers/optimize.py
+Comment: 
+
+Filename: model_navigator/pipelines/wrappers/profile.py
+Comment: 
+
 Filename: model_navigator/runners/__init__.py
 Comment: 
 
 Filename: model_navigator/runners/base.py
 Comment: 
 
 Filename: model_navigator/runners/jax.py
@@ -375,26 +414,23 @@
 
 Filename: model_navigator/utils/format_helpers.py
 Comment: 
 
 Filename: model_navigator/utils/module.py
 Comment: 
 
-Filename: model_navigator/utils/package.py
-Comment: 
-
-Filename: triton_model_navigator-0.5.6.dist-info/LICENSE
+Filename: triton_model_navigator-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.5.6.dist-info/METADATA
+Filename: triton_model_navigator-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.5.6.dist-info/WHEEL
+Filename: triton_model_navigator-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.5.6.dist-info/top_level.txt
+Filename: triton_model_navigator-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.5.6.dist-info/RECORD
+Filename: triton_model_navigator-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_navigator/__version__.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D100
-__version__ = "0.5.6"
+__version__ = "0.6.0"
```

## model_navigator/exceptions.py

```diff
@@ -58,14 +58,20 @@
 
 class ModelNavigatorWarning(ModelNavigatorError, Warning):
     """ModelNavigatorWarning exception."""
 
     pass
 
 
+class ModelNavigatorRuntimeError(ModelNavigatorError):
+    """ModelNavigatorRuntimeError exception."""
+
+    pass
+
+
 class ModelNavigatorUserInputError(ModelNavigatorError):
     """ModelNavigatorUserInputError exceptions.
 
     Raised when provided input data by user if not valid.
     """
 
     pass
@@ -137,7 +143,13 @@
     pass
 
 
 class ModelNavigatorConfigurationWarning(ModelNavigatorWarning):
     """Raised when the configuration is not valid, but the optimize command can still be run without ambiguity."""
 
     pass
+
+
+class ModelNavigatorCommandNotExecutable(ModelNavigatorError):
+    """Raised when command execution is not possible."""
+
+    pass
```

## model_navigator/api/__init__.py

```diff
@@ -20,23 +20,23 @@
     MinLatencyStrategy,
 )
 
 from .config import (  # noqa: F401
     DeviceKind,
     Format,
     JitType,
-    MeasurementMode,
     OnnxConfig,
-    ProfilerConfig,
+    OptimizationProfile,
     TensorFlowConfig,
     TensorFlowTensorRTConfig,
     TensorRTConfig,
     TensorRTPrecision,
     TensorRTPrecisionMode,
     TensorRTProfile,
+    TensorType,
     TorchConfig,
     TorchTensorRTConfig,
 )
 
 if is_torch_available():
     from . import torch  # noqa: F401
```

## model_navigator/api/config.py

```diff
@@ -36,17 +36,17 @@
 
 from model_navigator.core.constants import (
     DEFAULT_MAX_WORKSPACE_SIZE,
     DEFAULT_MIN_SEGMENT_SIZE,
     DEFAULT_ONNX_OPSET,
     DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD,
 )
+from model_navigator.core.logger import LOGGER
 from model_navigator.exceptions import ModelNavigatorConfigurationError
 from model_navigator.frameworks import Framework
-from model_navigator.logger import LOGGER
 from model_navigator.utils.common import DataObject
 
 Sample = Dict[str, numpy.ndarray]
 
 VerifyFunction = Callable[[Iterable[Sample], Iterable[Sample]], bool]
 
 
@@ -111,15 +111,15 @@
     TF_TRT = "tf-trt"
     TORCH_TRT = "torch-trt"
     ONNX = "onnx"
     TENSORRT = "trt"
 
 
 class JitType(Enum):
-    """TorchScript export paramter.
+    """TorchScript export parameter.
 
     Used for selecting the type of TorchScript export.
 
     Args:
         TRACE (str): Use tracing during export.
         SCRIPT (str): Use scripting during export.
     """
@@ -152,14 +152,23 @@
     """
 
     HIERARCHY = "hierarchy"
     SINGLE = "single"
     MIXED = "mixed"
 
 
+class TensorType(Enum):
+    """All model formats supported by Model Navigator 'optimize' function."""
+
+    NUMPY = "numpy"
+    TORCH = "torch"
+    TENSORFLOW = "tensorflow"
+    JAX = "jax"
+
+
 class TensorRTCompatibilityLevel(Enum):
     """Compatibility level for TensorRT.
 
     Args:
         AMPERE_PLUS (str): Support AMPERE plus architecture
     """
 
@@ -191,85 +200,82 @@
         return type(self).__name__ + self.__str__()
 
     def __iter__(self):
         """Iterate over shapes."""
         yield from [self.min, self.opt, self.max]
 
 
-class MeasurementMode(Enum):
-    """Profiler measurement mode.
-
-    Args:
-        TIME_WINDOWS (str): mode run measurement windows with fixed time length.
-        COUNT_WINDOWS (str): mode run measurement windows with fixed number of requests.
-    """
-
-    TIME_WINDOWS = "time_windows"
-    COUNT_WINDOWS = "count_windows"
-
-
 @dataclass
-class ProfilerConfig(DataObject):
-    """Profiler configuration.
+class OptimizationProfile(DataObject):
+    """Optimization profile configuration.
 
-    For each batch size profiler will run measurments in windows. Depending on the measurement mode,
-    each window will have fixed time length (MeasurementMode.TIME_WINDOWS)
-    or fixed number of requests (MeasurementMode.COUNT_WINDOWS).
+    For each batch size profiler will run measurements in windows of fixed number of queries.
     Batch sizes are profiled in the ascending order.
 
     Profiler will run multiple trials and will stop when the measurements
     are stable (within `stability_percentage` from the mean) within three consecutive windows.
     If the measurements are not stable after `max_trials` trials, the profiler will stop with an error.
     Profiler will also stop profiling when the throughput does not increase at least by `throughput_cutoff_threshold`.
 
 
     Args:
-        run_profiling (bool): If True, run profiling, otherwise skip profiling.
-        batch_sizes (Optional[List[Union[int, None]]]): List of batch sizes to profile.
-            None means that the model does not support batching.
-        measurement_mode (MeasurementMode): Measurement mode.
-        measurement_interval (Optional[float]): Measurement interval in milliseconds.
-            Used only in MeasurementMode.TIME_WINDOWS mode.
-        measurement_request_count (Optional[int]): Number of requests to measure in each window.
-            Used only in MeasurementMode.COUNT_WINDOWS mode.
-        stability_percentage (float): Allowed percentage of variation from the mean in three consecutive windows.
-        max_trials (int): Maximum number of window trials.
-        throughput_cutoff_threshold (float): Minimum throughput increase to continue profiling.
+        max_batch_size: Maximal batch size used during conversion and profiling. None mean automatic search is enabled.
+        batch_sizes : List of batch sizes to profile. None mean automatic search is enabled.
+        window_size: Number of requests to measure in each window.
+        stability_percentage: Allowed percentage of variation from the mean in three consecutive windows.
+        max_trials: Maximum number of window trials.
+        throughput_cutoff_threshold: Minimum throughput increase to continue profiling.
+        dataloader: Optional dataloader for profiling. Use only 1 sample.
     """
 
-    run_profiling: bool = True
+    max_batch_size: Optional[int] = None
     batch_sizes: Optional[List[Union[int, None]]] = None
-    measurement_mode: MeasurementMode = MeasurementMode.COUNT_WINDOWS
-    measurement_interval: Optional[float] = 5000  # ms
-    measurement_request_count: Optional[int] = 50
+    window_size: Optional[int] = 50
     stability_percentage: float = 10.0
     max_trials: int = 10
     throughput_cutoff_threshold: float = DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD
+    dataloader: Optional[SizedDataLoader] = None
+
+    def to_dict(self, filter_fields: Optional[List[str]] = None, parse: bool = False) -> Dict:
+        """Serialize to a dictionary.
+
+        Append `dataloader` field to filtered fields during dump.
+
+        Args:
+            filter_fields (Optional[List[str]], optional): List of fields to filter out.
+                Defaults to None.
+            parse (bool, optional): If True recursively parse field values to jsonable representation.
+                Defaults to False.
+
+        Returns:
+            Dict: Data serialized to a dictionary.
+        """
+        if not filter_fields:
+            filter_fields = []
+
+        filter_fields += ["dataloader"]
+        return super().to_dict(filter_fields=filter_fields, parse=parse)
 
     @classmethod
-    def from_dict(cls, profiler_config_dict: Mapping) -> "ProfilerConfig":
-        """Instantiate ProfilerConfig class from a dictionary.
+    def from_dict(cls, optimization_profile_dict: Mapping) -> "OptimizationProfile":
+        """Instantiate OptimizationProfile class from a dictionary.
 
         Args:
-            profiler_config_dict (Mapping): Data dictionary.
+            optimization_profile_dict (Mapping): Data dictionary.
 
         Returns:
-            ProfilerConfig
+            OptimizationProfile
         """
         return cls(
-            run_profiling=profiler_config_dict.get("run_profiling", True),
-            batch_sizes=profiler_config_dict.get("batch_sizes"),
-            measurement_interval=profiler_config_dict.get("measurement_interval"),
-            measurement_mode=MeasurementMode(
-                profiler_config_dict.get("measurement_mode", MeasurementMode.TIME_WINDOWS)
-            ),
-            measurement_request_count=profiler_config_dict.get("measurement_request_count"),
-            stability_percentage=profiler_config_dict.get("stability_percentage", 10.0),
-            max_trials=profiler_config_dict.get("max_trials", 10),
-            throughput_cutoff_threshold=profiler_config_dict.get("throughput_cutoff_threshold", -2),
+            max_batch_size=optimization_profile_dict.get("max_batch_size"),
+            batch_sizes=optimization_profile_dict.get("batch_sizes"),
+            window_size=optimization_profile_dict.get("window_size"),
+            stability_percentage=optimization_profile_dict.get("stability_percentage", 10.0),
+            max_trials=optimization_profile_dict.get("max_trials", 10),
+            throughput_cutoff_threshold=optimization_profile_dict.get("throughput_cutoff_threshold", -2),
         )
 
 
 class TensorRTProfile(Dict[str, ShapeTuple]):
     """Single optimization profile that can be used to build an engine.
 
     More specifically, it is an ``Dict[str, ShapeTuple]`` which maps binding
```

## model_navigator/api/jax.py

```diff
@@ -8,63 +8,62 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """JAX optimize API."""
-from pathlib import Path
+import pathlib
 from typing import Any, Callable, Mapping, Optional, Sequence, Tuple, Type, Union
 
 import tensorflow  # pytype: disable=import-error
 
 from model_navigator.api.config import (
     DEFAULT_JAX_TARGET_FORMATS,
     CustomConfig,
     DeviceKind,
     Format,
-    ProfilerConfig,
+    OptimizationProfile,
     SizedDataLoader,
     VerifyFunction,
     map_custom_configs,
 )
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config_builder import ModelConfigBuilder
 from model_navigator.core.constants import DEFAULT_SAMPLE_COUNT
-from model_navigator.core.package import Package
 from model_navigator.exceptions import ModelNavigatorConfigurationError
 from model_navigator.frameworks import Framework
 from model_navigator.frameworks.jax import JaxModel
+from model_navigator.package.package import Package
 from model_navigator.pipelines.builders import (
     correctness_builder,
     jax_export_builder,
+    performance_builder,
     preprocessing_builder,
-    profiling_builder,
     tensorflow_conversion_builder,
     verify_builder,
 )
 from model_navigator.pipelines.builders.find_device_max_batch_size import find_device_max_batch_size_builder
-from model_navigator.pipelines.pipeline_manager import PipelineManager
+from model_navigator.pipelines.wrappers.optimize import optimize_pipeline
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runners.utils import default_runners
 from model_navigator.utils import enums
-from model_navigator.utils.common import get_default_workspace
 
 
 def optimize(
     model: Callable,
     model_params: Any,
     dataloader: SizedDataLoader,
     sample_count: int = DEFAULT_SAMPLE_COUNT,
     batching: Optional[bool] = True,
-    target_formats: Optional[Union[Union[str, Format], Tuple[Union[str, Format], ...]]] = None,
+    target_formats: Optional[Tuple[Union[str, Format], ...]] = None,
     target_device: Optional[DeviceKind] = DeviceKind.CUDA,
-    runners: Optional[Union[Union[str, Type[NavigatorRunner]], Tuple[Union[str, Type[NavigatorRunner]], ...]]] = None,
-    profiler_config: Optional[ProfilerConfig] = None,
-    workspace: Optional[Path] = None,
+    runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
+    optimization_profile: Optional[OptimizationProfile] = None,
+    workspace: Optional[pathlib.Path] = None,
     verbose: bool = False,
     debug: bool = False,
     verify_func: Optional[VerifyFunction] = None,
     custom_configs: Optional[Sequence[CustomConfig]] = None,
 ) -> Package:
     """Entry point for JAX optimize.
 
@@ -74,20 +73,20 @@
         model: JAX forward function
         model_params: JAX model parameters (weights)
         dataloader: Sized iterable with data that will be feed to the model
         sample_count: Limits how many samples will be used from dataloader
         batching: Enable or disable batching on first (index 0) dimension of the model
         target_formats: Target model formats for optimize process
         target_device: Target device for optimize process, default is CUDA
-        runners: Use only runners provided as paramter
-        profiler_config: Profiling config
+        runners: Use only runners provided as parameter
+        optimization_profile: Optimization profile for conversion and profiling
         workspace: Workspace where packages will be extracted
         verbose: Enable verbose logging
         debug: Enable debug logging from commands
-        verify_func: Function for additional model verifcation
+        verify_func: Function for additional model verification
         custom_configs: Sequence of CustomConfigs used to control produced artifacts
 
     Returns:
         Package descriptor representing created package.
     """
     if target_device == DeviceKind.CPU and any(
         device.device_type == "GPU" for device in tensorflow.config.get_visible_devices()
@@ -96,47 +95,45 @@
             "\n"
             "    'target_device == nav.DeviceKind.CPU' is not supported for TensorFlow2 "
             "(exported from JAX) when GPU is available.\n"
             "    To optimize model for CPU, disable GPU with: "
             "'tf.config.set_visible_devices([], 'GPU')' directly after importing TensorFlow.\n"
         )
     if isinstance(model, str):
-        model = Path(model)
-    if workspace is None:
-        workspace = get_default_workspace()
+        model = pathlib.Path(model)
+
     if target_formats is None:
         target_formats = DEFAULT_JAX_TARGET_FORMATS
 
     sample = next(iter(dataloader))
     forward_kw_names = tuple(sample.keys()) if isinstance(sample, Mapping) else None
 
     if runners is None:
         runners = default_runners(device_kind=target_device)
 
-    if profiler_config is None:
-        profiler_config = ProfilerConfig()
+    if optimization_profile is None:
+        optimization_profile = OptimizationProfile()
 
     target_formats_enums = enums.parse(target_formats, Format)
     runner_names = enums.parse(runners, lambda runner: runner if isinstance(runner, str) else runner.name())
 
     if Format.JAX not in target_formats_enums:
         target_formats_enums = (Format.JAX,) + target_formats_enums
 
     config = CommonConfig(
         Framework.JAX,
         model=JaxModel(model=model, params=model_params),
         dataloader=dataloader,
         forward_kw_names=forward_kw_names,
-        workspace=workspace,
         target_formats=target_formats_enums,
         target_device=target_device,
         sample_count=sample_count,
         batch_dim=0 if batching else None,
         runner_names=runner_names,
-        profiler_config=profiler_config,
+        optimization_profile=optimization_profile,
         verbose=verbose,
         debug=debug,
         verify_func=verify_func,
         custom_configs=map_custom_configs(custom_configs=custom_configs),
     )
 
     models_config = ModelConfigBuilder.generate_model_config(
@@ -147,19 +144,19 @@
 
     builders = [
         preprocessing_builder,
         jax_export_builder,
         find_device_max_batch_size_builder,
         tensorflow_conversion_builder,
         correctness_builder,
+        performance_builder,
+        verify_builder,
     ]
-    if profiler_config.run_profiling:
-        builders.append(profiling_builder)
-    builders.append(verify_builder)
-
-    package = PipelineManager.run(
-        pipeline_builders=builders,
+    package = optimize_pipeline(
+        model=model,
+        workspace=workspace,
+        builders=builders,
         config=config,
         models_config=models_config,
     )
 
     return package
```

## model_navigator/api/onnx.py

```diff
@@ -8,58 +8,57 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ONNX optimize API."""
-from pathlib import Path
+import pathlib
 from typing import Optional, Sequence, Tuple, Type, Union
 
 from model_navigator.api.config import (
     DEFAULT_ONNX_TARGET_FORMATS,
     CustomConfig,
     DeviceKind,
     Format,
-    ProfilerConfig,
+    OptimizationProfile,
     SizedDataLoader,
     VerifyFunction,
     map_custom_configs,
 )
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config_builder import ModelConfigBuilder
 from model_navigator.core.constants import DEFAULT_SAMPLE_COUNT
-from model_navigator.core.package import Package
 from model_navigator.frameworks import Framework
+from model_navigator.package.package import Package
 from model_navigator.pipelines.builders import (
     correctness_builder,
     onnx_conversion_builder,
     onnx_export_builder,
+    performance_builder,
     preprocessing_builder,
-    profiling_builder,
     verify_builder,
 )
 from model_navigator.pipelines.builders.find_device_max_batch_size import find_device_max_batch_size_builder
-from model_navigator.pipelines.pipeline_manager import PipelineManager
+from model_navigator.pipelines.wrappers.optimize import optimize_pipeline
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runners.utils import default_runners
 from model_navigator.utils import enums
-from model_navigator.utils.common import get_default_workspace
 
 
 def optimize(
-    model: Union[Path, str],
+    model: Union[pathlib.Path, str],
     dataloader: SizedDataLoader,
     sample_count: int = DEFAULT_SAMPLE_COUNT,
     batching: Optional[bool] = True,
-    target_formats: Optional[Union[Union[str, Format], Tuple[Union[str, Format], ...]]] = None,
+    target_formats: Optional[Tuple[Union[str, Format], ...]] = None,
     target_device: Optional[DeviceKind] = DeviceKind.CUDA,
-    runners: Optional[Union[Union[str, Type[NavigatorRunner]], Tuple[Union[str, Type[NavigatorRunner]], ...]]] = None,
-    profiler_config: Optional[ProfilerConfig] = None,
-    workspace: Optional[Path] = None,
+    runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
+    optimization_profile: Optional[OptimizationProfile] = None,
+    workspace: Optional[pathlib.Path] = None,
     verbose: bool = False,
     debug: bool = False,
     verify_func: Optional[VerifyFunction] = None,
     custom_configs: Optional[Sequence[CustomConfig]] = None,
 ) -> Package:
     """Entrypoint for ONNX optimize.
 
@@ -69,54 +68,52 @@
         model: ONNX model path or string
         dataloader: Sized iterable with data that will be feed to the model
         sample_count: Limits how many samples will be used from dataloader
         batching: Enable or disable batching on first (index 0) dimension of the model
         target_formats: Target model formats for optimize process
         target_device: Target device for optimize process, default is CUDA
         runners: Use only runners provided as parameter
-        profiler_config: Profiling config
+        optimization_profile: Optimization profile for conversion and profiling
         workspace: Workspace where packages will be extracted
         verbose: Enable verbose logging
         debug: Enable debug logging from commands
         verify_func: Function for additional model verification
         custom_configs: Sequence of CustomConfigs used to control produced artifacts
 
     Returns:
         Package descriptor representing created package.
     """
     if isinstance(model, str):
-        model = Path(model)
-    if workspace is None:
-        workspace = get_default_workspace()
+        model = pathlib.Path(model)
+
     if target_formats is None:
         target_formats = DEFAULT_ONNX_TARGET_FORMATS
 
     if runners is None:
         runners = default_runners(device_kind=target_device)
 
-    if profiler_config is None:
-        profiler_config = ProfilerConfig()
+    if optimization_profile is None:
+        optimization_profile = OptimizationProfile()
 
     target_formats_enums = enums.parse(target_formats, Format)
     runner_names = enums.parse(runners, lambda runner: runner if isinstance(runner, str) else runner.name())
 
     if Format.ONNX not in target_formats_enums:
         target_formats_enums = (Format.ONNX,) + target_formats_enums
 
     config = CommonConfig(
         Framework.ONNX,
         model=model,
         dataloader=dataloader,
-        workspace=workspace,
         target_formats=target_formats_enums,
         target_device=target_device,
         sample_count=sample_count,
         batch_dim=0 if batching else None,
         runner_names=runner_names,
-        profiler_config=profiler_config,
+        optimization_profile=optimization_profile,
         verbose=verbose,
         debug=debug,
         verify_func=verify_func,
         custom_configs=map_custom_configs(custom_configs=custom_configs),
     )
 
     models_config = ModelConfigBuilder.generate_model_config(
@@ -127,19 +124,20 @@
 
     builders = [
         preprocessing_builder,
         onnx_export_builder,
         find_device_max_batch_size_builder,
         onnx_conversion_builder,
         correctness_builder,
+        performance_builder,
+        verify_builder,
     ]
-    if profiler_config.run_profiling:
-        builders.append(profiling_builder)
-    builders.append(verify_builder)
 
-    package = PipelineManager.run(
-        pipeline_builders=builders,
+    package = optimize_pipeline(
+        model=model,
+        workspace=workspace,
+        builders=builders,
         config=config,
         models_config=models_config,
     )
 
     return package
```

## model_navigator/api/package.py

```diff
@@ -10,93 +10,108 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Package operations related API."""
 
 
-from pathlib import Path
+import pathlib
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 from model_navigator.api.config import (
-    DEFAULT_TARGET_FORMATS,
     SOURCE_FORMATS,
     CustomConfig,
     DeviceKind,
     Format,
-    ProfilerConfig,
+    OptimizationProfile,
+    SizedDataLoader,
     VerifyFunction,
     map_custom_configs,
 )
 from model_navigator.commands.base import CommandStatus
 from model_navigator.commands.verification.verify import VerifyModel
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
 from model_navigator.configuration.model.model_config_builder import ModelConfigBuilder
-from model_navigator.core.package import Package
-from model_navigator.core.status import ModelStatus
+from model_navigator.core.constants import DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD
+from model_navigator.core.logger import LOGGER
+from model_navigator.core.workspace import Workspace
 from model_navigator.exceptions import (
     ModelNavigatorEmptyPackageError,
     ModelNavigatorMissingSourceModelError,
     ModelNavigatorNotFoundError,
 )
 from model_navigator.frameworks import Framework
 from model_navigator.frameworks.torch.utils import update_allowed_batching_parameters
+from model_navigator.package.builder import PackageBuilder
+from model_navigator.package.loader import PackageLoader
+from model_navigator.package.package import Package
+from model_navigator.package.status import ModelStatus
 from model_navigator.pipelines.builders import (
     PipelineBuilder,
     correctness_builder,
+    performance_builder,
     preprocessing_builder,
-    profiling_builder,
 )
 from model_navigator.pipelines.builders.find_device_max_batch_size import find_device_max_batch_size_builder
+from model_navigator.pipelines.builders.profiling import profiling_builder
 from model_navigator.pipelines.builders.verify import verify_builder
-from model_navigator.pipelines.pipeline_manager import PipelineManager
+from model_navigator.pipelines.wrappers.optimize import optimize_pipeline
+from model_navigator.pipelines.wrappers.profile import ProfilingResults, profile_pipeline
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runners.registry import runner_registry
 from model_navigator.runners.utils import default_runners
 from model_navigator.runtime_analyzer.strategy import RuntimeSearchStrategy
 from model_navigator.utils import enums
-from model_navigator.utils.format_helpers import FRAMEWORK2BASE_FORMAT
+from model_navigator.utils.format_helpers import FRAMEWORK2BASE_FORMAT, get_target_formats
 
 
 def load(
-    path: Union[str, Path],
-    workspace: Optional[Union[str, Path]] = None,
+    path: Union[str, pathlib.Path],
+    workspace: Optional[Union[str, pathlib.Path]] = None,
 ) -> Package:
     """Load package from provided path.
 
     Args:
         path: The location of package to load
         workspace: Workspace where packages will be extracted
 
     Returns:
         Package.
     """
-    return Package.load(path=path, workspace=workspace)
+    LOGGER.info(f"Loading package from {path} to {workspace}.")
+
+    workspace = Workspace(workspace)
+    workspace.initialize()
+
+    loader = PackageLoader()
+    package = loader.from_file(path=path, workspace=workspace)
+    LOGGER.info(f"Package loaded and unpacked {workspace}.")
+
+    return package
 
 
 def save(
     package: Package,
-    path: Union[str, Path],
-    keep_workspace: bool = True,
+    path: Union[str, pathlib.Path],
     override: bool = False,
     save_data: bool = True,
 ) -> None:
     """Save export results into the .nav package at given path.
 
     Args:
         package: A package object to prepare the package
         path: A path to file where the package has to be saved
-        keep_workspace: flag to remove the working directory after saving the package
         override: flag to override existing package in provided path
         save_data: disable saving samples from the dataloader
     """
-    package.save(
+    builder = PackageBuilder()
+    builder.save(
+        package=package,
         path=path,
-        keep_workspace=keep_workspace,
         override=override,
         save_data=save_data,
     )
 
 
 def get_best_model_status(
     package: Package,
@@ -117,96 +132,197 @@
         ModelStatus of best model for given strategy or None.
     """
     return package.get_best_model_status(strategy=strategy, include_source=include_source)
 
 
 def optimize(
     package: Package,
-    target_formats: Optional[Union[Union[str, Format], Tuple[Union[str, Format], ...]]] = None,
+    target_formats: Optional[Tuple[Union[str, Format], ...]] = None,
     target_device: Optional[DeviceKind] = DeviceKind.CUDA,
-    runners: Optional[Union[Union[str, Type[NavigatorRunner]], Tuple[Union[str, Type[NavigatorRunner]], ...]]] = None,
-    profiler_config: Optional[ProfilerConfig] = None,
+    runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
+    optimization_profile: Optional[OptimizationProfile] = None,
     verbose: bool = False,
     debug: bool = False,
     verify_func: Optional[VerifyFunction] = None,
     custom_configs: Optional[List[CustomConfig]] = None,
     defaults: bool = True,
+    fail_on_empty: bool = True,
 ) -> Package:
     """Generate target formats and run correctness and profiling tests for available runners.
 
     Args:
         package: Package to optimize.
         target_formats: Formats to generate and profile. Defaults to target formats from the package.
         target_device: Target device for optimize process, default is CUDA
         runners: Runners to run correctness tests and profiling on. Defaults to runners from the package.
-        profiler_config: Configuration of the profiler. Defaults to config from the package.
+        optimization_profile: Optimization profile used for conversion and profiling.
         verbose: If True enable verbose logging. Defaults to False.
         debug: If True print debugging logs. Defaults to False.
         verify_func: Function used for verifying generated models. Defaults to None.
         custom_configs: Custom formats configuration. Defaults to None.
         defaults: reset configuration of custom configs to defaults
+        fail_on_empty: Fail optimization when empty (no model or base exported model) package provided
 
     Returns:
         Optimized package
     """
-    if package.is_empty() and package.model is None:
+    if fail_on_empty and package.is_empty() and package.model is None:
         raise ModelNavigatorEmptyPackageError(
             "Package is empty and source model is not loaded. Unable to run optimize."
         )
     config = package.config
 
+    is_source_available = package.model is not None
     if target_formats is None:
-        target_formats = DEFAULT_TARGET_FORMATS[package.framework]
+        target_formats = get_target_formats(framework=package.framework, is_source_available=is_source_available)
         if package.framework == Framework.TORCH and config.batch_dim is not None:
             target_formats, custom_configs = update_allowed_batching_parameters(
                 target_formats=target_formats,
                 custom_configs=custom_configs,
             )
 
     if runners is None:
         runners = default_runners(device_kind=target_device)
 
-    if profiler_config is None:
-        profiler_config = ProfilerConfig()
+    if optimization_profile is None:
+        optimization_profile = OptimizationProfile()
 
-    is_source_available = package.model is not None
     _update_config(
         config=config,
         is_source_available=is_source_available,
         target_formats=target_formats,
         runners=runners,
-        profiler_config=profiler_config,
+        optimization_profile=optimization_profile,
         verbose=verbose,
         debug=debug,
         verify_func=verify_func,
         custom_configs=custom_configs,
         defaults=defaults,
         target_device=target_device,
     )
 
     builders = _get_builders(
         framework=package.framework,
-        run_profiling=config.profiler_config.run_profiling,
     )
 
-    model_configs = _get_model_configs(
+    models_config = _get_model_configs(
         config=config,
         custom_configs=list(config.custom_configs.values()),
     )
 
-    optimized_package = PipelineManager.run(
-        pipeline_builders=builders,
-        config=config,
-        models_config=model_configs,
+    optimized_package = optimize_pipeline(
         package=package,
+        workspace=package.workspace.path,
+        builders=builders,
+        config=config,
+        models_config=models_config,
     )
 
     return optimized_package
 
 
+def profile(
+    package: Package,
+    dataloader: Optional[SizedDataLoader] = None,
+    target_formats: Optional[Tuple[Union[str, Format], ...]] = None,
+    target_device: Optional[DeviceKind] = DeviceKind.CUDA,
+    runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
+    max_batch_size: Optional[int] = None,
+    batch_sizes: Optional[List[int]] = None,
+    window_size: int = 50,
+    stability_percentage: float = 10.0,
+    max_trials: int = 10,
+    throughput_cutoff_threshold: float = DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD,
+    verbose: bool = False,
+) -> ProfilingResults:
+    """Profile provided package.
+
+    When `dataloader` is provided, use all samples obtained from dataloader per-each batch size to perform profiling.
+    The profiling result return the min, max and average results per batch size from all samples.
+
+    When no `dataloader` provided, the profiling sample from package is used.
+
+    Args:
+        package: Package to profile.
+        dataloader: Sized iterable with data that will be feed to the model
+        target_formats: Formats to profile. Defaults to target formats from the package.
+        target_device: Target device to run profiling on.
+        runners: Runners to run profiling on. Defaults to runners from the package.
+        max_batch_size: Maximal batch size used for profiling. Default: None
+        batch_sizes: List of batch sizes to profile. Default: None
+        window_size: Number of inference queries performed in measurement window
+        stability_percentage: Allowed percentage of variation from the mean in three consecutive windows.
+        max_trials: Maximum number of window trials.
+        throughput_cutoff_threshold: Minimum throughput increase to continue profiling.
+        verbose: If True enable verbose logging. Defaults to False.
+
+    Returns:
+        Profiling results
+    """
+    if package.is_empty() and package.model is None:
+        raise ModelNavigatorEmptyPackageError(
+            "Package is empty and source model is not loaded. Unable to run optimize."
+        )
+
+    config = package.config
+    is_source_available = package.model is not None
+
+    if target_formats is None:
+        target_formats = get_target_formats(framework=package.framework, is_source_available=is_source_available)
+        if package.framework == Framework.TORCH and config.batch_dim is not None:
+            target_formats, custom_configs = update_allowed_batching_parameters(
+                target_formats=target_formats,
+                custom_configs=(),
+            )
+
+    if runners is None:
+        runners = default_runners(device_kind=target_device)
+
+    if dataloader is None:
+        dataloader = []
+
+    optimization_profile = OptimizationProfile(
+        max_batch_size=max_batch_size,
+        batch_sizes=batch_sizes,
+        window_size=window_size,
+        stability_percentage=stability_percentage,
+        max_trials=max_trials,
+        throughput_cutoff_threshold=throughput_cutoff_threshold,
+    )
+
+    _update_config(
+        config=config,
+        dataloader=dataloader,
+        is_source_available=is_source_available,
+        target_formats=target_formats,
+        runners=runners,
+        optimization_profile=optimization_profile,
+        verbose=verbose,
+        target_device=target_device,
+    )
+
+    builders = [
+        preprocessing_builder,
+        profiling_builder,
+    ]
+
+    model_configs = _get_model_configs(
+        config=config,
+        custom_configs=[],
+    )
+    profiling_results = profile_pipeline(
+        package=package,
+        config=config,
+        builders=builders,
+        models_config=model_configs,
+    )
+
+    return profiling_results
+
+
 def set_verified(
     package: Package,
     model_key: str,
     runner_name: str,
 ) -> None:
     """Set verified status for model and runner.
 
@@ -221,38 +337,37 @@
     try:
         runner_results = package.status.models_status[model_key].runners_status[runner_name]
     except KeyError:
         raise ModelNavigatorNotFoundError(f"Model {model_key} and runner {runner_name} not found.")
     runner_results.status[VerifyModel.__name__] = CommandStatus.OK
 
 
-def _get_builders(framework: Framework, run_profiling: bool) -> List[PipelineBuilder]:
+def _get_builders(framework: Framework) -> List[PipelineBuilder]:
     """Build list of pipeline builders for nav.package.optimize.
 
     Args:
         framework (Framework): Package framework.
-        run_profiling (bool): If True attach profiling pipeline builder.
     """
     if framework == Framework.TORCH:
         from model_navigator.pipelines.builders import torch_conversion_builder as conversion_builder
     elif framework in (Framework.TENSORFLOW, Framework.JAX):
         from model_navigator.pipelines.builders import tensorflow_conversion_builder as conversion_builder
     else:
         assert framework == Framework.ONNX
         from model_navigator.pipelines.builders import onnx_conversion_builder as conversion_builder
 
     builders: List[PipelineBuilder] = [
         preprocessing_builder,
         find_device_max_batch_size_builder,
         conversion_builder,
         correctness_builder,
+        performance_builder,
+        verify_builder,
     ]
-    if run_profiling:
-        builders.append(profiling_builder)
-    builders.append(verify_builder)
+
     return builders
 
 
 def _get_model_configs(config: CommonConfig, custom_configs: List[CustomConfig]) -> Dict[Format, List[ModelConfig]]:
     """Build model configs for nav.package.optimize.
 
     Args:
@@ -266,18 +381,19 @@
     )
     return custom_model_configs
 
 
 def _update_config(
     config: CommonConfig,
     is_source_available: bool,
-    target_formats: Optional[Union[Union[str, Format], Tuple[Union[str, Format], ...]]],
+    target_formats: Optional[Tuple[Union[str, Format], ...]],
     *,
-    runners: Optional[Union[Union[str, Type[NavigatorRunner]], Tuple[Union[str, Type[NavigatorRunner]], ...]]] = None,
-    profiler_config: Optional[ProfilerConfig] = None,
+    dataloader: Optional[SizedDataLoader] = None,
+    runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
+    optimization_profile: Optional[OptimizationProfile] = None,
     verbose: bool = False,
     debug: bool = False,
     verify_func: Optional[VerifyFunction] = None,
     custom_configs: Optional[List[CustomConfig]] = None,
     defaults: bool = True,
     target_device: DeviceKind = DeviceKind.CUDA,
 ) -> None:
@@ -288,20 +404,22 @@
     if base_format in target_formats_enums and base_format in SOURCE_FORMATS and not is_source_available:
         raise ModelNavigatorMissingSourceModelError(
             "Source model is not available in the package.\n"
             "Load source model with package.load_source_model(model) to use it "
             f"or remove {base_format} from target_formats."
         )
     config.target_formats = target_formats_enums
+    if dataloader is not None:
+        config.dataloader = dataloader
 
     # Reset profiling config
-    if profiler_config is None:
-        profiler_config = ProfilerConfig()
+    if optimization_profile is None:
+        optimization_profile = OptimizationProfile()
 
-    config.profiler_config = profiler_config
+    config.optimization_profile = optimization_profile
 
     # Reset runner names
     if runners is None:
         runners = tuple(runner_registry.keys())
 
     config.runner_names = enums.parse(runners, lambda runner: runner if isinstance(runner, str) else runner.name())
```

## model_navigator/api/python.py

```diff
@@ -8,53 +8,52 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Python optimize API."""
-from pathlib import Path
+import pathlib
 from typing import Callable, Mapping, Optional, Sequence, Tuple, Type, Union
 
 from model_navigator.api.config import (
     DEFAULT_NONE_FRAMEWORK_TARGET_FORMATS,
     CustomConfig,
     DeviceKind,
-    ProfilerConfig,
+    OptimizationProfile,
     SizedDataLoader,
     VerifyFunction,
     map_custom_configs,
 )
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config_builder import ModelConfigBuilder
 from model_navigator.core.constants import DEFAULT_SAMPLE_COUNT
-from model_navigator.core.package import Package
 from model_navigator.frameworks import Framework
+from model_navigator.package.package import Package
 from model_navigator.pipelines.builders import (
     correctness_builder,
+    performance_builder,
     preprocessing_builder,
-    profiling_builder,
     verify_builder,
 )
-from model_navigator.pipelines.pipeline_manager import PipelineManager
+from model_navigator.pipelines.wrappers.optimize import optimize_pipeline
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runners.utils import default_runners
 from model_navigator.utils import enums
-from model_navigator.utils.common import get_default_workspace
 
 
 def optimize(
     model: Callable,
     dataloader: SizedDataLoader,
     sample_count: int = DEFAULT_SAMPLE_COUNT,
     batching: Optional[bool] = True,
     target_device: Optional[DeviceKind] = DeviceKind.CPU,
-    runners: Optional[Union[Union[str, Type[NavigatorRunner]], Tuple[Union[str, Type[NavigatorRunner]], ...]]] = None,
-    profiler_config: Optional[ProfilerConfig] = None,
-    workspace: Optional[Path] = None,
+    runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
+    optimization_profile: Optional[OptimizationProfile] = None,
+    workspace: Optional[pathlib.Path] = None,
     verbose: bool = False,
     debug: bool = False,
     verify_func: Optional[VerifyFunction] = None,
     custom_configs: Optional[Sequence[CustomConfig]] = None,
 ) -> Package:
     """Entrypoint for Python model optimize.
 
@@ -62,71 +61,73 @@
 
     Args:
         model: Model inference function
         dataloader: Sized iterable with data that will be feed to the model
         sample_count: Limits how many samples will be used from dataloader
         batching: Enable or disable batching on first (index 0) dimension of the model
         target_device: Target device for optimize process, default is CPU
-        runners: Use only runners provided as paramter
-        profiler_config: Profiling config
+        runners: Use only runners provided as parameter
+        optimization_profile: Optimization profile for conversion and profiling
         workspace: Workspace where packages will be extracted
         verbose: Enable verbose logging
         debug: Enable debug logging from commands
-        verify_func: Function for additional model verifcation
+        verify_func: Function for additional model verification
         custom_configs: Sequence of CustomConfigs used to control produced artifacts
 
     Returns:
         Package descriptor representing created package.
     """
     if isinstance(model, str):
-        model = Path(model)
-    if workspace is None:
-        workspace = get_default_workspace()
+        model = pathlib.Path(model)
 
     sample = next(iter(dataloader))
     forward_kw_names = tuple(sample.keys()) if isinstance(sample, Mapping) else None
 
     if runners is None:
         runners = default_runners(device_kind=target_device)
 
-    if profiler_config is None:
-        profiler_config = ProfilerConfig()
+    if optimization_profile is None:
+        optimization_profile = OptimizationProfile()
 
     runner_names = enums.parse(runners, lambda runner: runner if isinstance(runner, str) else runner.name())
 
     target_formats = DEFAULT_NONE_FRAMEWORK_TARGET_FORMATS
+
     config = CommonConfig(
         Framework.NONE,
         model=model,
         dataloader=dataloader,
         forward_kw_names=forward_kw_names,
-        workspace=workspace,
         target_formats=target_formats,
         target_device=target_device,
         sample_count=sample_count,
         batch_dim=0 if batching else None,
         runner_names=runner_names,
-        profiler_config=profiler_config,
+        optimization_profile=optimization_profile,
         verbose=verbose,
         debug=debug,
         verify_func=verify_func,
         custom_configs=map_custom_configs(custom_configs=custom_configs),
     )
 
     models_config = ModelConfigBuilder.generate_model_config(
         framework=Framework.NONE,
         target_formats=target_formats,
         custom_configs=[],
     )
 
-    builders = [preprocessing_builder, correctness_builder]
-    if profiler_config.run_profiling:
-        builders.append(profiling_builder)
-    builders.append(verify_builder)
+    builders = [
+        preprocessing_builder,
+        correctness_builder,
+        performance_builder,
+        verify_builder,
+    ]
 
-    package = PipelineManager.run(
-        pipeline_builders=builders,
+    package = optimize_pipeline(
+        model=model,
+        workspace=workspace,
+        builders=builders,
         config=config,
         models_config=models_config,
     )
 
     return package
```

## model_navigator/api/pytriton.py

```diff
@@ -15,16 +15,16 @@
 
 import enum
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Type, Union
 
 import numpy as np
 
-from model_navigator.core.package import Package
 from model_navigator.exceptions import ModelNavigatorNotFoundError
+from model_navigator.package.package import Package
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runtime_analyzer.strategy import MaxThroughputAndMinLatencyStrategy, RuntimeSearchStrategy
 
 
 class TimeoutAction(enum.Enum):
     """Timeout action definition for timeout_action QueuePolicy field.
```

## model_navigator/api/tensorflow.py

```diff
@@ -8,63 +8,62 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """TensorFlow optimize API."""
-from pathlib import Path
+import pathlib
 from typing import Mapping, Optional, Sequence, Tuple, Type, Union
 
 import tensorflow  # pytype: disable=import-error
 
 from model_navigator.api.config import (
     DEFAULT_TENSORFLOW_TARGET_FORMATS,
     CustomConfig,
     DeviceKind,
     Format,
-    ProfilerConfig,
+    OptimizationProfile,
     SizedDataLoader,
     VerifyFunction,
     map_custom_configs,
 )
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config_builder import ModelConfigBuilder
 from model_navigator.core.constants import DEFAULT_SAMPLE_COUNT
-from model_navigator.core.package import Package
 from model_navigator.exceptions import ModelNavigatorConfigurationError
 from model_navigator.frameworks import Framework
+from model_navigator.package.package import Package
 from model_navigator.pipelines.builders import (
     correctness_builder,
+    performance_builder,
     preprocessing_builder,
-    profiling_builder,
     tensorflow_conversion_builder,
     tensorflow_export_builder,
     verify_builder,
 )
 from model_navigator.pipelines.builders.find_device_max_batch_size import find_device_max_batch_size_builder
-from model_navigator.pipelines.pipeline_manager import PipelineManager
+from model_navigator.pipelines.wrappers.optimize import optimize_pipeline
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runners.utils import default_runners
 from model_navigator.utils import enums
-from model_navigator.utils.common import get_default_workspace
 
 
 def optimize(
     model: tensorflow.keras.Model,
     dataloader: SizedDataLoader,
     sample_count: int = DEFAULT_SAMPLE_COUNT,
     batching: Optional[bool] = True,
     input_names: Optional[Tuple[str, ...]] = None,
     output_names: Optional[Tuple[str, ...]] = None,
-    target_formats: Optional[Union[Union[str, Format], Tuple[Union[str, Format], ...]]] = None,
+    target_formats: Optional[Tuple[Union[str, Format], ...]] = None,
     target_device: Optional[DeviceKind] = DeviceKind.CUDA,
-    runners: Optional[Union[Union[str, Type[NavigatorRunner]], Tuple[Union[str, Type[NavigatorRunner]], ...]]] = None,
-    profiler_config: Optional[ProfilerConfig] = None,
-    workspace: Optional[Path] = None,
+    runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
+    optimization_profile: Optional[OptimizationProfile] = None,
+    workspace: Optional[pathlib.Path] = None,
     verbose: bool = False,
     debug: bool = False,
     verify_func: Optional[VerifyFunction] = None,
     custom_configs: Optional[Sequence[CustomConfig]] = None,
 ) -> Package:
     """Entrypoint for TensorFlow2 optimize.
 
@@ -75,69 +74,67 @@
         dataloader: Sized iterable with data that will be feed to the model
         sample_count: Limits how many samples will be used from dataloader
         batching: Enable or disable batching on first (index 0) dimension of the model
         input_names: Model input names
         output_names: Model output names
         target_formats: Target model formats for optimize process
         target_device: Target device for optimize process, default is CUDA
-        runners: Use only runners provided as paramter
-        profiler_config: Profiling config
+        runners: Use only runners provided as parameter
+        optimization_profile: Optimization profile for conversion and profiling
         workspace: Workspace where packages will be extracted
         verbose: Enable verbose logging
         debug: Enable debug logging from commands
-        verify_func: Function for additional model verifcation
+        verify_func: Function for additional model verification
         custom_configs: Sequence of CustomConfigs used to control produced artifacts
 
     Returns:
         Package descriptor representing created package.
     """
     if target_device == DeviceKind.CPU and any(
         device.device_type == "GPU" for device in tensorflow.config.get_visible_devices()
     ):
         raise ModelNavigatorConfigurationError(
             "\n"
             "    'target_device == nav.DeviceKind.CPU' is not supported for TensorFlow2 when GPU is available.\n"
             "    To optimize model for CPU, disable GPU with: "
             "'tf.config.set_visible_devices([], 'GPU')' directly after importing TensorFlow.\n"
         )
-    if workspace is None:
-        workspace = get_default_workspace()
+
     if target_formats is None:
         target_formats = DEFAULT_TENSORFLOW_TARGET_FORMATS
 
     if runners is None:
         runners = default_runners(device_kind=target_device)
 
     forward_kw_names = None
     sample = next(iter(dataloader))
     if isinstance(sample, Mapping):
         forward_kw_names = tuple(sample.keys())
 
     target_formats_enums = enums.parse(target_formats, Format)
     runner_names = enums.parse(runners, lambda runner: runner if isinstance(runner, str) else runner.name())
 
-    if profiler_config is None:
-        profiler_config = ProfilerConfig()
+    if optimization_profile is None:
+        optimization_profile = OptimizationProfile()
 
     if Format.TENSORFLOW not in target_formats_enums:
         target_formats_enums = (Format.TENSORFLOW,) + target_formats_enums
 
     config = CommonConfig(
         Framework.TENSORFLOW,
         model=model,
         dataloader=dataloader,
         target_formats=target_formats_enums,
         target_device=target_device,
-        workspace=workspace,
         sample_count=sample_count,
         _input_names=input_names,
         _output_names=output_names,
         batch_dim=0 if batching else None,
         runner_names=runner_names,
-        profiler_config=profiler_config,
+        optimization_profile=optimization_profile,
         forward_kw_names=forward_kw_names,
         verbose=verbose,
         debug=debug,
         verify_func=verify_func,
         custom_configs=map_custom_configs(custom_configs=custom_configs),
     )
 
@@ -149,19 +146,20 @@
 
     builders = [
         preprocessing_builder,
         tensorflow_export_builder,
         find_device_max_batch_size_builder,
         tensorflow_conversion_builder,
         correctness_builder,
+        performance_builder,
+        verify_builder,
     ]
-    if profiler_config.run_profiling:
-        builders.append(profiling_builder)
-    builders.append(verify_builder)
 
-    package = PipelineManager.run(
-        pipeline_builders=builders,
+    package = optimize_pipeline(
+        model=model,
+        workspace=workspace,
+        builders=builders,
         config=config,
         models_config=models_config,
     )
 
     return package
```

## model_navigator/api/torch.py

```diff
@@ -8,64 +8,63 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Torch optimize API."""
-from pathlib import Path
+import pathlib
 from typing import Mapping, Optional, Sequence, Tuple, Type, Union
 
 import torch  # pytype: disable=import-error
 
 from model_navigator.api.config import (
     DEFAULT_TORCH_TARGET_FORMATS,
     CustomConfig,
     DeviceKind,
     Format,
-    ProfilerConfig,
+    OptimizationProfile,
     SizedDataLoader,
     VerifyFunction,
     map_custom_configs,
 )
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config_builder import ModelConfigBuilder
 from model_navigator.core.constants import DEFAULT_SAMPLE_COUNT
-from model_navigator.core.package import Package
+from model_navigator.core.logger import LOGGER
 from model_navigator.frameworks import Framework
 from model_navigator.frameworks.torch.utils import update_allowed_batching_parameters
-from model_navigator.logger import LOGGER
+from model_navigator.package.package import Package
 from model_navigator.pipelines.builders import (
     correctness_builder,
+    performance_builder,
     preprocessing_builder,
-    profiling_builder,
     torch_conversion_builder,
     torch_export_builder,
     verify_builder,
 )
 from model_navigator.pipelines.builders.find_device_max_batch_size import find_device_max_batch_size_builder
-from model_navigator.pipelines.pipeline_manager import PipelineManager
+from model_navigator.pipelines.wrappers.optimize import optimize_pipeline
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runners.utils import default_runners
 from model_navigator.utils import enums
-from model_navigator.utils.common import get_default_workspace
 
 
 def optimize(
     model: torch.nn.Module,
     dataloader: SizedDataLoader,
     sample_count: Optional[int] = DEFAULT_SAMPLE_COUNT,
     batching: Optional[bool] = True,
     input_names: Optional[Tuple[str, ...]] = None,
     output_names: Optional[Tuple[str, ...]] = None,
-    target_formats: Optional[Union[Union[str, Format], Tuple[Union[str, Format], ...]]] = None,
+    target_formats: Optional[Tuple[Union[str, Format], ...]] = None,
     target_device: Optional[DeviceKind] = DeviceKind.CUDA,
-    runners: Optional[Union[Union[str, Type[NavigatorRunner]], Tuple[Union[str, Type[NavigatorRunner]], ...]]] = None,
-    profiler_config: Optional[ProfilerConfig] = None,
-    workspace: Optional[Path] = None,
+    runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
+    optimization_profile: Optional[OptimizationProfile] = None,
+    workspace: Optional[pathlib.Path] = None,
     verbose: Optional[bool] = False,
     debug: Optional[bool] = False,
     verify_func: Optional[VerifyFunction] = None,
     custom_configs: Optional[Sequence[CustomConfig]] = None,
 ) -> Package:
     """Entrypoint for Torch optimize.
 
@@ -77,26 +76,24 @@
         sample_count: Limits how many samples will be used from dataloader
         batching: Enable or disable batching on first (index 0) dimension of the model
         input_names: Model input names
         output_names: Model output names
         target_formats: Target model formats for optimize process
         target_device: Target device for optimize process, default is CUDA
         runners: Use only runners provided as parameter
-        profiler_config: Profiling config
+        optimization_profile: Optimization profile for conversion and profiling
         workspace: Workspace where packages will be extracted
         verbose: Enable verbose logging
         debug: Enable debug logging from commands
         verify_func: Function for additional model verification
         custom_configs: Sequence of CustomConfigs used to control produced artifacts
 
     Returns:
         Package descriptor representing created package.
     """
-    if workspace is None:
-        workspace = get_default_workspace()
     if target_formats is None:
         target_formats = DEFAULT_TORCH_TARGET_FORMATS
         if batching:
             target_formats, custom_configs = update_allowed_batching_parameters(
                 target_formats=target_formats,
                 custom_configs=custom_configs,
             )
@@ -110,34 +107,33 @@
 
     if runners is None:
         runners = default_runners(device_kind=target_device)
 
     target_formats = enums.parse(target_formats, Format)
     runner_names = enums.parse(runners, lambda runner: runner if isinstance(runner, str) else runner.name())
 
-    if profiler_config is None:
-        profiler_config = ProfilerConfig()
+    if optimization_profile is None:
+        optimization_profile = OptimizationProfile()
 
     if Format.TORCH not in target_formats:
         target_formats = (Format.TORCH,) + target_formats
 
     config = CommonConfig(
         framework=Framework.TORCH,
         model=model,
         dataloader=dataloader,
         target_formats=target_formats,
-        workspace=workspace,
         sample_count=sample_count,
         _input_names=input_names,
         _output_names=output_names,
         target_device=target_device,
         forward_kw_names=forward_kw_names,
         batch_dim=0 if batching else None,
         runner_names=runner_names,
-        profiler_config=profiler_config,
+        optimization_profile=optimization_profile,
         verbose=verbose,
         debug=debug,
         verify_func=verify_func,
         custom_configs=map_custom_configs(custom_configs=custom_configs),
     )
 
     models_config = ModelConfigBuilder.generate_model_config(
@@ -148,19 +144,20 @@
 
     builders = [
         preprocessing_builder,
         torch_export_builder,
         find_device_max_batch_size_builder,
         torch_conversion_builder,
         correctness_builder,
+        performance_builder,
+        verify_builder,
     ]
-    if profiler_config.run_profiling:
-        builders.append(profiling_builder)
-    builders.append(verify_builder)
 
-    package = PipelineManager.run(
-        pipeline_builders=builders,
+    package = optimize_pipeline(
+        model=model,
+        workspace=workspace,
+        builders=builders,
         config=config,
         models_config=models_config,
     )
 
     return package
```

## model_navigator/commands/base.py

```diff
@@ -12,56 +12,94 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Base module for commands common classes and helpers."""
 import abc
 from dataclasses import dataclass
 from enum import Enum
 from inspect import getfullargspec
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Type
+from typing import Any, Callable, Dict, List, Optional, Type
 
-from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
+from model_navigator.exceptions import ModelNavigatorWrongParameterError
 from model_navigator.runners.base import NavigatorRunner
-
-if TYPE_CHECKING:
-    from model_navigator.core.status import Status
+from model_navigator.utils.common import DataObject
 
 
 class CommandStatus(str, Enum):
     """Status for commands."""
 
     OK = "OK"
     FAIL = "FAIL"
     NOOP = "NOOP"
     INITIALIZED = "INITIALIZED"
     SKIPPED = "SKIPPED"
 
 
 @dataclass
-class CommandOutput:
+class CommandOutput(DataObject):
     """Command output dataclass structure."""
 
     status: CommandStatus
     output: Optional[Dict[str, Any]] = None
-    save: bool = False
 
+    @classmethod
+    def from_dict(cls, data_dict: Dict) -> "CommandOutput":
+        """Create CommandOutput from the dictionary.
+
+        Args:
+            data_dict (Dict): dictionary with command output data.
+
+        Returns:
+            CommandOutput
+        """
+        return cls(status=CommandStatus(data_dict["status"]), output=data_dict["output"])
+
+
+class CommandMeta(abc.ABCMeta):  # noqa: B024
+    """Metaclass for command."""
+
+    @property
+    def name(cls):
+        """Return name of the command.
+
+        Return:
+            Name of command as a string
+        """
+        return cls.__name__
 
-class Command(abc.ABC):
+
+class Command(metaclass=CommandMeta):
     """Base class for command definition."""
 
     _is_required: bool = False
+    _requires: Optional[List[str]] = None
 
-    def __init_subclass__(cls, is_required: bool = False, **kwargs):
+    def __init_subclass__(cls, is_required: bool = False, requires: Optional[List[str]] = None, **kwargs):
         """Initialization of a command subclass."""
         super().__init_subclass__(**kwargs)
         cls._is_required = is_required
+        cls._requires = requires if requires is not None else []
 
-    def __init__(self, status: Optional["Status"] = None) -> None:
-        """Initialization of a command."""
-        self._status = status
+    @classmethod
+    def is_required(cls):
+        """Indicates if Command should be considered as required.
+
+        Returns:
+            True if required, False otherwise
+        """
+        return cls._is_required
+
+    @classmethod
+    def requires(cls):
+        """Return required commands to execute current command.
+
+        Returns:
+            List of required commands
+        """
+        return cls._requires
 
     def run(self, *args, **kwargs) -> CommandOutput:
         """Run command execution.
 
         Args:
             *args: Positional arguments
             **kwargs: Keyword arguments
@@ -112,55 +150,34 @@
         Args:
             output: Command output
             *args: Positional arguments
             **kwargs: Keyword arguments
         """
         pass
 
-    @classmethod
-    def is_required(cls):
-        """Indicates if Command should be considered as required.
-
-        Returns:
-            True if required, False otherwise
-        """
-        return cls._is_required
-
-    @classmethod
-    def name(cls) -> str:
-        """Return name of the command.
-
-        Return:
-            Name of command as a string
-        """
-        return cls.__name__
-
-    @property
-    def status(self) -> Optional["Status"]:
-        """Return navigator status."""
-        return self._status
-
 
 class ExecutionUnit:
     """Command along with configuration and runner."""
 
     def __init__(
         self,
+        *,
         command: Type[Command],
-        config: CommonConfig,
         model_config: Optional[ModelConfig] = None,
         runner_cls: Optional[Type[NavigatorRunner]] = None,
         **kwargs,
     ) -> None:
         """Initialize object.
 
         Args:
             command: A command to execute
             config: Global configuration provide by user
             model_config: Optional configuration of model that has to be produced by command
             runner_cls: Optional runner for correctness or performance evaluation
         """
         self.command = command
-        self.config = config
         self.model_config = model_config
         self.runner_cls = runner_cls
         self.kwargs = kwargs
+
+        if self.runner_cls and not self.model_config:
+            raise ModelNavigatorWrongParameterError("Unable to execute unit with runner without a model.")
```

## model_navigator/commands/infer_metadata.py

```diff
@@ -8,28 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Inputs and outputs metadata commands."""
-from pathlib import Path
+import pathlib
 from typing import Dict, Iterator, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
-from model_navigator.api.config import Sample, SizedDataLoader, SizedIterable, TensorRTProfile
+from model_navigator.api.config import OptimizationProfile, SizedDataLoader, SizedIterable, TensorRTProfile
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
-from model_navigator.core.tensor import TensorMetadata, TensorSpec
+from model_navigator.commands.execution_context import ExecutionContext
+from model_navigator.core.logger import LOGGER
+from model_navigator.core.tensor import FRAMEWORK_TO_TENSOR_TYPE, TensorMetadata, TensorSpec
+from model_navigator.core.workspace import Workspace
 from model_navigator.exceptions import ModelNavigatorUserInputError
-from model_navigator.execution_context import ExecutionContext
 from model_navigator.frameworks import Framework
-from model_navigator.logger import LOGGER
 from model_navigator.runners.utils import get_format_default_runners
-from model_navigator.utils.dataloader import extract_sample, sample_to_tuple, validate_sample_input
+from model_navigator.utils.dataloader import extract_sample, load_samples, sample_to_tuple, validate_sample_input
 from model_navigator.utils.devices import is_cuda_available
 from model_navigator.utils.format_helpers import FRAMEWORK2BASE_FORMAT
 
 
 def _extract_axes_shapes(
     dataloader: Union[SizedDataLoader, Iterator],
     input_names: Sequence[str],
@@ -43,26 +44,39 @@
     ), "dataloader is not an instance of SizedDataLoader, unable to check length."
 
     axes_shapes = {name: {ax: [] for ax in range(ndim)} for name, ndim in zip(input_names, input_ndims)}
     for i, sample in enumerate(dataloader):
         if i >= num_samples:
             LOGGER.warning(f"{len(dataloader)=}, but more samples found.")
             break
-        validate_sample_input(sample, framework)
+        validate_sample_input(sample, FRAMEWORK_TO_TENSOR_TYPE[framework])
         sample = extract_sample(sample, input_names, framework)
         for name, tensor in sample.items():
             for k, dim in enumerate(tensor.shape):
                 axes_shapes[name][k].append(dim)
 
     if check_len:
         assert i + 1 >= len(dataloader), f"{len(dataloader)=}, but only {i + 1} samples found."
 
     return axes_shapes
 
 
+def _get_metadata_from_axes_shapes(axes_shapes, batch_dim, dtypes):
+    metadata = TensorMetadata()
+    for name, axes in axes_shapes.items():
+        tensor_shape = []
+        for ax, shapes in axes.items():
+            if ax == batch_dim or min(shapes) != max(shapes):
+                tensor_shape.append(-1)
+            else:
+                tensor_shape.append(shapes[0])
+        metadata.add(name, tuple(tensor_shape), dtypes[name])
+    return metadata
+
+
 def _extract_max_batch_size(axes_shapes: Dict[str, Dict[int, List[int]]], batch_dim: Optional[int]) -> int:
     if batch_dim is not None:
         return max(list(axes_shapes.values())[0][batch_dim])
     return 0
 
 
 def _get_trt_profile_from_axes_shapes(axes_shapes, batch_dim):
@@ -81,35 +95,23 @@
                 f"Missing shape information for {name} input from dataloader."
                 "Scalar values are not supported by Triton Inference Server."
                 "Wrap it in tuple to add dimension e.g. tensor(3) -> tensor((3,))"
             )
     return trt_profile
 
 
-def _get_metadata_from_axes_shapes(axes_shapes, batch_dim, dtypes):
-    metadata = TensorMetadata()
-    for name, axes in axes_shapes.items():
-        tensor_shape = []
-        for ax, shapes in axes.items():
-            if ax == batch_dim or min(shapes) != max(shapes):
-                tensor_shape.append(-1)
-            else:
-                tensor_shape.append(shapes[0])
-        metadata.add(name, tuple(tensor_shape), dtypes[name])
-    return metadata
-
-
 class InferInputMetadata(Command, is_required=True):
     """Command to collect model inputs metadata."""
 
     def _run(
         self,
-        model: Union[object, Path],
+        model: Union[object, pathlib.Path],
         framework: Framework,
         dataloader: SizedDataLoader,
+        optimization_profile: OptimizationProfile,
         _input_names: Optional[Tuple[str, ...]] = None,
         batch_dim: Optional[int] = None,
     ) -> CommandOutput:
         """Execute the InferInputMetadata command.
 
         Args:
             framework: Framework of model to run inference
@@ -118,48 +120,68 @@
             _input_names: Name of model inputs
             batch_dim: Location of batch dimension in data samples
 
         Returns:
             CommandOutput object
         """
         sample = next(iter(dataloader))
-        validate_sample_input(sample, framework)
+        validate_sample_input(sample, FRAMEWORK_TO_TENSOR_TYPE[framework])
         input_names = _input_names
         if input_names is None:
             input_names = self._get_default_input_names(model, sample, framework)
 
         input_sample = extract_sample(sample, input_names, framework)
         input_ndims = [t.ndim for t in input_sample.values()]
         input_dtypes = {n: t.dtype for n, t in input_sample.items()}
         num_samples = len(dataloader)
         axes_shapes = _extract_axes_shapes(dataloader, input_names, input_ndims, num_samples, framework)
         dataloader_max_batch_size = _extract_max_batch_size(axes_shapes, batch_dim)
         dataloader_trt_profile = _get_trt_profile_from_axes_shapes(axes_shapes, batch_dim)
-
         input_metadata = _get_metadata_from_axes_shapes(axes_shapes, batch_dim, input_dtypes)
+
+        if optimization_profile.dataloader:
+            pd_sample = next(iter(optimization_profile.dataloader))
+            pd_input_sample = extract_sample(pd_sample, input_names, framework)
+            pd_input_ndims = [t.ndim for t in pd_input_sample.values()]
+            pd_input_dtypes = {n: t.dtype for n, t in pd_input_sample.items()}
+
+            if pd_input_ndims != input_ndims:
+                raise ModelNavigatorUserInputError(
+                    "Provided performance dataloader does not match dataset dataloader size."
+                )
+
+            if pd_input_dtypes != input_dtypes:
+                raise ModelNavigatorUserInputError(
+                    "Provided performance dataloader does not match dataset dataloader data types."
+                )
+
+            self._validate_performance_dataloader_trt_profiles(
+                optimization_profile=optimization_profile,
+                input_names=input_names,
+                input_ndims=pd_input_ndims,
+                framework=framework,
+                batch_dim=batch_dim,
+                dataloader_trt_profile=dataloader_trt_profile,
+            )
+
         return CommandOutput(
             status=CommandStatus.OK,
             output={
                 "input_metadata": input_metadata,
                 "dataloader_trt_profile": dataloader_trt_profile,
                 "dataloader_max_batch_size": dataloader_max_batch_size,
             },
         )
 
-    @staticmethod
-    def _get_default_input_names(
-        model,
-        sample,
-        framework,
-    ):
+    def _get_default_input_names(self, model, sample, framework):
         input_tuple = sample_to_tuple(sample)
         if framework == Framework.ONNX:
             from model_navigator.runners.onnx import OnnxrtCPURunner, OnnxrtCUDARunner
 
-            assert isinstance(model, Path), "ONNX model must be a pathlib.Path"
+            assert isinstance(model, pathlib.Path), "ONNX model must be a pathlib.Path"
 
             onnxrt_runner_cls = OnnxrtCUDARunner if is_cuda_available() else OnnxrtCPURunner
             onnx_runner = onnxrt_runner_cls(
                 model=model,
                 input_metadata=TensorMetadata(),
                 output_metadata=TensorMetadata(),
                 disable_fallback=False,
@@ -169,27 +191,54 @@
                 input_names = tuple(input_metadata.keys())
         elif isinstance(sample, Mapping):
             input_names = tuple(sample.keys())
         else:
             input_names = tuple(f"input__{i}" for i in range(len(input_tuple)))
         return input_names
 
+    def _validate_performance_dataloader_trt_profiles(
+        self,
+        optimization_profile: OptimizationProfile,
+        input_names,
+        input_ndims,
+        framework,
+        batch_dim,
+        dataloader_trt_profile,
+    ):
+        axes_shapes = _extract_axes_shapes(
+            dataloader=optimization_profile.dataloader,
+            input_names=input_names,
+            input_ndims=input_ndims,
+            num_samples=1,
+            framework=framework,
+            check_len=False,
+        )
+        performance_dataloader_trt_profile = _get_trt_profile_from_axes_shapes(axes_shapes, batch_dim)
+        for name, shape in performance_dataloader_trt_profile.items():
+            dshape = dataloader_trt_profile[name]
+            if shape.min < dshape.min or shape.max > dshape.max:
+                raise ModelNavigatorUserInputError(
+                    """Provided performance dataloader has invalid shape against the dataset dataloader."""
+                    f""" Performance dataloader shape for input `{name}` is min: {shape.min}, max: {shape.max}."""
+                    f""" Dataset dataloader shape for input `{name}` is min: {dshape.min}, max: {dshape.max}."""
+                )
+
 
 class InferOutputMetadata(Command, is_required=True):
     """Command to collect model outputs  metadata."""
 
     def _run(
         self,
         framework: Framework,
-        model: Union[object, Path],
+        model: Union[object, pathlib.Path],
         dataloader: SizedDataLoader,
-        profiling_sample: Sample,
-        conversion_samples: List[Sample],
+        profiling_sample: pathlib.Path,
+        conversion_samples: pathlib.Path,
         input_metadata: TensorMetadata,
-        workspace: Path,
+        workspace: Workspace,
         verbose: bool,
         _output_names: Optional[Tuple[str, ...]] = None,
         dynamic_axes: Optional[Dict[str, Union[Dict[int, str], List[int]]]] = None,
         forward_kw_names: Optional[Tuple[str, ...]] = None,
         batch_dim: Optional[int] = None,
     ) -> CommandOutput:
         """Execute the InferOutputMetadata command.
@@ -220,14 +269,17 @@
             model=model,
             input_metadata=input_metadata,
             output_metadata=temp_output_metadata,
             input_metadata_mapping=forward_kw_names,
             disable_fallback=False,
         )  # pytype: disable=not-instantiable
 
+        profiling_sample = load_samples("profiling_sample", workspace.path, batch_dim)[0]
+        conversion_samples = load_samples("conversion_sample", workspace.path, batch_dim)
+
         with runner, ExecutionContext(workspace=workspace, verbose=verbose):
             output_sample = runner.infer(profiling_sample)
             output_names = list(output_sample.keys())
             output_generator = (runner.infer(sample) for sample in conversion_samples)
 
             output_ndims = [t.ndim for t in output_sample.values()]
             output_dtypes = {n: t.dtype for n, t in output_sample.items()}
```

## model_navigator/commands/load.py

```diff
@@ -9,31 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Commands for loading samples from the drive."""
 
-from pathlib import Path
 from typing import Optional
 
 import yaml
 
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
-from model_navigator.core.status import Status
+from model_navigator.core.workspace import Workspace
+from model_navigator.package.status import Status
 from model_navigator.utils.common import get_default_status_filename
 from model_navigator.utils.dataloader import load_samples
 
 
-class LoadMetadata(Command):
+class LoadMetadata(Command, is_required=True):
     """Load IO metadata from the status.yaml file."""
 
     def _run(
         self,
-        workspace: Path,
+        workspace: Workspace,
     ) -> CommandOutput:
         """Run loading IO metadata from the status.yaml.
 
         Metadata that are being loaded:
             1) Input metadata,
             2) Output metadata,
             3) TensorRT profile,
@@ -41,15 +41,15 @@
 
         Args:
             workspace (Path): Model Navigator workspace path.
 
         Returns:
             CommandOutput
         """
-        with open(workspace / get_default_status_filename()) as f:
+        with open(workspace.path / get_default_status_filename()) as f:
             status = Status.from_dict(yaml.safe_load(f))
         return CommandOutput(
             status=CommandStatus.OK,
             output={
                 "input_metadata": status.input_metadata,
                 "output_metadata": status.output_metadata,
                 "dataloader_trt_profile": status.dataloader_trt_profile,
@@ -59,42 +59,42 @@
 
 
 class LoadSamples(Command):
     """Load IO samples from the drive."""
 
     def _run(
         self,
-        workspace: Path,
+        workspace: Workspace,
         batch_dim: Optional[int] = None,
     ) -> CommandOutput:
         """Run loading IO samples.
 
         Samples that are being loaded:
             1) Profiling samples and it's output,
             2) Conversion samples and their outputs,
             3) Correctness samples and their outputs.
 
         Args:
-            workspace (Path): Model Navigator workspace path.
-            batch_dim (Optional[int], optional): Batch dimension. Defaults to None.
+            workspace: Model Navigator workspace path.
+            batch_dim: Batch dimension. Defaults to None.
 
         Returns:
             CommandOutput
         """
         samples_name = (
             "profiling_sample",
             "correctness_samples",
             "conversion_samples",
             "profiling_sample_output",
             "correctness_samples_output",
             "conversion_samples_output",
         )
         ret = {}
         for name in samples_name:
-            samples = load_samples(name, workspace, batch_dim)
+            samples = load_samples(name, workspace.path, batch_dim)
             if name.startswith("profiling"):
                 ret[name] = samples[0]
             else:
                 ret[name] = samples
 
         return CommandOutput(
             status=CommandStatus.OK,
```

## model_navigator/commands/convert/base.py

```diff
@@ -14,15 +14,15 @@
 """ConvertONNX2TRT command."""
 
 from typing import Callable, Generator, Optional
 
 from model_navigator.api.config import TensorRTProfile
 from model_navigator.commands.base import Command
 from model_navigator.core.constants import DEFAULT_MAX_BATCH_SIZE_HALVING
-from model_navigator.logger import LOGGER
+from model_navigator.core.logger import LOGGER
 
 
 class Convert2TensorRTWithMaxBatchSizeSearch(Command):
     """Command that converts models with conversion max batch size search."""
 
     @classmethod
     def _execute_conversion(
```

## model_navigator/commands/convert/tf.py

```diff
@@ -8,35 +8,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Saved Model conversions."""
-from pathlib import Path
+import pathlib
 from typing import Optional
 
 from model_navigator.api.config import TensorRTPrecision, TensorRTProfile
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
 from model_navigator.commands.convert.base import Convert2TensorRTWithMaxBatchSizeSearch
 from model_navigator.commands.convert.converters import sm2tftrt
-from model_navigator.execution_context import ExecutionContext
-from model_navigator.logger import LOGGER
+from model_navigator.commands.execution_context import ExecutionContext
+from model_navigator.core.logger import LOGGER
+from model_navigator.core.workspace import Workspace
 from model_navigator.utils import devices
 from model_navigator.utils.common import parse_kwargs_to_cmd
 
 
 class ConvertSavedModel2ONNX(Command):
     """Convert SavedModel to ONNX."""
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
-        parent_path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
+        parent_path: pathlib.Path,
         opset: int,
         verbose: bool,
     ) -> CommandOutput:
         """Run Conversion from SavedModel to ONNX.
 
         Args:
             workspace (Path): Navigator workspace.
@@ -46,30 +47,30 @@
             verbose (bool): If True verbose logging.
 
         Returns:
             CommandOutput: Conversion output.
         """
         LOGGER.info("SavedModel to ONNX conversion started")
 
-        exported_model_path = workspace / parent_path
-        converted_model_path = workspace / path
+        exported_model_path = workspace.path / parent_path
+        converted_model_path = workspace.path / path
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported SavedModel model not found at {exported_model_path}. Skipping conversion")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         convert_cmd = [
             "python",
             "-m",
             "tf2onnx.convert",
             "--saved-model",
-            exported_model_path.relative_to(workspace).as_posix(),
+            exported_model_path.relative_to(workspace.path).as_posix(),
             "--output",
-            converted_model_path.relative_to(workspace).as_posix(),
+            converted_model_path.relative_to(workspace.path).as_posix(),
             "--opset",
             str(opset),
         ]
 
         with ExecutionContext(
             workspace=workspace,
             cmd_path=converted_model_path.parent / "reproduce_conversion.sh",
@@ -83,17 +84,17 @@
 class ConvertSavedModel2TFTRT(Convert2TensorRTWithMaxBatchSizeSearch):
     """Convert SavedModel to Tensorflow-TensorRT."""
 
     def _run(
         self,
         max_workspace_size: int,
         minimum_segment_size: int,
-        workspace: Path,
-        path: Path,
-        parent_path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
+        parent_path: pathlib.Path,
         precision: TensorRTPrecision,
         verbose: bool,
         dataloader_trt_profile: TensorRTProfile,
         batch_dim: Optional[int] = None,
         dataloader_max_batch_size: Optional[int] = None,
         device_max_batch_size: Optional[int] = None,
         trt_profile: Optional[TensorRTProfile] = None,
@@ -122,16 +123,16 @@
         Returns:
             CommandOutput: Conversion output.
         """
         LOGGER.info("SavedModel to Tensorflow-TensorRT conversion started")
         if not devices.get_available_gpus():
             raise RuntimeError("No GPUs available.")
 
-        exported_model_path = workspace / parent_path
-        converted_model_path = workspace / path
+        exported_model_path = workspace.path / parent_path
+        converted_model_path = workspace.path / path
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported SavedModel model not found at {exported_model_path}. Skipping conversion")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         custom_trt_profile = trt_profile
@@ -145,21 +146,21 @@
             max_batch_size = None
 
         if trt_profile is not None:
             LOGGER.info("TF-TensorRT conversion currently does not support custom profiles.")
 
         def get_args(max_batch_size: int = max_batch_size):
             kwargs = {
-                "exported_model_path": exported_model_path.relative_to(workspace).as_posix(),
-                "converted_model_path": converted_model_path.relative_to(workspace).as_posix(),
+                "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
+                "converted_model_path": converted_model_path.relative_to(workspace.path).as_posix(),
                 "max_workspace_size": max_workspace_size,
                 "target_precision": precision.value,
                 "minimum_segment_size": minimum_segment_size,
                 "batch_dim": batch_dim,
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
                 "max_batch_size": max_batch_size,
             }
 
             args = parse_kwargs_to_cmd(kwargs)
             return args
 
         with ExecutionContext(
```

## model_navigator/commands/convert/torch.py

```diff
@@ -9,37 +9,38 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """TorchScript conversions."""
 
-from pathlib import Path
+import pathlib
 from typing import Optional, Tuple
 
 from model_navigator.api.config import DeviceKind, TensorRTPrecision, TensorRTPrecisionMode, TensorRTProfile
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
 from model_navigator.commands.convert.base import Convert2TensorRTWithMaxBatchSizeSearch
 from model_navigator.commands.convert.converters import ts2onnx, ts2torchtrt
+from model_navigator.commands.execution_context import ExecutionContext
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.execution_context import ExecutionContext
+from model_navigator.core.workspace import Workspace
 from model_navigator.frameworks.tensorrt import utils as tensorrt_utils
-from model_navigator.logger import LOGGER
 from model_navigator.utils import devices
 from model_navigator.utils.common import parse_kwargs_to_cmd
 
 
 class ConvertTorchScript2ONNX(Command):
     """Convert TorchScript to ONNX."""
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
-        parent_path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
+        parent_path: pathlib.Path,
         opset: int,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         target_device: DeviceKind,
         verbose: bool,
         forward_kw_names: Optional[Tuple[str, ...]] = None,
         batch_dim: Optional[int] = None,
@@ -59,28 +60,28 @@
                 Defaults to None.
             batch_dim (Optional[int], optional): Batch dimension. Defaults to None.
 
         Returns:
             CommandOutput: Status OK.
         """
         LOGGER.info("TorchScript to ONNX conversion started")
-        exported_model_path = workspace / parent_path
-        converted_model_path = workspace / path
+        exported_model_path = workspace.path / parent_path
+        converted_model_path = workspace.path / path
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         with ExecutionContext(
             workspace=workspace,
             script_path=converted_model_path.parent / "reproduce_conversion.py",
             cmd_path=converted_model_path.parent / "reproduce_conversion.sh",
             verbose=verbose,
         ) as context:
             kwargs = {
-                "workspace": workspace.as_posix(),
-                "exported_model_path": exported_model_path.relative_to(workspace).as_posix(),
-                "converted_model_path": converted_model_path.relative_to(workspace).as_posix(),
+                "workspace": workspace.path.as_posix(),
+                "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
+                "converted_model_path": converted_model_path.relative_to(workspace.path).as_posix(),
                 "opset": opset,
                 "input_names": list(input_metadata.keys()),
                 "output_names": list(output_metadata.keys()),
                 "dynamic_axes": dict(**input_metadata.dynamic_axes, **output_metadata.dynamic_axes),
                 "batch_dim": batch_dim,
                 "forward_kw_names": list(forward_kw_names) if forward_kw_names else None,
                 "target_device": target_device.value,
@@ -94,17 +95,17 @@
 
 
 class ConvertTorchScript2TorchTensorRT(Convert2TensorRTWithMaxBatchSizeSearch):
     """Convert TorchScript to Torch-TensorRT."""
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
-        parent_path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
+        parent_path: pathlib.Path,
         precision: TensorRTPrecision,
         input_metadata: TensorMetadata,
         precision_mode: TensorRTPrecisionMode,
         max_workspace_size: int,
         target_device: DeviceKind,
         verbose: bool,
         debug: bool,
@@ -144,16 +145,17 @@
 
         Returns:
             CommandOutput: Status OK.
         """
         LOGGER.info("Conversion TorchScript to TorchTensorRT started")
         if not devices.get_available_gpus():
             raise RuntimeError("No GPUs available.")
-        exported_model_path = workspace / parent_path
-        converted_model_path = workspace / path
+
+        exported_model_path = workspace.path / parent_path
+        converted_model_path = workspace.path / path
 
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported TorchScript model not found at {exported_model_path}. Skipping conversion.")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         custom_trt_profile = trt_profile
         trt_profile = self._get_trt_profile(
@@ -163,23 +165,23 @@
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         input_dtypes_str = [tensorrt_utils.cast_type(input_spec.dtype).name for input_spec in input_metadata.values()]
 
         def get_args(max_batch_size=None):
             shapes = self._get_shape_args(trt_profile=trt_profile, batch_dim=batch_dim, max_batch_size=max_batch_size)
             kwargs = {
-                "exported_model_path": exported_model_path.relative_to(workspace).as_posix(),
-                "converted_model_path": converted_model_path.relative_to(workspace).as_posix(),
+                "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
+                "converted_model_path": converted_model_path.relative_to(workspace.path).as_posix(),
                 "shapes": shapes,
                 "input_dtypes": input_dtypes_str,
                 "max_workspace_size": max_workspace_size,
                 "precision": precision.value,
                 "precision_mode": precision_mode.value,
                 "target_device": target_device.value,
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
                 "debug": debug,
             }
             args = parse_kwargs_to_cmd(kwargs)
             return args
 
         with ExecutionContext(
             workspace=workspace,
```

## model_navigator/commands/convert/onnx/onnx2trt.py

```diff
@@ -13,42 +13,42 @@
 # limitations under the License.
 """ConvertONNX2TRT command."""
 import json
 import pathlib
 import sys
 import tempfile
 from distutils.version import LooseVersion
-from pathlib import Path
 from typing import Optional
 
 from model_navigator.api.config import (
     TensorRTCompatibilityLevel,
     TensorRTPrecision,
     TensorRTPrecisionMode,
     TensorRTProfile,
 )
 from model_navigator.commands.base import CommandOutput, CommandStatus
 from model_navigator.commands.convert.base import Convert2TensorRTWithMaxBatchSizeSearch
+from model_navigator.commands.execution_context import ExecutionContext
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.execution_context import ExecutionContext
+from model_navigator.core.workspace import Workspace
 from model_navigator.frameworks.tensorrt import utils as tensorrt_utils
-from model_navigator.logger import LOGGER
 from model_navigator.runners.tensorrt import TensorRTRunner
 from model_navigator.utils import devices
 from model_navigator.utils.common import parse_kwargs_to_cmd
 
 
 class ConvertONNX2TRT(Convert2TensorRTWithMaxBatchSizeSearch):
     """Command that converts ONNX checkpoint to TensorRT model plan."""
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
-        parent_path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
+        parent_path: pathlib.Path,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         precision: TensorRTPrecision,
         precision_mode: TensorRTPrecisionMode,
         dataloader_trt_profile: TensorRTProfile,
         max_workspace_size: Optional[int] = None,
         batch_dim: Optional[int] = None,
@@ -84,16 +84,16 @@
         Returns:
             CommandOutput: Status and results of the command.
         """
         LOGGER.info("ONNX to TRT conversion started")
         if not devices.get_available_gpus():
             raise RuntimeError("No GPUs available.")
 
-        input_model_path = workspace / parent_path
-        converted_model_path = workspace / path
+        input_model_path = workspace.path / parent_path
+        converted_model_path = workspace.path / path
 
         if not input_model_path.exists():
             LOGGER.warning(f"Exported ONNX model not found at {input_model_path}. Skipping conversion.")
             return CommandOutput(status=CommandStatus.SKIPPED)
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         custom_trt_profile = trt_profile
@@ -106,17 +106,17 @@
             input_metadata=input_metadata,
             output_metadata=output_metadata,
             workspace=workspace,
             reproduce_script_path=converted_model_path.parent,
             verbose=verbose,
         )
 
-        convert_cmd = ["polygraphy", "convert", input_model_path.relative_to(workspace).as_posix()]
+        convert_cmd = ["polygraphy", "convert", input_model_path.relative_to(workspace.path).as_posix()]
         convert_cmd.extend(["--convert-to", "trt"])
-        convert_cmd.extend(["-o", converted_model_path.relative_to(workspace).as_posix()])
+        convert_cmd.extend(["-o", converted_model_path.relative_to(workspace.path).as_posix()])
 
         if optimization_level is not None:
             convert_cmd.extend(["--builder-optimization-level", optimization_level])
 
         if compatibility_level is not None:
             convert_cmd.extend(["--hardware-compatibility-level", compatibility_level.value])
 
@@ -155,15 +155,15 @@
         with ExecutionContext(
             workspace=workspace,
             cmd_path=converted_model_path.parent / "reproduce_conversion.sh",
             verbose=verbose,
         ) as context:
             kwargs = {
                 "batch_dim": batch_dim,
-                "model_path": converted_model_path.relative_to(workspace).as_posix(),
+                "model_path": converted_model_path.relative_to(workspace.path).as_posix(),
                 "runner_name": TensorRTRunner.name(),
                 "input_metadata": input_metadata.to_json(),
                 "output_metadata": output_metadata.to_json(),
             }
 
             load_args = parse_kwargs_to_cmd(kwargs)
             from . import trt_load_script
@@ -208,29 +208,29 @@
             if shapes:
                 shape_args.extend([f"{arg}"] + shapes)
 
         return shape_args
 
     def _get_onnx_input_metadata(
         self,
-        workspace: pathlib.Path,
+        workspace: Workspace,
         input_model_path: pathlib.Path,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         reproduce_script_path: pathlib.Path,
         verbose: bool,
     ):
         with ExecutionContext(
             script_path=reproduce_script_path / "reproduce_onnx_input_metadata.py",
             cmd_path=reproduce_script_path / "reproduce_onnx_input_metadata.sh",
             workspace=workspace,
             verbose=verbose,
         ) as context, tempfile.NamedTemporaryFile() as temp_file:
             kwargs = {
-                "model_path": input_model_path.relative_to(workspace).as_posix(),
+                "model_path": input_model_path.relative_to(workspace.path).as_posix(),
                 "input_metadata": input_metadata.to_json(),
                 "output_metadata": output_metadata.to_json(),
                 "results_path": temp_file.name,
             }
             args = parse_kwargs_to_cmd(kwargs)
             from . import collect_onnx_input_metadata
```

## model_navigator/commands/copy/onnx.py

```diff
@@ -9,41 +9,42 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Command for copying ONNX model."""
 
+import pathlib
 import shutil
-from pathlib import Path
 from typing import Optional
 
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
+from model_navigator.core.workspace import Workspace
 
 
 class CopyONNX(Command):
     """ONNX copy command."""
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
-        model: Optional[Path] = None,
+        workspace: Workspace,
+        path: pathlib.Path,
+        model: Optional[pathlib.Path] = None,
     ) -> CommandOutput:
         """Run copy of the ONNX model.
 
         Args:
             workspace (Path): Model Navigator workspace path.
             path (Path): ONNX model path to copy to. Relative to workspace path.
             model (Optional[Path], optional): ONNX model path to copy from. Defaults to None.
 
         Returns:
             CommandOutput: Status OK.
         """
-        destination_model_path = workspace / path
+        destination_model_path = workspace.path / path
         if destination_model_path.exists():
             return CommandOutput(status=CommandStatus.SKIPPED)
         assert model is not None
         destination_model_path.parent.mkdir(parents=True, exist_ok=True)
         shutil.copy(src=model, dst=destination_model_path)
 
         return CommandOutput(status=CommandStatus.OK)
```

## model_navigator/commands/correctness/correctness.py

```diff
@@ -10,24 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Correctness command and it's results."""
 
 import json
+import pathlib
 import tempfile
 from dataclasses import dataclass
-from pathlib import Path
 from typing import Any, Dict, List, Optional, Type
 
 from model_navigator.api.config import Format
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
+from model_navigator.commands.execution_context import ExecutionContext
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.execution_context import ExecutionContext
-from model_navigator.logger import LOGGER
+from model_navigator.core.workspace import Workspace
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.utils.common import DataObject, parse_kwargs_to_cmd
 from model_navigator.utils.format_helpers import is_source_format
 
 
 @dataclass
 class Tolerance(DataObject):
@@ -80,21 +81,21 @@
 
 
 class Correctness(Command):
     """Correctness Command."""
 
     def _run(
         self,
-        workspace: Path,
+        workspace: Workspace,
         format: Format,
         runner_cls: Type[NavigatorRunner],
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         batch_dim: Optional[int],
-        path: Path,
+        path: pathlib.Path,
         verbose: bool,
         model: Optional[Any] = None,
     ) -> CommandOutput:
         """Run correcntess command.
 
         Args:
             workspace (Path): Model Navigator worksapce path.
@@ -109,29 +110,29 @@
                 Defaults to None.
 
         Returns:
             CommandOutput: Status OK and TolerancePerOutputName of the model with runner.
         """
         per_output_tolerance = None
         LOGGER.info(f"Correctness test for: {format} {runner_cls} started.")
-        model_path = workspace / path
+        model_path = workspace.path / path
         model_dir = model_path.parent
 
         if not is_source_format(format) and not model_path.exists():
             LOGGER.warning(f"Model: {model_path.as_posix()!r} not found, command skipped.")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         with ExecutionContext(
             workspace=workspace,
             script_path=model_dir / "reproduce_correctness.py",
             cmd_path=model_dir / "reproduce_correctness.sh",
             verbose=verbose,
         ) as context, tempfile.NamedTemporaryFile() as temp_file:
             kwargs = {
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
                 "batch_dim": batch_dim,
                 "results_path": temp_file.name,
                 "runner_name": runner_cls.name(),
                 "input_metadata": input_metadata.to_json(),
                 "output_metadata": output_metadata.to_json(),
             }
```

## model_navigator/commands/correctness/correctness_script.py

```diff
@@ -18,16 +18,16 @@
 import sys
 from typing import List, Optional
 
 import fire
 import numpy as np
 
 from model_navigator.commands.correctness.correctness import Tolerance, TolerancePerOutputName
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.logger import LOGGER
 from model_navigator.runners.registry import get_runner
 from model_navigator.utils.dataloader import load_samples
 
 
 def get_model() -> object:
     """Get model instance.
 
@@ -84,24 +84,28 @@
     per_output_tolerance = TolerancePerOutputName({name: Tolerance(0.0, 0.0) for name in output_metadata})
     with runner:
         for sample, original_output in zip(correctness_samples, correctness_samples_output):
             comp_output = runner.infer(sample)
 
             is_len_valid = len(original_output) == len(comp_output)
             if not is_len_valid:
-                LOGGER.error("Original model output length is different from exported model output")
+                LOGGER.error(
+                    """Original model output length is different from exported model output"""
+                    f"""Original output: {original_output}"""
+                    f"""Computed output: {comp_output}"""
+                )
                 sys.exit(1)
 
             for name in output_metadata:
                 if any(np.isnan(comp_output[name]).flatten()):
-                    LOGGER.error("Comparison output contains NaN")
+                    LOGGER.error(f"Comparison output {name} contains NaN")
                     sys.exit(1)
 
                 if any(np.isinf(comp_output[name]).flatten()):
-                    LOGGER.error("Comparison output contains inf")
+                    LOGGER.error(f"Comparison output {name} contains inf")
                     sys.exit(1)
 
                 out0, out1 = original_output[name], comp_output[name]
                 absdiff = np.abs(out0 - out1)
                 absout1 = np.abs(out1)
 
                 reldiff = absdiff / absout1
```

## model_navigator/commands/data_dump/samples.py

```diff
@@ -8,29 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Commands for fetching and dumping model IO."""
-
-from pathlib import Path
+import pathlib
 from typing import Any, List, Optional, Tuple
 
-import numpy
 import numpy as np
 
-from model_navigator.api.config import Sample, SizedDataLoader, TensorRTProfile
+from model_navigator.api.config import OptimizationProfile, Sample, SizedDataLoader, TensorRTProfile
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
+from model_navigator.core.workspace import Workspace
 from model_navigator.exceptions import ModelNavigatorUserInputError
 from model_navigator.frameworks import Framework
-from model_navigator.logger import LOGGER
 from model_navigator.runners.utils import get_format_default_runners
-from model_navigator.utils.dataloader import extract_bs1, extract_sample
+from model_navigator.utils.dataloader import extract_bs1, extract_sample, load_samples
 from model_navigator.utils.format_helpers import FRAMEWORK2BASE_FORMAT
 
 
 def _validate_tensor(tensor: np.ndarray, *, raise_on_error: bool = True):
     if any(np.isnan(tensor.flatten())):
         message = "Tensor data contains `NaN` value. Please verify the dataloader and model."
         if raise_on_error:
@@ -42,15 +41,17 @@
         message = "Tensor data contains `inf` value. Please verify the dataloader and model."
         if raise_on_error:
             raise ModelNavigatorUserInputError(message)
         else:
             LOGGER.warning(message)
 
 
-def samples_to_npz(samples: List[Sample], path: Path, batch_dim: Optional[int], *, raise_on_error: bool = True) -> None:
+def samples_to_npz(
+    samples: List[Sample], path: pathlib.Path, batch_dim: Optional[int], *, raise_on_error: bool = True
+) -> None:
     """Save samples to .npz files. Each sample is saved to `path/{sample index}.npz` file.
 
     Args:
         samples (List[Sample]): Samples to save.
         path (Path): Output directory.
         batch_dim (Optional[int]): Batch dimension
         raise_on_error (bool, optional): If True raise an error when sample is invalid. Defaults to True.
@@ -70,65 +71,89 @@
 
 
 class FetchInputModelData(Command, is_required=True):
     """Command for fetching input samples from the dataloader."""
 
     def _run(
         self,
+        workspace: Workspace,
         framework: Framework,
         dataloader: SizedDataLoader,
         sample_count: int,
         input_metadata: TensorMetadata,
         batch_dim: Optional[int],
         seed: int,
         dataloader_trt_profile: TensorRTProfile,
+        optimization_profile: OptimizationProfile,
+        raise_on_error: Optional[bool] = False,
     ) -> CommandOutput:
         """Run the command.
 
         There are three types of samples that are fetched form the dataloader:
             1) profiling sample - one sample for profiling,
             2) conversion samples - samples spanning all dimensions sizes from min to max,
-            3) correctness samples - `sample_count` samples for veryfing correctness.
+            3) correctness samples - `sample_count` samples for verifying correctness.
 
         Args:
-            framework (Framework): Model framework.
-            dataloader (SizedDataLoader): Dataloader for the model.
-            sample_count (int): Number of correctness samples to fetch.
-            input_metadata (TensorMetadata): Input metadata.
-            batch_dim (Optional[int]): Batch dimension.
-            seed (int): Random seed.
-            trt_profile (Profile): Model TensorRT Profile.
+            workspace: Workspace of current execution.
+            framework: Model framework.
+            dataloader: Dataloader for the model.
+            sample_count: Number of correctness samples to fetch.
+            input_metadata: Input metadata.
+            batch_dim: Batch dimension.
+            seed: Random seed.
+            dataloader_trt_profile: Model TensorRT Profile.
+            optimization_profile: Performance configuration with dataloader override
+            raise_on_error: If True raise an error when one of the samples is invalid. Defaults to False.
 
         Returns:
             CommandOutput: Fetched samples.
         """
         num_samples = len(dataloader)
         if sample_count > num_samples:
             LOGGER.warning(
                 f"Requested sample_count ({sample_count}) is larger than "
                 f"the number of available samples ({num_samples}). Using {num_samples} samples."
             )
             sample_count = num_samples
 
-        numpy.random.seed(seed)
-        correctness_samples_ind = set(numpy.random.choice(num_samples, size=sample_count, replace=False))
+        LOGGER.info("Collecting input samples for model.")
+        np.random.seed(seed)
+        correctness_samples_ind = set(np.random.choice(num_samples, size=sample_count, replace=False))
         profiling_sample, correctness_samples, conversion_samples = self._collect_samples(
-            dataloader, input_metadata, dataloader_trt_profile, framework, batch_dim, correctness_samples_ind
-        )
-        return CommandOutput(
-            status=CommandStatus.OK,
-            output={
-                "profiling_sample": profiling_sample,
-                "correctness_samples": correctness_samples,
-                "conversion_samples": conversion_samples,
-            },
+            dataloader,
+            input_metadata,
+            dataloader_trt_profile,
+            framework,
+            batch_dim,
+            correctness_samples_ind,
+            optimization_profile.dataloader,
         )
 
+        sample_data_path = workspace.path / "model_input"
+        sample_data_path.mkdir(parents=True, exist_ok=True)
+
+        output = {}
+
+        LOGGER.info("Saving samples into the workspace.")
+        for samples, dirname, sample_name in [
+            ([profiling_sample], "profiling", "profiling_sample"),
+            (correctness_samples, "correctness", "correctness_samples"),
+            (conversion_samples, "conversion", "conversion_samples"),
+        ]:
+            sample_path = sample_data_path / dirname
+            samples_to_npz(samples, sample_path, batch_dim, raise_on_error=raise_on_error)
+            output[sample_name] = sample_path
+
+        return CommandOutput(status=CommandStatus.OK, output=output)
+
     @staticmethod
-    def _collect_samples(dataloader, input_metadata, trt_profile, framework, batch_dim, correctness_samples_ind):
+    def _collect_samples(
+        dataloader, input_metadata, trt_profile, framework, batch_dim, correctness_samples_ind, performance_dataloader
+    ):
         profiling_sample = None
         correctness_samples = []
         conversion_samples = []
         conversion_min_max_sampled = {
             name: {ax: {"min": False, "max": False} for ax in range(len(input_metadata[name].shape))}
             for name in input_metadata
         }
@@ -155,119 +180,76 @@
                         do_sample_profiling = True
 
             if do_sample_conversion:
                 conversion_samples.append(extract_bs1(sample, batch_dim))
             if do_sample_profiling:
                 profiling_sample = extract_bs1(sample, batch_dim)
 
+        if performance_dataloader:
+            LOGGER.info("Using performance dataloader for profiling sample. Collecting first item only.")
+            sample = next(iter(performance_dataloader))
+            sample = extract_sample(sample, input_metadata, framework)
+            profiling_sample = extract_bs1(sample, batch_dim)
+
         if not conversion_samples:
             conversion_samples = correctness_samples[:1]
         if profiling_sample is None:
             profiling_sample = conversion_samples[0]
 
         return profiling_sample, correctness_samples, conversion_samples
 
 
-class DumpInputModelData(Command, is_required=True):
-    """Comand for saving input samples."""
-
-    def _run(
-        self,
-        workspace: Path,
-        profiling_sample: Sample,
-        correctness_samples: List[Sample],
-        conversion_samples: List[Sample],
-        batch_dim: Optional[int],
-        raise_on_error: Optional[bool] = False,
-    ) -> CommandOutput:
-        """Run the command and save input samples.
-
-        Args:
-            workspace (Path): Model Navigator workspace path.
-            profiling_sample (Sample): Profiling sample.
-            correctness_samples (List[Sample]): Correctness samples.
-            conversion_samples (List[Sample]): Conversion samples.
-            batch_dim (Optional[int]): Batch dimension.
-            raise_on_error (Optional[bool], optional): If True raise an error when one of the samples is invalid.
-                Defaults to False.
-
-        Returns:
-            CommandOutput
-        """
-        sample_data_path = workspace / "model_input"
-        sample_data_path.mkdir(parents=True, exist_ok=True)
-
-        for samples, dirname in [
-            ([profiling_sample], "profiling"),
-            (correctness_samples, "correctness"),
-            (conversion_samples, "conversion"),
-        ]:
-            samples_to_npz(samples, sample_data_path / dirname, batch_dim, raise_on_error=raise_on_error)
-
-        return CommandOutput(status=CommandStatus.OK)
-
-
-class DumpOutputModelData(Command, is_required=True):
-    """Comand for saving model outputs."""
+class FetchOutputModelData(Command, is_required=True):
+    """Command for saving model outputs."""
 
     def _run(
         self,
         framework: Framework,
-        workspace: Path,
+        workspace: Workspace,
         model: Any,
-        profiling_sample: Sample,
-        correctness_samples: List[Sample],
-        conversion_samples: List[Sample],
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         batch_dim: Optional[int],
         raise_on_error: Optional[bool] = True,
         forward_kw_names: Optional[Tuple[str, ...]] = None,
     ) -> CommandOutput:
         """Run the command and save model outputs.
 
         Args:
-            framework (Framework): Model framework.
-            workspace (Path): Model Navigator workspace path.
-            model (Any): Model instance.
-            profiling_sample (Sample): Profiling sample.
-            correctness_samples (List[Sample]): Correctness samples.
-            conversion_samples (List[Sample]): Conversion samples.
-            input_metadata (TensorMetadata): Input metadata.
-            output_metadata (TensorMetadata): Output metadata.
-            batch_dim (Optional[int]): Batch dimension.
-            raise_on_error (Optional[bool], optional): If True raise an error when one of the samples is invalid.
+            framework: Model framework.
+            workspace: Model Navigator workspace path.
+            model: Model instance.
+            input_metadata: Input metadata.
+            output_metadata: Output metadata.
+            batch_dim: Batch dimension.
+            raise_on_error: If True raise an error when one of the samples is invalid.
                 Defaults to True.
-            forward_kw_names (Optional[Tuple[str, ...]], optional): List of source model input signature naems.
-                Defaults to None.
+            forward_kw_names: List of source model input signature names. Defaults to None.
 
         Returns:
             CommandOutput
         """
-        output_data_path = workspace / "model_output"
+        output_data_path = workspace.path / "model_output"
         output_data_path.mkdir(parents=True, exist_ok=True)
 
         runner = get_format_default_runners(FRAMEWORK2BASE_FORMAT[framework])[0](
             model=model,
             input_metadata=input_metadata,
             output_metadata=output_metadata,
             input_metadata_mapping=forward_kw_names,
         )  # pytype: disable=not-instantiable
 
-        ret = []
-        for samples, dirname in [
-            ([profiling_sample], "profiling"),
-            (correctness_samples, "correctness"),
-            (conversion_samples, "conversion"),
+        output = {}
+        for input_sample, sample_name, output_sample in [
+            ("profiling_sample", "profiling", "profiling_sample_output"),
+            ("correctness_samples", "correctness", "correctness_samples_output"),
+            ("conversion_samples", "conversion", "conversion_samples_output"),
         ]:
+            samples = load_samples(samples_name=input_sample, workspace=workspace.path, batch_dim=batch_dim)
             with runner:
                 outputs = [runner.infer(sample) for sample in samples]
 
-            samples_to_npz(outputs, output_data_path / dirname, batch_dim, raise_on_error=raise_on_error)
-            ret.append(outputs)
+            sample_path = output_data_path / sample_name
+            samples_to_npz(outputs, sample_path, batch_dim, raise_on_error=raise_on_error)
+            output[output_sample] = sample_path
 
-        outputs_names = (
-            "profiling_sample_output",
-            "correctness_samples_output",
-            "conversion_samples_output",
-        )
-        return CommandOutput(status=CommandStatus.OK, output=dict(zip(outputs_names, ret)))
+        return CommandOutput(status=CommandStatus.OK, output=output)
```

## model_navigator/commands/export/jax.py

```diff
@@ -9,33 +9,34 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """JAX export."""
 
-from pathlib import Path
+import pathlib
 from typing import Optional
 
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
+from model_navigator.commands.execution_context import ExecutionContext
 from model_navigator.commands.export import exporters
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.execution_context import ExecutionContext
+from model_navigator.core.workspace import Workspace
 from model_navigator.frameworks.jax import JaxModel
-from model_navigator.logger import LOGGER
 from model_navigator.utils.common import parse_kwargs_to_cmd
 
 
 class ExportJAX2SavedModel(Command):
     """Export JAX to SavedModel command."""
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
         jit_compile: bool,
         enable_xla: bool,
         input_metadata: TensorMetadata,
         verbose: bool,
         model: Optional[JaxModel] = None,
     ) -> CommandOutput:
         """Run export from JAX to SavedModel.
@@ -53,15 +54,15 @@
             model (Optional[JaxModel], optional): JAX model. Defaults to None.
 
         Returns:
             CommandOutput: _description_
         """
         LOGGER.info(f"JAX to SavedModel export started {jit_compile=}, {enable_xla=}")
 
-        exported_model_path = workspace / path
+        exported_model_path = workspace.path / path
         if exported_model_path.is_file() or exported_model_path.is_dir():
             return CommandOutput(status=CommandStatus.SKIPPED)
         assert model is not None
         exported_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         exporters.jax2savedmodel.get_model = lambda: model.model
         exporters.jax2savedmodel.get_model_params = lambda: model.params
@@ -73,15 +74,15 @@
             verbose=verbose,
         ) as context:
             kwargs = {
                 "exported_model_path": exported_model_path.as_posix(),
                 "jit_compile": jit_compile,
                 "enable_xla": enable_xla,
                 "input_metadata": input_metadata.to_json(),
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
             }
 
             args = parse_kwargs_to_cmd(kwargs)
 
             context.execute_local_runtime_script(
                 exporters.jax2savedmodel.__file__, exporters.jax2savedmodel.export, args
             )
```

## model_navigator/commands/export/tf.py

```diff
@@ -9,37 +9,38 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Commands for exporting Tensorflow models."""
 
-from pathlib import Path
+import pathlib
 from typing import Optional, Tuple
 
 import tensorflow as tf  # pytype: disable=import-error
 
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
+from model_navigator.commands.execution_context import ExecutionContext
 from model_navigator.commands.export import exporters
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.execution_context import ExecutionContext
-from model_navigator.logger import LOGGER
+from model_navigator.core.workspace import Workspace
 from model_navigator.utils.common import parse_kwargs_to_cmd
 
 
 class ExportTF2SavedModel(Command):
     """Tensorflow to SavedModel exporter."""
 
     def _run(
         self,
         model: tf.keras.Model,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
-        workspace: Path,
-        path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
         verbose: bool,
         forward_kw_names: Optional[Tuple[str, ...]] = None,
     ) -> CommandOutput:
         """Run Tensorflow to SavedModel export.
 
         Args:
             model (tf.keras.Model): Keras model to be exported.
@@ -52,15 +53,15 @@
                 Defaults to None.
 
         Returns:
             CommandOutput: Status OK.
         """
         LOGGER.info("TensorFlow2 to SavedModel export started")
 
-        exported_model_path = workspace / path
+        exported_model_path = workspace.path / path
         if exported_model_path.exists():
             LOGGER.info("Model already exists. Skipping export.")
             return CommandOutput(status=CommandStatus.SKIPPED)
         assert model is not None
         exported_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         exporters.keras2savedmodel.get_model = lambda: model
@@ -69,19 +70,19 @@
             workspace=workspace,
             script_path=exported_model_path.parent / "reproduce_export.py",
             cmd_path=exported_model_path.parent / "reproduce_export.sh",
             verbose=verbose,
         ) as context:
 
             kwargs = {
-                "exported_model_path": exported_model_path.relative_to(workspace).as_posix(),
+                "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
                 "input_metadata": input_metadata.to_json(),
                 "output_names": list(output_metadata.keys()),
                 "keras_input_names": list(forward_kw_names) if forward_kw_names else None,
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
             }
 
             args = parse_kwargs_to_cmd(kwargs)
 
             context.execute_local_runtime_script(
                 exporters.keras2savedmodel.__file__, exporters.keras2savedmodel.export, args
             )
@@ -90,18 +91,18 @@
 
 
 class UpdateSavedModelSignature(Command):
     """SavedModel signature udpater."""
 
     def _run(
         self,
-        path: Path,
+        path: pathlib.Path,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
-        workspace: Path,
+        workspace: Workspace,
         verbose: bool,
     ) -> CommandOutput:
         """Update SavedModel signature so it matches IO metadata.
 
         Args:
             path (Path): SavedModel path relative to workspace path.
             input_metadata (TensorMetadata): Input metadata.
@@ -110,32 +111,32 @@
             verbose (bool): If True verbose logging.
 
         Returns:
             CommandOutput: Status OK.
         """
         LOGGER.info("TensorFlow2 to SavedModel export started")
 
-        exported_model_path = workspace / path
+        exported_model_path = workspace.path / path
         assert exported_model_path.exists()
         exported_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         exporters.savedmodel2savedmodel.get_model = lambda: tf.keras.models.load_model(exported_model_path)
 
         with ExecutionContext(
             workspace=workspace,
             script_path=exported_model_path.parent / "reproduce_export.py",
             cmd_path=exported_model_path.parent / "reproduce_export.sh",
             verbose=verbose,
         ) as context:
 
             kwargs = {
-                "exported_model_path": exported_model_path.relative_to(workspace).as_posix(),
+                "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
                 "input_metadata": input_metadata.to_json(),
                 "output_names": list(output_metadata.keys()),
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
             }
 
             args = parse_kwargs_to_cmd(kwargs)
             context.execute_local_runtime_script(
                 exporters.savedmodel2savedmodel.__file__, exporters.savedmodel2savedmodel.update_signature, args
             )
```

## model_navigator/commands/export/torch.py

```diff
@@ -11,24 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Commands for exporting PyTorch model from source to serialized formats.
 
 The module provide functionality to export model to TorchScript and/or ONNX.
 """
-from pathlib import Path
+import pathlib
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from model_navigator.api.config import DeviceKind, JitType
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
+from model_navigator.commands.execution_context import ExecutionContext
 from model_navigator.commands.export import exporters
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
+from model_navigator.core.workspace import Workspace
 from model_navigator.exceptions import ModelNavigatorConfigurationError
-from model_navigator.execution_context import ExecutionContext
-from model_navigator.logger import LOGGER
 from model_navigator.utils.common import parse_kwargs_to_cmd
 
 
 class ExportTorch2TorchScript(Command):
     """Command for export PyTorch model to TorchScript.
 
     Example of use:
@@ -41,16 +42,16 @@
             model=torch.nn.Identity(),
             batch_dim=[0]
         )
     """
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
         target_device: DeviceKind,
         jit_type: JitType,
         verbose: bool,
         strict: bool,
         model: Optional[Any] = None,
         batch_dim: Optional[int] = None,
     ) -> CommandOutput:
@@ -65,15 +66,15 @@
             batch_dim: Location of batch position in shapes.
 
         Returns:
             CommandOutput object with status
         """
         LOGGER.info("TorchScrip export started")
 
-        exported_model_path = workspace / path
+        exported_model_path = workspace.path / path
         if exported_model_path.is_file() or exported_model_path.is_dir():
             LOGGER.info("Model already exists. Skipping export.")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         exported_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         if model is None:
@@ -92,20 +93,20 @@
             script_path=exported_model_path.parent / "reproduce_export.py",
             cmd_path=exported_model_path.parent / "reproduce_export.sh",
             verbose=verbose,
             on_exit=on_exit,
         ) as context:
 
             kwargs = {
-                "exported_model_path": exported_model_path.relative_to(workspace).as_posix(),
+                "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
                 "target_jit_type": jit_type.value,
                 "batch_dim": batch_dim,
                 "target_device": target_device.value,
                 "strict": strict,
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
             }
 
             args = parse_kwargs_to_cmd(kwargs)
 
             context.execute_local_runtime_script(
                 exporters.torch2torchscript.__file__, exporters.torch2torchscript.export, args
             )
@@ -130,16 +131,16 @@
             model=torch.nn.Identity(),
             batch_dim=[0]
         )
     """
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
         opset: int,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         target_device: DeviceKind,
         verbose: bool,
         forward_kw_names: Optional[Tuple[str, ...]] = None,
         model: Optional[Any] = None,
@@ -161,15 +162,15 @@
             batch_dim: Location of batch position in shapes
             dynamic_axes: Definition of model inputs dynamic axes
 
         Returns:
             CommandOutput object with status
         """
         LOGGER.info("PyTorch to ONNX export started")
-        exported_model_path = workspace / path
+        exported_model_path = workspace.path / path
         if exported_model_path.exists():
             LOGGER.info("Model already exists. Skipping export.")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         exported_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         if model is None:
@@ -194,16 +195,16 @@
             script_path=exported_model_path.parent / "reproduce_export.py",
             cmd_path=exported_model_path.parent / "reproduce_export.sh",
             verbose=verbose,
             on_exit=on_exit,
         ) as context:
 
             kwargs = {
-                "navigator_workspace": workspace.as_posix(),
-                "exported_model_path": exported_model_path.relative_to(workspace).as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
+                "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
                 "opset": opset,
                 "input_names": list(input_metadata.keys()),
                 "output_names": list(output_metadata.keys()),
                 "dynamic_axes": dynamic_axes,
                 "batch_dim": batch_dim,
                 "forward_kw_names": list(forward_kw_names) if forward_kw_names else None,
                 "target_device": target_device.value,
```

## model_navigator/commands/find_max_batch_size/find_max_batch_size.py

```diff
@@ -12,26 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Functionality to perform search of max possible batch size that model can be loaded with on device."""
 import dataclasses
 import logging
 import pathlib
 import tempfile
-from pathlib import Path
 from typing import List, Optional, Type, Union
 
 import jsonlines
 
-from model_navigator.api.config import ProfilerConfig
+from model_navigator.api.config import OptimizationProfile
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
-from model_navigator.commands.performance.performance import Profiler, ProfilingResults
+from model_navigator.commands.execution_context import ExecutionContext
+from model_navigator.commands.performance import Profiler, ProfilingResults
 from model_navigator.core.constants import DEFAULT_MAX_BATCH_SIZE_THRESHOLD
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.execution_context import ExecutionContext
-from model_navigator.logger import LOGGER
+from model_navigator.core.workspace import Workspace
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.utils.common import parse_kwargs_to_cmd
 
 
 class MaxBatchSizeFinder(Profiler):
     """Overriden profiled for max batch size search."""
 
@@ -50,97 +50,108 @@
 
 class FindMaxBatchSize(Command):
     """Command for searching maximal possible batch size that model can be loaded with."""
 
     def _run(
         self,
         configurations: List[FindMaxBatchSizeConfig],
-        workspace: Path,
+        workspace: Workspace,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         batch_dim: Optional[int],
+        optimization_profile: OptimizationProfile,
         verbose: bool,
-        reproduce_script_dir: Optional[Path] = None,
+        reproduce_script_dir: Optional[pathlib.Path] = None,
     ) -> CommandOutput:
         """Execute command.
 
         Args:
             configurations: Configuration to use during search
             workspace: Workspace where artifacts are stored
             input_metadata: Information about model inputs
             output_metadata: Information about model outputs
             batch_dim: Place where batch dimension is located in shape
+            optimization_profile: Configuration for performance measurement
             verbose: Flag to enable/disable verbose logging for command
             reproduce_script_dir: Script where reproduction of command is saved
 
         Returns:
             CommandOutput with status and additional output parameters
         """
         device_max_batch_size = None
         for configuration in configurations:
             device_max_batch_size = self._execute_configuration(
                 workspace=workspace,
                 path=configuration.model_path,
                 input_metadata=input_metadata,
                 output_metadata=output_metadata,
                 batch_dim=batch_dim,
+                optimization_profile=optimization_profile,
                 verbose=verbose,
                 runner_cls=configuration.runner_cls,
                 reproduce_script_dir=reproduce_script_dir,
             )
             if device_max_batch_size is not None:
                 break
 
         return CommandOutput(
             status=CommandStatus.OK,
             output={"device_max_batch_size": device_max_batch_size},
-            save=True,
         )
 
     def _execute_configuration(
         self,
-        workspace: Path,
-        path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         batch_dim: Optional[int],
+        optimization_profile: OptimizationProfile,
         verbose: bool,
         runner_cls: Type[NavigatorRunner],
-        reproduce_script_dir: Optional[Path] = None,
+        reproduce_script_dir: Optional[pathlib.Path] = None,
     ):
-        model_path = workspace / path
+        model_path = workspace.path / path
         model_dir = model_path.parent
         reproduce_script_dir = reproduce_script_dir or model_dir
         device_max_batch_size = None
 
         if not model_path.exists():
             LOGGER.warning(f"Model: {model_path.as_posix()!r} not found, command skipped.")
             return device_max_batch_size
 
         if batch_dim is None:
             LOGGER.info("Model does not support batching.")
             return device_max_batch_size
 
-        profiler_config = ProfilerConfig(
+        if optimization_profile.max_batch_size or optimization_profile.batch_sizes:
+            if optimization_profile.max_batch_size:
+                device_max_batch_size = optimization_profile.max_batch_size
+            else:
+                device_max_batch_size = max(optimization_profile.batch_sizes)
+            LOGGER.info(f"Using maximal batch size provided in optimization profile: {device_max_batch_size}")
+            return device_max_batch_size
+
+        optimization_profile = OptimizationProfile(
             max_trials=1,
-            measurement_request_count=1,
+            window_size=1,
             throughput_cutoff_threshold=-2,
         )
 
         with ExecutionContext(
             workspace=workspace,
             script_path=reproduce_script_dir / "reproduce_max_batch_size.py",
             cmd_path=reproduce_script_dir / "reproduce_max_batch_size.sh",
             verbose=verbose,
         ) as context, tempfile.NamedTemporaryFile() as temp_file:
             kwargs = {
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
                 "batch_dim": batch_dim,
                 "results_path": temp_file.name,
-                "profiler_config": profiler_config.to_dict(parse=True),
+                "optimization_profile": optimization_profile.to_dict(parse=True),
                 "model_path": path,
                 "runner_name": runner_cls.name(),
                 "input_metadata": input_metadata.to_json(),
                 "output_metadata": output_metadata.to_json(),
             }
 
             args = parse_kwargs_to_cmd(kwargs)
```

## model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py

```diff
@@ -14,38 +14,38 @@
 """Script for finding device maximum batch size for a runner."""
 
 import pathlib
 from typing import Dict, List, Optional
 
 import fire
 
-from model_navigator.api.config import ProfilerConfig
+from model_navigator.api.config import OptimizationProfile
 from model_navigator.commands.find_max_batch_size.find_max_batch_size import MaxBatchSizeFinder
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.logger import LOGGER
 from model_navigator.runners.registry import get_runner
 from model_navigator.utils.dataloader import load_samples
 
 
 def find_max_batch_size(
     batch_dim: int,
     results_path: str,
-    profiler_config: Dict,
+    optimization_profile: Dict,
     model_path: str,
     runner_name: str,
     input_metadata: List,
     output_metadata: List,
     navigator_workspace: Optional[str] = None,
 ) -> None:
     """Find device maximum batch size.
 
     Args:
         batch_dim (int): Batch dimension.
         results_path (str): Output results path.
-        profiler_config (Dict): Profiler configuration.
+        optimization_profile (Dict): Optimization profile used during conversion and profiling.
         model_path (str): Path to the model.
         runner_name (str): Name of the model's runner.
         input_metadata (List): Input metadata.
         output_metadata (List): Output metadata.
         navigator_workspace (Optional[str], optional): Model Navigator workspace path.
             When None use current workdir. Defaults to None.
     """
@@ -60,20 +60,21 @@
         model=navigator_workspace / model_path,
         input_metadata=TensorMetadata.from_json(input_metadata),
         output_metadata=TensorMetadata.from_json(output_metadata),
         disable_fallback=False,
     )  # pytype: disable=not-instantiable
     try:
         MaxBatchSizeFinder(
-            config=ProfilerConfig.from_dict(profiler_config),
+            profile=OptimizationProfile.from_dict(optimization_profile),
             batch_dim=batch_dim,
             results_path=results_path,
         ).run(
             runner=runner,
             profiling_sample=profiling_sample,
+            sample_id=0,
         )
     except Exception as e:
         if results_path.is_file():
             LOGGER.info("Max batch size search finished with success.")
         else:
             raise e
```

## model_navigator/commands/performance/__init__.py

```diff
@@ -8,8 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D104
-from .performance import Performance, Profiler  # noqa: F401
+from .performance import Performance  # noqa: F401
+from .profile import Profile  # noqa: F401
+from .profiler import Profiler, ProfilingResults  # noqa: F401
```

## model_navigator/commands/performance/performance.py

```diff
@@ -7,377 +7,112 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Runners profiling."""
-
-import logging
+"""Command for performance measurement."""
+import pathlib
+import shutil
 import tempfile
-import time
-from dataclasses import dataclass
-from pathlib import Path
-from typing import Any, List, Mapping, Optional, Type
+from typing import Any, Optional, Type
 
-import numpy as np
 from jsonlines import jsonlines
 
-from model_navigator.api.config import Format, MeasurementMode, ProfilerConfig, Sample
+from model_navigator.api.config import Format, OptimizationProfile
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
+from model_navigator.commands.execution_context import ExecutionContext
+from model_navigator.commands.performance.results import ProfilingResults
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
-from model_navigator.exceptions import ModelNavigatorError, ModelNavigatorProfilingError
-from model_navigator.execution_context import ExecutionContext
-from model_navigator.logger import LOGGER
-from model_navigator.runners.base import NavigatorRunner, NavigatorStabilizedRunner
-from model_navigator.utils.common import DataObject, parse_kwargs_to_cmd
-from model_navigator.utils.dataloader import expand_sample
+from model_navigator.core.workspace import Workspace
+from model_navigator.exceptions import ModelNavigatorProfilingError
+from model_navigator.runners.base import NavigatorRunner
+from model_navigator.utils.common import parse_kwargs_to_cmd
 from model_navigator.utils.format_helpers import is_source_format
 
 
-@dataclass
-class ProfilingResults(DataObject):
-    """Profiling results."""
-
-    batch_size: int
-    avg_latency: float  # ms
-    std_latency: float  # ms
-    p50_latency: float  # ms
-    p90_latency: float  # ms
-    p95_latency: float  # ms
-    p99_latency: float  # ms
-    throughput: float  # infer / sec
-    request_count: int
-
-    @classmethod
-    def from_dict(cls, d: Mapping) -> "ProfilingResults":
-        """Instantiate ProfilingResults from a json dictionary.
-
-        Args:
-            d (Mapping): Data dictionary.
-
-        Returns:
-            ProfilingResults
-        """
-        return cls(**d)
-
-    @classmethod
-    def from_measurements(cls, measurements: List[float], batch_size: Optional[int]) -> "ProfilingResults":
-        """Instantiate ProfilingResults from a list of measurements.
-
-        Args:
-            measurements (List[float]): List of measurements.
-            batch_size (int): Batch size.
-
-        Returns:
-            ProfilingResults
-        """
-        measurements = np.array(measurements)
-        return cls(
-            batch_size=batch_size,
-            avg_latency=float(np.mean(measurements)),
-            std_latency=float(np.std(measurements)),
-            p50_latency=float(np.percentile(measurements, 50)),
-            p90_latency=float(np.percentile(measurements, 90)),
-            p95_latency=float(np.percentile(measurements, 95)),
-            p99_latency=float(np.percentile(measurements, 99)),
-            throughput=float(1000 * (batch_size or 1) / np.mean(measurements)),
-            request_count=len(measurements),
-        )
-
-    @classmethod
-    def from_profiling_results(cls, profiling_results: List["ProfilingResults"]) -> "ProfilingResults":
-        """Instantiate ProfilingResults as a mean of other profiling results.
-
-        Args:
-            profiling_results (List[ProfilingResults]): List of profiling results to average.
-
-        Returns:
-            ProfilingResults
-        """
-        batch_size = profiling_results[0].batch_size
-
-        return cls(
-            batch_size=batch_size,
-            avg_latency=float(np.mean([result.avg_latency for result in profiling_results])),
-            std_latency=float(np.mean([result.std_latency for result in profiling_results])),
-            p50_latency=float(np.mean([result.p50_latency for result in profiling_results])),
-            p90_latency=float(np.mean([result.p90_latency for result in profiling_results])),
-            p95_latency=float(np.mean([result.p95_latency for result in profiling_results])),
-            p99_latency=float(np.mean([result.p99_latency for result in profiling_results])),
-            throughput=float(np.mean([result.throughput for result in profiling_results])),
-            request_count=int(np.mean([result.request_count for result in profiling_results])),
-        )
-
-    @classmethod
-    def from_stable_runner(cls, runner: NavigatorStabilizedRunner, batch_size: int) -> "ProfilingResults":
-        """Instantiate ProfilingResults from a stable runner results.
-
-        Args:
-            runner (NavigatorStabilizedRunner): Stable runner instance.
-            batch_size (int): Batch size.
-
-        Returns:
-            ProfilingResults
-        """
-        return cls(
-            batch_size=batch_size,
-            avg_latency=runner.avg_latency(),
-            std_latency=runner.std_latency(),
-            p50_latency=runner.p50_latency(),
-            p90_latency=runner.p90_latency(),
-            p95_latency=runner.p95_latency(),
-            p99_latency=runner.p99_latency(),
-            throughput=float(1000 * max(1, batch_size) / runner.avg_latency()),
-            request_count=runner.request_count(),
-        )
-
-    def __str__(self) -> str:
-        """Get string representation."""
-        return (
-            f"Batch: {self.batch_size}\n"
-            f"Request count: {self.request_count}\n"
-            f"Throughput: {self.throughput:.4f} [infer/sec]\n"
-            f"Avg Latency: {self.avg_latency:.4f} [ms]\n"
-            f"Std Latency: {self.std_latency:.4f} [ms]\n"
-            f"p50 Latency: {self.p50_latency:.4f} [ms]\n"
-            f"p90 Latency: {self.p90_latency:.4f} [ms]\n"
-            f"p95 Latency: {self.p95_latency:.4f} [ms]\n"
-            f"p99 Latency: {self.p99_latency:.4f} [ms]"
-        )
-
-
-class Profiler:
-    """Runs profiling on a runner an profiling sample.
-
-    Example:
-        Profiler(
-            config=ProfilerConfig(),
-            results_path="results.jsonl",
-        ).run(
-            runner=runner,
-            profiling_sample={"input_1": np.ones(1, 3)}
-        )
-    """
-
-    def __init__(
-        self,
-        config: ProfilerConfig,
-        results_path: Path,
-        batch_dim: Optional[int] = 0,
-    ) -> None:
-        """Initialize the Profiler.
-
-        Args:
-            config (ProfilerConfig): Profiler configuration.
-            results_path (Path): Jsonlines path to store the results in.
-            batch_dim (Optional[int], optional): Batch dimension. Defaults to 0.
-
-        Raises:
-            ValueError: When batch_dim is None, but config.batch_sizes is not None.
-        """
-        self._config = config
-        self._batch_dim = batch_dim
-        self._results_path = results_path
-
-        if self._batch_dim is None:
-            self._batch_sizes = [None]
-        else:
-            self._batch_sizes = (
-                self._config.batch_sizes if self._config.batch_sizes else (2 ** np.arange(31, dtype=np.int32)).tolist()
-            )
-
-    @property
-    def _profiling_results_logging_level(self):
-        return logging.INFO
-
-    def _run_time_window_measurement(
-        self, runner: NavigatorRunner, sample: Sample, batch_size: int
-    ) -> ProfilingResults:
-        measurements = []
-        start = time.monotonic()
-        while (time.monotonic() - start) * 1000 < self._config.measurement_interval:
-            runner.infer(sample)
-            measurements.append(runner.last_inference_time() * 1000)
-
-        return ProfilingResults.from_measurements(measurements, batch_size)
-
-    def _run_count_window_measurement(
-        self, runner: NavigatorRunner, sample: Sample, batch_size: Optional[int]
-    ) -> ProfilingResults:
-        measurements = []
-        for _ in range(self._config.measurement_request_count):
-            runner.infer(sample)
-            measurements.append(runner.last_inference_time() * 1000)
-
-        return ProfilingResults.from_measurements(measurements, batch_size)
-
-    def _is_measurement_stable(self, profiling_results: List[ProfilingResults], count: int = 3) -> bool:
-        if len(profiling_results) < count:
-            return False
-
-        profiling_results = profiling_results[-count:]
-        avg_latencies = [result.avg_latency for result in profiling_results]
-        avg_latency = np.mean(avg_latencies)
-        deviation_perc = np.abs((avg_latencies - avg_latency) / avg_latency * 100)
-
-        return np.all(deviation_perc < self._config.stability_percentage)
-
-    def _measurements_result(self, profiling_results: List[ProfilingResults], count: int = 3) -> ProfilingResults:
-        if len(profiling_results) < count:
-            raise ModelNavigatorError("Measurements results requires at least 3 consecutive stable measurements.")
-
-        profiling_results = profiling_results[-count:]
-        profiling_result = ProfilingResults.from_profiling_results(profiling_results)
-
-        return profiling_result
-
-    def _run_measurement(self, runner: NavigatorRunner, sample: Sample, batch_size: Optional[int]) -> ProfilingResults:
-        profiling_results = []
-
-        measurement_fn = {
-            MeasurementMode.TIME_WINDOWS: self._run_time_window_measurement,
-            MeasurementMode.COUNT_WINDOWS: self._run_count_window_measurement,
-        }[self._config.measurement_mode]
-
-        if runner.is_stabilized():
-            assert isinstance(runner, NavigatorStabilizedRunner)
-            runner.infer(sample)
-            profiling_result = ProfilingResults.from_stable_runner(runner, batch_size)
-            return profiling_result
-        else:
-            for idx in range(self._config.max_trials):
-                profiling_result = measurement_fn(runner, sample, batch_size)
-                profiling_results.append(profiling_result)
-                LOGGER.debug(
-                    f"Measurement [{idx}]: {profiling_result.throughput} infer/sec, {profiling_result.avg_latency} ms"
-                )
-                if self._is_measurement_stable(profiling_results, count=min(3, self._config.max_trials)):
-                    return self._measurements_result(profiling_results, count=min(3, self._config.max_trials))
-
-        raise RuntimeError(
-            "Unable to get stable performance results. Consider increasing "
-            "measurement_interval | measurement_request_count | stability_percentage | max_trials in ProfilerConfig."
-        )
-
-    def run(
-        self,
-        runner: NavigatorRunner,
-        profiling_sample: Sample,
-    ) -> List[ProfilingResults]:
-        """Run profiling.
-
-        Args:
-            runner (NavigatorRunner): Runner to profile.
-            profiling_sample (Sample): Sample used for profiling.
-
-        Returns:
-            List[ProfilingResults]: Results for each of the batch sizes from profiler configuration.
-        """
-        results, prev_result = [], None
-        with runner:
-            for batch_size in self._batch_sizes:
-                LOGGER.log(self._profiling_results_logging_level, f"Performance profiling for {runner.name()} started.")
-                if batch_size:
-                    LOGGER.log(self._profiling_results_logging_level, f"Batch size: {batch_size}.")
-                sample = expand_sample(profiling_sample, self._batch_dim, batch_size)
-                profiling_result = self._run_measurement(runner, sample, batch_size)
-                LOGGER.log(
-                    self._profiling_results_logging_level,
-                    (
-                        f"Performance profiling result for {runner.name()} "
-                        f"and batch size: {batch_size}:\n{profiling_result}"
-                    ),
-                )
-                with jsonlines.open(self._results_path.as_posix(), "a") as f:
-                    f.write(profiling_result.to_dict())
-
-                results.append(profiling_result)
-                if prev_result is not None and profiling_result.throughput < prev_result.throughput * (
-                    1 + self._config.throughput_cutoff_threshold
-                ):
-                    break
-                prev_result = profiling_result
-
-        return results
-
-
 class Performance(Command):
     """Performance command."""
 
     def _run(
         self,
-        workspace: Path,
-        path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
         format: Format,
-        profiler_config: ProfilerConfig,
+        optimization_profile: OptimizationProfile,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         batch_dim: Optional[int],
         verbose: bool,
         runner_cls: Type[NavigatorRunner],
-        reproduce_script_dir: Optional[Path] = None,
+        reproduce_script_dir: Optional[pathlib.Path] = None,
         model: Optional[Any] = None,
     ) -> CommandOutput:
         """Run performance command.
 
         Args:
-            workspace (Path): Model Navigator workspace path.
-            path (Path): Model path, relative to the workspace.
-            format (Format): Model format.
-            profiler_config (ProfilerConfig): Profiler configuration.
-            input_metadata (TensorMetadata): Input metadata.
-            output_metadata (TensorMetadata): Output metadata.
-            batch_dim (Optional[int]): Batch dimension.
-            verbose (bool): If True verbose logging.
-            runner_cls (Type[NavigatorRunner]): Runner type to profile the model with.
-            reproduce_script_dir (Optional[Path], optional): Path to store the reproducting scripts for the command.
+            workspace: Model Navigator workspace path.
+            path: Model path, relative to the workspace.
+            format: Model format.
+            optimization_profile: Optimization profile used during conversion and profiling.
+            input_metadata: Input metadata.
+            output_metadata: Output metadata.
+            batch_dim: Batch dimension.
+            verbose: If True verbose logging.
+            runner_cls: Runner type to profile the model with.
+            reproduce_script_dir: Path to store the reproducing scripts for the command.
                 When None use model directory. Defaults to None.
-            model (Optional[Any], optional): Model when profiling on a source format. Defaults to None.
+            model: Model when profiling on a source format. Defaults to None.
 
         Returns:
             CommandOutput: Output of the command containing profiling results.
         """
-        model_path = workspace / path
+        model_path = workspace.path / path
         model_dir = model_path.parent
         reproduce_script_dir = reproduce_script_dir or model_dir
 
         if not is_source_format(format) and not model_path.exists():
             LOGGER.warning(f"Model: {model_path.as_posix()!r} not found, command skipped.")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
+        profiler_samples = workspace.path / "model_input" / "profiler"
+        if profiler_samples.exists():
+            shutil.rmtree(profiler_samples.as_posix())
+
+        profiling_samples = workspace.path / "model_input" / "profiling"
+        shutil.copytree(profiling_samples, profiler_samples)
+
         with ExecutionContext(
             workspace=workspace,
             script_path=reproduce_script_dir / "reproduce_profiling.py",
             cmd_path=reproduce_script_dir / "reproduce_profiling.sh",
             verbose=verbose,
         ) as context, tempfile.NamedTemporaryFile() as temp_file:
             kwargs = {
-                "navigator_workspace": workspace.as_posix(),
+                "navigator_workspace": workspace.path.as_posix(),
                 "batch_dim": batch_dim,
                 "results_path": temp_file.name,
                 "runner_name": runner_cls.name(),
-                "profiler_config": profiler_config.to_dict(parse=True),
+                "optimization_profile": optimization_profile.to_dict(parse=True),
                 "input_metadata": input_metadata.to_json(),
                 "output_metadata": output_metadata.to_json(),
             }
 
-            args = parse_kwargs_to_cmd(kwargs)
-
-            from model_navigator.commands.performance import performance_script
+            from model_navigator.commands.performance import profile_script
 
             if is_source_format(format):
-                performance_script.get_model = lambda: model
+                profile_script.get_model = lambda: model
                 args = parse_kwargs_to_cmd(kwargs)
                 context.execute_local_runtime_script(
-                    performance_script.__file__, performance_script.profile, args, allow_failure=True
+                    profile_script.__file__, profile_script.profile, args, allow_failure=True
                 )
             else:
                 kwargs["model_path"] = path
                 args = parse_kwargs_to_cmd(kwargs)
-                context.execute_external_runtime_script(performance_script.__file__, args, allow_failure=True)
+                context.execute_external_runtime_script(profile_script.__file__, args, allow_failure=True)
             with jsonlines.open(temp_file.name, "r") as f:
                 profiling_results = [ProfilingResults.from_dict(res) for res in f]
         if not profiling_results:
             raise ModelNavigatorProfilingError("No profiling results found.")
         return CommandOutput(status=CommandStatus.OK, output={"profiling_results": profiling_results})
```

## model_navigator/commands/verification/verify.py

```diff
@@ -10,77 +10,59 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Runtime verification command."""
 
 
-from pathlib import Path
+import pathlib
 from typing import Any, Optional, Type
 
 from model_navigator.api.config import Format, SizedDataLoader, VerifyFunction
 from model_navigator.commands.base import Command, CommandOutput, CommandStatus
 from model_navigator.commands.correctness import Correctness
 from model_navigator.commands.performance import Performance
+from model_navigator.core.logger import LOGGER
 from model_navigator.core.tensor import TensorMetadata
+from model_navigator.core.workspace import Workspace
 from model_navigator.frameworks import Framework
-from model_navigator.logger import LOGGER
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runners.registry import get_runner
 from model_navigator.runners.utils import get_source_default_runners
 from model_navigator.utils.dataloader import extract_sample
 from model_navigator.utils.format_helpers import FRAMEWORK2BASE_FORMAT
 
 
-class VerifyModel(Command):
+class VerifyModel(Command, requires=[Correctness.name, Performance.name]):
     """Verify model with a runner."""
 
     def _pre_run(
         self,
         verify_func: VerifyFunction,
-        key: str,
-        runner_cls: Type[NavigatorRunner],
     ) -> bool:
         """Check if command should be run.
 
         Args:
             verify_func (VerifyFunction): verification function.
-            key (str): Modek key.
-            runner_cls (Type[NavigatorRunner]): Runner class to be verified.
 
         Returns:
             bool: True if command should be run, False otherwise.
         """
-        if self.status is None:
-            raise ValueError("Status must be set before running command.")
-
         if verify_func is None:
             LOGGER.info("verify_function not provided - SKIPPED")
             return False
 
-        runner_status = self.status.models_status[key].runners_status[runner_cls.name()]
-
-        correctness_status = runner_status.status.get(Correctness.name())
-        if correctness_status != CommandStatus.OK:
-            LOGGER.info(f"Runner {runner_cls.name()} correctness results is not OK - SKIPPED")
-            return False
-
-        performance_status = runner_status.status.get(Performance.name())
-        if performance_status is not None and performance_status != CommandStatus.OK:
-            LOGGER.info(f"Runner {runner_cls.name()} performance results is not OK - SKIPPED")
-            return False
-
         return True
 
     def _run(
         self,
         framework: Framework,
         format: Format,
-        workspace: Path,
-        path: Path,
+        workspace: Workspace,
+        path: pathlib.Path,
         dataloader: SizedDataLoader,
         verify_func: VerifyFunction,
         runner_cls: Type[NavigatorRunner],
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         model: Optional[Any] = None,
     ) -> CommandOutput:
@@ -115,15 +97,15 @@
             with runner:
                 for sample in dataloader:
                     sample = extract_sample(sample, input_metadata, framework)
                     output = runner.infer(sample)
                     yield output
 
         runner = get_runner(runner_cls)(
-            model=model if format == source_format else workspace / path,
+            model=model if format == source_format else workspace.path / path,
             input_metadata=input_metadata,
             output_metadata=output_metadata,
         )
         y_pred = _get_outputs(runner)
 
         fw_runner = get_runner(source_runners[0])(
             model=model,
```

## model_navigator/configuration/common_config.py

```diff
@@ -10,58 +10,48 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Config object to handle user inputs and define the execution of commands."""
 
 import dataclasses
-import json
 from dataclasses import dataclass
-from pathlib import Path
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Sequence
 
-from model_navigator.api.config import CustomConfig, DeviceKind, Format, ProfilerConfig, SizedDataLoader, VerifyFunction
+from model_navigator.api.config import (
+    CustomConfig,
+    DeviceKind,
+    Format,
+    OptimizationProfile,
+    SizedDataLoader,
+    VerifyFunction,
+)
 from model_navigator.frameworks import Framework
-from model_navigator.logger import LOGGER
-from model_navigator.utils.common import DataObject, pad_string
+from model_navigator.utils.common import DataObject
 
 
 @dataclass
 class CommonConfig(DataObject):
-    """Command conxtext stores paramters used during commands execution not related to any particular model format."""
+    """Command context stores parameters used during commands execution not related to any particular model format."""
 
     framework: Framework
     model: object
     dataloader: SizedDataLoader
-    workspace: Path
-    target_formats: Tuple[Format, ...]
+    target_formats: Sequence[Format]
     target_device: DeviceKind
     sample_count: int
-    profiler_config: ProfilerConfig
-    runner_names: Tuple[str, ...]
+    optimization_profile: OptimizationProfile
+    runner_names: Sequence[str]
     batch_dim: Optional[int] = 0
     seed: int = 0
-    _input_names: Optional[Tuple[str, ...]] = None
-    _output_names: Optional[Tuple[str, ...]] = None
+    _input_names: Optional[Sequence[str]] = None
+    _output_names: Optional[Sequence[str]] = None
     from_source: bool = True
-    forward_kw_names: Optional[Tuple[str, ...]] = None
+    forward_kw_names: Optional[Sequence[str]] = None
     verify_func: Optional[VerifyFunction] = None
     custom_configs: Dict[str, CustomConfig] = dataclasses.field(default_factory=lambda: {})
 
     # Verbose logging - enable debug mode in export and conversion paths
     verbose: bool = False
 
     # Debug - enabled debug mode for converters
     debug: bool = False
-
-    def log(self) -> None:
-        """Display the configuration as formatted string."""
-        LOGGER.info(pad_string("Common config parameters"))
-        log_dict = self.to_dict(
-            filter_fields=[
-                "model",
-                "dataloader",
-                "verify_func",
-            ],
-            parse=True,
-        )
-        LOGGER.info(json.dumps(log_dict, indent=4))
```

## model_navigator/configuration/model/model_config.py

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module contains classes representing model configurations."""
 
+import pathlib
 from abc import ABC, abstractmethod
-from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
 from model_navigator.api.config import (
     Format,
     JitType,
     TensorRTCompatibilityLevel,
     TensorRTPrecision,
@@ -139,32 +139,32 @@
             if params:
                 key_params_array.extend(params)
 
         key = "-".join(key_params_array)
         return key
 
     @property
-    def path(self) -> Path:
+    def path(self) -> pathlib.Path:
         """Get path to model checkpoint."""
         path_str = self.key
 
         if is_source_format(self.format):
-            path = Path(path_str) / "----"
+            path = pathlib.Path(path_str) / "----"
         else:
-            path = Path(path_str) / f"model{FORMAT2SUFFIX[self.format]}"
+            path = pathlib.Path(path_str) / f"model{FORMAT2SUFFIX[self.format]}"
 
         return path
 
     @property
-    def log_path(self) -> Path:
+    def log_path(self) -> pathlib.Path:
         """Get path to log file."""
         return self.path.parent / "format.log"
 
     @property
-    def parent_path(self) -> Optional[Path]:
+    def parent_path(self) -> Optional[pathlib.Path]:
         """Get path to parent model checkpoint."""
         if self.parent:
             return self.parent.path
         else:
             return None
 
     @property
```

## model_navigator/core/constants.py

```diff
@@ -12,15 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Constants definition."""
 from model_navigator.__version__ import __version__  # noqa: F401
 
 # Version
 NAVIGATOR_VERSION = __version__
-NAVIGATOR_PACKAGE_VERSION = "0.2.1"
+NAVIGATOR_PACKAGE_VERSION = "0.2.2"
+
+# Workspace related
+DEFAULT_WORKSPACE = "navigator_workspace"
 
 # Profiling related
 DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD = 0.05
 
 # Dataloader related
 DEFAULT_SAMPLE_COUNT = 100
```

## model_navigator/core/tensor.py

```diff
@@ -11,18 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utilities for working with tensors in different environments."""
 import abc
 import dataclasses
 from collections import defaultdict
-from typing import Dict, List, Optional, Sequence, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union
 
 import numpy as np
 
+from model_navigator.api.config import TensorType
+from model_navigator.frameworks import Framework, is_jax_available, is_tf_available, is_torch_available
+from model_navigator.utils import common, module
+
+torch = module.lazy_import("torch")
+tf = module.lazy_import("tensorflow")
+jax = module.lazy_import("jax")
+
 # pytype: disable=annotation-type-mismatch
 # pytype: disable=wrong-keyword-args
 # pytype: disable=name-error
 
 
 @dataclasses.dataclass
 class TensorSpec:
@@ -65,27 +73,48 @@
             raise TypeError(f"Shape items should be integers equal to -1 or positive numbers. Got {self.shape}")
 
     def astype(self, dtype: Union[np.dtype, Type[np.dtype]]) -> "TensorSpec":
         """Change the TensorSpec dtype."""
         tensor = TensorSpec(name=self.name, shape=self.shape, dtype=np.dtype(dtype), optional=self.optional)
         return tensor
 
-    def is_dtype_compatible(self, tensor: np.ndarray) -> bool:
+    def is_dtype_compatible(self, spec: "TensorSpec") -> bool:
         """Check if `tensor` has dtype compatible with `self`. E.g. dtype of `tensor` is subtype of `self`."""
-        return np.issubdtype(tensor.dtype, self.dtype)
+        return np.issubdtype(spec.dtype, self.dtype)
 
-    def is_shape_compatible(self, tensor: np.ndarray) -> bool:
+    def is_shape_compatible(self, spec: "TensorSpec") -> bool:
         """Check if `tensor` has shape compatible with `self`. E.g. `tensor` has shape (3, 1) and `self` has (-1, 1)."""
-        if len(self.shape) != len(tensor.shape):
+        if len(self.shape) != len(spec.shape):
             return False
-        for self_dim, spec_dim in zip(self.shape, tensor.shape):
+        for self_dim, spec_dim in zip(self.shape, spec.shape):
             if self_dim != spec_dim and self_dim != -1:
                 return False
         return True
 
+    @classmethod
+    def from_numpy_tensor(cls, tensor: np.ndarray, name: str) -> "TensorSpec":
+        """Create TensorSpec from numpy array."""
+        return cls(name=name, shape=tensor.shape, dtype=np.dtype(tensor.dtype))
+
+    @classmethod
+    def from_torch_tensor(cls, tensor: "torch.Tensor", name: str) -> "TensorSpec":
+        """Create TensorSpec from torch tensor."""
+        return cls(name=name, shape=tensor.shape, dtype=np.dtype(common.torch_to_numpy_dtype(tensor.dtype)))
+
+    @classmethod
+    def from_tensor(cls, tensor, name: str) -> "TensorSpec":
+        """Create TensorSpec from tensor."""
+        tensor_type = get_tensor_type(tensor)
+        if tensor_type == TensorType.NUMPY:
+            return cls.from_numpy_tensor(tensor, name)
+        elif tensor_type == TensorType.TORCH:
+            return cls.from_torch_tensor(tensor, name)
+        else:
+            raise TypeError(f"Unsupported tensor type: {type(tensor)}")
+
 
 class TensorUtils(abc.ABC):
     """Abstract class for utils of different implementations of tensor data."""
 
     @staticmethod
     def for_data(data):
         """Return correct utils for provided data."""
@@ -124,32 +153,28 @@
 
 class PyTorchTensorUtils(TensorUtils):
     """Utils for PyTorch tensors."""
 
     @staticmethod
     def eq(a, b):
         """Comparison of two tensors."""
-        import torch  # pytype: disable=import-error
-
         return a.device == b.device and a.dtype == b.dtype and a.shape == b.shape and torch.all(torch.eq(a, b))
 
     @staticmethod
     def to_numpy(a):
         """Cast tensor to numpy format."""
         return a.cpu().detach().numpy()
 
 
 class TensorFlowTensorUtils(TensorUtils):
     """Utils for TensorFlow tensors."""
 
     @staticmethod
     def eq(a, b):
         """Comparison of two tensors."""
-        import tensorflow as tf  # pytype: disable=import-error
-
         return a.device == b.device and a.dtype == b.dtype and a.shape == b.shape and tf.reduce_all(a == b)
 
     @staticmethod
     def to_numpy(a):
         """Cast tensor to numpy format."""
         return a.numpy()
 
@@ -232,7 +257,30 @@
                 if d == -1:
                     dynamic_axes[name].append(ax)
         return dynamic_axes
 
     @staticmethod
     def _parse_tensorspec(spec: TensorSpec):
         return {"name": spec.name, "shape": spec.shape, "dtype": str(spec.dtype)}
+
+
+def get_tensor_type(tensor: Any) -> TensorType:
+    """Get tensor type from tensor."""
+    if isinstance(tensor, np.ndarray):
+        return TensorType.NUMPY
+    elif is_torch_available() and torch.is_tensor(tensor):
+        return TensorType.TORCH
+    elif is_tf_available() and tf.is_tensor(tensor):
+        return TensorType.TENSORFLOW
+    elif is_jax_available() and isinstance(tensor, jax.numpy.ndarray):
+        return TensorType.JAX
+    else:
+        raise TypeError(f"Unsupported tensor type: {type(tensor)}")
+
+
+FRAMEWORK_TO_TENSOR_TYPE = {
+    Framework.TORCH: TensorType.TORCH,
+    Framework.TENSORFLOW: TensorType.TENSORFLOW,
+    Framework.JAX: TensorType.NUMPY,
+    Framework.ONNX: TensorType.NUMPY,
+    Framework.NONE: TensorType.NUMPY,
+}
```

## model_navigator/frameworks/tensorrt/cuda.py

```diff
@@ -18,16 +18,19 @@
 import os
 import sys
 from typing import Optional, Sequence, Tuple
 
 import numpy as np
 
 import model_navigator.utils.common as utils
+from model_navigator.core.logger import LOGGER
 from model_navigator.exceptions import ModelNavigatorError, ModelNavigatorUserInputError
-from model_navigator.logger import LOGGER
+from model_navigator.utils import module
+
+torch = module.lazy_import("torch")
 
 
 def void_ptr(val=None):
     """Returns a void pointer to the given value."""
     return ctypes.c_void_p(val)
 
 
@@ -489,14 +492,30 @@
         Returns:
             The newly created NumPy array.
         """
         arr = np.empty(self.shape, dtype=self.dtype)
         self.copy_to(arr)
         return arr
 
+    def torch(self, stream=None):
+        """Create a new NumPy array containing the contents of this device buffer.
+
+        Returns:
+            The newly created NumPy array.
+        """
+        arr = torch.empty(self.shape, dtype=utils.numpy_to_torch_dtype(self.dtype), device="cuda")
+        wrapper().memcpy(
+            dst=arr.data_ptr(),
+            src=self.ptr,
+            nbytes=self.nbytes,
+            kind=MemcpyKind.DeviceToDevice,
+            stream_ptr=try_get_stream_handle(stream),
+        )
+        return arr
+
     def __str__(self):
         """Returns a string representation of the device buffer."""
         return f"DeviceView[(dtype={np.dtype(self.dtype).name}, shape={self.shape}), ptr={hex(self.ptr)}]"
 
     def __repr__(self):
         """Returns a string representation of the device buffer."""
         return _make_repr("DeviceView", ptr=self.ptr, shape=self.shape, dtype=self.dtype)[0]
```

## model_navigator/frameworks/tensorrt/utils.py

```diff
@@ -14,27 +14,29 @@
 """TensorRT utils."""
 import contextlib
 import logging
 import math
 import os
 import signal
 from distutils.version import LooseVersion
-from typing import Callable, Union
+from typing import Callable, Optional, TypeVar, Union
 
 import numpy as np
 
-from model_navigator.api.config import ShapeTuple, TensorRTProfile
+from model_navigator.api.config import ShapeTuple, TensorRTProfile, TensorType
 from model_navigator.core.constants import OPT_MAX_SHAPE_RATIO
-from model_navigator.core.tensor import TensorMetadata, TensorSpec
+from model_navigator.core.tensor import TensorMetadata, get_tensor_type
 from model_navigator.exceptions import ModelNavigatorNotFoundError
 from model_navigator.utils import module
-from model_navigator.utils.common import invoke_if_callable
+from model_navigator.utils.common import invoke_if_callable, numpy_to_torch_dtype, torch_to_numpy_dtype
 
 trt = module.lazy_import("tensorrt")
 
+T = TypeVar("T")
+
 LOGGER = logging.getLogger(__name__)
 _TYPE_CASTS = {
     np.dtype(np.int64): np.dtype(np.int32),
     np.dtype(np.float64): np.dtype(np.float32),
     np.dtype(np.uint64): np.dtype(np.uint32),
 }
 
@@ -60,24 +62,43 @@
     """Cast type and return new dtype."""
     if dtype in _TYPE_CASTS:
         return _TYPE_CASTS[dtype]
 
     return dtype
 
 
-def cast_tensor(tensor: TensorSpec) -> TensorSpec:
-    """Cast type and return new dtype."""
-    if tensor.dtype in _TYPE_CASTS:
-        target_dtype = _TYPE_CASTS[tensor.dtype]
-        LOGGER.debug(f"Casting {tensor.dtype} tensor to {target_dtype.type}.")
-        return tensor.astype(target_dtype.type)
+def _cast_torch_tensor(tensor, dtype):
+    target_dtype = dtype or _TYPE_CASTS.get(np.dtype(torch_to_numpy_dtype(tensor.dtype)))
+    if target_dtype:
+        LOGGER.debug(f"Casting {dtype} tensor to {target_dtype}.")
+        return tensor.to(numpy_to_torch_dtype(target_dtype))
+    return tensor
 
+
+def _cast_numpy_tensor(tensor, dtype):
+    target_dtype = dtype or _TYPE_CASTS.get(tensor.dtype)
+    if target_dtype:
+        LOGGER.debug(f"Casting {dtype} tensor to {target_dtype}.")
+        return tensor.astype(target_dtype.type)
     return tensor
 
 
+def cast_tensor(tensor: T, dtype: Optional[np.dtype] = None) -> T:
+    """Cast type and return tensor with new dtype."""
+    if dtype is not None:
+        assert isinstance(dtype, np.dtype)
+
+    tensor_type = get_tensor_type(tensor)
+    if tensor_type == TensorType.TORCH:
+        return _cast_torch_tensor(tensor, dtype)
+    else:
+        assert tensor_type == TensorType.NUMPY
+        return _cast_numpy_tensor(tensor, dtype)
+
+
 def get_trt_profile_with_new_max_batch_size(
     trt_profile: TensorRTProfile, max_batch_size: int, batch_dim: int
 ) -> TensorRTProfile:
     """Create new TensorRT profile with maximum batch size.
 
     Args:
         trt_profile (TensorRTProfile): TensorRT Profile.
```

## model_navigator/frameworks/torch/utils.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Torch utils."""
 from typing import Optional, Sequence, Tuple
 
 from model_navigator.api.config import CustomConfig, Format, TorchTensorRTConfig
-from model_navigator.logger import LOGGER
+from model_navigator.core.logger import LOGGER
 
 
 def update_allowed_batching_parameters(
     target_formats: Tuple[Format, ...], custom_configs: Optional[Sequence[CustomConfig]]
 ):
     """Update target formats and custom configs to disable Torch-TensorRT when batching is True."""
     target_formats = tuple(tf for tf in target_formats if tf != Format.TORCH_TRT)
```

## model_navigator/pipelines/pipeline.py

```diff
@@ -11,23 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Definition of Pipeline module - Direct Acyclic Graph (DAG) of commands execution."""
 import contextlib
 import sys
 import traceback
-from typing import Any, Dict, List
+from typing import List
 
 from model_navigator.commands.base import CommandOutput, CommandStatus, ExecutionUnit
 from model_navigator.configuration.common_config import CommonConfig
-from model_navigator.core.package import Package
-from model_navigator.core.status import Status
-from model_navigator.exceptions import ModelNavigatorUserInputError
-from model_navigator.logger import LOGGER, LoggingContext, StdoutLogger
-from model_navigator.utils.common import pad_string
+from model_navigator.core.logger import LOGGER, LoggingContext, StdoutLogger, pad_string
+from model_navigator.core.workspace import Workspace
+from model_navigator.exceptions import ModelNavigatorCommandNotExecutable, ModelNavigatorUserInputError
+from model_navigator.pipelines.pipeline_context import PipelineContext
 
 
 class Pipeline:
     """Definition of Direct Acyclic Graph (DAG) of commands execution."""
 
     def __init__(
         self,
@@ -40,97 +39,92 @@
             name: Name of the pipeline
             execution_units: List of execution units objects
         """
         self.name = name
         self.id = name.lower().replace(" ", "_").replace("-", "_")
         self.execution_units = execution_units
 
-    def run(self, config: CommonConfig, package: Package, **kwargs) -> Dict[str, Any]:
+    def run(self, workspace: Workspace, config: CommonConfig, context: PipelineContext) -> None:
         """Execute pipeline.
 
         Args:
+            workspace: Workspace where unit is executed
             config: A global config provided by user
-            package: Package descriptor for collecting the pipeline execution status
-            **kwargs: Additional keyword arguments
-
-        Returns:
-            Dictionary with shared parameters
+            context: Context of pipeline execution
         """
         LOGGER.info(pad_string(f"Pipeline {self.name!r} started"))
-        shared_parameters = kwargs
+
         for execution_unit in self.execution_units:
             command_output = self._execute_unit(
-                execution_unit=execution_unit, config=config, status=package.status, shared_parameters=shared_parameters
+                workspace=workspace,
+                execution_unit=execution_unit,
+                config=config,
+                context=context,
             )
-            package._update_status(
+            context.update(
                 execution_unit=execution_unit,
                 command_output=command_output,
-                shared_parameters=shared_parameters,
             )
-            if command_output.output is not None:
-                shared_parameters.update(command_output.output)
-                for name, value in command_output.output.items():
-                    if name in config.__dataclass_fields__:
-                        setattr(config, name, value)
-        return shared_parameters
+            context.save()
 
     def _execute_unit(
-        self, execution_unit: ExecutionUnit, config: CommonConfig, status: Status, shared_parameters: Dict
+        self,
+        workspace: Workspace,
+        execution_unit: ExecutionUnit,
+        config: CommonConfig,
+        context: PipelineContext,
     ) -> CommandOutput:
         """Execute a single unit.
 
         Args:
+            workspace: Workspace where unit is executed
             execution_unit: A unit to execute
-            shared_parameters: Parameters shared between execution units
+            config: Common configuration parameters
+            context: Pipeline execution context
 
         Returns:
             Command execution result
         """
-        log_dir = (
-            execution_unit.config.workspace / execution_unit.model_config.path.parent
-            if execution_unit.model_config
-            else None
-        )
+        log_dir = None
+        if execution_unit.model_config:
+            log_dir = workspace.path / execution_unit.model_config.path.parent
 
-        if execution_unit.config.debug:
+        if config.debug:
             redirect_stdout_context = StdoutLogger(LOGGER)
         else:
             redirect_stdout_context = contextlib.nullcontext()
+
         with LoggingContext(log_dir=log_dir), redirect_stdout_context:
-            LOGGER.info(pad_string(f"Command {execution_unit.command.name()!r} started"))
-            input_paramters = {
-                **execution_unit.config.__dict__,
-                **shared_parameters,
-            }
-
-            input_paramters.update(execution_unit.kwargs)
-            if execution_unit.runner_cls:
-                input_paramters["runner_cls"] = execution_unit.runner_cls
-            if execution_unit.model_config:
-                input_paramters.update(**execution_unit.model_config.get_config_dict_for_command())
+            LOGGER.info(pad_string(f"Command {execution_unit.command.name!r} started"))
             try:
-                command_output = execution_unit.command(status).run(
-                    **input_paramters
-                )  # pytype: disable=not-instantiable
+                context.validate_execution(execution_unit=execution_unit)
+                input_parameters = context.command_args(
+                    workspace=workspace,
+                    config=config,
+                    execution_unit=execution_unit,
+                )
+                command_output = execution_unit.command().run(**input_parameters)  # pytype: disable=not-instantiable
             except ModelNavigatorUserInputError as e:
                 command_output = CommandOutput(status=CommandStatus.FAIL)
 
                 if config.verbose and e.__context__:
                     LOGGER.info(e.__context__)
 
                 error = traceback.format_exc()
                 LOGGER.warning(
                     "Command finished with ModelNavigatorUserInputError. "
                     "The error is considered as external error. Usually caused by "
                     "incompatibilities between the model and the target formats and/or runtimes. "
                     "Please review the command output.\n"
                     f"{error}"
                 )
+            except ModelNavigatorCommandNotExecutable:
+                command_output = CommandOutput(status=CommandStatus.SKIPPED)
             except Exception:
                 command_output = CommandOutput(status=CommandStatus.FAIL)
                 error = traceback.format_exc()
                 LOGGER.error(f"Command finished with unexpected error: {error}")
 
-            if command_output.status == CommandStatus.FAIL and execution_unit.command.is_required():
+            if command_output.status != CommandStatus.OK and execution_unit.command.is_required():
                 sys.exit("The required command has failed. Please, review the log and verify the reported problems.")
 
             return command_output
```

## model_navigator/pipelines/pipeline_manager.py

```diff
@@ -8,191 +8,102 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Pipeline manager submodule."""
-import shutil
-import uuid
 from typing import Dict, List, Optional, Sequence
 
-from tabulate import tabulate
-
-from model_navigator.api.config import Format, TensorRTProfile
+from model_navigator.api.config import Format
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
-from model_navigator.core.constants import NAVIGATOR_PACKAGE_VERSION, NAVIGATOR_VERSION
-from model_navigator.core.package import Package
-from model_navigator.core.status import ModelStatus, Status
-from model_navigator.core.tensor import TensorMetadata
-from model_navigator.logger import LOGGER, add_log_file_handler
+from model_navigator.core.logger import LOGGER, log_dict
+from model_navigator.core.workspace import Workspace
+from model_navigator.package.package import Package
 from model_navigator.pipelines.builders import PipelineBuilder
+from model_navigator.pipelines.pipeline_context import PipelineContext
 from model_navigator.pipelines.validation import PipelineManagerConfigurationValidator
-from model_navigator.utils.common import pad_string
-from model_navigator.utils.environment import get_env
 
 
 class PipelineManager:
     """Class for managing pipelines runs."""
 
     _common_config_filter_fields = [
         "model",
         "model_params",
         "dataloader",
         "workspace",
         "forward_kw_names",
         "verify_func",
     ]
 
-    @classmethod
+    def __init__(self, workspace: Workspace):
+        """Initialize PipelineManager."""
+        self._workspace = workspace
+
     def run(
-        cls,
-        pipeline_builders: Sequence[PipelineBuilder],
+        self,
+        workspace: Workspace,
+        builders: Sequence[PipelineBuilder],
         config: CommonConfig,
         package: Optional[Package] = None,
         models_config: Optional[Dict[Format, List[ModelConfig]]] = None,
-    ) -> Package:
+    ) -> PipelineContext:
         """Run pipeline manager and build a package.
 
         Args:
-            pipeline_builders: List of pipelines builders to run.
+            workspace: Workspace where unit is executed
+            builders: List of pipelines builders to run.
             config: A configuration object
             package: Package to update, if None new package is build. Defaults to None.
             models_config: List of model configs to use in pipelines builders. Defaults to None.
 
         Returns:
             Package object
         """
         if config.verbose or config.debug:
-            config.log()
+            data = config.to_dict(
+                filter_fields=[
+                    "model",
+                    "dataloader",
+                    "verify_func",
+                ],
+                parse=True,
+            )
+            log_dict(title="Common config parameters", data=data)
 
         PipelineManagerConfigurationValidator.run(config, package)
 
-        package = cls._prepare_package(package, config)
+        context = PipelineContext(workspace=self._workspace)
+        context.initialize()
 
-        cls._prepare_log_file(config)
-        cls._run_pipelines_builders(
-            pipeline_builders=pipeline_builders, models_config=models_config, config=config, package=package
-        )
-        package.status.config = config.to_dict(
-            cls._common_config_filter_fields,
-            parse=True,
+        pipelines = self._build_pipelines(
+            builders=builders,
+            models_config=models_config,
+            config=config,
         )
 
-        package.save_status_file()
+        for pipeline in pipelines:
+            pipeline.run(workspace=workspace, config=config, context=context)
+
+        context.log_status()
 
         LOGGER.warning(
             "Initially models are not verified. Validate exported models and use "
             "PackageDescriptor.set_verified(format, runtime, jit_type, precision) method to set models as verified."
         )
 
-        package._forward_kw_names = config.forward_kw_names
-
-        return package
-
-    @classmethod
-    def _new_package(cls, config: CommonConfig):
-        status = Status(
-            uuid=str(uuid.uuid1()),
-            format_version=NAVIGATOR_PACKAGE_VERSION,
-            model_navigator_version=NAVIGATOR_VERSION,
-            environment=get_env(),
-            config={},
-            models_status={},
-            input_metadata=TensorMetadata(),
-            output_metadata=TensorMetadata(),
-            dataloader_trt_profile=TensorRTProfile(),
-            dataloader_max_batch_size=1,
-        )
-
-        package = Package(status, config.workspace, model=config.model)
-
-        return package
-
-    @classmethod
-    def _from_package(cls, package: Package):
-        status = Status(
-            uuid=str(uuid.uuid1()),
-            format_version=NAVIGATOR_PACKAGE_VERSION,
-            model_navigator_version=NAVIGATOR_VERSION,
-            environment=get_env(),
-            config={},
-            models_status={},
-            input_metadata=TensorMetadata(),
-            output_metadata=TensorMetadata(),
-            dataloader_trt_profile=TensorRTProfile(),
-            dataloader_max_batch_size=1,
-        )
+        return context
 
-        package = Package(status, workspace=package.workspace, model=package.model)
-
-        return package
-
-    @classmethod
-    def _prepare_package(cls, package: Optional[Package], config: CommonConfig) -> Package:
-        if package is None:
-            package = cls._new_package(config)
-            cls._prepare_workspace(config)
-        else:
-            package = cls._from_package(package)
-
-        return package
-
-    @classmethod
-    def _run_pipelines_builders(
-        cls,
-        pipeline_builders: Sequence[PipelineBuilder],
+    def _build_pipelines(
+        self,
+        builders: Sequence[PipelineBuilder],
         config: CommonConfig,
-        package: Package,
         models_config: Optional[Dict[Format, List[ModelConfig]]] = None,
-    ) -> None:
-        shared_parameters = {}
-        for pipeline_builder in pipeline_builders:
+    ) -> List:
+        pipelines = []
+        for pipeline_builder in builders:
             pipeline = pipeline_builder(config, models_config)
-            shared_parameters = pipeline.run(config=config, package=package, **shared_parameters)
-            package.save_status_file()
-
-        cls._log_model_status(package.status.models_status)
+            pipelines.append(pipeline)
 
-    @staticmethod
-    def _log_model_status(models_status: Dict[str, ModelStatus]):
-        summary = [[] for _ in range(len(models_status))]
-        model_status, runner_status = None, None
-        for i, model_status in enumerate(models_status.values()):
-            summary[i].append(model_status.model_config.format.value)
-            summary[i].append(model_status.model_config.key)
-            if model_status.model_config.parent_key:
-                summary[i].append(model_status.model_config.parent_key)
-            else:
-                summary[i].append("framework")
-            summary[i].append("\n".join([f"{k}: {v.value}" for k, v in model_status.status.items()]))
-            runtime_status = []
-
-            for runner_status in model_status.runners_status.values():
-                runtime_status.append(
-                    "\n".join(
-                        [runner_status.runner_name] + [f"    {k}: {v.value}" for k, v in runner_status.status.items()]
-                    )
-                )
-            summary[i].append("\n".join(runtime_status))
-
-        headers = ["Format", "Key", "Parent model key"]
-        if model_status:
-            headers.append("Model status")
-        if runner_status:
-            headers.append("Runner status")
-        table = tabulate(summary, headers, "grid")
-        LOGGER.info(f"\n{pad_string('Model Navigator Summary')}\n{table}")
-
-    @staticmethod
-    def _prepare_workspace(config: CommonConfig):
-        workspace = config.workspace
-        if workspace.exists():
-            LOGGER.info(f"Removing exiting workspace at {workspace}")
-            shutil.rmtree(workspace, ignore_errors=True)
-
-        workspace.mkdir(parents=True, exist_ok=True)
-
-    @staticmethod
-    def _prepare_log_file(config: CommonConfig):
-        add_log_file_handler(log_dir=config.workspace)
+        return pipelines
```

## model_navigator/pipelines/validation.py

```diff
@@ -9,32 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Pipeline manager submodule."""
 import warnings
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union, get_args, get_origin
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, get_args, get_origin
 
 from model_navigator.api.config import (
     AVAILABLE_TARGET_FORMATS,
     CustomConfigForFormat,
     Format,
     OnnxConfig,
     ShapeTuple,
     TensorFlowTensorRTConfig,
     TensorRTConfig,
     TensorRTProfile,
     TorchTensorRTConfig,
 )
 from model_navigator.configuration.common_config import CommonConfig
-from model_navigator.core.package import Package
 from model_navigator.exceptions import ModelNavigatorConfigurationError, ModelNavigatorConfigurationWarning
 from model_navigator.frameworks import Framework
+from model_navigator.package.package import Package
 from model_navigator.runners.registry import get_runner
 from model_navigator.utils.format_helpers import get_base_format, get_framework_export_formats
 
 
 class PipelineManagerConfigurationValidator:
     """PipelineManager configuration validator."""
 
@@ -44,21 +43,21 @@
         config: CommonConfig,
         package: Optional[Package] = None,
     ):
         """Validate PipelineManager configuration.
 
         Args:
             config: A configuration object
-            package: Package to be optimized, if None package is yet to be build. Defaults to None.
+            package: Package to be optimized, if None package is yet to be built. Defaults to None.
         """
         cls._validate_if_runners_match_target_device(config)
         cls._validate_config_types(config)
         cls._validate_if_custom_configs_match_target_formats(config)
         cls._validate_if_target_formats_match_framework(config)
-        cls._validate_profiler_config_batch_sizes_when_batching_is_disabled(config)
+        cls._validate_optimization_profile_batch_sizes_when_batching_is_disabled(config)
         for custom_config in config.custom_configs.values():
             if isinstance(custom_config, (TensorRTConfig, TorchTensorRTConfig, TensorFlowTensorRTConfig)):
                 cls._validate_trt_profile_input_names(custom_config.trt_profile, config._input_names)
                 cls._validate_trt_profile_batch_dimension(custom_config.trt_profile, config.batch_dim)
                 for onnx_custom_config in config.custom_configs.values():
                     if isinstance(onnx_custom_config, OnnxConfig):
                         cls._validate_if_trt_profile_aligns_with_dynamic_axes(
@@ -97,18 +96,18 @@
             if target_format not in AVAILABLE_TARGET_FORMATS[config.framework]:
                 raise ModelNavigatorConfigurationError(
                     f"{target_format} is not available for framework {config.framework}. "
                     f"Available target formats: ({AVAILABLE_TARGET_FORMATS[config.framework]})"
                 )
 
     @classmethod
-    def _validate_profiler_config_batch_sizes_when_batching_is_disabled(cls, config: CommonConfig):
-        if config.batch_dim is None and config.profiler_config.batch_sizes:
+    def _validate_optimization_profile_batch_sizes_when_batching_is_disabled(cls, config: CommonConfig):
+        if config.batch_dim is None and config.optimization_profile.batch_sizes:
             raise ModelNavigatorConfigurationError(
-                f"Model does not support batching, but profiling batch sizes are {config.profiler_config.batch_sizes}."
+                f"Model does not support batching, but profiling batch sizes are {config.optimization_profile.batch_sizes}."
             )
 
     @classmethod
     def _validate_trt_profile_input_names(
         cls,
         trt_profile: Optional[TensorRTProfile],
         input_names: Optional[Tuple[str, ...]] = None,
@@ -131,26 +130,26 @@
                         raise ModelNavigatorConfigurationError(
                             f"Shape values are not matching on the batch dimension: {batch_dim} "
                             f"for all inputs in trt_profile: {trt_profile}."
                         )
 
     @classmethod
     def _validate_if_target_formats_sources_are_available_in_package(
-        cls, package: Package, target_formats: Tuple[Format, ...], framework: Framework
+        cls, package: Package, target_formats: Sequence[Format], framework: Framework
     ):
         for target_format in target_formats:
             base_format = (
                 target_format
                 if target_format in get_framework_export_formats(framework)
                 else get_base_format(target_format, framework)
             )
             base_format_available = False
             for model_status in package.status.models_status.values():
                 if model_status.model_config.format == base_format and (
-                    package.workspace / model_status.model_config.path
+                    package.workspace.path / model_status.model_config.path
                 ):
                     base_format_available = True
                     break
             if not base_format_available:
                 warnings.warn(
                     f"Target format {target_format} requires {base_format} format "
                     "to be saved in the package but it is not found. "
@@ -174,17 +173,14 @@
                 continue
 
             if not isinstance(value, expected_type):
                 raise ModelNavigatorConfigurationError(
                     f"Incorrect type for {field_name}. Expected type {expected_type} got {type(value)} instead."
                 )
 
-        if isinstance(config.workspace, str):
-            object.__setattr__(config, "workspace", Path(config.workspace))
-
         if config.from_source:
             try:
                 iter(config.dataloader)
             except TypeError as e:
                 raise ModelNavigatorConfigurationError("Datalaoder must be iterable.") from e
             try:
                 len(config.dataloader)
```

## model_navigator/pipelines/builders/__init__.py

```diff
@@ -15,16 +15,16 @@
 from typing import Callable, Dict, List
 
 from model_navigator.api.config import Format
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
 from model_navigator.frameworks import is_jax_available, is_tf_available, is_torch_available
 from model_navigator.pipelines.builders.correctness import correctness_builder  # noqa: F401
+from model_navigator.pipelines.builders.performance import performance_builder  # noqa: F401
 from model_navigator.pipelines.builders.preprocessing import preprocessing_builder  # noqa: F401
-from model_navigator.pipelines.builders.profiling import profiling_builder  # noqa: F401
 from model_navigator.pipelines.builders.verify import verify_builder  # noqa: F401
 from model_navigator.pipelines.pipeline import Pipeline  # noqa: F401
 
 if is_torch_available():
     from .torch import torch_conversion_builder, torch_export_builder  # noqa: F401
 
 if is_tf_available():
```

## model_navigator/pipelines/builders/correctness.py

```diff
@@ -40,9 +40,11 @@
         for model_config in models_config_list:
             for runner in runner_registry.values():
                 if (
                     runner.format() == model_config.format
                     and runner.name() in config.runner_names
                     and config.target_device in runner.devices_kind()
                 ):
-                    execution_units.append(ExecutionUnit(Correctness, config, model_config, runner))
+                    execution_units.append(
+                        ExecutionUnit(command=Correctness, model_config=model_config, runner_cls=runner)
+                    )
     return Pipeline(name="Correctness", execution_units=execution_units)
```

## model_navigator/pipelines/builders/find_device_max_batch_size.py

```diff
@@ -20,16 +20,16 @@
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import (
     ModelConfig,
     TensorFlowTensorRTConfig,
     TensorRTConfig,
     TorchTensorRTConfig,
 )
+from model_navigator.core.logger import LOGGER
 from model_navigator.frameworks import Framework
-from model_navigator.logger import LOGGER
 from model_navigator.pipelines.pipeline import Pipeline
 from model_navigator.runners.onnx import OnnxrtCUDARunner
 from model_navigator.runners.tensorflow import TensorFlowSavedModelCUDARunner
 from model_navigator.runners.torch import TorchScriptCUDARunner
 
 
 def do_run_max_batch_size_search(
@@ -61,14 +61,15 @@
         Pipeline with steps for find max batch size.
     """
     pipeline_name = "Find Device Max Batch Size"
     execution_units: List[ExecutionUnit] = []
     model_formats = models_config.keys()
     adaptive_formats = {Format.TORCH_TRT, Format.TENSORRT, Format.TF_TRT}
     matching_formats = adaptive_formats.intersection(set(model_formats))
+
     if len(matching_formats) == 0 or config.target_device != DeviceKind.CUDA:
         LOGGER.debug("No matching formats found")
         return Pipeline(name=pipeline_name, execution_units=execution_units)
 
     run_search = False
     for fmt in adaptive_formats:
         for model_cfg in models_config.get(fmt, []):
@@ -129,13 +130,12 @@
                 runner_cls=runner_cls,
             )
             configurations.append(mbs_config)
 
     execution_units.append(
         ExecutionUnit(
             command=FindMaxBatchSize,
-            config=config,
             configurations=configurations,
         )
     )
 
     return Pipeline(name=pipeline_name, execution_units=execution_units)
```

## model_navigator/pipelines/builders/jax.py

```diff
@@ -31,9 +31,9 @@
         models_config: List of model configs per format
 
     Returns:
         Pipeline with steps for export
     """
     execution_units: List[ExecutionUnit] = []
     for model_cfg in models_config.get(Format.TF_SAVEDMODEL, []):
-        execution_units.append(ExecutionUnit(ExportJAX2SavedModel, config, model_cfg))
+        execution_units.append(ExecutionUnit(command=ExportJAX2SavedModel, model_config=model_cfg))
     return Pipeline(name="JAX Export", execution_units=execution_units)
```

## model_navigator/pipelines/builders/onnx.py

```diff
@@ -32,15 +32,15 @@
         models_config (Dict[Format, List[ModelConfig]]): Models optimize configs.
 
     Returns:
         Pipeline: Export pipeline.
     """
     execution_units: List[ExecutionUnit] = []
     for model_cfg in models_config.get(Format.ONNX, []):
-        execution_units.append(ExecutionUnit(CopyONNX, config, model_cfg))
+        execution_units.append(ExecutionUnit(command=CopyONNX, model_config=model_cfg))
 
     return Pipeline(name="ONNX Export", execution_units=execution_units)
 
 
 def onnx_conversion_builder(config: CommonConfig, models_config: Dict[Format, List[ModelConfig]]) -> Pipeline:
     """Build ONNX conversion pipeline.
 
@@ -52,9 +52,9 @@
         Pipeline: Conversion pipeline.
     """
     execution_units: List[ExecutionUnit] = []
     if is_trt_available() and config.target_device == DeviceKind.CUDA:
         from model_navigator.commands.convert.onnx import ConvertONNX2TRT
 
         for model_cfg in models_config.get(Format.TENSORRT, []):
-            execution_units.append(ExecutionUnit(ConvertONNX2TRT, config, model_cfg))
+            execution_units.append(ExecutionUnit(command=ConvertONNX2TRT, model_config=model_cfg))
     return Pipeline(name="ONNX Conversion", execution_units=execution_units)
```

## model_navigator/pipelines/builders/preprocessing.py

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 """Preprocessing pipelines builders."""
 
 from typing import Dict, List
 
 from model_navigator.api.config import Format
 from model_navigator.commands.base import ExecutionUnit
-from model_navigator.commands.data_dump.samples import DumpInputModelData, DumpOutputModelData, FetchInputModelData
+from model_navigator.commands.data_dump.samples import FetchInputModelData, FetchOutputModelData
 from model_navigator.commands.infer_metadata import InferInputMetadata, InferOutputMetadata
-from model_navigator.commands.load import LoadMetadata, LoadSamples
+from model_navigator.commands.load import LoadMetadata
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
 from model_navigator.pipelines.pipeline import Pipeline
 
 
 def preprocessing_builder(config: CommonConfig, models_config: Dict[Format, List[ModelConfig]]) -> Pipeline:
     """Build profiling pipeline.
@@ -39,18 +39,17 @@
     Returns:
         Pipeline with steps for profiling.
     """
     execution_units: List[ExecutionUnit] = []
     if config.from_source:
         execution_units.extend(
             [
-                ExecutionUnit(InferInputMetadata, config),
-                ExecutionUnit(FetchInputModelData, config),
-                ExecutionUnit(InferOutputMetadata, config),
-                ExecutionUnit(DumpInputModelData, config),
-                ExecutionUnit(DumpOutputModelData, config),
+                ExecutionUnit(command=InferInputMetadata),
+                ExecutionUnit(command=FetchInputModelData),
+                ExecutionUnit(command=InferOutputMetadata),
+                ExecutionUnit(command=FetchOutputModelData),
             ]
         )
     else:
-        execution_units.extend([ExecutionUnit(LoadMetadata, config), ExecutionUnit(LoadSamples, config)])
+        execution_units.extend([ExecutionUnit(command=LoadMetadata)])
 
     return Pipeline(name="Preprocessing", execution_units=execution_units)
```

## model_navigator/pipelines/builders/profiling.py

```diff
@@ -14,16 +14,15 @@
 """Profiling pipelines builders."""
 
 
 from typing import Dict, List
 
 from model_navigator.api.config import Format
 from model_navigator.commands.base import ExecutionUnit
-from model_navigator.commands.load import LoadMetadata, LoadSamples
-from model_navigator.commands.performance import Performance
+from model_navigator.commands.performance import Profile
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
 from model_navigator.pipelines.pipeline import Pipeline
 from model_navigator.runners.registry import runner_registry
 from model_navigator.utils.format_helpers import is_source_format
 
 
@@ -34,30 +33,29 @@
         config: A configuration for pipelines
         models_config: List of model configs per format
 
     Returns:
         Pipeline with steps for profiling.
     """
     execution_units: List[ExecutionUnit] = []
-    execution_units.extend([ExecutionUnit(LoadMetadata, config), ExecutionUnit(LoadSamples, config)])
 
     source_last_formats = [
         *[model_format for model_format in models_config.keys() if not is_source_format(model_format)],
         *[model_format for model_format in models_config.keys() if is_source_format(model_format)],
     ]
+
     for model_format in source_last_formats:
         for model_config in models_config[model_format]:
             for runner in runner_registry.values():
                 if (
                     runner.format() == model_config.format
                     and runner.name() in config.runner_names
                     and config.target_device in runner.devices_kind()
                 ):
                     execution_units.append(
                         ExecutionUnit(
-                            Performance,
-                            config,
-                            model_config,
-                            runner,
+                            command=Profile,
+                            model_config=model_config,
+                            runner_cls=runner,
                         )
                     )
     return Pipeline(name="Profiling", execution_units=execution_units)
```

## model_navigator/pipelines/builders/tensorflow.py

```diff
@@ -33,15 +33,15 @@
         models_config (Dict[Format, List[ModelConfig]]): Models optimize configs.
 
     Returns:
         Pipeline: Export pipeline.
     """
     execution_units: List[ExecutionUnit] = []
     for model_cfg in models_config.get(Format.TF_SAVEDMODEL, []):
-        execution_units.append(ExecutionUnit(ExportTF2SavedModel, config, model_cfg))
+        execution_units.append(ExecutionUnit(command=ExportTF2SavedModel, model_config=model_cfg))
     return Pipeline(name="TensorFlow2 Export", execution_units=execution_units)
 
 
 def tensorflow_conversion_builder(config: CommonConfig, models_config: Dict[Format, List[ModelConfig]]) -> Pipeline:
     """Build Tensorflow conversion pipeline.
 
     Args:
@@ -49,15 +49,15 @@
         models_config (Dict[Format, List[ModelConfig]]): Models optimize configs.
 
     Returns:
         Pipeline: Conversion pipeline.
     """
     execution_units: List[ExecutionUnit] = []
     for model_cfg in models_config.get(Format.ONNX, []):
-        execution_units.append(ExecutionUnit(ConvertSavedModel2ONNX, config, model_cfg))
+        execution_units.append(ExecutionUnit(command=ConvertSavedModel2ONNX, model_config=model_cfg))
     if config.target_device == DeviceKind.CUDA:
         for model_cfg in models_config.get(Format.TF_TRT, []):
-            execution_units.append(ExecutionUnit(ConvertSavedModel2TFTRT, config, model_cfg))
+            execution_units.append(ExecutionUnit(command=ConvertSavedModel2TFTRT, model_config=model_cfg))
         for model_cfg in models_config.get(Format.TENSORRT, []):
-            execution_units.append(ExecutionUnit(ConvertONNX2TRT, config, model_cfg))
+            execution_units.append(ExecutionUnit(command=ConvertONNX2TRT, model_config=model_cfg))
 
     return Pipeline(name="TensorFlow2 Conversion", execution_units=execution_units)
```

## model_navigator/pipelines/builders/torch.py

```diff
@@ -32,19 +32,19 @@
         models_config: List of model configs per format
 
     Returns:
         Pipeline with steps for export
     """
     execution_units: List[ExecutionUnit] = []
     for model_cfg in models_config.get(Format.TORCHSCRIPT, []):
-        execution_units.append(ExecutionUnit(ExportTorch2TorchScript, config, model_cfg))
+        execution_units.append(ExecutionUnit(command=ExportTorch2TorchScript, model_config=model_cfg))
 
     for model_cfg in models_config.get(Format.ONNX, []):
         if model_cfg.parent_path in (None, Format.TORCH):
-            execution_units.append(ExecutionUnit(ExportTorch2ONNX, config, model_cfg))
+            execution_units.append(ExecutionUnit(command=ExportTorch2ONNX, model_config=model_cfg))
 
     return Pipeline(name="PyTorch Export", execution_units=execution_units)
 
 
 def torch_conversion_builder(config: CommonConfig, models_config: Dict[Format, List[ModelConfig]]) -> Pipeline:
     """Prepare conversions steps for pipeline.
 
@@ -56,15 +56,15 @@
         Pipeline with steps for conversion
     """
     execution_units: List[ExecutionUnit] = []
     for model_cfg in models_config.get(Format.ONNX, []):
         if (
             model_cfg.parent_path and Format.TORCHSCRIPT.value in model_cfg.parent_path.as_posix()
         ):  # FIXME find better way to distinguish ONNX from source from ONNX from TorchScript
-            execution_units.append(ExecutionUnit(ConvertTorchScript2ONNX, config, model_cfg))
+            execution_units.append(ExecutionUnit(command=ConvertTorchScript2ONNX, model_config=model_cfg))
     if config.target_device == DeviceKind.CUDA:
         for model_cfg in models_config.get(Format.TORCH_TRT, []):
-            execution_units.append(ExecutionUnit(ConvertTorchScript2TorchTensorRT, config, model_cfg))
+            execution_units.append(ExecutionUnit(command=ConvertTorchScript2TorchTensorRT, model_config=model_cfg))
         for model_cfg in models_config.get(Format.TENSORRT, []):
-            execution_units.append(ExecutionUnit(ConvertONNX2TRT, config, model_cfg))
+            execution_units.append(ExecutionUnit(command=ConvertONNX2TRT, model_config=model_cfg))
 
     return Pipeline(name="PyTorch Conversion", execution_units=execution_units)
```

## model_navigator/pipelines/builders/verify.py

```diff
@@ -40,9 +40,11 @@
         for model_config in models_config_list:
             for runner in runner_registry.values():
                 if (
                     runner.format() == model_config.format
                     and runner.name() in config.runner_names
                     and config.target_device in runner.devices_kind()
                 ):
-                    execution_units.append(ExecutionUnit(VerifyModel, config, model_config, runner))
-    return Pipeline(name="Verfiy Models", execution_units=execution_units)
+                    execution_units.append(
+                        ExecutionUnit(command=VerifyModel, model_config=model_config, runner_cls=runner)
+                    )
+    return Pipeline(name="Verify Models", execution_units=execution_units)
```

## model_navigator/runners/base.py

```diff
@@ -15,17 +15,17 @@
 
 import abc
 import time
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 
-from model_navigator.api.config import DeviceKind, Format
-from model_navigator.core.tensor import TensorMetadata
-from model_navigator.logger import LOGGER
+from model_navigator.api.config import DeviceKind, Format, TensorType
+from model_navigator.core.logger import LOGGER
+from model_navigator.core.tensor import TensorMetadata, TensorSpec, get_tensor_type
 from model_navigator.utils.dataloader import validate_sample_output
 
 
 class NavigatorRunner(abc.ABC):
     """Base abstract runner.
 
     Example usage:
@@ -36,30 +36,35 @@
 
     def __init__(
         self,
         model: Any,
         input_metadata: TensorMetadata,
         output_metadata: TensorMetadata,
         input_metadata_mapping: Optional[Dict[str, str]] = None,
+        return_type: TensorType = TensorType.NUMPY,
         *args,
         **kwargs,
     ) -> None:
         """Initialize object.
 
         Args:
             model: A model for which runner has to be initialized
             input_metadata: A model inputs metadata
             output_metadata: A model outputs metadata
             input_metadata_mapping: Optional mapping for input metadata
+            return_type: A type of return value
         """
         self._model = model
         self._input_metadata = input_metadata
         self._output_metadata = output_metadata
         self._input_metadata_mapping = input_metadata_mapping
 
+        self._check_return_type(return_type)
+        self._return_type = return_type
+
         self.inference_time = None
         self.is_active = False
 
         self.init_impl()
 
     @property
     def model(self) -> Any:
@@ -77,14 +82,19 @@
         return self._output_metadata
 
     @property
     def input_metadata_mapping(self) -> Optional[Dict[str, str]]:
         """Property for obtaining model input metadata mapping."""
         return self._input_metadata_mapping
 
+    @property
+    def return_type(self) -> TensorType:
+        """Property for obtaining runner return type."""
+        return self._return_type
+
     @classmethod
     def name(cls) -> str:
         """Return name of the runner."""
         return cls.__name__
 
     @classmethod
     @abc.abstractmethod
@@ -178,28 +188,27 @@
                 "If you really want to activate this runner again, call activate_impl() directly"
             )
             return
 
         self.activate_impl()
         self.is_active = True
 
-    def infer(
-        self, feed_dict: Dict[str, np.ndarray], check_inputs: bool = True, *args: Any, **kwargs: Any
-    ) -> Dict[str, np.ndarray]:
+    def infer(self, feed_dict: Dict[str, Any], check_inputs: bool = True, *args: Any, **kwargs: Any) -> Dict[str, Any]:
         """Runs inference using the provided feed_dict.
 
         Must be called only after ``activate()`` and before ``deactivate()``.
 
         NOTE: Some runners may accept additional parameters in infer().
         For details on these, see the documentation for their `infer_impl()` methods.
 
         Args:
             feed_dict: A mapping of input tensor names to corresponding input NumPy arrays.
-            check_inputs: Whether to check that the provided ``feed_dict`` includes the expected inputs with the
-                    expected data types and shapes. Disabling this may improve performance. Defaults to True.
+            check_inputs: Whether to check that the provided ``feed_dict`` and generated outputs includes the expected
+                inputs / outputs with the expected data types and shapes. Disabling this may improve performance.
+                Defaults to True.
 
         Returns:
             A dictionary with mapping of output tensor names to their corresponding NumPy arrays.
 
             IMPORTANT: Runners may reuse these output buffers. Thus, if you need to save
             outputs from multiple inferences, you should make a copy with ``copy.deepcopy(outputs)``.
         """
@@ -211,32 +220,40 @@
             LOGGER.debug(f"Runner input metadata is: {input_metadata}")
 
             for name in input_metadata:
                 if name not in feed_dict:
                     LOGGER.warning("Input tensor: {name} | Missing input in `feed_dict`: {name}.")
 
             for name, inp in feed_dict.items():
+                if get_tensor_type(inp) not in self.get_available_input_types():
+                    LOGGER.warning(
+                        f"Input tensor: {name} | Received unexpected type: {get_tensor_type(inp)}.\n"
+                        f"Note: Expected one of: {self.get_available_input_types()}"
+                    )
+
                 meta = input_metadata[name]
-                if not meta.is_dtype_compatible(inp):
+                inp_spec = TensorSpec.from_tensor(inp, name)
+                if not meta.is_dtype_compatible(inp_spec):
                     LOGGER.warning(
-                        f"Input tensor: {name} | Received unexpected dtype: {inp.dtype}.\n"
+                        f"Input tensor: {name} | Received unexpected dtype: {inp_spec.dtype}.\n"
                         f"Note: Expected type: {meta.dtype}"
                     )
 
-                if not meta.is_shape_compatible(inp):
+                if not meta.is_shape_compatible(inp_spec):
                     LOGGER.warning(
-                        f"Input tensor: {name} | Received incompatible shape: {inp.shape}.\n"
+                        f"Input tensor: {name} | Received incompatible shape: {inp_spec.shape}.\n"
                         f"Note: Expected a shape compatible with: {meta.shape}"
                     )
 
         start_time = time.monotonic()
         output = self.infer_impl(feed_dict, *args, **kwargs)
         end_time = time.monotonic()
 
-        validate_sample_output(output)
+        if check_inputs:
+            validate_sample_output(output, self.return_type)
 
         self.inference_time = end_time - start_time
         return output
 
     def last_inference_time(self) -> Optional[float]:
         """Returns the total inference time in seconds required during the last call to ``infer()``.
 
@@ -265,20 +282,65 @@
 
         self.inference_time = None
         self.is_active = None
 
         self.deactivate_impl()
         self.is_active = False
 
+    def get_available_return_types(self) -> List[TensorType]:
+        """Returns a list of available return types.
+
+        Returns:
+            A list of available return types.
+        """
+        return self.get_available_return_types_impl()
+
+    def get_available_return_types_impl(self) -> List[TensorType]:
+        """Implementation for getting available return types.
+
+        Derived classes should override this function rather than ``get_available_return_types()``.
+        """
+        return [TensorType.NUMPY]
+
+    def get_available_input_types(self) -> List[TensorType]:
+        """Returns a list of available input types.
+
+        Returns:
+            A list of available input types.
+        """
+        return self.get_available_input_types_impl()
+
+    def get_available_input_types_impl(self) -> List[TensorType]:
+        """Implementation for getting available input types.
+
+        Derived classes should override this function rather than ``get_available_input_types()``.
+        """
+        return [TensorType.NUMPY]
+
     def __del__(self):
         """Cleanup of object removal. Log warning when `deactivate` was not called before runner was removed."""
         if self.is_active:
             # __del__ is not guaranteed to be called, but when it is, this could be a useful warning.
             LOGGER.warning(f"{self.name()} | Was activated but never deactivated. This could cause a memory leak!")
 
+    def _check_return_type(self, return_type: TensorType) -> None:
+        """Check if return type is available.
+
+        Args:
+            return_type: TensorType to check.
+
+        Raises:
+            ValueError: If return_type is not available.
+        """
+        available_return_types = self.get_available_return_types()
+        if return_type not in available_return_types:
+            raise ValueError(
+                f"{self.name()} | `return_type` must be one of {available_return_types}, but got: {return_type}"
+            )
+
 
 class NavigatorStabilizedRunner(NavigatorRunner):
     """Stabilized runner base class."""
 
     @classmethod
     def is_stabilized(cls) -> bool:
         """Override is_stabilized class method and always return True."""
```

## model_navigator/runners/onnx.py

```diff
@@ -12,19 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ONNX runners."""
 from collections import OrderedDict
 from typing import List, Optional, Sequence, Union
 
 import model_navigator.utils.common as utils
-from model_navigator.api.config import Format
-from model_navigator.core.tensor import TensorMetadata
+from model_navigator.api.config import Format, TensorType
+from model_navigator.core.logger import LOGGER
+from model_navigator.core.tensor import TensorMetadata, get_tensor_type
 from model_navigator.exceptions import ModelNavigatorNotFoundError
 from model_navigator.frameworks.onnx.utils import ONNX_RT_TYPE_TO_NP
-from model_navigator.logger import LOGGER
+from model_navigator.frameworks.tensorrt.cuda import DeviceView
 from model_navigator.runners.base import DeviceKind, NavigatorRunner
 from model_navigator.runners.registry import register_runner
 from model_navigator.utils import module
 
 onnxrt = module.lazy_import("onnxruntime")
 np = module.lazy_import("numpy")
 
@@ -98,15 +99,15 @@
         meta = TensorMetadata()
         for node in self.sess.get_inputs():
             dtype = ONNX_RT_TYPE_TO_NP[node.type] if node.type in ONNX_RT_TYPE_TO_NP else None
             meta.add(node.name, dtype=dtype, shape=node.shape)
         return meta
 
     def get_onnx_input_metadata(self):
-        assert self.is_active, "Runner must be activated."
+        assert self.is_active and hasattr(self, "sess"), "Runner must be activated."
 
         input_metadata = TensorMetadata()
         for node in self.sess.get_inputs():
             dtype = ONNX_RT_TYPE_TO_NP[node.type] if node.type in ONNX_RT_TYPE_TO_NP else None
             shape = tuple(dim if isinstance(dim, int) else -1 for dim in node.shape)
             input_metadata.add(node.name, shape, dtype)
         return input_metadata
@@ -122,28 +123,23 @@
         self.sess, _ = utils.invoke_if_callable(self._sess)
         if self._disable_fallback:
             LOGGER.info("Disable fallback for ONNX execution provider.")
             active_providers = self.sess.get_providers()
             if self._provider not in active_providers:
                 raise RuntimeError(f"Unable to initialize defined provider: {self._provider}.")
 
-    def infer_impl(self, feed_dict):
-        input_metadata = self.get_onnx_input_metadata()
-        feed_dict = {name: tensor for name, tensor in feed_dict.items() if name in input_metadata}
-
-        inference_outputs = self.sess.run(None, feed_dict)
-        out_dict = OrderedDict()
-        for node, out in zip(self.sess.get_outputs(), inference_outputs):
-            out_dict[node.name] = out
-        out_dict = {k: v for k, v in out_dict.items() if k in self.output_metadata}
-        return out_dict
-
     def deactivate_impl(self):
         del self.sess
 
+    def get_available_input_types(self) -> List[TensorType]:
+        return [TensorType.NUMPY, TensorType.TORCH]
+
+    def get_available_return_types_impl(self) -> List[TensorType]:
+        return [TensorType.NUMPY, TensorType.TORCH]
+
 
 class OnnxrtCPURunner(_BaseOnnxrtRunner):
     """ONNX runner for CPU runtime provider."""
 
     _provider = "CPUExecutionProvider"
 
     @classmethod
@@ -152,14 +148,38 @@
         return "OnnxCPU"
 
     @classmethod
     def devices_kind(cls) -> List[DeviceKind]:
         """Return supported devices for runner."""
         return [DeviceKind.CPU]
 
+    def infer_impl(self, feed_dict):
+        """Run inference."""
+        assert self.is_active and hasattr(self, "sess"), "Runner must be activated."
+
+        input_metadata = self.get_onnx_input_metadata()
+        feed_dict = {name: self._to_numpy(tensor) for name, tensor in feed_dict.items() if name in input_metadata}
+
+        inference_outputs = self.sess.run(None, feed_dict)
+        out_dict = OrderedDict()
+        for node, out in zip(self.sess.get_outputs(), inference_outputs):
+            out_dict[node.name] = out
+        out_dict = {k: v for k, v in out_dict.items() if k in self.output_metadata}
+        return out_dict
+
+    @staticmethod
+    def _to_numpy(tensor):
+        tensor_type = get_tensor_type(tensor)
+        if tensor_type == TensorType.NUMPY:
+            return tensor
+        elif tensor_type == TensorType.TORCH:
+            return tensor.detach().cpu().numpy()
+        else:
+            raise ValueError(f"Unsupported tensor type: {tensor_type}")
+
 
 class OnnxrtCUDARunner(_BaseOnnxrtRunner):
     """ONNX runner for CUDA runtime provider."""
 
     _provider = "CUDAExecutionProvider"
 
     @classmethod
@@ -168,16 +188,61 @@
         return "OnnxCUDA"
 
     @classmethod
     def devices_kind(cls) -> List[DeviceKind]:
         """Return supported devices for runner."""
         return [DeviceKind.CUDA]
 
+    def infer_impl(self, feed_dict):
+        """Run inference."""
+        assert self.is_active and hasattr(self, "sess"), "Runner must be activated."
+
+        input_metadata = self.get_onnx_input_metadata()
+        feed_dict = {name: tensor for name, tensor in feed_dict.items() if name in input_metadata}
+
+        io_binding = self._get_io_bindings(feed_dict)
+        self.sess.run_with_iobinding(io_binding)
+        io_binding.synchronize_outputs()
+
+        out_dict = OrderedDict()
+        for node, out in zip(self.sess.get_outputs(), io_binding.get_outputs()):
+            device_view = DeviceView(out.data_ptr(), out.shape(), ONNX_RT_TYPE_TO_NP[out.data_type()])
+            out_dict[node.name] = device_view.torch() if self.return_type == TensorType.TORCH else device_view.numpy()
+
+        out_dict = {k: v for k, v in out_dict.items() if k in self.output_metadata}
+        return out_dict
+
+    def _get_io_bindings(self, feed_dict):
+        assert self.is_active and hasattr(self, "sess"), "Runner must be activated."
+
+        io_binding = self.sess.io_binding()
+        for name, tensor in feed_dict.items():
+            tensor_type = get_tensor_type(tensor)
+            if tensor_type == TensorType.TORCH:
+                tensor = tensor.to(DeviceKind.CUDA.value)
+                io_binding.bind_input(
+                    name,
+                    DeviceKind.CUDA.value,
+                    0,
+                    utils.torch_to_numpy_dtype(tensor.dtype),
+                    tensor.shape,
+                    tensor.data_ptr(),
+                )
+            else:
+                assert tensor_type == TensorType.NUMPY
+                io_binding.bind_cpu_input(name, tensor)
+        io_binding.synchronize_inputs()
+
+        for name in self.output_metadata:
+            io_binding.bind_output(name, DeviceKind.CUDA.value, 0)
+
+        return io_binding
+
 
-class OnnxrtTensorRTRunner(_BaseOnnxrtRunner):
+class OnnxrtTensorRTRunner(OnnxrtCUDARunner):
     """ONNX runner for TensorRT runtime provider."""
 
     _provider = "TensorrtExecutionProvider"
 
     @classmethod
     def name(cls) -> str:
         """Get runner name."""
```

## model_navigator/runners/registry.py

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Runners global registry."""
 from typing import Dict, Type, Union
 
 import pkg_resources
 
-from model_navigator.logger import LOGGER
+from model_navigator.core.logger import LOGGER
 from model_navigator.runners.base import NavigatorRunner
 
 runner_registry: Dict[str, Type[NavigatorRunner]] = {}
 
 
 def load_runners_from_entry_points():
     """Load runners from package entrypoints."""
```

## model_navigator/runners/tensorrt.py

```diff
@@ -16,25 +16,27 @@
 import copy
 from collections import OrderedDict
 from distutils.version import LooseVersion
 from typing import List, Optional, Sequence
 
 import numpy as np
 
-from model_navigator.api.config import Format
+from model_navigator.api.config import Format, TensorType
+from model_navigator.core.logger import LOGGER
+from model_navigator.core.tensor import get_tensor_type
 from model_navigator.exceptions import ModelNavigatorError, ModelNavigatorUserInputError
 from model_navigator.frameworks.tensorrt import cuda as cuda_utils
 from model_navigator.frameworks.tensorrt import utils as trt_utils
-from model_navigator.logger import LOGGER
 from model_navigator.runners.base import DeviceKind, NavigatorRunner
 from model_navigator.runners.registry import register_runner
 from model_navigator.utils import common as utils
 from model_navigator.utils import module
 
 trt = module.lazy_import("tensorrt")
+torch = module.lazy_import("torch")
 
 
 class FormattedArray:
     """Representes an array whose semantic shape differs from its physical size in memory.
 
     [EXPERIMENTAL, UNTESTED] This API is experimental and untested and may be significantly
     modified in future releases. Use with caution!
@@ -147,14 +149,28 @@
             self.context.set_optimization_profile_async
         except AttributeError:
             self.context.active_optimization_profile = index
         else:
             if not self.context.set_optimization_profile_async(index, self.stream.ptr):
                 raise ModelNavigatorError(f"Failed to set optimization profile to: {index}")
 
+    def get_available_return_types_impl(self) -> List[TensorType]:
+        """Implementation of get_available_return_types method."""
+        if trt_utils._should_use_v3_api():
+            return [TensorType.NUMPY, TensorType.TORCH]
+        else:
+            return [TensorType.NUMPY]
+
+    def get_available_input_types(self) -> List[TensorType]:
+        """Implementation of get_available_return_types method."""
+        if trt_utils._should_use_v3_api():
+            return [TensorType.NUMPY, TensorType.TORCH]
+        else:
+            return [TensorType.NUMPY]
+
     def get_input_metadata_impl(self):
         """Implementation of get_input_metadata method.
 
         Returns:
             TensorMetadata: Input metadata.
         """
         if trt_utils._should_use_v3_api():
@@ -340,26 +356,24 @@
                 output_buffers[name] = self.host_output_buffers[name]
             else:
                 output_buffers[name] = dev_bufs[name].view()
 
         self.stream.synchronize()
         return output_buffers
 
-    def _infer_impl_v3(self, feed_dict, copy_outputs_to_host):  # noqa: C901
+    def _infer_impl_v3(self, feed_dict):  # noqa C901
         reshape = False
         for idx in range(self.engine.num_io_tensors):
             name = self.engine.get_tensor_name(idx)
 
             if self.engine.get_tensor_mode(name) != trt.TensorIOMode.INPUT:
                 continue
 
             # Set up input tensor shapes and copy from host memory if needed
-            array = feed_dict[name]
-            if not isinstance(array, FormattedArray):
-                array = FormattedArray(array, shape=array.shape, dtype=array.dtype)  # pytype: disable=wrong-arg-types
+            array = self._input_tensor_view(feed_dict, name)
 
             underlying_array = array.array
 
             ptr = None
             if self.engine.is_shape_inference_io(name):
                 if not isinstance(underlying_array, np.ndarray):
                     raise ModelNavigatorUserInputError(
@@ -389,19 +403,23 @@
                         f"For input: {name}, unrecognized type in feed_dict: {type(underlying_array).__name__}.\n"
                         "Please provide either a NumPy array or DeviceView. "
                     )
 
             # Only update the input shape/address if something has changed. Otherwise, we'd be
             # doing extra work unnecessarily.
             # We retrieve the semantic shape from the FormattedArray, *not* the underlying array.
-            if self.context.get_tensor_shape(name) != array.shape:
+            tensor_shape = self.context.get_tensor_shape(name)
+            if tensor_shape != array.shape:
                 LOGGER.debug(f"Setting {name} input shape to: {array.shape}")
                 reshape = True
                 if not self.context.set_input_shape(name, array.shape):
-                    raise ModelNavigatorError(f"For input: {name}, failed to set shape to: {array.shape}")
+                    raise ModelNavigatorError(
+                        f"""For input: {name}, failed to set shape from {tensor_shape} to: {array.shape}."""
+                        f"""Please, review if input data shape match the maximal input size which is {tensor_shape}."""
+                    )
 
             if self.context.get_tensor_address(name) != ptr:
                 if not self.context.set_tensor_address(name, ptr):
                     raise ModelNavigatorError(f"For input: {name}, failed to set tensor address to: {ptr}")
         # Any change in shape requires recapture of CUDA graph
         if reshape:
             self.cuda_graph = None
@@ -433,44 +451,64 @@
             if not self.context.execute_async_v3(self.stream.ptr):
                 raise ModelNavigatorError(
                     "`execute_async_v3()` failed. Please see the logging output above for details."
                 )
 
         output_buffers = OrderedDict()
         for name in self.host_output_buffers.keys():
-            # If we're dealing with vectorized formats, we need to return a FormattedArray.
-            # Otherwise, we create a view instead with the correct shape/dtype.
-            raw_array = self.output_allocator.buffers[name]
-            shape = self.output_allocator.shapes[name]
-            dtype = np.dtype(trt.nptype(self.engine.get_tensor_dtype(name)))
-
-            using_nonlinear_format = self.engine.get_tensor_format(name) != trt.TensorFormat.LINEAR
-            # The memory allocated by the output allocator may be larger than actually required.
-            # If we're using a vectorized format, then we need to copy the whole thing.
-            # Otherwise, we can determine how much we actually need.
-            nbytes = raw_array.nbytes if using_nonlinear_format else (utils.volume(shape) * dtype.itemsize)
-
-            if copy_outputs_to_host:
-                self.host_output_buffers[name] = utils.resize_buffer(self.host_output_buffers[name], (nbytes,))
-                raw_array.view(shape=(nbytes,)).copy_to(self.host_output_buffers[name], stream=self.stream)
-                raw_array = self.host_output_buffers[name]
-
-            if using_nonlinear_format:
-                array = FormattedArray(raw_array, shape=shape, dtype=dtype)
-            else:
-                if copy_outputs_to_host:
-                    array = raw_array.view(dtype).reshape(shape)
-                else:
-                    array = cuda_utils.DeviceView(raw_array.ptr, shape, dtype)
-            output_buffers[name] = array
+            output_buffers[name] = self._output_tensor_view(name, self.return_type)
 
         self.stream.synchronize()
         return output_buffers
 
-    def infer_impl(self, feed_dict, copy_outputs_to_host=None):
+    def _input_tensor_view(self, feed_dict, name) -> FormattedArray:
+        # Set up input tensor shapes and copy from host memory if needed
+        array = feed_dict[name]
+        tensor_type = get_tensor_type(array)
+        if tensor_type == TensorType.TORCH:
+            if not array.is_cuda:
+                array = array.cuda()
+            array = cuda_utils.DeviceView(
+                ptr=array.data_ptr(), shape=array.shape, dtype=utils.torch_to_numpy_dtype(array.dtype)
+            )
+        array = FormattedArray(array, shape=array.shape, dtype=array.dtype)  # pytype: disable=wrong-arg-types
+        return array
+
+    def _output_tensor_view(self, name, return_type):
+        # If we're dealing with vectorized formats, we need to return a FormattedArray.
+        # Otherwise, we create a view instead with the correct shape/dtype.
+        raw_array = self.output_allocator.buffers[name]
+        shape = self.output_allocator.shapes[name]
+        dtype = np.dtype(trt.nptype(self.engine.get_tensor_dtype(name)))
+
+        using_nonlinear_format = self.engine.get_tensor_format(name) != trt.TensorFormat.LINEAR
+        if using_nonlinear_format:
+            raise NotImplementedError("Nonlinear formats are not yet supported.")
+        # The memory allocated by the output allocator may be larger than actually required.
+        # If we're using a vectorized format, then we need to copy the whole thing.
+        # Otherwise, we can determine how much we actually need.
+        nbytes = raw_array.nbytes if using_nonlinear_format else (utils.volume(shape) * dtype.itemsize)
+
+        if return_type == TensorType.NUMPY:
+            self.host_output_buffers[name] = utils.resize_buffer(self.host_output_buffers[name], (nbytes,))
+            raw_array.view(shape=(nbytes,)).copy_to(self.host_output_buffers[name], stream=self.stream)
+            raw_array = self.host_output_buffers[name]
+
+            array = FormattedArray(raw_array, shape=shape, dtype=dtype)
+            array = raw_array.view(dtype).reshape(shape)
+        else:
+            assert return_type == TensorType.TORCH
+            array = cuda_utils.DeviceView(raw_array.ptr, shape, dtype).torch(stream=self.stream)
+
+        return array
+
+    def infer_impl(
+        self,
+        feed_dict,
+    ):
         """Implementation for running inference with TensorRT.
 
         Do not call this method directly - use ``infer()`` instead,
         which will forward unrecognized arguments to this method.
 
         In addition to accepting NumPy arrays in the feed_dict, this runner can also
         accept DeviceViews. In that case, no host-to-device copy is necessary for the inputs.
@@ -489,23 +527,23 @@
         Returns:
             OrderedDict[str, Union[numpy.ndarray, DeviceView]]:
                     A mapping of output tensor names to corresponding output NumPy arrays
                     or DeviceViews.
         """
         input_metadata = self.get_input_metadata_impl()
         feed_dict = {
-            name: trt_utils.cast_tensor(tensor) for name, tensor in feed_dict.items() if name in input_metadata
+            name: trt_utils.cast_tensor(tensor, dtype=input_metadata[name].dtype)
+            for name, tensor in feed_dict.items()
+            if name in input_metadata
         }
 
-        copy_outputs_to_host = utils.default(copy_outputs_to_host, True)
-
         if trt_utils._should_use_v3_api():
-            output_buffers = self._infer_impl_v3(feed_dict, copy_outputs_to_host)
+            output_buffers = self._infer_impl_v3(feed_dict)
         else:
-            output_buffers = self._infer_impl_legacy(feed_dict, copy_outputs_to_host)
+            output_buffers = self._infer_impl_legacy(feed_dict, True)
         out_dict = {k: v for k, v in output_buffers.items() if k in self.output_metadata}
 
         return out_dict
 
     def deactivate_impl(self):
         """Implementation for deactivating the runner.
```

## model_navigator/runners/torch.py

```diff
@@ -11,19 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Torch runners."""
 from collections import OrderedDict
 from typing import List, Mapping
 
-from model_navigator.api.config import Format
+from model_navigator.api.config import Format, TensorType
+from model_navigator.core.tensor import get_tensor_type
+from model_navigator.frameworks import is_torch2_available
 from model_navigator.frameworks.tensorrt import utils as tensorrt_utils
 from model_navigator.runners.base import DeviceKind, NavigatorRunner
 from model_navigator.runners.registry import register_runner
 from model_navigator.utils import module
+from model_navigator.utils.common import numpy_to_torch_dtype
 from model_navigator.utils.dataloader import get_default_output_names
 
 torch = module.lazy_import("torch")
 
 
 class _BaseTorchRunner(NavigatorRunner):
     """Base runner for inference using PyTorch."""
@@ -32,57 +35,107 @@
 
     @classmethod
     def format(cls) -> Format:
         """Runner supported format."""
         return Format.TORCH
 
     def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
         """Initialization implementation."""
+        super().__init__(*args, **kwargs)
         self._loaded_model = None
+        if is_torch2_available():
+            self._infer = self._infer_inference_mode
+        else:
+            self._infer = self._infer_no_grad
 
     def activate_impl(self):
         """Activation implementation."""
         self._loaded_model = self.model
         self._loaded_model.to(self._target_device).eval()
 
     def deactivate_impl(self):
         """Deactivation implementation."""
         self._loaded_model = None
 
     def infer_impl(self, feed_dict):
         """Inference handler implementation."""
-        with torch.no_grad():
-            inputs = [
-                torch.from_numpy(self._cast_value(feed_dict[input_name], spec.dtype)).to(self._target_device)
-                for (input_name, spec) in self.input_metadata.items()
-            ]
-            if self.input_metadata_mapping is None:
-                outputs = self._loaded_model(*inputs)
-            else:
-                inputs_dict = dict(zip(self.input_metadata_mapping, inputs))
-                outputs = self._loaded_model(**inputs_dict)
+        outputs = self._infer(feed_dict=feed_dict)
 
         if torch.is_tensor(outputs):
             outputs = (outputs,)
         if isinstance(outputs, Mapping):
             outputs = outputs.values()
 
         out_dict = OrderedDict()
         if self.output_metadata:
             output_names = self.output_metadata.keys()
         else:
             output_names = outputs.keys() if isinstance(outputs, Mapping) else get_default_output_names(len(outputs))
+
         for name, output in zip(output_names, outputs):
-            out_dict[name] = output.cpu().numpy()
+            out_dict[name] = output
+        out_dict = self._prepare_outputs(out_dict)
+
         return out_dict
 
-    def _cast_value(self, value, dtype):
-        value = value.astype(dtype)
-        return value
+    def get_available_input_types(self) -> List[TensorType]:
+        return [TensorType.NUMPY, TensorType.TORCH]
+
+    def get_available_return_types_impl(self) -> List[TensorType]:
+        return [TensorType.NUMPY, TensorType.TORCH]
+
+    def _infer_inference_mode(self, feed_dict):
+        with torch.inference_mode():
+            inputs = self._prepare_inputs(feed_dict)
+            if self.input_metadata_mapping is None:
+                outputs = self._loaded_model(*inputs)
+            else:
+                inputs_dict = dict(zip(self.input_metadata_mapping, inputs))
+                outputs = self._loaded_model(**inputs_dict)
+
+        return outputs
+
+    def _infer_no_grad(self, feed_dict):
+        with torch.no_grad():
+            inputs = self._prepare_inputs(feed_dict)
+            if self.input_metadata_mapping is None:
+                outputs = self._loaded_model(*inputs)
+            else:
+                inputs_dict = dict(zip(self.input_metadata_mapping, inputs))
+                outputs = self._loaded_model(**inputs_dict)
+
+        return outputs
+
+    def _prepare_inputs(self, feed_dict):
+        """Prepare inputs for inference."""
+        inputs = []
+        for input_name, spec in self.input_metadata.items():
+            value = feed_dict[input_name]
+            value = self._to_torch_tensor(value, spec.dtype)
+            inputs.append(value)
+        return inputs
+
+    def _prepare_outputs(self, out_dict):
+        """Prepare outputs for inference."""
+        for name, outputs in out_dict.items():
+            if self.return_type == TensorType.NUMPY:
+                out_dict[name] = outputs.cpu().numpy()
+        return out_dict
+
+    @classmethod
+    def _to_torch_tensor(cls, value, dtype):
+        tensor_type = get_tensor_type(value)
+        if tensor_type == TensorType.TORCH:
+            value = value.to(numpy_to_torch_dtype(dtype))
+        elif tensor_type == TensorType.NUMPY:
+            value = value.astype(dtype)
+            value = torch.from_numpy(value)
+        else:
+            raise ValueError(f"Unsupported type {type(value)}")
+        return value.to(cls._target_device)
 
 
 class _BaseTorchScriptRunner(_BaseTorchRunner):
     """Base runner for inference of TorchScript models."""
 
     @classmethod
     def format(cls) -> Format:
@@ -184,16 +237,17 @@
         """Runner name."""
         return "TorchTensorRT"
 
     def init_impl(self):
         """Initialization implementation."""
         import torch_tensorrt  # pytype: disable=import-error # noqa: F401
 
-    def _cast_value(self, value, dtype):
-        value = value.astype(dtype)
+    @classmethod
+    def _to_torch_tensor(cls, value, dtype):
+        value = super()._to_torch_tensor(value, dtype)
         value = tensorrt_utils.cast_tensor(value)
         return value
 
 
 def register_torch_runners():
     """Register runners in global registry."""
     register_runner(TorchCUDARunner)
@@ -204,14 +258,22 @@
 
 
 class TorchCompileCUDARunner(_BaseTorchRunner):
     """Torch Compile model CUDA based runner."""
 
     _target_device = "cuda"
 
+    def __init__(self, *args, **kwargs) -> None:
+        """Initialization implementation."""
+        # FIXME:
+        #  Remove this constructor once inference_mode is fixed for TorchCompile.
+        #  Related closed issue: https://github.com/pytorch/pytorch/issues/101151
+        super().__init__(*args, **kwargs)
+        self._infer = self._infer_no_grad
+
     @classmethod
     def name(cls) -> str:
         """Runner name."""
         return "TorchCompileCUDA"
 
     @classmethod
     def devices_kind(cls) -> List[DeviceKind]:
```

## model_navigator/runners/utils.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Helper function for runners."""
 from typing import List, Type
 
 from model_navigator.api.config import Format
-from model_navigator.logger import LOGGER
+from model_navigator.core.logger import LOGGER
 from model_navigator.runners.base import DeviceKind, NavigatorRunner
 from model_navigator.runners.registry import runner_registry
 from model_navigator.utils.devices import is_cuda_available
 from model_navigator.utils.format_helpers import is_source_format
 
 
 def default_runners(device_kind: DeviceKind) -> List:
```

## model_navigator/runtime_analyzer/analyzer.py

```diff
@@ -14,17 +14,17 @@
 """RuntimeAnalyzer class module."""
 import dataclasses
 from math import inf
 from typing import Dict, Optional, Sequence
 
 from model_navigator.commands.correctness.correctness import Correctness
 from model_navigator.commands.performance.performance import Performance
-from model_navigator.core.status import CommandStatus, ModelStatus, RunnerStatus
+from model_navigator.core.logger import LOGGER
 from model_navigator.exceptions import ModelNavigatorRuntimeAnalyzerError, ModelNavigatorUserInputError
-from model_navigator.logger import LOGGER
+from model_navigator.package.status import CommandStatus, ModelStatus, RunnerStatus
 from model_navigator.runtime_analyzer.strategy import (
     MaxThroughputAndMinLatencyStrategy,
     MaxThroughputStrategy,
     MaxThroughputWithLatencyBudgetStrategy,
     MinLatencyStrategy,
     RuntimeSearchStrategy,
     SelectedRuntimeStrategy,
```

## model_navigator/triton/model_repository.py

```diff
@@ -23,26 +23,25 @@
             backend=Backend.ONNX
         )
     )
 """
 import logging
 import pathlib
 import shutil
-from pathlib import Path
 from typing import List, Optional, Union
 
 from model_navigator.api.config import Format
 from model_navigator.commands.performance import Performance
-from model_navigator.core.package import Package
 from model_navigator.exceptions import (
     ModelNavigatorEmptyPackageError,
     ModelNavigatorError,
     ModelNavigatorWrongParameterError,
 )
 from model_navigator.frameworks import is_tf_available, is_torch_available  # noqa: F401
+from model_navigator.package.package import Package
 from model_navigator.runners.onnx import OnnxrtCPURunner, OnnxrtCUDARunner, OnnxrtTensorRTRunner
 from model_navigator.runners.tensorflow import (
     TensorFlowSavedModelCPURunner,
     TensorFlowSavedModelCUDARunner,
     TensorFlowTensorRTRunner,
 )
 from model_navigator.runners.tensorrt import TensorRTRunner
@@ -114,14 +113,15 @@
         TensorFlowModelConfig,
     ],
     model_version: int = 1,
 ) -> pathlib.Path:
     """Generate model deployment inside provided model store path.
 
     The config requires specialized configuration to be passed for backend on which model is executed. Example:
+
     - ONNX model requires ONNXModelConfig
     - TensorRT model requires TensorRTModelConfig
     - TorchScript or Torch-TensorRT models requires PyTorchModelConfig
     - TensorFlow SavedModel or TensorFlow-TensorRT models requires TensorFlowModelConfig
     - Python model requires PythonModelConfig
 
     Args:
@@ -213,15 +213,15 @@
         models_status=package.status.models_status,
         strategy=strategy,
         formats=[fmt.value for fmt in TRITON_FORMATS],
         runners=[runner.name() for runner in TRITON_RUNNERS],
     )
     max_batch_size = max(
         profiling_results.batch_size
-        for profiling_results in runtime_result.runner_status.result[Performance.name()]["profiling_results"]
+        for profiling_results in runtime_result.runner_status.result[Performance.name]["profiling_results"]
     )
 
     if runtime_result.model_status.model_config.format == Format.ONNX:
         config = _onnx_config_from_runtime_result(
             batching=batching,
             max_batch_size=max_batch_size,
             response_cache=response_cache,
@@ -264,15 +264,15 @@
             f"Unsupported model format selected: {runtime_result.model_status.model_config.format}"
         )
 
     return add_model(
         model_repository_path=model_repository_path,
         model_name=model_name,
         model_version=model_version,
-        model_path=package.workspace / runtime_result.model_status.model_config.path,
+        model_path=package.workspace.path / runtime_result.model_status.model_config.path,
         config=config,
     )
 
 
 class _TritonModelRepository:
     """Class for deploying models inside the Triton Model Store."""
 
@@ -320,15 +320,15 @@
     def _copy_model(
         self,
         *,
         model_path: pathlib.Path,
         backend: Backend,
         model_name: str,
         version: int,
-    ) -> Path:
+    ) -> pathlib.Path:
         dst_path = self._get_model_path(
             model_name=model_name,
             version=version,
             backend=backend,
         )
         dst_path.parent.mkdir(exist_ok=True, parents=True)
         LOGGER.debug(f"Copying {model_path} to {dst_path}")
@@ -346,15 +346,15 @@
 
     def _get_model_path(
         self,
         *,
         model_name: str,
         version: int,
         backend: Backend,
-    ) -> Path:
+    ) -> pathlib.Path:
         return self._model_repository_path / model_name / str(version) / self._get_filename(backend=backend)
 
     def _get_filename(self, *, backend: Backend):
         suffix = BACKEND2SUFFIX[backend]
         return f"model{suffix}"
```

## model_navigator/utils/common.py

```diff
@@ -14,25 +14,23 @@
 """Common utils."""
 
 import dataclasses
 import glob
 import os
 import pathlib
 from enum import Enum
-from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Type, TypeVar, Union
 
-import dacite
 import numpy
 from polygraphy.backend.trt.profile import Profile, ShapeTuple
 
-from model_navigator.logger import LOGGER
+from model_navigator.core.logger import LOGGER
+from model_navigator.utils import module
 
-if TYPE_CHECKING:
-    import torch  # pytype: disable=import-error
+torch = module.lazy_import("torch")
 
 T = TypeVar("T")
 
 
 def dataclass2dict(config: Any) -> Dict:
     """Parse a dataclass to a dictionary.
 
@@ -48,15 +46,15 @@
         result = []
         for key_, value_ in fields_:
             if isinstance(key_, Enum):
                 key_ = key_.value
 
             if isinstance(value_, Enum):
                 value_ = value_.value
-            elif isinstance(value_, Path):
+            elif isinstance(value_, pathlib.Path):
                 value_ = value_.as_posix()
             elif isinstance(value_, numpy.dtype):
                 value_ = str(value_)
             elif isinstance(value_, (tuple, list)):
                 value_ = [v.value if isinstance(v, Enum) else v for v in value_]
             elif isinstance(value_, dict):
                 value_ = _dict_factory_with_enum_values_extraction(value_.items())
@@ -66,30 +64,14 @@
     init_fields_names = [field.name for field in dataclasses.fields(config) if field.init]
 
     new_config_dict = dataclasses.asdict(config, dict_factory=_dict_factory_with_enum_values_extraction)
     config_dict_with_only_init_items = {k: v for k, v in new_config_dict.items() if k in init_fields_names}
     return config_dict_with_only_init_items
 
 
-def dict2dataclass(cls: Type[T], data: Dict) -> T:
-    """Parse a dictionary to a dataclass.
-
-    Args:
-        cls (Type[T]): Type of the dataclass.
-        data (Dict): Dictionary with the dataclass data.
-
-    Returns:
-        T: Dataclass.
-    """
-    dataclass = dacite.from_dict(cls, data, config=dacite.Config(cast=[Enum, Path, tuple, numpy.dtype]))
-    assert isinstance(dataclass, cls)
-    assert dataclasses.is_dataclass(dataclass)
-    return dataclass
-
-
 class DataObject:
     """Class for storing data about configurations, statuses, etc."""
 
     def to_dict(self, filter_fields: Optional[List[str]] = None, parse: bool = False) -> Dict:
         """Serialize to a dictionary.
 
         Args:
@@ -100,27 +82,59 @@
 
         Returns:
             Dict: Data serialized to a dictionary.
         """
         data = {}
 
         if filter_fields:
-            filtered_data = {key: value for key, value in self.__dict__.items() if key not in filter_fields}
+            filtered_data = DataObject.filter_data(
+                data=self.__dict__,
+                filter_fields=filter_fields,
+            )
         else:
             filtered_data = self.__dict__
 
         if parse:
-            for key, value in filtered_data.items():
-                data[key] = self.parse_value(value)
+            data = DataObject.parse_data(filtered_data)
         else:
             data = filtered_data
 
         return data
 
     @staticmethod
+    def filter_data(data: Dict, filter_fields: List[str]):
+        """Filter fields in dictionary.
+
+        Args:
+            data: Dictionary with data to filter
+            filter_fields: Fields to filter
+
+        Returns:
+            Filtered dictionary
+        """
+        filtered_data = {key: value for key, value in data.items() if key not in filter_fields}
+        return filtered_data
+
+    @staticmethod
+    def parse_data(data: Dict):
+        """Parse values in provided data.
+
+        Args:
+            data: Dictionary with data to parse
+
+        Returns:
+            Parsed dictionary
+        """
+        parsed_data = {}
+        for key, value in data.items():
+            parsed_data[key] = DataObject.parse_value(value)
+
+        return parsed_data
+
+    @staticmethod
     def parse_value(value: Any) -> Union[str, Dict, List]:
         """Parse value to jsonable format.
 
         Args:
             value (Any): Value to be parsed.
 
         Returns:
@@ -136,14 +150,15 @@
             value = DataObject._from_list(value)
         elif isinstance(value, Enum):
             value = value.value
         elif isinstance(value, pathlib.Path):
             value = str(value)
         elif isinstance(value, ShapeTuple):
             value = vars(value)
+
         return value
 
     @staticmethod
     def _from_dict(values: Dict) -> Dict:
         data = {}
         for key, value in values.items():
             data[key] = DataObject.parse_value(value)
@@ -173,71 +188,65 @@
     if value is not None:
         value = tuple(value) if isinstance(value, (tuple, list)) else (value,)
         value = tuple(enum_type(v) for v in value)
         return value
     return ()
 
 
-def numpy_to_torch_dtype(np_dtype: numpy.dtype) -> "torch.dtype":
-    """Cast numpy dtype to torch dtype.
-
-    Args:
-        np_dtype (numpy.dtype): numpy dtype.
-
-    Returns:
-        torch.dtype: torch dtype.
-    """
-    np_dtype = numpy.dtype(np_dtype).type
-    import torch  # pytype: disable=import-error
-
+def _get_numpy_to_torch_dtype_dict():
     return {
         numpy.bool_: torch.bool,
         numpy.uint8: torch.uint8,
         numpy.int8: torch.int8,
         numpy.int16: torch.int16,
         numpy.int32: torch.int32,
         numpy.int64: torch.int64,
         numpy.float16: torch.float16,
         numpy.float32: torch.float32,
         numpy.float64: torch.float64,
         numpy.complex64: torch.complex64,
         numpy.complex128: torch.complex128,
-    }[np_dtype]
+    }
 
 
-def get_default_status_filename() -> str:
-    """Get default status filename.
+def numpy_to_torch_dtype(np_dtype: numpy.dtype) -> "torch.dtype":
+    """Cast numpy dtype to torch dtype.
+
+    Args:
+        np_dtype (numpy.dtype): numpy dtype.
 
     Returns:
-        str: Filename.
+        torch.dtype: torch dtype.
     """
-    return "status.yaml"
+    np_dtype = numpy.dtype(np_dtype).type
+    numpy_to_torch_dtype_dict = _get_numpy_to_torch_dtype_dict()
+    return numpy_to_torch_dtype_dict[np_dtype]
+
 
+def torch_to_numpy_dtype(torch_dtype: "torch.dtype") -> numpy.dtype:
+    """Cast torch dtype to numpy dtype.
 
-def get_default_workspace() -> Path:
-    """Get default workspace path.
+    Args:
+        np_dtype (torch.dtype): torch dtype.
 
     Returns:
-        Path: Worskspace path.
+        numpy.dtype: numpy dtype.
     """
-    return Path.cwd() / "navigator_workspace"
+    numpy_to_torch_dtype_dict = _get_numpy_to_torch_dtype_dict()
+    torch_to_numpy_dtype_dict = {v: k for k, v in numpy_to_torch_dtype_dict.items()}
+    return torch_to_numpy_dtype_dict[torch_dtype]
 
 
-def pad_string(s: str) -> str:
-    """Pad string with `=` signs.
-
-    Args:
-        s (str): String.
+def get_default_status_filename() -> str:
+    """Get default status filename.
 
     Returns:
-        str: Padded string.
+        str: Filename.
     """
-    s = f"{30 * '='} {s} "
-    s = s.ljust(100, "=")
-    return s
+    return "status.yaml"
 
 
 def parse_kwargs_to_cmd(kwargs: Dict[str, Any]) -> List[str]:
     """Parse kwargs so that they can be passed as a commandline arguments.
 
     Args:
         kwargs (Dict[str, Any]): keyword arguments to be parsed to commandline.
@@ -352,15 +361,17 @@
         obj.write  # pytype: disable=attribute-error
     except AttributeError:
         return False
     else:
         return True
 
 
-def load_file(src: Union[str, Path], mode: str = "rb", description: Optional[str] = None) -> Union[str, bytes, None]:
+def load_file(
+    src: Union[str, pathlib.Path], mode: str = "rb", description: Optional[str] = None
+) -> Union[str, bytes, None]:
     """Reads from the specified source path or file-like object.
 
     Args:
         src: The path or file-like object to read from.
 
 
         mode: The mode to use when reading. Defaults to "rb".
```

## model_navigator/utils/dataloader.py

```diff
@@ -9,20 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Dataloader definition and helpers module."""
 import pathlib
-from pathlib import Path
 from typing import Any, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
-from model_navigator.api.config import Sample
+from model_navigator.api.config import Sample, TensorType
 from model_navigator.exceptions import ModelNavigatorUserInputError
 from model_navigator.frameworks import Framework
 
 
 def to_numpy(tensor: Any, from_framework: Framework) -> np.ndarray:
     """Convert tensor to numpy array.
 
@@ -84,110 +83,112 @@
         A formatted sample data
     """
     if batch_dim is not None:
         return {name: tensor.take([0], batch_dim) for name, tensor in sample.items()}
     return sample
 
 
-def is_tensor(tensor: Any, framework: Framework) -> bool:
+def is_tensor(tensor: Any, tensor_type: TensorType) -> bool:
     """Validate if provided object is a valid tensor.
 
     Args:
         tensor: An object to validate
         framework: A framework for which the object has to be tested
 
     Returns:
         True if object is a valid tensor, False otherwise
     """
-    if framework == Framework.TORCH:
+    if tensor_type == TensorType.TORCH:
         import torch  # pytype: disable=import-error
 
         return torch.is_tensor(tensor) or isinstance(tensor, np.ndarray)
-    elif framework == Framework.TENSORFLOW:
+    elif tensor_type == TensorType.TENSORFLOW:
         import tensorflow  # pytype: disable=import-error
 
         return tensorflow.is_tensor(tensor) or isinstance(tensor, np.ndarray)
     else:
         return isinstance(tensor, np.ndarray)
 
 
-def get_tensor_type_name(framework: Optional[Framework] = None) -> str:
+def get_tensor_type_name(tensor_type: TensorType) -> str:
     """Obtain name of tensor type for given framework.
 
     Args:
         framework: A framework for which tensor type name has to be obtained
 
     Returns:
         Name of tensor type in form o string
     """
-    if framework == Framework.TORCH:
+    if tensor_type == TensorType.TORCH:
         return "Union[torch.Tensor, numpy.ndarray]"
-    elif framework == Framework.TENSORFLOW:
+    elif tensor_type == TensorType.TENSORFLOW:
         return "Union[tensorflow.Tensor, numpy.ndarray]"
-    else:
+    elif tensor_type == TensorType.NUMPY:
         return "numpy.ndarray"
+    else:
+        raise ValueError(f"Unknown tensor type {tensor_type}")
 
 
-def _is_valid_io(sample: Any, framework: Framework) -> bool:
+def _is_valid_io(sample: Any, tensor_type: TensorType) -> bool:
     """Validate if provided sample is correct I/O object.
 
     Args:
         sample: A sample to validate
         framework: A framework for which the validation is performed
 
     Returns:
         True if sample is valid I/O, False otherwise
     """
-    if is_tensor(sample, framework):
+    if is_tensor(sample, tensor_type):
         return True
     if isinstance(sample, Mapping):
         for tensor in sample.values():
-            if not is_tensor(tensor, framework):
+            if not is_tensor(tensor, tensor_type):
                 return False
         return True
     elif isinstance(sample, Iterable):
         for tensor in sample:
-            if not is_tensor(tensor, framework):
+            if not is_tensor(tensor, tensor_type):
                 return False
         return True
     return False
 
 
-def validate_sample_input(sample: Any, framework: Optional[Framework] = None) -> None:
+def validate_sample_input(sample: Any, tensor_type: TensorType = TensorType.NUMPY) -> None:
     """Validate if sample input is correct input object.
 
     Args:
         sample: A sample to validate
         framework: A framework for which the validation is performed
 
     Raises:
         ModelNavigatorUserInputError when provided sample if not a valid input object
 
     """
-    if not _is_valid_io(sample, framework):
-        tensor_type = get_tensor_type_name(framework)
+    if not _is_valid_io(sample, tensor_type):
+        tensor_type = get_tensor_type_name(tensor_type)
         raise ModelNavigatorUserInputError(
             f"Invalid sample type. Sample must be of type Union[{tensor_type}, "
             f"Iterable[{tensor_type}], Mapping[str, {tensor_type}]]. Dataloader returned {sample}."
         )
 
 
-def validate_sample_output(sample, framework: Optional[Framework] = None):
+def validate_sample_output(sample, tensor_type: TensorType = TensorType.NUMPY):
     """Validate if sample output is correct output object.
 
     Args:
         sample: A sample to validate
         framework: A framework for which the validation is performed
 
     Raises:
         ModelNavigatorUserInputError when provided sample if not a valid output object
 
     """
-    if not _is_valid_io(sample, framework):
-        tensor_type = get_tensor_type_name(framework)
+    if not _is_valid_io(sample, tensor_type):
+        tensor_type = get_tensor_type_name(tensor_type)
         raise ModelNavigatorUserInputError(
             f"Invalid model output type. Output must be of type Union[{tensor_type}, "
             f"Iterable[{tensor_type}]], Mapping[str, {tensor_type}]]. Model returned {sample}."
         )
 
 
 def load_samples(samples_name: str, workspace: Union[pathlib.Path, str], batch_dim: Optional[int]) -> List[Sample]:
@@ -198,15 +199,15 @@
         workspace: Working directory
         batch_dim: Position of batch dimension
 
     Returns:
         List of data samples
     """
     if isinstance(workspace, str):
-        workspace = Path(workspace)
+        workspace = pathlib.Path(workspace)
     samples_type = samples_name.split("_")[0]
     samples_dirname = "model_output" if samples_name.split("_")[-1] == "output" else "model_input"
     samples_dirpath = workspace / samples_dirname / samples_type
     samples = []
     for sample_filepath in sorted(samples_dirpath.iterdir()):
         sample = {}
         with np.load(sample_filepath.as_posix()) as data:
```

## model_navigator/utils/format_helpers.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Helpers functions for formats."""
 
 from typing import Optional, Set
 
-from model_navigator.api.config import Format
+from model_navigator.api.config import AVAILABLE_TARGET_FORMATS, DEFAULT_TARGET_FORMATS, Format
 from model_navigator.frameworks import Framework
 
 
 def is_source_format(format: Format) -> bool:
     """Validate if provided format is a Python model.
 
     Args:
@@ -32,14 +32,32 @@
         Format.JAX,
         Format.TENSORFLOW,
         Format.TORCH,
         Format.PYTHON,
     )
 
 
+def get_target_formats(framework: Framework, is_source_available: bool):
+    """Obtain available target formats for framework.
+
+    Args:
+        framework: Framework for which target format has to be prepared
+        is_source_available: Flag indicating if source is available
+
+    Returns:
+        List of target formats
+    """
+    if is_source_available:
+        target_formats = AVAILABLE_TARGET_FORMATS[framework]
+    else:
+        target_formats = DEFAULT_TARGET_FORMATS[framework]
+
+    return target_formats
+
+
 def get_framework_export_formats(framework: Framework) -> Set[Optional[Format]]:
     """Get the base export formats for framework.
 
     The base export format is the one which can be generated directly from the Python sources.
     Python based models cannot be serialized to any format.
 
     Args:
```

## model_navigator/utils/module.py

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Module related utilities."""
 import importlib
 from types import ModuleType
 from typing import Any, Optional
 
-from model_navigator.logger import LOGGER
+from model_navigator.core.logger import LOGGER
 
 MODULE_VAR_NAME = "module"
 
 
 def lazy_import(name: str):
     """Lazy load module with given name.
```

## Comparing `model_navigator/execution_context.py` & `model_navigator/commands/execution_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 import logging
 import os
 import pathlib
 import shutil
 import subprocess
 import sys
 import textwrap
-from pathlib import Path
 from typing import Callable, List, Optional, Union
 
 import fire
 
+from model_navigator.core.logger import LOGGER
+from model_navigator.core.workspace import Workspace
 from model_navigator.exceptions import ModelNavigatorUserInputError
-from model_navigator.logger import LOGGER
 
 
 class FileHandlersLogging:
     """Disable everything that is not a FileHandler.
 
     Example usage:
         with FileHandlersLogging():
@@ -83,34 +83,33 @@
     """
 
     accepted_types = (int, float, bool, str)
 
     def __init__(
         self,
         *,
-        workspace: Path,
-        script_path: Optional[Path] = None,
-        cmd_path: Optional[Path] = None,
+        workspace: Workspace,
+        script_path: Optional[pathlib.Path] = None,
+        cmd_path: Optional[pathlib.Path] = None,
         verbose: bool = False,
         on_exit: Optional[Callable] = None,
     ):
         """Initialize the context.
 
         Args:
             workspace: directory where scripts are created and executed
             script_path: path to Python script for reproduction
             cmd_path: path to Bash script for reproduction
             verbose: enable verbose logging
             on_exit: Perform operation despite success or error
         """
         super().__init__()
         self._workspace = workspace
-        self._script_path = Path(script_path) if script_path else script_path
-        self._script_path = Path(script_path) if script_path else script_path
-        self._cmd_path = Path(cmd_path) if cmd_path else cmd_path
+        self._script_path = pathlib.Path(script_path) if script_path else script_path
+        self._cmd_path = pathlib.Path(cmd_path) if cmd_path else cmd_path
         self._cache = {}
         self._output = None
         self._verbose = verbose
         self._on_exit = on_exit
 
     def __exit__(self, exc_type, exc_value, traceback):  # noqa: F841
         """Exit the context and store the command output to file.
@@ -156,15 +155,15 @@
             allow_failure: if True, do not raise exception when script execution failed
 
 
         Raises:
             ModelNavigatorUserInputError when command execution failed
         """
         shutil.copy(path, self._script_path)
-        script_path_relative = self._script_path.relative_to(self._workspace)
+        script_path_relative = self._script_path.relative_to(self._workspace.path)
 
         filtered_args = self._filter_workspace_args(args)
         cmd = self._bake_command([sys.executable, script_path_relative.as_posix()] + filtered_args)
         try:
             unwrapped_args = self._unwrap_args(args)
             fire.Fire(func, unwrapped_args)
         except Exception as e:
@@ -178,15 +177,15 @@
 
         Args:
             path: Path to script that has to be executed
             args: Additional arguments to be passed to script during execution
             allow_failure: if True, do not raise exception when command execution failed
         """
         shutil.copy(path, self._script_path)
-        script_path_relative = self._script_path.relative_to(self._workspace)
+        script_path_relative = self._script_path.relative_to(self._workspace.path)
 
         filtered_args = self._filter_workspace_args(args)
         cmd = [sys.executable, script_path_relative.as_posix()] + filtered_args
         self.execute_cmd(cmd, allow_failure=allow_failure)
 
     def execute_cmd(self, cmd: List, dry_run=False, allow_failure: bool = False):
         """Execute command as subprocess.
@@ -205,15 +204,15 @@
             return run_cmd
 
         process = subprocess.Popen(
             run_cmd,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             encoding="utf-8",
-            cwd=self._workspace,
+            cwd=self._workspace.path,
         )
 
         if self._verbose:
             LOGGER.info("Command output:")
 
         self._output = ""
         while True:
@@ -242,15 +241,15 @@
 
         if self._cmd_path is None:
             raise ValueError("cmd_path is required when using `execute_cmd` method.")
 
         with self._cmd_path.open("w") as f:
             f.write(" ".join(cmd))
 
-        cmd_path_relative = self._cmd_path.relative_to(self._workspace)
+        cmd_path_relative = self._cmd_path.relative_to(self._workspace.path)
         run_cmd = [os.environ.get("SHELL", "bash"), cmd_path_relative.as_posix()]
 
         return run_cmd
 
     def _filter_workspace_args(self, args: List) -> List:
         filtered_args = copy.deepcopy(args)
         try:
```

## Comparing `model_navigator/logger.py` & `model_navigator/core/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Logger module."""
 import contextlib
+import json
 import logging
-from pathlib import Path
-from typing import Optional
+import pathlib
+from typing import Dict, Optional
 
 import coloredlogs
 
 from model_navigator.core.constants import NAVIGATOR_LOG_NAME, NAVIGATOR_LOGGER_NAME
 
 LOGGER = logging.getLogger(NAVIGATOR_LOGGER_NAME)
 LOGGER.propagate = False
@@ -66,48 +67,27 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Exit the context manager."""
         self._redirect_stdout.__exit__(exc_type, exc_value, traceback)
 
 
-def add_log_file_handler(log_dir: Path) -> None:
-    """Add log file handler to file in defined path.
-
-    Args:
-        log_dir: A path to log directory
-    """
-    log_file = log_dir / NAVIGATOR_LOG_NAME
-    fh = logging.FileHandler(log_file)
-    fh.setLevel(logging.DEBUG)
-    LOGGER.addHandler(fh)
-
-
-def get_logger_names() -> list:
-    """Collect logger names as list.
-
-    Returns:
-        List with names of the loggers
-    """
-    return list(logging.root.manager.loggerDict.keys())
-
-
 class LoggingContext(contextlib.AbstractContextManager):
     """LoggingContext to handle correct logging options when commands are executed.
 
     Example of use:
         log_dir = pathlib.Path("/path/to/log/directory")
         with LoggingContext(log_dir=log_dir):
             LOGGER.info("Log inside the context")
     """
 
     def __init__(
         self,
         *,
-        log_dir: Optional[Path] = None,
+        log_dir: Optional[pathlib.Path] = None,
     ):
         """Initialize the context.
 
         Args:
             log_dir: Optional path to directory where log file is stored.
         """
         super().__init__()
@@ -141,7 +121,53 @@
         if self.log_dir:
             for logger in self.loggers:
                 if isinstance(logger, str):
                     logger = logging.getLogger(logger)
                 logger.handlers = [h for h in logger.handlers if h != self.log_file_handler]
             LOGGER.removeHandler(self.log_file_handler)
             self.log_file_handler = None
+
+
+def add_log_file_handler(log_dir: pathlib.Path) -> None:
+    """Add log file handler to file in defined path.
+
+    Args:
+        log_dir: A path to log directory
+    """
+    log_file = log_dir / NAVIGATOR_LOG_NAME
+    fh = logging.FileHandler(log_file)
+    fh.setLevel(logging.DEBUG)
+    LOGGER.addHandler(fh)
+
+
+def get_logger_names() -> list:
+    """Collect logger names as list.
+
+    Returns:
+        List with names of the loggers
+    """
+    return list(logging.root.manager.loggerDict.keys())
+
+
+def log_dict(title: str, data: Dict):
+    """Log dictionary data with provided tittle.
+
+    Args:
+        title: The title for logged information
+        data: The dictionary with content to log
+
+    """
+    LOGGER.info(pad_string(title))
+    LOGGER.info(json.dumps(data, indent=4))
+
+
+def pad_string(s: str) -> str:
+    """Pad string with `=` signs.
+
+    Args:
+        s (str): String.
+
+    Returns:
+        str: Padded string.
+    """
+    s = f" {s} "
+    return s.center(118, "=")
```

## Comparing `model_navigator/commands/performance/performance_script.py` & `model_navigator/commands/performance/profile_script.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """Script for running profiling on a runner."""
 
 import pathlib
 from typing import Dict, List, Optional
 
 import fire
 
-from model_navigator.api.config import ProfilerConfig
-from model_navigator.commands.performance import Profiler
+from model_navigator.api.config import OptimizationProfile
+from model_navigator.commands.performance.profiler import Profiler
 from model_navigator.core.tensor import TensorMetadata
 from model_navigator.runners.registry import get_runner
 from model_navigator.utils.dataloader import load_samples
 
 
 def get_model() -> object:
     """Get model instance.
@@ -36,56 +36,59 @@
     )
 
 
 def profile(
     batch_dim: int,
     results_path: str,
     runner_name: str,
-    profiler_config: Dict,
+    optimization_profile: Dict,
     input_metadata: List,
     output_metadata: List,
+    sample_id: int = 0,
     navigator_workspace: Optional[str] = None,
     model_path: Optional[str] = None,
 ) -> None:
     """Run profiling.
 
     Args:
-        batch_dim (int): Batch dimension.
-        results_path (str): Path to store the profiling results in.
-        runner_name (str): Name of the runner to profile.
-        profiler_config (Dict): Profiler configuration.
-        input_metadata (List): Input metadata.
-        output_metadata (List): Output metadata.
-        navigator_workspace (Optional[str], optional): Path of the Model Navigator workspace.
+        batch_dim: Batch dimension.
+        results_path: Path to store the profiling results in.
+        runner_name: Name of the runner to profile.
+        optimization_profile: Optimization profile used for configuration.
+        input_metadata: Input metadata.
+        output_metadata: Output metadata.
+        sample_id: Identifier of profiled sample.
+        navigator_workspace: Path of the Model Navigator workspace.
             When None use current workdir. Defaults to None.
-        model_path (Optional[str], optional): Path to the model.
+        model_path: Path to the model.
             When None use `get_model()` to load the model. Defaults to None.
     """
     if not navigator_workspace:
         navigator_workspace = pathlib.Path.cwd()
     navigator_workspace = pathlib.Path(navigator_workspace)
 
-    profiling_sample = load_samples("profiling_sample", navigator_workspace, batch_dim)[0]
+    profiling_sample = load_samples("profiler_sample", navigator_workspace, batch_dim)[0]
 
     if model_path:
         model = navigator_workspace / model_path
     else:
         model = get_model()
 
     runner = get_runner(runner_name)(
         model=model,
         input_metadata=TensorMetadata.from_json(input_metadata),
         output_metadata=TensorMetadata.from_json(output_metadata),
     )  # pytype: disable=not-instantiable
 
     Profiler(
-        config=ProfilerConfig.from_dict(profiler_config),
+        profile=OptimizationProfile.from_dict(optimization_profile),
         batch_dim=batch_dim,
         results_path=pathlib.Path(results_path),
     ).run(
         runner=runner,
         profiling_sample=profiling_sample,
+        sample_id=sample_id,
     )
 
 
 if __name__ == "__main__":
     fire.Fire(profile)
```

## Comparing `model_navigator/core/package.py` & `model_navigator/package/status.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,491 +7,517 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""PackageDescriptor module - structure to handle execution status."""
+"""Collection of status classes.
 
-import os
-import shutil
-import zipfile
-from pathlib import Path
-from typing import Dict, List, Optional, Set, Union
+Those classes are used to store information about the Model Navigator process.
+"""
+import collections
+import dataclasses
+import datetime
+import pathlib
+from dataclasses import dataclass, field
+from typing import Dict, List, Optional, Sequence, Tuple
 
-import yaml
 from packaging import version
 
-from model_navigator.api.config import CUSTOM_CONFIGS_MAPPING, SERIALIZED_FORMATS, DeviceKind, Format, ProfilerConfig
-from model_navigator.commands.base import CommandOutput, CommandStatus, ExecutionUnit
-from model_navigator.commands.correctness.correctness import Correctness
-from model_navigator.commands.performance.performance import Performance
-from model_navigator.commands.verification.verify import VerifyModel
-from model_navigator.configuration.common_config import CommonConfig
-from model_navigator.core.status import ModelStatus, RunnerStatus, Status
-from model_navigator.exceptions import (
-    ModelNavigatorMissingSourceModelError,
-    ModelNavigatorNotFoundError,
-    ModelNavigatorRuntimeAnalyzerError,
+from model_navigator.api.config import (
+    Format,
+    OnnxConfig,
+    OptimizationProfile,
+    TensorFlowTensorRTConfig,
+    TensorRTConfig,
+    TensorRTPrecisionMode,
+    TensorRTProfile,
+    TorchTensorRTConfig,
 )
+from model_navigator.commands.base import CommandStatus
+from model_navigator.commands.correctness.correctness import Correctness, TolerancePerOutputName
+from model_navigator.commands.performance.performance import Performance, ProfilingResults
+from model_navigator.commands.verification.verify import VerifyModel
+from model_navigator.configuration.model.model_config import ModelConfig
+from model_navigator.core.constants import NAVIGATOR_PACKAGE_VERSION, NAVIGATOR_VERSION
+from model_navigator.core.logger import LOGGER
+from model_navigator.core.tensor import TensorMetadata
 from model_navigator.frameworks import Framework
-from model_navigator.logger import LOGGER
-from model_navigator.runners.base import NavigatorRunner
-from model_navigator.runners.registry import get_runner
-from model_navigator.runtime_analyzer.analyzer import RuntimeAnalyzer
-from model_navigator.runtime_analyzer.strategy import (
-    MaxThroughputAndMinLatencyStrategy,
-    MaxThroughputStrategy,
-    MinLatencyStrategy,
-    RuntimeSearchStrategy,
-)
-from model_navigator.utils import package as package_utils
-from model_navigator.utils.common import get_default_status_filename, get_default_workspace
-from model_navigator.utils.format_helpers import FORMAT2SUFFIX, get_framework_export_formats, is_source_format
+from model_navigator.frameworks.tensorrt.utils import get_trt_profile_from_trt_dynamic_axes
+from model_navigator.utils.common import DataObject
 
 
-class Package:
-    """Class for storing pipeline execution status."""
+@dataclass
+class RunnerStatus(DataObject):
+    """Runner results."""
 
-    status_filename = get_default_status_filename()
+    runner_name: str
+    status: Dict[str, CommandStatus] = field(default_factory=lambda: {})
+    result: Dict = field(default_factory=lambda: {})
 
-    def __init__(self, status: Status, workspace: Optional[Path], model: Optional[object] = None):
-        """Initialize object.
+    @classmethod
+    def from_dict(cls, data_dict: Dict) -> "RunnerStatus":
+        """Create RunnerStatus from the dictionary.
 
         Args:
-            status: A navigator execution status
-            workspace: A workspace path
-            model: An optional model
-        """
-        self.status = status
-        self.workspace = workspace
-        self._model = model
-        self._forward_kw_names = None
-
-    @property
-    def framework(self) -> Framework:
-        """Framework for which package was created.
+            data_dict (Dict): dictionary with runner results data.
 
         Returns:
-            Framework object for package
+            RunnerStatus
         """
-        return Framework(self.status.config["framework"])
+        status = {k: CommandStatus(v) for k, v in data_dict["status"].items()}
+        result = {}
 
-    @property
-    def model(self) -> object:
-        """Return source model.
+        for c, s in status.items():
+            if s != CommandStatus.OK:
+                continue
 
-        Returns:
-            Source model.
-        """
-        return self._model
+            if c == Correctness.name:
+                result[c] = {
+                    "per_output_tolerance": TolerancePerOutputName.from_json(
+                        data_dict["result"][Correctness.__name__]["per_output_tolerance"]
+                    )
+                }
+            elif c == Performance.name:
+                result[c] = {
+                    "profiling_results": [
+                        ProfilingResults.from_dict(profiling_results_dict)
+                        for profiling_results_dict in data_dict["result"][Performance.__name__]["profiling_results"]
+                    ]
+                }
+
+        return cls(
+            runner_name=data_dict["runner_name"],
+            status=status,
+            result=result,
+        )
 
-    def save_status_file(self) -> None:
-        """Save the status.yaml."""
-        self._delete_status_file()
-        self._create_status_file()
 
-    def get_model_path(self, model_key: str) -> Path:
-        """Return path of the model.
+@dataclass
+class ModelStatus(DataObject):
+    """Model Status."""
+
+    model_config: ModelConfig
+    runners_status: Dict[str, RunnerStatus] = field(default_factory=lambda: {})
+    status: Dict[str, CommandStatus] = field(default_factory=lambda: {})
+    result: Dict = field(default_factory=lambda: {})
 
-        Args:
-            model_key (str): Unique key of the model.
+    @classmethod
+    def from_dict(cls, data_dict: Dict) -> "ModelStatus":
+        """Create ModelStatus from the dictionary.
 
-        Raises:
-            ModelNavigatorNotFoundError: When model not found.
+        Args:
+            data_dict (Dict): dictionary with model status data.
 
         Returns:
-            Path: model path
-        """
-        try:
-            model_config = self.status.models_status[model_key].model_config
-        except KeyError:
-            raise ModelNavigatorNotFoundError(f"Model {model_key} not found.")
-        return self.workspace / model_config.path
-
-    def save(
-        self,
-        path: Union[str, Path],
-        keep_workspace: bool = True,
-        override: bool = False,
-        save_data: bool = True,
-    ) -> None:
-        """Save export results into the .nav package at given path.
-
-        Args:
-            path: A path to file where the package has to be saved
-            keep_workspace: flag to remove the working directory after saving the package
-            override: flag to override existing package in provided path
-            save_data: disable saving samples from the dataloader
+            ModelStatus
         """
-        path = Path(path)
-        if path.exists():
-            if override:
-                path.unlink()
-            else:
-                raise FileExistsError(path)
-
-        if not self.workspace.exists():
-            raise FileNotFoundError("Workspace has been removed. Save() no longer available.")
-
-        if self.is_empty():
-            LOGGER.warning("No successful exports, .nav package will be empty.")
-
-        models_files_to_save = self._get_models_paths_to_save(self.workspace)
-        reproduction_files_to_save = self._get_reproduction_paths_to_save(self.workspace)
-        files_to_save = (
-            [self.workspace / "status.yaml", self.workspace / "navigator.log"]
-            + models_files_to_save
-            + reproduction_files_to_save
+        return cls(
+            model_config=ModelConfig.from_dict(data_dict["model_config"]),
+            runners_status={
+                runner_name: RunnerStatus.from_dict(runner_res)
+                for runner_name, runner_res in data_dict["runners_status"].items()
+            },
+            status={k: CommandStatus(v) for k, v in data_dict.get("status", {}).items()},
+            result=data_dict.get("result", {}),
         )
-        dirs_to_save = []
-        if save_data:
-            dirs_to_save.extend([self.workspace / "model_output", self.workspace / "model_input"])
-        self._make_zip(path, self.workspace, dirs_to_save, files_to_save)
 
-        if not keep_workspace:
-            self._cleanup()
+
+@dataclass
+class Status(DataObject):
+    """Model Navigator Status."""
+
+    format_version: str
+    model_navigator_version: str
+    uuid: str
+    environment: Dict
+    config: Dict
+    models_status: Dict[str, ModelStatus]
+    input_metadata: TensorMetadata
+    output_metadata: TensorMetadata
+    dataloader_trt_profile: TensorRTProfile
+    dataloader_max_batch_size: int
+    status: Dict[str, CommandStatus] = field(default_factory=lambda: {})
+    result: Dict = field(default_factory=lambda: {})
+    timestamp: str = dataclasses.field(default_factory=lambda: f"{datetime.datetime.utcnow():%Y-%m-%dT%H:%M:%S.%f}")
 
     @classmethod
-    def load(
-        cls,
-        path: Union[str, Path],
-        workspace: Optional[Union[str, Path]] = None,
-    ) -> "Package":
-        """Load package from provided path and updates to the current version.
+    def from_dict(cls, data_dict: Dict) -> "Status":
+        """Create NavigatorStatus from the dictionary.
 
         Args:
-            path: The location of package to load
-            workspace: Workspace where packages will be extracted
+            data_dict (Dict): Dictionary with navigator status data.
 
         Returns:
-            Package.
+            NavigatorStatus
         """
 
-        def _filter_out_generated_files(paths: List[str]):
-            generated_files_extensions = [".log", ".sh", ".py"]
-            return [p for p in paths if not any(p.endswith(suffix) for suffix in generated_files_extensions)]
-
-        def _extract_pkg_version(status_dict):
-            return version.parse(status_dict.get("model_navigator_version", "0.3.0"))
-
-        path = Path(path)
-        if workspace is None:
-            workspace = get_default_workspace()
-        workspace = Path(workspace)
-
-        with zipfile.ZipFile(path, "r") as zf:
-            with zf.open(Package.status_filename) as status_file:
-                status_dict = yaml.safe_load(status_file)
-            pkg_version = _extract_pkg_version(status_dict)
-            status = Status.from_dict(status_dict)
-
-            if workspace.exists():
-                shutil.rmtree(workspace)
-
-            package = Package(status, workspace)
-            all_members = zf.namelist()
-            filtered_members = _filter_out_generated_files(all_members)
-            zf.extractall(workspace, members=filtered_members)
-
-        package_utils.PackageUpdater().update(package, pkg_version)
-        package.save_status_file()
-        return package
-
-    @property
-    def config(self) -> CommonConfig:
-        """Generate configuration from package.
-
-        Returns:
-            The configuration object
-        """
-        config_dict = {**self.status.config}
-        config_dict["framework"] = self.framework
-        config_dict["target_formats"] = self._target_formats
-        config_dict["runner_names"] = tuple(config_dict["runner_names"])
-        config_dict["profiler_config"] = ProfilerConfig.from_dict(config_dict.get("profiler_config", {}))
-        if "batch_dim" not in config_dict:
-            config_dict["batch_dim"] = None
-
-        config_dict["custom_configs"] = self._get_custom_configs(self.status.config["custom_configs"])
-        config_dict["target_device"] = DeviceKind(config_dict["target_device"])
-        return CommonConfig(
-            model=None,
-            workspace=self.workspace,
-            dataloader=[],
-            **config_dict,
+        def _extract_format_version(status_dict):
+            format_version = status_dict.get("format_version", "0.1.0")
+            if format_version == "0.1.0" and "optimization_profile" in status_dict["export_config"]:
+                format_version = "0.1.1"
+            return version.parse(format_version)
+
+        format_version = _extract_format_version(data_dict)
+        StatusDictUpdater().update(data_dict, format_version)
+
+        if isinstance(data_dict["config"].get("_input_names"), Sequence):
+            data_dict["config"]["_input_names"] = tuple(data_dict["config"]["_input_names"])
+        if isinstance(data_dict["config"].get("_output_names"), Sequence):
+            data_dict["config"]["_output_names"] = tuple(data_dict["config"]["_output_names"])
+
+        dataloader_trt_profile = TensorRTProfile()
+        for name, val in data_dict["dataloader_trt_profile"].items():
+            dataloader_trt_profile.add(name, **val)
+
+        models_status = {
+            model_key: ModelStatus.from_dict(models_status)
+            for model_key, models_status in data_dict["models_status"].items()
+        }
+        # update model_config parents
+        for model_status, model_status_dict in zip(models_status.values(), data_dict["models_status"].values()):
+            for parent_model_key in models_status:
+                if parent_model_key == model_status_dict["model_config"]["parent_key"]:
+                    model_status.model_config.parent = models_status[parent_model_key].model_config
+
+        return cls(
+            format_version=NAVIGATOR_PACKAGE_VERSION,
+            model_navigator_version=NAVIGATOR_VERSION,
+            uuid=data_dict["uuid"],
+            environment=data_dict["environment"],
+            config=data_dict["config"],
+            models_status=models_status,
+            input_metadata=TensorMetadata.from_json(data_dict["input_metadata"]),
+            output_metadata=TensorMetadata.from_json(data_dict["output_metadata"]),
+            dataloader_trt_profile=dataloader_trt_profile,
+            dataloader_max_batch_size=int(data_dict["dataloader_max_batch_size"]),
+            timestamp=data_dict["timestamp"],
         )
 
-    def load_source_model(self, model: object) -> None:
-        """Load model defined in Python code.
-
-        Args:
-            model: A model object
-        """
-        if self._model is not None:
-            LOGGER.warning("Overriding existing source model.")
-        self._model = model
-
-    def _get_best_runtime(
-        self,
-        strategy: Optional[RuntimeSearchStrategy] = None,
-        include_source: bool = True,
-    ):
-        if strategy is None:
-            strategy = MaxThroughputAndMinLatencyStrategy()
-
-        formats = None
-        if not include_source:
-            formats = [fmt.value for fmt in SERIALIZED_FORMATS]
-
-        runtime_result = RuntimeAnalyzer.get_runtime(self.status.models_status, strategy=strategy, formats=formats)
-        return runtime_result
-
-    def get_runner(
-        self,
-        strategy: Optional[RuntimeSearchStrategy] = None,
-        include_source: bool = True,
-    ) -> NavigatorRunner:
-        """Get the runner according to the strategy.
-
-        Args:
-            strategy: Strategy for finding the best runtime. Defaults to `MaxThroughputAndMinLatencyStrategy`.
-            include_source: Flag if Python based model has to be included in analysis
+    def get_model_configs(self) -> Dict[Format, List[ModelConfig]]:
+        """Get model configurations from the status.
 
         Returns:
-            The optimal runner for the optimized model.
+            Dict[Format, List[ModelConfig]]: Dictionary where key is a model format
+                and value is a list of model configs for this format.
         """
-        runtime_result = self._get_best_runtime(strategy=strategy, include_source=include_source)
+        model_configs = collections.defaultdict(list)
+        for models_status in self.models_status.values():
+            model_configs[models_status.model_config.format].append(models_status.model_config)
+        return model_configs
+
+
+class StatusDictUpdater:
+    """Update status dictionary to the current version."""
+
+    def __init__(self):
+        """Construct StatusDictUpdater."""
+        self._updates = {
+            version.parse("0.1.0"): self._update_from_v0_1_0,
+            version.parse("0.1.2"): self._update_from_v0_1_2,
+            version.parse("0.1.3"): self._update_from_v0_1_3,
+            version.parse("0.1.4"): self._update_from_v0_1_4,
+            version.parse("0.2.1"): self._update_from_v0_2_1,
+        }
 
-        model_config = runtime_result.model_status.model_config
-        runner_status = runtime_result.runner_status
+    def update(self, data_dict: Dict, format_version: version.Version):
+        """Update the status data dict from the format_version to the current version.
 
-        if not is_source_format(model_config.format) and not (self.workspace / model_config.path).exists():
-            raise ModelNavigatorNotFoundError(
-                f"The best runner expects {model_config.format.value!r} "
-                "model but it is not available in the loaded package."
+        Args:
+            data_dict (Dict): Data dict to be updated.
+            format_version (version.Version): Version of the data dict to be updated.
+        """
+        if format_version < version.parse("0.1.4"):
+            LOGGER.warning(
+                f"The version of this package is outdated. Your package's version is {format_version}, "
+                f"but the current API version {NAVIGATOR_PACKAGE_VERSION} requires at least version 0.1.4. "
+                "We do not guarantee that all Package API functions works correctly. "
+                "Please, update your package running 'nav.package.optimize(package)' function."
             )
+        for update_from_version, update_func in self._updates.items():
+            if format_version <= update_from_version:
+                update_func(data_dict)
+
+    def _update_from_v0_1_0(self, data_dict: Dict):
+        for i, model_status in enumerate(data_dict["model_status"]):
+            for runtime_results in model_status["runtime_results"]:
+                for i in range(len(runtime_results.get("performance", []))):
+                    perf_results = runtime_results["performance"][i]
+                    runtime_results["performance"][i] = {
+                        "batch_size": perf_results["batch_size"],
+                        "avg_latency": perf_results["latency"],
+                        "std_latency": None,
+                        "p50_latency": None,
+                        "p90_latency": None,
+                        "p95_latency": None,
+                        "p99_latency": None,
+                        "throughput": perf_results["throughput"],
+                        "request_count": None,
+                    }
+
+        if data_dict["export_config"]["framework"] == "pytorch" and "precision_mode" not in data_dict["config"]:
+            default_val = TensorRTPrecisionMode.SINGLE.value
+            LOGGER.info(f"Using default `precision_mode`: {default_val}")
+            data_dict["export_config"]["precision_mode"] = default_val
+        if "optimization_profile" not in data_dict["export_config"]:
+            default_val = OptimizationProfile().to_dict()
+            LOGGER.info(f"Using default `optimization_profile`: {default_val}")
+            data_dict["export_config"]["optimization_profile"] = default_val
+        if (
+            "git_info" not in data_dict
+        ):  # FIXME problably git_info should be removed from package updater - git_info no longer saved in status.yaml
+            data_dict["git_info"] = {}
+
+    def _update_from_v0_1_2(self, data_dict: Dict):
+        data_dict["trt_profile"] = DataObject.parse_value(
+            get_trt_profile_from_trt_dynamic_axes(data_dict["export_config"]["trt_dynamic_axes"])
+        )
+        for model_status in data_dict["model_status"]:
+            if model_status["format"] == "torch-trt" and model_status.get("precision") is None:
+                model_status["precision"] = "fp32"
+
+    def _update_from_v0_1_3(self, data_dict: Dict):
+        if (
+            data_dict["export_config"]["framework"] == "pytorch"
+            and data_dict["export_config"].get("precision_mode") is None
+        ):
+            default_val = TensorRTPrecisionMode.SINGLE.value
+            LOGGER.info(f"Using default `precision_mode`: {default_val}")
+            data_dict["export_config"]["precision_mode"] = default_val
+        if "onnx_runtimes" in data_dict["export_config"]:
+            data_dict["export_config"]["runtimes"] = data_dict["export_config"].pop("onnx_runtimes")
+
+    def _update_from_v0_1_4(self, data_dict: Dict):
+        models_status = {}
+        dataloader_max_batch_size = 1
+        for i, model_status in enumerate(data_dict["model_status"]):
+            model_path = model_status["path"]
+            if not model_path:
+                continue
 
-        if is_source_format(model_config.format) and self._model is None:
-            raise ModelNavigatorMissingSourceModelError(
-                "The best runner uses the source model but it is not available in the loaded package. "
-                "Please load the source model with `package.load_source_model(model)` "
-                "or exclude source model from optimal runner search "
-                "with `package.get_runner(include_source=False)`."
+            model_key = pathlib.Path(model_path).parent.name
+            model_config_dict = {
+                "key": model_key,
+                "path": model_status.get("path"),
+                "format": model_status.get("format"),
+                "parent_path": None,
+                "parent_key": None,
+                "log_path": None,
+            }
+            if "precision" in model_status:
+                model_config_dict["precision"] = model_status.get("precision")
+            if "torch_jit" in model_status:
+                model_config_dict["jit_type"] = model_status.get("torch_jit")
+            if "enable_xla" in model_status:
+                model_config_dict["enable_xla"] = model_status.get("enable_xla")
+            if "jit_compile" in model_status:
+                model_config_dict["jit_compile"] = model_status.get("jit_compile")
+
+            data_dict["model_status"][i]["model_config"] = model_config_dict
+
+            model_format = data_dict["model_status"][i]["format"]
+            runtime_results = data_dict["model_status"][i]["runtime_results"]
+            dataloader_max_batch_size, runners_status = self._prepare_runners_status_for_0_1_4(
+                dataloader_max_batch_size,
+                model_format,
+                runtime_results,
             )
 
-        return self._get_runner(model_config.key, runner_status.runner_name)
-
-    def is_empty(self) -> bool:
-        """Validate if package is empty - no models were produced.
-
-        Returns:
-            True if empty package, False otherwise.
-        """
-        for model_status in self.status.models_status.values():
-            if not is_source_format(model_status.model_config.format):
-                for runner_status in model_status.runners_status.values():
-                    if (
-                        runner_status.status.get(Correctness.__name__) == CommandStatus.OK
-                        and runner_status.status.get(Performance.__name__) != CommandStatus.FAIL
-                        and (self.workspace / model_status.model_config.path.parent).exists()
-                    ):
-                        return False
-        return True
-
-    def _get_runner(
-        self,
-        model_key: str,
-        runner_name: str,
-    ) -> NavigatorRunner:
-        """Load runner.
+            data_dict["model_status"][i].pop("runtime_results")
+            data_dict["model_status"][i]["runners_status"] = runners_status
 
-        Args:
-            model_key (str): Unique key of the model.
-            runner_name (str): Name of the runner.
+            models_status[model_key] = data_dict["model_status"][i]
 
-        Raises:
-            ModelNavigatorNotFoundError when no runner found for provided constraints.
+        data_dict.pop("model_status")
+        data_dict["models_status"] = models_status
 
-        Returns:
-            NavigatorRunner object
-        """
-        try:
-            model_config = self.status.models_status[model_key].model_config
-        except KeyError:
-            raise ModelNavigatorNotFoundError(f"Model {model_key} not found.")
-
-        if is_source_format(model_config.format):
-            model = self._model
-        else:
-            model = self.workspace / model_config.path
-        return get_runner(runner_name)(
-            model=model,
-            input_metadata=self.status.input_metadata,
-            output_metadata=self.status.output_metadata,
-        )  # pytype: disable=not-instantiable
-
-    def _create_status_file(self) -> None:
-        """Create a status.yaml file for package."""
-        path = self.workspace / self.status_filename
-        with path.open("w") as f:
-            yaml.safe_dump(self.status.to_dict(parse=True), f, sort_keys=False)
-
-    def _delete_status_file(self):
-        """Delete the status.yaml file from package."""
-        path = self.workspace / self.status_filename
-        if path.exists():
-            path.unlink()
-
-    def _update_status(
-        self,
-        execution_unit: ExecutionUnit,
-        command_output: CommandOutput,
-        shared_parameters: dict,
-    ):
-
-        self.status.input_metadata = shared_parameters.get("input_metadata", self.status.input_metadata)
-        self.status.dataloader_trt_profile = shared_parameters.get(
-            "dataloader_trt_profile", self.status.dataloader_trt_profile
-        )
-        self.status.output_metadata = shared_parameters.get("output_metadata", self.status.output_metadata)
-        self.status.dataloader_max_batch_size = shared_parameters.get(
-            "dataloader_max_batch_size", self.status.dataloader_max_batch_size
+        export_config = data_dict.pop("export_config")
+        config = self._config_from_0_1_4(export_config)
+        data_dict["config"] = config
+        data_dict["dataloader_max_batch_size"] = dataloader_max_batch_size
+        data_dict["dataloader_trt_profile"] = data_dict.get("trt_profile") or {}
+
+        data_dict["timestamp"] = export_config["timestamp"]
+
+    def _framework2framework_for_0_1_4(self, framework: str) -> str:
+        mapping = {
+            "pytorch": Framework.TORCH,
+            "tensorflow2": Framework.TENSORFLOW,
+        }
+        return mapping.get(framework, framework)
+
+    def _runtime2runners_for_0_1_4(self, model_format: str, runtime_result: Dict) -> Optional[RunnerStatus]:
+        format_and_runtime2runner = {
+            Format.ONNX.value: {
+                "CPUExecutionProvider": "OnnxCPU",
+                "CUDAExecutionProvider": "OnnxCUDA",
+                "TensorrtExecutionProvider": "OnnxTensorRT",
+            },
+            Format.TENSORRT.value: {
+                "TensorrtExecutionProvider": "TensorRT",
+                "TrtexecExecutionProvider": None,
+            },
+            Format.TF_TRT.value: {
+                "TensorFlowExecutionProvider": "TensorFlowTensorRT",
+            },
+            Format.TF_SAVEDMODEL.value: {
+                "TensorFlowExecutionProvider": "TensorFlowSavedModel",
+            },
+            Format.TORCH_TRT.value: {
+                "PyTorchExecutionProvider": "TorchTensorRT",
+            },
+            Format.TORCHSCRIPT.value: {
+                "PyTorchExecutionProvider": "TorchScriptCUDA",
+            },
+        }
+
+        runner_name = format_and_runtime2runner[model_format][runtime_result["runtime"]]
+        if not runner_name:
+            return None
+
+        tolerance = runtime_result["tolerance"]
+        performance = runtime_result["performance"]
+        verified = runtime_result["verified"]
+
+        tolerance_status = CommandStatus.OK
+        performance_status = CommandStatus.OK
+        verify_status = CommandStatus.OK
+
+        if not tolerance:
+            tolerance_status = CommandStatus.FAIL
+            performance_status = CommandStatus.SKIPPED
+            verify_status = CommandStatus.SKIPPED
+        elif not performance:
+            performance_status = CommandStatus.FAIL
+            verify_status = CommandStatus.SKIPPED
+        elif not verified:
+            verify_status = CommandStatus.SKIPPED
+
+        result = {}
+        if tolerance:
+            result[Correctness.__name__] = {
+                "per_output_tolerance": tolerance,
+            }
+
+        if performance:
+            result[Performance.__name__] = {
+                "profiling_results": performance,
+            }
+
+        runner_status = RunnerStatus(
+            runner_name=runner_name,
+            status={
+                Correctness.__name__: tolerance_status,
+                Performance.__name__: performance_status,
+                VerifyModel.__name__: verify_status,
+            },
+            result=result,
         )
 
-        if execution_unit.model_config is not None:
-            # If not models_status with given model_config then add new ModelStatus.
-            if execution_unit.model_config.key not in self.status.models_status:
-                self.status.models_status[execution_unit.model_config.key] = ModelStatus(
-                    model_config=execution_unit.model_config,
-                )
-
-            if execution_unit.runner_cls is None:
-                model_status = self.status.models_status[execution_unit.model_config.key]
-                model_status.status[execution_unit.command.__name__] = command_output.status
-                if command_output.output:
-                    model_status.result[execution_unit.command.__name__] = command_output.output
-            else:
-                model_status = self.status.models_status[execution_unit.model_config.key]
-                if execution_unit.runner_cls.name() not in model_status.runners_status:
-                    model_status.runners_status[execution_unit.runner_cls.name()] = RunnerStatus(
-                        runner_name=execution_unit.runner_cls.name(),
-                    )
-                runners_status = model_status.runners_status[execution_unit.runner_cls.name()]
-                runners_status.status[execution_unit.command.__name__] = command_output.status
-                if command_output.output:
-                    runners_status.result[execution_unit.command.__name__] = command_output.output
-        elif execution_unit.model_config is None and command_output.save:
-            self.status.status[execution_unit.command.__name__] = command_output.status
-            if command_output.output:
-                self.status.result[execution_unit.command.__name__] = command_output.output
-
-    def _cleanup(self):
-        if self.workspace.exists():
-            shutil.rmtree(self.workspace, ignore_errors=True)
-
-    @property
-    def _target_formats(self):
-        return tuple(Format(target_format) for target_format in self.status.config["target_formats"])
-
-    def _make_zip(self, zip_path, workspace, dirs_to_save, files_to_save) -> None:
-        with zipfile.ZipFile(zip_path.as_posix(), "w") as zf:
-            for dir_to_save in dirs_to_save:
-                for root, _, files in os.walk(dir_to_save.as_posix()):
-                    for filename in files:
-                        zf.write(
-                            os.path.join(root, filename), os.path.relpath(os.path.join(root, filename), workspace / ".")
-                        )  # noqa: E203
-            for filepath in files_to_save:
-                zf.write(filepath, os.path.relpath(filepath, workspace / "."))  # noqa: E203
-
-    def get_best_model_status(
-        self,
-        strategy: Optional[RuntimeSearchStrategy] = None,
-        include_source: bool = True,
-    ) -> ModelStatus:
-        """Returns ModelStatus of best model for given strategy.
+        return runner_status
 
-        Args:
-            strategy: Strategy for finding the best runtime. Defaults to `MaxThroughputAndMinLatencyStrategy`.
-            include_source: Flag if Python based model has to be included in analysis
+    def _prepare_runners_status_for_0_1_4(self, dataloader_max_batch_size, model_format, runtime_results) -> Tuple:
+        runners_status = {}
+        for runtime_result in runtime_results:
+            runner_status = self._runtime2runners_for_0_1_4(model_format, runtime_result)
+            if not runner_status:
+                continue
 
-        Returns:
-            ModelStatus of best model for given strategy or None.
-        """
-        runtime_result = self._get_best_runtime(strategy=strategy, include_source=include_source)
-        return runtime_result.model_status
+            dataloader_max_batch_size = self._get_dataloader_max_batch_size_for_0_1_4(
+                dataloader_max_batch_size,
+                runner_status=runner_status,
+            )
 
-    def _get_onnx_external_weights_filepaths(self, model_path: Path) -> Set[Path]:
-        """Returns external weights paths for ONNX model."""
-        return {fp for fp in model_path.parent.iterdir() if fp.is_file()} - set(
-            self._get_reproduction_paths_to_save(self.workspace)
-        )
+            runners_status[runner_status.runner_name] = runner_status.to_dict()
 
-    def _get_models_paths_to_save(
-        self,
-        package_path: Path,
-    ) -> List[Path]:
-        models_paths_to_save = set()
-        for model_status in self.status.models_status.values():
-            format = model_status.model_config.format
-            if format in get_framework_export_formats(self.framework):
-                model_path = package_path / model_status.model_config.path
-                if not model_path.exists():
-                    LOGGER.warning(f"Model not found for {model_path.parent.name}.")
-                    continue
-
-                for runtime_results in model_status.runners_status.values():
-                    runtime = runtime_results.runner_name
-                    if runtime_results.status.get(VerifyModel.__name__) in (None, CommandStatus.SKIPPED):
-                        LOGGER.warning(f"Unverified runtime: {runtime} for the {model_path.parent.name} model.")
-
-                models_paths_to_save.add(model_path)
-
-        for strategy in [MaxThroughputStrategy(), MinLatencyStrategy()]:
-            try:
-                best_model_status = self.get_best_model_status(include_source=False, strategy=strategy)
-                best_format_path = package_path / best_model_status.model_config.path
-                if best_format_path.exists():
-                    models_paths_to_save.add(best_format_path)
-            except ModelNavigatorRuntimeAnalyzerError:
-                LOGGER.info(f"No model found with strategy: {strategy}")
-
-        external_weights_paths = set()
-        for model_path in models_paths_to_save:
-            if model_path.suffix == FORMAT2SUFFIX[Format.ONNX]:
-                external_weights_paths.update(self._get_onnx_external_weights_filepaths(model_path))
-        models_paths_to_save.update(external_weights_paths)
-
-        return list(models_paths_to_save)
-
-    def _get_reproduction_paths_to_save(self, package_path: Path) -> List[Path]:
-        reproduction_paths_to_save = set()
-        for model_status in self.status.models_status.values():
-            model_path = package_path / model_status.model_config.key
-            if not model_path.exists():
-                LOGGER.warning(f"Model path not found {model_path.name}.")
-                continue
+        return dataloader_max_batch_size, runners_status
 
-            for file in model_path.iterdir():
-                if file.suffix in [".py", ".sh", ".log"]:
-                    reproduction_paths_to_save.add(file)
+    def _get_dataloader_max_batch_size_for_0_1_4(
+        self, dataloader_max_batch_size: int, runner_status: RunnerStatus
+    ) -> int:
+        performance_result = runner_status.result.get(Performance.__name__)
+        if not performance_result:
+            return dataloader_max_batch_size
+
+        for profiling_result in performance_result.get("profiling_results", []):
+            batch_size = int(profiling_result["batch_size"])
+            if batch_size > dataloader_max_batch_size:
+                dataloader_max_batch_size = batch_size
+
+        return dataloader_max_batch_size
+
+    def _config_from_0_1_4(self, export_config: Dict):
+        framework = self._framework2framework_for_0_1_4(export_config["framework"])
+        config = {
+            "framework": framework,
+        }
+
+        valid_fields = [
+            "target_formats",
+            "sample_count",
+            "batch_dim",
+            "_input_names",
+            "_output_names",
+            "optimization_profile",
+            "forward_kw_names",
+            "target_device",
+            "dynamic_axes",
+            "opset",
+            "trt_dynamic_axes",
+        ]
+
+        framework_based_classes = []
+        if framework == Framework.TORCH:
+            framework_based_classes = [TorchTensorRTConfig]
+        elif framework in [Framework.TENSORFLOW, Framework.JAX]:
+            framework_based_classes = [TensorFlowTensorRTConfig]
+
+        custom_configs_fields = {
+            "dynamic_axes": [OnnxConfig],
+            "opset": [OnnxConfig],
+            "trt_profile": [TensorRTConfig] + framework_based_classes,
+        }
+
+        custom_configs = {}
+        for field_name, value in export_config.items():
+            if field_name not in valid_fields:
+                continue
+            if field_name == "trt_dynamic_axes":
+                field_name = "trt_profile"
+                value = get_trt_profile_from_trt_dynamic_axes(value)
+
+            custom_config_classes = custom_configs_fields.get(field_name)
+            if custom_config_classes:
+                for config_class in custom_config_classes:
+                    obj = custom_configs.get(config_class.name(), {})
+                    obj[field_name] = value
+                    custom_configs[config_class.name()] = obj
+            else:
+                config[field_name] = value
 
-        return list(reproduction_paths_to_save)
+        config["custom_configs"] = custom_configs
 
-    def _get_custom_configs(self, custom_configs: Dict[str, Dict]) -> Dict:
-        """Build custom configs from config data.
+        if "runtimes" in export_config:
+            config["runner_names"] = export_config["runtimes"]
 
-        Args:
-            custom_configs: Dictionary with custom configs data
+        return config
 
-        Returns:
-            List with mapped objects
-        """
-        custom_configs_mapped = {}
-        for class_name, fields in custom_configs.items():
-            custom_config_class = CUSTOM_CONFIGS_MAPPING[class_name]
-            obj = custom_config_class.from_dict(fields)  # pytype: disable=not-instantiable
-            custom_configs_mapped[class_name] = obj
+    def _update_from_v0_2_1(self, data_dict: Dict):
+        config = data_dict["config"]
+        optimization_profile = {}
+        if "profiler_config" in config:
+            profiler_config = config.pop("profiler_config")
+
+            if "run_profiling" in profiler_config:
+                profiler_config.pop("run_profiling")
+
+            optimization_profile = {
+                "batch_sizes": profiler_config["batch_sizes"],
+                "window_size": profiler_config["measurement_request_count"],
+                "stability_percentage": profiler_config["stability_percentage"],
+                "max_trials": profiler_config["max_trials"],
+                "throughput_cutoff_threshold": profiler_config["throughput_cutoff_threshold"],
+            }
 
-        return custom_configs_mapped
+        if optimization_profile:
+            config["optimization_profile"] = optimization_profile
```

## Comparing `triton_model_navigator-0.5.6.dist-info/LICENSE` & `triton_model_navigator-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.5.6.dist-info/METADATA` & `triton_model_navigator-0.6.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.5.6
+Version: 0.6.0
 Summary: Triton Model Navigator provides tools supporting to create Deep Learning production ready inference models
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,14 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: coloredlogs (>=15.0.0)
-Requires-Dist: dacite (>=1.6.0)
 Requires-Dist: fire (>=0.4.0)
 Requires-Dist: jsonlines (>=3.1.0)
 Requires-Dist: mpmath (<1.0.0)
 Requires-Dist: numpy (<1.24,~=1.21)
 Requires-Dist: onnx (>=1.8.1)
 Requires-Dist: onnxruntime-gpu (<1.14,~=1.13)
 Requires-Dist: onnx-graphsurgeon (>=0.3.14)
@@ -87,69 +86,65 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 Triton Model Navigator
 ========================
 
-Model conversion plays a crucial role in unlocking the maximum performance capabilities of the underlying hardware.
-By applying these transformation techniques, models can be optimized to fully utilize the specific features and optimizations offered by the hardware architecture.
-Furthermore, conversions allow for serialization of models, separating them from the source code.
-This serialization process enhances portability, allowing the models to be seamlessly deployed in production environments.
-The decoupling of models from the source code also facilitates maintenance, updates, and collaboration among developers.
-
-However, this process comprises multiple steps and offers various potential paths,
-making manual execution complicated and time-consuming. The `Triton Model Navigator`_ offers a user-friendly and automatic solution for converting,
-optimizing and deploying machine learning models. It offers a single entry point for various supported frameworks,
-allowing users to start the process of searching for the best deployment option with a single call to the dedicated `optimize` function.
-Model Navigator handles model export, conversion, correctness testing, and performance profiling, saving all generated artifacts.
-
-Throughout the optimize process, the Model Navigator considers multiple factors, including different precisions,
-runtimes, and data shapes. This careful consideration allows for the adjustment of the model's configuration to achieve improved performance,
-effectively minimizing the costs associated with serving the model.
-
-Converted models can be easily deployed on the `PyTriton`_ or `Triton Inference Server`_ .
-
+Model optimization plays a crucial role in unlocking the maximum performance capabilities of the underlying hardware. By
+applying various transformation techniques, models can be optimized to fully utilize the specific features offered by
+the hardware architecture to improve the inference performance and cost. Furthermore, in many cases allow for
+serialization of models, separating them from the source code. The serialization process enhances portability, allowing
+the models to be seamlessly deployed in production environments. The decoupling of models from the source code also
+facilitates maintenance, updates, and collaboration among developers. However, this process comprises multiple steps and
+offers various potential paths, making manual execution complicated and time-consuming.
+
+The `Triton Model Navigator` offers a user-friendly and
+automated solution for optimizing and deploying machine learning models. Using a single entry point for
+various supported frameworks, allowing users to start the process of searching for the best deployment option with a
+single call to the dedicated `optimize` function. Model Navigator handles model export, conversion, correctness testing,
+and profiling to select optimal model format and save generated artifacts for inference deployment on the
+`PyTriton`_ or `Triton Inference Server`_ .
 
 The Model Navigator generates multiple optimized and production-ready models.
 The table below illustrates the model formats that can be obtained by using the Model Navigator with various frameworks.
 
 **Table:** Supported conversion target formats per each supported Python framework or file.
 
-+--------------------+--------------------+--------------------+----------+
-| PyTorch            | TensorFlow 2       | JAX                | ONNX     |
-+====================+====================+====================+==========+
-| Torch 2 Compile    | SavedModel         | SavedModel         | TensorRT |
-| TorchScript Trace  | TensorFlowTensorRT | TensorFlowTensorRT |          |
-| TorchScript Script | ONNX               | ONNX               |          |
-| TorchTensorRT      | TensorRT           | TensorRT           |          |
-| ONNX               |                    |                    |          |
-| TensorRT           |                    |                    |          |
-+--------------------+--------------------+--------------------+----------+
++--------------------+------------------------+------------------------+----------+
+| PyTorch            | TensorFlow 2           | JAX                    | ONNX     |
++====================+========================+========================+==========+
+| Torch 2 Compile    | SavedModel             | SavedModel             | TensorRT |
+| TorchScript Trace  | TensorRT in TensorFlow | TensorRT in TensorFlow |          |
+| TorchScript Script | ONNX                   | ONNX                   |          |
+| TorchTensorRT      | TensorRT               | TensorRT               |          |
+| ONNX               |                        |                        |          |
+| TensorRT           |                        |                        |          |
++--------------------+------------------------+------------------------+----------+
 
 **Note:** The Model Navigator has the capability to support any Python function as input.
 However, in this particular case, its role is limited to profiling the function without generating any serialized models.
 
 The Model Navigator stores all artifacts within the `navigator_workspace`.
 Additionally, it provides the option to save a portable and transferable `Navigator Package` that includes only the models with minimal latency and maximal throughput.
 This package also includes base formats that can be used to regenerate the `TensorRT` plan on the target hardware.
 
 **Table:** Model formats that can be generated from saved `Navigator Package` and from model sources.
 
 +------------------------+-----------------------------+
 |   From model source    |   From Navigator Package    |
 +========================+=============================+
 | SavedModel             | TorchTensorRT               |
-| TensorFlowTensorRT     | TensorFlowTensorRT          |
+| TensorRT in TensorFlow | TensorRT in TensorFlow      |
 | TorchScript Trace      | ONNX                        |
 | TorchScript Script     | TensorRT                    |
 | Torch 2 Compile        |                             |
 | TorchTensorRT          |                             |
 | ONNX                   |                             |
-| TensoRT                |                             |
+| TensorRT               |                             |
 +------------------------+-----------------------------+
 
 Installation
 --------------
 
 The package can be installed using extra index url:
 
@@ -173,80 +168,48 @@
 - `jax` - Model Navigator with dependencies for JAX
 
 For using with PyTorch no extras are needed.
 
 Quick Start
 -------------
 
-Using Model Navigator is as simply as calling `optimize` with `model` and `dataloader`:
-The `optimize` function will save all the artifacts it generates in the `navigator_workspace`.
+Optimizing models using Model Navigator is as simply as calling `optimize` function. The optimization process requires
+at least:
 
-**Note:** The `dataloader` is utilized to determine the maximum and minimum shapes of the inputs utilized during model conversions.
-The `Model Navigator` employs a single sample from the `dataloader`, which is then repeated to generate synthetic batches for profiling purposes.
-Correctness tests are conducted on a subset of the `dataloader` samples, while verification tests are executed on the entire `dataloader`.
+- `model` - a Python object, callable or file path with model to optimize.
+- `dataloader` - a method or class generating input data. The data is utilized to determine the maximum and minimum
+  shapes of the model inputs and create output samples that are used during the optimization process.
+
+Here is an example of running `optimize` on Torch Hub ResNet50 model:
 
 .. code-block:: python
 
     import logging
 
     import torch
     import model_navigator as nav
 
     nav.torch.optimize(
         model=torch.hub.load('NVIDIA/DeepLearningExamples:torchhub', 'nvidia_resnet50', pretrained=True).eval(),
         dataloader=[torch.randn(1, 3, 256, 256) for _ in range(10)],
     )
 
-The code snippet below demonstrates the usage of the `PyTritonAdapter` to retrieve the `runner` and other necessary information.
-The `runner` serves as an abstraction that connects the model checkpoint with its runtime, making the inference process more accessible and straightforward.
-Following that, it initiates the `PyTriton`_  server using the provided parameters.
-
-.. code-block:: python
-
-    pytriton_adapter = nav.pytriton.PyTritonAdapter(package=package, strategy=nav.MaxThroughputStrategy())
-    runner = pytriton_adapter.runner
-
-    runner.activate()
-
-    @batch
-    def infer_func(**inputs):
-        return runner.infer(inputs)
-
-    with Triton() as triton:
-        triton.bind(
-            model_name="resnet50",
-            infer_func=infer_func,
-            inputs=pytriton_adapter.inputs,
-            outputs=pytriton_adapter.outputs,
-            config=pytriton_adapter.config,
-        )
-        triton.serve()
-
-Alternatively, Model Navigator can generate `model_repository` that can be served on the `Triton Inference Server`_:
-
-
-.. code-block:: python
-
-    nav.triton.model_repository.add_model_from_package(
-        model_repository_path=pathlib.Path("model_repository"),
-        model_name="resnet50",
-        package=package,
-        strategy=nav.MaxThroughputStrategy(),
-    )
-
+Once the model has been optimized the created artifacts are stored in `navigator_workspace` and a Package object is
+returned from the function. The returned object can be used to create `Navigator Package` or deploy model on `PyTriton`_
+or `Triton Inference Server`_. Read more about it in `documentation`_
 
 Examples
 ----------
 
 We provide step-by-step examples that demonstrate how to use various features of Model Navigator.
 For the sake of readability and accessibility, we use a simple `torch.nn.Linear` model as an example.
 These examples illustrate how to optimize, test and deploy the model on
 the PyTriton and Triton Inference Server.
 
-https://github.com/triton-inference-server/model_navigator/tree/main/examples.
+Examples: https://github.com/triton-inference-server/model_navigator/tree/main/examples.
 
 Links
 -------
 
 * Documentation: https://triton-inference-server.github.io/model_navigator
 * Source: https://github.com/triton-inference-server/model_navigator
 * Issues: https://github.com/triton-inference-server/model_navigator/issues
@@ -254,7 +217,8 @@
 * Known Issues: https://github.com/triton-inference-server/model_navigator/blob/main/docs/known_issues.md
 * Contributing: https://github.com/triton-inference-server/model_navigator/blob/main/CONTRIBUTING.md
 
 .. _Triton Model Navigator: https://github.com/triton-inference-server/model_navigator
 .. _Triton Inference Server: https://github.com/triton-inference-server/server
 .. _TensorRT: https://github.com/NVIDIA/TensorRT
 .. _PyTriton: https://github.com/triton-inference-server/pytriton
+.. _documentation: https://triton-inference-server.github.io/model_navigator
```

## Comparing `triton_model_navigator-0.5.6.dist-info/RECORD` & `triton_model_navigator-0.6.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,133 +1,145 @@
 model_navigator/__init__.py,sha256=YQ8MA8xQgnLgxeQ_oK_E7W8Tpxavwj0SKvbiq4r-JJE,881
-model_navigator/__version__.py,sha256=OAsic7CwhOApIQYmiIX1VsDMoVwieEfdphmvFQ01s-Y,649
-model_navigator/exceptions.py,sha256=6wR9REQeNkmHOklMPQ46SrGC61EJVH4jz0n2BC4e7ek,3668
-model_navigator/execution_context.py,sha256=eYV2YJU4V8X-v-dWTI6Oi5zJl3RdtK41XWtPxPRxNvU,9474
-model_navigator/logger.py,sha256=946izjz2i81kuehttGIkJ2_NhpNVCgTt6y9fL-s19-U,4790
-model_navigator/api/__init__.py,sha256=ZCychLWYCVP_Q5BWXK7-8FzldMSyFTiGgcT6c_kOnJc,1716
-model_navigator/api/config.py,sha256=MkYyt3XiD37d5ptOOJOvb9HwW-sYKCZetKgCDJfT7lk,24304
-model_navigator/api/jax.py,sha256=eLDXpJsYNhVkquv6bJaO20aXO7aBqWmCGrDd1cvkzDc,6425
-model_navigator/api/onnx.py,sha256=RI9d_-H7_3Q7hkDNSGvQ89jbbbAxS1kLv-8YKlR5Kx0,5423
-model_navigator/api/package.py,sha256=8fi6d_O3z3PqiNa6SrwdvqzVctpLj2DGP5LhcLvlkn0,11860
-model_navigator/api/python.py,sha256=6OaBA1SLP_0YWnqdLf5J8C4DdN2oFjh5SjQq5I6u-_I,4906
-model_navigator/api/pytriton.py,sha256=Wz31ISb3skDmJnOzlBzmwGdr_90febOsPIzqie6K_Dc,7748
-model_navigator/api/tensorflow.py,sha256=hG7e9-NxjRz602wmgKl-JNidslbbanOQPuJO1bjgHgo,6519
-model_navigator/api/torch.py,sha256=IY_FLbh4ntAwqRR1Ji213r2XVOsd6GnjSeyAD2MmIgA,6325
+model_navigator/__version__.py,sha256=W3QIw5mWecu8uoAzvIDja1C1lD37ya3_K2g7NUKuHJM,649
+model_navigator/exceptions.py,sha256=AnYKlbe6WHk4_3lEhksgONKjtcNK7_g0-qs8mIHARuA,3915
+model_navigator/api/__init__.py,sha256=Jt9Du5gr7UP0ljMEur81SAqLg99DokO0vyw1qaonOqY,1716
+model_navigator/api/config.py,sha256=buMLeLqvirV4efpIAxgDBFo0gSoHGNttOns4dHkU_V4,24220
+model_navigator/api/jax.py,sha256=QwOjMl89TPZpj4lOOMLrGOnNrWMoVMCFhgTgk1mmCLA,6263
+model_navigator/api/onnx.py,sha256=CwX50QTt6seCbCDAOvgPLbOQjw29sL-bVWvMViFlU18,5268
+model_navigator/api/package.py,sha256=BqPo9VD_alP4aMbvvQCdqGEZZ3YrQ1PNMcDH-B-uBC8,16279
+model_navigator/api/python.py,sha256=n3Pdc_2TK9Q1yYui4R2rLh8ImC3ezhHnh-n0K1Hcom0,4795
+model_navigator/api/pytriton.py,sha256=qTMb83nJvOHCGMXVRwYMlGRKI8kW-Eqwt_K9lJJwTR4,7751
+model_navigator/api/tensorflow.py,sha256=cjo_-HGh8ZOh0kCs-4dJOkBvJTyOE4wtTp3J5kNlCiI,6350
+model_navigator/api/torch.py,sha256=y6hLMmkkl3OJICEOTZDL6yQ7b-ijiiOEWEe6joXIReM,6158
 model_navigator/api/triton.py,sha256=hdrU_WJn5DFzhJ5slcdJqzRcC7n69vhmP0RKa1B3QYQ,1553
 model_navigator/api/utilities.py,sha256=iDAsvY2lFZ1ri54OSmThTVokJ31vCnHoylBHiKkYUNg,1811
 model_navigator/commands/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/commands/base.py,sha256=O75ENxJH4GtjYHru56h5XSLrR_iqnsbaQE7YHbtOnLk,4938
-model_navigator/commands/infer_metadata.py,sha256=uFDHHnadjjOFTjNVSPigBXcZYTD3h9jtPPj8-EtndWc,10065
-model_navigator/commands/load.py,sha256=7v1YqLbG0VZOf981XW-2Y6ad828d4Ynq2HNmj7_a8ys,3289
+model_navigator/commands/base.py,sha256=apYokswe-yQ8DvRKcGp6jQR6KNFGAtpLMIG5pIkugw8,5542
+model_navigator/commands/execution_context.py,sha256=v7cecavg6Xn0QD-3b_3qb9IaIzcKY8htnSZZtDw-fzM,9486
+model_navigator/commands/infer_metadata.py,sha256=xWwubLpHI_Y46XrH0yXWvo1inSkDuIXXakpnA1rlI6Q,12793
+model_navigator/commands/load.py,sha256=NhcPPfkWqnRJJt18qCaNw54mffqs84Aotei8Vt72qv4,3325
 model_navigator/commands/convert/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/commands/convert/base.py,sha256=YlFjgaik1oqZr9m8FujYQ-gunFoHXA8dgLScgXTG__E,9863
-model_navigator/commands/convert/tf.py,sha256=-5YBgVGglo1hLsyjmF7RRrOsEg1jRIfdtpN0Efar9EU,7489
-model_navigator/commands/convert/torch.py,sha256=rWsZDF8Wv-xdv2AyFNGKWbJtNu_-N42j2lHMdb94CE0,9879
+model_navigator/commands/convert/base.py,sha256=A_1BeYl2eEz7mAIJyt0j4KV_4p6T8-tEGaM_oO5jf8o,9868
+model_navigator/commands/convert/tf.py,sha256=d3whrl14w0i9wmertOc96XpZlaApsQInBs2ovpbTCOw,7633
+model_navigator/commands/convert/torch.py,sha256=acOP_Xm0PeNsPWo24IES5MM5R6AD2hmPJxZOTR9O-tk,10029
 model_navigator/commands/convert/converters/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/convert/converters/sm2tftrt.py,sha256=AcNyKV60yCUrzJ5B501H5SHKjtkr7kaNXNIewnOFJzk,3418
 model_navigator/commands/convert/converters/ts2onnx.py,sha256=ezjlPeHHbhx2LB4HDoLkVlmaZa1dreVMQMk2PL5UMos,3105
 model_navigator/commands/convert/converters/ts2torchtrt.py,sha256=a_mpR0j4y5ClaY6Ik_oIKEAlh45zD-ycCLHigsy1C7M,4992
 model_navigator/commands/convert/onnx/__init__.py,sha256=LwvvDj4oH7rwmUJXVEyRxIOWZnUxix6n_DmkAJzEJBY,680
 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py,sha256=KQR-qrVWVVBGVr5pqcKink2dcDNCk1Lszvl8x6TwqjU,1727
-model_navigator/commands/convert/onnx/onnx2trt.py,sha256=2dCVmkRhC0jJOANzdjilzXkG3NdDxMx_xXGkRILxJnM,10643
+model_navigator/commands/convert/onnx/onnx2trt.py,sha256=hOwaQ5oIIuVyaniXOusRtBUk5VLeOVrKWs2xcwaBMFg,10733
 model_navigator/commands/convert/onnx/trt_load_script.py,sha256=D2fTNNIBELAsBSmy3ij9oxMyRDxi0RNFV29zAlPYFz8,2235
 model_navigator/commands/copy/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/commands/copy/onnx.py,sha256=Z2dtowzXW1qVJq2L4bNNLLRRTbyeiJT7MoIxi4y42fk,1729
+model_navigator/commands/copy/onnx.py,sha256=iQvV13MLoE9XjPKv--gSBTnDrjO-WYeSHOQI3ITRSp4,1798
 model_navigator/commands/correctness/__init__.py,sha256=Xm-ikcHX6zpdmukjkSgL4JnPt2FIImoxXUPsL-334FM,678
-model_navigator/commands/correctness/correctness.py,sha256=qPBKlBE_wuJTtIJ2tt8zXWjFestp-nDvIn3Zh5T5xsc,5594
-model_navigator/commands/correctness/correctness_script.py,sha256=USxoVaa0flsEjNy-vYxjDTkF5Z-lVSY6Jl6Zv9sqNOA,4550
+model_navigator/commands/correctness/correctness.py,sha256=qM4FhOAnLzazob4PyZLdcZkWMG62PLG54k4QHyvJW8Y,5674
+model_navigator/commands/correctness/correctness_script.py,sha256=Ejdk8rM7_wPxP5gwIkryOVghKMzCUrqF9L2J8V9kKF0,4733
 model_navigator/commands/data_dump/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/commands/data_dump/samples.py,sha256=9oJ8WEQLz5tGr1RvskjvXganpnL1p3E0BDcTF9lrI5I,11162
+model_navigator/commands/data_dump/samples.py,sha256=SH_4Aejt16bN6JoQPd-sVa4wwFJKtkGjudK9PhBG3RA,10740
 model_navigator/commands/export/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/commands/export/jax.py,sha256=A9MBAKbu99UNqbHxAp87sKkwZnQgLn9ZY1kD40XLYEc,3531
-model_navigator/commands/export/tf.py,sha256=JSQ4JrMf2duzhxoimae0g3tJtJaD7RXHsuyMUHkC-b0,5485
-model_navigator/commands/export/torch.py,sha256=gueN1U39frfBMxeWL5Ivi7OaB87gH5HVcUQDg0E8p-Q,9043
+model_navigator/commands/export/jax.py,sha256=O-4Ua4GnulFDC8DJhtjh40rYgEy0OHqKgkRgPpn_0RE,3611
+model_navigator/commands/export/tf.py,sha256=SX7-VJJSUJ86BCSZsz7ZLsi2B4OHnrk5du7-7zLb8FY,5598
+model_navigator/commands/export/torch.py,sha256=uCYN6IaJrO8nmOiCcapQ09V6JXDqU9hobR72_UTdeF8,9156
 model_navigator/commands/export/exporters/__init__.py,sha256=ZkOuCGTEqfxCY1PilU3DJV4IMMuMpTEEm2KsCmmcoMQ,1056
 model_navigator/commands/export/exporters/jax2savedmodel.py,sha256=LSr8I4mRHpwYZNDCs3IfUAyk3n89951bjA1JM_rnQks,3945
 model_navigator/commands/export/exporters/keras2savedmodel.py,sha256=oG4BqcklEmTtpwd3tlyKhNBub41VrQBqiiTfRKZaU6Q,3171
 model_navigator/commands/export/exporters/savedmodel2savedmodel.py,sha256=sdE76nSyXD8i_OfePhOEFBiMQFSOsVRiFf8bu26SoaE,3122
 model_navigator/commands/export/exporters/torch2onnx.py,sha256=sTj6uVxFfr-avTjSWC9RXayQhyPkyvjY1YWJhXFrQxc,3077
 model_navigator/commands/export/exporters/torch2torchscript.py,sha256=UdBcw1TVoaj85Tg6ww-MhkGkHB15ZfbJf6x9szJ3PXE,2728
 model_navigator/commands/find_max_batch_size/__init__.py,sha256=-j67tQs-RhZGWwXSqmRZ7OqR7NOdNRjg4RhBgvOhBhg,715
-model_navigator/commands/find_max_batch_size/find_max_batch_size.py,sha256=_iOAw1NPGPwzaeMu8yy-xBdougxFNSDlVu3RrsBw9ng,6396
-model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py,sha256=WWbNxCUm8D4KoUl0VIka4E8roqGU8NI3IHVYr6dgHhg,2984
-model_navigator/commands/performance/__init__.py,sha256=ypw9fRZEp0MA0z1qAxb4-7t9LuUtyRASNP5WHBoMAlw,688
-model_navigator/commands/performance/performance.py,sha256=Kq5-gYrxhXpzNhCeVVSw_EL8I8zQaaPpfAwi7qjGknU,15770
-model_navigator/commands/performance/performance_script.py,sha256=oIUR9gDtknCq6RQ-B9NFQFLwtiRIPjPlqw8VxFkV5Q8,3037
+model_navigator/commands/find_max_batch_size/find_max_batch_size.py,sha256=UWXtr4rSQvqx7c_K-f-3Zd_ENE4-dXXZQnhlPj2p3mo,7156
+model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py,sha256=HHEFm_lGMktDgNkkPkR6z3fw7_8hlMepOdi1iZHrjBA,3075
+model_navigator/commands/performance/__init__.py,sha256=n2cNwGfJdB8BWley7UvQJoI-zmrSfer9OXmOBJsnJI0,784
+model_navigator/commands/performance/performance.py,sha256=QATSOzJGD05E0xSzhe9t-X73rPw4J4aiTDsZ9Bph2sk,5260
+model_navigator/commands/performance/profile.py,sha256=YZZ2uM6NtGjU2Q2s8DWBb1m5GK4mPvKRHc-zS1AAJ24,6964
+model_navigator/commands/performance/profile_script.py,sha256=29c4eJKWWuRFNX8dSavVl3FS7lNL2EnraraEHInU3LA,3104
+model_navigator/commands/performance/profiler.py,sha256=GZJ6Jg3pt9plRTt5AF755oWHgWhUOFRku-ukIIscby4,7269
+model_navigator/commands/performance/results.py,sha256=nwHs7iJlSdxmLebQvUjEhVtd6--xwdRSmo308rIJh48,5476
 model_navigator/commands/verification/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/commands/verification/verify.py,sha256=WPZlbUgaQFprBPVhbCYWfk3m1k65f8RMJVtvBYocNt8,5441
+model_navigator/commands/verification/verify.py,sha256=V_xJaHcKjO42hj2VUU3WgPqe-aK0CaVWA5CHNy_8FHs,4657
 model_navigator/configuration/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/configuration/common_config.py,sha256=MgweUSANUGWnVSlvPvYH1VHxXYspkQ5YLQrZifKlb0g,2473
+model_navigator/configuration/common_config.py,sha256=PUYxuhOSJ79BPUN7S0WuGurYaRU1v2siaaKLtnaMN7Y,2002
 model_navigator/configuration/model/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/configuration/model/model_config.py,sha256=LHeJ9oWqigacrWLf0_bc0PIC4EoJMduaec3C8-QgF2I,15623
+model_navigator/configuration/model/model_config.py,sha256=fmcaM9PzKpVAkL6G-EvbPi2bFArlToknPPhJeRSNJA8,15653
 model_navigator/configuration/model/model_config_builder.py,sha256=ZkCiMQDzJz8s53bp6lCBENlIr_p_65ET8UPEtj8j7Cs,13677
 model_navigator/core/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/core/constants.py,sha256=lzbcvfiiXrGjUfkGv1qTjsgSSKpUmyxvs2rBLOGeWLM,1326
-model_navigator/core/package.py,sha256=sOJ1pi4ygF2Xl4yodEKYf4r-BS8yupJiiMshQQsCkl0,20111
-model_navigator/core/status.py,sha256=BPRoUsETy-YC4bD3B5u4WUUCNK6YDalkpFagvW6Dn7I,20337
-model_navigator/core/tensor.py,sha256=21C_4LlFnakdc2Ix1QVRcvL917QoFcsi5f-xgN94O3k,8052
+model_navigator/core/constants.py,sha256=YLeoH188MYjgWMCLWcvftnE8wMBj0Y5lDu4WUhlWt44,1389
+model_navigator/core/logger.py,sha256=bm6Fh2IXxa0drnvmnwKJMuNtmrg9HS8AZykxxbds17I,5299
+model_navigator/core/tensor.py,sha256=-pzcLSJ6KWAYsK6pAn4Wu_eKa1P6M41gf-3ltyxWhpQ,9941
+model_navigator/core/workspace.py,sha256=BWC5I5I1fthZVrjoJqLg_AFWv8RH6nvSIQnrzV63F7U,2147
 model_navigator/frameworks/__init__.py,sha256=4ACuhCJjgzDo3zub8dNU_FYLiioG8n8iFFiO3LftbFg,2817
 model_navigator/frameworks/jax/__init__.py,sha256=DBjOUuVsMRMwOEPVPFVKQxPQTkYYcRLHvT0jjh907b4,669
 model_navigator/frameworks/jax/model.py,sha256=WROviV0IDfQKkfneaX88wZm7f3WhrB4DwB3-bl4_Qio,1554
 model_navigator/frameworks/onnx/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/frameworks/onnx/utils.py,sha256=L3IDVu0r-_BHSdf4htXwsmMVPoInk9Qset6SA66LusI,1085
 model_navigator/frameworks/tensorrt/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/frameworks/tensorrt/cuda.py,sha256=dT5HPExUqQnsR3npcpgCuc0iCnAUTSfjkLK-2eNkiw4,26575
-model_navigator/frameworks/tensorrt/utils.py,sha256=sPmc1OF84WRzYLi7MFgjpKJkx8Rv4-Xx-fbMFRfGggs,9874
+model_navigator/frameworks/tensorrt/cuda.py,sha256=T2mHYLdgBTqf2eIgryECZmp_EiTTLIVZEuK_Q3Gl7JA,27191
+model_navigator/frameworks/tensorrt/utils.py,sha256=ZzerG6EUlJx4hivcknnyN92b7SSaZdQuXRmgg_Nby4Y,10627
 model_navigator/frameworks/torch/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/frameworks/torch/utils.py,sha256=czQ3umUl1UtYydDApapftpEOBZsWCAdVyPD5wF9Gjq8,1508
+model_navigator/frameworks/torch/utils.py,sha256=dv3m37LjHV286b4THAOefyDX9jBi2J3iJWRMET6M2H4,1513
+model_navigator/package/__init__.py,sha256=ygs5wE6IuzQ0w4g8nWq8jrkkoYoWtdPY0zxJmKiW80M,622
+model_navigator/package/builder.py,sha256=H_G2_9UVcQWCvL7nwzaRML-gG3Ppc50-azmEUqFweuw,12176
+model_navigator/package/loader.py,sha256=gv61Ks9vDJ0nHWK4Tug_RIycBLkWkBsUYKOOndiJHL0,4651
+model_navigator/package/package.py,sha256=pYEN7wxN4QYZmsWgi-cM1XEiz0Al8hWoiopH52oa6Dw,11755
+model_navigator/package/profiling_results.py,sha256=SPT3JXXwzIJK355ccegFtIXdXI6jqqqIUciwulkH0bw,2819
+model_navigator/package/status.py,sha256=WqKhUhkjWj0LZEINO35PE1Aizqy-lxtuEN55NgqvnIo,21135
 model_navigator/pipelines/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/pipelines/pipeline.py,sha256=l5ZGqSbdLwKanojJJGdQfDnABgJB_c-NGPnYJoQkB14,5685
-model_navigator/pipelines/pipeline_manager.py,sha256=4iBxa5-cT-Dch4Y1NNsPtK32-ypYPfFpkrKVwFsyKRA,7333
-model_navigator/pipelines/validation.py,sha256=5N8KOjMCOI_TH3JYKMQgyWH24l5OXvZrMAsSoI8n1-s,9805
-model_navigator/pipelines/builders/__init__.py,sha256=itg2I3yJgd25bTF1ewdEla6R5xjYO-8IwtOOYf0NQAg,1879
-model_navigator/pipelines/builders/correctness.py,sha256=LIm_qCMu33l1tbKw2FcJ_8rAlumg7hHZxsXwuRylJCM,2036
-model_navigator/pipelines/builders/find_device_max_batch_size.py,sha256=K8TJrw_4GlM6N8ZZMKxjhM8tipo6yK7Zt5qXE05Yjqk,5703
-model_navigator/pipelines/builders/jax.py,sha256=Xy-C-ciFrQ7_9QQYCq5JOGm58SLz3t9i-pgMnfxSvlU,1647
-model_navigator/pipelines/builders/onnx.py,sha256=QOs0HzZkDmHzIPXj0zGtkq38R-7-7TyrlztcyXIVzTo,2483
-model_navigator/pipelines/builders/preprocessing.py,sha256=pqie8TQVNV-X6YxDDn3CDNJUvevbHQ99tRED4NblAtE,2365
-model_navigator/pipelines/builders/profiling.py,sha256=sa3q3AvdQOVLJiCxEG50RYuS12LZcLJx2iGEU9XloNk,2685
-model_navigator/pipelines/builders/tensorflow.py,sha256=vFt59zR0XiRr2BF2sbSpnRgaSG6VyywexiAx_0qnrb8,2869
-model_navigator/pipelines/builders/torch.py,sha256=Cd-dNkKqhwSDzu898s0hzqE1jyipTRaLx0efRFTaZWk,3261
-model_navigator/pipelines/builders/verify.py,sha256=GIK2mGl1h45TSdqXYOzFyCkBovTaYSsEzcJ9DssrGTU,2042
+model_navigator/pipelines/pipeline.py,sha256=81YfJxylmZUt1_AYinwnq8h9lqy5tl5UDPOa_fikXps,5232
+model_navigator/pipelines/pipeline_context.py,sha256=_ZDSiSFXyFiPJI8GERvIq5J2qTJYYFZhP5c_y-gKTIs,14762
+model_navigator/pipelines/pipeline_manager.py,sha256=Moy6zVv9ya6Bl2vrAICMonpsPvxcwLK841ZXqQ0nuwg,3832
+model_navigator/pipelines/validation.py,sha256=8W57a57B5IfnEQKLoMu16V8SWfH73p-3oRoc0FT-92o,9693
+model_navigator/pipelines/builders/__init__.py,sha256=EtN2lemirbxIcltc-ChUOrTrSC5Kzp-BpGffjiM2JWc,1883
+model_navigator/pipelines/builders/correctness.py,sha256=gMEb2zZTnyY1zz9BDgmpTZCRHmgK_I0TvdeMbMyyrMU,2106
+model_navigator/pipelines/builders/find_device_max_batch_size.py,sha256=-rOS2b5dxOSDdrF2NhSKU9nII4sp9-xvKhbrmQ-L5ro,5682
+model_navigator/pipelines/builders/jax.py,sha256=YA16JCveG3xChhcA4_GX5Rvd42OOdadXeMXbylmmFII,1660
+model_navigator/pipelines/builders/onnx.py,sha256=CwyxvfLnlMflLAKg6hQ7tMCGMqorZ0aNT6E9jAbc-pc,2509
+model_navigator/pipelines/builders/performance.py,sha256=YWZF-_nWHYfGqJAypFfLMeIlQqImckQpqO3bQdtALNs,2516
+model_navigator/pipelines/builders/preprocessing.py,sha256=Ks2QPjbFJh75umrbkDNpRidxCT5qo6htETHwtWrpLfk,2239
+model_navigator/pipelines/builders/profiling.py,sha256=TYYVWGZvOQkbJbLv0agreMDVImn7msSIOIeDb0eKBUI,2504
+model_navigator/pipelines/builders/tensorflow.py,sha256=dMtNCVO7lh2lWzqy_43t_Fs_faP7v9UaU0zdKGlS6OU,2921
+model_navigator/pipelines/builders/torch.py,sha256=gWt0dN3BdWoE7BlMmc98msxumR2MzuPLQAkVYEdBkA0,3326
+model_navigator/pipelines/builders/verify.py,sha256=ad45zZTOs99bLyW5Fyau-U9ug4rduQ2jT11Mrsnj_0E,2112
+model_navigator/pipelines/wrappers/__init__.py,sha256=ygs5wE6IuzQ0w4g8nWq8jrkkoYoWtdPY0zxJmKiW80M,622
+model_navigator/pipelines/wrappers/optimize.py,sha256=8mVZb4xOHeKdawsDQmWBqrlBOJuFmzTpbg_-Fzy92JE,2747
+model_navigator/pipelines/wrappers/profile.py,sha256=YVy6Kr_ObBVXEKqPgtHjTcDkn1Rrt-tfodxJVqZno18,4881
 model_navigator/runners/__init__.py,sha256=gTYI3-v7K3z8eeT3JEa4E8DSQZtnx-iBGkzFvgfVquM,1584
-model_navigator/runners/base.py,sha256=bC-73tO3tMaeZiKbtV69lLLyae_7m8fdcIPLYKhfDTo,11369
+model_navigator/runners/base.py,sha256=HIBZ8SvVODvdz8o13Spy0_uI-8-J4synYzP2NJpwYos,13796
 model_navigator/runners/jax.py,sha256=4zDe8dhv08-alz2aKJUmbkr_XgqAzkWOgjPPMtRKDjo,2620
-model_navigator/runners/onnx.py,sha256=9kwqHf4SrZlwN4S_XLVgjZ-HlmsPBhReQL93R_GemKI,7302
+model_navigator/runners/onnx.py,sha256=ofq64i3sMEvX6X4j6T48qnMRHd6pQhXdmG0wM__CFCc,9999
 model_navigator/runners/python.py,sha256=8B9ttZbMZ5Iau0TttHQJvb59HoyzHg6u-2XIcqBB7Qg,2267
-model_navigator/runners/registry.py,sha256=FmCtd7gAP5thuPzKnRZpgU_jmPhPBO_O3GenbmyCCJE,2285
+model_navigator/runners/registry.py,sha256=08eSwObowr04GmCPwDQVyywLsJNv1mNxbwlu8wC8zmk,2290
 model_navigator/runners/tensorflow.py,sha256=ghITBvu0A6w7tMvlyYCNM9JSCXalY_6jXDLssG_xWYw,7976
-model_navigator/runners/tensorrt.py,sha256=z8-uvjXEbeT7yKe01Grso0YYnr_iePtF6JV1xOZtXu0,25301
-model_navigator/runners/torch.py,sha256=_kNrSu8QOjtUYKkfQr4wCODmsVc_zQLSzONiF4gZM9I,7699
-model_navigator/runners/utils.py,sha256=PPWpRDY3Qi6kjiD8oa7J_k7kljzbesHEIPQR84KVnm0,3554
+model_navigator/runners/tensorrt.py,sha256=y5XjuZ3SCR9jeoIe2sugHJettfO-BJbmSYuSqv7gNCw,26748
+model_navigator/runners/torch.py,sha256=c4jQYEHUdO067ixVl15vS6Ro_4HjKy5ieXnf5396qR4,10041
+model_navigator/runners/utils.py,sha256=f2TNlaFKlnSqR7hP1zMicE5S4hHb7DKmDvwn4qqvGnk,3559
 model_navigator/runtime_analyzer/__init__.py,sha256=BrhKs-NzpT0ilLmYe38kUtOS7AJ-KfzyV-Hc7ANJWEE,937
-model_navigator/runtime_analyzer/analyzer.py,sha256=Y5vBtEEKPv7Ce1Mg3GV6sxe61zDj_fz7RZD8Ge6NM8s,11706
+model_navigator/runtime_analyzer/analyzer.py,sha256=9uOdHo4I9Hp0iyqJaWCS8QkGud99oJIp0AWcDbWaWjE,11714
 model_navigator/runtime_analyzer/strategy.py,sha256=L6dqnf1OS0s5mrBvxTTFgNPghKbuEFC2X_2tMm3_Hs4,2304
 model_navigator/triton/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/triton/model_config.py,sha256=Efcx0_48bmkmBwJgqm6Ejsuwh0ZPnYmyR1o6bz4Y5to,3180
 model_navigator/triton/model_config_builder.py,sha256=4uh5xArtOMnyzIKO2Duliz9SRltrP5El2xPqzE1At_0,5218
 model_navigator/triton/model_config_generator.py,sha256=i45y9ezQJ9xcQmNcGHW_5r0TZ7-Ikxvmzb9pgfBlZaY,23090
-model_navigator/triton/model_repository.py,sha256=z_9SWYHGqO7a-FP3nkP2vfQgZN6v2Lwwgvqmc-1l2eg,15245
+model_navigator/triton/model_repository.py,sha256=w8LtO3UoYB4gDstfye5x-oUuPOnYmX18pLAU_SNr3VQ,15243
 model_navigator/triton/utils.py,sha256=uJeGyzMSvxZj2hyUAC3bTk0cuMcKTYeCKAi7zerP3hA,2081
 model_navigator/triton/specialized_configs/__init__.py,sha256=lcQy-49A74vMSidK-avYy6xdX4p3OG3ygzSw6y9-OQw,944
 model_navigator/triton/specialized_configs/base_model_config.py,sha256=UOeuce-xT9lC3Zv3H3BbdSem7cTNyn7boKybxChzRgs,2872
 model_navigator/triton/specialized_configs/common.py,sha256=l6FPhZTU1WQHDVXG8HxEXx2c8s87EWgYUvtQrxqUH1k,22326
 model_navigator/triton/specialized_configs/internal.py,sha256=R42XlgUEOC5B-WotI_dAQs8sQyHJOnVyTvVk3CaZ6kM,2229
 model_navigator/triton/specialized_configs/onnx_model_config.py,sha256=oN76Ux7JI4eqlarlEVSSiIbbajAqdrF3bW0n6WQBPPw,2685
 model_navigator/triton/specialized_configs/python_model_config.py,sha256=NGijgogtoJnbBLL1hQqhw-n4rBo_OgFsCdn9ezw24VI,1785
 model_navigator/triton/specialized_configs/pytorch_model_config.py,sha256=GxJnFB4UpnUwB75t09d5XZ2iqeMZM1SmTbGe2aqmph8,2239
 model_navigator/triton/specialized_configs/tensorflow_model_config.py,sha256=C_qMi-5TAWTSL_wBDIoJju3gHRHX10RBbHvBE9of780,3162
 model_navigator/triton/specialized_configs/tensorrt_model_config.py,sha256=ikNi_i_cPjL2Mhea1uJHXe3KElvpHkiPH_zXK895pQU,3040
 model_navigator/utils/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/utils/common.py,sha256=AHqkU5xRTR6OFFq0T-UNWCQ9AoMkVdjxnyVGVhuecsw,14113
-model_navigator/utils/dataloader.py,sha256=pOXC63nRpSqUMhTh-Rr7VOSE7ohwwafXbKAcY-OfMM0,8004
+model_navigator/utils/common.py,sha256=7VBJ-f0V9aqvdGLjxsAwZEP_VuoNwASxfNh5W3bq7Mk,14528
+model_navigator/utils/dataloader.py,sha256=r549fsb5tq7ZQpnKFw4Zk9Mgc8WKzwP4wZHlpWXNj1g,8132
 model_navigator/utils/devices.py,sha256=pGjRBByJqFjG6dyJ0H2E6GJA7hIgF6rgeINLNdS27kU,3902
 model_navigator/utils/enums.py,sha256=T-G5VV5CqimxpctOqPaCvVoAwx-pp10Eeo0rKlWoVGU,1308
 model_navigator/utils/environment.py,sha256=MnpdF5eCx2DJpHtaq8fUSky0hdT03qTJrGnJDhCnFhM,6163
-model_navigator/utils/format_helpers.py,sha256=VAbRMfBw-eZljk_yDcV6Q1ojkl8ah1OnqZR6DshXNqU,3528
-model_navigator/utils/module.py,sha256=fkokQmxhWgShqrhsXDPa-g-jBA0XaUQvuVuM74WPOIM,2325
-model_navigator/utils/package.py,sha256=wp1xOwrKuB_rtVfe61y2AznmA-up320RtHNNV2UExe4,3233
-triton_model_navigator-0.5.6.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.5.6.dist-info/METADATA,sha256=b71-boQKxHg9IE_sQiYu47g8cYK1Wrc5OB3ZV2t3LN4,12074
-triton_model_navigator-0.5.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-triton_model_navigator-0.5.6.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.5.6.dist-info/RECORD,,
+model_navigator/utils/format_helpers.py,sha256=3UGJhNTFZiMorbMQrciDzJgfFW2nvLMroNmeqC8FlGs,4096
+model_navigator/utils/module.py,sha256=BX9Da3b-tOHvOFb4Ffts0Qc1i9hbgwreGbScqq_DINY,2330
+triton_model_navigator-0.6.0.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.6.0.dist-info/METADATA,sha256=MrRwS7J2lUYKGmEnXnqZ1qJgIZx8MXRllABfi8XDiTM,10798
+triton_model_navigator-0.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+triton_model_navigator-0.6.0.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.6.0.dist-info/RECORD,,
```

