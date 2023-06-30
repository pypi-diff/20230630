# Comparing `tmp/sparseml_nightly-1.6.0.20230623-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230629-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,374 +1,377 @@
-Zip file size: 959522 bytes, number of entries: 372
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-23 01:31 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-23 01:31 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-23 01:31 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-23 01:31 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-23 01:31 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jun-23 01:31 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-23 01:31 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-23 01:31 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-23 01:31 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-23 01:31 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-23 01:31 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-23 01:31 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-23 01:31 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-23 01:31 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-23 01:31 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-23 01:31 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     6058 b- defN 23-Jun-23 01:31 sparseml/exporters/kv_cache_injector.py
--rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-23 01:31 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2276 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4866 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4681 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/kv_cache/__init__.py
--rw-rw-r--  2.0 unx    20939 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
--rw-rw-r--  2.0 unx     6763 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx    10570 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-23 01:31 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-23 01:31 sparseml/framework/info.py
--rw-rw-r--  2.0 unx     1144 b- defN 23-Jun-23 01:31 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-23 01:31 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jun-23 01:31 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-23 01:31 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-23 01:31 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-23 01:31 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-23 01:31 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-23 01:31 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jun-23 01:31 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-23 01:31 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-23 01:31 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-23 01:31 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-23 01:31 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-23 01:31 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-23 01:31 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jun-23 01:31 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-23 01:31 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jun-23 01:31 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-23 01:31 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-23 01:31 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-23 01:31 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-23 01:31 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-23 01:31 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-23 01:31 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-23 01:31 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jun-23 01:31 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-23 01:31 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jun-23 01:31 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-23 01:31 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jun-23 01:31 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-23 01:31 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-23 01:31 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-23 01:31 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jun-23 01:31 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-23 01:31 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-23 01:31 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-23 01:31 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jun-23 01:31 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-23 01:31 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-23 01:31 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-23 01:31 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-23 01:31 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-23 01:31 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     2190 b- defN 23-Jun-23 01:31 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6117 b- defN 23-Jun-23 01:31 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jun-23 01:31 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10884 b- defN 23-Jun-23 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jun-23 01:31 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-23 01:31 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20676 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jun-23 01:31 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-23 01:31 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-23 01:31 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-23 01:31 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17905 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    76796 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-23 01:31 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-23 01:31 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-23 01:31 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-23 01:31 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-23 01:31 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-23 01:31 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-23 01:31 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-23 01:31 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-23 01:31 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-23 01:31 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-23 01:31 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-23 01:31 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-23 01:31 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-23 01:31 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-23 01:31 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    21290 b- defN 23-Jun-23 01:31 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-23 01:31 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-23 01:31 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-23 01:31 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-23 01:31 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-23 01:31 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-23 01:31 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-23 01:31 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-23 01:31 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jun-23 01:31 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-23 01:31 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-23 01:31 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-23 01:31 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-23 01:31 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jun-23 01:31 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26562 b- defN 23-Jun-23 01:31 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-23 01:31 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-23 01:31 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-23 01:31 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-23 01:31 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-23 01:31 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-23 01:31 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-23 01:31 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-23 01:31 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-23 01:31 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-23 01:31 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-23 01:31 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-23 01:31 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-23 01:31 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-23 01:31 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-23 01:31 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-23 01:31 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-23 01:31 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    35086 b- defN 23-Jun-23 01:31 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-23 01:31 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-23 01:31 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jun-23 01:31 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-23 01:31 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-23 01:31 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21712 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    37031 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/RECORD
-372 files, 3472697 bytes uncompressed, 899562 bytes compressed:  74.1%
+Zip file size: 965532 bytes, number of entries: 375
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-29 01:31 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-29 01:31 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-29 01:31 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-29 01:31 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-29 01:31 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jun-29 01:31 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17763 b- defN 23-Jun-29 01:31 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-29 01:31 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jun-29 01:31 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-29 01:31 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-29 01:31 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-29 01:31 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-29 01:31 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-29 01:31 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-29 01:31 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-29 01:31 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     6325 b- defN 23-Jun-29 01:31 sparseml/exporters/kv_cache_injector.py
+-rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-29 01:31 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2276 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4866 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4681 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      909 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/__init__.py
+-rw-rw-r--  2.0 unx    26599 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
+-rw-rw-r--  2.0 unx     6192 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/configs.py
+-rw-rw-r--  2.0 unx     1660 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
+-rw-rw-r--  2.0 unx     3377 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
+-rw-rw-r--  2.0 unx     4951 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx    10570 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-29 01:31 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-29 01:31 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Jun-29 01:31 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-29 01:31 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jun-29 01:31 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-29 01:31 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-29 01:31 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-29 01:31 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-29 01:31 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-29 01:31 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jun-29 01:31 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-29 01:31 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-29 01:31 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-29 01:31 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-29 01:31 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-29 01:31 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-29 01:31 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jun-29 01:31 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-29 01:31 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jun-29 01:31 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-29 01:31 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-29 01:31 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-29 01:31 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-29 01:31 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-29 01:31 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-29 01:31 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-29 01:31 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jun-29 01:31 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-29 01:31 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jun-29 01:31 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-29 01:31 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jun-29 01:31 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-29 01:31 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-29 01:31 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-29 01:31 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    18825 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jun-29 01:31 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-29 01:31 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-29 01:31 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-29 01:31 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jun-29 01:31 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-29 01:31 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-29 01:31 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-29 01:31 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-29 01:31 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-29 01:31 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     2190 b- defN 23-Jun-29 01:31 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6155 b- defN 23-Jun-29 01:31 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-29 01:31 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10884 b- defN 23-Jun-29 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jun-29 01:31 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-29 01:31 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20676 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jun-29 01:31 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-29 01:31 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-29 01:31 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-29 01:31 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17905 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    76796 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-29 01:31 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-29 01:31 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-29 01:31 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-29 01:31 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-29 01:31 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-29 01:31 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-29 01:31 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-29 01:31 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-29 01:31 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-29 01:31 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-29 01:31 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-29 01:31 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-29 01:31 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-29 01:31 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-29 01:31 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    21290 b- defN 23-Jun-29 01:31 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-29 01:31 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-29 01:31 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-29 01:31 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-29 01:31 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-29 01:31 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-29 01:31 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-29 01:31 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-29 01:31 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jun-29 01:31 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-29 01:31 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-29 01:31 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-29 01:31 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jun-29 01:31 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jun-29 01:31 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26562 b- defN 23-Jun-29 01:31 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-29 01:31 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-29 01:31 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-29 01:31 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-29 01:31 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-29 01:31 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-29 01:31 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-29 01:31 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-29 01:31 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-29 01:31 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-29 01:31 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-29 01:31 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-29 01:31 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-29 01:31 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-29 01:31 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-29 01:31 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-29 01:31 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-29 01:31 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    35106 b- defN 23-Jun-29 01:31 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-29 01:31 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-29 01:31 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jun-29 01:31 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-29 01:31 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-29 01:31 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21775 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2326 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    37382 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/RECORD
+375 files, 3491114 bytes uncompressed, 904984 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -129,15 +129,24 @@
 
 Filename: sparseml/exporters/transforms/kv_cache/__init__.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
 Comment: 
 
-Filename: sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py
+Filename: sparseml/exporters/transforms/kv_cache/configs.py
+Comment: 
+
+Filename: sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
+Comment: 
+
+Filename: sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
+Comment: 
+
+Filename: sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/utils/__init__.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
 Comment: 
@@ -1089,29 +1098,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230623.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230629.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230623.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230629.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230623.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230629.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230623.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230629.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230623.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230629.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230623.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230629.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230623.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230629.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/benchmark/info.py

```diff
@@ -100,15 +100,15 @@
 from sparseml.benchmark.serialization import (
     BatchBenchmarkResult,
     BenchmarkConfig,
     BenchmarkInfo,
     BenchmarkResult,
 )
 from sparseml.framework.info import FrameworkInferenceProviderInfo, FrameworkInfo
-from sparseml.utils import clean_path, create_parent_dirs
+from sparseml.utils import clean_path, create_parent_dirs, deprecation_warning
 from sparseml.utils.helpers import convert_to_bool
 
 
 __all__ = [
     "BenchmarkRunner",
     "save_benchmark_results",
     "load_benchmark_info",
@@ -540,14 +540,17 @@
         help=("If specified, will show the progress of the benchmark."),
     )
 
     return parser.parse_args()
 
 
 def _main():
+    deprecation_warning(
+        message=f"{__file__} is scheduled for deprecation in a future version",
+    )
     args = _parse_args()
     save_benchmark_results(
         model=args.model,
         data=args.data,
         batch_size=args.batch_size,
         iterations=args.iterations,
         warmup_iterations=args.warmup_iterations,
```

## sparseml/exporters/kv_cache_injector.py

```diff
@@ -8,139 +8,113 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import logging
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import onnx
 
 from sparseml.exporters.base_exporter import BaseExporter
+from sparseml.exporters.transforms import OnnxTransform
 from sparseml.exporters.transforms.kv_cache import (
     CacheKeysAndValues,
-    PositionEmbeddingsAdjustment,
+    KeyValueCacheConfig,
+    get_kv_cache_config,
 )
 from sparsezoo.utils import save_onnx
 
 
 _LOGGER = logging.getLogger(__name__)
 
-_SUPPORTED_ARCHITECTURES = ["opt"]
-
 
 class KeyValueCacheInjector(BaseExporter):
     def __init__(
         self,
         model_path: Optional[str] = None,
         inplace: bool = True,
         **kwargs: Any,
     ):
         """
         A transformation that injects Key Value cache support into the model.
-        This means that the autoregressive model takes as an input / returns
-        as an output a cache of key value pairs that are used to speed up the
-        autoregressive generation process (reduce the compute of key/value pairs
-        by storing the results of previous computations in memory).
-
-        The exporter will look for a `config.json` file in the `model_path` directory
-        to determine the values:
-        - num_attention_heads
-        - hidden_size_kv_cache
-        required to enforce static dimensions of the kv cache input/output.
-        If `model_path` is not provided, the two aforementioned values must
-        be provided in the `kwargs`.
-
-        This transformation not only injects the cache support, but also adjusts
-        the model to account for the cache support. This means altering the input
-        to the model, such as altering the positions to account for the injected
-        key/value pairs.
+        This means that the
+        - autoregressive model that
+            * takes input_ids and attention_mask as INPUT
+            * returns logits as OUTPUT
+        - is transformed into a model that
+            * takes input_ids, attention_mask, and kv_cache as INPUT
+            * returns logits and updated kv_cache as OUTPUT
+
+        The goal of the KV cache injection is speed up the autoregressive
+        generation process (reduce the compute of key/value pairs by storing
+        the results of previous computations in memory).
+
+        The exporter will look for a `config.json` file in the `model_path`
+        directory to determine the parameters for KV cache injection.
+        If `model_path` is not provided, the requested parameters can be
+        provided in the `kwargs`.
+
+        This transformation not only solely injects the kv cache
+        inputs/outputs, but also adjusts the original ONNX graph to
+        account for the necessary changes. This involves e.g. adding
+        the 'position' input to the model, so that the positional
+        embeddings of the new model are compatible with the past kv
+        cache information.
 
         Usage:
         ```python
         onnx_model: onnx.ModelProto = ...
         exporter = KeyValueCacheInjector(model_path="path/to/model")
-        # alternatively
-        # exporter = KeyValueCacheInjector(num_attention_heads = 16,
-        #                                  hidden_size_dim = 64)
+        exporter.export(onnx_model, "model.onnx")
+        ```
+
+        Alternatively:
+        ```python
+        onnx_model: onnx.ModelProto = ...
+        exporter = KeyValueCacheInjector(model_path="path/to/model")
+        exporter = KeyValueCacheInjector(num_attention_heads = 16,
+                                         hidden_size_dim = 64)
         exporter.export(onnx_model, "model.onnx")
         ```
 
         You can also just optimize the model directly without saving to disk:
         ```python
         onnx_model: onnx.ModelProto = ...
         exporter = KeyValueCacheInjector(model_path="path/to/model")
         optimized_model = exporter.apply(onnx_model)
         ```
 
         :param model_path: The path to the directory containing the model.
         :param inplace: If True, the model will be modified in place.
             If False, a copy of the model will be made and modified.
+        :param kwargs: (Optionally) the parameters for the KV cache injection
+            if no `model_path` is provided.
         """
         self.inplace = inplace
-        if model_path:
-            self.config = self.get_config(model_path)
-            if not self.config["model_type"] in _SUPPORTED_ARCHITECTURES:
-                raise ValueError(
-                    f"Model type {self.config.model_type} is currently not supported. "
-                    f"Supported model types: {_SUPPORTED_ARCHITECTURES}."
-                    f"Proceeding with transformation, but may require additional "
-                    f"customization..."
-                )
 
-            num_attention_heads = self.config["num_attention_heads"]
-            hidden_size_kv_cache = self.config["hidden_size"] // num_attention_heads
-        elif kwargs:
-            num_attention_heads = kwargs.get("num_attention_heads")
-            hidden_size_kv_cache = kwargs.get("hidden_size_kv_cache")
-        else:
-            raise ValueError(
-                "Either `model_path` or `kwargs` must be provided to the "
-                "KeyValueCacheInjector."
-            )
+        config = get_kv_cache_config(model_path)
 
-        transforms = [
-            CacheKeysAndValues(
-                num_attention_heads=num_attention_heads,
-                hidden_size_kv_cache=hidden_size_kv_cache,
-            ),
-            PositionEmbeddingsAdjustment(),
-        ]
+        if config is not None:
+            transforms = self._get_transforms_from_config(config)
 
-        super().__init__(transforms)
-
-    def get_config(self, model_path: Union[str, Path]) -> Dict[str, Any]:
-        """
-        From the model path, get the config.json file and return it as a dict.
-
-        :param model_path: The path to the directory containing the model.
-        :return: The config.json file as a dict.
-        """
-        model_path = Path(model_path) if isinstance(model_path, str) else model_path
+        elif kwargs:
+            transforms = self._get_transforms_from_kwargs(kwargs)
 
-        if not model_path.is_dir():
+        else:
             raise ValueError(
-                f"`model_path` is expected to be a directory, found {model_path}"
+                "Either `model_path` or kwargs must be provided to "
+                "KeyValueCacheInjector"
             )
-        config_file = [
-            file for file in model_path.iterdir() if file.name == "config.json"
-        ]
-        config_file = config_file[0]
-
-        _LOGGER.info(f"Found config file {config_file}")
 
-        with open(config_file) as f:
-            config = json.load(f)
-
-        return config
+        super().__init__(transforms)
 
     def pre_validate(self, model: Union[onnx.ModelProto, str, Path]) -> onnx.ModelProto:
         if isinstance(model, (str, Path)):
             model = onnx.load(str(model))
 
         if not isinstance(model, onnx.ModelProto):
             raise TypeError(f"Expected onnx.ModelProto, found {type(model)}")
@@ -150,7 +124,40 @@
         if not isinstance(model, onnx.ModelProto):
             raise TypeError(f"Expected onnx.ModelProto, found {type(model)}")
         return model
 
     def export(self, pre_transforms_model: onnx.ModelProto, file_path: str):
         post_transforms_model: onnx.ModelProto = self.apply(pre_transforms_model)
         save_onnx(post_transforms_model, file_path)
+
+    @staticmethod
+    def _get_transforms_from_config(config: KeyValueCacheConfig) -> List[OnnxTransform]:
+        positions_adjustment = config.positions_adjustment_transform
+
+        transforms = [
+            CacheKeysAndValues(
+                num_attention_heads=config.num_attention_heads,
+                hidden_size_kv_cache=config.hidden_size_kv_cache,
+                multiply_batch_by_num_att_heads=config.multiply_batch_by_num_att_heads,
+                transpose_value_input=config.transpose_value_input,
+                transpose_key_input=config.transpose_key_input,
+            )
+        ]
+        if positions_adjustment is not None:
+            transforms += [positions_adjustment()]
+
+        return transforms
+
+    @staticmethod
+    def _get_transforms_from_kwargs(kwargs: Dict[str, Any]) -> List[OnnxTransform]:
+        transforms = [
+            CacheKeysAndValues(
+                num_attention_heads=kwargs.get("num_attention_heads"),
+                hidden_size_kv_cache=kwargs.get("hidden_size_kv_cache"),
+                multiply_batch_by_num_att_heads=kwargs.get(
+                    "multiply_batch_by_num_att_heads", False
+                ),
+                transpose_value_input=kwargs.get("transpose_value_input", None),
+                transpose_key_input=kwargs.get("transpose_key_input", None),
+            )
+        ]
+        return transforms
```

## sparseml/exporters/transforms/kv_cache/__init__.py

```diff
@@ -15,8 +15,11 @@
 Transforms for adding KV caching mechanism into language models
 """
 
 # flake8: noqa
 # isort:skip_file
 
 from .cache_keys_and_values import *
-from .position_embeddings_adjustment import *
+from .positions_adjustment_base import *
+from .positions_adjustment_opt import *
+from .positions_adjustment_codegen import *
+from .configs import *
```

## sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py

```diff
@@ -25,14 +25,15 @@
 
 
 __all__ = ["CacheKeysAndValues"]
 
 
 _LOGGER = logging.getLogger(__name__)
 
+ALLOWED_NODES_BEFORE_SOFTMAX = ["Cast"]
 OUTPUT_CACHE_NAME = """present.{attention_layer_idx}.{cache_type}"""
 INPUT_CACHE_NAME = """past_key_values.{attention_layer_idx}.{cache_type}"""
 
 
 class CacheKeysAndValues(OnnxTransform):
     """
     Inject the key and value caches into the graph for the attention layers.
@@ -41,34 +42,45 @@
     1.  Find all the MatMuls that are preceded by a Softmax operation.
         Those are the MatMuls that perform V x Softmax(Q x K^T) operation
         (the "value" MatMuls).
     2.  Given the "value" MatMuls found in step 1, perform a Breadth First Search
         to find the "key" MatMuls that perform Q x K^T operation.
     3.  Before each pair of "key" and "value" MatMuls, inject a cache node that
         concatenates the current keys/values with the cached keys/values.
-    4.  For the key cache, the concatenation happens before the Transpose node, that
-        precedes the "key" MatMul.
-    5.  For the value cache, the concatenation happens directly before the "value"
-        MatMul.
+    4.  For the key or value cache, if there is a Transpose node present before
+        the MatMul, the concatenation will be performed before the Transpose node
+    6. (Optional) To account for the variance in the operations in the vicinity
+        of the "key" and "value" MatMuls, the user can specify whether to additionally
+        inject a Reshape or Transpose node, so that the dimensions of the cache
+        inputs/outputs are compatible with the values they are concatenated with.
 
     This transform also sets the subset of kv cache inputs/outputs dimensions (
-    num_attention_heads and hidden_size_kv_cache ) to the appropriate static values.
+    num_attention_heads and hidden_size_kv_cache) to the appropriate static values.
 
     :param num_attention_heads: number of attention heads of the model
     :param hidden_size_kv_cache: hidden size of the key and value cache
-    :param internally_multiply_batch_by_num_attention_heads: every model created by
+    :param multiply_batch_by_num_att_heads: every model created by
         this transformation, will have kv_cache inputs/outputs that have dimensions:
-
         [`batch_size`,`num_attention_heads`,`past_sequence_len`,`hidden_size_kv_cache`]
 
         However, internally, there may be a need of reshaping the kv_cache
         inputs/outputs ("merging" the `batch_size` and `num_attention_heads`
-        dimensions) so that it is compatible with the attention layer.
-        If True, the batch size will be multiplied
-        by the number of attention heads just before the appropriate concatenation node.
+        dimensions) so that it is compatible with the values it is concatenated with.
+        If True, the batch size will be multiplied by the number of attention
+        heads just before the appropriate concatenation node (as reflected by
+        the "Reshape" nodes in the diagram below).
+    :param transpose_value_input: if not None, transpose the kv cache value
+        input before the "value" MatMul. The argument needs to be a tuple of
+        4 integers that represent the permutation of the input dimensions.
+        This will insert a Transpose node before the "value" MatMul. If
+        multiply_batch_by_num_att_heads is True, the Transpose node will be
+        inserted before the Reshape node.
+    :param transpose_key_input: works analogously to transpose_value_input,
+        but for the key input.
+
 
     Transforms
     ```
     |
     |     Key
     |      |    Query
     |  Transpose |
@@ -77,67 +89,83 @@
     |        |
     |   "key" MatMul
     |        |
     |       ...    Value
     |        |      |
     |     Softmax  |
     |        |    |
-    |       ...  |
+    |       ...  ...
     |        |  |
     |         |
     |   "value" MatMul
     |        |
     |       ...
     ```
     to
 
     ```
     |
-    | KeyCache  Key
-    |    |      |
-    | Reshape   |
-    |(optional)|
+    | KeyCache
+    |    |
+    | Transpose
+    |(optional)
+    |    |
+    |    |         Key
+    | Reshape      |
+    |(optional)   |
+    |    |       |
+    |     |    |
     |      | |
-    |       |
+    |      |
     |   Concat ------------> OutputKeyCache
     |      |
-    |      |    Query
-    |  Transpose |      ValueCache
-    |      |    | Value     |
-    |       | |     |    Reshape
-    |        |      |  (optional)
-    |        |       |  |
-    |   "key" MatMul  |
-    |        |       |
+    |      |     Query
+    |     ...      |
+    |      |      |
+    |      |      |
+    |      |      |       ValueCache
+    |      |      |          |
+    |      |      |      Transpose
+    |      |      |      (optional)
+    |      |     |          |
+    |      |    |        Reshape
+    |      |   |         (optional)
+    |       |  |    Value  |
+    |       | |       |   |
+    |        |        |  |
+    |   "key" MatMul  | |
+    |        |        |
     |       ...   Concat --> OutputValueCache
     |        |      |
     |     Softmax  |
-    |        |    |
+    |        |   ...
     |       ...  |
     |        |  |
     |         |
     |   "value" MatMul
     |        |
     |       ...
     ```
 
     """
 
     def __init__(
         self,
         num_attention_heads: int,
         hidden_size_kv_cache: int,
-        internally_multiply_batch_by_num_attention_heads: bool = True,
+        multiply_batch_by_num_att_heads: bool,
+        transpose_value_input: Optional[Tuple[int, int, int, int]] = None,
+        transpose_key_input: Optional[Tuple[int, int, int, int]] = None,
     ):
         super().__init__()
         self.num_attention_heads = num_attention_heads
         self.hidden_size_kv_cache = hidden_size_kv_cache
-        self.internally_multiply_batch_by_num_attention_heads = (
-            internally_multiply_batch_by_num_attention_heads
-        )
+        self.multiply_batch_by_num_att_heads = multiply_batch_by_num_att_heads
+        self.transpose_value_input = transpose_value_input
+        self.transpose_key_input = transpose_key_input
 
     def transform(self, model: ModelProto) -> ModelProto:
         graph = ONNXGraph(model)
 
         key_value_matmul_pairs = _find_key_value_matmul_pairs(graph)
 
         # Inject kv cache to the graph as the model input,
@@ -161,30 +189,32 @@
                 ),
                 cache_output_name=OUTPUT_CACHE_NAME.format(
                     attention_layer_idx=idx, cache_type="key"
                 ),
                 use_uint8_if_quantized=use_uint8_if_quantized,
                 num_attention_heads=self.num_attention_heads,
                 hidden_size_kv_cache=self.hidden_size_kv_cache,
-                multiply_batch_by_num_attention_heads=self.internally_multiply_batch_by_num_attention_heads,  # noqa E501
+                transpose_input=self.transpose_key_input,
+                multiply_batch_by_num_att_heads=self.multiply_batch_by_num_att_heads,  # noqa E501
             )
             value_concat_node, value_input_tensor, value_output_tensor = create_cache(
                 model=model,
                 node=value_matmul,
                 cache_input_idx=value_input_idx,
                 cache_input_name=INPUT_CACHE_NAME.format(
                     attention_layer_idx=idx, cache_type="value"
                 ),
                 cache_output_name=OUTPUT_CACHE_NAME.format(
                     attention_layer_idx=idx, cache_type="value"
                 ),
                 use_uint8_if_quantized=use_uint8_if_quantized,
                 num_attention_heads=self.num_attention_heads,
                 hidden_size_kv_cache=self.hidden_size_kv_cache,
-                multiply_batch_by_num_attention_heads=self.internally_multiply_batch_by_num_attention_heads,  # noqa E501
+                transpose_input=self.transpose_value_input,
+                multiply_batch_by_num_att_heads=self.multiply_batch_by_num_att_heads,  # noqa E501
             )
 
             inputs_to_add.extend([key_input_tensor, value_input_tensor])
             outputs_to_add.extend([key_output_tensor, value_output_tensor])
 
             self.log_match(key_matmul)
             self.log_match(value_matmul)
@@ -204,15 +234,16 @@
     cache_input_idx: int,
     cache_input_name: str,
     cache_output_name: str,
     num_attention_heads: int,
     hidden_size_kv_cache: int,
     use_uint8_if_quantized: bool = True,
     batch_size: int = 1,
-    multiply_batch_by_num_attention_heads: bool = True,
+    multiply_batch_by_num_att_heads: bool = True,
+    transpose_input: Optional[Tuple[int, int, int, int]] = None,
 ) -> Tuple[NodeProto, ValueInfoProto, ValueInfoProto]:
     """
     Injects a cache (value or key) into the graph for a given Matmul node.
 
     :param model: Model to update
     :param node: MatMul node that follows the cache injection point
     :param cache_input_idx: Index of the input
@@ -220,17 +251,21 @@
     :param cache_input_name: Name of cache input
     :param cache_output_name: Name of cache output
     :param num_attention_heads: number of attention heads of the model
     :param hidden_size_kv_cache: hidden size of the key/value cache
     :param use_uint8_if_quantized: True if quantized MatMuls should have uint8
         inputs, if False, uses int8
     :param batch_size: batch size of the kv cache. By default, this is 1.
-    :param multiply_batch_by_num_attention_heads: If True, the batch size of the
+    :param multiply_batch_by_num_att_heads: If True, the batch size of the
         kv cache is multiplied by the number of attention heads before the
         concat node.
+    :param transpose_input: If not None, transpose the input to the cache
+        before the concat node. If `multiply_batch_by_num_att_heads` is True,
+        the transpose is applied after the batch size is multiplied by the
+        number of attention heads.
     :return: tuple of concat node to add, cache input to add, and cache output to add,
         updates existing nodes in-place
     """
     CACHE_INPUT_DIMS = [
         batch_size,
         num_attention_heads,
         "past_sequence_len",
@@ -280,15 +315,29 @@
     else:
         pre_cache_input_id = node.input[cache_input_idx]
 
     cache_input_name_concat = cache_input_name
     cache_output_name_concat = cache_output_name
     cache_input_dims_concat = CACHE_INPUT_DIMS
 
-    if multiply_batch_by_num_attention_heads:
+    if transpose_input:
+        (
+            graph,
+            cache_input_dims_concat,
+            cache_input_name_concat,
+            cache_output_name_concat,
+        ) = transpose_kv_cache_inputs_outputs(
+            graph=graph,
+            cache_input_name=cache_input_name_concat,
+            cache_output_name=cache_output_name_concat,
+            cache_input_dims=cache_input_dims_concat,
+            transpose_input=transpose_input,
+        )
+
+    if multiply_batch_by_num_att_heads:
         (
             model,
             cache_input_dims_concat,
             cache_input_name_concat,
             cache_output_name_concat,
         ) = reshape_kv_cache_inputs_outputs(
             model=model,
@@ -428,26 +477,96 @@
         model,
         reshape_input_dims_in,
         cache_input_name_reshaped,
         cache_output_name_reshaped,
     )
 
 
+def transpose_kv_cache_inputs_outputs(
+    graph: ONNXGraph,
+    cache_input_name: str,
+    cache_output_name: str,
+    cache_input_dims: List[Union[int, str]],
+    transpose_input: Tuple[int, int, int, int],
+) -> Tuple[ModelProto, List[Union[int, str]], str, str]:
+    """
+    Transposes the input and output of a kv cache in the model
+    according to the transpose_input sequence
+
+    Transform:
+    ```
+    |      cache_input_name
+    |            |
+    |           ...
+    |            |
+    |      cache_output_name
+    ```
+    to:
+    ```
+    |      cache_input_name
+    |            |
+    |      cache_input_name_transposed
+    |            |
+    |           ...
+    |            |
+    |      cache_output_name_transposed
+    |            |
+    |      cache_output_name
+
+    :param graph: The graph to update
+    :param cache_input_name: The name of the input to the submodel
+    :param cache_output_name: The name of the output from the submodel
+    :param transpose_input: The permutation of the input dimensions
+    :param cache_input_dims: The dimensions of the input to the submodel
+    :return: The updated model, the updated input dimensions,
+        the updated input name, and the updated output name
+    """
+
+    cache_input_name_transposed = f"{cache_input_name}_transposed"
+    cache_output_name_transposed = f"{cache_output_name}_transposed"
+
+    transpose_node_in = onnx.helper.make_node(
+        op_type="Transpose",
+        inputs=[cache_input_name],
+        outputs=[cache_input_name_transposed],
+        name=f"transpose.{cache_input_name}",
+        perm=transpose_input,
+    )
+    transpose_node_out = onnx.helper.make_node(
+        op_type="Transpose",
+        inputs=[cache_output_name_transposed],
+        outputs=[cache_output_name],
+        name=f"transpose.{cache_output_name}",
+        perm=transpose_input,
+    )
+    transposed_input_dims = [cache_input_dims[i] for i in transpose_input]
+
+    graph.add_node(transpose_node_in)
+    graph.add_node(transpose_node_out)
+
+    return (
+        graph,
+        transposed_input_dims,
+        cache_input_name_transposed,
+        cache_output_name_transposed,
+    )
+
+
 def _find_key_value_matmul_pairs(
     graph: ONNXGraph,
 ) -> List[Tuple[NodeProto, NodeProto]]:
     # Find pairs of "key" and "value" MatMuls.
     # Each attention block contains a pair of MatMuls:
     #    - key MatMul that computes Q x K^T
     #    - value MatMul that computes Softmax(Q x K^T) x V
     # The function returns:
     #   [(key_matmul_0, value_matmul_0), (key_matmul_1, value_matmul_1), ...]
 
     key_value_matmul_pairs = []
-    value_matmuls = [node for node in graph.nodes if _is_value_matmul(node, graph)]
+    value_matmuls = [node for node in graph.nodes if is_value_matmul(node, graph)]
     value_matmul_names = {node.name for node in value_matmuls}
 
     # for every value matmul, find the corresponding key matmul
     for value_matmul in value_matmuls:
         key_matmul = _find_key_matmul_from_value_matmul(
             value_matmul, graph, value_matmul_names
         )
@@ -457,30 +576,60 @@
             raise RuntimeError(
                 f"Could not find key matmul for value matmul {value_matmul.name}"
             )
 
     return key_value_matmul_pairs
 
 
-def _is_value_matmul(node: NodeProto, graph: ONNXGraph) -> bool:
-    # A valid value MatMul needs to meet the following criteria:
-    #   - is_matmul(node) is True
-    #   - have no parameters
-    #   - have a single parent node: a Softmax
+def is_value_matmul(
+    node: NodeProto,
+    graph: ONNXGraph,
+    allowed_nodes_before_softmax: Set[str] = ALLOWED_NODES_BEFORE_SOFTMAX,
+) -> bool:
+    """
+    Returns True if the node is a "value" MatMul, i.e. a MatMul that meets
+    the following criteria:
+        -   is_matmul(node) is True
+        -   node has no parameters
+        -   node has a single `Softmax` parent node
+                or
+            the parent node `Softmax` is preceded by
+            a set of nodes that are specified in the
+            `allowed_nodes_before_softmax` set
+
+    :param node: node to check
+    :param graph: graph containing the node
+    :param allowed_nodes_before_softmax: set of node types that are allowed
+        to be located between the node in question a Softmax node, so that
+        the node can still be considered a "value" MatMul
+    """
 
     if not is_matmul(node) or _is_parameterized_matmul(node, graph):
         # not a matmul or MatMul op has a parameter
         return False
 
-    for parent in graph.get_node_parents(node):
+    parent = graph.get_node_single_parent(node, index=0)
+    while parent.op_type in allowed_nodes_before_softmax:
         if not isinstance(parent, NodeProto):
-            continue
-        if parent.op_type == "Softmax":
-            # a parent is a Softmax node, assume this is a "value" MatMul
-            return True
+            break
+        parent = graph.get_node_single_parent(parent, index=0)
+        if parent is None:
+            raise ValueError(
+                "While traversing the graph to find a Softmax that precedes "
+                f"the candidate for a `value` MatMul: {node.name}, found a node "
+                f"with multiple parents {parent.name}. "
+                "It is assumed that the graph that connects the Softmax "
+                "node and the `value` MatMul node is a linear chain of nodes "
+                "and thus none of the encountered nodes should have multiple "
+                "parents"
+            )
+
+    if parent.op_type == "Softmax":
+        # a parent is a Softmax node, assume this is a "value" MatMul
+        return True
 
     # no parents are a softmax node
     return False
 
 
 def _find_key_matmul_from_value_matmul(
     value_matmul: NodeProto,
```

## sparseml/onnx/utils/graph_editor.py

```diff
@@ -191,18 +191,18 @@
         self._delete_node_edges(node)
 
     def delete_nodes(self, nodes: List[NodeProto]):
         """
         deletes the given nodes from the graph
         :param nodes: list of nodes to delete
         """
-        node_ouptut_ids_to_delete = {node.output[0] for node in nodes}
+        node_output_ids_to_delete = {node.output[0] for node in nodes}
         nodes_to_keep = []
         for node in self._model.graph.node:
-            if node.output[0] in node_ouptut_ids_to_delete:
+            if node.output[0] in node_output_ids_to_delete:
                 self._delete_node_edges(node)
             else:
                 nodes_to_keep.append(node)
         self._model.graph.ClearField("node")
         self._model.graph.node.extend(nodes_to_keep)
 
     def delete_initializers(self, initializers: List[Union[str, TensorProto]]):
@@ -238,14 +238,66 @@
                 init
                 for init in self._model.graph.initializer
                 if not self._input_id_to_nodes[init.name]
                 and (init.name not in output_names)
             ]
         )  # delete inits that have no edge
 
+    def find_orphaned_nodes(self, node: NodeProto) -> List[NodeProto]:
+        """
+        Given a node, that is to be removed from the graph, find all nodes that
+        will be orphaned as a result of the removal. Orphaned nodes are nodes
+        that will have no inputs after the removal of the given node.
+        The method traverses the graph upwards from the given node until
+        a node with multiple outputs is found. All nodes that are traversed
+        are considered orphaned and will be removed.
+
+        :param node: The node to remove
+        :return: A tuple of the model and a list of orphaned nodes
+        """
+        nodes_to_delete = [node]
+        # start queue with previous positions input node
+        queue = [node]
+        while queue:
+            current_node = queue.pop(0)
+            if not isinstance(current_node, NodeProto):
+                continue
+            node_parents = self.get_node_parents(current_node)
+            # if node parent has only one output (current child)
+            # than it is orphaned and will be removed.
+            # continue traversing the graph upwards until
+            # a node with output that is not current child is found
+            for parent in node_parents:
+
+                if not isinstance(parent, NodeProto):
+                    # if parent is not a node, it is a graph input
+                    # and should not be removed
+                    continue
+                elif parent.op_type == "Constant":
+                    # if constant node is found,
+                    # automatically remove it and continue traversing
+                    nodes_to_delete.append(parent)
+
+                parent_output_node_names = set(
+                    n.name for n in self.get_node_parents(node=parent)
+                )
+                if len(parent_output_node_names) == 1:
+                    # if parent has only one output, it is orphaned
+                    queue.append(parent)
+                    nodes_to_delete.append(parent)
+                elif not parent_output_node_names.difference(
+                    set(n.name for n in nodes_to_delete)
+                ):
+                    # if parent has multiple outputs, but they are all already in the
+                    # nodes_to_delete list, it is orphaned
+                    queue.append(parent)
+                    nodes_to_delete.append(parent)
+
+        return nodes_to_delete
+
     def sort_nodes_topologically(self):
         """
         Sorts the order of the graph Node repeated field in place in topological
         order as per the ONNX Model proto specifications
         """
         if len(self._model.graph.node) == 1:
             return
```

## sparseml/pytorch/base.py

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 import functools
+import os
 from typing import Optional
 
 from sparseml.base import check_version
 
 
 try:
     import torch
@@ -45,15 +45,15 @@
     "check_torchvision_install",
     "require_torch",
     "require_torchvision",
 ]
 
 
 _TORCH_MIN_VERSION = "1.0.0"
-_TORCH_MAX_VERSION = "2.0.100"
+_TORCH_MAX_VERSION = os.environ.get("MAX_TORCH", "2.0.100")
 
 
 def check_torch_install(
     min_version: Optional[str] = _TORCH_MIN_VERSION,
     max_version: Optional[str] = _TORCH_MAX_VERSION,
     raise_on_error: bool = True,
 ) -> bool:
```

## sparseml/yolov8/trainers.py

```diff
@@ -551,15 +551,15 @@
                 Model(model_str), model_suffix="pt"
             )
             model_str = str(model)
             self.is_sparseml_checkpoint = True
 
         if model_str.endswith(".pt"):
             if os.path.exists(model_str):
-                ckpt = torch.load(model_str)
+                ckpt = torch.load(model_str, map_location="cpu")
                 self.is_sparseml_checkpoint = (
                     "source" in ckpt and ckpt["source"] == "sparseml"
                 )
             else:
                 self.is_sparseml_checkpoint = False
         else:
             self.is_sparseml_checkpoint = False
```

## Comparing `sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py` & `sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from copy import deepcopy
-
 from onnx import ModelProto, NodeProto
 
-from sparseml.exporters.transforms.onnx_transform import OnnxTransform
+from sparseml.exporters.transforms.kv_cache.positions_adjustment_base import (
+    PositionsAdjustmentBase,
+)
 from sparseml.onnx.utils import ONNXGraph
 
 
-__all__ = ["PositionEmbeddingsAdjustment"]
+__all__ = ["PositionsAdjustmentOPT"]
 
 
 # name position embeddings weights
 _EMBED_POSITIONS_ID = "model.decoder.embed_positions.weight"
 
 
-class PositionEmbeddingsAdjustment(OnnxTransform):
+class PositionsAdjustmentOPT(PositionsAdjustmentBase):
     """
     Base class for model architecture specific transforms to adjust graph
     to take input_id positions as an argument rather than computing them
     based on input. This provides a better source of truth rather than
     computing in a static graph where factors such as number of tokens,
     cache size, and padding may affect accurate, efficient static
     computation of the position indices.
@@ -65,49 +65,23 @@
     |   Add (Optional)
     |     |
     |  Gather(model.decoder.embed_positions.weight)
     ```
 
     """
 
-    POSITIONS_NAME = "positions"  # matches intermediate var name in torch
-
     def transform(self, model: ModelProto) -> ModelProto:
         model = self.add_positions_input(model)
         position_embeddings_node = self.find_embed_positions_gather_node(model)
         model = self._update_position_embeddings_for_graph_input(
             model, position_embeddings_node
         )
         return model
 
     @classmethod
-    def add_positions_input(cls, model: ModelProto) -> ModelProto:
-        """
-        Adds positions as an input to the model
-
-        :param model: model to update
-        :return: updated model
-        """
-        # positions tensor should have shape equal to input_ids
-        input_ids_info = [
-            input_info
-            for input_info in model.graph.input
-            if input_info.name == "input_ids"
-        ][0]
-        if not input_ids_info:
-            raise RuntimeError(
-                f"{cls.__name__} - unable to find 'input_ids' in model input"
-            )
-
-        positions_input_info = deepcopy(input_ids_info)
-        positions_input_info.name = cls.POSITIONS_NAME
-        model.graph.input.append(positions_input_info)
-        return model
-
-    @classmethod
     def find_embed_positions_gather_node(cls, model: ModelProto) -> NodeProto:
         for node in model.graph.node:
             if node.op_type != "Gather":
                 continue
             if node.input[0] == _EMBED_POSITIONS_ID:
                 # found the embed_positions_gather_node
                 return node
@@ -143,37 +117,17 @@
 
         # reroute target node input to the positions graph input
         old_positions_input = target_update_node.input[target_input_idx]
         target_update_node.input[target_input_idx] = self.POSITIONS_NAME
         graph.update()
         self.log_match(target_update_node)
 
-        # traverse graph upwards to delete any nodes that are now orphaned
-        nodes_to_delete = []
-        # start queue with previous positions input node
-        queue = [graph.get_node_by_output_id(old_positions_input)]
-        seen_node_names = {queue[0].name}
-        while queue:
-            current_node = queue.pop(0)
-            if not isinstance(current_node, NodeProto):
-                continue
-
-            node_children = graph.get_node_children(current_node)
-            if any(child not in nodes_to_delete for child in node_children):
-                # node has a child that is not on the orphaned branch
-                # do not remove and do not traverse further
-                continue
-            else:
-                nodes_to_delete.append(current_node)
-                self.log_match(current_node)
-                for parent in graph.get_node_parents(current_node):
-                    if isinstance(parent, NodeProto) and (
-                        parent.name not in seen_node_names
-                    ):
-                        seen_node_names.add(parent.name)
-                        queue.append(parent)
+        nodes_to_delete = graph.find_orphaned_nodes(
+            graph.get_node_by_output_id(old_positions_input)
+        )
+        [self.log_match(node) for node in nodes_to_delete]
 
         graph.delete_nodes(nodes_to_delete)
         graph.update()
         graph.delete_unused_initializers()
 
         return model
```

## Comparing `sparseml_nightly-1.6.0.20230623.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230629.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230623.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230629.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.6.0.20230623
+Version: 1.6.0.20230629
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -26,32 +26,34 @@
 Description-Content-Type: text/markdown
 Requires-Dist: sparsezoo-nightly (~=1.6.0)
 Requires-Dist: setuptools (<=59.5.0)
 Requires-Dist: jupyter (>=1.0.0)
 Requires-Dist: ipywidgets (>=7.0.0)
 Requires-Dist: pyyaml (>=5.0.0)
 Requires-Dist: progressbar2 (>=3.0.0)
-Requires-Dist: numpy (<=1.21.6,>=1.0.0)
+Requires-Dist: numpy (>=1.0.0)
 Requires-Dist: matplotlib (>=3.0.0)
 Requires-Dist: merge-args (>=0.1.0)
 Requires-Dist: onnx (<1.15.0,>=1.5.0)
 Requires-Dist: pandas (>=0.25.0)
 Requires-Dist: packaging (>=20.0)
 Requires-Dist: psutil (>=5.0.0)
 Requires-Dist: pydantic (>=1.5.0)
 Requires-Dist: requests (>=2.0.0)
 Requires-Dist: scikit-image (>=0.15.0)
 Requires-Dist: scikit-learn (>=0.24.2)
 Requires-Dist: tqdm (>=4.0.0)
 Requires-Dist: toposort (>=1.0)
 Requires-Dist: GPUtil (>=1.4.0)
-Requires-Dist: protobuf (<=3.20.1,>=3.12.2)
+Requires-Dist: protobuf (>=3.12.2)
 Requires-Dist: click (!=8.0.0,>=7.1.2)
 Requires-Dist: scipy (<1.9.2,>=1.8) ; python_version <= "3.9"
 Requires-Dist: scipy (>=1.0.0) ; python_version > "3.9"
+Provides-Extra: clip
+Requires-Dist: open-clip-torch (==2.20.0) ; extra == 'clip'
 Provides-Extra: deepsparse
 Requires-Dist: deepsparse-nightly (~=1.6.0) ; extra == 'deepsparse'
 Provides-Extra: deepsparse-ent
 Requires-Dist: deepsparse-ent (~=1.6.0) ; extra == 'deepsparse-ent'
 Provides-Extra: dev
 Requires-Dist: beautifulsoup4 (==4.9.3) ; extra == 'dev'
 Requires-Dist: black (==22.12.0) ; extra == 'dev'
@@ -226,15 +228,15 @@
 - [Ultralytics YOLOv5](integrations/ultralytics-yolov5#tutorials)
 
 ## Installation
 
 This repository is tested on Python 3.8-3.10, and Linux/Debian systems.
 
 It is recommended to install in a [virtual environment](https://docs.python.org/3/library/venv.html) to keep your system in order.
-Currently supported ML Frameworks are the following: `torch>=1.1.0,<1.14`, `tensorflow>=1.8.0,<2.0.0`, `tensorflow.keras >= 2.2.0`.
+Currently supported ML Frameworks are the following: `torch>=1.1.0,<=2.0`, `tensorflow>=1.8.0,<2.0.0`, `tensorflow.keras >= 2.2.0`.
 
 Install with pip using:
 
 ```bash
 pip install sparseml
 ```
```

## Comparing `sparseml_nightly-1.6.0.20230623.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230629.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230623.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230629.dist-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [console_scripts]
-sparseml.benchmark = sparseml.benchmark.info:_main
 sparseml.framework = sparseml.framework.info:_main
 sparseml.image_classification.export_onnx = sparseml.pytorch.torchvision.export_onnx:main
 sparseml.image_classification.train = sparseml.pytorch.torchvision.train:cli
 sparseml.openpifpaf.export_onnx = sparseml.openpifpaf.export:main
 sparseml.openpifpaf.train = sparseml.openpifpaf.train:main
 sparseml.pytorch.image_classification.export_onnx = sparseml.pytorch.image_classification.export:main
 sparseml.pytorch.image_classification.lr_analysis = sparseml.pytorch.image_classification.lr_analysis:main
```

## Comparing `sparseml_nightly-1.6.0.20230623.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230629.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 sparseml/__init__.py,sha256=nxuiUykjTFTYiw28TB9H75wWbdzr6Y0j-2h4dabdp54,1413
 sparseml/analytics.py,sha256=WhXdKgK1-ll9sRzn2n8z-FAikQ02J8rUeWmceiX5S7E,898
 sparseml/base.py,sha256=oOPiaU2JhI0beFwp8Obe7hbt3kUuNvI5XD1wTBCtLnc,10284
 sparseml/log.py,sha256=K5E3goPRIPY7Uc14JcX-4oLXVWu7ecOPf1NYBGHc1r0,2483
 sparseml/version.py,sha256=IANtJ2lwLlKC1tGVdfq0LveVx77c3yZrd5RIhvbn8MM,1511
 sparseml/benchmark/__init__.py,sha256=WynUhMzXq3-iQAhPwcmcMOj2_xCa9brLubs7gxq9T3U,758
-sparseml/benchmark/info.py,sha256=yRA5QgKQNKjOZhQH9uNvVuWlqL4eXDVikA8pL5Mzha4,17631
+sparseml/benchmark/info.py,sha256=VjZ7cUD66h1u7IJeRXKjiSfvS8aSr-cbAJdnsTmLmoI,17763
 sparseml/benchmark/serialization.py,sha256=FPpcC93x5H86Fqil9YbERUpltu7qhhIQjsyYaSlW_20,10778
 sparseml/deepsparse/__init__.py,sha256=o5ITzTEOlH--61_SXMISrmPcRk4ci91FGlR-aQxwOn4,863
 sparseml/deepsparse/base.py,sha256=nRjU6TSao0J2iWXcdHwj62X6dVT9vl6TQ2y4Bdn3KN0,3516
 sparseml/deepsparse/framework/__init__.py,sha256=ZHrXXM3AMH78zKcF8Y40IBuy38UFy4fLrvytozw_bNY,801
 sparseml/deepsparse/framework/info.py,sha256=HVDPHFXggFeDqbpM20PkByf1nBccwKnjpTWh0EfrVas,6032
 sparseml/deepsparse/sparsification/__init__.py,sha256=re_2FtHWvO-iQQwRRJZDKz3l_pFZuwe266-4ZFxQqbY,813
 sparseml/deepsparse/sparsification/info.py,sha256=O5FJg5KMJvj-HcJn9W9iiKGZ6Z7_1SavOX-TstXRr6Q,1348
 sparseml/exporters/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/exporters/base_exporter.py,sha256=M1HEe9GNf51uYx1z-qxWjIYo5iGZ_Ish8uZ3mj6OZR8,1477
-sparseml/exporters/kv_cache_injector.py,sha256=0SeVr1l_o3LZm_yFBv1s34Uz41sRXIezrN0uSUp-ZCw,6058
+sparseml/exporters/kv_cache_injector.py,sha256=P14Ma0IRvLUJ7bdKmxWTHwHmTIxJaPYn2z0E8P2aa4U,6325
 sparseml/exporters/onnx_to_deepsparse.py,sha256=OO7WosKj8jtd-pSoh7RzaJh-ScWPHV7d-F75gOvJu08,4783
 sparseml/exporters/transforms/__init__.py,sha256=x0mpqLIbsRXjVVot0MH7ebFBmJwV_oZdOp7LhUEydI4,2276
 sparseml/exporters/transforms/base_transform.py,sha256=IpvdUdEADl2SfqHawcp6-lcNgz-R3L0zpS05WaWF5h8,2333
 sparseml/exporters/transforms/constants_to_initializers.py,sha256=_PX3y16OC-q85d-6DeOOVpKAAMNIU1m5BdYTZlFV_tk,1388
 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py,sha256=9z2HRqJAM68HPiSfu2RMyrn93dr8HCTpMcMrh_1-x2w,3866
 sparseml/exporters/transforms/conv_to_qlinearconv.py,sha256=CwCXtIBCOQ1qX5Z2JZhsdXSDk683wRCIBILF_1vd0GI,5838
 sparseml/exporters/transforms/delete_repeated_qdq.py,sha256=YiIOrvKqrxYboOA4A8YTbQIQ4s4MDdmqeLNYHPP4kjs,2440
@@ -37,17 +37,20 @@
 sparseml/exporters/transforms/propagate_embedding_quantization.py,sha256=XTEiUTX5nzLUtndGs_0t7nTgjIad-FyjuNc0O4f6Xro,3398
 sparseml/exporters/transforms/quantize_qat_embedding.py,sha256=_v1dEEt5vCSaMF6dJkg9fVGof145-_Lmo0DMjpXsnUE,4464
 sparseml/exporters/transforms/quantize_residuals.py,sha256=f3kNF930ymHI5CmCA0OmYW7vDKvEm9sYhN0UX0UC1EQ,3869
 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py,sha256=mod-7bnlkg20LjerZ7tKKmp_7XyO3FKo13BtIZkDsmM,3331
 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py,sha256=2FSXzaY3jdxOgj3xBaUOUqtk-hzg4kwhheELhoOKpS8,2545
 sparseml/exporters/transforms/skip_input_quantize.py,sha256=ANiYDwSos9gPW4960fMwmGubTDgpAcqFVSIHKf_ffYw,3210
 sparseml/exporters/transforms/unwrap_batchnorms.py,sha256=ly7GHCXN_2r8Gnk8PABWCqcoS-NL3GMfquEK0hRlFCs,1373
-sparseml/exporters/transforms/kv_cache/__init__.py,sha256=ykMEDNKJuV2jGlG1oydxopFrVD8U1h0AmSo22Um6vyk,807
-sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py,sha256=YYloawGYmaWfHe2Km5r86HahwTSksKlivt2R2qWvtlc,20939
-sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py,sha256=pGThjU3jLGtgxXPAOxTC91oKerGhE6d1e0cSh--SSHw,6763
+sparseml/exporters/transforms/kv_cache/__init__.py,sha256=6wiIglqacQ56SO_4i5zemLL3VcUfTfJA-AMc5gOHmOE,909
+sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py,sha256=PEN6NU9huZEgPkWpN-hpmYq-mfRDkbRWyoN8ozklsaY,26599
+sparseml/exporters/transforms/kv_cache/configs.py,sha256=yLIZpF2d90hoeXo-lqPlmSe7wuxXeq1DhroQ_BGOxZQ,6192
+sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py,sha256=bSiZF-U4LRoBxJfnSGXLlaG1pL5MzNPXlzmbDvAXtFw,1660
+sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py,sha256=1FSG9npk_R0UK56fap-yRvSjNs5RWRejXJI4fYFD3lk,3377
+sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py,sha256=d3xqHqbxdRbLIEi5ebXaRwPauvsMjdLPLuRpYyx_DsM,4951
 sparseml/exporters/transforms/utils/__init__.py,sha256=tXSSUnzdyIc_H73xQ5dYhHb1Gj4Nb7GLLDVwJds8c_s,730
 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=I6kugQ0J9yHxCz7Yx3TlxQTUxcaAko4XkBDsQD7v5eo,10570
 sparseml/exporters/transforms/utils/helpers.py,sha256=vkEYL2Bdp_YNXlPg_TGd82Q2ef1EYEr11LVgmORQDiY,6457
 sparseml/exporters/transforms/utils/matching.py,sha256=CnVJLbJARBJwvFjoKh9vwYt6dLP4WXG3p7nCY5VUFaE,14429
 sparseml/framework/__init__.py,sha256=EcIX435yx552d7BkbxmAbQ_X3KAISInHVbD9X-AT1Uk,790
 sparseml/framework/info.py,sha256=TaZAMYdhBHcjl9Xyk3PWjJkDB6g3_f4vD3B6KmhgOl8,9479
 sparseml/keras/__init__.py,sha256=9D-eU-wi0UGuq55i2BTYDgS0mD6UJB10Gi8LQwh9KSk,1144
@@ -102,15 +105,15 @@
 sparseml/onnx/optim/quantization/quantize_model_post_training.py,sha256=aoz5ixUpQB_6XkowhozqRp8_njthBeqVuwvV2ctM1q0,4552
 sparseml/onnx/sparsification/__init__.py,sha256=hFZDQQXFcXqSqiXlRBRUX7e7GavLphgRd8c21peq8fg,869
 sparseml/onnx/sparsification/analyzer.py,sha256=DCKc8nYo0i3NDu73GVjvBYjuflXUZhkhB14FoFRlTBE,10209
 sparseml/onnx/sparsification/info.py,sha256=UnrwVgOuj-HErwTMc-19h-QOrs1yG_mM45O9VL8oiXU,1363
 sparseml/onnx/sparsification/model_info.py,sha256=Y0tpY9fWN3gr4KlkAdXv2QYJrrrjMvVZOCA-ujPJFPM,8009
 sparseml/onnx/utils/__init__.py,sha256=fGZED95Xmko70ZmTWlZWX3-C4dajmbZcKgaap3HXmVw,867
 sparseml/onnx/utils/data.py,sha256=eh1URN6lmPpVUTg_iHK1R6lLKi4jJh3XGg5OPkgGD_Y,13013
-sparseml/onnx/utils/graph_editor.py,sha256=IBNbKWjOLy7oW-bjsxBkSw5HULHIoeVFQFs2ccYVTs0,16407
+sparseml/onnx/utils/graph_editor.py,sha256=WLRf0LN__Ou99BIb8Y5Y0ErovGEOuu3J_4PAdFFlxDQ,18825
 sparseml/onnx/utils/graph_optimizer.py,sha256=AfS2zdxW1tJ6xYAe-2n3KdAdDenxiqslOFUIVAzD-cY,8133
 sparseml/onnx/utils/helpers.py,sha256=I1CJ8loycHBNR35ZaBKxnoFA9TwPHwTEjKlsH1jIgQc,40230
 sparseml/onnx/utils/loss.py,sha256=2njnY0qY2n6DS9HHB0kqLz7N8wgPaDTkAi6Z2DLYPLc,1958
 sparseml/onnx/utils/model.py,sha256=jpuomHDXg4pMngluDRGvGPTO1qhTmyRLTMoHasAC8Co,31591
 sparseml/onnx/utils/sparse_tensor.py,sha256=6Bu9fVJqLCtve3qpg9ScYGqcv4X7ZcRKhVrp8pCLBRI,5437
 sparseml/openpifpaf/__init__.py,sha256=aGr1xneMg-zE7LNhYNjjmEznKB6-xHbpZCT91uv4j3c,931
 sparseml/openpifpaf/export.py,sha256=XkAKuXcCJ64RPZ1YwqzyJKfr9pnn3b0GcROKRXnAWeg,3713
@@ -119,15 +122,15 @@
 sparseml/optim/__init__.py,sha256=3oGQ4LY0MSrbTAwuyPHEOEyYiZ7JI7OX2BgWup5NPuw,882
 sparseml/optim/analyzer.py,sha256=LUYBYyvfVwaw_V1aAiOmaybUGJQk4vRK5RG3k3nD7pA,6302
 sparseml/optim/helpers.py,sha256=Zb7YPYe07vuVyYUhHJ-BlcMrZa-sxt1TUZ-Ec9Z6o_U,25563
 sparseml/optim/manager.py,sha256=KeDVHj9ea9EUaV908qfvq8ONwS8nUmAvQb1yXflOBWo,25984
 sparseml/optim/modifier.py,sha256=qYfVUL9thw94p4oEsNZgitUJ3y9izWYb8nUI3enyzOU,30708
 sparseml/optim/sensitivity.py,sha256=neMP_hTRqzDUV0MrATevC2-JQYnOIvNW_AlIf_y_ydw,26315
 sparseml/pytorch/__init__.py,sha256=n1a6y27bzfG73uLbifhIx5DY9hDg1RM1pTIN1DgBpDw,2190
-sparseml/pytorch/base.py,sha256=C5ced9i5Y_fy-cnYkEFt6GuOGDHYu7fZ3pHrCm1W6mE,6117
+sparseml/pytorch/base.py,sha256=8HUpCMuP7gg6s4nvJVHU15AksGH5yhWLfeAMW6XvW18,6155
 sparseml/pytorch/opset.py,sha256=-BsKarkkKfq09HYJLZfxt_AEHEfuENpRDZF_J2va1Ck,933
 sparseml/pytorch/torch_to_onnx_exporter.py,sha256=HHgmXDopADURZcO50F5pX2wNffQGykWkwy0aTYw2H0U,10884
 sparseml/pytorch/datasets/__init__.py,sha256=2xoH_fCMojldFY1RCWSkt9pGfa8SzHAxU5em-_ZiwV8,998
 sparseml/pytorch/datasets/generic.py,sha256=nl-fFlpd7u5sNswe1AORZvQUne3sqrrPWnNgOUp6_Fc,4193
 sparseml/pytorch/datasets/registry.py,sha256=cEA3d5ju5EMft92f2StVLWARnAxlRpidKZaozujmFdE,2814
 sparseml/pytorch/datasets/classification/__init__.py,sha256=GMKhziJkRwSC7E_1Nox8FxnxhPFozZ6MxQWUWi1BN_Y,828
 sparseml/pytorch/datasets/classification/cifar.py,sha256=k32Z552YrrJv7IlshH8AWylaRKCOUC8KSrzRLLTHTag,4017
@@ -353,20 +356,20 @@
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
 sparseml/yolov8/__init__.py,sha256=l6f1TkolWl2ejQQ63jN3VFft7mMpQDURpWDIeflVKGQ,1115
 sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
-sparseml/yolov8/trainers.py,sha256=AAMOpH47N-T4RmNENWbXMW-nkmaXKamwtVNXQtudtCM,35086
+sparseml/yolov8/trainers.py,sha256=GiYoNrWxiqZMVe3Q1ThZHiA9ZQ1wVKCDmf_j7Cb1d9Q,35106
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=gn7et_J-OfnCTEYP0iLXx2W-HARgxqUnHqJWHBG72KM,6288
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.6.0.20230623.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.6.0.20230623.dist-info/METADATA,sha256=mKbU7V6spYb5nC2DAr2dmqu54dKylG_nxSEFuH1CWkQ,21712
-sparseml_nightly-1.6.0.20230623.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.6.0.20230623.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.6.0.20230623.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
-sparseml_nightly-1.6.0.20230623.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.6.0.20230623.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230629.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230629.dist-info/METADATA,sha256=ZMd1kbvW9kEzyVqYVeqcDa-kRzTgjE9pagT-Y0cXWe4,21775
+sparseml_nightly-1.6.0.20230629.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230629.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230629.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
+sparseml_nightly-1.6.0.20230629.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230629.dist-info/RECORD,,
```

