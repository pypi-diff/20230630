# Comparing `tmp/optimum-1.8.8.tar.gz` & `tmp/optimum-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-1.8.8.tar", last modified: Fri Jun 16 12:41:33 2023, max compression
+gzip compressed data, was "optimum-1.9.0.tar", last modified: Fri Jun 30 01:19:24 2023, max compression
```

## Comparing `optimum-1.8.8.tar` & `optimum-1.9.0.tar`

### file list

```diff
@@ -1,149 +1,153 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.665369 optimum-1.8.8/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-16 10:34:30.000000 optimum-1.8.8/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-16 10:34:30.000000 optimum-1.8.8/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    11475 2023-06-16 12:41:33.665369 optimum-1.8.8/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9876 2023-06-16 10:34:42.000000 optimum-1.8.8/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.635369 optimum-1.8.8/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.635369 optimum-1.8.8/optimum/bettertransformer/
--rw-r--r--   0 ella      (1000) ella      (1000)      707 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/bettertransformer/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.635369 optimum-1.8.8/optimum/bettertransformer/models/
--rw-r--r--   0 ella      (1000) ella      (1000)     8420 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/bettertransformer/models/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    21474 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/bettertransformer/models/attention.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8092 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/bettertransformer/models/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    12222 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/bettertransformer/models/decoder_models.py
--rw-r--r--   0 ella      (1000) ella      (1000)    60023 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/bettertransformer/models/encoder_models.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17127 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/bettertransformer/transformation.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.635369 optimum-1.8.8/optimum/commands/
--rw-r--r--   0 ella      (1000) ella      (1000)      952 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5872 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2475 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/env.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/commands/export/
--rw-r--r--   0 ella      (1000) ella      (1000)      716 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/export/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1340 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/export/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8554 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/commands/export/onnx.py
--rw-r--r--   0 ella      (1000) ella      (1000)     9100 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/export/tflite.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/commands/onnxruntime/
--rw-r--r--   0 ella      (1000) ella      (1000)      759 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/onnxruntime/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1374 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/onnxruntime/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3885 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/onnxruntime/optimize.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4011 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/commands/onnxruntime/quantize.py
--rw-r--r--   0 ella      (1000) ella      (1000)     6871 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/optimum_cli.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/commands/register/
--rw-r--r--   0 ella      (1000) ella      (1000)      621 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/commands/register/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17957 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/configuration_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1454 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/conftest.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/exporters/
--rw-r--r--   0 ella      (1000) ella      (1000)      688 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/exporters/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)      707 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/exporters/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)      903 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/error_utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/exporters/onnx/
--rw-r--r--   0 ella      (1000) ella      (1000)     1918 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/exporters/onnx/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17290 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/onnx/__main__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    44198 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/onnx/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    16221 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/onnx/config.py
--rw-r--r--   0 ella      (1000) ella      (1000)      865 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/exporters/onnx/constants.py
--rw-r--r--   0 ella      (1000) ella      (1000)    31628 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/onnx/convert.py
--rw-r--r--   0 ella      (1000) ella      (1000)    37124 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/onnx/model_configs.py
--rw-r--r--   0 ella      (1000) ella      (1000)     7326 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/onnx/model_patcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)    11480 2023-06-16 10:35:24.000000 optimum-1.8.8/optimum/exporters/onnx/utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    60556 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/tasks.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/exporters/tflite/
--rw-r--r--   0 ella      (1000) ella      (1000)     1209 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/exporters/tflite/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5256 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/tflite/__main__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15507 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/exporters/tflite/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1397 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/exporters/tflite/config.py
--rw-r--r--   0 ella      (1000) ella      (1000)    16963 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/exporters/tflite/convert.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3588 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/exporters/tflite/model_configs.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/fx/
--rw-r--r--   0 ella      (1000) ella      (1000)      672 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/fx/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/fx/optimization/
--rw-r--r--   0 ella      (1000) ella      (1000)      866 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/fx/optimization/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    32725 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/fx/optimization/transformations.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/fx/quantization/
--rw-r--r--   0 ella      (1000) ella      (1000)      675 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/fx/quantization/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13591 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/fx/quantization/functions.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1450 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/fx/utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15269 2023-06-16 10:35:24.000000 optimum-1.8.8/optimum/modeling_base.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.645369 optimum-1.8.8/optimum/onnx/
--rw-r--r--   0 ella      (1000) ella      (1000)     1276 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnx/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3830 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnx/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    11198 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnx/graph_transformations.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4316 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnx/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13025 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnx/transformations_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3307 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnx/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.655369 optimum-1.8.8/optimum/onnxruntime/
--rw-r--r--   0 ella      (1000) ella      (1000)     4279 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    32544 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnxruntime/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    45434 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnxruntime/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      901 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/constants.py
--rw-r--r--   0 ella      (1000) ella      (1000)      955 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/graph.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.655369 optimum-1.8.8/optimum/onnxruntime/io_binding/
--rw-r--r--   0 ella      (1000) ella      (1000)      675 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/io_binding/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     7767 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/io_binding/io_binding_helper.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3915 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/model.py
--rw-r--r--   0 ella      (1000) ella      (1000)    30965 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/modeling_decoder.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17940 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    83591 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnxruntime/modeling_ort.py
--rw-r--r--   0 ella      (1000) ella      (1000)    58316 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnxruntime/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15083 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnxruntime/optimization.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.655369 optimum-1.8.8/optimum/onnxruntime/preprocessors/
--rw-r--r--   0 ella      (1000) ella      (1000)      686 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/preprocessors/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.655369 optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/
--rw-r--r--   0 ella      (1000) ella      (1000)      760 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3048 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/excluders.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1377 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/fully_connected.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1415 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/gelu.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1580 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/layernorm.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2350 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/preprocessors/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    23448 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnxruntime/quantization.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.655369 optimum-1.8.8/optimum/onnxruntime/runs/
--rw-r--r--   0 ella      (1000) ella      (1000)     8001 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnxruntime/runs/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4070 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/runs/calibrator.py
--rw-r--r--   0 ella      (1000) ella      (1000)      625 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/runs/utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    88945 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    38387 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17122 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1362 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/onnxruntime/training_args_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    11746 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/onnxruntime/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.655369 optimum-1.8.8/optimum/pipelines/
--rw-r--r--   0 ella      (1000) ella      (1000)      770 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/pipelines/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.655369 optimum-1.8.8/optimum/pipelines/diffusers/
--rw-r--r--   0 ella      (1000) ella      (1000)    11266 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2211 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/pipelines/diffusers/pipeline_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13522 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/pipelines/pipelines_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)      948 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/quantization_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10268 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/runs_base.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.655369 optimum-1.8.8/optimum/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)     1989 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)      845 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/constant.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2001 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/doc.py
--rw-r--r--   0 ella      (1000) ella      (1000)      953 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/dummy_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3747 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/file_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     6246 2023-06-16 10:38:42.000000 optimum-1.8.8/optimum/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)    23612 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/utils/input_generators.py
--rw-r--r--   0 ella      (1000) ella      (1000)     7836 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/logging.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1295 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/modeling_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     9323 2023-06-16 10:34:42.000000 optimum-1.8.8/optimum/utils/normalized_config.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.665369 optimum-1.8.8/optimum/utils/preprocessing/
--rw-r--r--   0 ella      (1000) ella      (1000)      977 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/preprocessing/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10271 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/preprocessing/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4263 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/preprocessing/image_classification.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3995 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/preprocessing/question_answering.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2169 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/preprocessing/task_processors_manager.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4436 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/preprocessing/text_classification.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3940 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/preprocessing/token_classification.py
--rw-r--r--   0 ella      (1000) ella      (1000)    11609 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/runs.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2364 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/save_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5762 2023-06-16 10:34:30.000000 optimum-1.8.8/optimum/utils/testing_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      639 2023-06-16 10:39:39.000000 optimum-1.8.8/optimum/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-16 12:41:33.635369 optimum-1.8.8/optimum.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    11475 2023-06-16 12:41:33.000000 optimum-1.8.8/optimum.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     4271 2023-06-16 12:41:33.000000 optimum-1.8.8/optimum.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-16 12:41:33.000000 optimum-1.8.8/optimum.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-16 12:41:33.000000 optimum-1.8.8/optimum.egg-info/entry_points.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-16 12:41:33.000000 optimum-1.8.8/optimum.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)     1129 2023-06-16 12:41:33.000000 optimum-1.8.8/optimum.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-16 12:41:33.000000 optimum-1.8.8/optimum.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)     1212 2023-06-16 10:34:30.000000 optimum-1.8.8/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      423 2023-06-16 12:41:33.665369 optimum-1.8.8/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     3591 2023-06-16 10:35:24.000000 optimum-1.8.8/setup.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11357 2022-04-11 08:30:37.000000 optimum-1.9.0/LICENSE
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      651 2022-04-11 08:30:37.000000 optimum-1.9.0/MANIFEST.in
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12733 2023-06-30 01:19:24.367601 optimum-1.9.0/PKG-INFO
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11114 2023-05-30 06:59:27.000000 optimum-1.9.0/README.md
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.363597 optimum-1.9.0/optimum/
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/bettertransformer/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/bettertransformer/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/bettertransformer/models/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9234 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/bettertransformer/models/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    26249 2023-06-09 09:29:41.000000 optimum-1.9.0/optimum/bettertransformer/models/attention.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8092 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/bettertransformer/models/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13124 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/bettertransformer/models/decoder_models.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    60021 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/bettertransformer/models/encoder_models.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    18000 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/bettertransformer/transformation.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/commands/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      952 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5872 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2475 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/env.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/commands/export/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      716 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/export/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1340 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/export/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      998 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/commands/export/ggml.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9198 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/commands/export/onnx.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9100 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/commands/export/tflite.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/commands/onnxruntime/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      759 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/onnxruntime/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1374 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/onnxruntime/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3885 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/onnxruntime/optimize.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4291 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/commands/onnxruntime/quantize.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6871 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/optimum_cli.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/commands/register/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      621 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/register/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17957 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/configuration_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1454 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/conftest.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/exporters/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      688 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      953 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/exporters/error_utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/exporters/onnx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1918 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/onnx/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    20403 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/__main__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    47953 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16370 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/config.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1051 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/constants.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    38753 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/convert.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    43664 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/model_configs.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9286 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/model_patcher.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12499 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    66149 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/tasks.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/exporters/tflite/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1209 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/tflite/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5693 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/tflite/__main__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15712 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/exporters/tflite/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1397 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/tflite/config.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16963 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/exporters/tflite/convert.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3588 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/tflite/model_configs.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/fx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      672 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/fx/optimization/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      866 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/optimization/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32725 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/optimization/transformations.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/fx/quantization/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/quantization/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13591 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/quantization/functions.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1450 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15218 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/modeling_base.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1276 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/onnx/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3830 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/onnx/configuration.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11171 2023-05-30 06:59:28.000000 optimum-1.9.0/optimum/onnx/graph_transformations.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4316 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/onnx/modeling_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13025 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/onnx/transformations_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3307 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/onnx/utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4279 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    33264 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    45341 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/onnxruntime/configuration.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      901 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/onnxruntime/constants.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      955 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/graph.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/io_binding/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/io_binding/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7767 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/io_binding/io_binding_helper.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3915 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/model.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    31047 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/modeling_decoder.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17940 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/modeling_diffusion.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    84386 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/modeling_ort.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    58294 2023-06-20 12:54:57.000000 optimum-1.9.0/optimum/onnxruntime/modeling_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15964 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/optimization.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/preprocessors/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      686 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      760 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3048 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/excluders.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1377 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/fully_connected.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1415 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/gelu.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1580 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/layernorm.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2350 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/quantization.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23561 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/quantization.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/runs/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7990 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/onnxruntime/runs/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4070 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/runs/calibrator.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      625 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/onnxruntime/runs/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    89043 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/trainer.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    38387 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/trainer_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17122 2023-04-17 07:37:27.000000 optimum-1.9.0/optimum/onnxruntime/training_args.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1362 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/training_args_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12010 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/pipelines/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      770 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/pipelines/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/pipelines/diffusers/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11266 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2211 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/pipelines/diffusers/pipeline_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13478 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/pipelines/pipelines_base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      948 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/quantization_base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10268 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/runs_base.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/utils/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2084 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/utils/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      845 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/constant.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2001 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/doc.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      953 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/dummy_diffusers_objects.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3747 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/file_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6422 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/utils/import_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    25488 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/utils/input_generators.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7836 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/utils/logging.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1295 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/modeling_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9820 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/utils/normalized_config.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/utils/preprocessing/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      977 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10271 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4263 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/image_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3995 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/question_answering.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2169 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/utils/preprocessing/task_processors_manager.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4436 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/utils/preprocessing/text_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3940 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/token_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11609 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/runs.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2364 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/save_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5762 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/utils/testing_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      639 2023-06-30 00:47:35.000000 optimum-1.9.0/optimum/version.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum.egg-info/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12733 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/PKG-INFO
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4365 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/SOURCES.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/dependency_links.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)       66 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/entry_points.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-04-17 13:27:45.000000 optimum-1.9.0/optimum.egg-info/not-zip-safe
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1109 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/requires.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        8 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/top_level.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1212 2023-03-21 09:04:22.000000 optimum-1.9.0/pyproject.toml
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      423 2023-06-30 01:19:24.367601 optimum-1.9.0/setup.cfg
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3554 2023-06-30 00:45:49.000000 optimum-1.9.0/setup.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/tests/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3382 2023-05-30 06:59:28.000000 optimum-1.9.0/tests/test_configuration_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1936 2023-04-11 18:28:52.000000 optimum-1.9.0/tests/test_modeling_base.py
```

### Comparing `optimum-1.8.8/LICENSE` & `optimum-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/MANIFEST.in` & `optimum-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/PKG-INFO` & `optimum-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.8.8
+Version: 1.9.0
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -82,26 +83,72 @@
 - [OpenVINO](https://huggingface.co/docs/optimum/intel/inference)
 - Habana first-gen Gaudi / Gaudi2, more details [here](https://huggingface.co/docs/optimum/main/en/habana/usage_guides/accelerate_inference)
 
 The [export](https://huggingface.co/docs/optimum/exporters/overview) and optimizations can be done both programmatically and with a command line.
 
 ### Features summary
 
-| Features                           | ONNX Runtime       | Neural Compressor  | OpenVINO           | TensorFlow Lite    |
+| Features                           | [ONNX Runtime](https://huggingface.co/docs/optimum/main/en/onnxruntime/overview)| [Neural Compressor](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc)| [OpenVINO](https://huggingface.co/docs/optimum/main/en/intel/inference)| [TensorFlow Lite](https://huggingface.co/docs/optimum/main/en/exporters/tflite/overview)|
 |:----------------------------------:|:------------------:|:------------------:|:------------------:|:------------------:|
 | Graph optimization                 | :heavy_check_mark: | N/A                | :heavy_check_mark: | N/A                |
 | Post-training dynamic quantization | :heavy_check_mark: | :heavy_check_mark: | N/A                | :heavy_check_mark: |
 | Post-training static quantization  | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 | Quantization Aware Training (QAT)  | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 | FP16 (half precision)              | :heavy_check_mark: | N/A                | :heavy_check_mark: | :heavy_check_mark: |
 | Pruning                            | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 | Knowledge Distillation             | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 
+
+### OpenVINO
+
+This requires to install the OpenVINO extra by doing `pip install optimum[openvino,nncf]`
+
+To load a model and run inference with OpenVINO Runtime, you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class. To load a PyTorch checkpoint and convert it to the OpenVINO format on-the-fly, you can set `export=True` when loading your model.
+
+```diff
+- from transformers import AutoModelForSequenceClassification
++ from optimum.intel import OVModelForSequenceClassification
+  from transformers import AutoTokenizer, pipeline
+
+  model_id = "distilbert-base-uncased-finetuned-sst-2-english"
+  tokenizer = AutoTokenizer.from_pretrained(model_id)
+- model = AutoModelForSequenceClassification.from_pretrained(model_id)
++ model = OVModelForSequenceClassification.from_pretrained(model_id, export=True)
+  model.save_pretrained("./distilbert")
+
+  classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
+  results = classifier("He's a dreadful magician.")
+```
+
+You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/inference) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/openvino).
+
+### Neural Compressor
+
+This requires to install the Neural Compressor extra by doing `pip install optimum[neural-compressor]`
+
+Dynamic quantization can be applied on your model:
+
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
+```
+
+To load a model quantized with Intel Neural Compressor, hosted locally or on the 🤗 hub, you can do as follows :
+```python
+from optimum.intel import INCModelForSequenceClassification
+
+model_id = "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
+model = INCModelForSequenceClassification.from_pretrained(model_id)
+```
+
+You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/optimization_inc) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/neural_compressor).
+
 ### ONNX + ONNX Runtime
 
+This requires to install the ONNX Runtime extra by doing `pip install optimum[exporters,onnxruntime]`
+
 It is possible to export 🤗 Transformers models to the [ONNX](https://onnx.ai/) format and perform graph optimization as well as quantization easily:
 
 ```plain
 optimum-cli export onnx -m deepset/roberta-base-squad2 --optimize O2 roberta_base_qa_onnx
 ```
 
 The model can then be quantized using `onnxruntime`:
@@ -117,82 +164,56 @@
 
 For more information on the ONNX export, please check the [documentation](https://huggingface.co/docs/optimum/exporters/onnx/usage_guides/export_a_model).
 
 #### Run the exported model using ONNX Runtime
 
 Once the model is exported to the ONNX format, we provide Python classes enabling you to run the exported ONNX model in a seemless manner using [ONNX Runtime](https://onnxruntime.ai/) in the backend:
 
-```python
-from transformers import AutoTokenizer
-from optimum.onnxruntime import ORTModelForQuestionAnswering
-
-model_name = "roberta_base_qa_onnx"
-tokenizer = AutoTokenizer.from_pretrained(model_name)
-ort_model = ORTModelForQuestionAnswering.from_pretrained(model_name)
-
-question = "What's Optimum?"
-text = "Optimum is an awesome library everyone should use!"
-inputs = tokenizer(question, text, return_tensors="pt") 
-
-# Run with ONNX Runtime.
-outputs = ort_model(**inputs)
-
-answer_start_index = outputs.start_logits.argmax()
-answer_end_index = outputs.end_logits.argmax()
+```diff
+- from transformers import AutoModelForQuestionAnswering
++ from optimum.onnxruntime import ORTModelForQuestionAnswering
+  from transformers import AutoTokenizer, pipeline
 
-predict_answer_tokens = inputs.input_ids[0, answer_start_index : answer_end_index + 1]
-answer = tokenizer.decode(predict_answer_tokens, skip_special_tokens=True)
+  model_id = "deepset/roberta-base-squad2"
+  tokenizer = AutoTokenizer.from_pretrained(model_id)
+- model = AutoModelForQuestionAnswering.from_pretrained(model_id)
++ model = ORTModelForQuestionAnswering.from_pretrained("roberta_base_qa_onnx")
+  qa_pipe = pipeline("question-answering", model=model, tokenizer=tokenizer)
+  question = "What's Optimum?"
+  context = "Optimum is an awesome library everyone should use!"
+  results = qa_pipe(question=question, context=context)
 ```
 
 More details on how to run ONNX models with `ORTModelForXXX` classes [here](https://huggingface.co/docs/optimum/main/en/onnxruntime/usage_guides/models).
 
 ### TensorFlow Lite
 
+This requires to install the Exporters extra by doing `pip install optimum[exporters-tf]`
+
 Just as for ONNX, it is possible to export models to [TensorFlow Lite](https://www.tensorflow.org/lite) and quantize them:
 
 ```plain
 optimum-cli export tflite \
   -m deepset/roberta-base-squad2 \
   --sequence_length 384  \
   --quantize int8-dynamic roberta_tflite_model
 ```
-### OpenVINO
-
-*This requires to install the Optimum OpenVINO extra by doing `pip install optimum[openvino,nncf]`.*
-
-To load a model and run inference with [OpenVINO Runtime](https://docs.openvino.ai/latest/home.html), you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class. To load a PyTorch checkpoint and convert it to the OpenVINO format on-the-fly, you can set `export=True` when loading your model.
-
-```diff
-- from transformers import AutoModelForSequenceClassification
-+ from optimum.intel import OVModelForSequenceClassification
-  from transformers import AutoTokenizer, pipeline
-
-  model_id = "distilbert-base-uncased-finetuned-sst-2-english"
-  tokenizer = AutoTokenizer.from_pretrained(model_id)
-- model = AutoModelForSequenceClassification.from_pretrained(model_id)
-+ model = OVModelForSequenceClassification.from_pretrained(model_id, export=True)
-  model.save_pretrained("./distilbert")
-
-  classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
-  results = classifier("He's a dreadful magician.")
-```
-
-You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/inference) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/openvino).
-
 
 ## Accelerated training
 
 🤗 Optimum provides wrappers around the original 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer) to enable training on powerful hardware easily.
 We support many providers:
 
 - Habana's Gaudi processors
 - ONNX Runtime (optimized for GPUs)
 
 ### Habana
 
+This requires to install the Habana extra by doing `pip install optimum[habana]`
+
 ```diff
 - from transformers import Trainer, TrainingArguments
 + from optimum.habana import GaudiTrainer, GaudiTrainingArguments
 
   # Download a pretrained model from the Hub
   model = AutoModelForXxx.from_pretrained("bert-base-uncased")
 
@@ -249,7 +270,9 @@
   )
 
   # Use ONNX Runtime for training!
   trainer.train()
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/trainer) and in the [examples](https://github.com/huggingface/optimum/tree/main/examples/onnxruntime/training).
+
+
```

### Comparing `optimum-1.8.8/README.md` & `optimum-1.9.0/optimum.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+Metadata-Version: 2.1
+Name: optimum
+Version: 1.9.0
+Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
+Home-page: https://github.com/huggingface/optimum
+Author: HuggingFace Inc. Special Ops Team
+Author-email: hardware@huggingface.co
+License: Apache
+Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: onnxruntime
+Provides-Extra: onnxruntime-gpu
+Provides-Extra: exporters
+Provides-Extra: exporters-gpu
+Provides-Extra: exporters-tf
+Provides-Extra: intel
+Provides-Extra: openvino
+Provides-Extra: nncf
+Provides-Extra: neural-compressor
+Provides-Extra: graphcore
+Provides-Extra: habana
+Provides-Extra: neuron
+Provides-Extra: neuronx
+Provides-Extra: dev
+Provides-Extra: tests
+Provides-Extra: quality
+Provides-Extra: benchmark
+License-File: LICENSE
+
 [![ONNX Runtime](https://github.com/huggingface/optimum/actions/workflows/test_onnxruntime.yml/badge.svg)](https://github.com/huggingface/optimum/actions/workflows/test_onnxruntime.yml)
 
 # Hugging Face Optimum
 
 🤗 Optimum is an extension of 🤗 Transformers and Diffusers, providing a set of optimization tools enabling maximum efficiency to train and run models on targeted hardware, while keeping things easy to use.
 
 ## Installation
@@ -42,26 +83,72 @@
 - [OpenVINO](https://huggingface.co/docs/optimum/intel/inference)
 - Habana first-gen Gaudi / Gaudi2, more details [here](https://huggingface.co/docs/optimum/main/en/habana/usage_guides/accelerate_inference)
 
 The [export](https://huggingface.co/docs/optimum/exporters/overview) and optimizations can be done both programmatically and with a command line.
 
 ### Features summary
 
-| Features                           | ONNX Runtime       | Neural Compressor  | OpenVINO           | TensorFlow Lite    |
+| Features                           | [ONNX Runtime](https://huggingface.co/docs/optimum/main/en/onnxruntime/overview)| [Neural Compressor](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc)| [OpenVINO](https://huggingface.co/docs/optimum/main/en/intel/inference)| [TensorFlow Lite](https://huggingface.co/docs/optimum/main/en/exporters/tflite/overview)|
 |:----------------------------------:|:------------------:|:------------------:|:------------------:|:------------------:|
 | Graph optimization                 | :heavy_check_mark: | N/A                | :heavy_check_mark: | N/A                |
 | Post-training dynamic quantization | :heavy_check_mark: | :heavy_check_mark: | N/A                | :heavy_check_mark: |
 | Post-training static quantization  | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 | Quantization Aware Training (QAT)  | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 | FP16 (half precision)              | :heavy_check_mark: | N/A                | :heavy_check_mark: | :heavy_check_mark: |
 | Pruning                            | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 | Knowledge Distillation             | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 
+
+### OpenVINO
+
+This requires to install the OpenVINO extra by doing `pip install optimum[openvino,nncf]`
+
+To load a model and run inference with OpenVINO Runtime, you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class. To load a PyTorch checkpoint and convert it to the OpenVINO format on-the-fly, you can set `export=True` when loading your model.
+
+```diff
+- from transformers import AutoModelForSequenceClassification
++ from optimum.intel import OVModelForSequenceClassification
+  from transformers import AutoTokenizer, pipeline
+
+  model_id = "distilbert-base-uncased-finetuned-sst-2-english"
+  tokenizer = AutoTokenizer.from_pretrained(model_id)
+- model = AutoModelForSequenceClassification.from_pretrained(model_id)
++ model = OVModelForSequenceClassification.from_pretrained(model_id, export=True)
+  model.save_pretrained("./distilbert")
+
+  classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
+  results = classifier("He's a dreadful magician.")
+```
+
+You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/inference) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/openvino).
+
+### Neural Compressor
+
+This requires to install the Neural Compressor extra by doing `pip install optimum[neural-compressor]`
+
+Dynamic quantization can be applied on your model:
+
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
+```
+
+To load a model quantized with Intel Neural Compressor, hosted locally or on the 🤗 hub, you can do as follows :
+```python
+from optimum.intel import INCModelForSequenceClassification
+
+model_id = "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
+model = INCModelForSequenceClassification.from_pretrained(model_id)
+```
+
+You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/optimization_inc) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/neural_compressor).
+
 ### ONNX + ONNX Runtime
 
+This requires to install the ONNX Runtime extra by doing `pip install optimum[exporters,onnxruntime]`
+
 It is possible to export 🤗 Transformers models to the [ONNX](https://onnx.ai/) format and perform graph optimization as well as quantization easily:
 
 ```plain
 optimum-cli export onnx -m deepset/roberta-base-squad2 --optimize O2 roberta_base_qa_onnx
 ```
 
 The model can then be quantized using `onnxruntime`:
@@ -77,82 +164,56 @@
 
 For more information on the ONNX export, please check the [documentation](https://huggingface.co/docs/optimum/exporters/onnx/usage_guides/export_a_model).
 
 #### Run the exported model using ONNX Runtime
 
 Once the model is exported to the ONNX format, we provide Python classes enabling you to run the exported ONNX model in a seemless manner using [ONNX Runtime](https://onnxruntime.ai/) in the backend:
 
-```python
-from transformers import AutoTokenizer
-from optimum.onnxruntime import ORTModelForQuestionAnswering
-
-model_name = "roberta_base_qa_onnx"
-tokenizer = AutoTokenizer.from_pretrained(model_name)
-ort_model = ORTModelForQuestionAnswering.from_pretrained(model_name)
-
-question = "What's Optimum?"
-text = "Optimum is an awesome library everyone should use!"
-inputs = tokenizer(question, text, return_tensors="pt") 
-
-# Run with ONNX Runtime.
-outputs = ort_model(**inputs)
-
-answer_start_index = outputs.start_logits.argmax()
-answer_end_index = outputs.end_logits.argmax()
+```diff
+- from transformers import AutoModelForQuestionAnswering
++ from optimum.onnxruntime import ORTModelForQuestionAnswering
+  from transformers import AutoTokenizer, pipeline
 
-predict_answer_tokens = inputs.input_ids[0, answer_start_index : answer_end_index + 1]
-answer = tokenizer.decode(predict_answer_tokens, skip_special_tokens=True)
+  model_id = "deepset/roberta-base-squad2"
+  tokenizer = AutoTokenizer.from_pretrained(model_id)
+- model = AutoModelForQuestionAnswering.from_pretrained(model_id)
++ model = ORTModelForQuestionAnswering.from_pretrained("roberta_base_qa_onnx")
+  qa_pipe = pipeline("question-answering", model=model, tokenizer=tokenizer)
+  question = "What's Optimum?"
+  context = "Optimum is an awesome library everyone should use!"
+  results = qa_pipe(question=question, context=context)
 ```
 
 More details on how to run ONNX models with `ORTModelForXXX` classes [here](https://huggingface.co/docs/optimum/main/en/onnxruntime/usage_guides/models).
 
 ### TensorFlow Lite
 
+This requires to install the Exporters extra by doing `pip install optimum[exporters-tf]`
+
 Just as for ONNX, it is possible to export models to [TensorFlow Lite](https://www.tensorflow.org/lite) and quantize them:
 
 ```plain
 optimum-cli export tflite \
   -m deepset/roberta-base-squad2 \
   --sequence_length 384  \
   --quantize int8-dynamic roberta_tflite_model
 ```
-### OpenVINO
-
-*This requires to install the Optimum OpenVINO extra by doing `pip install optimum[openvino,nncf]`.*
-
-To load a model and run inference with [OpenVINO Runtime](https://docs.openvino.ai/latest/home.html), you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class. To load a PyTorch checkpoint and convert it to the OpenVINO format on-the-fly, you can set `export=True` when loading your model.
-
-```diff
-- from transformers import AutoModelForSequenceClassification
-+ from optimum.intel import OVModelForSequenceClassification
-  from transformers import AutoTokenizer, pipeline
-
-  model_id = "distilbert-base-uncased-finetuned-sst-2-english"
-  tokenizer = AutoTokenizer.from_pretrained(model_id)
-- model = AutoModelForSequenceClassification.from_pretrained(model_id)
-+ model = OVModelForSequenceClassification.from_pretrained(model_id, export=True)
-  model.save_pretrained("./distilbert")
-
-  classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
-  results = classifier("He's a dreadful magician.")
-```
-
-You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/inference) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/openvino).
-
 
 ## Accelerated training
 
 🤗 Optimum provides wrappers around the original 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer) to enable training on powerful hardware easily.
 We support many providers:
 
 - Habana's Gaudi processors
 - ONNX Runtime (optimized for GPUs)
 
 ### Habana
 
+This requires to install the Habana extra by doing `pip install optimum[habana]`
+
 ```diff
 - from transformers import Trainer, TrainingArguments
 + from optimum.habana import GaudiTrainer, GaudiTrainingArguments
 
   # Download a pretrained model from the Hub
   model = AutoModelForXxx.from_pretrained("bert-base-uncased")
 
@@ -209,7 +270,9 @@
   )
 
   # Use ONNX Runtime for training!
   trainer.train()
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/trainer) and in the [examples](https://github.com/huggingface/optimum/tree/main/examples/onnxruntime/training).
+
+
```

### Comparing `optimum-1.8.8/optimum/bettertransformer/__init__.py` & `optimum-1.9.0/optimum/bettertransformer/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/bettertransformer/models/__init__.py` & `optimum-1.9.0/optimum/bettertransformer/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import warnings
 
+from .attention import _llama_prepare_decoder_attention_mask
 from .decoder_models import (
     BartAttentionLayerBetterTransformer,
     BlenderbotAttentionLayerBetterTransformer,
     CodegenAttentionLayerBetterTransformer,
     GPT2AttentionLayerBetterTransformer,
     GPTJAttentionLayerBetterTransformer,
     GPTNeoAttentionLayerBetterTransformer,
     GPTNeoXAttentionLayerBetterTransformer,
+    LlamaAttentionLayerBetterTransformer,
     M2M100AttentionLayerBetterTransformer,
     MarianAttentionLayerBetterTransformer,
     OPTAttentionLayerBetterTransformer,
     PegasusAttentionLayerBetterTransformer,
     T5AttentionLayerBetterTransformer,
 )
 from .encoder_models import (
@@ -50,28 +52,30 @@
             "BartEncoderLayer": BartEncoderLayerBetterTransformer,
             "BartAttention": BartAttentionLayerBetterTransformer,
         },
         "bert": {"BertLayer": BertLayerBetterTransformer},
         "bert-generation": {"BertGenerationLayer": BertLayerBetterTransformer},
         "blenderbot": {"BlenderbotAttention": BlenderbotAttentionLayerBetterTransformer},
         "camembert": {"CamembertLayer": BertLayerBetterTransformer},
+        "blip-2": {"T5Attention": T5AttentionLayerBetterTransformer},
         "clip": {"CLIPEncoderLayer": CLIPLayerBetterTransformer},
         "codegen": {"CodeGenAttention": CodegenAttentionLayerBetterTransformer},
         "data2vec-text": {"Data2VecTextLayer": BertLayerBetterTransformer},
         "deit": {"DeiTLayer": ViTLayerBetterTransformer},
         "distilbert": {"TransformerBlock": DistilBertLayerBetterTransformer},
         "electra": {"ElectraLayer": BertLayerBetterTransformer},
         "ernie": {"ErnieLayer": BertLayerBetterTransformer},
         "fsmt": {"EncoderLayer": FSMTEncoderLayerBetterTransformer},
         "gpt2": {"GPT2Attention": GPT2AttentionLayerBetterTransformer},
         "gptj": {"GPTJAttention": GPTJAttentionLayerBetterTransformer},
         "gpt_neo": {"GPTNeoSelfAttention": GPTNeoAttentionLayerBetterTransformer},
         "gpt_neox": {"GPTNeoXAttention": GPTNeoXAttentionLayerBetterTransformer},
         "hubert": {"HubertEncoderLayer": Wav2Vec2EncoderLayerBetterTransformer},
         "layoutlm": {"LayoutLMLayer": BertLayerBetterTransformer},
+        "llama": {"LlamaAttention": LlamaAttentionLayerBetterTransformer},
         "m2m_100": {
             "M2M100EncoderLayer": MBartEncoderLayerBetterTransformer,
             "M2M100Attention": M2M100AttentionLayerBetterTransformer,
         },
         "marian": {
             "MarianEncoderLayer": BartEncoderLayerBetterTransformer,
             "MarianAttention": MarianAttentionLayerBetterTransformer,
@@ -97,24 +101,74 @@
             "Wav2Vec2EncoderLayerStableLayerNorm": Wav2Vec2EncoderLayerBetterTransformer,
         },
         "whisper": {"WhisperEncoderLayer": WhisperEncoderLayerBetterTransformer},
         "xlm-roberta": {"XLMRobertaLayer": BertLayerBetterTransformer},
         "yolos": {"YolosLayer": ViTLayerBetterTransformer},
     }
 
+    OVERWRITE_METHODS = {
+        "llama": {"LlamaModel": ("_prepare_decoder_attention_mask", _llama_prepare_decoder_attention_mask)}
+    }
+
     EXCLUDE_FROM_TRANSFORM = {
         # clip's text model uses causal attention, that is most likely not supported in BetterTransformer
         "clip": ["text_model"],
+        # blip-2's Q-former and vision model should not be identified as the last layers of the model
+        "blip-2": ["qformer.encoder.layer", "vision_model.encoder.layers"],
     }
 
     CAN_NOT_BE_SUPPORTED = {
         "deberta-v2": "DeBERTa v2 does not use a regular attention mechanism, which is not supported in PyTorch's BetterTransformer.",
         "glpn": "GLPN has a convolutional layer present in the FFN network, which is not supported in PyTorch's BetterTransformer.",
     }
 
+    NOT_REQUIRES_NESTED_TENSOR = {
+        "blenderbot",
+        "codegen",
+        "gpt2",
+        "gptj",
+        "gpt_neo",
+        "gpt_neox",
+        "llama",
+        "opt",
+        "pegasus",
+        "t5",
+    }
+
+    NOT_REQUIRES_STRICT_VALIDATION = {
+        "blenderbot",
+        "blip-2",
+        "codegen",
+        "gpt2",
+        "gptj",
+        "gpt_neo",
+        "gpt_neox",
+        "llama",
+        "opt",
+        "pegasus",
+        "t5",
+    }
+
+    REQUIRES_TORCH_20 = {
+        "blenderbot",
+        "bart",
+        "codegen",
+        "gpt2",
+        "gptj",
+        "gpt_neo",
+        "gpt_neox",
+        "llama",
+        "m2m_100",
+        "marian",
+        "mbart",
+        "opt",
+        "pegasus",
+        "t5",
+    }
+
     @staticmethod
     def cannot_support(model_type: str) -> bool:
         """
         Returns True if a given model type can not be supported by PyTorch's Better Transformer.
 
         Args:
             model_type (`str`):
@@ -138,60 +192,37 @@
         """
         Returns True if the BetterTransformer implementation for a given architecture uses nested tensors, False otherwise.
 
         Args:
             model_type (`str`):
                 The model type to check.
         """
-        if model_type in ["blenderbot", "codegen", "gpt2", "gptj", "gpt_neo", "gpt_neox", "opt", "pegasus", "t5"]:
-            return False
-        else:
-            return True
+        return model_type not in BetterTransformerManager.NOT_REQUIRES_NESTED_TENSOR
 
     @staticmethod
     def requires_strict_validation(model_type: str) -> bool:
         """
         Returns True if the architecture requires to make sure all conditions of `validate_bettertransformer` are met.
 
         Args:
             model_type (`str`):
                 The model type to check.
         """
-        if model_type in ["blenderbot", "codegen", "gpt2", "gptj", "gpt_neo", "gpt_neox", "opt", "pegasus", "t5"]:
-            return False
-        else:
-            return True
+        return model_type not in BetterTransformerManager.NOT_REQUIRES_STRICT_VALIDATION
 
     @staticmethod
     def requires_torch_20(model_type: str) -> bool:
         """
         Returns True if the architecture requires PyTorch 2.0 to be used with BetterTransformer.
 
         Args:
             model_type (`str`):
                 The model type to check.
         """
-        if model_type in [
-            "blenderbot",
-            "bart",
-            "codegen",
-            "gpt2",
-            "gptj",
-            "gpt_neo",
-            "gpt_neox",
-            "m2m_100",
-            "marian",
-            "mbart",
-            "opt",
-            "pegasus",
-            "t5",
-        ]:
-            return True
-        else:
-            return False
+        return model_type in BetterTransformerManager.REQUIRES_TORCH_20
 
 
 class warn_uncompatible_save(object):
     def __init__(self, callback):
         self.callback = callback
 
     def __enter__(self):
```

### Comparing `optimum-1.8.8/optimum/bettertransformer/models/attention.py` & `optimum-1.9.0/optimum/bettertransformer/models/attention.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple
 
 import torch
+from transformers.models.llama.modeling_llama import _expand_mask as _llama_expand_mask
+from transformers.models.llama.modeling_llama import _make_causal_mask as _llama_make_causal_mask
+from transformers.models.llama.modeling_llama import apply_rotary_pos_emb
 
 
 def raise_on_head_mask(head_mask: Optional[torch.Tensor]):
     if head_mask is not None:
         raise ValueError(
             "layer_head_mask different than None is unsupported for now with BetterTransformer, please"
             "open a PR or an issue at https://github.com/huggingface/optimum."
@@ -496,7 +499,107 @@
     # Use the `embed_dim` from the config (stored in the class) rather than `hidden_state` because `attn_output` can be
     # partitioned aross GPUs when using tensor-parallelism.
     attn_output = attn_output.reshape(bsz, tgt_len, self.embed_dim)
 
     attn_output = self.out_proj(attn_output)
 
     return attn_output, None, past_key_value
+
+
+# Adapted from transformers.models.bart.modeling_bart.BartDecoder._prepare_decoder_attention_mask
+def _llama_prepare_decoder_attention_mask(self, attention_mask, input_shape, inputs_embeds, past_key_values_length):
+    # create causal mask
+    # [bsz, seq_len] -> [bsz, 1, tgt_seq_len, src_seq_len]
+    combined_attention_mask = None
+
+    # We do not care about the attention mask in the batch size = 1 case
+    if attention_mask.size(0) > 1:
+        if input_shape[-1] > 1:
+            combined_attention_mask = _llama_make_causal_mask(
+                input_shape,
+                inputs_embeds.dtype,
+                device=inputs_embeds.device,
+                past_key_values_length=past_key_values_length,
+            )
+
+        if attention_mask is not None:
+            # [bsz, seq_len] -> [bsz, 1, tgt_seq_len, src_seq_len]
+            expanded_attn_mask = _llama_expand_mask(attention_mask, inputs_embeds.dtype, tgt_len=input_shape[-1]).to(
+                inputs_embeds.device
+            )
+
+            combined_attention_mask = (
+                expanded_attn_mask if combined_attention_mask is None else expanded_attn_mask + combined_attention_mask
+            )
+    else:
+        if input_shape[-1] > 1 and attention_mask is not None and attention_mask[0][0] == 0:
+            raise ValueError("BetterTransformer does not support padding='max_length' with a batch size of 1.")
+
+    return combined_attention_mask
+
+
+def llama_forward(
+    self,
+    hidden_states: torch.Tensor,
+    attention_mask: Optional[torch.Tensor] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    past_key_value: Optional[Tuple[torch.Tensor]] = None,
+    output_attentions: bool = False,
+    use_cache: bool = False,
+) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
+    if output_attentions is True:
+        raise ValueError("output_attentions=True can not be supported with BetterTransformer.")
+
+    bsz, q_len, _ = hidden_states.size()
+
+    query_states = self.q_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+    key_states = self.k_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+    value_states = self.v_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+
+    kv_seq_len = key_states.shape[-2]
+    if past_key_value is not None:
+        kv_seq_len += past_key_value[0].shape[-2]
+    cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
+    query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
+    # [bsz, nh, t, hd]
+
+    if past_key_value is not None:
+        # reuse k, v, self_attention
+        key_states = torch.cat([past_key_value[0], key_states], dim=2)
+        value_states = torch.cat([past_key_value[1], value_states], dim=2)
+
+    past_key_value = (key_states, value_states) if use_cache else None
+
+    if bsz == 1 or self.training:
+        # BEWARE: at this stage, attention_mask is not the same as in transformers llama
+        if query_states.shape[2] > 1:
+            attn_output = torch.nn.functional.scaled_dot_product_attention(
+                query_states, key_states, value_states, attn_mask=None, dropout_p=0.0, is_causal=True
+            )
+        else:
+            attn_output = torch.nn.functional.scaled_dot_product_attention(
+                query_states, key_states, value_states, attn_mask=None, dropout_p=0.0, is_causal=False
+            )
+    else:
+        # At this stage, **attention_mask is the same** as in transformers llama
+        if attention_mask is not None:
+            if attention_mask.size() != (bsz, 1, q_len, kv_seq_len):
+                raise ValueError(
+                    f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}, but is {attention_mask.size()}"
+                )
+
+        # This line is necessary for numerical equivalence, although I'm not sure it is useful in any way.
+        attention_mask = torch.max(attention_mask, torch.tensor(torch.finfo(attention_mask.dtype).min))
+
+        attn_output = torch.nn.functional.scaled_dot_product_attention(
+            query_states, key_states, value_states, attn_mask=attention_mask, dropout_p=0.0, is_causal=False
+        )
+
+    attn_output = attn_output.transpose(1, 2)
+    attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
+
+    attn_output = self.o_proj(attn_output)
+
+    if not output_attentions:
+        attn_weights = None
+
+    return attn_output, attn_weights, past_key_value
```

### Comparing `optimum-1.8.8/optimum/bettertransformer/models/base.py` & `optimum-1.9.0/optimum/bettertransformer/models/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/bettertransformer/models/decoder_models.py` & `optimum-1.9.0/optimum/bettertransformer/models/decoder_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,27 @@
 from transformers.models.bart.modeling_bart import BartAttention
 from transformers.models.blenderbot.modeling_blenderbot import BlenderbotAttention
 from transformers.models.codegen.modeling_codegen import CodeGenAttention
 from transformers.models.gpt2.modeling_gpt2 import GPT2Attention
 from transformers.models.gpt_neo.modeling_gpt_neo import GPTNeoSelfAttention
 from transformers.models.gpt_neox.modeling_gpt_neox import GPTNeoXAttention
 from transformers.models.gptj.modeling_gptj import GPTJAttention
+from transformers.models.llama.modeling_llama import LlamaAttention
 from transformers.models.m2m_100.modeling_m2m_100 import M2M100Attention
 from transformers.models.marian.modeling_marian import MarianAttention
 from transformers.models.opt.modeling_opt import OPTAttention
 from transformers.models.pegasus.modeling_pegasus import PegasusAttention
 from transformers.models.t5.modeling_t5 import T5Attention
 
 from .attention import (
     bart_forward,
     codegen_wrapped_scaled_dot_product,
     gpt2_wrapped_scaled_dot_product,
     gpt_neo_wrapped_scaled_dot_product,
+    llama_forward,
     opt_forward,
     t5_forward,
 )
 from .base import BetterTransformerBaseLayer
 
 
 if TYPE_CHECKING:
@@ -221,14 +223,16 @@
     def forward(self, *args, **kwargs):
         super().forward_checker()
         return opt_forward(self, *args, **kwargs)
 
 
 class T5AttentionLayerBetterTransformer(BetterTransformerBaseLayer, T5Attention, torch.nn.Module):
     def __init__(self, layer: "nn.Module", config: "PretrainedConfig"):
+        if hasattr(config, "text_config"):
+            config = config.text_config
         super().__init__(config)
 
         with torch.device("meta"):
             super(BetterTransformerBaseLayer, self).__init__(config, layer.has_relative_attention_bias)
 
         submodules = ["q", "k", "v", "o"]
         for attr in submodules:
@@ -317,7 +321,26 @@
 class PegasusAttentionLayerBetterTransformer(BetterTransformerBaseLayer, PegasusAttention, nn.Module):
     def __init__(self, layer: "nn.Module", config: "PretrainedConfig"):
         bart_bettertransformer_init(self, layer, config)
 
     def forward(self, *args, **kwargs):
         super().forward_checker()
         return bart_forward(self, *args, **kwargs)
+
+
+class LlamaAttentionLayerBetterTransformer(BetterTransformerBaseLayer, LlamaAttention, nn.Module):
+    def __init__(self, layer: "nn.Module", config: "PretrainedConfig"):
+        with torch.device("meta"):
+            super(BetterTransformerBaseLayer, self).__init__(config)
+
+        self.module_mapping = None
+        submodules = ["k_proj", "v_proj", "q_proj", "o_proj", "rotary_emb"]
+        for attr in submodules:
+            setattr(self, attr, getattr(layer, attr))
+
+        self.original_layers_mapping = {submodule: submodule for submodule in submodules}
+
+        self.supports_training = True
+
+    def forward(self, *args, **kwargs):
+        super().forward_checker()
+        return llama_forward(self, *args, **kwargs)
```

### Comparing `optimum-1.8.8/optimum/bettertransformer/models/encoder_models.py` & `optimum-1.9.0/optimum/bettertransformer/models/encoder_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -635,15 +635,15 @@
         if attn_mask is not None:
             # attention mask comes in with values 0 and -inf. we convert to torch.nn.TransformerEncoder style bool mask
             # 0->false->keep this token -inf->true->mask this token
             attn_mask = attn_mask.bool()
             attn_mask = torch.reshape(attn_mask, (attn_mask.shape[0], attn_mask.shape[-1]))
             seqlen = attn_mask.shape[1]
             lengths = torch.sum(~attn_mask, 1)
-            if not all([l == seqlen for l in lengths]):
+            if not all(l == seqlen for l in lengths):
                 x = torch._nested_tensor_from_mask(x, attn_mask)
             attn_mask = None
 
         x = torch._transformer_encoder_layer_fwd(
             x,
             self.embed_dim,
             self.num_heads,
```

### Comparing `optimum-1.8.8/optimum/bettertransformer/transformation.py` & `optimum-1.9.0/optimum/bettertransformer/transformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import logging
+import os
+import types
 from copy import deepcopy
-from typing import TYPE_CHECKING, Dict, Optional
+from typing import TYPE_CHECKING, Dict, Optional, Union
 
 import torch
 from packaging.version import parse
 
 from ..utils import check_if_pytorch_greater, is_accelerate_available, recurse_getattr, recurse_setattr
 from .models import BetterTransformerManager
 
@@ -74,14 +76,25 @@
                 "`load_in_8bit` and `BetterTransformers` are mutually exclusive",
                 " please pass a model that is not loaded in 8-bit.",
             )
 
         # replace the module if it is a transformer layer compatible with bettertransformer
         target_classes = list(BetterTransformerManager.MODEL_MAPPING[config.model_type].keys())
 
+        # We may want to override methods without having to override whole modules.
+        # For example, some methods handle the mask generation, which we do not need when using PyTorch SDPA.
+        if config.model_type in BetterTransformerManager.OVERWRITE_METHODS:
+            for class_name, method_name_and_replacement in BetterTransformerManager.OVERWRITE_METHODS[
+                config.model_type
+            ].items():
+                if module.__class__.__name__ == class_name:
+                    method_name = method_name_and_replacement[0]
+                    new_method = method_name_and_replacement[1]
+                    setattr(module, method_name, types.MethodType(new_method, module))
+
         should_replace_module = False
         for target_class in target_classes:
             should_replace_module = module.__class__.__name__ == target_class
             if should_replace_module:
                 bettertransformer_module = BetterTransformerManager.MODEL_MAPPING[config.model_type][target_class](
                     module, config
                 )
@@ -167,15 +180,19 @@
     """
 
     @check_if_pytorch_greater(
         "1.13.0",
         "Please upgrade PyTorch following https://pytorch.org/get-started/locally/ in order to use BetterTransformer.",
     )
     def transform(
-        model: torch.nn.Module, keep_original_model: bool = False, max_memory: Optional[Dict] = None, **kwargs
+        model: torch.nn.Module,
+        keep_original_model: bool = False,
+        max_memory: Optional[Dict] = None,
+        offload_dir: Optional[Union[str, os.PathLike]] = None,
+        **kwargs,
     ) -> torch.nn.Module:
         r"""
         Conversion script from `transformers` model to its BetterTransformers version
 
         Args:
             model (`torch.nn.Module`):
                 Original `transformers` model
@@ -231,17 +248,17 @@
         if keep_original_model:
             try:
                 if not check_if_pytorch_greater(2.0, "Please upgrade PyTorch to >=2.0 to use training mode"):
                     model = model.requires_grad_(False)
                 model_fast = deepcopy(model)
             except RuntimeError:
                 raise ValueError(
-                    f"The model {model.__class__.__name__} does not support `deepcopy` operation that is "
+                    f"The model {model.__class__.__name__} does not support `deepcopy` operation that is"
                     " internally used to create a copy of the original model when using"
-                    " `keep_original_model=True`. Please run the conversion with "
+                    " `keep_original_model=True`. Please run the conversion with"
                     " `keep_original_model=False` and create a new copy of the original"
                     " model somewhere else."
                 )
             model_fast = replace_to_bettertransformer(model_fast, hf_config).eval()
         else:
             model_fast = replace_to_bettertransformer(model, hf_config).eval()
             model = None
@@ -261,20 +278,20 @@
             if len(all_model_tensors) > 0:
                 # This is the case where a transformed submodule is broken into several devices:
                 # as the submodules map may differ, we need to reinfer the device map
                 bt_device_map = infer_auto_device_map(model_fast, max_memory=max_memory)
             else:
                 bt_device_map = hf_device_map
 
-            model_fast = dispatch_model(model_fast, bt_device_map)
+            model_fast = dispatch_model(model_fast, bt_device_map, offload_dir=offload_dir)
 
             # It is not recommended to have `keep_original_model=True` with a model
             # that is loaded with accelerate but just in case
             if keep_original_model:
-                model = dispatch_model(model, hf_device_map)
+                model = dispatch_model(model, hf_device_map, offload_dir=offload_dir)
 
         # See: https://github.com/pytorch/pytorch/issues/96099
         if BetterTransformerManager.requires_torch_20(model_fast.config.model_type):
             logging.warning(
                 f"For training, the BetterTransformer implementation for {model_fast.config.model_type} "
                 " architecture currently does not support padding as fused kernels do not support custom"
                 " attention masks. Beware that passing padded batched training data may result in unexpected outputs."
```

### Comparing `optimum-1.8.8/optimum/commands/__init__.py` & `optimum-1.9.0/optimum/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/base.py` & `optimum-1.9.0/optimum/commands/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/env.py` & `optimum-1.9.0/optimum/commands/env.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/export/__init__.py` & `optimum-1.9.0/optimum/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/export/base.py` & `optimum-1.9.0/optimum/commands/export/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/export/onnx.py` & `optimum-1.9.0/optimum/commands/export/onnx.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,29 @@
     )
     input_group.add_argument(
         "--audio_sequence_length",
         type=int,
         default=DEFAULT_DUMMY_SHAPES["audio_sequence_length"],
         help=f"Audio tasks only. Audio sequence length {doc_input}",
     )
+    input_group.add_argument(
+        "--point_batch_size",
+        type=int,
+        default=DEFAULT_DUMMY_SHAPES["point_batch_size"],
+        help=(
+            "For Segment Anything. It corresponds to how many segmentation masks we want the model to predict per "
+            "input point."
+        ),
+    )
+    input_group.add_argument(
+        "--nb_points_per_image",
+        type=int,
+        default=DEFAULT_DUMMY_SHAPES["nb_points_per_image"],
+        help="For Segment Anything. It corresponds to the number of points per segmentation masks.",
+    )
 
     # deprecated argument
     parser.add_argument("--for-ort", action="store_true", help=argparse.SUPPRESS)
 
 
 class ONNXExportCommand(BaseOptimumCLICommand):
     @staticmethod
@@ -194,15 +209,16 @@
 
     def run(self):
         from ...exporters.onnx.__main__ import main_export
 
         # Get the shapes to be used to generate dummy inputs
         input_shapes = {}
         for input_name in DEFAULT_DUMMY_SHAPES.keys():
-            input_shapes[input_name] = getattr(self.args, input_name)
+            if hasattr(self.args, input_name):
+                input_shapes[input_name] = getattr(self.args, input_name)
 
         main_export(
             model_name_or_path=self.args.model,
             output=self.args.output,
             task=self.args.task,
             opset=self.args.opset,
             device=self.args.device,
@@ -212,9 +228,10 @@
             no_post_process=self.args.no_post_process,
             framework=self.args.framework,
             atol=self.args.atol,
             cache_dir=self.args.cache_dir,
             trust_remote_code=self.args.trust_remote_code,
             pad_token_id=self.args.pad_token_id,
             for_ort=self.args.for_ort,
+            use_subprocess=True,
             **input_shapes,
         )
```

### Comparing `optimum-1.8.8/optimum/commands/export/tflite.py` & `optimum-1.9.0/optimum/commands/export/tflite.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/onnxruntime/__init__.py` & `optimum-1.9.0/optimum/commands/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/onnxruntime/base.py` & `optimum-1.9.0/optimum/commands/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/onnxruntime/optimize.py` & `optimum-1.9.0/optimum/commands/onnxruntime/optimize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/onnxruntime/quantize.py` & `optimum-1.9.0/optimum/commands/onnxruntime/quantize.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,13 +88,15 @@
         elif self.args.avx2:
             qconfig = AutoQuantizationConfig.avx2(is_static=False, per_channel=self.args.per_channel)
         elif self.args.avx512:
             qconfig = AutoQuantizationConfig.avx512(is_static=False, per_channel=self.args.per_channel)
         elif self.args.avx512_vnni:
             qconfig = AutoQuantizationConfig.avx512_vnni(is_static=False, per_channel=self.args.per_channel)
         elif self.args.tensorrt:
-            qconfig = AutoQuantizationConfig.tensorrt(per_channel=self.args.per_channel)
+            raise ValueError(
+                "TensorRT quantization relies on static quantization that requires calibration, which is currently not supported through optimum-cli. Please adapt Optimum static quantization examples to run static quantization for TensorRT: https://github.com/huggingface/optimum/tree/main/examples/onnxruntime/quantization"
+            )
         else:
             qconfig = ORTConfig.from_pretained(self.args.config).quantization
 
         for q in quantizers:
             q.quantize(save_dir=save_dir, quantization_config=qconfig)
```

### Comparing `optimum-1.8.8/optimum/commands/optimum_cli.py` & `optimum-1.9.0/optimum/commands/optimum_cli.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/commands/register/__init__.py` & `optimum-1.9.0/optimum/commands/register/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/configuration_utils.py` & `optimum-1.9.0/optimum/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/conftest.py` & `optimum-1.9.0/optimum/conftest.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/exporters/__init__.py` & `optimum-1.9.0/optimum/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/exporters/base.py` & `optimum-1.9.0/optimum/exporters/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/exporters/error_utils.py` & `optimum-1.9.0/optimum/exporters/error_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,7 +29,11 @@
 
 class NumberOfInputsMatchError(ValueError):
     pass
 
 
 class NumberOfOutputsMatchError(ValueError):
     pass
+
+
+class MinimumVersionError(ValueError):
+    pass
```

### Comparing `optimum-1.8.8/optimum/exporters/onnx/__init__.py` & `optimum-1.9.0/optimum/exporters/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/exporters/onnx/__main__.py` & `optimum-1.9.0/optimum/exporters/onnx/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,37 +13,42 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Entry point to the optimum.exporters.onnx command line."""
 
 import argparse
 from pathlib import Path
 
+from requests.exceptions import ConnectionError as RequestsConnectionError
 from transformers import AutoTokenizer
 from transformers.utils import is_torch_available
 
 from ...commands.export.onnx import parse_args_onnx
 from ...utils import DEFAULT_DUMMY_SHAPES, logging
 from ...utils.save_utils import maybe_save_preprocessors
 from ..error_utils import AtolError, OutputMatchError, ShapeError
 from ..tasks import TasksManager
 from .base import OnnxConfigWithPast
+from .constants import UNPICKABLE_ARCHS
 from .convert import export_models, validate_models_outputs
 from .utils import (
     get_decoder_models_for_export,
     get_encoder_decoder_models_for_export,
     get_stable_diffusion_models_for_export,
 )
 
 
 if is_torch_available():
     import torch
 
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 
+if TYPE_CHECKING:
+    from .base import OnnxConfig
+
 logger = logging.get_logger()
 logger.setLevel(logging.INFO)
 
 
 def main_export(
     model_name_or_path: str,
     output: Union[str, Path],
@@ -62,14 +67,17 @@
     subfolder: str = "",
     revision: str = "main",
     force_download: bool = False,
     local_files_only: bool = False,
     use_auth_token: Optional[Union[bool, str]] = None,
     for_ort: bool = False,
     do_validation: bool = True,
+    model_kwargs: Optional[Dict[str, Any]] = None,
+    custom_onnx_configs: Optional[Dict[str, "OnnxConfig"]] = None,
+    use_subprocess: bool = False,
     **kwargs_shapes,
 ):
     """
     Full-suite ONNX export.
 
     Args:
         > Required parameters
@@ -121,14 +129,26 @@
             Whether or not to force the (re-)download of the model weights and configuration files, overriding the
             cached versions if they exist.
         local_files_only (`Optional[bool]`, defaults to `False`):
             Whether or not to only look at local files (i.e., do not try to download the model).
         use_auth_token (`Optional[str]`, defaults to `None`):
             The token to use as HTTP bearer authorization for remote files. If `True`, will use the token generated
             when running `transformers-cli login` (stored in `~/.huggingface`).
+        model_kwargs (`Optional[Dict[str, Any]]`, defaults to `None`):
+            Experimental usage: keyword arguments to pass to the model during
+            the export. This argument should be used along the `custom_onnx_configs` argument
+            in case, for example, the model inputs/outputs are changed (for example, if
+            `model_kwargs={"output_attentions": True}` is passed).
+        custom_onnx_configs (`Optional[Dict[str, OnnxConfig]]`, defaults to `None`):
+            Experimental usage: override the default ONNX config used for the given model. This argument may be useful for advanced users that desire a finer-grained control on the export. An example is available [here](https://huggingface.co/docs/optimum/main/en/exporters/onnx/usage_guides/export_a_model).
+        use_subprocess (`bool`):
+            Do the ONNX exported model validation in subprocesses. This is especially useful when
+            exporting on CUDA device, where ORT does not release memory at inference session
+            destruction. When set to `True`, the `main_export` call should be guarded in
+            `if __name__ == "__main__":` block.
         **kwargs_shapes (`Dict`):
             Shapes to use during inference. This argument allows to override the default shapes used during the ONNX export.
 
     Example usage:
     ```python
     >>> from optimum.exporters.onnx import main_export
 
@@ -158,40 +178,46 @@
             "The --fp16 option is supported only when exporting on GPU. Please pass the option `--device cuda`."
         )
 
     # get the shapes to be used to generate dummy inputs
     input_shapes = {}
     for input_name in DEFAULT_DUMMY_SHAPES.keys():
         input_shapes[input_name] = (
-            kwargs_shapes[input_name] if input_name in input_shapes else DEFAULT_DUMMY_SHAPES[input_name]
+            kwargs_shapes[input_name] if input_name in kwargs_shapes else DEFAULT_DUMMY_SHAPES[input_name]
         )
 
     torch_dtype = None if fp16 is False else torch.float16
+
+    if task == "auto":
+        try:
+            task = TasksManager.infer_task_from_model(model_name_or_path)
+        except KeyError as e:
+            raise KeyError(
+                f"The task could not be automatically inferred. Please provide the argument --task with the relevant task from {', '.join(TasksManager.get_all_tasks())}. Detailed error: {e}"
+            )
+        except RequestsConnectionError as e:
+            raise RequestsConnectionError(
+                f"The task could not be automatically inferred as this is available only for models hosted on the Hugging Face Hub. Please provide the argument --task with the relevant task from {', '.join(TasksManager.get_all_tasks())}. Detailed error: {e}"
+            )
+
     model = TasksManager.get_model_from_task(
         task,
         model_name_or_path,
         subfolder=subfolder,
         revision=revision,
         cache_dir=cache_dir,
         use_auth_token=use_auth_token,
         local_files_only=local_files_only,
         force_download=force_download,
         trust_remote_code=trust_remote_code,
         framework=framework,
         torch_dtype=torch_dtype,
+        device=device,
     )
 
-    if task == "auto":
-        try:
-            task = TasksManager.infer_task_from_model(model_name_or_path)
-        except KeyError as e:
-            raise KeyError(
-                f"The task could not be automatically inferred. Please provide the argument --task with the task from {', '.join(TasksManager.get_all_tasks())}. Detailed error: {e}"
-            )
-
     if task != "stable-diffusion" and task + "-with-past" in TasksManager.get_supported_tasks_for_model_type(
         model.config.model_type.replace("_", "-"), "onnx"
     ):
         if original_task == "auto":  # Make -with-past the default if --task was not explicitely specified
             task = task + "-with-past"
         else:
             logger.info(
@@ -203,15 +229,21 @@
         task_non_past = task.replace("-with-past", "")
         raise ValueError(
             f"The task {task} is not compatible with the --monolith argument. Please either use"
             f" `--task {task_non_past} --monolith`, or `--task {task}` without the monolith argument."
         )
 
     if original_task == "auto":
-        logger.info(f"Automatic task detection to {task}.")
+        synonyms_for_task = sorted(TasksManager.synonyms_for_task(task))
+        if synonyms_for_task:
+            synonyms_for_task = ", ".join(synonyms_for_task)
+            possible_synonyms = f" (possible synonyms are: {synonyms_for_task})"
+        else:
+            possible_synonyms = ""
+        logger.info(f"Automatic task detection to {task}{possible_synonyms}.")
 
     if task != "stable-diffusion":
         onnx_config_constructor = TasksManager.get_exporter_config_constructor(model=model, exporter="onnx", task=task)
         onnx_config = onnx_config_constructor(model.config)
 
         needs_pad_token_id = (
             isinstance(onnx_config, OnnxConfigWithPast)
@@ -278,32 +310,39 @@
             model.config.is_encoder_decoder
             and task.startswith(
                 (
                     "text2text-generation",
                     "automatic-speech-recognition",
                     "image-to-text",
                     "feature-extraction-with-past",
+                    "visual-question-answering",
+                    "document-question-answering",
                 )
             )
             and not monolith
         ):
             models_and_onnx_configs = get_encoder_decoder_models_for_export(model, onnx_config)
         elif task.startswith("text-generation") and not monolith:
             models_and_onnx_configs = get_decoder_models_for_export(model, onnx_config)
         else:
             models_and_onnx_configs = {"model": (model, onnx_config)}
 
+    if custom_onnx_configs is not None:
+        for key, custom_onnx_config in custom_onnx_configs.items():
+            models_and_onnx_configs[key] = (models_and_onnx_configs[key][0], custom_onnx_config)
+
     _, onnx_outputs = export_models(
         models_and_onnx_configs=models_and_onnx_configs,
         opset=opset,
         output_dir=output,
         output_names=onnx_files_subpaths,
         input_shapes=input_shapes,
         device=device,
         dtype="fp16" if fp16 is True else None,
+        model_kwargs=model_kwargs,
     )
 
     if optimize == "O4" and device != "cuda":
         raise ValueError(
             "Requested O4 optimization, but this optimization requires to do the export on GPU."
             " Please pass the argument `--device cuda`."
         )
@@ -329,25 +368,36 @@
                 output, models_and_onnx_configs, onnx_files_subpaths
             )
         except Exception as e:
             raise Exception(
                 f"The post-processing of the ONNX export failed. The export can still be performed by passing the option --no-post-process. Detailed error: {e}"
             )
 
+    if task == "stable-diffusion":
+        use_subprocess = (
+            False  # TODO: fix Can't pickle local object 'get_stable_diffusion_models_for_export.<locals>.<lambda>'
+        )
+    elif model.config.model_type in UNPICKABLE_ARCHS:
+        # Pickling is bugged for nn.utils.weight_norm: https://github.com/pytorch/pytorch/issues/102983
+        # TODO: fix "Cowardly refusing to serialize non-leaf tensor" error for wav2vec2-conformer
+        use_subprocess = False
+
     if do_validation is True:
         try:
             validate_models_outputs(
                 models_and_onnx_configs=models_and_onnx_configs,
                 onnx_named_outputs=onnx_outputs,
                 atol=atol,
                 output_dir=output,
                 onnx_files_subpaths=onnx_files_subpaths,
                 input_shapes=input_shapes,
                 device=device,
                 dtype=torch_dtype,
+                use_subprocess=use_subprocess,
+                model_kwargs=model_kwargs,
             )
             logger.info(f"The ONNX export succeeded and the exported model was saved at: {output.as_posix()}")
         except ShapeError as e:
             raise e
         except AtolError as e:
             logger.warning(
                 f"The ONNX export succeeded with the warning: {e}.\n The exported model was saved at: {output.as_posix()}"
```

### Comparing `optimum-1.8.8/optimum/exporters/onnx/base.py` & `optimum-1.9.0/optimum/exporters/onnx/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,17 @@
     DummyInputGenerator,
     DummyLabelsGenerator,
     DummySeq2SeqPastKeyValuesGenerator,
     is_diffusers_available,
     logging,
 )
 from ...utils import TORCH_MINIMUM_VERSION as GLOBAL_MIN_TORCH_VERSION
+from ...utils import TRANSFORMERS_MINIMUM_VERSION as GLOBAL_MIN_TRANSFORMERS_VERSION
 from ...utils.doc import add_dynamic_docstring
-from ...utils.import_utils import is_onnx_available, is_onnxruntime_available
+from ...utils.import_utils import check_if_transformers_greater, is_onnx_available, is_onnxruntime_available
 from ..base import ExportConfig
 from .constants import ONNX_DECODER_MERGED_NAME, ONNX_DECODER_NAME, ONNX_DECODER_WITH_PAST_NAME, ONNX_ENCODER_NAME
 from .model_patcher import ModelPatcher, Seq2SeqModelPatcher
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedModel, TFPreTrainedModel
@@ -98,14 +99,17 @@
     - DUMMY_INPUT_GENERATOR_CLASSES (`Tuple[Type]`) -- A tuple of classes derived from
     [`~optimum.utils.DummyInputGenerator`] specifying how to create dummy inputs.
     - ATOL_FOR_VALIDATION (`Union[float, Dict[str, float]]`) -- A float or a dictionary mapping task names to float,
     where the float values represent the absolute tolerance value to use during model conversion validation.
     - DEFAULT_ONNX_OPSET (`int`, defaults to 11) -- The default ONNX opset to use for the ONNX export.
     - MIN_TORCH_VERSION (`packaging.version.Version`, defaults to [`~optimum.exporters.onnx.utils.TORCH_MINIMUM_VERSION`]) -- The
     minimum torch version supporting the export of the model to ONNX.
+    - MIN_TRANSFORMERS_VERSION (`packaging.version.Version`, defaults to
+    [`~optimum.exporters.onnx.utils.TRANSFORMERS_MINIMUM_VERSION`] -- The minimum transformers version supporting the
+    export of the model to ONNX. Not always up-to-date or accurate. This is more for internal use.
     - PATCHING_SPECS (`Optional[List[PatchingSpec]]`, defaults to `None`) -- Specify which operators / modules should be
     patched before performing the export, and how. This is useful when some operator is not supported in ONNX for
     instance.
 
     Args:
         config (`transformers.PretrainedConfig`):
             The model configuration.
@@ -114,33 +118,38 @@
     """
 
     NORMALIZED_CONFIG_CLASS = None
     DUMMY_INPUT_GENERATOR_CLASSES = ()
     DEFAULT_ONNX_OPSET = 11
     ATOL_FOR_VALIDATION: Union[float, Dict[str, float]] = 1e-5
     MIN_TORCH_VERSION = GLOBAL_MIN_TORCH_VERSION
+    MIN_TRANSFORMERS_VERSION = GLOBAL_MIN_TRANSFORMERS_VERSION
     PATCHING_SPECS: Optional[List["PatchingSpec"]] = None
     _TASK_TO_COMMON_OUTPUTS = {
         "audio-classification": OrderedDict({"logits": {0: "batch_size"}}),
         "audio-frame-classification": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "automatic-speech-recognition": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "audio-xvector": OrderedDict({"logits": {0: "batch_size"}, "embeddings": {0: "batch_size"}}),
-        "text-generation": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "document-question-answering": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "feature-extraction": OrderedDict({"last_hidden_state": {0: "batch_size", 1: "sequence_length"}}),
+        "fill-mask": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "image-classification": OrderedDict({"logits": {0: "batch_size"}}),
         # TODO: Is this the same thing as semantic-segmentation?
         "image-segmentation": OrderedDict(
             {
                 "logits": {0: "batch_size", 1: "num_queries"},
                 "pred_boxes": {0: "batch_size", 1: "num_queries"},
                 "pred_masks": {0: "batch_size", 1: "num_queries"},
             }
         ),
-        "masked-im": OrderedDict({"logits": {0: "batch_size"}}),
-        "fill-mask": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "image-to-text": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "mask-generation": OrderedDict({"logits": {0: "batch_size"}}),
+        "masked-im": OrderedDict(
+            {"reconstruction" if check_if_transformers_greater("4.29.0") else "logits": {0: "batch_size"}}
+        ),
         "multiple-choice": OrderedDict({"logits": {0: "batch_size", 1: "num_choices"}}),
         "object-detection": OrderedDict(
             {
                 "logits": {0: "batch_size", 1: "num_queries"},
                 "pred_boxes": {0: "batch_size", 1: "num_queries"},
             }
         ),
@@ -149,29 +158,33 @@
                 "start_logits": {0: "batch_size", 1: "sequence_length"},
                 "end_logits": {0: "batch_size", 1: "sequence_length"},
             }
         ),
         "semantic-segmentation": OrderedDict({"logits": {0: "batch_size", 1: "num_labels", 2: "height", 3: "width"}}),
         "text2text-generation": OrderedDict({"logits": {0: "batch_size", 1: "decoder_sequence_length"}}),
         "text-classification": OrderedDict({"logits": {0: "batch_size"}}),
+        "text-generation": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "token-classification": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
-        "image-to-text": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "visual-question-answering": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "zero-shot-image-classification": OrderedDict(
             {
                 "logits_per_image": {0: "image_batch_size", 1: "text_batch_size"},
                 "logits_per_text": {0: "text_batch_size", 1: "image_batch_size"},
                 "text_embeds": {0: "text_batch_size"},
                 "image_embeds": {0: "image_batch_size"},
             }
         ),
-        # TODO: enable that and verify that once OwlViTOnnxConfig can work.
-        # "zero-shot-object-detection": OrderedDict({
-        #     "logits": {0: "batch_size"},
-        #     "pred_boxes": {0: "batch_size"},
-        # }),
+        "zero-shot-object-detection": OrderedDict(
+            {
+                "logits": {0: "batch_size", 1: "num_queries"},
+                "pred_boxes": {0: "batch_size", 1: "num_queries"},
+                "text_embeds": {0: "text_batch_size"},
+                "image_embeds": {0: "image_batch_size"},
+            }
+        ),
     }
 
     def __init__(self, config: "PretrainedConfig", task: str = "feature-extraction"):
         if task not in self._TASK_TO_COMMON_OUTPUTS:
             raise ValueError(
                 f"{task} is not a supported task, supported tasks: {', '.join(self._TASK_TO_COMMON_OUTPUTS.keys())}"
             )
@@ -218,15 +231,14 @@
         return copy.deepcopy(common_outputs)
 
     def fix_dynamic_axes(
         self, model_path: "Path", device: str = "cpu", dtype: Optional[str] = None, input_shapes: Optional[Dict] = None
     ):
         """
         Fixes potential issues with dynamic axes.
-
         During the export, ONNX will infer some axes to be dynamic which are actually static. This method is called
         right after the export to fix such issues.
 
         Args:
             model_path (`Path`):
                 The path of the freshly exported ONNX model.
         """
@@ -250,51 +262,57 @@
         else:
             providers = ["CPUExecutionProvider"]
 
         session_options = SessionOptions()
         session_options.graph_optimization_level = GraphOptimizationLevel.ORT_DISABLE_ALL  # no need to optimize here
         session = InferenceSession(model_path.as_posix(), providers=providers, sess_options=session_options)
 
+        onnx_input_names = [inp.name for inp in session.get_inputs()]
+
         to_fix = []
         for output_idx, node in enumerate(session.get_outputs()):
             for idx, axis in enumerate(node.shape):
                 if isinstance(axis, str) and axis not in allowed_dynamic_axes:
                     to_fix.append((output_idx, idx))
 
         # We branch here to avoid doing an unnecessary forward pass.
         if to_fix:
             if input_shapes is None:
                 input_shapes = {}
             dummy_inputs = self.generate_dummy_inputs(framework="np", **input_shapes)
-            dummy_inputs = self.generate_dummy_inputs_for_validation(dummy_inputs)
+            dummy_inputs = self.generate_dummy_inputs_for_validation(dummy_inputs, onnx_input_names=onnx_input_names)
             onnx_inputs = {}
             for name, value in dummy_inputs.items():
                 if isinstance(value, (list, tuple)):
                     value = self.flatten_output_collection_property(name, value)
                     onnx_inputs.update(dict(value.items()))
                 else:
                     onnx_inputs[name] = value
+
             for name, value in onnx_inputs.items():
                 if value.dtype == np.float32 and dtype == "fp16":
                     onnx_inputs[name] = onnx_inputs[name].astype(np.float16)
+
             outputs = session.run(None, onnx_inputs)
             del session
 
             onnx_model = onnx.load(model_path.as_posix(), load_external_data=False)
 
             for output_idx, dim_idx in to_fix:
                 dims = onnx_model.graph.output[output_idx].type.tensor_type.shape.dim
                 dims[dim_idx].dim_value = outputs[output_idx].shape[dim_idx]
 
             onnx.save(onnx_model, model_path.as_posix())
             del onnx_model
             gc.collect()
 
-    def patch_model_for_export(self, model: Union["PreTrainedModel", "TFPreTrainedModel"]) -> ModelPatcher:
-        return ModelPatcher(self, model)
+    def patch_model_for_export(
+        self, model: Union["PreTrainedModel", "TFPreTrainedModel"], model_kwargs: Optional[Dict[str, Any]] = None
+    ) -> ModelPatcher:
+        return ModelPatcher(self, model, model_kwargs=model_kwargs)
 
     @property
     def values_override(self) -> Optional[Dict[str, Any]]:
         """
         Dictionary of keys to override in the model's config before exporting.
 
         Returns:
@@ -302,17 +320,28 @@
         """
         if hasattr(self._config, "use_cache"):
             return {"use_cache": False}
 
         return None
 
     @property
+    def is_transformers_support_available(self) -> bool:
+        """
+        Whether the installed version of Transformers allows for the ONNX export.
+
+        Returns:
+            `bool`: Whether the install version of Transformers is compatible with the model.
+
+        """
+        return check_if_transformers_greater(self.MIN_TRANSFORMERS_VERSION)
+
+    @property
     def is_torch_support_available(self) -> bool:
         """
-        The minimum PyTorch version required to export the model.
+        Whether the installed version of PyTorch allows for the ONNX export.
 
         Returns:
             `bool`: Whether the installed version of PyTorch is compatible with the model.
         """
         if is_torch_available():
             from ...utils import torch_version
 
@@ -404,24 +433,32 @@
             field (`Iterable[Any]`):
                 The structure to potentially flattened.
 
         Returns:
             `Dict[str, Any]`: Outputs with flattened structure and key mapping this new structure.
 
         """
-        return {f"{name}.{idx}": item for idx, item in enumerate(itertools.chain.from_iterable(field))}
+        if isinstance(field[0], (list, tuple)):
+            return {f"{name}.{idx}": item for idx, item in enumerate(itertools.chain.from_iterable(field))}
+        else:
+            return {f"{name}.{idx}": item for idx, item in enumerate(field)}
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+    def generate_dummy_inputs_for_validation(
+        self, reference_model_inputs: Dict[str, Any], onnx_input_names: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
         """
         Generates inputs for ONNX Runtime using the reference model inputs. Override this to run inference with seq2seq
         models which have the encoder and decoder exported as separate ONNX files.
 
         Args:
-            reference_model_inputs ([`Dict[str, Tensor]`):
+            reference_model_inputs (`Dict[str, Tensor]`):
                 Reference inputs for the model.
+            onnx_input_names (`Optional[List[str]]`, defaults to `None`):
+                Names of the actual inputs to the ONNX model. This argument may be required as an unused
+                input to the model is automatically removed by torch.onnx.export (e.g. encoder_outputs in the decoder with past)
 
         Returns:
             `Dict[str, Tensor]`: The mapping holding the kwargs to provide to the model's forward function
         """
         return reference_model_inputs
 
     def post_process_exported_models(
@@ -570,14 +607,23 @@
             dummy_inputs["attention_mask"] = DummyInputGenerator.pad_input_on_dim(
                 dummy_inputs["attention_mask"],
                 desired_length=past_length + 1,
                 dim=1,
                 dtype=dummy_inputs["attention_mask"].dtype,
             )
 
+        if self.use_past_in_inputs and self.use_cache_branch is not False and "decoder_attention_mask" in dummy_inputs:
+            past_length = dummy_inputs["past_key_values"][0][0].shape[2]
+            dummy_inputs["decoder_attention_mask"] = DummyInputGenerator.pad_input_on_dim(
+                dummy_inputs["decoder_attention_mask"],
+                desired_length=past_length + 1,
+                dim=1,
+                dtype=dummy_inputs["decoder_attention_mask"].dtype,
+            )
+
         return dummy_inputs
 
     def add_past_key_values(self, inputs_or_outputs: Dict[str, Dict[int, str]], direction: str):
         """
         Fills `input_or_outputs` mapping with past_key_values dynamic axes considering the direction.
 
         Args:
@@ -611,15 +657,17 @@
             for idx, t in enumerate(field):
                 self.flatten_past_key_values(flattened_output, name, idx, t)
         else:
             flattened_output = super().flatten_output_collection_property(name, field)
 
         return flattened_output
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+    def generate_dummy_inputs_for_validation(
+        self, reference_model_inputs: Dict[str, Any], onnx_input_names: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
         if self.is_merged is True and self.use_cache_branch is True:
             reference_model_inputs["use_cache_branch"] = DummyInputGenerator.constant_tensor(shape=[1], value=True)
         elif self.is_merged is True and self.use_cache_branch is False:
             reference_model_inputs["use_cache_branch"] = DummyInputGenerator.constant_tensor(shape=[1], value=False)
 
             # We don't support optional inputs for now, so even though the non-cache branch is used,
             # dummy past key values are necessary
@@ -760,16 +808,18 @@
 
     def flatten_past_key_values(self, flattened_output, name, idx, t):
         flattened_output[f"{name}.{idx}.decoder.key"] = t[0]
         flattened_output[f"{name}.{idx}.decoder.value"] = t[1]
         flattened_output[f"{name}.{idx}.encoder.key"] = t[2]
         flattened_output[f"{name}.{idx}.encoder.value"] = t[3]
 
-    def patch_model_for_export(self, model: Union["PreTrainedModel", "TFPreTrainedModel"]) -> ModelPatcher:
-        return Seq2SeqModelPatcher(self, model)
+    def patch_model_for_export(
+        self, model: Union["PreTrainedModel", "TFPreTrainedModel"], model_kwargs: Optional[Dict[str, Any]] = None
+    ) -> ModelPatcher:
+        return Seq2SeqModelPatcher(self, model, model_kwargs=model_kwargs)
 
     def post_process_exported_models(
         self,
         path: Path,
         models_and_onnx_configs: Dict[
             str, Tuple[Union["PreTrainedModel", "TFPreTrainedModel", "ModelMixin"], "OnnxConfig"]
         ],
@@ -813,27 +863,45 @@
             models_and_onnx_configs[ONNX_DECODER_NAME][1].use_past_in_inputs = True
 
             models_and_onnx_configs[ONNX_DECODER_WITH_PAST_NAME][1].use_cache_branch = True
             models_and_onnx_configs[ONNX_DECODER_WITH_PAST_NAME][1].is_merged = True
 
         return models_and_onnx_configs, onnx_files_subpaths
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+    def generate_dummy_inputs_for_validation(
+        self, reference_model_inputs: Dict[str, Any], onnx_input_names: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
         if self._behavior is ConfigBehavior.DECODER:
             if "decoder_input_ids" in reference_model_inputs:
                 reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
 
-            if "encoder_outputs" in reference_model_inputs:
-                if self.use_past_in_inputs is False or self.is_merged:
-                    # ONNX without past uses encoder_hidden_states even when we don't outputing them
-                    reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
-                else:
-                    # ONNX with past does not use encoder_hidden_states when we don't output them
-                    reference_model_inputs.pop("encoder_outputs")
+            if "attention_mask" in reference_model_inputs:
+                reference_model_inputs["encoder_attention_mask"] = reference_model_inputs.pop("attention_mask")
 
+            if onnx_input_names is not None:
+                if "encoder_outputs" in reference_model_inputs:
+                    if "encoder_hidden_states" in onnx_input_names:
+                        # This is typically the case for the decoder without past, and for **some**
+                        # decoder with past, e.g. t5.
+                        reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop(
+                            "encoder_outputs"
+                        )[0]
+                    else:
+                        reference_model_inputs.pop("encoder_outputs")
+            else:
+                # TODO: remove this else in optimum 2.0 and make onnx_input_names a required argument
+                if "encoder_outputs" in reference_model_inputs:
+                    if self.use_past_in_inputs is False or self.is_merged:
+                        # ONNX without past uses encoder_hidden_states even when we don't outputing them
+                        reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop(
+                            "encoder_outputs"
+                        )[0]
+                    else:
+                        # ONNX with past does not use encoder_hidden_states when we don't output them
+                        reference_model_inputs.pop("encoder_outputs")
         return super().generate_dummy_inputs_for_validation(reference_model_inputs)
 
 
 class OnnxConfigWithLoss(OnnxConfig, ABC):
     """
     Wrapper for the children classes of `optimum.exporters.onnx.OnnxConfig` to export the model through the ONNX format
     with loss in outputs and labels in the inputs. For seq-to-seq models, labels will be appended to the inputs of
@@ -917,15 +985,17 @@
             if not input_was_inserted:
                 raise RuntimeError(
                     f'Could not generate dummy input for "{input_name}". Try adding a proper dummy input generator to the model ONNX config.'
                 )
 
         return dummy_inputs
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+    def generate_dummy_inputs_for_validation(
+        self, reference_model_inputs: Dict[str, Any], onnx_input_names: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
         return self._onnx_config.generate_dummy_inputs_for_validation(reference_model_inputs)
 
     def flatten_decoder_past_key_values(self, flattened_output, name, idx, t):
         flattened_output[f"{name}.{idx}.key"] = t[0]
         flattened_output[f"{name}.{idx}.value"] = t[1]
 
     def flatten_seq2seq_past_key_values(self, flattened_output, name, idx, t):
```

### Comparing `optimum-1.8.8/optimum/exporters/onnx/config.py` & `optimum-1.9.0/optimum/exporters/onnx/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,28 +159,22 @@
         common_inputs = {}
         if self._behavior is not ConfigBehavior.DECODER:
             common_inputs["input_ids"] = {0: "batch_size", 1: "encoder_sequence_length"}
 
         common_inputs["attention_mask"] = {0: "batch_size", 1: "encoder_sequence_length"}
 
         if self._behavior is not ConfigBehavior.ENCODER:
-            # TODO: it is likely this pop() is unwanted as we then always hit
-            # https://github.com/huggingface/transformers/blob/v4.26.0/src/transformers/models/t5/modeling_t5.py#L965-L969
-            common_inputs.pop("attention_mask")
-
             if self.use_past_in_inputs:
                 # TODO: validate the axis name for attention_mask
                 # common_inputs["attention_mask"][1] = "past_encoder_sequence_length + sequence_length"
                 common_inputs["decoder_input_ids"] = {0: "batch_size"}
+                self.add_past_key_values(common_inputs, direction="inputs")
             else:
                 common_inputs["decoder_input_ids"] = {0: "batch_size", 1: "decoder_sequence_length"}
 
-            if self.use_past_in_inputs:
-                self.add_past_key_values(common_inputs, direction="inputs")
-
         if self._behavior is ConfigBehavior.DECODER:
             common_inputs["encoder_outputs"] = {0: "batch_size", 1: "encoder_sequence_length"}
 
         return common_inputs
 
     def _create_dummy_input_generator_classes(self, **kwargs) -> List["DummyInputGenerator"]:
         dummy_text_input_generator = self.DUMMY_INPUT_GENERATOR_CLASSES[0](
@@ -319,14 +313,19 @@
             if use_past and not self.is_decoder_with_past:
                 raise ValueError(
                     f"The decoder part of the encoder-decoder model is {config.decoder.model_type} which does not need "
                     "past key values."
                 )
 
             self._decoder_onnx_config = decoder_onnx_config_constructor(config.decoder, **kwargs)
+            if issubclass(decoder_onnx_config_constructor.func, OnnxSeq2SeqConfigWithPast):
+                self._decoder_onnx_config = self._decoder_onnx_config.with_behavior(
+                    self._behavior, use_past=kwargs["use_past"]
+                )
+
             self._normalized_config.DECODER_NORMALIZED_CONFIG_CLASS = self._decoder_onnx_config._normalized_config
 
             if isinstance(self._decoder_onnx_config, OnnxSeq2SeqConfigWithPast):
                 self._past_key_values_generator = (
                     DummySeq2SeqDecoderTextInputGenerator,
                     DummySeq2SeqPastKeyValuesGenerator,
                 )
@@ -355,23 +354,28 @@
     def flatten_past_key_values(self, flattened_output, name, idx, t):
         if self.is_decoder_with_past:
             return self._decoder_onnx_config.flatten_past_key_values(flattened_output, name, idx, t)
 
     def flatten_output_collection_property(self, name: str, field: Iterable[Any]) -> Dict[str, Any]:
         return self._decoder_onnx_config.flatten_output_collection_property(name, field)
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+    def generate_dummy_inputs_for_validation(
+        self, reference_model_inputs: Dict[str, Any], onnx_input_names: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
         if self._behavior is ConfigBehavior.ENCODER:
             return self._encoder_onnx_config.generate_dummy_inputs_for_validation(reference_model_inputs)
         else:
             if self._behavior is ConfigBehavior.DECODER:
                 reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
 
-                # for encoder-decoder custom models, always pass encoder_hidden_states as input
-                reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
+            if "encoder_outputs" in reference_model_inputs:
+                if "encoder_hidden_states" in onnx_input_names:
+                    reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
+                else:
+                    reference_model_inputs.pop("encoder_outputs")
 
             return self._decoder_onnx_config.generate_dummy_inputs_for_validation(reference_model_inputs)
 
     def post_process_exported_models(
         self,
         path: Path,
         models_and_onnx_configs: Dict[
```

### Comparing `optimum-1.8.8/optimum/exporters/onnx/constants.py` & `optimum-1.9.0/optimum/exporters/onnx/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,7 +16,20 @@
 # 2 GB
 EXTERNAL_DATA_FORMAT_SIZE_LIMIT = 2 * 1024 * 1024 * 1024
 
 ONNX_ENCODER_NAME = "encoder_model"
 ONNX_DECODER_NAME = "decoder_model"
 ONNX_DECODER_WITH_PAST_NAME = "decoder_with_past_model"
 ONNX_DECODER_MERGED_NAME = "decoder_model_merged"
+
+UNPICKABLE_ARCHS = [
+    "encodec",
+    "hubert",
+    "sew",
+    "sew-d",
+    "speecht5",
+    "unispeech",
+    "unispeech-sat",
+    "wav2vec2",
+    "wav2vec2-conformer",
+    "wavlm",
+]
```

### Comparing `optimum-1.8.8/optimum/exporters/onnx/convert.py` & `optimum-1.9.0/optimum/exporters/onnx/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,35 +10,37 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ONNX model check and export functions."""
 
+import multiprocessing as mp
 import os
+import traceback
 from inspect import signature
 from itertools import chain
 from pathlib import Path
-from typing import Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import onnx
 from transformers.utils import is_tf_available, is_torch_available
 
 from ...onnx.utils import _get_onnx_external_data_tensors, check_model_uses_external_data
 from ...utils import (
     TORCH_MINIMUM_VERSION,
     is_diffusers_available,
     is_torch_onnx_support_available,
     logging,
     require_numpy_strictly_lower,
 )
-from ..error_utils import AtolError, OutputMatchError, ShapeError
+from ..error_utils import AtolError, MinimumVersionError, OutputMatchError, ShapeError
 from .base import OnnxConfig
-from .utils import recursive_to_device, recursive_to_dtype
+from .utils import PickableInferenceSession, recursive_to_device, recursive_to_dtype
 
 
 if is_torch_available():
     import torch
     import torch.nn as nn
     from transformers.modeling_utils import PreTrainedModel
     from transformers.pytorch_utils import is_torch_less_than_1_11
@@ -46,14 +48,17 @@
 if is_diffusers_available():
     from diffusers import ModelMixin
 
 if is_tf_available():
     from transformers.modeling_tf_utils import TFPreTrainedModel
 
 
+mp.set_start_method("spawn", force=True)
+
+
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 class DynamicAxisNameError(ValueError):
     pass
 
 
@@ -88,14 +93,16 @@
     onnx_named_outputs: List[List[str]],
     output_dir: Path,
     atol: Optional[float] = None,
     onnx_files_subpaths: Optional[List[str]] = None,
     input_shapes: Optional[Dict] = None,
     device: str = "cpu",
     dtype: Optional["torch.dtype"] = None,
+    use_subprocess: Optional[bool] = True,
+    model_kwargs: Optional[Dict[str, Any]] = None,
 ):
     """
     Validates the export of several models, by checking that the outputs from both the reference and the exported model match.
     The following method validates the ONNX models exported using the `export_models` method.
 
     Args:
         models_and_onnx_configs (`Dict[str, Tuple[Union[`PreTrainedModel`, `TFPreTrainedModel`], `OnnxConfig`]]):
@@ -111,48 +118,59 @@
             in the ordered dict `models_and_onnx_configs`. If None, will use the keys from the `models_and_onnx_configs` as names.
         input_shapes (`Optional[Dict]`, defaults to `None`):
             If specified, allows to use specific shapes to validate the ONNX model on.
         device (`str`, defaults to `"cpu"`):
             The device on which the ONNX models will be validated. Either `cpu` or `cuda`. Validation on a CUDA device is supported only for PyTorch.
         dtype (`Optional[torch.dtype]`, defaults to `None`):
             Data type of the inputs to perform validation on. Validation on float16 is supported only for PyTorch.
-
+        use_subprocess (`Optional[bool]`, defaults to `True`):
+            Launch validation of each exported model in a subprocess.
+        model_kwargs (`Optional[Dict[str, Any]]`, defaults to `None`):
+            Experimental usage: keyword arguments to pass to the model during
+            the export and validation.
     Raises:
         ValueError: If the outputs shapes or values do not match between the reference and the exported model.
     """
     if len(onnx_named_outputs) != len(models_and_onnx_configs.keys()):
         raise ValueError(
             f"Invalid number of ONNX named outputs. Required {len(models_and_onnx_configs.keys())}, Provided {len(onnx_named_outputs)}"
         )
 
     if onnx_files_subpaths is not None and len(onnx_files_subpaths) != len(models_and_onnx_configs):
         raise ValueError(
             f"Provided custom names {onnx_files_subpaths} for the validation of {len(models_and_onnx_configs)} models. Please provide the same number of ONNX file names as models to export."
         )
 
+    if use_subprocess:
+        logger.info("Validating models in subprocesses...")
     exceptions = []  # run all validations before raising
     onnx_paths = []
     for i, model_name in enumerate(models_and_onnx_configs.keys()):
         submodel, sub_onnx_config = models_and_onnx_configs[model_name]
         onnx_model_path = (
             output_dir.joinpath(onnx_files_subpaths[i])
             if onnx_files_subpaths is not None
             else output_dir.joinpath(model_name + ".onnx")
         )
         onnx_paths.append(onnx_model_path)
         try:
+            # Model validation is done in subprocesses, as ONNX Runtime has the bad habit of
+            # not releasing memory once an InferenceSession is initialized.
+            # Reference: https://github.com/huggingface/optimum/pull/1115
             validate_model_outputs(
                 config=sub_onnx_config,
                 reference_model=submodel,
                 onnx_model=onnx_model_path,
                 onnx_named_outputs=onnx_named_outputs[i],
                 atol=atol,
                 input_shapes=input_shapes,
                 device=device,
                 dtype=dtype,
+                use_subprocess=use_subprocess,
+                model_kwargs=model_kwargs,
             )
         except Exception as e:
             exceptions.append(e)
 
     if len(exceptions) != 0:
         for i, exception in enumerate(exceptions[:-1]):
             logger.error(f"Validation {i} for the model {onnx_paths[i].as_posix()} raised: {exception}")
@@ -164,18 +182,19 @@
     reference_model: Union["PreTrainedModel", "TFPreTrainedModel", "ModelMixin"],
     onnx_model: Path,
     onnx_named_outputs: List[str],
     atol: Optional[float] = None,
     input_shapes: Optional[Dict] = None,
     device: str = "cpu",
     dtype: Optional["torch.dtype"] = None,
+    use_subprocess: Optional[bool] = True,
+    model_kwargs: Optional[Dict[str, Any]] = None,
 ):
     """
     Validates the export by checking that the outputs from both the reference and the exported model match.
-
     Args:
         config ([`~OnnxConfig`]:
             The configuration used to export the model.
         reference_model ([`~PreTrainedModel`] or [`~TFPreTrainedModel`]):
             The model used for the export.
         onnx_model (`Path`):
             The path to the exported model.
@@ -183,19 +202,60 @@
             The names of the outputs to check.
         atol (`Optional[float]`, defaults to `None`):
             The absolute tolerance in terms of outputs difference between the reference and the exported model.
         input_shapes (`Optional[Dict]`, defaults to `None`):
             If specified, allows to use specific shapes to validate the ONNX model on.
         device (`str`, defaults to `"cpu"`):
             The device on which the ONNX model will be validated. Either `cpu` or `cuda`. Validation on a CUDA device is supported only for PyTorch.
-
+        use_subprocess (`Optional[bool]`, defaults to `True`):
+            Launch validation of each exported model in a subprocess.
+        model_kwargs (`Optional[Dict[str, Any]]`, defaults to `None`):
+            Experimental usage: keyword arguments to pass to the model during
+            the export and validation.
     Raises:
         ValueError: If the outputs shapes or values do not match between the reference and the exported model.
     """
-    from onnxruntime import GraphOptimizationLevel, InferenceSession, SessionOptions
+    if use_subprocess:
+        io_process = ValidationProcess(
+            config, reference_model, onnx_model, onnx_named_outputs, atol, input_shapes, device, dtype, model_kwargs
+        )
+        io_process.start()
+        io_process.join()
+
+        if io_process.exception:
+            error, traceback = io_process.exception
+            raise error
+    else:
+        _run_validation(
+            config,
+            reference_model,
+            onnx_model,
+            onnx_named_outputs,
+            atol,
+            input_shapes,
+            device,
+            dtype,
+            model_kwargs=model_kwargs,
+        )
+
+
+def _run_validation(
+    config: OnnxConfig,
+    reference_model: Union["PreTrainedModel", "TFPreTrainedModel", "ModelMixin"],
+    onnx_model: Path,
+    onnx_named_outputs: List[str],
+    atol: Optional[float] = None,
+    input_shapes: Optional[Dict] = None,
+    device: str = "cpu",
+    dtype: Optional["torch.dtype"] = None,
+    model_kwargs: Optional[Dict[str, Any]] = None,
+):
+    from onnxruntime import GraphOptimizationLevel, SessionOptions
+
+    model_kwargs = model_kwargs if model_kwargs is not None else {}
 
     logger.info(f"Validating ONNX model {onnx_model.as_posix()}...")
 
     if atol is None:
         atol = config.ATOL_FOR_VALIDATION
 
     if "diffusers" in str(reference_model.__class__) and not is_diffusers_available():
@@ -213,15 +273,15 @@
     session_options.graph_optimization_level = GraphOptimizationLevel.ORT_ENABLE_BASIC
 
     if device.startswith("cuda"):
         provider = "CUDAExecutionProvider"
     else:
         provider = "CPUExecutionProvider"
 
-    session = InferenceSession(onnx_model.as_posix(), sess_options=session_options, providers=[provider])
+    session = PickableInferenceSession(onnx_model.as_posix(), sess_options=session_options, providers=[provider])
 
     # Sometimes the exported model can have more outputs than what is specified in the ONNX config because the original
     # PyTorch model has more outputs that were forgotten in the config, so we check for that.
     all_onnx_outputs = {output.name for output in session.get_outputs()}
     config_outputs = set(config.outputs)
     if all_onnx_outputs != config_outputs:
         if len(all_onnx_outputs) > len(config_outputs):
@@ -257,32 +317,50 @@
 
         for key, value in reference_model_inputs.items():
             reference_model_inputs[key] = recursive_to_device(value=value, device=device)
             reference_model_inputs[key] = recursive_to_dtype(
                 value=reference_model_inputs[key], dtype=dtype, start_dtype=torch.float32
             )
 
-    ref_outputs = reference_model(**reference_model_inputs)
+    if is_torch_available() and isinstance(reference_model, nn.Module):
+        with torch.inference_mode():
+            ref_outputs = reference_model(**reference_model_inputs, **model_kwargs)
+    else:
+        ref_outputs = reference_model(**reference_model_inputs, **model_kwargs)
     ref_outputs_dict = {}
 
     # We flatten potential collection of outputs (i.e. past_keys) to a flat structure
     for name, value in ref_outputs.items():
         # Overwriting the output name as "present" since it is the name used for the ONNX outputs
         # ("past_key_values" being taken for the ONNX inputs)
         if name == "past_key_values":
             name = "present"
         if isinstance(value, (list, tuple)):
-            value = config.flatten_output_collection_property(name, value)
+            onnx_output_name = config.torch_to_onnx_output_map.get(name, name)
+            value = config.flatten_output_collection_property(onnx_output_name, value)
             ref_outputs_dict.update(value)
         else:
             ref_outputs_dict[name] = value
 
+    onnx_input_names = [inp.name for inp in session.get_inputs()]
+
     # Possibly edit the input for the onnxruntime.InferenceSession, this is for example the case for merged
     # models where the input `use_cache_branch` is added
-    reference_ort_inputs = config.generate_dummy_inputs_for_validation(reference_model_inputs)
+    reference_ort_inputs = config.generate_dummy_inputs_for_validation(
+        reference_model_inputs, onnx_input_names=onnx_input_names
+    )
+
+    # generate_dummy_inputs_for_validation may add inputs (e.g. past_key_values) that are by
+    # default on torch.float32 dtype. Thus, to run validation of fp16 model, these inputs need
+    # to be casted as well.
+    if is_torch_available() and isinstance(reference_model, nn.Module):
+        for key, value in reference_ort_inputs.items():
+            reference_ort_inputs[key] = recursive_to_dtype(
+                value=reference_ort_inputs[key], dtype=dtype, start_dtype=torch.float32
+            )
 
     # We flatten potential collection of inputs (i.e. past_keys)
     onnx_inputs = {}
     for name, value in reference_ort_inputs.items():
         if isinstance(value, (list, tuple)):
             value = config.flatten_output_collection_property(name, value)
             onnx_inputs.update({tensor_name: pt_tensor.cpu().numpy() for tensor_name, pt_tensor in value.items()})
@@ -298,15 +376,15 @@
 
     # Check we have a subset of the keys into onnx_outputs against ref_outputs
     ref_outputs_set, onnx_outputs_set = set(ref_outputs_dict.keys()), set(onnx_named_outputs)
     if not onnx_outputs_set.issubset(ref_outputs_set):
         raise OutputMatchError(
             "ONNX model output names do not match reference model output names.\n"
             f"Reference model output names: {ref_outputs_set}\n"
-            f"ONNX model output names: {onnx_outputs_set}"
+            f"ONNX model output names: {onnx_outputs_set}\n"
             f"Difference: {onnx_outputs_set.difference(ref_outputs_set)}"
         )
     else:
         onnx_output_names = ", ".join(onnx_outputs_set)
         logger.info(f"\t-[✓] ONNX model output names match reference model ({onnx_output_names})")
 
     if "diffusers" in str(reference_model.__class__) and not is_diffusers_available():
@@ -349,22 +427,74 @@
     if value_failures:
         msg = "\n".join(f"- {t[0]}: max diff = {t[1]}" for t in value_failures)
         raise AtolError(
             f"The maximum absolute difference between the output of the reference model and the ONNX exported model is not within the set tolerance {atol}:\n{msg}"
         )
 
 
+class ValidationProcess(mp.Process):
+    def __init__(
+        self,
+        config: OnnxConfig,
+        reference_model: Union["PreTrainedModel", "TFPreTrainedModel", "ModelMixin"],
+        onnx_model: Path,
+        onnx_named_outputs: List[str],
+        atol: Optional[float] = None,
+        input_shapes: Optional[Dict] = None,
+        device: str = "cpu",
+        dtype: Optional["torch.dtype"] = None,
+        model_kwargs: Optional[Dict[str, Any]] = None,
+    ):
+        super().__init__()
+        self._pconn, self._cconn = mp.Pipe()
+        self._exception = None
+        self.config = config
+        self.reference_model = reference_model
+        self.onnx_model = onnx_model
+        self.onnx_named_outputs = onnx_named_outputs
+        self.atol = atol
+        self.input_shapes = input_shapes
+        self.device = device
+        self.dtype = dtype
+        self.model_kwargs = model_kwargs
+
+    def run(self):
+        try:
+            _run_validation(
+                config=self.config,
+                reference_model=self.reference_model,
+                onnx_model=self.onnx_model,
+                onnx_named_outputs=self.onnx_named_outputs,
+                atol=self.atol,
+                input_shapes=self.input_shapes,
+                device=self.device,
+                dtype=self.dtype,
+                model_kwargs=self.model_kwargs,
+            )
+        except Exception as e:
+            tb = traceback.format_exc()
+            self._cconn.send((e, tb))
+            return
+
+    @property
+    def exception(self):
+        if self._pconn.poll():
+            self._exception = self._pconn.recv()
+        return self._exception
+
+
 def export_pytorch(
     model: Union["PreTrainedModel", "ModelMixin"],
     config: OnnxConfig,
     opset: int,
     output: Path,
     device: str = "cpu",
     dtype: Optional["torch.dtype"] = None,
     input_shapes: Optional[Dict] = None,
+    model_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Tuple[List[str], List[str]]:
     """
     Exports a PyTorch model to an ONNX Intermediate Representation.
 
     Args:
         model ([`PreTrainedModel`]):
             The model to export.
@@ -377,14 +507,19 @@
         device (`str`, defaults to `"cpu"`):
             The device on which the ONNX model will be exported. Either `cpu` or `cuda`. Only PyTorch is supported for
             export on CUDA devices.
         dtype (`Optional[torch.dtype]`, defaults to `None`):
             Data type to remap the model inputs to. PyTorch-only. Only `torch.float16` is supported.
         input_shapes (`Optional[Dict]`, defaults to `None`):
             If specified, allows to use specific shapes for the example input provided to the ONNX exporter.
+        model_kwargs (`Optional[Dict[str, Any]]`, defaults to `None`):
+            Experimental usage: keyword arguments to pass to the model during
+            the export. This argument should be used along the `custom_onnx_config` argument
+            in case, for example, the model inputs/outputs are changed (for example, if
+            `model_kwargs={"output_attentions": True}` is passed).
 
     Returns:
         `Tuple[List[str], List[str]]`: A tuple with an ordered list of the model's inputs, and the named outputs from
         the ONNX configuration.
     """
     from torch.onnx import export as onnx_export
     from torch.utils._pytree import tree_map
@@ -428,15 +563,15 @@
         output_names = list(config.outputs.keys())
 
         # PyTorch deprecated the `enable_onnx_checker` and `use_external_data_format` arguments in v1.11,
         # so we check the torch version for backwards compatibility
         if is_torch_less_than_1_11:
             raise RuntimeError("The ONNX export using the PyTorch framework is only supported for v1.11+")
         else:
-            with config.patch_model_for_export(model):
+            with config.patch_model_for_export(model, model_kwargs=model_kwargs):
                 # Export can work with named args but the dict containing named args has to be the last element of the args
                 # tuple.
                 onnx_export(
                     model,
                     (dummy_inputs,),
                     f=output.as_posix(),
                     input_names=input_names,
@@ -504,20 +639,20 @@
     Returns:
         `Tuple[List[str], List[str]]`: A tuple with an ordered list of the model's inputs, and the named outputs from
         the ONNX configuration.
     """
     # This is needed to import onnx and tf2onnx because onnx is also the name of the current directory.
     import sys
 
+    import onnx
     import tensorflow as tf
+    import tf2onnx
 
     sys_path_backup = sys.path
     sys.path.pop(0)
-    import onnx
-    import tf2onnx
 
     sys.path = sys_path_backup
 
     logger.info(f"Using framework TensorFlow: {tf.__version__}")
 
     model.config.return_dict = True
 
@@ -558,14 +693,15 @@
     output_dir: Path,
     opset: Optional[int] = None,
     output_names: Optional[List[str]] = None,
     device: str = "cpu",
     input_shapes: Optional[Dict] = None,
     disable_dynamic_axes_fix: Optional[bool] = False,
     dtype: Optional[str] = None,
+    model_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Tuple[List[List[str]], List[List[str]]]:
     """
     Exports a Pytorch or TensorFlow encoder decoder model to an ONNX Intermediate Representation.
     The following method exports the encoder and decoder components of the model as separate
     ONNX files.
 
     Args:
@@ -583,14 +719,19 @@
             export on CUDA devices.
         input_shapes (`Optional[Dict]`, defaults to `None`):
             If specified, allows to use specific shapes for the example input provided to the ONNX exporter.
         disable_dynamic_axes_fix (`Optional[bool]`, defaults to `False`):
             Whether to disable the default dynamic axes fixing.
         dtype (`Optional[str]`, defaults to `None`):
             Data type to remap the model inputs to. PyTorch-only. Only `fp16` is supported.
+        model_kwargs (`Optional[Dict[str, Any]]`, defaults to `None`):
+            Experimental usage: keyword arguments to pass to the model during
+            the export. This argument should be used along the `custom_onnx_config` argument
+            in case, for example, the model inputs/outputs are changed (for example, if
+            `model_kwargs={"output_attentions": True}` is passed).
     Returns:
         `Tuple[List[List[str]], List[List[str]]]`: A tuple with an ordered list of the model's inputs, and the named
         outputs from the ONNX configuration.
     """
     outputs = []
 
     if output_names is not None and len(output_names) != len(models_and_onnx_configs):
@@ -611,14 +752,15 @@
                 config=sub_onnx_config,
                 output=output_path,
                 opset=opset,
                 device=device,
                 input_shapes=input_shapes,
                 disable_dynamic_axes_fix=disable_dynamic_axes_fix,
                 dtype=dtype,
+                model_kwargs=model_kwargs,
             )
         )
 
     outputs = list(map(list, zip(*outputs)))
     return outputs
 
 
@@ -627,14 +769,15 @@
     config: OnnxConfig,
     output: Path,
     opset: Optional[int] = None,
     device: str = "cpu",
     input_shapes: Optional[Dict] = None,
     disable_dynamic_axes_fix: Optional[bool] = False,
     dtype: Optional[str] = None,
+    model_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Tuple[List[str], List[str]]:
     """
     Exports a Pytorch or TensorFlow model to an ONNX Intermediate Representation.
 
     Args:
         model ([`PreTrainedModel`] or [`TFPreTrainedModel`]):
             The model to export.
@@ -649,14 +792,19 @@
             export on CUDA devices.
         input_shapes (`Optional[Dict]`, defaults to `None`):
             If specified, allows to use specific shapes for the example input provided to the ONNX exporter.
         disable_dynamic_axes_fix (`Optional[bool]`, defaults to `False`):
             Whether to disable the default dynamic axes fixing.
         dtype (`Optional[str]`, defaults to `None`):
             Data type to remap the model inputs to. PyTorch-only. Only `fp16` is supported.
+        model_kwargs (`Optional[Dict[str, Any]]`, defaults to `None`):
+            Experimental usage: keyword arguments to pass to the model during
+            the export. This argument should be used along the `custom_onnx_config` argument
+            in case, for example, the model inputs/outputs are changed (for example, if
+            `model_kwargs={"output_attentions": True}` is passed).
 
     Returns:
         `Tuple[List[str], List[str]]`: A tuple with an ordered list of the model's inputs, and the named outputs from
         the ONNX configuration.
     """
     if not (is_torch_available() or is_tf_available()):
         raise ImportError(
@@ -670,39 +818,58 @@
 
     if opset is None:
         opset = config.DEFAULT_ONNX_OPSET
 
     if "diffusers" in str(model.__class__) and not is_diffusers_available():
         raise ImportError("The pip package `diffusers` is required to export stable diffusion models to ONNX.")
 
+    if not config.is_transformers_support_available:
+        import transformers
+
+        raise MinimumVersionError(
+            f"The current version of Transformers does not allow for the export of the model. Minimum required is "
+            f"{config.MIN_TRANSFORMERS_VERSION}, got: {transformers.__version__}"
+        )
+
     if is_torch_available() and isinstance(model, nn.Module):
         from ...utils import torch_version
 
         if not is_torch_onnx_support_available():
-            raise AssertionError(
+            raise MinimumVersionError(
                 f"Unsupported PyTorch version, minimum required is {TORCH_MINIMUM_VERSION}, got: {torch_version}"
             )
 
         if not config.is_torch_support_available:
-            logger.warning(
+            raise MinimumVersionError(
                 f"Unsupported PyTorch version for this model. Minimum required is {config.MIN_TORCH_VERSION},"
                 f" got: {torch.__version__}"
             )
 
         torch_dtype = None
         if dtype == "fp16":
             torch_dtype = torch.float16
         elif dtype is not None:
             raise ValueError("Unsupported dtype, supported dtypes are: `torch.float16`.")
 
         export_output = export_pytorch(
-            model, config, opset, output, device=device, input_shapes=input_shapes, dtype=torch_dtype
+            model,
+            config,
+            opset,
+            output,
+            device=device,
+            input_shapes=input_shapes,
+            dtype=torch_dtype,
+            model_kwargs=model_kwargs,
         )
 
     elif is_tf_available() and issubclass(type(model), TFPreTrainedModel):
+        if model_kwargs is not None:
+            raise NotImplementedError(
+                "The argument `model_kwargs` is used only for PyTorch ONNX export, and unavailable for the Tensorflow export."
+            )
         if device == "cuda":
             raise RuntimeError("`tf2onnx` does not support export on CUDA device.")
         if input_shapes is not None:
             logger.info("`input_shapes` argument is not supported by the Tensorflow ONNX export and will be ignored.")
         export_output = export_tensorflow(model, config, opset, output)
 
     else:
```

### Comparing `optimum-1.8.8/optimum/exporters/onnx/model_configs.py` & `optimum-1.9.0/optimum/exporters/onnx/model_configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from transformers.utils import is_tf_available
 
 from ...utils import (
     DEFAULT_DUMMY_SHAPES,
     DummyAudioInputGenerator,
     DummyDecoderTextInputGenerator,
     DummyPastKeyValuesGenerator,
+    DummyPix2StructInputGenerator,
+    DummyPointsGenerator,
     DummySeq2SeqDecoderTextInputGenerator,
     DummySeq2SeqPastKeyValuesGenerator,
     DummyTextInputGenerator,
     DummyTimestepInputGenerator,
     DummyVisionInputGenerator,
     NormalizedConfig,
     NormalizedEncoderDecoderConfig,
@@ -292,27 +294,38 @@
 
 
 class T5OnnxConfig(TextSeq2SeqOnnxConfig):
     DEFAULT_ONNX_OPSET = 13
     DUMMY_INPUT_GENERATOR_CLASSES = TextSeq2SeqOnnxConfig.DUMMY_INPUT_GENERATOR_CLASSES[:-1] + (
         T5DummySeq2SeqPastKeyValuesGenerator,
     )
+    DUMMY_PKV_GENERATOR_CLASS = T5DummySeq2SeqPastKeyValuesGenerator
     NORMALIZED_CONFIG_CLASS = NormalizedSeq2SeqConfig.with_args(
         hidden_size="d_model",
         num_attention_heads="num_heads",
         encoder_num_layers="num_layers",
         decoder_num_layers="num_decoder_layers",
         key_value_dim="d_kv",
         allow_new=True,
     )
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+    def generate_dummy_inputs_for_validation(
+        self, reference_model_inputs: Dict[str, Any], onnx_input_names: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
         if self._behavior is ConfigBehavior.DECODER:
             reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
 
+        if onnx_input_names is not None:
+            if "encoder_outputs" in reference_model_inputs:
+                if "encoder_hidden_states" in onnx_input_names:
+                    reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
+                else:
+                    reference_model_inputs.pop("encoder_outputs")
+        else:
+            # TODO: remove this else in optimum 2.0 and make onnx_input_names a required argument
             # T5 requires encoder_hidden_states as an input for both the without/with past models,
             # which is different than other architectures that require it only for the without past case
             reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
 
         return super().generate_dummy_inputs_for_validation(reference_model_inputs)
 
 
@@ -533,14 +546,19 @@
     MIN_TORCH_VERSION = version.parse("1.11")
 
     @property
     def inputs(self) -> Dict[str, Dict[int, str]]:
         return {"pixel_values": {0: "batch_size", 1: "num_channels", 2: "height", 3: "width"}}
 
 
+class CvTOnnxConfig(ViTOnnxConfig):
+    DEFAULT_ONNX_OPSET = 13
+    ATOL_FOR_VALIDATION = 1e-2
+
+
 class LevitOnnxConfig(ViTOnnxConfig):
     pass
 
 
 class DeiTOnnxConfig(ViTOnnxConfig):
     pass
 
@@ -763,17 +781,33 @@
         }
 
 
 class GroupViTOnnxConfig(CLIPOnnxConfig):
     pass
 
 
-# TODO: not supported now because of aten:broadcast_to, can be most likely patched.
-# class OwlViTOnnxConfig(CLIPOnnxConfig):
-#     pass
+class OwlViTOnnxConfig(CLIPOnnxConfig):
+    # Sets the absolute tolerance to when validating the exported ONNX model against the
+    # reference model.
+    ATOL_FOR_VALIDATION = 1e-4
+    MIN_TORCH_VERSION = version.parse("2.1")
+
+    @property
+    def outputs(self) -> Dict[str, Dict[int, str]]:
+        outputs = {}
+        if self.task == "feature-extraction":
+            outputs["logits_per_image"] = {0: "image_batch_size", 1: "text_batch_size"}
+            outputs["logits_per_text"] = {0: "text_batch_size", 1: "image_batch_size"}
+        elif self.task == "zero-shot-object-detection":
+            outputs["logits"] = {0: "batch_size", 1: "num_queries"}
+            outputs["pred_boxes"] = {0: "batch_size", 1: "num_queries"}
+
+        outputs["text_embeds"] = {0: "text_batch_size"}
+        outputs["image_embeds"] = {0: "image_batch_size"}
+        return outputs
 
 
 class LayoutLMOnnxConfig(TextAndVisionOnnxConfig):
     NORMALIZED_CONFIG_CLASS = NormalizedTextConfig.with_args(
         allow_new=True,
         MAX_2D_POSITION_EMBEDDINGS="max_2d_position_embeddings",
     )
@@ -807,14 +841,29 @@
             "input_ids": {0: "batch_size", 1: "sequence_length"},
             "attention_mask": {0: "batch_size", 1: "sequence_length"},
             "bbox": {0: "batch_size", 1: "sequence_length"},
             "pixel_values": pixel_values_dynamic_axes,
         }
 
 
+class LiltOnnxConfig(TextAndVisionOnnxConfig):
+    NORMALIZED_CONFIG_CLASS = NormalizedTextConfig.with_args(
+        allow_new=True,
+        MAX_2D_POSITION_EMBEDDINGS="max_2d_position_embeddings",
+    )
+
+    @property
+    def inputs(self) -> Dict[str, Dict[int, str]]:
+        return {
+            "input_ids": {0: "batch_size", 1: "sequence_length"},
+            "bbox": {0: "batch_size", 1: "sequence_length"},
+            "attention_mask": {0: "batch_size", 1: "sequence_length"},
+        }
+
+
 class Data2VecTextOnnxConfig(DistilBertOnnxConfig):
     pass
 
 
 class Data2VecVisionOnnxConfig(ViTOnnxConfig):
     pass
 
@@ -903,16 +952,18 @@
 
 class WavLMOnnxConfig(HubertOnnxConfig):
     DEFAULT_ONNX_OPSET = 12
 
     # we need to set output_attentions=True in the model input to avoid calling
     # torch.nn.functional.scaled_dot_product_attention that is not supported by the ONNX export
     # due to the op torch.nn.functional.multi_head_attention_forward used for WavLM
-    def patch_model_for_export(self, model: Union["PreTrainedModel", "TFPreTrainedModel"]) -> "ModelPatcher":
-        return WavLMModelPatcher(self, model)
+    def patch_model_for_export(
+        self, model: Union["PreTrainedModel", "TFPreTrainedModel"], model_kwargs: Optional[Dict[str, Any]] = None
+    ) -> "ModelPatcher":
+        return WavLMModelPatcher(self, model, model_kwargs=model_kwargs)
 
 
 class ASTDummyAudioInputGenerator(DummyAudioInputGenerator):
     def generate(self, input_name: str, framework: str = "pt"):
         shape = [self.batch_size, self.normalized_config.max_length, self.normalized_config.num_mel_bins]
         if input_name == "input_values":
             return self.random_float_tensor(shape, min_value=-1, max_value=1, framework=framework)
@@ -1009,29 +1060,29 @@
 
             if self.use_past_in_inputs:
                 self.add_past_key_values(common_inputs, direction="inputs")
 
         if self._behavior is ConfigBehavior.DECODER:
             common_inputs["encoder_outputs"] = {
                 0: "batch_size",
-                1: f"encoder_sequence_length / {( 2 * self._config.num_conv_layers)}",
+                1: f"encoder_sequence_length / {(2 * self._config.num_conv_layers)}",
             }
 
         return common_inputs
 
     @property
     def outputs(self) -> Dict[str, Dict[int, str]]:
         common_outputs = super().outputs
         if self._behavior is ConfigBehavior.ENCODER:
             # for Speech2text, we need to name the second axis as
             # encoder_sequence_length / 2 * self._config.num_conv_layers as the axis name is
             # used for dummy input generation
             common_outputs["last_hidden_state"][
                 1
-            ] = f"{common_outputs['last_hidden_state'][1]} / {( 2 * self._config.num_conv_layers)}"
+            ] = f"{common_outputs['last_hidden_state'][1]} / {(2 * self._config.num_conv_layers)}"
         return common_outputs
 
 
 # TODO: Replace the TextSeq2SeqOnnxConfig inheritance with VisionToTextOnnxConfig when added.
 # The change below however does not affect the export for the model
 class TrOCROnnxConfig(TextSeq2SeqOnnxConfig):
     NORMALIZED_CONFIG_CLASS = NormalizedSeq2SeqConfig.with_args(
@@ -1081,7 +1132,111 @@
 
             if self.use_past_in_inputs:
                 self.add_past_key_values(common_inputs, direction="inputs")
         if self._behavior is ConfigBehavior.DECODER:
             common_inputs["encoder_outputs"] = {0: "batch_size", 1: "encoder_sequence_length"}
 
         return common_inputs
+
+
+class SamOnnxConfig(OnnxConfig):
+    MIN_TRANSFORMERS_VERSION = version.parse("4.29.0.dev0")
+    NORMALIZED_CONFIG_CLASS = NormalizedEncoderDecoderConfig
+    DUMMY_INPUT_GENERATOR_CLASSES = (DummyVisionInputGenerator, DummyPointsGenerator)
+    DEFAULT_ONNX_OPSET = 12  # einsum op not supported with opset 11
+
+    def __init__(self, config: "PretrainedConfig", task: str = "feature-extraction"):
+        super().__init__(config, task)
+        self._normalized_config.ENCODER_NORMALIZED_CONFIG_CLASS = NormalizedVisionConfig(self._config.vision_config)
+
+    @property
+    def inputs(self) -> Dict[str, Dict[int, str]]:
+        inputs = {
+            "pixel_values": {0: "batch_size"},
+            "input_points": {0: "batch_size", 1: "point_batch_size", 2: "nb_points_per_image"},
+        }
+
+        return inputs
+
+    @property
+    def outputs(self) -> Dict[str, Dict[int, str]]:
+        outputs = {
+            "iou_scores": {0: "batch_size", 1: "point_batch_size"},
+            "pred_masks": {0: "batch_size", 1: "point_batch_size"},
+        }
+
+        return outputs
+
+
+class Pix2StructNormalizedConfig(NormalizedSeq2SeqConfig):
+    ENCODER_NUM_LAYERS = "vision_config.num_hidden_layers"
+    DECODER_NUM_LAYERS = "text_config.num_layers"
+    ENCODER_NUM_ATTENTION_HEADS = "vision_config.num_attention_heads"
+    DECODER_NUM_ATTENTION_HEADS = "text_config.num_heads"
+    HIDDEN_SIZE = "text_config.hidden_size"  # TODO: Isn't this bug prone?
+    VOCAB_SIZE = "text_config.vocab_size"
+
+
+class Pix2StructOnnxConfig(OnnxSeq2SeqConfigWithPast):
+    NORMALIZED_CONFIG_CLASS = Pix2StructNormalizedConfig
+    DUMMY_INPUT_GENERATOR_CLASSES = (
+        DummyTextInputGenerator,
+        DummySeq2SeqDecoderTextInputGenerator,
+        DummySeq2SeqPastKeyValuesGenerator,
+        DummyPix2StructInputGenerator,
+    )
+    # Min operator needs to support int64, which is the case for opset>=12
+    DEFAULT_ONNX_OPSET = 12
+
+    @property
+    def inputs(self):
+        common_inputs = {}
+        common_inputs["attention_mask"] = {0: "batch_size", 1: "max_patches"}
+
+        if self._behavior is not ConfigBehavior.DECODER:
+            common_inputs["flattened_patches"] = {0: "batch_size", 1: "max_patches", 2: "patch_size"}
+
+        if self._behavior is not ConfigBehavior.ENCODER:
+            if self.use_past_in_inputs:
+                common_inputs["decoder_input_ids"] = {0: "batch_size"}
+            else:
+                common_inputs["decoder_input_ids"] = {0: "batch_size", 1: "decoder_sequence_length"}
+
+        if self._behavior is ConfigBehavior.DECODER:
+            if self.use_past_in_inputs:
+                self.add_past_key_values(common_inputs, direction="inputs")
+
+            common_inputs["encoder_outputs"] = {0: "batch_size", 1: "max_patches"}
+
+            common_inputs["decoder_attention_mask"] = {0: "batch_size", 1: "past_sequence_length + 1"}
+
+        return common_inputs
+
+    @property
+    def torch_to_onnx_input_map(self) -> Dict[str, str]:
+        if self._behavior is ConfigBehavior.DECODER:
+            return {
+                "decoder_input_ids": "input_ids",
+                "encoder_outputs": "encoder_hidden_states",
+                "attention_mask": "encoder_attention_mask",
+            }
+        return {}
+
+    def generate_dummy_inputs_for_validation(
+        self, reference_model_inputs: Dict[str, Any], onnx_input_names: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
+        if self._behavior is ConfigBehavior.DECODER:
+            reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
+
+        if onnx_input_names is not None:
+            if "encoder_outputs" in reference_model_inputs:
+                if "encoder_hidden_states" in onnx_input_names:
+                    reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
+                else:
+                    reference_model_inputs.pop("encoder_outputs")
+        else:
+            # TODO: remove this else in optimum 2.0 and make onnx_input_names a required argument
+            # Pix2Struct requires encoder_hidden_states as an input for both the without/with past models,
+            # which is different than other architectures that require it only for the without past case
+            reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
+
+        return super().generate_dummy_inputs_for_validation(reference_model_inputs)
```

### Comparing `optimum-1.8.8/optimum/exporters/onnx/utils.py` & `optimum-1.9.0/optimum/exporters/onnx/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -272,7 +272,36 @@
         for i, val in enumerate(value):
             value[i] = recursive_to_dtype(val, dtype)
     elif isinstance(value, torch.Tensor):
         if start_dtype is None or (start_dtype is not None and value.dtype == start_dtype):
             value = value.to(dtype=dtype)
 
     return value
+
+
+# Copied from https://github.com/microsoft/onnxruntime/issues/7846#issuecomment-850217402
+class PickableInferenceSession:  # This is a wrapper to make the current InferenceSession class pickable.
+    def __init__(self, model_path, sess_options, providers):
+        import onnxruntime as ort
+
+        self.model_path = model_path
+        self.sess_options = sess_options
+        self.providers = providers
+        self.sess = ort.InferenceSession(self.model_path, sess_options=sess_options, providers=providers)
+
+    def run(self, *args):
+        return self.sess.run(*args)
+
+    def get_outputs(self):
+        return self.sess.get_outputs()
+
+    def get_inputs(self):
+        return self.sess.get_inputs()
+
+    def __getstate__(self):
+        return {"model_path": self.model_path}
+
+    def __setstate__(self, values):
+        import onnxruntime as ort
+
+        self.model_path = values["model_path"]
+        self.sess = ort.InferenceSession(self.model_path, sess_options=self.sess_options, providers=self.providers)
```

### Comparing `optimum-1.8.8/optimum/exporters/tasks.py` & `optimum-1.9.0/optimum/exporters/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,38 +16,39 @@
 
 import importlib
 import inspect
 import itertools
 import os
 from functools import partial
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
 import huggingface_hub
+from packaging import version
+from requests.exceptions import ConnectionError as RequestsConnectionError
 from transformers import AutoConfig, PretrainedConfig, is_tf_available, is_torch_available
-from transformers.utils import TF2_WEIGHTS_NAME, WEIGHTS_NAME, logging
+from transformers.utils import SAFE_WEIGHTS_NAME, TF2_WEIGHTS_NAME, WEIGHTS_NAME, logging
 
 from ..utils.import_utils import is_onnx_available
 
 
 if TYPE_CHECKING:
-    import torch
-
     from .base import ExportConfig
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 if not is_torch_available() and not is_tf_available():
     logger.warning(
         "The export tasks are only supported for PyTorch or TensorFlow. You will not be able to export models"
         " without one of these libraries installed."
     )
 
 if is_torch_available():
+    import torch
     from transformers import PreTrainedModel
 
 if is_tf_available():
     from transformers import TFPreTrainedModel
 
 ExportConfigConstructor = Callable[[PretrainedConfig], "ExportConfig"]
 TaskNameToExportConfigDict = Dict[str, ExportConfigConstructor]
@@ -140,41 +141,47 @@
 
     _TASKS_TO_AUTOMODELS = {}
     _TASKS_TO_TF_AUTOMODELS = {}
     if is_torch_available():
         # Refer to https://huggingface.co/datasets/huggingface/transformers-metadata/blob/main/pipeline_tags.json
         # In case the same task (pipeline tag) may map to several loading classes, we use a tuple and the
         # auto-class _model_mapping to determine the right one.
+
+        # TODO: having several tasks pointing to the same auto-model class is bug prone to auto-detect the
+        # task in a Hub repo that has no pipeline_tag, and no transformersInfo.pipeline_tag, as we then rely on
+        # on transformersInfo["auto_model"] and this dictionary.
         _TASKS_TO_AUTOMODELS = {
             "conversational": ("AutoModelForCausalLM", "AutoModelForSeq2SeqLM"),
             "feature-extraction": "AutoModel",
             "fill-mask": "AutoModelForMaskedLM",
             "text-generation": "AutoModelForCausalLM",
             "text2text-generation": "AutoModelForSeq2SeqLM",
             "text-classification": "AutoModelForSequenceClassification",
             "token-classification": "AutoModelForTokenClassification",
             "multiple-choice": "AutoModelForMultipleChoice",
             "object-detection": "AutoModelForObjectDetection",
             "question-answering": "AutoModelForQuestionAnswering",
             "image-classification": "AutoModelForImageClassification",
             "image-segmentation": "AutoModelForImageSegmentation",
+            "mask-generation": "AutoModel",
             "masked-im": "AutoModelForMaskedImageModeling",
             "semantic-segmentation": "AutoModelForSemanticSegmentation",
             "automatic-speech-recognition": ("AutoModelForSpeechSeq2Seq", "AutoModelForCTC"),
             "audio-classification": "AutoModelForAudioClassification",
             "audio-frame-classification": "AutoModelForAudioFrameClassification",
             "audio-xvector": "AutoModelForAudioXVector",
             "image-to-text": "AutoModelForVision2Seq",
             "stable-diffusion": "StableDiffusionPipeline",
             "zero-shot-image-classification": "AutoModelForZeroShotImageClassification",
             "zero-shot-object-detection": "AutoModelForZeroShotObjectDetection",
         }
     if is_tf_available():
         _TASKS_TO_TF_AUTOMODELS = {
             "conversational": ("TFAutoModelForCausalLM", "TFAutoModelForSeq2SeqLM"),
+            "document-question-answering": "TFAutoModelForDocumentQuestionAnswering",
             "feature-extraction": "TFAutoModel",
             "fill-mask": "TFAutoModelForMaskedLM",
             "text-generation": "TFAutoModelForCausalLM",
             "image-classification": "TFAutoModelForImageClassification",
             "text2text-generation": "TFAutoModelForSeq2SeqLM",
             "text-classification": "TFAutoModelForSequenceClassification",
             "token-classification": "TFAutoModelForTokenClassification",
@@ -198,55 +205,64 @@
         "causal-lm": "text-generation",
         "causal-lm-with-past": "text-generation-with-past",
         "seq2seq-lm": "text2text-generation",
         "seq2seq-lm-with-past": "text2text-generation-with-past",
         "speech2seq-lm": "automatic-speech-recognition",
         "speech2seq-lm-with-past": "automatic-speech-recognition-with-past",
         "masked-lm": "fill-mask",
+        "mask-generation": "feature-extraction",
         "vision2seq-lm": "image-to-text",
         "default": "feature-extraction",
         "default-with-past": "feature-extraction-with-past",
         "audio-ctc": "automatic-speech-recognition",
         "translation": "text2text-generation",
+        "sentence-similarity": "feature-extraction",
         "summarization": "text2text-generation",
         "zero-shot-classification": "text-classification",
     }
 
     # Reverse dictionaries str -> str, where several automodels may map to the same task
     _AUTOMODELS_TO_TASKS = get_automodels_to_tasks(_TASKS_TO_AUTOMODELS)
     _TF_AUTOMODELS_TO_TASKS = get_automodels_to_tasks(_TASKS_TO_TF_AUTOMODELS)
 
     _CUSTOM_CLASSES = {
         ("pt", "pix2struct", "image-to-text"): ("transformers", "Pix2StructForConditionalGeneration"),
+        ("pt", "pix2struct", "visual-question-answering"): ("transformers", "Pix2StructForConditionalGeneration"),
         ("pt", "visual-bert", "question-answering"): ("transformers", "VisualBertForQuestionAnswering"),
+        # VisionEncoderDecoderModel is not registered in AutoModelForDocumentQuestionAnswering
+        ("pt", "vision-encoder-decoder", "document-question-answering"): ("transformers", "VisionEncoderDecoderModel"),
     }
 
     _TASKS_TO_LIBRARY = {
         "conversational": "transformers",
+        "document-question-answering": "transformers",
         "feature-extraction": "transformers",
         "fill-mask": "transformers",
         "text-generation": "transformers",
         "text2text-generation": "transformers",
         "text-classification": "transformers",
         "token-classification": "transformers",
         "translation": "transformers",
         "multiple-choice": "transformers",
         "object-detection": "transformers",
         "question-answering": "transformers",
         "image-classification": "transformers",
         "image-segmentation": "transformers",
+        "mask-generation": "transformers",
         "masked-im": "transformers",
         "semantic-segmentation": "transformers",
         "automatic-speech-recognition": "transformers",
         "audio-classification": "transformers",
         "audio-frame-classification": "transformers",
         "audio-xvector": "transformers",
         "image-to-text": "transformers",
+        "sentence-similarity": "transformers",
         "stable-diffusion": "diffusers",
         "summarization": "transformers",
+        "visual-question-answering": "transformers",
         "zero-shot-classification": "transformers",
         "zero-shot-image-classification": "transformers",
         "zero-shot-object-detection": "transformers",
     }
 
     # TODO: some models here support text-generation export but are not supported in ORTModelForCausalLM
     # Set of model topologies we support associated to the tasks supported by each topology and the factory
@@ -382,14 +398,15 @@
             tflite="ConvBertTFLiteConfig",
         ),
         "convnext": supported_tasks_mapping(
             "feature-extraction",
             "image-classification",
             onnx="ConvNextOnnxConfig",
         ),
+        "cvt": supported_tasks_mapping("feature-extraction", "image-classification", onnx="CvTOnnxConfig"),
         "data2vec-text": supported_tasks_mapping(
             "feature-extraction",
             "fill-mask",
             "text-classification",
             "multiple-choice",
             "token-classification",
             "question-answering",
@@ -548,14 +565,21 @@
         "layoutlmv3": supported_tasks_mapping(
             "feature-extraction",
             "question-answering",
             "text-classification",
             "token-classification",
             onnx="LayoutLMv3OnnxConfig",
         ),
+        "lilt": supported_tasks_mapping(
+            "feature-extraction",
+            "question-answering",
+            "text-classification",
+            "token-classification",
+            onnx="LiltOnnxConfig",
+        ),
         "levit": supported_tasks_mapping("feature-extraction", "image-classification", onnx="LevitOnnxConfig"),
         "longt5": supported_tasks_mapping(
             "feature-extraction",
             "feature-extraction-with-past",
             "text2text-generation",
             "text2text-generation-with-past",
             onnx="LongT5OnnxConfig",
@@ -649,20 +673,19 @@
             "fill-mask",
             "multiple-choice",
             "question-answering",
             "text-classification",
             "token-classification",
             onnx="NystromformerOnnxConfig",
         ),
-        # TODO: owlvit cannot be exported yet, check model_config.py to know why.
-        # "owlvit": supported_tasks_mapping(
-        #     "feature-extraction",
-        #     "zero-shot-object-detection",
-        #     onnx="OwlViTOnnxConfig",
-        # ),
+        "owlvit": supported_tasks_mapping(
+            "feature-extraction",
+            "zero-shot-object-detection",
+            onnx="OwlViTOnnxConfig",
+        ),
         "opt": supported_tasks_mapping(
             "feature-extraction",
             "feature-extraction-with-past",
             "text-generation",
             "text-generation-with-past",
             "question-answering",
             "text-classification",
@@ -687,14 +710,21 @@
         ),
         "perceiver": supported_tasks_mapping(
             "fill-mask",
             "image-classification",
             "text-classification",
             onnx="PerceiverOnnxConfig",
         ),
+        "pix2struct": supported_tasks_mapping(
+            "image-to-text",
+            "image-to-text-with-past",
+            "visual-question-answering",
+            "visual-question-answering-with-past",
+            onnx="Pix2StructOnnxConfig",
+        ),
         "poolformer": supported_tasks_mapping(
             "feature-extraction",
             "image-classification",
             onnx="PoolFormerOnnxConfig",
         ),
         "regnet": supported_tasks_mapping(
             "feature-extraction",
@@ -725,14 +755,18 @@
             "token-classification",
             "multiple-choice",
             "question-answering",
             "token-classification",
             onnx="RoFormerOnnxConfig",
             tflite="RoFormerTFLiteConfig",
         ),
+        "sam": supported_tasks_mapping(
+            "mask-generation",
+            onnx="SamOnnxConfig",
+        ),
         "segformer": supported_tasks_mapping(
             "feature-extraction",
             "image-classification",
             "semantic-segmentation",
             onnx="SegformerOnnxConfig",
         ),
         "sew": supported_tasks_mapping(
@@ -813,14 +847,16 @@
         "vae-decoder": supported_tasks_mapping(
             "semantic-segmentation",
             onnx="VaeDecoderOnnxConfig",
         ),
         "vision-encoder-decoder": supported_tasks_mapping(
             "image-to-text",
             "image-to-text-with-past",
+            "document-question-answering",
+            "document-question-answering-with-past",
             onnx="VisionEncoderDecoderOnnxConfig",
         ),
         "vit": supported_tasks_mapping(
             "feature-extraction", "image-classification", "masked-im", onnx="ViTOnnxConfig"
         ),
         "wavlm": supported_tasks_mapping(
             "feature-extraction",
@@ -978,14 +1014,25 @@
         return [
             model_type.replace("-", "_")
             for model_type in TasksManager._SUPPORTED_MODEL_TYPE
             if task in TasksManager._SUPPORTED_MODEL_TYPE[model_type][exporter]
         ]
 
     @staticmethod
+    def synonyms_for_task(task: str) -> Set[str]:
+        synonyms = [k for k, v in TasksManager._SYNONYM_TASK_MAP.items() if v == task]
+        synonyms += [k for k, v in TasksManager._SYNONYM_TASK_MAP.items() if v == TasksManager.map_from_synonym(task)]
+        synonyms = set(synonyms)
+        try:
+            synonyms.remove(task)
+        except KeyError:
+            pass
+        return synonyms
+
+    @staticmethod
     def map_from_synonym(task: str) -> str:
         if task in TasksManager._SYNONYM_TASK_MAP:
             task = TasksManager._SYNONYM_TASK_MAP[task]
         return task
 
     @staticmethod
     def _validate_framework_choice(framework: str):
@@ -1082,23 +1129,26 @@
                             "For library other than transformers, the _TASKS_TO_AUTOMODELS mapping should be one to one."
                         )
 
             return getattr(loaded_library, model_class_name)
 
     @staticmethod
     def determine_framework(
-        model_name_or_path: Union[str, Path], subfolder: str = "", framework: Optional[str] = None
+        model_name_or_path: Union[str, Path],
+        subfolder: str = "",
+        framework: Optional[str] = None,
+        cache_dir: str = huggingface_hub.constants.HUGGINGFACE_HUB_CACHE,
     ) -> str:
         """
         Determines the framework to use for the export.
 
         The priority is in the following order:
             1. User input via `framework`.
             2. If local checkpoint is provided, use the same framework as the checkpoint.
-            3. If model repo, try to infer the framework from the Hub.
+            3. If model repo, try to infer the framework from the cache if available, else from the Hub.
             4. If could not infer, use available framework in environment, with priority given to PyTorch.
 
         Args:
             model_name_or_path (`Union[str, Path]`):
                 Can be either the model id of a model repo on the Hugging Face Hub, or a path to a local directory
                 containing a model.
             subfolder (`str`, *optional*, defaults to `""`):
@@ -1110,49 +1160,79 @@
         Returns:
             `str`: The framework to use for the export.
 
         """
         if framework is not None:
             return framework
 
+        request_exception = None
         full_model_path = Path(model_name_or_path) / subfolder
         if full_model_path.is_dir():
             all_files = [
                 os.path.relpath(os.path.join(dirpath, file), full_model_path)
                 for dirpath, _, filenames in os.walk(full_model_path)
                 for file in filenames
             ]
         else:
-            if not isinstance(model_name_or_path, str):
-                model_name_or_path = str(model_name_or_path)
-            all_files = huggingface_hub.list_repo_files(model_name_or_path, repo_type="model")
-            if subfolder != "":
-                all_files = [file[len(subfolder) + 1 :] for file in all_files if file.startswith(subfolder)]
-
-        weight_name = Path(WEIGHTS_NAME).stem
-        weight_extension = Path(WEIGHTS_NAME).suffix
-        is_pt_weight_file = [file.startswith(weight_name) and file.endswith(weight_extension) for file in all_files]
+            try:
+                if not isinstance(model_name_or_path, str):
+                    model_name_or_path = str(model_name_or_path)
+                all_files = huggingface_hub.list_repo_files(model_name_or_path, repo_type="model")
+                if subfolder != "":
+                    all_files = [file[len(subfolder) + 1 :] for file in all_files if file.startswith(subfolder)]
+            except RequestsConnectionError as e:  # Hub not accessible
+                request_exception = e
+                object_id = model_name_or_path.replace("/", "--")
+                full_model_path = Path(cache_dir, f"models--{object_id}")
+                if full_model_path.is_dir():  # explore the cache first
+                    # Resolve refs (for instance to convert main to the associated commit sha)
+                    revision_file = Path(full_model_path, "refs", "main")
+                    revision = ""
+                    if revision_file.is_file():
+                        with open(revision_file) as f:
+                            revision = f.read()
+                    cached_path = Path(full_model_path, "snapshots", revision, subfolder)
+                    all_files = [
+                        os.path.relpath(os.path.join(dirpath, file), cached_path)
+                        for dirpath, _, filenames in os.walk(cached_path)
+                        for file in filenames
+                    ]
+
+        pt_weight_name = Path(WEIGHTS_NAME).stem
+        pt_weight_extension = Path(WEIGHTS_NAME).suffix
+        safe_weight_name = Path(SAFE_WEIGHTS_NAME).stem
+        safe_weight_extension = Path(SAFE_WEIGHTS_NAME).suffix
+        is_pt_weight_file = [
+            (file.startswith(pt_weight_name) and file.endswith(pt_weight_extension))
+            or (file.startswith(safe_weight_name) and file.endswith(safe_weight_extension))
+            for file in all_files
+        ]
 
         weight_name = Path(TF2_WEIGHTS_NAME).stem
         weight_extension = Path(TF2_WEIGHTS_NAME).suffix
         is_tf_weight_file = [file.startswith(weight_name) and file.endswith(weight_extension) for file in all_files]
 
         if any(is_pt_weight_file):
             framework = "pt"
         elif any(is_tf_weight_file):
             framework = "tf"
         elif "model_index.json" in all_files and any(file.endswith(Path(WEIGHTS_NAME).suffix) for file in all_files):
             # stable diffusion case
             framework = "pt"
         else:
-            raise FileNotFoundError(
-                "Cannot determine framework from given checkpoint location."
-                f" There should be a {Path(WEIGHTS_NAME).stem}*{Path(WEIGHTS_NAME).suffix} for PyTorch"
-                f" or {Path(TF2_WEIGHTS_NAME).stem}*{Path(TF2_WEIGHTS_NAME).suffix} for TensorFlow."
-            )
+            if request_exception is not None:
+                raise RequestsConnectionError(
+                    f"The framework could not be automatically inferred. If using the command-line, please provide the argument --framework (pt,tf) Detailed error: {request_exception}"
+                )
+            else:
+                raise FileNotFoundError(
+                    "Cannot determine framework from given checkpoint location."
+                    f" There should be a {Path(WEIGHTS_NAME).stem}*{Path(WEIGHTS_NAME).suffix} for PyTorch"
+                    f" or {Path(TF2_WEIGHTS_NAME).stem}*{Path(TF2_WEIGHTS_NAME).suffix} for TensorFlow."
+                )
 
         if is_torch_available():
             framework = framework or "pt"
         elif is_tf_available():
             framework = framework or "tf"
         else:
             raise EnvironmentError("Neither PyTorch nor TensorFlow found in environment. Cannot export model.")
@@ -1197,28 +1277,21 @@
                 continue
             model_mapping = auto_cls._model_mapping._model_mapping
             if target_name in model_mapping.values():
                 task_name = task
                 break
         if task_name is None:
             raise ValueError(f"Could not infer the task name for {target_name}.")
+
         return task_name
 
     @classmethod
     def _infer_task_from_model_name_or_path(
         cls, model_name_or_path: str, subfolder: str = "", revision: Optional[str] = None
     ) -> str:
-        tasks_to_automodels = {}
-        class_name_prefix = ""
-        if is_torch_available():
-            tasks_to_automodels = TasksManager._TASKS_TO_AUTOMODELS
-        else:
-            tasks_to_automodels = TasksManager._TASKS_TO_TF_AUTOMODELS
-            class_name_prefix = "TF"
-
         inferred_task_name = None
         is_local = os.path.isdir(os.path.join(model_name_or_path, subfolder))
 
         if is_local:
             # TODO: maybe implement that.
             raise RuntimeError("Cannot infer the task from a local directory yet, please specify the task manually.")
         else:
@@ -1235,24 +1308,32 @@
                 pipeline_tag = getattr(model_info, "pipeline_tag", None)
                 # conversational is not a supported task per se, just an alias that may map to
                 # text-generaton or text2text-generation
                 if pipeline_tag is not None and pipeline_tag != "conversational":
                     inferred_task_name = TasksManager.map_from_synonym(model_info.pipeline_tag)
                 else:
                     transformers_info = model_info.transformersInfo
+                    if transformers_info is not None and transformers_info.get("pipeline_tag") is not None:
+                        inferred_task_name = TasksManager.map_from_synonym(transformers_info["pipeline_tag"])
+                    else:
+                        # transformersInfo does not always have a pipeline_tag attribute
+                        class_name_prefix = ""
+                        if is_torch_available():
+                            tasks_to_automodels = TasksManager._TASKS_TO_AUTOMODELS
+                        else:
+                            tasks_to_automodels = TasksManager._TASKS_TO_TF_AUTOMODELS
+                            class_name_prefix = "TF"
 
-                    if transformers_info is None or transformers_info.get("auto_model") is None:
-                        raise RuntimeError(f"Could not infer the task from the model repo {model_name_or_path}")
-                    auto_model_class_name = transformers_info["auto_model"]
-                    if not auto_model_class_name.startswith("TF"):
-                        auto_model_class_name = f"{class_name_prefix}{auto_model_class_name}"
-                    for task_name, class_name_for_task in tasks_to_automodels.items():
-                        if class_name_for_task == auto_model_class_name:
-                            inferred_task_name = task_name
-                            break
+                        auto_model_class_name = transformers_info["auto_model"]
+                        if not auto_model_class_name.startswith("TF"):
+                            auto_model_class_name = f"{class_name_prefix}{auto_model_class_name}"
+                        for task_name, class_name_for_task in tasks_to_automodels.items():
+                            if class_name_for_task == auto_model_class_name:
+                                inferred_task_name = task_name
+                                break
 
         if inferred_task_name is None:
             raise KeyError(f"Could not find the proper task name for {auto_model_class_name}.")
         return inferred_task_name
 
     @classmethod
     def infer_task_from_model(
@@ -1312,14 +1393,15 @@
         task: str,
         model_name_or_path: Union[str, Path],
         subfolder: str = "",
         revision: Optional[str] = None,
         framework: Optional[str] = None,
         cache_dir: Optional[str] = None,
         torch_dtype: Optional["torch.dtype"] = None,
+        device: Optional[Union["torch.device", str]] = None,
         **model_kwargs,
     ) -> Union["PreTrainedModel", "TFPreTrainedModel"]:
         """
         Retrieves a model from its name and the task to be enabled.
 
         Args:
             task (`str`):
@@ -1335,14 +1417,16 @@
             framework (`Optional[str]`, *optional*):
                 The framework to use for the export. See `TasksManager.determine_framework` for the priority should
                 none be provided.
             cache_dir (`Optional[str]`, *optional*):
                 Path to a directory in which a downloaded pretrained model weights have been cached if the standard cache should not be used.
             torch_dtype (`Optional[torch.dtype]`, defaults to `None`):
                 Data type to load the model on. PyTorch-only argument.
+            device (`Optional[torch.device]`, defaults to `None`):
+                Device to initialize the model on. PyTorch-only argument. For PyTorch, defaults to "cpu".
             model_kwargs (`Dict[str, Any]`, *optional*):
                 Keyword arguments to pass to the model `.from_pretrained()` method.
 
         Returns:
             The instance of the model.
 
         """
@@ -1350,33 +1434,49 @@
 
         original_task = task
         if task == "auto":
             task = TasksManager.infer_task_from_model(model_name_or_path, subfolder=subfolder, revision=revision)
 
         model_type = None
         model_class_name = None
+        kwargs = {"subfolder": subfolder, "revision": revision, "cache_dir": cache_dir, **model_kwargs}
+
         if TasksManager._TASKS_TO_LIBRARY[task.replace("-with-past", "")] == "transformers":
+            config = AutoConfig.from_pretrained(model_name_or_path, **kwargs)
+            model_type = config.model_type.replace("_", "-")
             # TODO: if automatic-speech-recognition is passed as task, it may map to several
             # different auto class (AutoModelForSpeechSeq2Seq or AutoModelForCTC),
             # depending on the model type
-            if original_task in ["auto", "automatic-speech-recognition"]:
-                config = AutoConfig.from_pretrained(model_name_or_path)
-                model_type = config.model_type.replace("_", "-")
+            # if original_task in ["auto", "automatic-speech-recognition"]:
+            if original_task == "automatic-speech-recognition" or task == "automatic-speech-recognition":
                 if original_task == "auto" and config.architectures is not None:
                     model_class_name = config.architectures[0]
 
         model_class = TasksManager.get_model_class_for_task(
             task, framework, model_type=model_type, model_class_name=model_class_name
         )
 
-        kwargs = {"subfolder": subfolder, "revision": revision, "cache_dir": cache_dir, **model_kwargs}
         try:
             if framework == "pt":
                 kwargs["torch_dtype"] = torch_dtype
-            model = model_class.from_pretrained(model_name_or_path, **kwargs)
+
+                if isinstance(device, str):
+                    device = torch.device(device)
+                elif device is None:
+                    device = torch.device("cpu")
+
+                if version.parse(torch.__version__) >= version.parse("2.0"):
+                    with device:
+                        # Initialize directly in the requested device, to save allocation time. Especially useful for large
+                        # models to initialize on cuda device.
+                        model = model_class.from_pretrained(model_name_or_path, **kwargs)
+                else:
+                    model = model_class.from_pretrained(model_name_or_path, **kwargs).to(device)
+            else:
+                model = model_class.from_pretrained(model_name_or_path, **kwargs)
         except OSError:
             if framework == "pt":
                 logger.info("Loading TensorFlow model in PyTorch before exporting.")
                 kwargs["from_tf"] = True
                 model = model_class.from_pretrained(model_name_or_path, **kwargs)
             else:
                 logger.info("Loading PyTorch model in TensorFlow before exporting.")
@@ -1423,19 +1523,24 @@
                 raise ValueError("Model type cannot be inferred. Please provide the model_type for the model!")
 
             model_type = model_type.replace("_", "-")
             model_name = getattr(model, "name", model_name)
 
         model_tasks = TasksManager.get_supported_tasks_for_model_type(model_type, exporter, model_name=model_name)
 
-        task = TasksManager.map_from_synonym(task)
         if task not in model_tasks:
-            raise ValueError(
-                f"{model_type} doesn't support task {task} for the {exporter} backend."
-                f" Supported tasks are: {', '.join(model_tasks.keys())}."
-            )
+            synonyms = TasksManager.synonyms_for_task(task)
+            for synonym in synonyms:
+                if synonym in model_tasks:
+                    task = synonym
+                    break
+            if task not in model_tasks:
+                raise ValueError(
+                    f"{model_type} doesn't support task {task} for the {exporter} backend."
+                    f" Supported tasks are: {', '.join(model_tasks.keys())}."
+                )
 
         exporter_config_constructor = TasksManager._SUPPORTED_MODEL_TYPE[model_type][exporter][task]
         if exporter_config_kwargs is not None:
             exporter_config_constructor = partial(exporter_config_constructor, **exporter_config_kwargs)
 
         return exporter_config_constructor
```

### Comparing `optimum-1.8.8/optimum/exporters/tflite/__init__.py` & `optimum-1.9.0/optimum/exporters/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/exporters/tflite/__main__.py` & `optimum-1.9.0/optimum/exporters/tflite/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Entry point to the optimum.exporters.tflite command line."""
 
 from argparse import ArgumentParser
 
+from requests.exceptions import ConnectionError as RequestsConnectionError
+
 from ...commands.export.tflite import parse_args_tflite
 from ...utils import logging
 from ...utils.save_utils import maybe_load_preprocessors, maybe_save_preprocessors
 from ..error_utils import AtolError, OutputMatchError, ShapeError
 from ..tasks import TasksManager
 from .base import TFLiteQuantizationConfig
 from .convert import export, validate_model_outputs
@@ -47,14 +49,18 @@
         try:
             task = TasksManager.infer_task_from_model(args.model)
         except KeyError as e:
             raise KeyError(
                 "The task could not be automatically inferred. Please provide the argument --task with the task "
                 f"from {', '.join(TasksManager.get_all_tasks())}. Detailed error: {e}"
             )
+        except RequestsConnectionError as e:
+            raise RequestsConnectionError(
+                f"The task could not be automatically inferred as this is available only for models hosted on the Hugging Face Hub. Please provide the argument --task with the relevant task from {', '.join(TasksManager.get_all_tasks())}. Detailed error: {e}"
+            )
 
     model = TasksManager.get_model_from_task(
         task, args.model, framework="tf", cache_dir=args.cache_dir, trust_remote_code=args.trust_remote_code
     )
 
     tflite_config_constructor = TasksManager.get_exporter_config_constructor(model=model, exporter="tflite", task=task)
     # TODO: find a cleaner way to do this.
```

### Comparing `optimum-1.8.8/optimum/exporters/tflite/base.py` & `optimum-1.9.0/optimum/exporters/tflite/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,16 @@
         num_choices: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         num_channels: Optional[int] = None,
         feature_size: Optional[int] = None,
         nb_max_frames: Optional[int] = None,
         audio_sequence_length: Optional[int] = None,
+        point_batch_size: Optional[int] = None,
+        nb_points_per_image: Optional[int] = None,
     ):
         self._config = config
         self._normalized_config = self.NORMALIZED_CONFIG_CLASS(self._config)
         self.mandatory_axes = ()
         self.task = task
         self._axes: Dict[str, int] = {}
 
@@ -203,14 +205,16 @@
             "num_choices": num_choices,
             "width": width,
             "height": height,
             "num_channels": num_channels,
             "feature_size": feature_size,
             "nb_max_frames": nb_max_frames,
             "audio_sequence_length": audio_sequence_length,
+            "point_batch_size": point_batch_size,
+            "nb_points_per_image": nb_points_per_image,
         }
         for name, value in axes_values.items():
             setattr(self, name, value)
 
     @classmethod
     def get_mandatory_axes_for_task(cls, task: str) -> Tuple[str]:
         axes = []
```

### Comparing `optimum-1.8.8/optimum/exporters/tflite/config.py` & `optimum-1.9.0/optimum/exporters/tflite/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/exporters/tflite/convert.py` & `optimum-1.9.0/optimum/exporters/tflite/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/exporters/tflite/model_configs.py` & `optimum-1.9.0/optimum/exporters/tflite/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/fx/__init__.py` & `optimum-1.9.0/optimum/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/fx/optimization/__init__.py` & `optimum-1.9.0/optimum/fx/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/fx/optimization/transformations.py` & `optimum-1.9.0/optimum/fx/optimization/transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/fx/quantization/__init__.py` & `optimum-1.9.0/optimum/fx/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/fx/quantization/functions.py` & `optimum-1.9.0/optimum/fx/quantization/functions.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/fx/utils.py` & `optimum-1.9.0/optimum/fx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/modeling_base.py` & `optimum-1.9.0/optimum/modeling_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,28 +165,27 @@
         api = HfApi()
 
         user = api.whoami(huggingface_token)
         self.git_config_username_and_email(git_email=user["email"], git_user=user["fullname"])
 
         api.create_repo(
             token=huggingface_token,
-            name=repository_id,
-            organization=user["name"],
+            repo_id=repository_id,
             exist_ok=True,
             private=private,
         )
         for path, subdirs, files in os.walk(save_directory):
             for name in files:
                 local_file_path = os.path.join(path, name)
                 _, hub_file_path = os.path.split(local_file_path)
                 # FIXME: when huggingface_hub fixes the return of upload_file
                 try:
                     api.upload_file(
                         token=huggingface_token,
-                        repo_id=f"{user['name']}/{repository_id}",
+                        repo_id=f"{repository_id}",
                         path_or_fileobj=os.path.join(os.getcwd(), local_file_path),
                         path_in_repo=hub_file_path,
                     )
                 except KeyError:
                     pass
                 except NameError:
                     pass
```

### Comparing `optimum-1.8.8/optimum/onnx/__init__.py` & `optimum-1.9.0/optimum/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnx/configuration.py` & `optimum-1.9.0/optimum/onnx/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnx/graph_transformations.py` & `optimum-1.9.0/optimum/onnx/graph_transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,14 @@
     cast_int64_tensorproto_to_int32,
 )
 
 
 logger = logging.get_logger()
 
 
-ONNX_BYTE_SIZE_LIMIT = 2147483648
-
-
 def remove_duplicate_weights(model: ModelProto, inplace: bool = False) -> ModelProto:
     """
     Finds and removes duplicate weights in a model by keeping only unique weights, and make the duplicate values point
     to them.
 
     Args:
         model (`onnx.ModelProto`): The model to remove duplicates from.
@@ -210,15 +207,15 @@
             opset_imports.append(opset_import)
             opset_domains.add(opset_import.domain)
 
     merged_model = onnx.helper.make_model(merged_graph, producer_name=producer_name, opset_imports=opset_imports)
 
     # for large models, a path must be provided instead of a ModelProto:
     # https://github.com/onnx/onnx/blob/main/docs/PythonAPIOverview.md#checking-a-large-onnx-model-2gb
-    if merged_model.ByteSize() < ONNX_BYTE_SIZE_LIMIT:
+    if merged_model.ByteSize() < onnx.checker.MAXIMUM_PROTOBUF:
         # For the try catch, refer to https://github.com/microsoft/onnxruntime/issues/14768
         try:
             onnx.checker.check_model(merged_model)
         except Exception as e:
             if "No Op registered for" in str(e):
                 pass
             else:
```

### Comparing `optimum-1.8.8/optimum/onnx/modeling_seq2seq.py` & `optimum-1.9.0/optimum/onnx/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnx/transformations_utils.py` & `optimum-1.9.0/optimum/onnx/transformations_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnx/utils.py` & `optimum-1.9.0/optimum/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/__init__.py` & `optimum-1.9.0/optimum/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/base.py` & `optimum-1.9.0/optimum/onnxruntime/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,20 @@
             raise RuntimeError("Could not find the past key values in the provided model.")
 
         if len(self.key_value_input_names) > 0:
             self.use_past = True
         else:
             self.use_past = False
 
+        self.use_fp16 = False
+        for inp in session.get_inputs():
+            if inp.name == "past_key_values" and inp.type == "tensor(float16)":
+                self.use_fp16 = True
+                break
+
         if len(self.key_value_output_names) != 0:
             # Attributes useful when computing the past key/values output shapes.
             self.expected_key_symbolic_shape = None
             self.expected_value_symbolic_shape = None
             for output in self.session.get_outputs():
                 if ".key" in output.name:
                     self.expected_key_symbolic_shape = output.shape
@@ -180,20 +186,20 @@
                 isinstance(self.expected_value_symbolic_shape[-1], str)
                 and "sequence_length" in self.expected_value_symbolic_shape[-1]
             ):
                 self.value_sequence_length_idx = -1
 
     def prepare_inputs_for_merged(
         self,
-        input_ids: Union[None, torch.LongTensor, np.ndarray] = None,
-        past_key_values: Union[None, Tuple[torch.FloatTensor], Tuple[np.ndarray]] = None,
-        use_torch: bool = False,
+        input_ids: Union[None, torch.LongTensor, np.ndarray],
+        past_key_values: Union[None, Tuple[torch.FloatTensor], Tuple[np.ndarray]],
+        use_torch: bool,
     ):
-        constructor = torch if use_torch is True else np
         if self.parent_model.use_merged:
+            constructor = torch if use_torch is True else np
             # Uses without/with branch of a merged decoder depending on whether real past key values are passed
             use_cache_branch = constructor.full((1,), past_key_values is not None)
         else:
             # Uses separate decoders
             use_cache_branch = None
 
         if use_torch and use_cache_branch is not None:
@@ -201,32 +207,33 @@
 
         # Generate dummy past for the first forward if uses a merged decoder
         if self.parent_model.use_merged and past_key_values is None:
             batch_size = input_ids.shape[0]
             num_attention_heads = self.normalized_config.num_attention_heads
             embed_size_per_head = self.normalized_config.hidden_size // num_attention_heads
 
+            dtype = constructor.float16 if self.use_fp16 else constructor.float32
             # TODO: find a way to better handle this controlflow, this is EXTREMELY ugly
             # "1" is the dummy sequence length
             if self.parent_model.config.model_type == "bloom":
                 shape_value = (batch_size * num_attention_heads, 1, embed_size_per_head)
                 shape_key = (batch_size * num_attention_heads, embed_size_per_head, 1)
-                key = constructor.zeros(shape_key, dtype=constructor.float32)
-                value = constructor.zeros(shape_value, dtype=constructor.float32)
+                key = constructor.zeros(shape_key, dtype=dtype)
+                value = constructor.zeros(shape_value, dtype=dtype)
 
                 if use_torch is True:
                     key = key.to(self.device)
                     value = value.to(self.device)
 
                 past_key_values = tuple(
                     key_or_value for _ in range(len(self.key_value_input_names) // 2) for key_or_value in [key, value]
                 )
             else:
                 shape = (batch_size, num_attention_heads, 1, embed_size_per_head)
-                key_or_value = constructor.zeros(shape, dtype=constructor.float32)
+                key_or_value = constructor.zeros(shape, dtype=dtype)
 
                 if use_torch is True:
                     key_or_value = key_or_value.to(self.device)
 
                 past_key_values = tuple(key_or_value for _ in range(len(self.key_value_input_names)))
 
         return use_cache_branch, past_key_values
@@ -300,22 +307,26 @@
             )
 
         # no-ops if merged decoder is not used
         use_cache_branch_tensor, past_key_values = self.prepare_inputs_for_merged(
             input_ids, past_key_values, use_torch=use_torch
         )
 
-        if self.device.type == "cuda" and self.parent_model.use_io_binding:
+        if self.parent_model.use_io_binding:
             known_output_shapes = self.compute_past_key_values_output_shapes(
                 input_ids,
                 use_cache_branch=use_cache_branch_tensor.item() if use_cache_branch_tensor is not None else None,
                 past_key_values=past_key_values,
             )
 
-            model_inputs = [input_ids]
+            # TODO: fix transformers generate to have contiguous input_ids here already
+            # For an unknown reason, calling `contigous()` here is necessary to not have errors
+            # on CPU EP with batch size > 1, despite it being also called in _prepare_io_binding.
+            # I suspect the reason is the contiguous python list that messes something up?
+            model_inputs = [input_ids.contiguous()]
 
             if "attention_mask" in self.input_names:
                 model_inputs.append(attention_mask)
 
             if past_key_values is not None:
                 model_inputs += past_key_values
 
@@ -329,17 +340,20 @@
             io_binding, output_shapes, output_buffers = self.parent_model._prepare_io_binding(
                 self.session,
                 *model_inputs,
                 known_output_shapes=known_output_shapes,
                 ordered_input_names=self._ordered_input_names,
             )
 
-            io_binding.synchronize_inputs()
-            self.session.run_with_iobinding(io_binding)
-            io_binding.synchronize_outputs()
+            if self.device.type == "cpu":
+                self.session.run_with_iobinding(io_binding)
+            else:
+                io_binding.synchronize_inputs()
+                self.session.run_with_iobinding(io_binding)
+                io_binding.synchronize_outputs()
 
             # Tuple of length equal to : number of layer * number of past_key_value per decoder layer(2)
             past_key_values = ()
             for name in self.key_value_output_names:
                 past_key_values += (output_buffers[name].view(output_shapes[name]),)
 
             # Tuple of tuple of length `n_layers`, with each tuple of length equal to 2 (self-attention key and value per decoder layer)
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/configuration.py` & `optimum-1.9.0/optimum/onnxruntime/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,23 +664,22 @@
             The default value is set to `True` since this fusion is incompatible with ONNX Runtime quantization
         disable_shape_inference (`bool`, defaults to `False`):
             Whether to disable symbolic shape inference.
             The default value is set to `False` but symbolic shape inference might cause issues sometimes.
         use_multi_head_attention (`bool`, defaults to `False`):
             Experimental argument. Use MultiHeadAttention instead of Attention operator, which has merged weights for Q/K/V projection,
             which might be faster in some cases since 3 MatMul is merged into one."
-            "Note that MultiHeadAttention might be slower than Attention since MatMul of input projection is excluded. "
-            "MultiHeadAttention has only CUDA implementation so the model can only run with CUDAExecutionProvider.
-        enable_gemm_fast_gelu (`bool`, defaults to `True`):
+            "Note that MultiHeadAttention might be slower than Attention when qkv are not packed. "
+        enable_gemm_fast_gelu_fusion (`bool`, defaults to `False`):
             Enable GemmfastGelu fusion.
         use_raw_attention_mask (`bool`, defaults to `False`):
             Use raw attention mask. Use this option if your input is not right-side padding. This might deactivate fused attention and get worse performance.
-        disable_group_norm (`bool`, defaults to `False`):
+        disable_group_norm_fusion (`bool`, defaults to `True`):
             Do not fuse GroupNorm. Only works for model_type=unet.
-        disable_packed_kv (`bool`, defaults to `False`):
+        disable_packed_kv (`bool`, defaults to `True`):
             Do not use packed kv in cross attention. Only works for model_type=unet.
     """
 
     optimization_level: int = 1
     optimize_for_gpu: bool = False
 
     fp16: bool = False
@@ -712,19 +711,19 @@
     enable_gelu_approximation: bool = False
     use_mask_index: bool = False
     no_attention_mask: bool = False
     disable_embed_layer_norm: bool = True
     disable_shape_inference: bool = False
 
     # ONNX Runtime 1.14.0 arguments
-    use_multi_head_attention = False
-    enable_gemm_fast_gelu_fusion = False
-    use_raw_attention_mask = False
-    disable_group_norm_fusion = True
-    disable_packed_kv = True
+    use_multi_head_attention: bool = False
+    enable_gemm_fast_gelu_fusion: bool = False
+    use_raw_attention_mask: bool = False
+    disable_group_norm_fusion: bool = True
+    disable_packed_kv: bool = True
 
     def __post_init__(self):
         def deprecate_renamed_attribute(old_name, new_name, mapping_func=None):
             if getattr(self, old_name, None) is not None:
                 if mapping_func is None:
 
                     def identity(x):
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/constants.py` & `optimum-1.9.0/optimum/onnxruntime/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/graph.py` & `optimum-1.9.0/optimum/onnxruntime/graph.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/io_binding/__init__.py` & `optimum-1.9.0/optimum/onnxruntime/io_binding/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/io_binding/io_binding_helper.py` & `optimum-1.9.0/optimum/onnxruntime/io_binding/io_binding_helper.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/model.py` & `optimum-1.9.0/optimum/onnxruntime/model.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/modeling_decoder.py` & `optimum-1.9.0/optimum/onnxruntime/modeling_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,26 +147,26 @@
                 The ONNX Runtime inference session associated to the decoder with past key values. This argument should not
                 be set if use_merged=True is used.
             onnx_paths (`List[str]`):
                 Path to ONNX files associated with the model.
             use_cache (`bool`, defaults to `True`):
                 Whether or not past key/values cache should be used. Defaults to `True`.
             use_io_binding (`Optional[bool]`, defaults to `None`):
-                Whether use IOBinding during inference to avoid memory copy between the host and devices. Defaults to
-                `True` if the device is CUDA, otherwise defaults to `False`.
+                Whether to use IOBinding during inference to avoid memory copy between the host and devices. Defaults to
+                `True` if the execution provider is CPUExecutionProvider or CUDAExecutionProvider, otherwise defaults to `False`.
             model_save_dir (`Optional[Union[str, Path, TemporaryDirectory]]`, defaults to `""`):
                 The directory under which the model exported to ONNX was saved.
             preprocessors (`Optional[List]`, defaults to `None`):
                 The list of the preprocessors (tokenizer, processor, feature_extractor) to save alongside the ORTModel.
             generation_config (`Optional[GenerationConfig]`, defaults to `None`):
                 The generation configuration used by default when calling `generate()`.
                 Refer to https://huggingface.co/docs/transformers/main/en/main_classes/text_generation#transformers.GenerationMixin.generate.
         """
         if use_io_binding is None:
-            if decoder_session.get_providers()[0] == "CUDAExecutionProvider":
+            if decoder_session.get_providers()[0] in ["CPUExecutionProvider", "CUDAExecutionProvider"]:
                 use_io_binding = True
             else:
                 use_io_binding = False
 
         self.shared_attributes_init(
             decoder_session,
             use_io_binding=use_io_binding,
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/modeling_diffusion.py` & `optimum-1.9.0/optimum/onnxruntime/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/modeling_ort.py` & `optimum-1.9.0/optimum/onnxruntime/modeling_ort.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,38 +610,43 @@
         cache_dir: Optional[str] = None,
         subfolder: str = "",
         config: Optional["PretrainedConfig"] = None,
         local_files_only: bool = False,
         provider: str = "CPUExecutionProvider",
         session_options: Optional[ort.SessionOptions] = None,
         provider_options: Optional[Dict[str, Any]] = None,
+        use_io_binding: Optional[bool] = None,
         **kwargs,
     ):
         """
         provider (`str`, defaults to `"CPUExecutionProvider"`):
             ONNX Runtime provider to use for loading the model. See https://onnxruntime.ai/docs/execution-providers/ for
             possible providers.
         session_options (`Optional[onnxruntime.SessionOptions]`, defaults to `None`),:
             ONNX Runtime session options to use for loading the model.
         provider_options (`Optional[Dict[str, Any]]`, defaults to `None`):
             Provider option dictionaries corresponding to the provider used. See available options
             for each provider: https://onnxruntime.ai/docs/api/c/group___global.html .
+        use_io_binding (`Optional[bool]`, defaults to `None`):
+            Whether to use IOBinding during inference to avoid memory copy between the host and device, or between numpy/torch tensors and ONNX Runtime ORTValue. Defaults to
+            `True` if the execution provider is CUDAExecutionProvider. For [~onnxruntime.ORTModelForCausalLM], defaults to `True` on CPUExecutionProvider,
+            in all other cases defaults to `False`.
         kwargs (`Dict[str, Any]`):
             Will be passed to the underlying model loading methods.
 
         > Parameters for decoder models (ORTModelForCausalLM, ORTModelForSeq2SeqLM, ORTModelForSeq2SeqLM, ORTModelForSpeechSeq2Seq, ORTModelForVision2Seq)
 
         use_cache (`Optional[bool]`, defaults to `True`):
             Whether or not past key/values cache should be used. Defaults to `True`.
 
         > Parameters for ORTModelForCausalLM
 
         use_merged (`Optional[bool]`, defaults to `None`):
             whether or not to use a single ONNX that handles both the decoding without and with past key values reuse. This option defaults
-            to `True` if loading from a local repository and a merged decoder is found. When exporting with `from_transformers=True`,
+            to `True` if loading from a local repository and a merged decoder is found. When exporting with `export=True`,
             defaults to `False`. This option should be set to `True` to minimize memory usage.
 
         Returns:
             `ORTModel`: The loaded ORTModel model.
         """
         return super().from_pretrained(
             model_id,
@@ -651,14 +656,15 @@
             cache_dir=cache_dir,
             subfolder=subfolder,
             config=config,
             local_files_only=local_files_only,
             provider=provider,
             session_options=session_options,
             provider_options=provider_options,
+            use_io_binding=use_io_binding,
             **kwargs,
         )
 
     def _prepare_output_buffer(self, model: ort.InferenceSession, output_shape: Tuple[int], output_name: str):
         """Prepares the buffer of output_name with a 1D tensor."""
         ort_type = TypeHelper.get_output_type(model, output_name)
         torch_type = TypeHelper.ort_type_to_torch_type(ort_type)
@@ -741,35 +747,35 @@
             containing the shape of each output, and another one pointing to the buffers containing the outputs data.
 
         """
         io_binding = model.io_binding()
 
         name_to_np_type = TypeHelper.get_io_numpy_type_map(model)
 
-        input_name_to_tensor = {}
+        input_name_to_shape = {}
         for idx, tensor in enumerate(model_inputs):
             if tensor is None:
                 continue
             name = ordered_input_names[idx]
-            input_name_to_tensor[name] = tensor
             tensor = tensor.contiguous()
+            input_name_to_shape[name] = tensor.shape
             io_binding.bind_input(
                 name,
                 tensor.device.type,
-                self.device.index,
+                IOBindingHelper.get_device_index(self.device),
                 name_to_np_type[name],
                 tuple(tensor.shape),
                 tensor.data_ptr(),
             )
         dimensions = {}
         for input_ in model.get_inputs():
             shape = input_.shape
             for idx, axis in enumerate(shape):
                 if isinstance(axis, str):
-                    dimensions[axis] = input_name_to_tensor[input_.name].shape[idx]
+                    dimensions[axis] = input_name_to_shape[input_.name][idx]
 
         output_shapes = {}
         output_buffers = {}
 
         if known_output_shapes is None:
             known_output_shapes = {}
 
@@ -789,15 +795,15 @@
                 for axis_name in output_node.shape:
                     output_shape.append(self._output_shape_inference(axis_name, dimensions))
             output_buffer = self._prepare_output_buffer(model, output_shape, output_name)
 
             io_binding.bind_output(
                 output_name,
                 output_buffer.device.type,
-                self.device.index,
+                IOBindingHelper.get_device_index(self.device),
                 name_to_np_type[output_name],
                 output_shape,
                 output_buffer.data_ptr(),
             )
             output_shapes[output_name] = output_shape
             output_buffers[output_name] = output_buffer
 
@@ -884,14 +890,17 @@
         token_type_ids: Optional[Union[torch.Tensor, np.ndarray]] = None,
         **kwargs,
     ):
         use_torch = isinstance(input_ids, torch.Tensor)
         self.raise_on_numpy_input_io_binding(use_torch)
 
         if self.device.type == "cuda" and self.use_io_binding:
+            if attention_mask is None:
+                attention_mask = torch.ones_like(input_ids)
+
             io_binding, output_shapes, output_buffers = self.prepare_io_binding(
                 input_ids,
                 attention_mask,
                 token_type_ids,
                 ordered_input_names=self._ordered_input_names,
             )
 
@@ -903,15 +912,18 @@
             # converts output to namedtuple for pipelines post-processing
             return BaseModelOutput(
                 last_hidden_state=output_buffers["last_hidden_state"].view(output_shapes["last_hidden_state"])
             )
         else:
             if use_torch:
                 input_ids = input_ids.cpu().detach().numpy()
-                attention_mask = attention_mask.cpu().detach().numpy()
+                if attention_mask is None:
+                    attention_mask = np.ones_like(input_ids)
+                else:
+                    attention_mask = attention_mask.cpu().detach().numpy()
                 if token_type_ids is not None:
                     token_type_ids = token_type_ids.cpu().detach().numpy()
 
             onnx_inputs = {
                 "input_ids": input_ids,
                 "attention_mask": attention_mask,
             }
@@ -1381,15 +1393,15 @@
     Example of mutliple choice:
 
     ```python
     >>> from transformers import {processor_class}
     >>> from optimum.onnxruntime import {model_class}
 
     >>> tokenizer = {processor_class}.from_pretrained("{checkpoint}")
-    >>> model = {model_class}.from_pretrained("{checkpoint}", from_transformers=True)
+    >>> model = {model_class}.from_pretrained("{checkpoint}", export=True)
 
     >>> num_choices = 4
     >>> first_sentence = ["Members of the procession walk down the street holding small horn brass instruments."] * num_choices
     >>> second_sentence = [
     ...     "A drum line passes by walking down the street playing their instruments.",
     ...     "A drum line has heard approaching them.",
     ...     "A drum line arrives and they're outside dancing and asleep.",
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/modeling_seq2seq.py` & `optimum-1.9.0/optimum/onnxruntime/modeling_seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     >>> from optimum.onnxruntime import {model_class}
     >>> from PIL import Image
     >>> import requests
 
 
     >>> processor = {processor_class}.from_pretrained("{checkpoint}")
     >>> tokenizer = {tokenizer_class}.from_pretrained("{checkpoint}")
-    >>> model = {model_class}.from_pretrained("{checkpoint}", from_transformers=True)
+    >>> model = {model_class}.from_pretrained("{checkpoint}", export=True)
 
     >>> url = "http://images.cocodataset.org/val2017/000000039769.jpg"
     >>> image = Image.open(requests.get(url, stream=True).raw)
     >>> inputs = processor(image, return_tensors="pt")
 
     >>> gen_tokens = model.generate(**inputs)
     >>> outputs = tokenizer.batch_decode(gen_tokens, skip_special_tokens=True)
@@ -266,15 +266,15 @@
     >>> from optimum.onnxruntime import {model_class}
     >>> from PIL import Image
     >>> import requests
 
 
     >>> processor = {processor_class}.from_pretrained("{checkpoint}")
     >>> tokenizer = {tokenizer_class}.from_pretrained("{checkpoint}")
-    >>> model = {model_class}.from_pretrained("{checkpoint}", from_transformers=True)
+    >>> model = {model_class}.from_pretrained("{checkpoint}", export=True)
 
     >>> url = "http://images.cocodataset.org/val2017/000000039769.jpg"
     >>> image = Image.open(requests.get(url, stream=True).raw)
 
     >>> image_to_text = pipeline("image-to-text", model=model, tokenizer=tokenizer, feature_extractor=processor, image_processor=processor)
     >>> pred = image_to_text(image)
     ```
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/optimization.py` & `optimum-1.9.0/optimum/onnxruntime/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from ..onnx.utils import check_model_uses_external_data
 from ..utils import CONFIG_NAME, NormalizedConfigManager, logging
 from ..utils.save_utils import maybe_save_preprocessors
 from .configuration import OptimizationConfig, ORTConfig
 from .modeling_decoder import ORTModelForCausalLM
 from .modeling_ort import ORTModel
-from .modeling_seq2seq import ORTModelForSeq2SeqLM
+from .modeling_seq2seq import ORTModelForConditionalGeneration
 from .utils import ONNX_WEIGHTS_NAME, ORTConfigManager
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig
 
 
@@ -85,28 +85,28 @@
             file_names(`Optional[List[str]]`, defaults to `None`):
                 The list of file names of the models to optimize.
         """
         onnx_model_path = []
         config = None
         if isinstance(model_or_path, ORTModel):
             from_ortmodel = True
-            if isinstance(model_or_path, ORTModelForSeq2SeqLM):
+            if isinstance(model_or_path, ORTModelForConditionalGeneration):
                 onnx_model_path += [
                     model_or_path.encoder_model_path,
                     model_or_path.decoder_model_path,
                 ]
                 # Add the decoder with past key/values if present
                 if model_or_path.use_cache:
                     onnx_model_path.append(model_or_path.decoder_with_past_model_path)
             elif isinstance(model_or_path, ORTModelForCausalLM):
                 if model_or_path.use_merged is True:
                     raise NotImplementedError(
                         "ORTOptimizer does not support ORTModelForCausalLM models that use a single ONNX for both the without/with past cases."
                         " Please pass an ORTModelForCausalLM that uses a separate ONNX for each without/with past cases. This can be done"
-                        " by using `ORTModelForCausalLM.from_pretrained(..., from_transformers=True, use_merged=False)`, or by"
+                        " by using `ORTModelForCausalLM.from_pretrained(..., export=True, use_merged=False)`, or by"
                         " using the option `--no-post-process` in the optimum-cli ONNX export tool."
                     )
                 onnx_model_path.append(model_or_path.decoder_model_path)
                 if model_or_path.use_cache:
                     onnx_model_path.append(model_or_path.decoder_with_past_model_path)
             else:
                 onnx_model_path.append(model_or_path.model_path)
@@ -182,42 +182,56 @@
         ort_config = ORTConfig(
             optimization=optimization_config,
             use_external_data_format=model_uses_external_data,
             one_external_file=one_external_file,
         )
 
         for model_path in self.onnx_model_path:
+            suffix = f"_{file_suffix}" if file_suffix else ""
+            output_path = save_dir.joinpath(f"{model_path.stem}{suffix}").with_suffix(model_path.suffix)
+
             try:
                 optimizer = optimize_model(
                     model_path.as_posix(),
                     model_type,
                     self.normalized_config.num_attention_heads,
                     self.normalized_config.hidden_size,
                     opt_level=optimization_config.optimization_level,
                     optimization_options=optimization_options,
                     use_gpu=optimization_config.optimize_for_gpu,
                     only_onnxruntime=not optimization_config.enable_transformers_specific_optimizations,
                 )
 
                 if optimization_config.fp16:
+                    if model_uses_external_data:
+                        # Refer to https://github.com/microsoft/onnxruntime/blob/v1.15.0/onnxruntime/python/tools/transformers/float16.py#L204
+                        # The ONNX infer_shapes_path method should be used instead of infer_shapes
+                        # for models >= 2 GB, and it expects a model written to disk.
+                        # Note that convert_float_to_float16 then overwrites optimizer.model as the
+                        # new ModelProto.
+                        optimizer.save_model_to_file(
+                            output_path.as_posix(),
+                            use_external_data_format=model_uses_external_data,
+                            all_tensors_to_one_file=one_external_file,
+                        )
+
+                        optimizer.model = output_path.as_posix()
+
                     # keep_io_types to keep inputs/outputs as float32
                     optimizer.convert_float_to_float16(
                         use_symbolic_shape_infer=not optimization_config.disable_shape_inference, keep_io_types=True
                     )
             except Exception as e:
                 if "Incomplete symbolic shape inference" in str(e):
                     err = RuntimeError(
                         f"{str(e)}. Try to set `disable_shape_inference=True` in your optimization configuration."
                     )
                     raise err from e
                 raise
 
-            suffix = f"_{file_suffix}" if file_suffix else ""
-            output_path = save_dir.joinpath(f"{model_path.stem}{suffix}").with_suffix(model_path.suffix)
-
             # TODO: ORT save_model_to_file will save as `.data` although we save as `.onnx_data` in the export
             optimizer.save_model_to_file(
                 output_path.as_posix(),
                 use_external_data_format=model_uses_external_data,
                 all_tensors_to_one_file=one_external_file,
             )
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/preprocessors/__init__.py` & `optimum-1.9.0/optimum/onnxruntime/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/__init__.py` & `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/excluders.py` & `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/excluders.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/fully_connected.py` & `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/fully_connected.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/gelu.py` & `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/gelu.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/preprocessors/passes/layernorm.py` & `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/layernorm.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/preprocessors/quantization.py` & `optimum-1.9.0/optimum/onnxruntime/preprocessors/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/quantization.py` & `optimum-1.9.0/optimum/onnxruntime/quantization.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     """
 
     def __init__(self, onnx_model_path: Path, config: Optional["PretrainedConfig"] = None):
         """
         Args:
             onnx_model_path (`Path`):
                 Path to the onnx model files you want to quantize.
-            config (`Optional[PretrainedConfig]`, *optional*):
+            config (`Optional[PretrainedConfig]`, defaults to `None`):
                 The configuration of the model.
         """
         super().__init__()
         self.onnx_model_path = onnx_model_path
         self.config = config
         if self.config is None:
             try:
@@ -118,15 +118,15 @@
         Instantiates a `ORTQuantizer` from a an ONNX model file or an `ORTModel`.
 
         Args:
             model_or_path (`Union[ORTModel, str, Path]`):
                 Can be either:
                     - A path to a saved exported ONNX Intermediate Representation (IR) model, e.g., `./my_model_directory/.
                     - Or an `ORTModelForXX` class, e.g., `ORTModelForQuestionAnswering`.
-            file_name(`Optional[str]`, *optional*):
+            file_name(`Optional[str]`, defaults to `None`):
                 Overwrites the default model file name from `"model.onnx"` to `file_name`.
                 This allows you to load different model files from the same repository or directory.
         Returns:
             An instance of `ORTQuantizer`.
         """
         ort_quantizer_error_message = "ORTQuantizer does not support multi-file quantization. Please create separate ORTQuantizer instances for each model/file, by passing the argument `file_name` to ORTQuantizer.from_pretrained()."
 
@@ -138,20 +138,15 @@
             raise NotImplementedError(ort_quantizer_error_message)
         elif isinstance(model_or_path, ORTModelForCausalLM):
             if model_or_path.use_cache is False:
                 path = Path(model_or_path.decoder_model_path)
             elif model_or_path.use_cache is True and model_or_path.use_merged is False:
                 raise NotImplementedError(ort_quantizer_error_message)
             else:
-                raise NotImplementedError(
-                    "ORTQuantizer does not support ORTModelForCausalLM models that use a single ONNX for both the without/with past cases."
-                    " Please pass an ORTModelForCausalLM that uses a separate ONNX for each without/with past cases. This can be done"
-                    " by using `ORTModelForCausalLM.from_pretrained(..., from_transformers=True, use_merged=False)`, or by"
-                    " using the option `--no-post-process` in the optimum-cli ONNX export tool."
-                )
+                path = Path(model_or_path.decoder_model_path)
         elif isinstance(model_or_path, Path) and file_name is None:
             onnx_files = list(model_or_path.glob("*.onnx"))
             if len(onnx_files) == 0:
                 raise FileNotFoundError(f"Could not find any ONNX model file in {model_or_path}")
             elif len(onnx_files) > 1:
                 raise RuntimeError(
                     f"Found too many ONNX model files in {model_or_path}. {ort_quantizer_error_message}"
@@ -182,25 +177,25 @@
         Performs the calibration step and computes the quantization ranges.
 
         Args:
             dataset (`Dataset`):
                 The dataset to use when performing the calibration step.
             calibration_config ([`~CalibrationConfig`]):
                 The configuration containing the parameters related to the calibration step.
-            onnx_augmented_model_name (`Union[str, Path]`, *optional*, defaults to `"augmented_model.onnx"`):
+            onnx_augmented_model_name (`Union[str, Path]`, defaults to `"augmented_model.onnx"`):
                 The path used to save the augmented model used to collect the quantization ranges.
-            operators_to_quantize (`Optional[List[NodeType]]`, *optional*):
+            operators_to_quantize (`Optional[List[NodeType]]`, defaults to `None`):
                 List of the operators types to quantize.
-            batch_size (`int`, *optional*, defaults to 1):
+            batch_size (`int`, defaults to 1):
                 The batch size to use when collecting the quantization ranges values.
             use_external_data_format (`bool`, defaults to `False`):
                 Whether to use external data format to store model which size is >= 2Gb.
             use_gpu (`bool`, defaults to `False`):
                 Whether to use the GPU when collecting the quantization ranges values.
-            force_symmetric_range (`bool`, *optional*, defaults to `False`):
+            force_symmetric_range (`bool`, defaults to `False`):
                 Whether to make the quantization ranges symmetric.
 
         Returns:
             The dictionary mapping the nodes name to their quantization ranges.
         """
         # If a dataset is provided, then we are in a static quantization mode
         LOGGER.info(
@@ -236,25 +231,25 @@
         Performs the calibration step and collects the quantization ranges without computing them.
 
         Args:
             dataset (`Dataset`):
                 The dataset to use when performing the calibration step.
             calibration_config (`CalibrationConfig`):
                 The configuration containing the parameters related to the calibration step.
-            onnx_augmented_model_name (`Union[str, Path]`, *optional*, defaults to `"augmented_model.onnx"`):
+            onnx_augmented_model_name (`Union[str, Path]`, defaults to `"augmented_model.onnx"`):
                 The path used to save the augmented model used to collect the quantization ranges.
-            operators_to_quantize (`Optional[List[NodeType]]`, *optional*):
+            operators_to_quantize (`Optional[List[NodeType]]`, defaults to `None`):
                 List of the operators types to quantize.
-            batch_size (`int`, *optional*, defaults to 1):
+            batch_size (`int`, defaults to 1):
                 The batch size to use when collecting the quantization ranges values.
-            use_external_data_format (`bool`, *optional*, defaults to `False`):
+            use_external_data_format (`bool`, defaults to `False`):
                 Whether uto se external data format to store model which size is >= 2Gb.
-            use_gpu (`bool`, *optional*, defaults to `False`):
+            use_gpu (`bool`, defaults to `False`):
                 Whether to use the GPU when collecting the quantization ranges values.
-            force_symmetric_range (`bool`, *optional*, defaults to `False`):
+            force_symmetric_range (`bool`, defaults to `False`):
                 Whether to make the quantization ranges symmetric.
         """
         # If no calibrator, then create one
         if calibration_config.method is not None:
             LOGGER.info(f"Creating calibrator: {calibration_config.method}({calibration_config})")
             self._calibrator = calibration_config.create_calibrator(
                 onnx_model_path=self.onnx_model_path.as_posix(),
@@ -299,31 +294,34 @@
         Quantizes a model given the optimization specifications defined in `quantization_config`.
 
         Args:
             quantization_config (`QuantizationConfig`):
                 The configuration containing the parameters related to quantization.
             save_dir (`Union[str, Path]`):
                 The directory where the quantized model should be saved.
-            file_suffix (`Optional[str]`, *optional*, defaults to `"quantized"`):
+            file_suffix (`Optional[str]`, defaults to `"quantized"`):
                 The file_suffix used to save the quantized model.
-            calibration_tensors_range (`Optional[Dict[NodeName, Tuple[float, float]]]`, *optional*):
-                The dictionary mapping the nodes name to their quantization ranges, used and required only when applying
-                static quantization.
-            use_external_data_format (`bool`, *optional*, defaults to `False`):
+            calibration_tensors_range (`Optional[Dict[NodeName, Tuple[float, float]]]`, defaults to `None`):
+                The dictionary mapping the nodes name to their quantization ranges, used and required only when applying static quantization.
+            use_external_data_format (`bool`, defaults to `False`):
                 Whether to use external data format to store model which size is >= 2Gb.
-            preprocessor (`Optional[QuantizationPreprocessor]`, *optional*):
+            preprocessor (`Optional[QuantizationPreprocessor]`, defaults to `None`):
                 The preprocessor to use to collect the nodes to include or exclude from quantization.
 
         Returns:
             The path of the resulting quantized model.
         """
         use_qdq = quantization_config.is_static and quantization_config.format == QuantFormat.QDQ
         save_dir = Path(save_dir)
         save_dir.mkdir(parents=True, exist_ok=True)
 
+        if quantization_config.is_static and calibration_tensors_range is None:
+            raise ValueError(
+                "Requested static quantization in the QuantizationConfig, but no calibration ranges were provided. Please run calibration first using the quantizer fit method, or use dynamic quantization."
+            )
         if not quantization_config.is_static:
             if quantization_config.mode != QuantizationMode.IntegerOps:
                 LOGGER.warning(
                     f"ONNX Runtime dynamic quantization mode should be QuantizationMode.IntegerOps "
                     f"(got: {quantization_config.mode})."
                 )
             if quantization_config.activations_dtype != QuantType.QUInt8:
@@ -342,15 +340,24 @@
 
             nodes_to_quantize.update(quantization_config.nodes_to_quantize)
             nodes_to_exclude.update(quantization_config.nodes_to_exclude)
 
             quantization_config.nodes_to_quantize = list(nodes_to_quantize)
             quantization_config.nodes_to_exclude = list(nodes_to_exclude)
 
+        has_subgraphs = False
         onnx_model = onnx.load(Path(self.onnx_model_path).as_posix())
+        for node in onnx_model.graph.node:
+            if node.op_type in ["If", "Loop", "Scan", "SequenceMap"]:
+                has_subgraphs = True
+                break
+
+        if quantization_config.is_static and has_subgraphs:
+            raise NotImplementedError("Static quantization is currently not supported for models with" " subgraphs.")
+
         quantizer_factory = QDQQuantizer if use_qdq else ONNXQuantizer
 
         if parse(ort_version) >= Version("1.13.0"):
             # The argument `input_qType` has been changed into `activation_qType` from ORT 1.13
             quantizer = quantizer_factory(
                 model=onnx_model,
                 static=quantization_config.is_static,
@@ -365,15 +372,15 @@
                 op_types_to_quantize=[
                     operator.value if isinstance(operator, ORTQuantizableOperator) else operator
                     for operator in quantization_config.operators_to_quantize
                 ],
                 extra_options={
                     "WeightSymmetric": quantization_config.weights_symmetric,
                     "ActivationSymmetric": quantization_config.activations_symmetric,
-                    "EnableSubgraph": False,
+                    "EnableSubgraph": has_subgraphs,
                     "ForceSymmetric": quantization_config.activations_symmetric
                     and quantization_config.weights_symmetric,
                     "AddQDQPairToWeight": quantization_config.qdq_add_pair_to_weight,
                     "DedicatedQDQPair": quantization_config.qdq_dedicated_pair,
                     "QDQOpTypePerChannelSupportToAxis": quantization_config.qdq_op_type_per_channel_support_to_axis,
                 },
             )
@@ -438,27 +445,27 @@
         """
         Creates the calibration `datasets.Dataset` to use for the post-training static quantization calibration step.
 
         Args:
             dataset_name (`str`):
                 The dataset repository name on the Hugging Face Hub or path to a local directory containing data files
                 to load to use for the calibration step.
-            num_samples (`int`, *optional*, defaults to 100):
+            num_samples (`int`, defaults to 100):
                 The maximum number of samples composing the calibration dataset.
-            dataset_config_name (`Optional[str]`, *optional*):
+            dataset_config_name (`Optional[str]`, defaults to `None`):
                 The name of the dataset configuration.
-            dataset_split (`Optional[str]`, *optional*):
+            dataset_split (`Optional[str]`, defaults to `None`):
                 Which split of the dataset to use to perform the calibration step.
-            preprocess_function (`Optional[Callable]`, *optional*):
+            preprocess_function (`Optional[Callable]`, defaults to `None`):
                 Processing function to apply to each example after loading dataset.
-            preprocess_batch (`bool`, *optional*, defaults to `True`):
+            preprocess_batch (`bool`, defaults to `True`):
                 Whether the `preprocess_function` should be batched.
-            seed (`int`, *optional*, defaults to 2016):
+            seed (`int`, defaults to 2016):
                 The random seed to use when shuffling the calibration dataset.
-            use_auth_token (`bool`, *optional*, defaults to `False`):
+            use_auth_token (`bool`, defaults to `False`):
                 Whether to use the token generated when running `transformers-cli login` (necessary for some datasets
                 like ImageNet).
         Returns:
             The calibration `datasets.Dataset` to use for the post-training static quantization calibration
             step.
         """
         if dataset_name is None:
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/runs/__init__.py` & `optimum-1.9.0/optimum/onnxruntime/runs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             weights_dtype=QuantType.QInt8,
             per_channel=run_config["per_channel"],
             reduce_range=False,
             operators_to_quantize=run_config["operators_to_quantize"],
         )
 
         onnx_model = ORT_SUPPORTED_TASKS[self.task]["class"][0].from_pretrained(
-            run_config["model_name_or_path"], from_transformers=True
+            run_config["model_name_or_path"], export=True
         )
 
         trfs_model = FeaturesManager.get_model_from_feature(
             onnx_model.export_feature, run_config["model_name_or_path"]
         )
         quantizer = ORTQuantizer.from_pretrained(onnx_model)
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/runs/calibrator.py` & `optimum-1.9.0/optimum/onnxruntime/runs/calibrator.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/runs/utils.py` & `optimum-1.9.0/optimum/onnxruntime/runs/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/trainer.py` & `optimum-1.9.0/optimum/onnxruntime/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -903,15 +903,16 @@
 
         Returns:
             A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
             dictionary also contains the epoch number which comes from the training state.
         """
         # memory metrics - must set up as early as possible
         # TODO: We need to enable evaluation using ORT backend.
-        self.model = unwrap_model(self.model)
+        if self.args.use_module_with_loss:
+            self.model = self.model._original_model
         self._memory_tracker.start()
 
         eval_dataloader = self.get_eval_dataloader(eval_dataset)
         start_time = time.time()
 
         if inference_with_ort:
             logger.info("[INFO] Evaluating with ONNX Runtime backend.")
@@ -996,15 +997,16 @@
 
             - predictions (`np.ndarray`): The predictions on `test_dataset`.
             - label_ids (`np.ndarray`, *optional*): The labels (if the dataset contained some).
             - metrics (`Dict[str, float]`, *optional*): The potential dictionary of metrics (if the dataset contained
               labels).
         """
         # TODO: We need to enable evaluation using ORT backend.
-        self.model = unwrap_model(self.model)
+        if self.args.use_module_with_loss:
+            self.model = self.model._original_model
 
         # memory metrics - must set up as early as possible
         self._memory_tracker.start()
 
         test_dataloader = self.get_test_dataloader(test_dataset)
         start_time = time.time()
```

### Comparing `optimum-1.8.8/optimum/onnxruntime/trainer_seq2seq.py` & `optimum-1.9.0/optimum/onnxruntime/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/training_args.py` & `optimum-1.9.0/optimum/onnxruntime/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/training_args_seq2seq.py` & `optimum-1.9.0/optimum/onnxruntime/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/onnxruntime/utils.py` & `optimum-1.9.0/optimum/onnxruntime/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,16 @@
         "mbart": "bart",
         "mt5": "bart",
         "m2m_100": "bart",
         "nystromformer": "bert",
         "pegasus": "bert",
         "roberta": "bert",
         "t5": "bert",
+        "vit": "vit",
+        "whisper": "bart",
         "xlm-roberta": "bert",
     }
 
     @classmethod
     def get_model_ort_type(cls, model_type: str) -> str:
         cls.check_supported_model(model_type)
         return cls._conf[model_type]
@@ -138,21 +140,32 @@
             raise KeyError(
                 f"{model_type} model type is not supported yet. Only {model_types} are supported. "
                 f"If you want to support {model_type} please propose a PR or open up an issue."
             )
 
     @classmethod
     def check_optimization_supported_model(cls, model_type: str, optimization_config):
-        # as of 1.14.O: https://github.com/microsoft/onnxruntime/blob/6ccaeddefa65ccac402a47fa4d9cad8229794bb2/onnxruntime/python/tools/transformers/optimizer.py#L39
-        supported_model_types_for_optimization = ["bert", "gpt2", "bart", "unet"]
+        # as of 1.15.O: https://github.com/microsoft/onnxruntime/blob/v1.15.0/onnxruntime/python/tools/transformers/optimizer.py#L42
+        supported_model_types_for_optimization = [
+            "bart",
+            "bert",
+            "gpt2",
+            "tnlr",
+            "t5",
+            "unet",
+            "vae",
+            "clip",
+            "vit",
+            "swin",
+        ]
 
         if (model_type not in cls._conf) or (cls._conf[model_type] not in supported_model_types_for_optimization):
             raise NotImplementedError(
                 f"ONNX Runtime doesn't support the graph optimization of {model_type} yet. Only {list(cls._conf.keys())} are supported. "
-                f"If you want to support {model_type} please propose a PR or open up an issue in ONNX Runtime:https://github.com/microsoft/onnxruntime."
+                f"If you want to support {model_type} please propose a PR or open up an issue in ONNX Runtime: https://github.com/microsoft/onnxruntime."
             )
 
 
 def generate_identified_filename(filename, identifier):
     return filename.parent.joinpath(filename.stem + identifier).with_suffix(filename.suffix)
 
 
@@ -247,18 +260,18 @@
 
 def check_io_binding(providers: List[str], use_io_binding: Optional[bool] = None) -> bool:
     """
     Whether to use IOBinding or not.
     """
     if use_io_binding is None and providers[0] == "CUDAExecutionProvider":
         use_io_binding = True
-    elif providers[0] != "CUDAExecutionProvider":
+    elif providers[0] != "CPUExecutionProvider" and providers[0] != "CUDAExecutionProvider":
         if use_io_binding is True:
             logger.warning(
-                "No need to enable IO Binding if the provider used is not CUDAExecutionProvider. IO Binding will be turned off."
+                "No need to enable IO Binding if the provider used is neither CPUExecutionProvider nor CUDAExecutionProvider. IO Binding will be turned off."
             )
         use_io_binding = False
 
     return use_io_binding
 
 
 def get_ordered_input_names(input_names: List[str], func: Callable) -> List[str]:
```

### Comparing `optimum-1.8.8/optimum/pipelines/__init__.py` & `optimum-1.9.0/optimum/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/pipelines/diffusers/pipeline_stable_diffusion.py` & `optimum-1.9.0/optimum/pipelines/diffusers/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/pipelines/diffusers/pipeline_utils.py` & `optimum-1.9.0/optimum/pipelines/diffusers/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/pipelines/pipelines_base.py` & `optimum-1.9.0/optimum/pipelines/pipelines_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
     **kwargs,
 ):
     if model_kwargs is None:
         model_kwargs = {}
 
     if model is None:
         model_id = SUPPORTED_TASKS[targeted_task]["default"]
-        model = SUPPORTED_TASKS[targeted_task]["class"][0].from_pretrained(model_id, from_transformers=True)
+        model = SUPPORTED_TASKS[targeted_task]["class"][0].from_pretrained(model_id, export=True)
     elif isinstance(model, str):
         from ..onnxruntime.modeling_seq2seq import ENCODER_ONNX_FILE_PATTERN, ORTModelForConditionalGeneration
 
         model_id = model
         ort_model_class = SUPPORTED_TASKS[targeted_task]["class"][0]
 
         if issubclass(ort_model_class, ORTModelForConditionalGeneration):
@@ -245,16 +245,16 @@
             model,
             pattern,
             glob_pattern="**/*.onnx",
             subfolder=subfolder,
             use_auth_token=use_auth_token,
             revision=revision,
         )
-        from_transformers = len(onnx_files) == 0
-        model = ort_model_class.from_pretrained(model, from_transformers=from_transformers, **model_kwargs)
+        export = len(onnx_files) == 0
+        model = ort_model_class.from_pretrained(model, export=export, **model_kwargs)
     elif isinstance(model, ORTModel):
         if tokenizer is None and load_tokenizer:
             for preprocessor in model.preprocessors:
                 if isinstance(preprocessor, (PreTrainedTokenizer, PreTrainedTokenizerFast)):
                     tokenizer = preprocessor
                     break
             if tokenizer is None:
```

### Comparing `optimum-1.8.8/optimum/quantization_base.py` & `optimum-1.9.0/optimum/quantization_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/runs_base.py` & `optimum-1.9.0/optimum/runs_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/__init__.py` & `optimum-1.9.0/optimum/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     DIFFUSION_MODEL_VAE_DECODER_SUBFOLDER,
     DIFFUSION_MODEL_VAE_ENCODER_SUBFOLDER,
 )
 from .import_utils import (
     DIFFUSERS_MINIMUM_VERSION,
     ORT_QUANTIZE_MINIMUM_VERSION,
     TORCH_MINIMUM_VERSION,
+    TRANSFORMERS_MINIMUM_VERSION,
     check_if_diffusers_greater,
     check_if_pytorch_greater,
     check_if_transformers_greater,
     is_accelerate_available,
     is_diffusers_available,
     is_onnx_available,
     is_onnxruntime_available,
@@ -40,14 +41,16 @@
     DEFAULT_DUMMY_SHAPES,
     DummyAudioInputGenerator,
     DummyBboxInputGenerator,
     DummyDecoderTextInputGenerator,
     DummyInputGenerator,
     DummyLabelsGenerator,
     DummyPastKeyValuesGenerator,
+    DummyPix2StructInputGenerator,
+    DummyPointsGenerator,
     DummySeq2SeqDecoderTextInputGenerator,
     DummySeq2SeqPastKeyValuesGenerator,
     DummyTextInputGenerator,
     DummyTimestepInputGenerator,
     DummyVisionInputGenerator,
 )
 from .modeling_utils import recurse_getattr, recurse_setattr
```

### Comparing `optimum-1.8.8/optimum/utils/constant.py` & `optimum-1.9.0/optimum/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/doc.py` & `optimum-1.9.0/optimum/utils/doc.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/dummy_diffusers_objects.py` & `optimum-1.9.0/optimum/utils/dummy_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/file_utils.py` & `optimum-1.9.0/optimum/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/import_utils.py` & `optimum-1.9.0/optimum/utils/import_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """Import utilities."""
 
 import importlib.util
 import inspect
 import sys
 from collections import OrderedDict
 from contextlib import contextmanager
+from typing import Union
 
 import numpy as np
 import packaging
 from transformers.utils import is_torch_available
 
 
 # The package importlib_metadata is in a different place, depending on the python version.
@@ -112,27 +113,30 @@
         )
     try:
         yield
     finally:
         pass
 
 
-def check_if_transformers_greater(target_version: str) -> bool:
+def check_if_transformers_greater(target_version: Union[str, packaging.version.Version]) -> bool:
     """
     Checks whether the current install of transformers is greater than or equal to the target version.
 
     Args:
-        target_version (str): version used as the reference for comparison.
+        target_version (`Union[str, packaging.version.Version]`): version used as the reference for comparison.
 
     Returns:
         bool: whether the check is True or not.
     """
     import transformers
 
-    return packaging.version.parse(transformers.__version__) >= packaging.version.parse(target_version)
+    if isinstance(target_version, str):
+        target_version = packaging.version.parse(target_version)
+
+    return packaging.version.parse(transformers.__version__) >= target_version
 
 
 def check_if_diffusers_greater(target_version: str) -> bool:
     """
     Checks whether the current install of diffusers is greater than or equal to the target version.
 
     Args:
```

### Comparing `optimum-1.8.8/optimum/utils/input_generators.py` & `optimum-1.9.0/optimum/utils/input_generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     "batch_size": 2,
     "sequence_length": 16,
     "num_choices": 4,
     # image
     "width": 64,
     "height": 64,
     "num_channels": 3,
+    "point_batch_size": 3,
+    "nb_points_per_image": 2,
     # audio
     "feature_size": 80,
     "nb_max_frames": 3000,
     "audio_sequence_length": 16000,
 }
 
 
@@ -657,7 +659,63 @@
         max_value = self.num_labels if self.num_labels is not None else 0
         if self.sequence_length is None:
             shape = [self.batch_size]
         else:
             shape = [self.batch_size, self.sequence_length]
 
         return self.random_int_tensor(shape, max_value=max_value, framework=framework)
+
+
+class DummyPointsGenerator(DummyInputGenerator):
+    """
+    Generates dummy time step inputs.
+    """
+
+    SUPPORTED_INPUT_NAMES = ("input_points",)
+
+    def __init__(
+        self,
+        task: str,
+        normalized_config: NormalizedConfig,
+        batch_size: int = DEFAULT_DUMMY_SHAPES["batch_size"],
+        point_batch_size: int = DEFAULT_DUMMY_SHAPES["point_batch_size"],
+        nb_points_per_image: int = DEFAULT_DUMMY_SHAPES["nb_points_per_image"],
+        **kwargs,
+    ):
+        self.task = task
+
+        self.batch_size = batch_size
+        self.point_batch_size = point_batch_size
+        self.nb_points_per_image = nb_points_per_image
+
+    def generate(self, input_name: str, framework: str = "pt"):
+        shape = [self.batch_size, self.point_batch_size, self.nb_points_per_image, 2]
+        return self.random_float_tensor(shape, framework=framework)
+
+
+class DummyPix2StructInputGenerator(DummyInputGenerator):
+    """
+    Generates dummy time step inputs.
+    """
+
+    SUPPORTED_INPUT_NAMES = ("flattened_patches",)
+
+    def __init__(
+        self,
+        task: str,
+        normalized_config: NormalizedConfig,
+        batch_size: int = DEFAULT_DUMMY_SHAPES["batch_size"],
+        patch_height: int = 16,
+        patch_width: int = 16,
+        max_patches: int = DEFAULT_DUMMY_SHAPES["sequence_length"],
+        num_channels: int = DEFAULT_DUMMY_SHAPES["num_channels"],
+        **kwargs,
+    ):
+        self.task = task
+
+        self.batch_size = batch_size
+        self.flattened_patch_size = 2 + patch_height * patch_width * num_channels
+        self.max_patches = max_patches
+
+    def generate(self, input_name: str, framework: str = "pt"):
+        shape = [self.batch_size, self.max_patches, self.flattened_patch_size]
+        return self.random_float_tensor(shape, framework=framework)
```

### Comparing `optimum-1.8.8/optimum/utils/logging.py` & `optimum-1.9.0/optimum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/modeling_utils.py` & `optimum-1.9.0/optimum/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/normalized_config.py` & `optimum-1.9.0/optimum/utils/normalized_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,29 @@
                 )
 
     @classmethod
     def with_args(cls, allow_new: bool = False, **kwargs) -> Callable[[PretrainedConfig], "NormalizedConfig"]:
         return functools.partial(cls, allow_new=allow_new, **kwargs)
 
     def __getattr__(self, attr_name):
+        if attr_name == "config":
+            return super().__getattr__(attr_name)
+
+        try:
+            attr_name = super().__getattribute__(attr_name.upper())
+        except AttributeError:  # e.g. in the NormalizedTextAndVisionConfig case
+            pass
+
         attr_name = attr_name.split(".")
         leaf_attr_name = attr_name[-1]
         config = self.config
         for attr in attr_name[:-1]:
             config = getattr(config, attr)
 
-        attr = getattr(config, super().__getattribute__(leaf_attr_name.upper()), None)
+        attr = getattr(config, leaf_attr_name, None)
 
         # If the attribute was not specified manually, try to fallback on the attribute_map.
         if attr is None:
             attribute_map = getattr(self.config, "attribute_map", {})
             attr = getattr(self.config, attribute_map.get(leaf_attr_name, ""), None)
 
         if attr is None:
@@ -125,14 +133,18 @@
 )
 
 GPT2LikeNormalizedTextConfig = NormalizedTextConfig.with_args(num_attention_heads="n_head", hidden_size="n_embd")
 T5LikeNormalizedTextConfig = NormalizedTextConfig.with_args(
     num_attention_heads="num_heads",
     hidden_size="d_model",
 )
+MPTNormalizedTextConfig = NormalizedTextConfig.with_args(
+    num_attention_heads="n_heads", hidden_size="d_model", num_layers="n_layers"
+)
+
 WhisperLikeNormalizedTextConfig = NormalizedTextConfig.with_args(
     hidden_size="d_model",
 )
 
 TrOCRLikeNormalizedTextConfig = NormalizedSeq2SeqConfig.with_args(
     decoder_num_layers="decoder_layers",
     num_layers="decoder_layers",
@@ -189,14 +201,15 @@
         # "big_bird": NormalizedTextConfig,
         # "bigbird_pegasus": BartLikeNormalizedTextConfig,
         "blenderbot": BartLikeNormalizedTextConfig,
         "blenderbot_small": BartLikeNormalizedTextConfig,
         "bloom": NormalizedTextConfig.with_args(num_layers="n_layer"),
         "camembert": NormalizedTextConfig,
         "codegen": GPT2LikeNormalizedTextConfig,
+        "cvt": NormalizedVisionConfig,
         "deberta": NormalizedTextConfig,
         "deberta-v2": NormalizedTextConfig,
         "deit": NormalizedVisionConfig,
         "distilbert": NormalizedTextConfig.with_args(num_attention_heads="n_heads", hidden_size="dim"),
         "donut-swin": NormalizedVisionConfig,
         "electra": NormalizedTextConfig,
         "gpt2": GPT2LikeNormalizedTextConfig,
@@ -209,27 +222,29 @@
         "marian": BartLikeNormalizedTextConfig,
         "mbart": BartLikeNormalizedTextConfig,
         "mt5": T5LikeNormalizedTextConfig,
         "m2m_100": BartLikeNormalizedTextConfig,
         "nystromformer": NormalizedTextConfig,
         "opt": NormalizedTextConfig,
         "pegasus": BartLikeNormalizedTextConfig,
+        "pix2struct": NormalizedVisionConfig,
         "poolformer": NormalizedVisionConfig,
         "regnet": NormalizedVisionConfig,
         "resnet": NormalizedVisionConfig,
         "roberta": NormalizedTextConfig,
         "speech_to_text": SpeechToTextLikeNormalizedTextConfig,
         "splinter": NormalizedTextConfig,
         "t5": T5LikeNormalizedTextConfig,
         "trocr": TrOCRLikeNormalizedTextConfig,
         "whisper": WhisperLikeNormalizedTextConfig,
         "vision-encoder-decoder": NormalizedEncoderDecoderConfig,
         "vit": NormalizedVisionConfig,
         "xlm-roberta": NormalizedTextConfig,
         "yolos": NormalizedVisionConfig,
+        "mpt": MPTNormalizedTextConfig,
     }
 
     @classmethod
     def check_supported_model(cls, model_type: str):
         if model_type not in cls._conf:
             model_types = ", ".join(cls._conf.keys())
             raise KeyError(
```

### Comparing `optimum-1.8.8/optimum/utils/preprocessing/__init__.py` & `optimum-1.9.0/optimum/utils/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/preprocessing/base.py` & `optimum-1.9.0/optimum/utils/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/preprocessing/image_classification.py` & `optimum-1.9.0/optimum/utils/preprocessing/image_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/preprocessing/question_answering.py` & `optimum-1.9.0/optimum/utils/preprocessing/question_answering.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/preprocessing/task_processors_manager.py` & `optimum-1.9.0/optimum/utils/preprocessing/task_processors_manager.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/preprocessing/text_classification.py` & `optimum-1.9.0/optimum/utils/preprocessing/text_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/preprocessing/token_classification.py` & `optimum-1.9.0/optimum/utils/preprocessing/token_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/runs.py` & `optimum-1.9.0/optimum/utils/runs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/save_utils.py` & `optimum-1.9.0/optimum/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/utils/testing_utils.py` & `optimum-1.9.0/optimum/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/optimum/version.py` & `optimum-1.9.0/optimum/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.8.8"
+__version__ = "1.9.0"
```

### Comparing `optimum-1.8.8/optimum.egg-info/PKG-INFO` & `optimum-1.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,7 @@
-Metadata-Version: 2.1
-Name: optimum
-Version: 1.8.8
-Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
-Home-page: https://github.com/huggingface/optimum
-Author: HuggingFace Inc. Special Ops Team
-Author-email: hardware@huggingface.co
-License: Apache
-Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: onnxruntime
-Provides-Extra: onnxruntime-gpu
-Provides-Extra: exporters
-Provides-Extra: exporters-gpu
-Provides-Extra: exporters-tf
-Provides-Extra: intel
-Provides-Extra: openvino
-Provides-Extra: nncf
-Provides-Extra: neural-compressor
-Provides-Extra: graphcore
-Provides-Extra: habana
-Provides-Extra: neuron
-Provides-Extra: neuronx
-Provides-Extra: dev
-Provides-Extra: tests
-Provides-Extra: quality
-Provides-Extra: benchmark
-License-File: LICENSE
-
 [![ONNX Runtime](https://github.com/huggingface/optimum/actions/workflows/test_onnxruntime.yml/badge.svg)](https://github.com/huggingface/optimum/actions/workflows/test_onnxruntime.yml)
 
 # Hugging Face Optimum
 
 🤗 Optimum is an extension of 🤗 Transformers and Diffusers, providing a set of optimization tools enabling maximum efficiency to train and run models on targeted hardware, while keeping things easy to use.
 
 ## Installation
@@ -82,26 +42,72 @@
 - [OpenVINO](https://huggingface.co/docs/optimum/intel/inference)
 - Habana first-gen Gaudi / Gaudi2, more details [here](https://huggingface.co/docs/optimum/main/en/habana/usage_guides/accelerate_inference)
 
 The [export](https://huggingface.co/docs/optimum/exporters/overview) and optimizations can be done both programmatically and with a command line.
 
 ### Features summary
 
-| Features                           | ONNX Runtime       | Neural Compressor  | OpenVINO           | TensorFlow Lite    |
+| Features                           | [ONNX Runtime](https://huggingface.co/docs/optimum/main/en/onnxruntime/overview)| [Neural Compressor](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc)| [OpenVINO](https://huggingface.co/docs/optimum/main/en/intel/inference)| [TensorFlow Lite](https://huggingface.co/docs/optimum/main/en/exporters/tflite/overview)|
 |:----------------------------------:|:------------------:|:------------------:|:------------------:|:------------------:|
 | Graph optimization                 | :heavy_check_mark: | N/A                | :heavy_check_mark: | N/A                |
 | Post-training dynamic quantization | :heavy_check_mark: | :heavy_check_mark: | N/A                | :heavy_check_mark: |
 | Post-training static quantization  | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 | Quantization Aware Training (QAT)  | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 | FP16 (half precision)              | :heavy_check_mark: | N/A                | :heavy_check_mark: | :heavy_check_mark: |
 | Pruning                            | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 | Knowledge Distillation             | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 
+
+### OpenVINO
+
+This requires to install the OpenVINO extra by doing `pip install optimum[openvino,nncf]`
+
+To load a model and run inference with OpenVINO Runtime, you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class. To load a PyTorch checkpoint and convert it to the OpenVINO format on-the-fly, you can set `export=True` when loading your model.
+
+```diff
+- from transformers import AutoModelForSequenceClassification
++ from optimum.intel import OVModelForSequenceClassification
+  from transformers import AutoTokenizer, pipeline
+
+  model_id = "distilbert-base-uncased-finetuned-sst-2-english"
+  tokenizer = AutoTokenizer.from_pretrained(model_id)
+- model = AutoModelForSequenceClassification.from_pretrained(model_id)
++ model = OVModelForSequenceClassification.from_pretrained(model_id, export=True)
+  model.save_pretrained("./distilbert")
+
+  classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
+  results = classifier("He's a dreadful magician.")
+```
+
+You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/inference) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/openvino).
+
+### Neural Compressor
+
+This requires to install the Neural Compressor extra by doing `pip install optimum[neural-compressor]`
+
+Dynamic quantization can be applied on your model:
+
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
+```
+
+To load a model quantized with Intel Neural Compressor, hosted locally or on the 🤗 hub, you can do as follows :
+```python
+from optimum.intel import INCModelForSequenceClassification
+
+model_id = "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
+model = INCModelForSequenceClassification.from_pretrained(model_id)
+```
+
+You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/optimization_inc) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/neural_compressor).
+
 ### ONNX + ONNX Runtime
 
+This requires to install the ONNX Runtime extra by doing `pip install optimum[exporters,onnxruntime]`
+
 It is possible to export 🤗 Transformers models to the [ONNX](https://onnx.ai/) format and perform graph optimization as well as quantization easily:
 
 ```plain
 optimum-cli export onnx -m deepset/roberta-base-squad2 --optimize O2 roberta_base_qa_onnx
 ```
 
 The model can then be quantized using `onnxruntime`:
@@ -117,82 +123,56 @@
 
 For more information on the ONNX export, please check the [documentation](https://huggingface.co/docs/optimum/exporters/onnx/usage_guides/export_a_model).
 
 #### Run the exported model using ONNX Runtime
 
 Once the model is exported to the ONNX format, we provide Python classes enabling you to run the exported ONNX model in a seemless manner using [ONNX Runtime](https://onnxruntime.ai/) in the backend:
 
-```python
-from transformers import AutoTokenizer
-from optimum.onnxruntime import ORTModelForQuestionAnswering
-
-model_name = "roberta_base_qa_onnx"
-tokenizer = AutoTokenizer.from_pretrained(model_name)
-ort_model = ORTModelForQuestionAnswering.from_pretrained(model_name)
-
-question = "What's Optimum?"
-text = "Optimum is an awesome library everyone should use!"
-inputs = tokenizer(question, text, return_tensors="pt") 
-
-# Run with ONNX Runtime.
-outputs = ort_model(**inputs)
-
-answer_start_index = outputs.start_logits.argmax()
-answer_end_index = outputs.end_logits.argmax()
+```diff
+- from transformers import AutoModelForQuestionAnswering
++ from optimum.onnxruntime import ORTModelForQuestionAnswering
+  from transformers import AutoTokenizer, pipeline
 
-predict_answer_tokens = inputs.input_ids[0, answer_start_index : answer_end_index + 1]
-answer = tokenizer.decode(predict_answer_tokens, skip_special_tokens=True)
+  model_id = "deepset/roberta-base-squad2"
+  tokenizer = AutoTokenizer.from_pretrained(model_id)
+- model = AutoModelForQuestionAnswering.from_pretrained(model_id)
++ model = ORTModelForQuestionAnswering.from_pretrained("roberta_base_qa_onnx")
+  qa_pipe = pipeline("question-answering", model=model, tokenizer=tokenizer)
+  question = "What's Optimum?"
+  context = "Optimum is an awesome library everyone should use!"
+  results = qa_pipe(question=question, context=context)
 ```
 
 More details on how to run ONNX models with `ORTModelForXXX` classes [here](https://huggingface.co/docs/optimum/main/en/onnxruntime/usage_guides/models).
 
 ### TensorFlow Lite
 
+This requires to install the Exporters extra by doing `pip install optimum[exporters-tf]`
+
 Just as for ONNX, it is possible to export models to [TensorFlow Lite](https://www.tensorflow.org/lite) and quantize them:
 
 ```plain
 optimum-cli export tflite \
   -m deepset/roberta-base-squad2 \
   --sequence_length 384  \
   --quantize int8-dynamic roberta_tflite_model
 ```
-### OpenVINO
-
-*This requires to install the Optimum OpenVINO extra by doing `pip install optimum[openvino,nncf]`.*
-
-To load a model and run inference with [OpenVINO Runtime](https://docs.openvino.ai/latest/home.html), you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class. To load a PyTorch checkpoint and convert it to the OpenVINO format on-the-fly, you can set `export=True` when loading your model.
-
-```diff
-- from transformers import AutoModelForSequenceClassification
-+ from optimum.intel import OVModelForSequenceClassification
-  from transformers import AutoTokenizer, pipeline
-
-  model_id = "distilbert-base-uncased-finetuned-sst-2-english"
-  tokenizer = AutoTokenizer.from_pretrained(model_id)
-- model = AutoModelForSequenceClassification.from_pretrained(model_id)
-+ model = OVModelForSequenceClassification.from_pretrained(model_id, export=True)
-  model.save_pretrained("./distilbert")
-
-  classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
-  results = classifier("He's a dreadful magician.")
-```
-
-You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/inference) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/openvino).
-
 
 ## Accelerated training
 
 🤗 Optimum provides wrappers around the original 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer) to enable training on powerful hardware easily.
 We support many providers:
 
 - Habana's Gaudi processors
 - ONNX Runtime (optimized for GPUs)
 
 ### Habana
 
+This requires to install the Habana extra by doing `pip install optimum[habana]`
+
 ```diff
 - from transformers import Trainer, TrainingArguments
 + from optimum.habana import GaudiTrainer, GaudiTrainingArguments
 
   # Download a pretrained model from the Hub
   model = AutoModelForXxx.from_pretrained("bert-base-uncased")
```

### Comparing `optimum-1.8.8/optimum.egg-info/SOURCES.txt` & `optimum-1.9.0/optimum.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 optimum/bettertransformer/models/encoder_models.py
 optimum/commands/__init__.py
 optimum/commands/base.py
 optimum/commands/env.py
 optimum/commands/optimum_cli.py
 optimum/commands/export/__init__.py
 optimum/commands/export/base.py
+optimum/commands/export/ggml.py
 optimum/commands/export/onnx.py
 optimum/commands/export/tflite.py
 optimum/commands/onnxruntime/__init__.py
 optimum/commands/onnxruntime/base.py
 optimum/commands/onnxruntime/optimize.py
 optimum/commands/onnxruntime/quantize.py
 optimum/commands/register/__init__.py
@@ -116,8 +117,10 @@
 optimum/utils/testing_utils.py
 optimum/utils/preprocessing/__init__.py
 optimum/utils/preprocessing/base.py
 optimum/utils/preprocessing/image_classification.py
 optimum/utils/preprocessing/question_answering.py
 optimum/utils/preprocessing/task_processors_manager.py
 optimum/utils/preprocessing/text_classification.py
-optimum/utils/preprocessing/token_classification.py
+optimum/utils/preprocessing/token_classification.py
+tests/test_configuration_utils.py
+tests/test_modeling_base.py
```

### Comparing `optimum-1.8.8/optimum.egg-info/requires.txt` & `optimum-1.9.0/optimum.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 coloredlogs
 sympy
 transformers[sentencepiece]>=4.26.0
 torch>=1.9
-torchvision
 packaging
 numpy
 huggingface_hub>=0.8.0
 datasets
 
 [benchmark]
 optuna
@@ -23,23 +22,23 @@
 pytest-xdist
 Pillow
 sacremoses
 torchvision
 diffusers>=0.17.0
 torchaudio
 black~=23.1
-ruff>=0.0.241
+ruff<=0.0.259,>=0.0.241
 
 [exporters]
-onnx<1.14.0
+onnx
 onnxruntime
 timm
 
 [exporters-gpu]
-onnx<1.14.0
+onnx
 onnxruntime-gpu
 timm
 
 [exporters-tf]
 tensorflow<2.11,>=2.4
 tf2onnx
 onnx
@@ -67,33 +66,33 @@
 [neuronx]
 optimum-neuron[neuronx]
 
 [nncf]
 optimum-intel[nncf]
 
 [onnxruntime]
-onnx<1.14.0
+onnx
 onnxruntime>=1.9.0
 datasets>=1.2.1
 evaluate
 protobuf>=3.20.1
 
 [onnxruntime-gpu]
-onnx<1.14.0
+onnx
 onnxruntime-gpu>=1.9.0
 datasets>=1.2.1
 evaluate
 protobuf>=3.20.1
 
 [openvino]
 optimum-intel[openvino]
 
 [quality]
 black~=23.1
-ruff>=0.0.241
+ruff<=0.0.259,>=0.0.241
 
 [tests]
 pytest
 requests
 parameterized
 pytest-xdist
 Pillow
```

### Comparing `optimum-1.8.8/pyproject.toml` & `optimum-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-1.8.8/setup.py` & `optimum-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 REQUIRED_PKGS = [
     "coloredlogs",
     "sympy",
     "transformers[sentencepiece]>=4.26.0",
     "torch>=1.9",
-    "torchvision",
     "packaging",
     "numpy",
     "huggingface_hub>=0.8.0",
     "datasets",
 ]
 
 TESTS_REQUIRE = [
@@ -32,35 +31,35 @@
     "Pillow",
     "sacremoses",
     "torchvision",
     "diffusers>=0.17.0",
     "torchaudio",
 ]
 
-QUALITY_REQUIRE = ["black~=23.1", "ruff>=0.0.241"]
+QUALITY_REQUIRE = ["black~=23.1", "ruff>=0.0.241,<=0.0.259"]
 
 BENCHMARK_REQUIRE = ["optuna", "tqdm", "scikit-learn", "seqeval", "torchvision", "evaluate>=0.2.0"]
 
 EXTRAS_REQUIRE = {
     "onnxruntime": [
-        "onnx<1.14.0",
+        "onnx",
         "onnxruntime>=1.9.0",
         "datasets>=1.2.1",
         "evaluate",
         "protobuf>=3.20.1",
     ],
     "onnxruntime-gpu": [
-        "onnx<1.14.0",
+        "onnx",
         "onnxruntime-gpu>=1.9.0",
         "datasets>=1.2.1",
         "evaluate",
         "protobuf>=3.20.1",
     ],
-    "exporters": ["onnx<1.14.0", "onnxruntime", "timm"],
-    "exporters-gpu": ["onnx<1.14.0", "onnxruntime-gpu", "timm"],
+    "exporters": ["onnx", "onnxruntime", "timm"],
+    "exporters-gpu": ["onnx", "onnxruntime-gpu", "timm"],
     "exporters-tf": ["tensorflow>=2.4,<2.11", "tf2onnx", "onnx", "onnxruntime", "timm", "h5py", "numpy<1.24.0"],
     "intel": "optimum-intel",
     "openvino": "optimum-intel[openvino]",
     "nncf": "optimum-intel[nncf]",
     "neural-compressor": "optimum-intel[neural-compressor]",
     "graphcore": "optimum-graphcore",
     "habana": ["transformers<4.29.0", "optimum-habana"],
```

