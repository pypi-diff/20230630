# Comparing `tmp/deepdoctection-0.24.tar.gz` & `tmp/deepdoctection-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdoctection-0.24.tar", last modified: Fri Jun  9 06:39:44 2023, max compression
+gzip compressed data, was "deepdoctection-0.25.tar", last modified: Fri Jun 30 11:37:43 2023, max compression
```

## Comparing `deepdoctection-0.24.tar` & `deepdoctection-0.25.tar`

### file list

```diff
@@ -1,268 +1,270 @@
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.115722 deepdoctection-0.24/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2022-06-16 05:58:47.000000 deepdoctection-0.24/LICENSE
--rw-rw-r--   0 janis     (1000) janis     (1000)    10917 2023-06-09 06:39:44.115722 deepdoctection-0.24/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)    10193 2023-06-09 06:36:46.000000 deepdoctection-0.24/README.md
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11864 2023-06-09 06:36:56.000000 deepdoctection-0.24/deepdoctection/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11612 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/analyzer/dd.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/configs/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/configs/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1032 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/configs/conf_dd_one.yaml
--rw-rw-r--   0 janis     (1000) janis     (1000)       35 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/configs/conf_tesseract.yaml
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6806 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/dataflow/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10039 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/dataflow/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6736 2023-02-23 18:53:18.000000 deepdoctection-0.24/deepdoctection/dataflow/custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20342 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/dataflow/custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15599 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/dataflow/parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/dataflow/serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9604 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/dataflow/stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19089 2023-06-01 11:26:25.000000 deepdoctection-0.24/deepdoctection/datapoint/annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23301 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/datapoint/box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6824 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/datapoint/convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    27294 2023-05-23 14:43:35.000000 deepdoctection-0.24/deepdoctection/datapoint/image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    29405 2023-06-08 09:26:52.000000 deepdoctection-0.24/deepdoctection/datapoint/view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7421 2023-06-06 08:01:17.000000 deepdoctection-0.24/deepdoctection/datasets/adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18887 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/datasets/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4105 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/dataflow_builder.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20603 2023-05-31 17:59:53.000000 deepdoctection-0.24/deepdoctection/datasets/info.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/datasets/instances/doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/datasets/instances/fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6491 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-02-20 09:20:02.000000 deepdoctection-0.24/deepdoctection/datasets/instances/publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11948 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/datasets/instances/pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8509 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/datasets/instances/pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/instances/xfund.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/datasets/instances/xsl/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/datasets/instances/xsl/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
--rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3326 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/datasets/save.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2022-06-30 08:30:21.000000 deepdoctection-0.24/deepdoctection/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19509 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/eval/accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4804 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/eval/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/eval/cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19345 2023-06-04 08:35:17.000000 deepdoctection-0.24/deepdoctection/eval/eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/eval/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9069 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/eval/tedsmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5713 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/eval/tp_eval_callback.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1140 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11828 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11010 2023-05-07 17:37:06.000000 deepdoctection-0.24/deepdoctection/extern/d2detect.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12381 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/extern/doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9319 2023-05-07 17:37:06.000000 deepdoctection-0.24/deepdoctection/extern/hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    39423 2023-06-06 08:40:23.000000 deepdoctection-0.24/deepdoctection/extern/hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    46200 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/extern/model.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/pdftext.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/pt/
--rw-rw-r--   0 janis     (1000) janis     (1000)      699 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/pt/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2022-06-22 06:44:07.000000 deepdoctection-0.24/deepdoctection/extern/pt/ptutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12369 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5654 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/extern/texocr.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/tp/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2022-06-22 06:44:07.000000 deepdoctection-0.24/deepdoctection/extern/tp/tfutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpcompat.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3664 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/common.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/config/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/config/config.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.083722 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9362 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13545 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11006 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17743 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4597 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4215 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/predict.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/preproc.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-02-13 13:44:17.000000 deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7525 2023-05-07 17:37:06.000000 deepdoctection-0.24/deepdoctection/extern/tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1390 2023-02-13 13:44:17.000000 deepdoctection-0.24/deepdoctection/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15505 2023-06-05 15:22:36.000000 deepdoctection-0.24/deepdoctection/mapper/cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6055 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/mapper/cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8536 2023-06-06 09:46:17.000000 deepdoctection-0.24/deepdoctection/mapper/d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5593 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/mapper/hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    35638 2023-05-31 17:59:53.000000 deepdoctection-0.24/deepdoctection/mapper/laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7775 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/mapper/maputils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7912 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/mapper/match.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/mapper/misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2022-09-21 17:02:22.000000 deepdoctection-0.24/deepdoctection/mapper/pascalstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6876 2022-09-27 06:19:11.000000 deepdoctection-0.24/deepdoctection/mapper/prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23583 2023-05-30 11:17:24.000000 deepdoctection-0.24/deepdoctection/mapper/pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5090 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/mapper/tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8808 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/mapper/xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1100 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13801 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/pipe/anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13245 2023-05-31 12:44:11.000000 deepdoctection-0.24/deepdoctection/pipe/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11062 2023-05-23 14:43:35.000000 deepdoctection-0.24/deepdoctection/pipe/cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14447 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9425 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8816 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/doctectionpipe.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6075 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4589 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/pipe/layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/pipe/lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    22256 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/pipe/refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      902 2022-08-12 12:59:53.000000 deepdoctection-0.24/deepdoctection/pipe/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    47806 2023-05-07 17:37:06.000000 deepdoctection-0.24/deepdoctection/pipe/segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    29451 2023-06-04 09:02:46.000000 deepdoctection-0.24/deepdoctection/pipe/text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3138 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/pipe/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-05-07 15:01:33.000000 deepdoctection-0.24/deepdoctection/py.typed
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15612 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/train/d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10538 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/train/hf_detr_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    21125 2023-06-04 08:51:52.000000 deepdoctection-0.24/deepdoctection/train/hf_layoutlm_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12968 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/train/tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.087722 deepdoctection-0.24/deepdoctection/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)     2238 2022-09-27 06:16:10.000000 deepdoctection-0.24/deepdoctection/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4612 2023-01-05 12:44:38.000000 deepdoctection-0.24/deepdoctection/utils/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3998 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/context.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2022-09-12 13:32:10.000000 deepdoctection-0.24/deepdoctection/utils/detection_types.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3441 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/develop.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17992 2023-02-23 18:53:12.000000 deepdoctection-0.24/deepdoctection/utils/file_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7626 2022-09-27 06:19:11.000000 deepdoctection-0.24/deepdoctection/utils/fs.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2022-06-16 05:58:47.000000 deepdoctection-0.24/deepdoctection/utils/identifier.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8627 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/logger.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/metacfg.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7564 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/pdf_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11954 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/utils/settings.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1923 2023-01-27 07:53:16.000000 deepdoctection-0.24/deepdoctection/utils/systools.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1813 2022-09-12 13:32:10.000000 deepdoctection-0.24/deepdoctection/utils/tqdm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8247 2023-02-09 09:34:37.000000 deepdoctection-0.24/deepdoctection/utils/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2022-09-27 06:19:11.000000 deepdoctection-0.24/deepdoctection/utils/utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10115 2023-06-04 09:03:45.000000 deepdoctection-0.24/deepdoctection/utils/viz.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.079722 deepdoctection-0.24/deepdoctection.egg-info/
--rw-rw-r--   0 janis     (1000) janis     (1000)    10917 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     7904 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/SOURCES.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)        1 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/dependency_links.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/requires.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)       30 2023-06-09 06:39:44.000000 deepdoctection-0.24/deepdoctection.egg-info/top_level.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2368 2023-06-09 06:39:44.115722 deepdoctection-0.24/setup.cfg
--rw-rw-r--   0 janis     (1000) janis     (1000)     6406 2023-06-09 06:38:44.000000 deepdoctection-0.24/setup.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.091722 deepdoctection-0.24/tests/
--rw-rw-r--   0 janis     (1000) janis     (1000)      725 2022-09-18 14:33:32.000000 deepdoctection-0.24/tests/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.091722 deepdoctection-0.24/tests/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5142 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/analyzer/test_dd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17378 2023-05-03 16:43:31.000000 deepdoctection-0.24/tests/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    64681 2022-11-28 15:25:21.000000 deepdoctection-0.24/tests/data.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.091722 deepdoctection-0.24/tests/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/dataflow/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/dataflow/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/dataflow/test_custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/dataflow/test_custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/dataflow/test_parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/dataflow/test_stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.095722 deepdoctection-0.24/tests/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2022-09-06 06:55:23.000000 deepdoctection-0.24/tests/datapoint/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4860 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/datapoint/test_annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/datapoint/test_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/datapoint/test_convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12141 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/datapoint/test_image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3670 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/datapoint/test_view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.095722 deepdoctection-0.24/tests/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/datasets/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.099722 deepdoctection-0.24/tests/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      974 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/datasets/instances/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2022-11-03 14:05:55.000000 deepdoctection-0.24/tests/datasets/instances/test_doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/datasets/instances/test_fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2091 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/datasets/instances/test_funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1263 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/datasets/instances/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/datasets/instances/test_layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/datasets/instances/test_publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1921 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/datasets/instances/test_pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/datasets/instances/test_pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/datasets/instances/test_rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2704 2022-06-29 12:05:00.000000 deepdoctection-0.24/tests/datasets/test_adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/datasets/test_info.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/datasets/test_registry.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.103722 deepdoctection-0.24/tests/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/eval/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/eval/test_accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3803 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/eval/test_cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2952 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/eval/test_eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/eval/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1253 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/eval/test_tedsmetric.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.107722 deepdoctection-0.24/tests/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/extern/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/extern/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1652 2022-11-03 14:06:59.000000 deepdoctection-0.24/tests/extern/test_deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4973 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/extern/test_doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2142 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/extern/test_fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3781 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/extern/test_hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19460 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/extern/test_hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2066 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/extern/test_pdftext.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/extern/test_tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1734 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/extern/test_texocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4372 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/extern/test_tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.111722 deepdoctection-0.24/tests/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/mapper/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    81693 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/mapper/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10518 2023-06-05 12:09:33.000000 deepdoctection-0.24/tests/mapper/test_cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/mapper/test_cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1907 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/mapper/test_d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2050 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/mapper/test_hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2382 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/mapper/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5556 2023-05-31 18:16:38.000000 deepdoctection-0.24/tests/mapper/test_laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/mapper/test_misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2867 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/mapper/test_prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/mapper/test_pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/mapper/test_tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/mapper/test_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/mapper/test_xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.115722 deepdoctection-0.24/tests/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6290 2022-10-24 07:01:39.000000 deepdoctection-0.24/tests/pipe/test_anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4498 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/pipe/test_cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3449 2023-02-13 13:44:17.000000 deepdoctection-0.24/tests/pipe/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3049 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/pipe/test_language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2022-10-24 07:01:39.000000 deepdoctection-0.24/tests/pipe/test_layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4604 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/pipe/test_lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9676 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/pipe/test_refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-05-07 15:01:33.000000 deepdoctection-0.24/tests/pipe/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14433 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests/pipe/test_segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9811 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/pipe/test_text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2022-11-03 14:06:59.000000 deepdoctection-0.24/tests/pipe/test_transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/test_utils.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.115722 deepdoctection-0.24/tests/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-01-27 07:53:16.000000 deepdoctection-0.24/tests/train/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2022-09-29 09:12:15.000000 deepdoctection-0.24/tests/train/test_d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3540 2022-10-12 13:27:51.000000 deepdoctection-0.24/tests/train/test_tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-09 06:39:44.115722 deepdoctection-0.24/tests_d2/
--rw-rw-r--   0 janis     (1000) janis     (1000)      761 2022-06-16 05:58:47.000000 deepdoctection-0.24/tests_d2/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1580 2022-09-21 17:02:23.000000 deepdoctection-0.24/tests_d2/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3226 2023-02-09 09:34:37.000000 deepdoctection-0.24/tests_d2/test_d2detect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.855733 deepdoctection-0.25/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2022-06-16 05:58:47.000000 deepdoctection-0.25/LICENSE
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10653 2023-06-30 11:37:43.855733 deepdoctection-0.25/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9929 2023-06-22 12:40:19.000000 deepdoctection-0.25/README.md
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.783733 deepdoctection-0.25/deepdoctection/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11919 2023-06-30 11:36:14.000000 deepdoctection-0.25/deepdoctection/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.783733 deepdoctection-0.25/deepdoctection/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14920 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/analyzer/dd.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.783733 deepdoctection-0.25/deepdoctection/configs/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/configs/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1971 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/configs/conf_dd_one.yaml
+-rw-rw-r--   0 janis     (1000) janis     (1000)       35 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/configs/conf_tesseract.yaml
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.787733 deepdoctection-0.25/deepdoctection/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6806 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/dataflow/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10039 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/dataflow/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6736 2023-02-23 18:53:18.000000 deepdoctection-0.25/deepdoctection/dataflow/custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20342 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/dataflow/custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15599 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/dataflow/parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/dataflow/serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9604 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/dataflow/stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.787733 deepdoctection-0.25/deepdoctection/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19089 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/datapoint/annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23341 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/datapoint/box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6824 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/datapoint/convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    27294 2023-05-23 14:43:35.000000 deepdoctection-0.25/deepdoctection/datapoint/image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    31183 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/datapoint/view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.787733 deepdoctection-0.25/deepdoctection/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7421 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/datasets/adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18887 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/datasets/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4105 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/dataflow_builder.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20603 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/datasets/info.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.791733 deepdoctection-0.25/deepdoctection/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/datasets/instances/doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11968 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/datasets/instances/fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6491 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-02-20 09:20:02.000000 deepdoctection-0.25/deepdoctection/datasets/instances/publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11948 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/datasets/instances/pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8509 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/datasets/instances/pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/instances/xfund.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.791733 deepdoctection-0.25/deepdoctection/datasets/instances/xsl/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/datasets/instances/xsl/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3326 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/datasets/save.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.795733 deepdoctection-0.25/deepdoctection/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2022-06-30 08:30:21.000000 deepdoctection-0.25/deepdoctection/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19509 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/eval/accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4804 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/eval/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8755 2023-06-28 06:38:28.000000 deepdoctection-0.25/deepdoctection/eval/cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19097 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/eval/eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/eval/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9069 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/eval/tedsmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5713 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/eval/tp_eval_callback.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.799733 deepdoctection-0.25/deepdoctection/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1140 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11989 2023-06-28 06:38:28.000000 deepdoctection-0.25/deepdoctection/extern/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11010 2023-05-07 17:37:06.000000 deepdoctection-0.25/deepdoctection/extern/d2detect.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12381 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/extern/doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9319 2023-05-07 17:37:06.000000 deepdoctection-0.25/deepdoctection/extern/hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    39403 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/extern/hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    46449 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/extern/model.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/pdftext.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.799733 deepdoctection-0.25/deepdoctection/extern/pt/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      699 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/pt/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2022-06-22 06:44:07.000000 deepdoctection-0.25/deepdoctection/extern/pt/ptutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12292 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/extern/tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5654 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/extern/texocr.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.803733 deepdoctection-0.25/deepdoctection/extern/tp/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2022-06-22 06:44:07.000000 deepdoctection-0.25/deepdoctection/extern/tp/tfutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpcompat.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.803733 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3664 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/common.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.803733 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/config/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/config/config.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.807733 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9362 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13545 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11006 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17743 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4597 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4215 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/predict.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/preproc.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.807733 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-02-13 13:44:17.000000 deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7525 2023-05-07 17:37:06.000000 deepdoctection-0.25/deepdoctection/extern/tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.811733 deepdoctection-0.25/deepdoctection/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1390 2023-02-13 13:44:17.000000 deepdoctection-0.25/deepdoctection/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15505 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/mapper/cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6055 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/mapper/cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8537 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/mapper/d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5593 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/mapper/hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    35638 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/mapper/laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7775 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/mapper/maputils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7912 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/mapper/match.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/mapper/misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2022-09-21 17:02:22.000000 deepdoctection-0.25/deepdoctection/mapper/pascalstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6876 2022-09-27 06:19:11.000000 deepdoctection-0.25/deepdoctection/mapper/prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23583 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/mapper/pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5090 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/mapper/tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8808 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/mapper/xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.819733 deepdoctection-0.25/deepdoctection/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1121 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13961 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13245 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/pipe/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11062 2023-05-23 14:43:35.000000 deepdoctection-0.25/deepdoctection/pipe/cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13942 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9425 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/pipe/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8872 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/doctectionpipe.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5579 2023-06-22 12:40:28.000000 deepdoctection-0.25/deepdoctection/pipe/language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5262 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/pipe/layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/pipe/lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    32279 2023-06-29 09:06:33.000000 deepdoctection-0.25/deepdoctection/pipe/order.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22418 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/pipe/refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      902 2022-08-12 12:59:53.000000 deepdoctection-0.25/deepdoctection/pipe/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    50554 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/pipe/segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10977 2023-06-30 07:04:23.000000 deepdoctection-0.25/deepdoctection/pipe/text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3138 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/pipe/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-05-07 15:01:33.000000 deepdoctection-0.25/deepdoctection/py.typed
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.819733 deepdoctection-0.25/deepdoctection/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15612 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/train/d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10538 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/train/hf_detr_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    21125 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/train/hf_layoutlm_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12968 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/train/tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.827733 deepdoctection-0.25/deepdoctection/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2238 2022-09-27 06:16:10.000000 deepdoctection-0.25/deepdoctection/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4612 2023-01-05 12:44:38.000000 deepdoctection-0.25/deepdoctection/utils/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3998 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/context.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2022-09-12 13:32:10.000000 deepdoctection-0.25/deepdoctection/utils/detection_types.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3441 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/develop.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17992 2023-02-23 18:53:12.000000 deepdoctection-0.25/deepdoctection/utils/file_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7626 2022-09-27 06:19:11.000000 deepdoctection-0.25/deepdoctection/utils/fs.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2022-06-16 05:58:47.000000 deepdoctection-0.25/deepdoctection/utils/identifier.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8627 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/logger.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/metacfg.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7564 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/pdf_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11954 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/utils/settings.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1923 2023-01-27 07:53:16.000000 deepdoctection-0.25/deepdoctection/utils/systools.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1813 2022-09-12 13:32:10.000000 deepdoctection-0.25/deepdoctection/utils/tqdm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8247 2023-02-09 09:34:37.000000 deepdoctection-0.25/deepdoctection/utils/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2022-09-27 06:19:11.000000 deepdoctection-0.25/deepdoctection/utils/utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10115 2023-06-09 06:48:22.000000 deepdoctection-0.25/deepdoctection/utils/viz.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.783733 deepdoctection-0.25/deepdoctection.egg-info/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10653 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7958 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/SOURCES.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)        1 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/dependency_links.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/requires.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)       30 2023-06-30 11:37:43.000000 deepdoctection-0.25/deepdoctection.egg-info/top_level.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2368 2023-06-30 11:37:43.859732 deepdoctection-0.25/setup.cfg
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6406 2023-06-30 11:37:35.000000 deepdoctection-0.25/setup.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.827733 deepdoctection-0.25/tests/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      725 2022-09-18 14:33:32.000000 deepdoctection-0.25/tests/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.827733 deepdoctection-0.25/tests/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5326 2023-06-30 07:04:23.000000 deepdoctection-0.25/tests/analyzer/test_dd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17378 2023-05-03 16:43:31.000000 deepdoctection-0.25/tests/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    64681 2022-11-28 15:25:21.000000 deepdoctection-0.25/tests/data.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.831733 deepdoctection-0.25/tests/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/dataflow/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/dataflow/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/dataflow/test_custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/dataflow/test_custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/dataflow/test_parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/dataflow/test_stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.831733 deepdoctection-0.25/tests/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2022-09-06 06:55:23.000000 deepdoctection-0.25/tests/datapoint/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4860 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/datapoint/test_annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/datapoint/test_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/datapoint/test_convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12141 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/datapoint/test_image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3670 2023-06-22 12:40:28.000000 deepdoctection-0.25/tests/datapoint/test_view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.835733 deepdoctection-0.25/tests/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/datasets/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.835733 deepdoctection-0.25/tests/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      974 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/datasets/instances/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2022-11-03 14:05:55.000000 deepdoctection-0.25/tests/datasets/instances/test_doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/datasets/instances/test_fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2091 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/datasets/instances/test_funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1263 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/datasets/instances/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/datasets/instances/test_layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/datasets/instances/test_publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1921 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/datasets/instances/test_pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/datasets/instances/test_pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/datasets/instances/test_rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2704 2022-06-29 12:05:00.000000 deepdoctection-0.25/tests/datasets/test_adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/datasets/test_info.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/datasets/test_registry.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.839733 deepdoctection-0.25/tests/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/eval/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/eval/test_accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3803 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/eval/test_cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2952 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/eval/test_eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/eval/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1253 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/eval/test_tedsmetric.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.843732 deepdoctection-0.25/tests/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/extern/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/extern/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1652 2022-11-03 14:06:59.000000 deepdoctection-0.25/tests/extern/test_deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4973 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/extern/test_doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2142 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/extern/test_fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3781 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/extern/test_hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19460 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/extern/test_hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2066 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/extern/test_pdftext.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/extern/test_tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1734 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/extern/test_texocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4372 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/extern/test_tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.847733 deepdoctection-0.25/tests/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/mapper/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    81693 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/mapper/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10518 2023-06-09 06:48:22.000000 deepdoctection-0.25/tests/mapper/test_cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/mapper/test_cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1907 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/mapper/test_d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2050 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/mapper/test_hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2382 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/mapper/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5556 2023-06-09 06:48:22.000000 deepdoctection-0.25/tests/mapper/test_laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/mapper/test_misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2867 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/mapper/test_prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/mapper/test_pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/mapper/test_tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/mapper/test_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/mapper/test_xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.855733 deepdoctection-0.25/tests/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6290 2022-10-24 07:01:39.000000 deepdoctection-0.25/tests/pipe/test_anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4498 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/pipe/test_cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3449 2023-02-13 13:44:17.000000 deepdoctection-0.25/tests/pipe/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2676 2023-06-22 12:40:28.000000 deepdoctection-0.25/tests/pipe/test_language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2022-10-24 07:01:39.000000 deepdoctection-0.25/tests/pipe/test_layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4604 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/pipe/test_lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-06-22 12:40:28.000000 deepdoctection-0.25/tests/pipe/test_order.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9676 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/pipe/test_refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-05-07 15:01:33.000000 deepdoctection-0.25/tests/pipe/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14433 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests/pipe/test_segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-06-22 12:40:28.000000 deepdoctection-0.25/tests/pipe/test_text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2022-11-03 14:06:59.000000 deepdoctection-0.25/tests/pipe/test_transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2260 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/test_utils.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.855733 deepdoctection-0.25/tests/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-01-27 07:53:16.000000 deepdoctection-0.25/tests/train/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2022-09-29 09:12:15.000000 deepdoctection-0.25/tests/train/test_d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3540 2022-10-12 13:27:51.000000 deepdoctection-0.25/tests/train/test_tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2023-06-30 11:37:43.855733 deepdoctection-0.25/tests_d2/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      761 2022-06-16 05:58:47.000000 deepdoctection-0.25/tests_d2/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1580 2022-09-21 17:02:23.000000 deepdoctection-0.25/tests_d2/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3226 2023-02-09 09:34:37.000000 deepdoctection-0.25/tests_d2/test_d2detect.py
```

### Comparing `deepdoctection-0.24/LICENSE` & `deepdoctection-0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/PKG-INFO` & `deepdoctection-0.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.24
+Version: 0.25
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -50,25 +50,22 @@
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
- - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
-   provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). 
-
-   [**!new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE) 
-   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v1_on_custom_token_classification.ipynb)
-   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3. Training 
-   scripts can now be tracked with W&B. Check the experimentation result of the notebooks [here](https://wandb.ai/jm76/FRFPE_layoutlmv1?workspace=user-jm76).
- - Table detection and table structure recognition with 
+ - Document and token classification with all LayoutLM models provided by the Transformer library. 
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
+   Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
+ - [**new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
+   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
+   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
```

### Comparing `deepdoctection-0.24/README.md` & `deepdoctection-0.25/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,22 @@
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
- - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
-   provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). 
-
-   [**!new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE) 
-   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v1_on_custom_token_classification.ipynb)
-   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3. Training 
-   scripts can now be tracked with W&B. Check the experimentation result of the notebooks [here](https://wandb.ai/jm76/FRFPE_layoutlmv1?workspace=user-jm76).
- - Table detection and table structure recognition with 
+ - Document and token classification with all LayoutLM models provided by the Transformer library. 
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
+   Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
+ - [**new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
+   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
+   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
```

### Comparing `deepdoctection-0.24/deepdoctection/__init__.py` & `deepdoctection-0.25/deepdoctection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import TYPE_CHECKING
 
 from packaging import version
 
 from .utils.file_utils import _LazyModule, get_tf_version, pytorch_available, tf_available
 from .utils.logger import logger
 
-__version__ = 0.24
+__version__ = 0.25
 
 _IMPORT_STRUCTURE = {
     "analyzer": ["get_dd_analyzer", "build_analyzer"],
     "configs": [],
     "dataflow": [
         "DataFlowTerminated",
         "DataFlowResetStateNotCalled",
@@ -240,22 +240,24 @@
         "MultiThreadPipelineComponent",
         "DoctectionPipe",
         "LanguageDetectionService",
         "ImageLayoutService",
         "get_tokenizer_from_architecture",
         "LMTokenClassifierService",
         "LMSequenceClassifierService",
+        "OrderGenerator",
+        "TextLineGenerator",
+        "TextOrderService",
         "TableSegmentationRefinementService",
         "generate_html_string",
         "pipeline_component_registry",
         "TableSegmentationService",
         "PubtablesSegmentationService",
         "SegmentationResult",
         "TextExtractionService",
-        "TextOrderService",
         "SimpleTransformPipelineComponent",
     ],
     "train": [
         "D2Trainer",
         "train_d2_faster_rcnn",
         "LayoutLMTrainer",
         "train_hf_layoutlm",
```

### Comparing `deepdoctection-0.24/deepdoctection/analyzer/__init__.py` & `deepdoctection-0.25/deepdoctection/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/configs/__init__.py` & `deepdoctection-0.25/deepdoctection/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/dataflow/__init__.py` & `deepdoctection-0.25/deepdoctection/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/dataflow/base.py` & `deepdoctection-0.25/deepdoctection/dataflow/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/dataflow/common.py` & `deepdoctection-0.25/deepdoctection/dataflow/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/dataflow/custom.py` & `deepdoctection-0.25/deepdoctection/dataflow/custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/dataflow/custom_serialize.py` & `deepdoctection-0.25/deepdoctection/dataflow/custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/dataflow/parallel_map.py` & `deepdoctection-0.25/deepdoctection/dataflow/parallel_map.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/dataflow/serialize.py` & `deepdoctection-0.25/deepdoctection/dataflow/serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/dataflow/stats.py` & `deepdoctection-0.25/deepdoctection/dataflow/stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datapoint/__init__.py` & `deepdoctection-0.25/deepdoctection/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datapoint/annotation.py` & `deepdoctection-0.25/deepdoctection/datapoint/annotation.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datapoint/box.py` & `deepdoctection-0.25/deepdoctection/datapoint/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,18 +323,18 @@
         :return: Either a list or np.array.
         """
 
         if absolute_coords != self.absolute_coords:  # only transforming in this case
             if self.absolute_coords:
                 transformed_box = BoundingBox(
                     absolute_coords=not self.absolute_coords,
-                    ulx=self.ulx / image_width,
-                    uly=self.uly / image_height,
-                    lrx=self.lrx / image_width,
-                    lry=self.lry / image_height,
+                    ulx=max(self.ulx / image_width, 0.0),
+                    uly=max(self.uly / image_height, 0.0),
+                    lrx=min(self.lrx / image_width, 1.0),
+                    lry=min(self.lry / image_height, 1.0),
                 )
             else:
                 transformed_box = BoundingBox(
                     absolute_coords=not self.absolute_coords,
                     ulx=self.ulx * image_width,
                     uly=self.uly * image_height,
                     lrx=self.lrx * image_width,
```

### Comparing `deepdoctection-0.24/deepdoctection/datapoint/convert.py` & `deepdoctection-0.25/deepdoctection/datapoint/convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datapoint/image.py` & `deepdoctection-0.25/deepdoctection/datapoint/image.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datapoint/view.py` & `deepdoctection-0.25/deepdoctection/datapoint/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 """
 Subclasses for ImageAnnotation and Image objects with various properties. These classes
 simplify consumption
 """
 
 from copy import copy
-from itertools import chain
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Type, Union, no_type_check
 
 import cv2
 import numpy as np
 
 from ..utils.detection_types import ImageType, JsonDict, Pathlike
 from ..utils.logger import logger
@@ -156,17 +155,34 @@
         return [self]
 
     @property
     def text(self) -> str:
         """
         Text captured within the instance respecting the reading order of each word.
         """
+        words = self.get_ordered_words()
+        return " ".join([word.characters for word in words])  # type: ignore
+
+    def get_ordered_words(self) -> List[ImageAnnotationBaseView]:
+        """Returns a list of words order by reading order. Words with no reading order will not be returned"""
         words_with_reading_order = [word for word in self.words if word.reading_order is not None]
         words_with_reading_order.sort(key=lambda x: x.reading_order)  # type: ignore
-        return " ".join([word.characters for word in words_with_reading_order])  # type: ignore
+        return words_with_reading_order
+
+    @property
+    def text_(self) -> Dict[str, Union[str, List[str]]]:
+        """Returns a dict `{"text": text string,
+        "text_list": list of single words,
+        "annotation_ids": word annotation ids`"""
+        words = self.get_ordered_words()
+        return {
+            "text": " ".join([word.characters for word in words]),  # type: ignore
+            "text_list": [word.characters for word in words],  # type: ignore
+            "annotation_ids": [word.annotation_id for word in words],
+        }
 
     def get_attribute_names(self) -> Set[str]:
         return {"words", "text"}.union(super().get_attribute_names()).union({Relationships.reading_order})
 
     def __len__(self) -> int:
         """len of text counted by number of characters"""
         return len(self.text)
@@ -259,47 +275,67 @@
         row or column spans will be shown at the upper left cell tile. All other tiles covered by the cell will be left
         as blank
         """
         cells = self.cells
         table_list = [["" for _ in range(self.number_of_columns)] for _ in range(self.number_of_rows)]  # type: ignore
         for cell in cells:
             table_list[cell.row_number - 1][cell.column_number - 1] = (  # type: ignore
-                table_list[cell.row_number - 1][cell.column_number - 1] + cell.text  # type: ignore
+                table_list[cell.row_number - 1][cell.column_number - 1] + cell.text + " "  # type: ignore
             )
         return table_list
 
     def __str__(self) -> str:
         out = " ".join([" ".join(row + ["\n"]) for row in self.csv])
         return out
 
     @property
     def text(self) -> str:
-        return str(self)
+        try:
+            return str(self)
+        except TypeError:
+            return super().text
+
+    @property
+    def text_(self) -> Dict[str, Union[str, List[str]]]:
+        cells = self.cells
+        if not cells:
+            return super().text_
+        text_list: List[str] = []
+        annotation_id_list: List[str] = []
+        for cell in cells:
+            text_list.extend(cell.text_["text_list"])  # type: ignore
+            annotation_id_list.extend(cell.text_["annotation_ids"])  # type: ignore
+        return {
+            "text": " ".join([cell.text for cell in cells]),  # type: ignore
+            "text_list": text_list,
+            "annotation_ids": annotation_id_list,
+        }
 
 
 IMAGE_ANNOTATION_TO_LAYOUTS: Dict[ObjectTypes, Type[Union[Layout, Table, Word]]] = {
     **{i: Layout for i in LayoutType if (i not in {LayoutType.table, LayoutType.word, LayoutType.cell})},
     LayoutType.table: Table,
+    LayoutType.table_rotated: Table,
     LayoutType.word: Word,
     LayoutType.cell: Cell,
     CellType.projected_row_header: Cell,
     CellType.spanning: Cell,
     CellType.row_header: Cell,
     CellType.column_header: Cell,
 }
 
 IMAGE_DEFAULTS: Dict[str, Union[LayoutType, Sequence[ObjectTypes]]] = {
     "text_container": LayoutType.word,
-    "top_level_text_block_names": [
-        LayoutType.table,
+    "floating_text_block_categories": [
         LayoutType.text,
         LayoutType.title,
         LayoutType.figure,
         LayoutType.list,
     ],
+    "text_block_categories": [LayoutType.text, LayoutType.title, LayoutType.figure, LayoutType.list, LayoutType.cell],
 }
 
 
 @no_type_check
 def ann_obj_view_factory(annotation: ImageAnnotation, text_container: ObjectTypes) -> ImageAnnotationBaseView:
     """
     Create an `ImageAnnotationBaseView` sub class given the mapping `IMAGE_ANNOTATION_TO_LAYOUTS` .
@@ -331,25 +367,22 @@
 
     Its factory function `Page().from_image(image, text_container, text_block_names)` creates for every
     `ImageAnnotation` a corresponding subclass of `ImageAnnotationBaseView` which drives the object towards
     less generic classes with custom attributes that are controlled some `ObjectTypes`.
 
     top_level_text_block_names: Top level layout objects, e.g. `LayoutType.text` or `LayoutType.table`.
 
-    text_block_names: layout objects that have associated text
-
     image_orig: Base image
 
     text_container: LayoutType to take the text from
     """
 
-    top_level_text_block_names: List[ObjectTypes]
-    text_block_names: Optional[List[ObjectTypes]]
-    image_orig: Image
     text_container: ObjectTypes
+    floating_text_block_categories: List[ObjectTypes]
+    image_orig: Image
 
     @no_type_check
     def get_annotation(
         self,
         category_names: Optional[Union[str, ObjectTypes, Sequence[Union[str, ObjectTypes]]]] = None,
         annotation_ids: Optional[Union[str, Sequence[str]]] = None,
         annotation_types: Optional[Union[str, Sequence[str]]] = None,
@@ -390,77 +423,63 @@
                     return sub_cat.value
                 return int(sub_cat.category_id)
         return None
 
     @property
     def layouts(self) -> List[ImageAnnotationBaseView]:
         """
-        A list of a layouts.
+        A list of a layouts. Layouts are all exactly all floating text block categories
         """
-        layouts = [layout for layout in self.top_level_text_block_names if layout != LayoutType.table]
-        return self.get_annotation(category_names=layouts)
+        return self.get_annotation(category_names=self.floating_text_block_categories)
 
     @property
     def words(self) -> List[ImageAnnotationBaseView]:
         """
-        A list of a words.
+        A list of a words. Word are all text containers
         """
         return self.get_annotation(category_names=self.text_container)
 
     @property
-    def residual_words(self) -> List[ImageAnnotationBaseView]:
-        """
-        A list of a words that have not been assigned to any text block but have a reading order.
-        Words having this property appear, once `text_containers_to_text_block=True`.
-        """
-        if self.text_block_names is None:
-            return []
-        text_block_anns = self.get_annotation(category_names=self.text_block_names)
-        text_ann_ids = list(
-            chain(*[text_block.get_relationship(Relationships.child) for text_block in text_block_anns])
-        )
-        text_container_anns = self.get_annotation(category_names=self.text_container)
-        residual_words = [ann for ann in text_container_anns if ann.annotation_id not in text_ann_ids]
-        return residual_words
-
-    @property
     def tables(self) -> List[ImageAnnotationBaseView]:
         """
         A list of a tables.
         """
         return self.get_annotation(category_names=LayoutType.table)
 
     @classmethod
     def from_image(
         cls,
         image_orig: Image,
         text_container: Optional[ObjectTypes] = None,
-        top_level_text_block_names: Optional[List[ObjectTypes]] = None,
-        text_block_names: Optional[List[ObjectTypes]] = None,
+        floating_text_block_categories: Optional[Sequence[ObjectTypes]] = None,
+        include_residual_text_container: bool = True,
         base_page: Optional["Page"] = None,
     ) -> "Page":
         """
         Factory function for generating a `Page` instance from `image_orig` .
 
         :param image_orig: `Image` instance to convert
         :param text_container: A LayoutType to get the text from. It will steer the output of `Layout.words`.
-        :param top_level_text_block_names: A list of top level layout objects
-        :param text_block_names: name of image annotation that have a relation with text containers (or which might be
-                                 text containers themselves). This is only necessary, when residual text_container (e.g.
-                                 words that have not been assigned to any text block) should be displayed in `page.text`
+        :param floating_text_block_categories: A list of top level layout objects
+        :param include_residual_text_container: This will regard synthetic text line annotations as floating text
+                                                blocks and therefore incorporate all image annotations of category
+                                                `word` when building text strings.
         :param base_page: For top level objects that are images themselves, pass the page that encloses all objects.
                           In doubt, do not populate this value.
         :return:
         """
 
         if text_container is None:
             text_container = IMAGE_DEFAULTS["text_container"]  # type: ignore
 
-        if top_level_text_block_names is None:
-            top_level_text_block_names = IMAGE_DEFAULTS["top_level_text_block_names"]  # type: ignore
+        if not floating_text_block_categories:
+            floating_text_block_categories = copy(IMAGE_DEFAULTS["floating_text_block_categories"])  # type: ignore
+
+        if include_residual_text_container and LayoutType.line not in floating_text_block_categories:  # type: ignore
+            floating_text_block_categories.append(LayoutType.line)  # type: ignore
 
         img_kwargs = image_orig.as_dict()
         page = cls(
             img_kwargs.get("file_name"), img_kwargs.get("location"), img_kwargs.get("external_id")  # type: ignore
         )
         page.image_orig = image_orig
         page.page_number = image_orig.page_number
@@ -480,45 +499,56 @@
             image_ann = ImageAnnotation.from_dict(**ann_dict)
             layout_ann = ann_obj_view_factory(image_ann, text_container)
             if "image" in ann_dict:
                 image_dict = ann_dict["image"]
                 if image_dict:
                     image = Image.from_dict(**image_dict)
                     layout_ann.image = cls.from_image(
-                        image, text_container, top_level_text_block_names, text_block_names, page
+                        image, text_container, floating_text_block_categories, base_page=page
                     )
             layout_ann.base_page = base_page if base_page is not None else page
             page.dump(layout_ann)
         if summary_dict := img_kwargs.get("_summary"):
             page.summary = SummaryAnnotation.from_dict(**summary_dict)
-        page.top_level_text_block_names = top_level_text_block_names  # type: ignore
-        page.text_block_names = text_block_names
+        page.floating_text_block_categories = floating_text_block_categories  # type: ignore
         page.text_container = text_container  # type: ignore
         return page
 
     def _order(self, block: str) -> List[ImageAnnotationBaseView]:
         blocks_with_order = [layout for layout in getattr(self, block) if layout.reading_order is not None]
-        if self.residual_words:
-            blocks_with_order.extend(self.residual_words)
         blocks_with_order.sort(key=lambda x: x.reading_order)
         return blocks_with_order
 
+    def _make_text(self, line_break: bool = True) -> str:
+        text: str = ""
+        block_with_order = self._order("layouts")
+        break_str = "\n" if line_break else " "
+        for block in block_with_order:
+            text += f"{block.text}{break_str}"
+        return text
+
     @property
     def text(self) -> str:
         """
         Get text of all layouts.
         """
-        text: str = ""
-        block_name = "layouts" if self.layouts else "words"
-        block_with_order = self._order(block_name)
-        linebreak = "\n" if block_name == "layouts" else " "
+        return self._make_text()
+
+    @property
+    def text_(self) -> Dict[str, Union[str, List[str]]]:
+        """Returns a dict `{"text": text string,
+        "text_list": list of single words,
+        "annotation_ids": word annotation ids`"""
+        block_with_order = self._order("layouts")
+        text_list: List[str] = []
+        annotation_id_list: List[str] = []
         for block in block_with_order:
-            block_attr = "text" if not isinstance(block, Word) else "characters"
-            text += f"{linebreak}{getattr(block, block_attr)}"
-        return text
+            text_list.extend(block.text_["text_list"])  # type: ignore
+            annotation_id_list.extend(block.text_["annotation_ids"])  # type: ignore
+        return {"text": self.text, "text_list": text_list, "annotation_ids": annotation_id_list}
 
     @property
     def chunks(self) -> List[Tuple[str, str, int, str, str, str, str]]:
         """
         :return: Returns a "chunk" of a layout element or a table as 6-tuple containing
 
                     - document id
@@ -551,20 +581,15 @@
 
     @property
     def text_no_line_break(self) -> str:
         """
         Get text of all layouts. While `text` will do a line break for each layout block this here will return the
         string in one single line.
         """
-        text: str = ""
-        layouts_with_order = self._order("layouts")
-        for layout in layouts_with_order:
-            text += " " + layout.text  # type: ignore
-
-        return text
+        return self._make_text(False)
 
     @no_type_check
     def viz(
         self,
         show_tables: bool = True,
         show_layouts: bool = True,
         show_cells: bool = True,
@@ -640,18 +665,17 @@
             for layout in self.layouts:
                 all_words.extend(layout.words)
             if not all_words:
                 all_words = self.get_annotation(category_names=LayoutType.word)
             for word in all_words:
                 box_stack.append(word.bbox)
                 if show_token_class:
-                    category_names_list.append(word.token_class.value)
+                    category_names_list.append(word.token_class.value if word.token_class is not None else None)
                 else:
-                    category_names_list.append(word.token_tag.value)
-
+                    category_names_list.append(word.token_tag.value if word.token_tag is not None else None)
 
         if self.image is not None:
             if box_stack:
                 boxes = np.vstack(box_stack)
                 if show_words:
                     img = draw_boxes(
                         self.image,
@@ -680,15 +704,14 @@
         return set(PageType).union(
             {
                 "text",
                 "chunks",
                 "tables",
                 "layouts",
                 "words",
-                "residual_words",
                 "file_name",
                 "location",
                 "document_id",
                 "page_number",
             }
         )
 
@@ -714,12 +737,20 @@
 
     @classmethod
     @no_type_check
     def from_file(
         cls,
         file_path: str,
         text_container: Optional[ObjectTypes] = None,
-        top_level_text_block_names: Optional[List[ObjectTypes]] = None,
-        text_block_names: Optional[List[ObjectTypes]] = None,
+        floating_text_block_categories: Optional[List[ObjectTypes]] = None,
+        include_residual_text_container: bool = True,
     ) -> "Page":
+        """Reading JSON file and building a `Page` object with given config.
+        :param file_path: Path to file
+        :param text_container: A LayoutType to get the text from. It will steer the output of `Layout.words`.
+        :param floating_text_block_categories: A list of top level layout objects
+        :param include_residual_text_container: This will regard synthetic text line annotations as floating text
+                                                blocks and therefore incorporate all image annotations of category
+                                                `word` when building text strings.
+        """
         image = Image.from_file(file_path)
-        return cls.from_image(image, text_container, top_level_text_block_names, text_block_names)
+        return cls.from_image(image, text_container, floating_text_block_categories, include_residual_text_container)
```

### Comparing `deepdoctection-0.24/deepdoctection/datasets/__init__.py` & `deepdoctection-0.25/deepdoctection/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/adapter.py` & `deepdoctection-0.25/deepdoctection/datasets/adapter.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/base.py` & `deepdoctection-0.25/deepdoctection/datasets/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/dataflow_builder.py` & `deepdoctection-0.25/deepdoctection/datasets/dataflow_builder.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/info.py` & `deepdoctection-0.25/deepdoctection/datasets/info.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/__init__.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/doclaynet.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/fintabnet.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/funsd.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/funsd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/iiitar13k.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/layouttest.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/publaynet.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/pubtables1m.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/pubtables1m.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/pubtabnet.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/rvlcdip.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/xfund.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/xfund.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/xsl/__init__.py` & `deepdoctection-0.25/deepdoctection/datasets/instances/xsl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/instances/xsl/pascal_voc.xsl` & `deepdoctection-0.25/deepdoctection/datasets/instances/xsl/pascal_voc.xsl`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/registry.py` & `deepdoctection-0.25/deepdoctection/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/datasets/save.py` & `deepdoctection-0.25/deepdoctection/datasets/save.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/eval/__init__.py` & `deepdoctection-0.25/deepdoctection/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/eval/accmetric.py` & `deepdoctection-0.25/deepdoctection/eval/accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/eval/base.py` & `deepdoctection-0.25/deepdoctection/eval/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/eval/cocometric.py` & `deepdoctection-0.25/deepdoctection/eval/cocometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,17 +133,17 @@
         anns_gt, anns_pr = [], []
 
         dataflow_gt.reset_state()
         dataflow_predictions.reset_state()
 
         for dp_gt, dp_pred in zip(dataflow_gt, dataflow_predictions):
             img_gt, ann_gt = cls.mapper(dp_gt)  # type: ignore
-            dp_pred = re_assign_cat_ids(  # pylint: disable=E1120
-                categories.get_categories(as_dict=True, filtered=True, name_as_key=True)
-            )(dp_pred)
+            dp_pred = re_assign_cat_ids(categories.get_categories(as_dict=True, filtered=True, name_as_key=True))(
+                dp_pred
+            )
             img_pr, ann_pr = cls.mapper(dp_pred)  # type: ignore
             imgs_gt.append(img_gt)
             imgs_pr.append(img_pr)
             anns_gt.extend(ann_gt)
             anns_pr.extend(ann_pr)
 
         dataset_gt = {"images": imgs_gt, "annotations": anns_gt, "categories": cats}
```

### Comparing `deepdoctection-0.24/deepdoctection/eval/eval.py` & `deepdoctection-0.25/deepdoctection/eval/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,24 +294,15 @@
         df_gt = self.dataset.dataflow.build(**kwargs)
         df_pr = self.dataset.dataflow.build(**kwargs)
         df_gt = MapData(df_gt, maybe_load_image)
         df_pr = MapData(df_pr, maybe_load_image)
         df_pr = MapData(df_pr, deepcopy)
         df_pr = self._clean_up_predict_dataflow_annotations(df_pr)
 
-        page_parsing_component = PageParsingService(
-            text_container=LayoutType.word,
-            top_level_text_block_names=[
-                LayoutType.title,
-                LayoutType.text,
-                LayoutType.list,
-                LayoutType.table,
-                LayoutType.figure,
-            ],
-        )
+        page_parsing_component = PageParsingService(text_container=LayoutType.word)
         df_gt = page_parsing_component.predict_dataflow(df_gt)
 
         if self.pipe_component:
             pipe_component = self.pipe_component.pipe_components[0]
             df_pr = pipe_component.predict_dataflow(df_pr)
             df_pr = page_parsing_component.predict_dataflow(df_pr)
```

### Comparing `deepdoctection-0.24/deepdoctection/eval/registry.py` & `deepdoctection-0.25/deepdoctection/eval/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/eval/tedsmetric.py` & `deepdoctection-0.25/deepdoctection/eval/tedsmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/eval/tp_eval_callback.py` & `deepdoctection-0.25/deepdoctection/eval/tp_eval_callback.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/__init__.py` & `deepdoctection-0.25/deepdoctection/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/base.py` & `deepdoctection-0.25/deepdoctection/extern/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 """
 Abstract classes for unifying external base- and Doctection predictors
 """
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, List, Mapping, Optional, Tuple, Union
+from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
 
 from ..utils.detection_types import ImageType, JsonDict, Requirement
 from ..utils.settings import DefaultType, ObjectTypes, TypeOrStr, get_type
 
 
 class PredictorBase(ABC):
     """
@@ -83,26 +83,29 @@
     `text`: text string. Used for OCR predictors
 
     `block`: block number. For reading order from some ocr predictors
 
     `line`: line number. For reading order from some ocr predictors
 
     `uuid`: uuid. For assigning detection result (e.g. text to image annotations)
+
+
     """
 
     box: Optional[List[float]] = None
     class_id: Optional[int] = None
     score: Optional[float] = None
     mask: Optional[List[float]] = None
     absolute_coords: bool = True
     class_name: ObjectTypes = DefaultType.default_type
     text: Optional[Union[str, ObjectTypes]] = None
     block: Optional[str] = None
     line: Optional[str] = None
     uuid: Optional[str] = None
+    relationships: Optional[Dict[str, Any]] = None
 
 
 class ObjectDetector(PredictorBase):
     """
     Abstract base class for object detection. This can be anything ranging from layout detection to OCR.
     Use this to connect external detectors with Deep-Doctection predictors on images.
 
@@ -238,36 +241,38 @@
 
      `bio_tag`: bio tag
 
      `score`: prediction score
     """
 
     uuid: str
-    token_id: int
     token: str
     class_id: int
     class_name: ObjectTypes = DefaultType.default_type
     semantic_name: ObjectTypes = DefaultType.default_type
     bio_tag: ObjectTypes = DefaultType.default_type
     score: Optional[float] = None
+    token_id: Optional[int] = None
 
 
 @dataclass
 class SequenceClassResult:
     """
     Storage for sequence classification results
 
     `class_id`: category id
     `class_name`: category name
     `score`: prediction score
+    `class_name_orig`: original class name
     """
 
     class_id: int
     class_name: ObjectTypes = DefaultType.default_type
     score: Optional[float] = None
+    class_name_orig: Optional[str] = None
 
 
 class LMTokenClassifier(PredictorBase):
     """
     Abstract base class for token classifiers. If you want to connect external token classifiers with Deepdoctection
     predictors wrap them into a class derived from this class. Note, that this class is still DL library agnostic.
     """
```

### Comparing `deepdoctection-0.24/deepdoctection/extern/d2detect.py` & `deepdoctection-0.25/deepdoctection/extern/d2detect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/deskew.py` & `deepdoctection-0.25/deepdoctection/extern/deskew.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/doctrocr.py` & `deepdoctection-0.25/deepdoctection/extern/doctrocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/fastlang.py` & `deepdoctection-0.25/deepdoctection/extern/fastlang.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/hfdetr.py` & `deepdoctection-0.25/deepdoctection/extern/hfdetr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/hflayoutlm.py` & `deepdoctection-0.25/deepdoctection/extern/hflayoutlm.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 def predict_token_classes(
     uuids: List[List[str]],
     input_ids: "Tensor",
     attention_mask: "Tensor",
     token_type_ids: "Tensor",
     boxes: "Tensor",
     tokens: List[List[str]],
-    model: Union["LayoutLMForTokenClassification",
-                 "LayoutLMv2ForTokenClassification",
-                 "LayoutLMv3ForTokenClassification"],
+    model: Union[
+        "LayoutLMForTokenClassification", "LayoutLMv2ForTokenClassification", "LayoutLMv3ForTokenClassification"
+    ],
     images: Optional["Tensor"] = None,
 ) -> List[TokenClassResult]:
     """
     :param uuids: A list of uuids that correspond to a word that induces the resulting token
     :param input_ids: Token converted to ids to be taken from LayoutLMTokenizer
     :param attention_mask: The associated attention masks from padded sequences taken from LayoutLMTokenizer
     :param token_type_ids: Torch tensor of token type ids taken from LayoutLMTokenizer
```

### Comparing `deepdoctection-0.24/deepdoctection/extern/model.py` & `deepdoctection-0.25/deepdoctection/extern/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     hf_repo_id: Optional[str] = field(default=None)
     hf_model_name: Optional[str] = field(default=None)
     hf_config_file: Optional[List[str]] = field(default=None)
     urls: Optional[List[str]] = field(default=None)
     categories: Optional[Dict[str, ObjectTypes]] = field(default=None)
     dl_library: Optional[str] = field(default=None)
     model_wrapper: Optional[str] = field(default=None)
+    architecture: Optional[str] = field(default=None)
 
     def as_dict(self) -> Dict[str, Any]:
         """
         returns a dict of the dataclass
         """
         return asdict(self)
 
@@ -404,15 +405,15 @@
             size=[115393245],
             tp_model=False,
             config="microsoft/table-transformer-detection/config.json",
             preprocessor_config="microsoft/table-transformer-detection/preprocessor_config.json",
             hf_repo_id="microsoft/table-transformer-detection",
             hf_model_name="pytorch_model.bin",
             hf_config_file=["config.json", "preprocessor_config.json"],
-            categories={"1": LayoutType.table},
+            categories={"1": LayoutType.table, "2": LayoutType.table_rotated},
             dl_library="PT",
             model_wrapper="HFDetrDerivedDetector",
         ),
         "microsoft/table-transformer-structure-recognition/pytorch_model.bin": ModelProfile(
             name="microsoft/table-transformer-structure-recognition/pytorch_model.bin",
             description="Table Transformer (DETR) model trained on PubTables1M. It was introduced in the paper "
             "PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents by Smock et "
@@ -442,47 +443,51 @@
             "Binarization”. For more information please check "
             "https://mindee.github.io/doctr/using_doctr/using_models.html#. This is the Pytorch artefact.",
             size=[101971449],
             urls=["https://doctr-static.mindee.com/models?id=v0.3.1/db_resnet50-ac60cadc.pt&src=0"],
             categories={"1": LayoutType.word},
             dl_library="PT",
             model_wrapper="DoctrTextlineDetector",
+            architecture="db_resnet50",
         ),
         "doctr/db_resnet50/tf/db_resnet50-adcafc63.zip": ModelProfile(
             name="doctr/db_resnet50/tf/db_resnet50-adcafc63.zip",
             description="Doctr implementation of DBNet from “Real-time Scene Text Detection with Differentiable "
             "Binarization”. For more information please check "
             "https://mindee.github.io/doctr/using_doctr/using_models.html#. This is the Tensorflow artefact.",
             size=[94178964],
             urls=["https://doctr-static.mindee.com/models?id=v0.2.0/db_resnet50-adcafc63.zip&src=0"],
             categories={"1": LayoutType.word},
             dl_library="TF",
             model_wrapper="DoctrTextlineDetector",
+            architecture="db_resnet50",
         ),
         "doctr/crnn_vgg16_bn/pt/crnn_vgg16_bn-9762b0b0.pt": ModelProfile(
             name="doctr/crnn_vgg16_bn/pt/crnn_vgg16_bn-9762b0b0.pt",
             description="Doctr implementation of CRNN from “An End-to-End Trainable Neural Network for Image-based "
             "Sequence Recognition and Its Application to Scene Text Recognition”. For more information "
             "please check https://mindee.github.io/doctr/using_doctr/using_models.html#. This is the Pytorch "
             "artefact.",
             size=[63286381],
             urls=["https://doctr-static.mindee.com/models?id=v0.3.1/crnn_vgg16_bn-9762b0b0.pt&src=0"],
             dl_library="PT",
             model_wrapper="DoctrTextRecognizer",
+            architecture="crnn_vgg16_bn",
         ),
         "doctr/crnn_vgg16_bn/tf/crnn_vgg16_bn-76b7f2c6.zip": ModelProfile(
             name="doctr/crnn_vgg16_bn/tf/crnn_vgg16_bn-76b7f2c6.zip",
             description="Doctr implementation of CRNN from “An End-to-End Trainable Neural Network for Image-based "
             "Sequence Recognition and Its Application to Scene Text Recognition”. For more information "
             "please check https://mindee.github.io/doctr/using_doctr/using_models.html#. This is the Tensorflow "
             "artefact.",
             size=[58758994],
             urls=["https://doctr-static.mindee.com/models?id=v0.3.0/crnn_vgg16_bn-76b7f2c6.zip&src=0"],
             dl_library="TF",
             model_wrapper="DoctrTextRecognizer",
+            architecture="crnn_vgg16_bn",
         ),
         "fasttext/lid.176.bin": ModelProfile(
             name="fasttext/lid.176.bin",
             description="Fasttext language detection model",
             size=[131266198],
             urls=["https://dl.fbaipublicfiles.com/fasttext/supervised-models/lid.176.bin"],
             categories={
```

### Comparing `deepdoctection-0.24/deepdoctection/extern/pdftext.py` & `deepdoctection-0.25/deepdoctection/extern/pdftext.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/pt/__init__.py` & `deepdoctection-0.25/deepdoctection/extern/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/pt/ptutils.py` & `deepdoctection-0.25/deepdoctection/extern/pt/ptutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tessocr.py` & `deepdoctection-0.25/deepdoctection/extern/tessocr.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,16 +236,14 @@
     ):
         score = float(caption[4])
         if int(score) != -1:
             word = DetectionResult(
                 box=[caption[0], caption[1], caption[0] + caption[2], caption[1] + caption[3]],
                 score=score / 100,
                 text=caption[5],
-                block=str(caption[6]),
-                line=str(caption[7]),
                 class_id=1,
                 class_name=LayoutType.word,
             )
             all_results.append(word)
     if text_lines:
         all_results = tesseract_line_to_detectresult(all_results)
     return all_results
```

### Comparing `deepdoctection-0.24/deepdoctection/extern/texocr.py` & `deepdoctection-0.25/deepdoctection/extern/texocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/__init__.py` & `deepdoctection-0.25/deepdoctection/extern/tp/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tfutils.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tfutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpcompat.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpcompat.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/common.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/config/config.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/config/config.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/predict.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/predict.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/preproc.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/preproc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py` & `deepdoctection-0.25/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/extern/tpdetect.py` & `deepdoctection-0.25/deepdoctection/extern/tpdetect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/__init__.py` & `deepdoctection-0.25/deepdoctection/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/cats.py` & `deepdoctection-0.25/deepdoctection/mapper/cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/cocostruct.py` & `deepdoctection-0.25/deepdoctection/mapper/cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/d2struct.py` & `deepdoctection-0.25/deepdoctection/mapper/d2struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     ann: ImageAnnotation, cat_to_sub_cat: Optional[Mapping[ObjectTypes, ObjectTypes]] = None
 ) -> Tuple[str, str, Optional[float]]:
     if cat_to_sub_cat:
         sub_cat_key = cat_to_sub_cat.get(get_type(ann.category_name))
         if sub_cat_key in ann.sub_categories:
             sub_cat = ann.get_sub_category(sub_cat_key)
             return sub_cat.category_name, sub_cat.category_id, sub_cat.score
-        return "", "", 0.
+        return "", "", 0.0
     return ann.category_name, ann.category_id, ann.score
 
 
 @curry
 def to_wandb_image(
     dp: Image,
     categories: Mapping[str, TypeOrStr],
```

### Comparing `deepdoctection-0.24/deepdoctection/mapper/hfstruct.py` & `deepdoctection-0.25/deepdoctection/mapper/hfstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/laylmstruct.py` & `deepdoctection-0.25/deepdoctection/mapper/laylmstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/maputils.py` & `deepdoctection-0.25/deepdoctection/mapper/maputils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/match.py` & `deepdoctection-0.25/deepdoctection/mapper/match.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/misc.py` & `deepdoctection-0.25/deepdoctection/mapper/misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/pascalstruct.py` & `deepdoctection-0.25/deepdoctection/mapper/pascalstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/prodigystruct.py` & `deepdoctection-0.25/deepdoctection/mapper/prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/pubstruct.py` & `deepdoctection-0.25/deepdoctection/mapper/pubstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/tpstruct.py` & `deepdoctection-0.25/deepdoctection/mapper/tpstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/mapper/xfundstruct.py` & `deepdoctection-0.25/deepdoctection/mapper/xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/pipe/__init__.py` & `deepdoctection-0.25/deepdoctection/pipe/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,12 +25,13 @@
 from .cell import *
 from .common import *
 from .concurrency import *
 from .doctectionpipe import *
 from .language import *
 from .layout import *
 from .lm import *
+from .order import *
 from .refine import *
 from .registry import *
 from .segment import *
 from .text import *
 from .transform import *
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/anngen.py` & `deepdoctection-0.25/deepdoctection/pipe/anngen.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,7 +312,11 @@
         """
         Deactivate annotation by given annotation_id
 
         :param annotation_id: annotation_id
         """
         ann = self._cache_anns[annotation_id]
         ann.deactivate()
+
+    def get_annotation(self, annotation_id: str) -> ImageAnnotation:
+        """get single `ImageAnnotation`"""
+        return self._cache_anns[annotation_id]
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/base.py` & `deepdoctection-0.25/deepdoctection/pipe/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/pipe/cell.py` & `deepdoctection-0.25/deepdoctection/pipe/cell.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/pipe/common.py` & `deepdoctection-0.25/deepdoctection/pipe/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for common pipeline components
 """
-from copy import deepcopy
+from copy import copy, deepcopy
 from typing import List, Literal, Mapping, Optional, Sequence, Union
 
 import numpy as np
 
 from ..dataflow import DataFlow, MapData
 from ..datapoint.image import Image
-from ..datapoint.view import Page
+from ..datapoint.view import IMAGE_DEFAULTS, Page
 from ..mapper.maputils import MappingContextManager
 from ..mapper.match import match_anns_by_intersection
 from ..mapper.misc import to_image
 from ..utils.detection_types import JsonDict
 from ..utils.file_utils import detectron2_available, pytorch_available, tf_available
 from ..utils.settings import LayoutType, ObjectTypes, Relationships, TypeOrStr, get_type
 from .base import PipelineComponent
@@ -165,75 +165,69 @@
     A "pseudo" pipeline component that can be added to a pipeline to convert `Image`s into `Page` formats. It allows a
     custom parsing depending on customizing options of other pipeline components.
     """
 
     def __init__(
         self,
         text_container: TypeOrStr,
-        top_level_text_block_names: Union[TypeOrStr, Sequence[TypeOrStr]],
-        text_block_names: Optional[Union[TypeOrStr, Sequence[TypeOrStr]]] = None,
+        floating_text_block_categories: Optional[Union[TypeOrStr, Sequence[TypeOrStr]]] = None,
+        include_residual_text_container: bool = True,
     ):
         """
         :param text_container: name of an image annotation that has a CHARS sub category. These annotations will be
                                ordered within all text blocks.
-        :param top_level_text_block_names: name of image annotation that have a relation with text containers (or which
-                                           might be text containers themselves).
-        :param text_block_names: name of image annotation that have a relation with text containers (or which might be
-                                 text containers themselves). This is only necessary, when residual text_container (e.g.
-                                 words that have not been assigned to any text block) should be displayed in `page.text`
+        :param floating_text_block_categories: name of image annotation that have a relation with text containers.
         """
         self.name = "page_parser"
-        if isinstance(top_level_text_block_names, (str, ObjectTypes)):
-            top_level_text_block_names = [top_level_text_block_names]
-        if isinstance(text_block_names, (str, ObjectTypes)):
-            text_block_names = [text_block_names]
-        if text_block_names is not None:
-            text_block_names = [get_type(text_block) for text_block in text_block_names]
-
-        self._text_container = get_type(text_container)
-        self._top_level_text_block_names = [get_type(text_block) for text_block in top_level_text_block_names]
-        self._text_block_names = text_block_names
+        if isinstance(floating_text_block_categories, (str, ObjectTypes)):
+            floating_text_block_categories = [floating_text_block_categories]
+        if floating_text_block_categories is None:
+            floating_text_block_categories = copy(IMAGE_DEFAULTS["floating_text_block_categories"])
+
+        self.text_container = get_type(text_container)
+        self.floating_text_block_categories = [get_type(text_block) for text_block in floating_text_block_categories]
+        self.include_residual_text_container = include_residual_text_container
         self._init_sanity_checks()
 
     def pass_datapoint(self, dp: Image) -> Page:
         """
         converts Image to Page
         :param dp: Image
         :return: Page
         """
-        return Page.from_image(
-            dp, self._text_container, self._top_level_text_block_names, self._text_block_names  # type: ignore
-        )
+        return Page.from_image(dp, self.text_container, self.floating_text_block_categories)
 
     def predict_dataflow(self, df: DataFlow) -> DataFlow:
         """
         Mapping a datapoint via `pass_datapoint` within a dataflow pipeline
 
         :param df: An input dataflow
         :return: A output dataflow
         """
         return MapData(df, self.pass_datapoint)
 
     def _init_sanity_checks(self) -> None:
-        assert self._text_container in [
+        assert self.text_container in (
             LayoutType.word,
             LayoutType.line,
-        ], f"text_container must be either {LayoutType.word} or {LayoutType.line}"
+        ), f"text_container must be either {LayoutType.word} or {LayoutType.line}"
 
     @staticmethod
     def get_meta_annotation() -> JsonDict:
         """
         meta annotation. We do not generate any new annotations here
         """
         return dict([("image_annotations", []), ("sub_categories", {}), ("relationships", {}), ("summaries", [])])
 
     def clone(self) -> "PageParsingService":
         """clone"""
         return self.__class__(
-            deepcopy(self._text_container), deepcopy(self._top_level_text_block_names), deepcopy(self._text_block_names)
+            deepcopy(self.text_container),
+            deepcopy(self.floating_text_block_categories),
+            self.include_residual_text_container,
         )
 
 
 @pipeline_component_registry.register("AnnotationNmsService")
 class AnnotationNmsService(PipelineComponent):
     """
     A service to pass `ImageAnnotation` to a non-maximum suppression (NMS) process for given pairs of categories.
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/concurrency.py` & `deepdoctection-0.25/deepdoctection/pipe/concurrency.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/pipe/doctectionpipe.py` & `deepdoctection-0.25/deepdoctection/pipe/doctectionpipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,32 +109,35 @@
     See `deepdoctection.analyzer.dd` for a concrete implementation.
 
     See also the explanations in `base.Pipeline`.
 
     By default, `DoctectionPipe` will instantiate a default `PageParsingService`
 
         PageParsingService(text_container=LayoutType.word,
-                           text_block_names=[LayoutType.title,
-                                             LayoutType.text,
-                                             LayoutType.list,
-                                             LayoutType.table])
+                           text_block_categories=[LayoutType.title,
+                                                  LayoutType.text,
+                                                  LayoutType.list,
+                                                  LayoutType.table])
 
     but you can overwrite the current setting:
 
     **Example:**
 
-            pipe = DoctectionPipe([comp_1, com_2])
-            pipe.page_parser =  PageParsingService(text_container= my_custom_setting)
+            pipe = DoctectionPipe([comp_1, com_2], PageParsingService(text_container= my_custom_setting))
     """
 
-    def __init__(self, pipeline_component_list: List[Union[PipelineComponent]]):
-        self.page_parser = PageParsingService(
-            text_container=LayoutType.word,
-            top_level_text_block_names=[LayoutType.title, LayoutType.text, LayoutType.list, LayoutType.table],
-        )
+    def __init__(
+        self,
+        pipeline_component_list: List[Union[PipelineComponent]],
+        page_parsing_service: Optional[PageParsingService] = None,
+    ):
+        if page_parsing_service is None:
+            self.page_parser = PageParsingService(text_container=LayoutType.word)
+        else:
+            self.page_parser = page_parsing_service
         assert all(
             isinstance(element, (PipelineComponent, PredictorPipelineComponent)) for element in pipeline_component_list
         )
         super().__init__(pipeline_component_list)
 
     def _entry(self, **kwargs: Union[str, DataFlow, bool, int, Pathlike, Union[str, List[str]]]) -> DataFlow:
         path, file_type, shuffle, max_datapoints, doc_path, dataset_dataflow = _collect_from_kwargs(**kwargs)
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/language.py` & `deepdoctection-0.25/deepdoctection/pipe/language.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 from copy import copy, deepcopy
 from typing import Optional, Sequence
 
 from ..datapoint.image import Image
 from ..datapoint.view import Page
 from ..extern.base import LanguageDetector, ObjectDetector
 from ..utils.detection_types import JsonDict
-from ..utils.logger import logger
-from ..utils.settings import LayoutType, PageType, TypeOrStr, get_type
+from ..utils.settings import PageType, TypeOrStr, get_type
 from .base import PipelineComponent
 from .registry import pipeline_component_registry
 
 
 @pipeline_component_registry.register("LanguageDetectionService")
 class LanguageDetectionService(PipelineComponent):
     """
@@ -55,73 +54,60 @@
     """
 
     def __init__(
         self,
         language_detector: LanguageDetector,
         text_container: Optional[TypeOrStr] = None,
         text_detector: Optional[ObjectDetector] = None,
-        text_block_names: Optional[Sequence[TypeOrStr]] = None,
+        floating_text_block_categories: Optional[Sequence[TypeOrStr]] = None,
     ):
         """
         :param language_detector: Detector to determine text
         :param text_container: text container, needed to generate the reading order. Not necessary when passing a
                                text detector.
         :param text_detector: Object detector to extract text. You cannot use a Pdfminer here.
 
-        :param text_block_names: text blocks, needed for generating the reading order. Not necessary
+        :param floating_text_block_categories: text blocks, needed for generating the reading order. Not necessary
                                  when passing a text detector.
         """
 
         self.predictor = language_detector
         self.text_detector = text_detector
         self.text_container = get_type(text_container) if text_container is not None else text_container
-        _text_block_names = []
-        if text_block_names:
-            _text_block_names = [get_type(text_block) for text_block in text_block_names]
-        self.text_block_names = _text_block_names
-        self._init_sanity_checks()
+        if floating_text_block_categories:
+            floating_text_block_categories = [get_type(text_block) for text_block in floating_text_block_categories]
+        self.floating_text_block_categories = floating_text_block_categories if floating_text_block_categories else []
         super().__init__(
             self._get_name(self.predictor.name)
         )  # cannot use PredictorPipelineComponent class because of return type of predict meth
 
     def serve(self, dp: Image) -> None:
         if self.text_detector is None:
-            page = Page.from_image(dp, self.text_container, self.text_block_names)
+            page = Page.from_image(dp, self.text_container, self.floating_text_block_categories)  # type: ignore
             text = page.text_no_line_break
         else:
             if dp.image is None:
                 raise ValueError("dp.image cannot be None")
             detect_result_list = self.text_detector.predict(dp.image)
             # this is a concatenation of all detection result. No reading order
             text = " ".join([result.text for result in detect_result_list if result.text is not None])
         predict_result = self.predictor.predict(text)
         self.dp_manager.set_summary_annotation(
             PageType.language, PageType.language, 1, predict_result.text, predict_result.score
         )
 
-    def _init_sanity_checks(self) -> None:
-        assert (
-            self.text_detector or self.text_container
-        ), "if no text_detector is provided a text container must be specified"
-        if not self.text_detector:
-            assert self.text_container in [LayoutType.word, LayoutType.line], (
-                f"text_container must be either {LayoutType.word} or " f"{LayoutType.line}"
-            )
-            if not self.text_block_names:
-                logger.info("text_block_names are set to None. This setting will return no reading order!")
-
     def clone(self) -> PipelineComponent:
         predictor = self.predictor.clone()
         if not isinstance(predictor, LanguageDetector):
             raise ValueError(f"Predictor must be of type LanguageDetector, but is of type {type(predictor)}")
         return self.__class__(
             predictor,
             copy(self.text_container),
             deepcopy(self.text_detector),
-            deepcopy(self.text_block_names),
+            deepcopy(self.floating_text_block_categories),
         )
 
     def get_meta_annotation(self) -> JsonDict:
         return dict(
             [
                 ("image_annotations", []),
                 ("sub_categories", {}),
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/layout.py` & `deepdoctection-0.25/deepdoctection/pipe/layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,29 +49,39 @@
 
     def __init__(
         self,
         layout_detector: ObjectDetector,
         to_image: bool = False,
         crop_image: bool = False,
         padder: Optional[PadTransform] = None,
+        skip_if_layout_extracted: bool = False,
     ):
         """
         :param layout_detector: object detector
         :param to_image: Generate an image for each detected block, e.g. populate `ImageAnnotation.image`. Useful,
                          if you want to process only some blocks in a subsequent pipeline component.
         :param crop_image: Do not only populate `ImageAnnotation.image` but also crop the detected block according
                            to its bounding box and populate the resulting sub image to
                            `ImageAnnotation.image.image`.
+        :param skip_if_layout_extracted: When `True` will check, if there are already `ImageAnnotation` of a category
+                                         available that will be predicted by the `layout_detector`. If yes, will skip
+                                         the prediction process.
         """
         self.to_image = to_image
         self.crop_image = crop_image
         self.padder = padder
+        self.skip_if_layout_extracted = skip_if_layout_extracted
         super().__init__(self._get_name(layout_detector.name), layout_detector)
 
     def serve(self, dp: Image) -> None:
+        if self.skip_if_layout_extracted:
+            categories = self.predictor.possible_categories()  # type: ignore
+            anns = dp.get_annotation(category_names=categories)
+            if anns:
+                return
         if dp.image is None:
             raise ValueError("image cannot be None")
         np_image = dp.image
         if self.padder:
             np_image = self.padder.apply_image(np_image)
         detect_result_list = self.predictor.predict(np_image)  # type: ignore
         if self.padder and detect_result_list:
@@ -101,8 +111,8 @@
     def clone(self) -> "PredictorPipelineComponent":
         predictor = self.predictor.clone()
         padder_clone = None
         if self.padder:
             padder_clone = self.padder.clone()
         if not isinstance(predictor, ObjectDetector):
             raise ValueError(f"predictor must be of type ObjectDetector, but is of type {type(predictor)}")
-        return self.__class__(predictor, self.to_image, self.crop_image, padder_clone)
+        return self.__class__(predictor, self.to_image, self.crop_image, padder_clone, self.skip_if_layout_extracted)
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/lm.py` & `deepdoctection-0.25/deepdoctection/pipe/lm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/pipe/refine.py` & `deepdoctection-0.25/deepdoctection/pipe/refine.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,16 +394,22 @@
 
             for dp in df:
                 ...
 
     """
 
     def __init__(self) -> None:
-        self._table_name = LayoutType.table
-        self._cell_names = [CellType.header, CellType.body, LayoutType.cell]
+        self._table_name = [LayoutType.table, LayoutType.table_rotated]
+        self._cell_names = [
+            LayoutType.cell,
+            CellType.column_header,
+            CellType.projected_row_header,
+            CellType.spanning,
+            CellType.row_header,
+        ]
         super().__init__("table_segment_refine")
 
     def serve(self, dp: Image) -> None:
         tables = dp.get_annotation(category_names=self._table_name)
         for table in tables:
             if table.image is None:
                 raise ValueError("table.image cannot be None")
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/registry.py` & `deepdoctection-0.25/deepdoctection/pipe/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/pipe/segment.py` & `deepdoctection-0.25/deepdoctection/pipe/segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     dp: Image, items: List[ImageAnnotation], table: ImageAnnotation, item_name: str
 ) -> None:
     if table.image is None:
         raise ValueError("table.image cannot be None")
     table_embedding_box = table.image.get_embedding(dp.image_id)
 
     tmp_item_xy = table_embedding_box.uly + 1.0 if item_name == LayoutType.row else table_embedding_box.ulx + 1.0
+    tmp_item_table_xy = 1.0
     for idx, item in enumerate(items):
         with MappingContextManager(
             dp_name=dp.file_name,
             filter_level="bounding box",
             image_annotation={"category_name": item.category_name, "annotation_id": item.annotation_id},
         ):
             if item.image is None:
@@ -231,23 +232,47 @@
                 lrx=item_embedding_box.lrx if item_name == LayoutType.row else tmp_next_item_xy,
                 lry=tmp_next_item_xy if item_name == LayoutType.row else item_embedding_box.lry,
                 absolute_coords=True,
             )
             item.image.set_embedding(dp.image_id, new_embedding_box)
             tmp_item_xy = tmp_next_item_xy
 
+            item_table_embedding_box = item.image.get_embedding(table.annotation_id)
+            if idx != len(items) - 1:
+                next_item_table_embedding_box = items[idx + 1].image.get_embedding(table.annotation_id)  # type: ignore
+                tmp_table_next_item_xy = (
+                    (item_table_embedding_box.lry + next_item_table_embedding_box.uly) / 2
+                    if item_name == LayoutType.row
+                    else (item_table_embedding_box.lrx + next_item_table_embedding_box.ulx) / 2
+                )
+            else:
+                tmp_table_next_item_xy = (
+                    table.image.height - 1.0 if item_name == LayoutType.row else table.image.width - 1.0
+                )
+
+            new_table_embedding_box = BoundingBox(
+                ulx=item_table_embedding_box.ulx if item_name == LayoutType.row else tmp_item_table_xy,
+                uly=tmp_item_table_xy if item_name == LayoutType.row else item_table_embedding_box.uly,
+                lrx=item_table_embedding_box.lrx if item_name == LayoutType.row else tmp_table_next_item_xy,
+                lry=tmp_table_next_item_xy if item_name == LayoutType.row else item_table_embedding_box.lry,
+                absolute_coords=True,
+            )
+            item.image.set_embedding(table.annotation_id, new_table_embedding_box)
+            tmp_item_table_xy = tmp_table_next_item_xy
+
 
 def _tile_by_stretching_rows_leftwise_column_downwise(
     dp: Image, items: List[ImageAnnotation], table: ImageAnnotation, item_name: str
 ) -> None:
     if table.image is None:
         raise ValueError("table.image cannot be None")
     table_embedding_box = table.image.get_embedding(dp.image_id)
 
     tmp_item_xy = table_embedding_box.uly + 1.0 if item_name == LayoutType.row else table_embedding_box.ulx + 1.0
+    tmp_item_table_xy = 1.0
     for item in items:
         with MappingContextManager(
             dp_name=dp.file_name,
             filter_level="bounding box",
             image_annotation={"category_name": item.category_name, "annotation_id": item.annotation_id},
         ):
             if item.image is None:
@@ -256,26 +281,45 @@
             new_embedding_box = BoundingBox(
                 ulx=item_embedding_box.ulx if item_name == LayoutType.row else tmp_item_xy,
                 uly=tmp_item_xy if item_name == LayoutType.row else item_embedding_box.uly,
                 lrx=item_embedding_box.lrx,
                 lry=item_embedding_box.lry,
                 absolute_coords=True,
             )
+            item_table_embedding_box = item.image.get_embedding(table.annotation_id)
+            new_table_embedding_box = BoundingBox(
+                ulx=item_table_embedding_box.ulx if item_name == LayoutType.row else tmp_item_table_xy,
+                uly=tmp_item_table_xy if item_name == LayoutType.row else item_table_embedding_box.uly,
+                lrx=item_table_embedding_box.lrx,
+                lry=item_table_embedding_box.lry,
+                absolute_coords=True,
+            )
 
             if item == items[-1]:
                 new_embedding_box = BoundingBox(
                     ulx=item_embedding_box.ulx if item_name == LayoutType.row else tmp_item_xy,
                     uly=tmp_item_xy if item_name == LayoutType.row else item_embedding_box.uly,
                     lrx=item_embedding_box.lrx if item_name == LayoutType.row else table_embedding_box.lrx - 1.0,
                     lry=table_embedding_box.lry - 1.0 if item_name == LayoutType.row else item_embedding_box.lry,
                     absolute_coords=True,
                 )
+                new_table_embedding_box = BoundingBox(
+                    ulx=item_table_embedding_box.ulx if item_name == LayoutType.row else tmp_item_table_xy,
+                    uly=tmp_item_table_xy if item_name == LayoutType.row else item_table_embedding_box.uly,
+                    lrx=item_table_embedding_box.lrx if item_name == LayoutType.row else table.image.width - 1.0,
+                    lry=table.image.height - 1.0 if item_name == LayoutType.row else item_table_embedding_box.lry,
+                    absolute_coords=True,
+                )
 
             tmp_item_xy = item_embedding_box.lry if item_name == LayoutType.row else item_embedding_box.lrx
+            tmp_item_table_xy = (
+                item_table_embedding_box.lry if item_name == LayoutType.row else item_table_embedding_box.lrx
+            )
             item.image.set_embedding(dp.image_id, new_embedding_box)
+            item.image.set_embedding(table.annotation_id, new_table_embedding_box)
 
 
 def tile_tables_with_items_per_table(
     dp: Image, table: ImageAnnotation, item_name: str, stretch_rule: Literal["left", "equal"] = "left"
 ) -> Image:
     """
     Tiling a table with items (i.e. rows or columns). To ensure that every position in a table can be assigned to a row
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/text.py` & `deepdoctection-0.25/deepdoctection/pipe/order.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,379 +1,422 @@
 # -*- coding: utf-8 -*-
-# File: text.py
+# File: order.py
 
-# Copyright 2021 Dr. Janis Meyer. All rights reserved.
+# Copyright 2023 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Module for text extraction pipeline component
+Module for ordering text and layout segments pipeline components
 """
-from copy import copy, deepcopy
+
+from copy import copy
 from itertools import chain
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
+import numpy as np
+
 from ..datapoint.annotation import ImageAnnotation
+from ..datapoint.box import BoundingBox, merge_boxes
 from ..datapoint.image import Image
-from ..extern.base import ObjectDetector, PdfMiner, TextRecognizer
-from ..extern.tessocr import TesseractOcrDetector
-from ..utils.detection_types import ImageType, JsonDict
-from ..utils.logger import logger
-from ..utils.settings import LayoutType, PageType, Relationships, TypeOrStr, WordType, get_type
-from .base import PipelineComponent, PredictorPipelineComponent
-from .registry import pipeline_component_registry
-
-__all__ = ["TextExtractionService", "TextOrderService"]
+from ..datapoint.view import IMAGE_DEFAULTS
+from ..extern.base import DetectionResult
+from ..extern.tp.tpfrcnn.utils.np_box_ops import ioa as np_ioa
+from ..pipe.base import PipelineComponent
+from ..pipe.registry import pipeline_component_registry
+from ..utils.detection_types import JsonDict
+from ..utils.settings import LayoutType, ObjectTypes, Relationships, TypeOrStr, get_type
 
 
-@pipeline_component_registry.register("TextExtractionService")
-class TextExtractionService(PredictorPipelineComponent):
+class OrderGenerator:
+    """
+    Class for implementing text ordering logic and tasks that have preparational character. This includes logic for
+    grouping word type `ImageAnnotation` into text lines, splitting text lines into sub-lines (by detecting gaps
+    between words) as well as ordering text blocks (e.g. titles, tables, etc.).
     """
-    Pipeline component for extracting text. Any detector can be selected, provided that it can evaluate a
-    numpy array as an image.
-
-    Text extraction can either be carried out over the entire image or over selected regions of interests (ROIs).
-    ROIs are layout components that have been determined by means of a pipeline component that has been run through
-    beforehand. ROI extraction is particularly suitable when an OCR component is selected as the detector and the
-    document has a complex structure. Instead of transferring the entire image, only the ROIs are transferred to
-    the detector. Since the ROI has a simpler structure than the entire document page, it can significantly improve
-    the OCR results.
-
-    Text components (currently only words) are attached to the image as image annotations. A relation is assigned in
-    relation to text and ROI or in relation to text and the entire image. When selecting ROIs, only the selected
-    categories are taken into account during processing. ROIs that are not selected are not presented to the
-    detector.
 
-        textract_predictor = TextractOcrDetector()
-        text_extract = TextExtractionService(textract_predictor)
+    def __init__(self, starting_point_tolerance: float, broken_line_tolerance: float, height_tolerance: float):
+        """
+        Parameters for steering grouping and ordering on word level as well as on text block level.
 
-        pipe = DoctectionPipe([text_extract])
-        df = pipe.analyze(path="path/to/document.pdf")
+        :param starting_point_tolerance: Threshold to identify if two text blocks belong to one column: To check if two
+                                         text blocks belong to the same column, one condition says, that
+                                         x-coordinates of vertices should not differ more than this threshold
+        :param broken_line_tolerance: Threshold to identify if two consecutive words belonging to one line should be
+                                      in two different sub lines (because they belong to two different text columns).
+        :param height_tolerance: Threshold to identify if two columns lying over each other belong together or need to
+                                 be separated. Scaling factor of relative text block height.
+        """
+        self.starting_point_tolerance = starting_point_tolerance
+        self.broken_line_tolerance = broken_line_tolerance
+        self.height_tolerance = height_tolerance
+        self.ioa_column_threshold = 0.9
 
-        for dp in df:
-            ...
-    """
+    @staticmethod
+    def group_words_into_lines(
+        word_anns: Sequence[ImageAnnotation], image_id: Optional[str] = None
+    ) -> List[Tuple[int, int, str]]:
+        """Arranging words into horizontal text lines and sorting text lines vertically in order to give
+        an enumeration of words that is used for establishing the reading order. Using this reading order arragement
+        makes only sense for words within a rectangle and needs to be revised in more complex appearances.
+        Function returns triplets for every word ann `(word reading order position, text line position, word annotation
+        id)`.
+        """
+        reading_lines = []
+        rows: List[Dict[str, float]] = []
+        for word in word_anns:
+            if word.image is not None and image_id is not None:
+                bounding_box = word.image.get_embedding(image_id)
+            else:
+                bounding_box = word.bounding_box
+            row_found = False
+            for idx, row in enumerate(rows):
+                row_cy = (row["upper"] + row["lower"]) / 2
+                # word belongs to row if center lies within the upper and lower bounds of the row or if the center y
+                # coordinate lies within the upper and lower bounds of the word bounding boxes.
+                # If word belongs to bound we do not update any row bounds. Thus, row bound are determined by the
+                # first word that defines the row
+                if (row["upper"] < bounding_box.cy < row["lower"]) or (bounding_box.uly < row_cy < bounding_box.lry):
+                    reading_lines.append((idx, word.annotation_id, bounding_box.cx))
+                    row_found = True
+                    break
+
+            # condition above not satisfied for any row, thus word defines a new row
+            if not row_found:
+                rows.append({"upper": bounding_box.uly, "lower": bounding_box.lry})
+                reading_lines.append((len(rows) - 1, word.annotation_id, bounding_box.cx))
+
+        rows_dict = {k: rows[k] for k in range(len(rows))}
+        rows_dict = {
+            idx: key[0]  # type:ignore
+            for idx, key in enumerate(sorted(rows_dict.items(), key=lambda it: it[1]["upper"]))
+        }
+        reading_lines.sort(key=lambda x: (rows_dict[x[0]], x[2]))
+        number_rows = len(rows_dict)
+        return [(idx + 1, number_rows - word[0], word[1]) for idx, word in enumerate(reading_lines)]
 
-    def __init__(
-        self,
-        text_extract_detector: Union[ObjectDetector, PdfMiner, TextRecognizer],
-        extract_from_roi: Optional[Union[Sequence[TypeOrStr], TypeOrStr]] = None,
-        run_time_ocr_language_selection: bool = False,
-        skip_if_text_extracted: bool = False,
-    ):
+    @staticmethod
+    def group_lines_into_lines(
+        line_anns: Sequence[ImageAnnotation], image_id: Optional[str] = None
+    ) -> List[Tuple[int, int, str]]:
         """
-        :param text_extract_detector: ObjectDetector
-        :param extract_from_roi: one or more category names for roi selection
-        :param run_time_ocr_language_selection: Only available for `TesseractOcrDetector` as this framework has
-                                                multiple language selections. Also requires that a language detection
-                                                pipeline component ran before. It will select the expert language OCR
-                                                model based on the determined language.
-        :param skip_if_text_extracted: Set to `True` if text has already been extracted in a previous pipeline component
-                                       and should not be extracted again. Use-case: A PDF with some scanned images.
-        """
-
-        if extract_from_roi is None:
-            extract_from_roi = []
-        self.extract_from_category = (
-            [get_type(extract_from_roi)]
-            if isinstance(extract_from_roi, str)
-            else [get_type(roi_category) for roi_category in extract_from_roi]
-        )
-        super().__init__(self._get_name(text_extract_detector.name), text_extract_detector)
-        if self.extract_from_category:
-            if not isinstance(self.predictor, (ObjectDetector, TextRecognizer)):
-                raise TypeError("Predicting from a cropped image requires to pass an ObjectDetector or TextRecognizer.")
-        if run_time_ocr_language_selection:
-            assert isinstance(self.predictor, TesseractOcrDetector), (
-                "Only TesseractOcrDetector supports multiple " "languages"
-            )
+        Sorting reading lines. Returns for a list of `ImageAnnotation` an list of tuples (each tuple containing the
+        reading order and the `annotation_id` for each list element.
+        :param line_anns: text line `ImageAnnotation`
+        :param image_id: image_id of underyling image (to find get the bounding boxes)
+        :return: `List[(reading_order, reading_order,annotation_id)]`
+        """
+        reading_lines = []
+        for ann in line_anns:
+            if ann.image is not None and image_id is not None:
+                bounding_box = ann.image.get_embedding(image_id)
+            else:
+                bounding_box = ann.bounding_box
+            reading_lines.append((bounding_box.cy, ann.annotation_id))
+        reading_lines.sort(key=lambda x: x[0])
+        return [(idx + 1, idx + 1, line[1]) for idx, line in enumerate(reading_lines)]
 
-        self.run_time_ocr_language_selection = run_time_ocr_language_selection
-        self.skip_if_text_extracted = skip_if_text_extracted
-        if self.skip_if_text_extracted and isinstance(self.predictor, TextRecognizer):
-            raise ValueError(
-                "skip_if_text_extracted=True and TextRecognizer in TextExtractionService is not " "compatible"
+    @staticmethod
+    def _connected_components(columns: List[BoundingBox]) -> List[Dict[str, Any]]:
+        # building connected components of columns
+        connected_components: List[Dict[str, Any]] = []
+        for idx, col in enumerate(columns):
+            col_dict = {"id": idx, "box": col}
+            component_found = False
+            for comp in connected_components:
+                if (
+                    comp["top"] < col.uly < comp["bottom"]
+                    or comp["top"] < col.lry < comp["bottom"]
+                    or col.uly < comp["top"] < col.lry
+                    or col.uly < comp["bottom"] < col.lry
+                ):
+                    comp["top"] = min(comp["top"], col.uly)
+                    comp["bottom"] = max(comp["bottom"], col.lry)
+                    comp["left"] = col.ulx
+                    comp["column"].append(col_dict)
+                    component_found = True
+                    break
+            if not component_found:
+                connected_components.append({"top": col.uly, "bottom": col.lry, "left": col.ulx, "column": [col_dict]})
+
+            # next, sorting columns in connected components by increasing x-value. In order to be tolerant to
+            # nearby values we are rounding values we want to sort
+            for comp in connected_components:
+                for column in comp["column"]:
+                    column["box"].ulx = round(column["box"].ulx, 2)
+                    column["box"].uly = round(column["box"].uly, 2)
+                comp["column"].sort(key=lambda x: (x["box"].ulx, x["box"].uly))
+
+            # finally, sorting connected components by increasing y-value
+            connected_components.sort(key=lambda x: x["top"])
+
+        return connected_components
+
+    def order_blocks(
+        self, anns: List[ImageAnnotation], image_width: float, image_height: float, image_id: Optional[str] = None
+    ) -> Sequence[Tuple[int, str]]:
+        """
+        Determining a text ordering of text blocks. These text blocks should be larger sections than barely words.
+        It will first try to detect columns, then try to consolidate columns and finally try to detecting connected
+        components of columns. A connected component of columns is a group of columns that lie next to each other.
+        Having to connected components lying over each other will infer a reading order where the upper block of
+        connected component will be read first followed by text blocks of columns of the second.
+
+        :param anns: list of `ImageAnnotation` with all list element to sort.
+        :param image_width: image width (to re-calculate bounding boxes into relative coords)
+        :param image_height: image height (to re-calculate bounding boxes into relative coords)
+        :param image_id: image id
+        :return: List of tuples with reading order position and `annotation_id`
+        """
+        if not anns:
+            return []
+        reading_blocks = []
+        columns: List[BoundingBox] = []
+        anns.sort(
+            key=lambda x: (
+                x.bounding_box.transform(image_width, image_height).cy,  # type: ignore
+                x.bounding_box.transform(image_width, image_height).cx,  # type: ignore
             )
+        )
+        for ann in anns:
+            if ann.image is not None and image_id is not None:
+                bounding_box = ann.image.get_embedding(image_id)
+            else:
+                bounding_box = ann.bounding_box
 
-    def serve(self, dp: Image) -> None:
-        maybe_batched_text_rois = self.get_text_rois(dp)
-        for text_roi in maybe_batched_text_rois:
-            ann_id = None
-            if isinstance(text_roi, ImageAnnotation):
-                ann_id = text_roi.annotation_id
-            predictor_input = self.get_predictor_input(text_roi)
-            if predictor_input is None:
-                raise ValueError("predictor_input cannot be None")
-            if predictor_input in [b""]:
-                pass
+            if bounding_box.absolute_coords:
+                rel_coords_box = bounding_box.transform(image_width, image_height)
             else:
-                width, height = None, None
-                if self.run_time_ocr_language_selection:
-                    self.predictor.set_language(dp.summary.get_sub_category(PageType.language).value)  # type: ignore
-                detect_result_list = self.predictor.predict(predictor_input)  # type: ignore
-                if isinstance(self.predictor, PdfMiner):
-                    width, height = self.predictor.get_width_height(predictor_input)  # type: ignore
-
-                for detect_result in detect_result_list:
-                    if isinstance(self.predictor, TextRecognizer):
-                        detect_ann_id = detect_result.uuid
-                    else:
-                        detect_ann_id = self.dp_manager.set_image_annotation(
-                            detect_result, ann_id, True, detect_result_max_width=width, detect_result_max_height=height
-                        )
-                    if detect_ann_id is not None:
-                        self.dp_manager.set_container_annotation(
-                            WordType.characters,
-                            None,
-                            WordType.characters,
-                            detect_ann_id,
-                            detect_result.text if detect_result.text is not None else "",
-                            detect_result.score,
-                        )
-                        if detect_result.block:
-                            self.dp_manager.set_category_annotation(
-                                WordType.block, detect_result.block, WordType.block, detect_ann_id
-                            )
-                        if detect_result.line:
-                            self.dp_manager.set_category_annotation(
-                                WordType.text_line, detect_result.line, WordType.text_line, detect_ann_id
-                            )
-
-    def get_text_rois(self, dp: Image) -> Sequence[Union[Image, ImageAnnotation, List[ImageAnnotation]]]:
-        """
-        Return image rois based on selected categories. As this selection makes only sense for specific text extractors
-        (e.g. those who do proper OCR and do not mine from text from native pdfs) it will do some sanity checks.
-        It is possible that a preceding text extractor dumped text before. If the predictor must not extract text as
-        well `get_text_rois` will return an empty list.
-        :return: list of ImageAnnotation or Image
-        """
-        if self.skip_if_text_extracted:
-            text_categories = self.predictor.possible_categories()  # type: ignore
-            text_anns = dp.get_annotation(category_names=text_categories)
-            if text_anns:
-                return []
-
-        if self.extract_from_category:
-            if self.predictor.accepts_batch:
-                return [dp.get_annotation(category_names=self.extract_from_category)]
-            return dp.get_annotation(category_names=self.extract_from_category)
-        return [dp]
-
-    def get_predictor_input(
-        self, text_roi: Union[Image, ImageAnnotation, List[ImageAnnotation]]
-    ) -> Optional[Union[bytes, ImageType, List[Tuple[str, ImageType]]]]:
-        """
-        Return raw input for a given `text_roi`. This can be a numpy array or pdf bytes and depends on the chosen
-        predictor.
-
-        :param text_roi: `Image` or `ImageAnnotation`
-        :return: pdf bytes or numpy array
-        """
-
-        if isinstance(text_roi, ImageAnnotation):
-            if text_roi.image is None:
-                raise ValueError("text_roi.image cannot be None")
-            if text_roi.image.image is None:
-                raise ValueError("text_roi.image.image cannot be None")
-            return text_roi.image.image
-        if isinstance(self.predictor, ObjectDetector):
-            if not isinstance(text_roi, Image):
-                raise ValueError("text_roi must be an image")
-            return text_roi.image
-        if isinstance(text_roi, list):
-            assert all(roi.image is not None for roi in text_roi)
-            assert all(roi.image.image is not None for roi in text_roi)  # type: ignore
-            return [(roi.annotation_id, roi.image.image) for roi in text_roi]  # type: ignore
-        if isinstance(self.predictor, PdfMiner) and text_roi.pdf_bytes is not None:
-            return text_roi.pdf_bytes
-        return b""
+                rel_coords_box = bounding_box
 
-    def get_meta_annotation(self) -> JsonDict:
-        if self.extract_from_category:
-            sub_cat_dict = {category: {WordType.characters} for category in self.extract_from_category}
-        else:
-            if not isinstance(self.predictor, (ObjectDetector, PdfMiner)):
-                raise TypeError(
-                    f"self.predictor must be of type ObjectDetector or PdfMiner but is of type "
-                    f"{type(self.predictor)}"
+            column_found = False
+            for idx, col in enumerate(columns):
+                # if the x-coordinate left and right is within starting_point_tolerance (first_condition and
+                # second_condition) or if x-coordinate left and right is within the left or right border of the column
+                # then the annotation will belong to this column and column left/right will be re-adjusted
+                first_condition = all(
+                    (
+                        col.ulx - self.starting_point_tolerance < rel_coords_box.ulx,
+                        rel_coords_box.lrx < col.lrx + self.starting_point_tolerance,
+                    )
                 )
-            sub_cat_dict = {category: {WordType.characters} for category in self.predictor.possible_categories()}
-        return dict(
-            [
-                (
-                    "image_annotations",
-                    self.predictor.possible_categories()
-                    if isinstance(self.predictor, (ObjectDetector, PdfMiner))
-                    else [],
-                ),
-                ("sub_categories", sub_cat_dict),
-                ("relationships", {}),
-                ("summaries", []),
-            ]
-        )
+                second_condition = all(
+                    (
+                        rel_coords_box.ulx - self.starting_point_tolerance < col.ulx,
+                        col.lrx < rel_coords_box.lrx + self.starting_point_tolerance,
+                    )
+                )
+                # broken line condition
+                third_condition = abs(rel_coords_box.ulx - col.lrx) < self.broken_line_tolerance
+                fourth_condition = abs(rel_coords_box.uly - col.lry) < self.height_tolerance * rel_coords_box.height
+                fifth_condition = abs(rel_coords_box.lry - col.uly) < self.height_tolerance * rel_coords_box.height
+
+                if (first_condition and (fourth_condition or fifth_condition)) or (  # pylint: disable=R0916
+                    second_condition
+                    and (fourth_condition or fifth_condition)
+                    or (third_condition and (fourth_condition or fifth_condition))
+                ):
+                    reading_blocks.append((idx, ann.annotation_id))
+                    # update the top and right with the new line added.
+                    col.ulx = min(rel_coords_box.ulx, col.ulx)
+                    col.uly = min(rel_coords_box.uly, col.uly)
+                    col.lrx = max(rel_coords_box.lrx, col.lrx)
+                    col.lry = max(rel_coords_box.lry, col.lry)
+                    column_found = True
+                    break
+
+            if not column_found:
+                columns.append(
+                    BoundingBox(
+                        absolute_coords=False,
+                        ulx=rel_coords_box.ulx,
+                        uly=rel_coords_box.uly,
+                        lrx=rel_coords_box.lrx,
+                        lry=rel_coords_box.lry,
+                    )
+                )
+                # update the top and right with the new reading block added.
+                reading_blocks.append((len(columns) - 1, ann.annotation_id))
+
+        consoldiated_cols = self._consolidate_columns(columns)
+        consolidated_columns = []
+        for idx, _ in enumerate(columns):
+            if columns[consoldiated_cols[idx]] not in consolidated_columns:
+                consolidated_columns.append(columns[consoldiated_cols[idx]])
+
+        reading_blocks = [(consoldiated_cols.get(x[0], x[0]), x[1]) for x in reading_blocks]
+
+        connected_components = self._connected_components(consolidated_columns)
+        columns_box = list(chain(*[comp["column"] for comp in connected_components]))
+
+        # old to new mapping
+        columns_dict = {col["id"]: k for k, col in enumerate(columns_box)}
+        blocks = [(columns_dict.get(x[0], consoldiated_cols.get(x[0])), x[1]) for x in reading_blocks]
+        blocks.sort(key=lambda x: x[0])  # type: ignore
+        sorted_blocks = []
+        max_block_number = max(list(columns_dict.values()))
+        filtered_blocks: Sequence[Tuple[int, str]]
+        for idx in range(max_block_number + 1):
+            filtered_blocks = list(filter(lambda x: x[0] == idx, blocks))  # type: ignore # pylint: disable=W0640
+            sorted_blocks.extend(self._sort_anns_grouped_by_blocks(filtered_blocks, anns, image_width, image_height))
+        reading_blocks = [(idx + 1, block[1]) for idx, block in enumerate(sorted_blocks)]
+        return reading_blocks
+
+    def _consolidate_columns(self, columns: List[BoundingBox]) -> Dict[int, int]:
+        if not columns:
+            return {}
+        np_boxes = np.array([col.to_list(mode="xyxy") for col in columns])
+        ioa_matrix = np.transpose(np_ioa(np_boxes, np_boxes))
+        np.fill_diagonal(ioa_matrix, 0)
+        output = ioa_matrix > self.ioa_column_threshold
+        child_index, parent_index = output.nonzero()
+        column_dict = dict(zip(child_index, parent_index))
+        counter = 0
+        for idx, _ in enumerate(columns):
+            if idx not in column_dict:
+                column_dict[idx] = counter
+                counter += 1
+        return column_dict
 
     @staticmethod
-    def _get_name(text_detector_name: str) -> str:
-        return f"text_extract_{text_detector_name}"
+    def _sort_anns_grouped_by_blocks(
+        block: Sequence[Tuple[int, str]], anns: Sequence[ImageAnnotation], image_width: float, image_height: float
+    ) -> List[Tuple[int, str]]:
+        if not block:
+            return []
+        anns_and_blocks_numbers = list(zip(*block))
+        ann_ids = anns_and_blocks_numbers[1]
+        block_number = anns_and_blocks_numbers[0][0]
+        block_anns = [ann for ann in anns if ann.annotation_id in ann_ids]
+        block_anns.sort(
+            key=lambda x: (
+                round(x.bounding_box.transform(image_width, image_height).uly, 2),  # type: ignore
+                round(x.bounding_box.transform(image_width, image_height).ulx, 2),  # type: ignore
+            )
+        )
+        return [(block_number, ann.annotation_id) for ann in block_anns]
 
-    def clone(self) -> "PredictorPipelineComponent":
-        predictor = self.predictor.clone()
-        if not isinstance(predictor, (ObjectDetector, PdfMiner, TextRecognizer)):
-            raise ValueError(f"predictor must be of type ObjectDetector or PdfMiner, but is of type {type(predictor)}")
-        return self.__class__(predictor, deepcopy(self.extract_from_category), self.run_time_ocr_language_selection)
-
-
-def _reading_lines(image_id: str, word_anns: List[ImageAnnotation]) -> List[Tuple[int, str]]:
-    reading_lines = []
-    rows: List[Dict[str, float]] = []
-    for word in word_anns:
-        if word.image is not None:
-            bounding_box = word.image.get_embedding(image_id)
-        else:
-            bounding_box = word.bounding_box
-        row_found = False
-        for idx, row in enumerate(rows):
-            row_cy = (row["upper"] + row["lower"]) / 2
-
-            if (row["upper"] < bounding_box.cy < row["lower"]) or (bounding_box.uly < row_cy < bounding_box.lry):
-                reading_lines.append((idx, word.annotation_id, bounding_box.cx))
-                row_found = True
-                break
-
-        if not row_found:
-            rows.append({"upper": bounding_box.uly, "lower": bounding_box.lry})
-            reading_lines.append((len(rows) - 1, word.annotation_id, bounding_box.cx))
-
-    rows_dict = {k: rows[k] for k in range(len(rows))}
-    rows_dict = {
-        idx: key[0] for idx, key in enumerate(sorted(rows_dict.items(), key=lambda it: it[1]["upper"]))  # type:ignore
-    }
-    reading_lines.sort(key=lambda x: (rows_dict[x[0]], x[2]))
-    return [(idx + 1, word[1]) for idx, word in enumerate(reading_lines)]
-
-
-def _reading_columns(
-    dp: Image,
-    anns: List[ImageAnnotation],
-    starting_point_tolerance: float,
-    height_tolerance: float,
-    ignore_category_when_building_column_blocks: List[LayoutType],
-) -> List[Tuple[int, str]]:
-    reading_blocks = []
-    columns: List[Dict[str, float]] = []
-    anns.sort(key=lambda x: (x.bounding_box.cy, x.bounding_box.cx))  # type: ignore
-    for ann in anns:
-        if ann.image is not None:
-            bounding_box = ann.image.get_embedding(dp.image_id)
-        else:
-            bounding_box = ann.bounding_box
 
-        if bounding_box.absolute_coords:
-            rel_coords_box = bounding_box.transform(dp.width, dp.height)
-        else:
-            rel_coords_box = bounding_box
+class TextLineGenerator:
+    """
+    Class for generating synthetic text lines from words. Possible to break text lines into sub lines by using
+    a paragraph break threshold. This allows to detect a multi column structure just by observing sub lines.
+    """
 
-        column_found = False
-        for idx, col in enumerate(columns):
-            # if the x-coordinate left and right is within starting_point_tolerance (first_condition and
-            # second_condition) or if x-coordinate left and right is within the left or right border of the column
-            # then the annotation will belong to this column and column left/right will be re-adjusted
-
-            first_condition = all(
-                (
-                    col["left"] - starting_point_tolerance < rel_coords_box.ulx,
-                    rel_coords_box.lrx < col["right"] + starting_point_tolerance,
-                )
-            )
-            second_condition = all(
-                (
-                    rel_coords_box.ulx - starting_point_tolerance < col["left"],
-                    col["right"] < rel_coords_box.lrx + starting_point_tolerance,
-                )
-            )
+    def __init__(
+        self, make_sub_lines: bool, line_category_id: Union[int, str], paragraph_break: Optional[float] = None
+    ):
+        """
+        :param make_sub_lines: Whether to build sub lines from lines
+        :param line_category_id: category_id to give a text line
+        :param paragraph_break: threshold of two consecutive words. If distance is larger than threshold, two sublines
+                                will be built
+        """
+        if make_sub_lines and paragraph_break is None:
+            raise ValueError("You must specify paragraph_break when setting make_sub_lines to True")
+        self.line_category_id = int(line_category_id)
+        self.make_sub_lines = make_sub_lines
+        self.paragraph_break = paragraph_break
+
+    def _make_detect_result(self, box: BoundingBox, relationships: Dict[str, List[str]]) -> DetectionResult:
+        return DetectionResult(
+            box=box.to_list(mode="xyxy"),
+            class_name=LayoutType.line,
+            class_id=self.line_category_id,
+            absolute_coords=box.absolute_coords,
+            relationships=relationships,
+        )
 
-            third_condition = abs(rel_coords_box.uly - col["bottom"]) < height_tolerance * rel_coords_box.height
-            fourth_condition = abs(rel_coords_box.lry - col["top"]) < height_tolerance * rel_coords_box.height
+    def create_detection_result(
+        self,
+        word_anns: Sequence[ImageAnnotation],
+        image_width: float,
+        image_height: float,
+        image_id: Optional[str] = None,
+    ) -> Sequence[DetectionResult]:
+        """
+        Creating detecting result of lines (or sub lines) from given word type `ImageAnnotation`.
 
-            if (first_condition and (third_condition or fourth_condition)) or (  # pylint: disable=R0916
-                second_condition and (third_condition or fourth_condition)
-            ):
-                reading_blocks.append((idx, ann.annotation_id))
-                # update the top and right with the new line added.
-                if ann.category_name not in ignore_category_when_building_column_blocks:
-                    col["left"] = min(rel_coords_box.ulx, col["left"])
-                    col["top"] = min(rel_coords_box.uly, col["top"])
-                    col["right"] = max(rel_coords_box.lrx, col["right"])
-                    col["bottom"] = max(rel_coords_box.lry, col["bottom"])
-                column_found = True
-                break
-
-        if not column_found:
-            columns.append(
-                {
-                    "left": rel_coords_box.ulx,
-                    "right": rel_coords_box.lrx,
-                    "top": rel_coords_box.uly,
-                    "bottom": rel_coords_box.lry,
-                }
-            )
-            # update the top and right with the new reading block added.
-            reading_blocks.append((len(columns) - 1, ann.annotation_id))
+        :param word_anns: list og given word type `ImageAnnotation`
+        :param image_width: image width
+        :param image_height: image height
+        :param image_id: image id
+        :return:
+        """
+        if not word_anns:
+            return []
+        # every list now non-empty
+        word_anns_dict = {ann.annotation_id: ann for ann in word_anns}
+        word_order_list = OrderGenerator.group_words_into_lines(word_anns, image_id)
+        number_rows = max([word[1] for word in word_order_list])
+        detection_result_list = []
+        for row in range(1, number_rows + 1):
+            ann_meta_per_row = [ann_meta for ann_meta in word_order_list if ann_meta[1] == row]
+            ann_ids = [ann_meta[2] for ann_meta in ann_meta_per_row]
+            anns_per_row = [word_anns_dict[ann_id] for ann_id in ann_ids]
+            anns_per_row.sort(key=lambda x: x.image.get_embedding(image_id).ulx)  # type: ignore
+
+            if len(anns_per_row) >= 2 or not self.make_sub_lines:
+                # words are already sorted horizontally
+                sub_line = [anns_per_row[0]]
+                sub_line_ann_ids = [anns_per_row[0].annotation_id]
+                for idx, ann in enumerate(anns_per_row[1:]):
+                    horiz_break = True
+                    if image_id is not None:
+                        prev_box = sub_line[-1].image.get_embedding(image_id)  # type: ignore
+                        current_box = ann.image.get_embedding(image_id)  # type: ignore
+                    else:
+                        prev_box = sub_line[-1].bounding_box
+                        current_box = ann.bounding_box
 
-    # building connected components of columns
-    connected_components: List[Dict[str, Any]] = []
-    for idx, col in enumerate(columns):
-        col["id"] = idx
-        component_found = False
-        for comp in connected_components:
-            if (
-                comp["top"] < col["top"] < comp["bottom"]
-                or comp["top"] < col["bottom"] < comp["bottom"]
-                or col["top"] < comp["top"] < col["bottom"]
-                or col["top"] < comp["bottom"] < col["bottom"]
-            ):
-                comp["top"] = min(comp["top"], col["top"])
-                comp["bottom"] = max(comp["bottom"], col["bottom"])
-                comp["left"] = col["left"]
-                comp["column"].append(col)
-                component_found = True
-                break
-        if not component_found:
-            connected_components.append(
-                {"top": col["top"], "bottom": col["bottom"], "left": col["left"], "column": [col]}
-            )
+                    if prev_box.absolute_coords:
+                        prev_box = prev_box.transform(image_width, image_height)
+                    if current_box.absolute_coords:
+                        current_box = current_box.transform(image_width, image_height)
+
+                    # If distance between boxes is lower than paragraph break, same subline
+                    if current_box.ulx - prev_box.lrx < self.paragraph_break:
+                        horiz_break = False
+
+                    if horiz_break or idx == len(anns_per_row) - 2:
+                        if idx == len(anns_per_row) - 2:
+                            sub_line.append(ann)
+                            sub_line_ann_ids.append(ann.annotation_id)
+                        if image_id is not None:
+                            boxes = [ann.image.get_embedding(image_id) for ann in sub_line]  # type: ignore
+                        else:
+                            boxes = [ann.bounding_box for ann in sub_line]
+                        merge_box = merge_boxes(*boxes)
+                        detection_result = self._make_detect_result(merge_box, {"child": sub_line_ann_ids})
+                        detection_result_list.append(detection_result)
+                        sub_line = []
+                        sub_line_ann_ids = []
+
+                    sub_line.append(ann)
+                    sub_line_ann_ids.append(ann.annotation_id)
+            else:
+                # either row has only one word or all words should belong to one line
+                boxes = [ann.image.get_embedding(image_id) for ann in anns_per_row]  # type: ignore
+                merge_box = merge_boxes(*boxes)
+                detection_result = self._make_detect_result(
+                    merge_box, {"child": [ann.annotation_id for ann in anns_per_row]}
+                )
+                detection_result_list.append(detection_result)
 
-    # next, sorting columns in connected components by increasing x-value. In order to be tolerant to nearby values
-    # we are rounding values we want to sort
-    for comp in connected_components:
-        for col in comp["column"]:
-            col["left"] = round(col["left"], 2)
-            col["top"] = round(col["top"], 2)
-        comp["column"].sort(key=lambda x: (x["left"], x["top"]))
-
-    # finally, sorting connected components by increasing y-value
-    connected_components.sort(key=lambda x: x["top"])
-    columns = list(chain(*[comp["column"] for comp in connected_components]))
-
-    # old to new mapping
-    columns_dict = {col["id"]: k for k, col in enumerate(columns)}
-    _blocks = [(columns_dict[x[0]], x[1]) for x in reading_blocks]
-    _blocks.sort(key=lambda x: x[0])
-    reading_blocks = [(idx + 1, block[1]) for idx, block in enumerate(_blocks)]
-    return reading_blocks
+        return detection_result_list
 
 
 @pipeline_component_registry.register("TextOrderService")
 class TextOrderService(PipelineComponent):
     """
     Reading order of words within floating text blocks as well as reading order of blocks within simple text blocks.
     To understand the difference between floating text blocks and simple text blocks consider a page containing an
@@ -396,186 +439,176 @@
           page and the left and right text block boundaries as the left and right column boundaries.
 
     A category annotation per word is generated, which fixes the order per word in the block, as well as a category
     annotation per block, which saves the reading order of the block per page.
 
     The blocks are defined in `_floating_text_block_names` and text blocks in `_floating_text_block_names`.
 
-        order = TextOrderService(text_container=names.C.WORD,
-                                 floating_text_block_names=[names.C.TITLE, names.C.TEXT, names.C.LIST],
-                                 text_block_names=[names.C.TITLE, names.C.TEXT, names.C.LIST, names.C.CELL,
-                                                   names.C.HEAD, names.C.BODY])
+        order = TextOrderService(text_container="word",
+                                 text_block_categories=["title", "text", "list", "cell",
+                                                        "head", "body"],
+                                 floating_text_block_categories=["title", "text", "list"])
     """
 
     def __init__(
         self,
         text_container: str,
-        floating_text_block_names: Optional[Union[str, Sequence[str]]] = None,
-        text_block_names: Optional[Union[str, Sequence[str]]] = None,
-        text_containers_to_text_block: bool = False,
-    ) -> None:
+        text_block_categories: Optional[Union[str, Sequence[TypeOrStr]]] = None,
+        floating_text_block_categories: Optional[Union[str, Sequence[TypeOrStr]]] = None,
+        include_residual_text_container: bool = True,
+        starting_point_tolerance: float = 0.005,
+        broken_line_tolerance: float = 0.003,
+        height_tolerance: float = 2.0,
+        paragraph_break: Optional[float] = 0.035,
+        line_category_id: int = 1,
+    ):
         """
         :param text_container: name of an image annotation that has a CHARS sub category. These annotations will be
                                ordered within all text blocks.
-        :param floating_text_block_names: name of image annotation that belong to floating text. These annotations form
-                                          the highest hierarchy of text blocks that will be ordered to generate a
-                                          sensible output of text
-        :param text_block_names: name of image annotation that have a relation with text containers (or which might be
-                                 text containers themselves).
-        :param text_containers_to_text_block: Text containers are in general no text blocks and belong to a lower
-                                              hierarchy. However, if a text container is not assigned to a text block
-                                              you can add it to the text block ordering to ensure that the full text is
-                                              part of the subsequent sub process. Note however, that if the text
-                                              container is on word level rather than line level, the results will not be
-                                              very convincing
-        """
-        if isinstance(floating_text_block_names, str):
-            floating_text_block_names = [floating_text_block_names]
-        elif floating_text_block_names is None:
-            floating_text_block_names = []
-        if isinstance(text_block_names, str):
-            text_block_names = [text_block_names]
-        elif text_block_names is None:
-            text_block_names = []
-
-        self._text_container = text_container
-        self._floating_text_block_names = floating_text_block_names
-        self._text_block_names = text_block_names
-        self._text_containers_to_text_block = text_containers_to_text_block
-        self.starting_point_tolerance = 0.05
-        self.height_tolerance = 2.0
-        self.ignore_category_when_building_column_blocks = [LayoutType.table]
-        self._init_sanity_checks()
+        :param text_block_categories: name of image annotation that have a relation with text containers and where
+                                      text containers need to be sorted. It will default to
+                                      `..datapoint.view.IMAGE_DEFAULTS["text_block_categories"]`
+        :param floating_text_block_categories: name of image annotation that belong to floating text. These annotations
+                               form the highest hierarchy of text blocks that will be ordered to generate a narrative
+                               output of text. It will default to
+                               `..datapoint.view.IMAGE_DEFAULTS["floating_text_block_categories"]`
+        :param include_residual_text_container: Text containers with no parent text block (e.g. not matched with any
+                                                parent annotation in `MatchingService`) will not be assigned with a
+                                                reading. (Reading order will only be assigned to image annotations that
+                                                are floating_text_block_categories or text containers matched with
+                                                text block annotations.) Setting `include_residual_text_container=True`
+                                                will build synthetic text lines from text containers and regard these
+                                                text lines as floating text blocks.
+        """
+        self.text_container = get_type(text_container)
+        if isinstance(text_block_categories, (str, ObjectTypes)):
+            text_block_categories = [text_block_categories]
+        if text_block_categories is None:
+            text_block_categories = IMAGE_DEFAULTS["text_block_categories"]
+        self.text_block_categories = [get_type(category) for category in text_block_categories]
+        if isinstance(floating_text_block_categories, (str, ObjectTypes)):
+            floating_text_block_categories = [floating_text_block_categories]
+        if floating_text_block_categories is None:
+            floating_text_block_categories = IMAGE_DEFAULTS["floating_text_block_categories"]
+        self.floating_text_block_categories = [get_type(category) for category in floating_text_block_categories]
+        if include_residual_text_container:
+            self.floating_text_block_categories.append(LayoutType.line)
+        self.include_residual_text_container = include_residual_text_container
+        self.order_generator = OrderGenerator(starting_point_tolerance, broken_line_tolerance, height_tolerance)
+        self.text_line_generator = TextLineGenerator(
+            self.include_residual_text_container, line_category_id, paragraph_break
+        )
         super().__init__("text_order")
-
-    @property
-    def text_container(self) -> str:
-        """text container"""
-        return self._text_container
-
-    @property
-    def floating_text_block_names(self) -> Sequence[str]:
-        """floating text block names"""
-        return self._floating_text_block_names
-
-    @property
-    def text_block_names(self) -> Sequence[str]:
-        """text block names"""
-        return self._text_block_names
+        self._init_sanity_checks()
 
     def serve(self, dp: Image) -> None:
-        # select all text blocks that are considered to be relevant for page text. This does not include some layout
-        # items that have to be considered independently (e.g. tables). Order the blocks by column wise reading order
-        floating_text_block_anns = dp.get_annotation(category_names=self._floating_text_block_names)
-        number_floating_text_block_anns_orig = len(floating_text_block_anns)
-        # maybe add all text containers that are not mapped to any text block
-        if self._text_containers_to_text_block:
-            text_block_anns = dp.get_annotation(category_names=self._text_block_names)
-            text_ann_ids = list(
+        text_container_anns = dp.get_annotation(category_names=self.text_container)
+        text_block_anns = dp.get_annotation(category_names=self.text_block_categories)
+        if self.include_residual_text_container:
+            mapped_text_container_ids = list(
                 chain(*[text_block.get_relationship(Relationships.child) for text_block in text_block_anns])
             )
-            text_container_anns = dp.get_annotation(category_names=self._text_container)
-            text_container_anns = [ann for ann in text_container_anns if ann.annotation_id not in text_ann_ids]
-            floating_text_block_anns.extend(text_container_anns)
-
-        # estimating reading columns. We will only do this if we have some text blocks that are no text_containers
-        # (number_text_block_anns_orig >0) or if the text container is not a word. Otherwise, we will have to skip that
-        # part
-        if self._text_container != LayoutType.word or number_floating_text_block_anns_orig:
-            raw_reading_order_list = _reading_columns(
-                dp,
-                floating_text_block_anns,
-                self.starting_point_tolerance,
-                self.height_tolerance,
-                self.ignore_category_when_building_column_blocks,
-            )
+            residual_text_container_anns = [
+                ann for ann in text_container_anns if ann.annotation_id not in mapped_text_container_ids
+            ]
+            if self.text_container == LayoutType.word:
+                text_block_anns.extend(self._create_lines_for_words(residual_text_container_anns))
+            else:
+                text_block_anns.extend(residual_text_container_anns)
+        for text_block_ann in text_block_anns:
+            self.order_text_in_text_block(text_block_ann)
+        self.order_blocks(text_block_anns)
+
+    def _create_lines_for_words(self, word_anns: Sequence[ImageAnnotation]) -> Sequence[ImageAnnotation]:
+        detection_result_list = self.text_line_generator.create_detection_result(
+            word_anns,
+            self.dp_manager.datapoint.width,
+            self.dp_manager.datapoint.height,
+            self.dp_manager.datapoint.image_id,
+        )
+        line_anns = []
+        for detect_result in detection_result_list:
+            ann_id = self.dp_manager.set_image_annotation(detect_result)
+            if ann_id:
+                line_ann = self.dp_manager.get_annotation(ann_id)
+                child_ann_id_list = detect_result.relationships["child"]  # type: ignore
+                for child_ann_id in child_ann_id_list:
+                    line_ann.dump_relationship(Relationships.child, child_ann_id)
+                line_anns.append(line_ann)
+        return line_anns
 
-            for raw_reading_order in raw_reading_order_list:
-                self.dp_manager.set_category_annotation(
-                    Relationships.reading_order, raw_reading_order[0], Relationships.reading_order, raw_reading_order[1]
-                )
+    def order_text_in_text_block(self, text_block_ann: ImageAnnotation) -> None:
+        """
+        Order text within a text block. It will take all child-like text containers (determined by a
+        `MatchingOrderService`)  from a block and going to order all items line-wise.
 
-        # next we select all blocks that might contain text. We sort all text within these blocks
-        block_anns = dp.get_annotation(category_names=self._text_block_names)
-        for text_block in block_anns:
-            text_container_ann_ids = text_block.get_relationship(Relationships.child)
-            text_container_anns = dp.get_annotation(
-                annotation_ids=text_container_ann_ids,
-                category_names=self._text_container,
+        :param text_block_ann: text block annotation (category one of `text_block_categories`).
+        """
+        text_container_ids = text_block_ann.get_relationship(Relationships.child)
+        text_container_ann = self.dp_manager.datapoint.get_annotation(annotation_ids=text_container_ids)
+        if self.text_container == LayoutType.word:
+            word_order_list = self.order_generator.group_words_into_lines(
+                text_container_ann, self.dp_manager.datapoint.image_id
+            )
+        else:
+            word_order_list = self.order_generator.group_lines_into_lines(
+                text_container_ann, self.dp_manager.datapoint.image_id
+            )
+        for word_order in word_order_list:
+            self.dp_manager.set_category_annotation(
+                Relationships.reading_order, word_order[0], Relationships.reading_order, word_order[2]
             )
-            raw_reading_order_list = _reading_lines(dp.image_id, text_container_anns)
-            for raw_reading_order in raw_reading_order_list:
-                self.dp_manager.set_category_annotation(
-                    Relationships.reading_order, raw_reading_order[0], Relationships.reading_order, raw_reading_order[1]
-                )
 
-        # this is the setting where we order words without having text blocks
-        if not block_anns:
-            text_container_anns = dp.get_annotation(category_names=self._text_container)
-            # some OCR systems return textline and blocks. If they are available we will sort first by block, then by
-            # line and finally by center x coord.
-            if text_container_anns:
-                text_container_ann = text_container_anns[0]
-                if WordType.block and WordType.text_line in text_container_ann.sub_categories:
-                    text_container_position = [
-                        (
-                            int(ann.get_sub_category(WordType.block).category_id),
-                            int(ann.get_sub_category(WordType.text_line).category_id),
-                            ann.bounding_box.cx,  # type: ignore
-                            ann.annotation_id,
-                        )
-                        for ann in text_container_anns
-                    ]
-                    text_container_position.sort(key=lambda x: (x[0], x[1], x[2]))
-                    for position, element in enumerate(text_container_position):
-                        self.dp_manager.set_category_annotation(
-                            Relationships.reading_order, position, Relationships.reading_order, element[3]
-                        )
-                else:
-                    # Last try. We only form lines without and define a reading from this
-                    raw_reading_order_list = _reading_lines(dp.image_id, text_container_anns)
-                    for raw_reading_order in raw_reading_order_list:
-                        self.dp_manager.set_category_annotation(
-                            Relationships.reading_order,
-                            raw_reading_order[0],
-                            Relationships.reading_order,
-                            raw_reading_order[1],
-                        )
+    def order_blocks(self, text_block_anns: List[ImageAnnotation]) -> None:
+        """
+        Ordering of text blocks. Will use the internal order generator.
 
-    def clone(self) -> PipelineComponent:
-        return self.__class__(
-            copy(self._text_container),
-            deepcopy(self._floating_text_block_names),
-            deepcopy(self._text_block_names),
-            deepcopy(self._text_containers_to_text_block),
+        :param text_block_anns: list of `ImageAnnotation`.
+        """
+        block_order_list = self.order_generator.order_blocks(
+            text_block_anns, self.dp_manager.datapoint.width, self.dp_manager.datapoint.height
         )
+        for word_order in block_order_list:
+            self.dp_manager.set_category_annotation(
+                Relationships.reading_order, word_order[0], Relationships.reading_order, word_order[1]
+            )
 
     def _init_sanity_checks(self) -> None:
-        assert self._text_container in [LayoutType.word, LayoutType.line], (
+        assert self.text_container in (LayoutType.word, LayoutType.line), (
             f"text_container must be either {LayoutType.word} or " f"{LayoutType.line}"
         )
-        assert set(self._floating_text_block_names) <= set(
-            self._text_block_names
-        ), "floating_text_block_names must be a subset of text_block_names"
-        if (
-            self._text_container == LayoutType.word
-            and self._text_containers_to_text_block
-            and not self._floating_text_block_names
-        ):
-            logger.info(
-                "Choosing %s text_container while choosing no text_blocks will give no sensible "
-                "results. Choose %s text_container if you do not have text_blocks available.",
-                LayoutType.word,
-                LayoutType.line,
-            )
+        add_category = []
+        if self.include_residual_text_container:
+            add_category.append(LayoutType.line)
+
+        assert set(self.floating_text_block_categories) <= set(
+            self.text_block_categories + add_category  # type: ignore
+        ), "floating_text_block_categories must be a subset of text_block_categories"
 
     def get_meta_annotation(self) -> JsonDict:
-        anns_with_reading_order = list(deepcopy(self._floating_text_block_names))
-        anns_with_reading_order.extend([LayoutType.word, LayoutType.line])
+        add_category = [self.text_container]
+        image_annotations = []
+        if self.include_residual_text_container and self.text_container == LayoutType.word:
+            add_category.append(LayoutType.line)
+            image_annotations.append(LayoutType.line)
+        anns_with_reading_order = list(copy(self.floating_text_block_categories)) + add_category
         return dict(
             [
-                ("image_annotations", []),
+                ("image_annotations", image_annotations),
                 ("sub_categories", {category: {Relationships.reading_order} for category in anns_with_reading_order}),
                 ("relationships", {}),
                 ("summaries", []),
             ]
         )
+
+    def clone(self) -> PipelineComponent:
+        return self.__class__(
+            copy(self.text_container),
+            copy(self.text_block_categories),
+            copy(self.floating_text_block_categories),
+            self.include_residual_text_container,
+            self.order_generator.starting_point_tolerance,
+            self.order_generator.broken_line_tolerance,
+            self.order_generator.height_tolerance,
+            self.text_line_generator.paragraph_break,
+            self.text_line_generator.line_category_id,
+        )
```

### Comparing `deepdoctection-0.24/deepdoctection/pipe/transform.py` & `deepdoctection-0.25/deepdoctection/pipe/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/train/__init__.py` & `deepdoctection-0.25/deepdoctection/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/train/d2_frcnn_train.py` & `deepdoctection-0.25/deepdoctection/train/d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/train/hf_detr_train.py` & `deepdoctection-0.25/deepdoctection/train/hf_detr_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/train/hf_layoutlm_train.py` & `deepdoctection-0.25/deepdoctection/train/hf_layoutlm_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/train/tp_frcnn_train.py` & `deepdoctection-0.25/deepdoctection/train/tp_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/__init__.py` & `deepdoctection-0.25/deepdoctection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/concurrency.py` & `deepdoctection-0.25/deepdoctection/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/context.py` & `deepdoctection-0.25/deepdoctection/utils/context.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/detection_types.py` & `deepdoctection-0.25/deepdoctection/utils/detection_types.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/develop.py` & `deepdoctection-0.25/deepdoctection/utils/develop.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/file_utils.py` & `deepdoctection-0.25/deepdoctection/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/fs.py` & `deepdoctection-0.25/deepdoctection/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/identifier.py` & `deepdoctection-0.25/deepdoctection/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/logger.py` & `deepdoctection-0.25/deepdoctection/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/metacfg.py` & `deepdoctection-0.25/deepdoctection/utils/metacfg.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/pdf_utils.py` & `deepdoctection-0.25/deepdoctection/utils/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/settings.py` & `deepdoctection-0.25/deepdoctection/utils/settings.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/systools.py` & `deepdoctection-0.25/deepdoctection/utils/systools.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/tqdm.py` & `deepdoctection-0.25/deepdoctection/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/transform.py` & `deepdoctection-0.25/deepdoctection/utils/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/utils.py` & `deepdoctection-0.25/deepdoctection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection/utils/viz.py` & `deepdoctection-0.25/deepdoctection/utils/viz.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/deepdoctection.egg-info/PKG-INFO` & `deepdoctection-0.25/deepdoctection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.24
+Version: 0.25
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -50,25 +50,22 @@
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
- - Document and token classification with all [LayoutLM](https://github.com/microsoft/unilm) models 
-   provided by the [**Transformer**](https://github.com/huggingface/transformers) library. 
-   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!). 
-
-   [**!new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE) 
-   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v1_on_custom_token_classification.ipynb)
-   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3. Training 
-   scripts can now be tracked with W&B. Check the experimentation result of the notebooks [here](https://wandb.ai/jm76/FRFPE_layoutlmv1?workspace=user-jm76).
- - Table detection and table structure recognition with 
+ - Document and token classification with all LayoutLM models provided by the Transformer library. 
+   (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
+   Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). You can try a pipeline using 
    [**this script**](https://github.com/deepdoctection/deepdoctection/discussions/116).  
+ - [**new!**] There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
+   and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
+   to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
    
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
```

### Comparing `deepdoctection-0.24/deepdoctection.egg-info/SOURCES.txt` & `deepdoctection-0.25/deepdoctection.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 deepdoctection/pipe/cell.py
 deepdoctection/pipe/common.py
 deepdoctection/pipe/concurrency.py
 deepdoctection/pipe/doctectionpipe.py
 deepdoctection/pipe/language.py
 deepdoctection/pipe/layout.py
 deepdoctection/pipe/lm.py
+deepdoctection/pipe/order.py
 deepdoctection/pipe/refine.py
 deepdoctection/pipe/registry.py
 deepdoctection/pipe/segment.py
 deepdoctection/pipe/text.py
 deepdoctection/pipe/transform.py
 deepdoctection/train/__init__.py
 deepdoctection/train/d2_frcnn_train.py
@@ -215,14 +216,15 @@
 tests/pipe/__init__.py
 tests/pipe/test_anngen.py
 tests/pipe/test_cell.py
 tests/pipe/test_common.py
 tests/pipe/test_language.py
 tests/pipe/test_layout.py
 tests/pipe/test_lm.py
+tests/pipe/test_order.py
 tests/pipe/test_refine.py
 tests/pipe/test_registry.py
 tests/pipe/test_segment.py
 tests/pipe/test_text.py
 tests/pipe/test_transform.py
 tests/train/__init__.py
 tests/train/conftest.py
```

### Comparing `deepdoctection-0.24/deepdoctection.egg-info/requires.txt` & `deepdoctection-0.25/deepdoctection.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/setup.cfg` & `deepdoctection-0.25/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/setup.py` & `deepdoctection-0.25/setup.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/__init__.py` & `deepdoctection-0.25/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/analyzer/__init__.py` & `deepdoctection-0.25/tests/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/analyzer/test_dd.py` & `deepdoctection-0.25/tests/analyzer/test_dd.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 @mark.integration
 def test_dd_analyzer_builds_and_process_image_layout_correctly() -> None:
     """
     Analyzer integration test with setting tables = False and ocr = False
     """
 
     # Arrange
-    analyzer = get_dd_analyzer(tables=False, ocr=False)
+    analyzer = get_dd_analyzer(config_overwrite=["USE_TABLE_SEGMENTATION=False", "USE_OCR=False"])
 
     # Act
     df = analyzer.analyze(path=get_integration_test_path())
     output = collect_datapoint_from_dataflow(df)
 
     # Assert
     assert len(output) == 1
@@ -53,15 +53,15 @@
 @mark.integration
 def test_dd_analyzer_builds_and_process_image_layout_and_tables_correctly() -> None:
     """
     Analyzer integration test with setting tables = True and ocr = False
     """
 
     # Arrange
-    analyzer = get_dd_analyzer(tables=True, ocr=False)
+    analyzer = get_dd_analyzer(config_overwrite=["USE_OCR=False"])
 
     # Act
     df = analyzer.analyze(path=get_integration_test_path())
     output = collect_datapoint_from_dataflow(df)
 
     # Assert
     assert len(output) == 1
@@ -88,15 +88,15 @@
 @mark.integration
 def test_dd_analyzer_builds_and_process_image_correctly() -> None:
     """
     Analyzer integration test with setting tables = True and ocr = True
     """
 
     # Arrange
-    analyzer = get_dd_analyzer(tables=True, ocr=True)
+    analyzer = get_dd_analyzer()
 
     # Act
     df = analyzer.analyze(path=get_integration_test_path())
     output = collect_datapoint_from_dataflow(df)
 
     # Assert
     assert len(output) == 1
@@ -122,7 +122,11 @@
         "EUR 1.468.434</td></tr><tr><td>Gesamtvergiitung fuir sonstige Risikotrager</td><td>EUR 324.229</td></tr><tr>"
         "<td>Gesamtvergiitung fir Mitarbeiter mit Kontrollfunktionen</td><td>EUR 554.046</td></tr></table>",
     }
     assert page.height == 2339
     assert page.width == 1654
     # first number for tp model, second for pt model
     assert len(page.text) in {5045}
+    text_ = page.text_
+    assert text_["text"] == page.text
+    assert len(text_["text_list"]) == 632
+    assert len(text_["annotation_ids"]) == 632
```

### Comparing `deepdoctection-0.24/tests/conftest.py` & `deepdoctection-0.25/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/data.py` & `deepdoctection-0.25/tests/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/dataflow/__init__.py` & `deepdoctection-0.25/tests/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/dataflow/conftest.py` & `deepdoctection-0.25/tests/dataflow/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/dataflow/test_common.py` & `deepdoctection-0.25/tests/dataflow/test_common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/dataflow/test_custom.py` & `deepdoctection-0.25/tests/dataflow/test_custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/dataflow/test_custom_serialize.py` & `deepdoctection-0.25/tests/dataflow/test_custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/dataflow/test_parallel_map.py` & `deepdoctection-0.25/tests/dataflow/test_parallel_map.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/dataflow/test_stats.py` & `deepdoctection-0.25/tests/dataflow/test_stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datapoint/__init__.py` & `deepdoctection-0.25/tests/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datapoint/conftest.py` & `deepdoctection-0.25/tests/datapoint/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datapoint/test_annotation.py` & `deepdoctection-0.25/tests/datapoint/test_annotation.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datapoint/test_box.py` & `deepdoctection-0.25/tests/datapoint/test_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datapoint/test_convert.py` & `deepdoctection-0.25/tests/datapoint/test_convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datapoint/test_image.py` & `deepdoctection-0.25/tests/datapoint/test_image.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datapoint/test_view.py` & `deepdoctection-0.25/tests/datapoint/test_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     page = Page.from_image(
         dp_image,
         LayoutType.word,
         [LayoutType.text, LayoutType.title, LayoutType.list],
     )
 
     # Assert
-    assert page.text == "\nhello world\nbye world"
+    assert page.text == "hello world\nbye world\n"
 
 
 @mark.basic
 def test_image_with_anns_can_be_saved(image: WhiteImage) -> None:
     """
     test  save does not raise any exception
     """
```

### Comparing `deepdoctection-0.24/tests/datasets/__init__.py` & `deepdoctection-0.25/tests/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/__init__.py` & `deepdoctection-0.25/tests/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/conftest.py` & `deepdoctection-0.25/tests/datasets/instances/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_doclaynet.py` & `deepdoctection-0.25/tests/datasets/instances/test_doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_fintabnet.py` & `deepdoctection-0.25/tests/datasets/instances/test_fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_funsd.py` & `deepdoctection-0.25/tests/datasets/instances/test_funsd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_iiitar13k.py` & `deepdoctection-0.25/tests/datasets/instances/test_iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_layouttest.py` & `deepdoctection-0.25/tests/datasets/instances/test_layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_publaynet.py` & `deepdoctection-0.25/tests/datasets/instances/test_publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_pubtables1m.py` & `deepdoctection-0.25/tests/datasets/instances/test_pubtables1m.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_pubtabnet.py` & `deepdoctection-0.25/tests/datasets/instances/test_pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/instances/test_rvlcdip.py` & `deepdoctection-0.25/tests/datasets/instances/test_rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/test_adapter.py` & `deepdoctection-0.25/tests/datasets/test_adapter.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/test_info.py` & `deepdoctection-0.25/tests/datasets/test_info.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/datasets/test_registry.py` & `deepdoctection-0.25/tests/datasets/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/eval/__init__.py` & `deepdoctection-0.25/tests/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/eval/conftest.py` & `deepdoctection-0.25/tests/eval/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/eval/test_accmetric.py` & `deepdoctection-0.25/tests/eval/test_accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/eval/test_cocometric.py` & `deepdoctection-0.25/tests/eval/test_cocometric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/eval/test_eval.py` & `deepdoctection-0.25/tests/eval/test_eval.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/eval/test_registry.py` & `deepdoctection-0.25/tests/eval/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/eval/test_tedsmetric.py` & `deepdoctection-0.25/tests/eval/test_tedsmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/conftest.py` & `deepdoctection-0.25/tests/extern/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/data.py` & `deepdoctection-0.25/tests/extern/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_deskew.py` & `deepdoctection-0.25/tests/extern/test_deskew.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_doctrocr.py` & `deepdoctection-0.25/tests/extern/test_doctrocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_fastlang.py` & `deepdoctection-0.25/tests/extern/test_fastlang.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_hfdetr.py` & `deepdoctection-0.25/tests/extern/test_hfdetr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_hflayoutlm.py` & `deepdoctection-0.25/tests/extern/test_hflayoutlm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_pdftext.py` & `deepdoctection-0.25/tests/extern/test_pdftext.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_tessocr.py` & `deepdoctection-0.25/tests/extern/test_tessocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_texocr.py` & `deepdoctection-0.25/tests/extern/test_texocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/extern/test_tpdetect.py` & `deepdoctection-0.25/tests/extern/test_tpdetect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/__init__.py` & `deepdoctection-0.25/tests/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/conftest.py` & `deepdoctection-0.25/tests/mapper/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/data.py` & `deepdoctection-0.25/tests/mapper/data.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_cats.py` & `deepdoctection-0.25/tests/mapper/test_cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_cocostruct.py` & `deepdoctection-0.25/tests/mapper/test_cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_d2struct.py` & `deepdoctection-0.25/tests/mapper/test_d2struct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_hfstruct.py` & `deepdoctection-0.25/tests/mapper/test_hfstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_iiitar13k.py` & `deepdoctection-0.25/tests/mapper/test_iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_laylmstruct.py` & `deepdoctection-0.25/tests/mapper/test_laylmstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_misc.py` & `deepdoctection-0.25/tests/mapper/test_misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_prodigystruct.py` & `deepdoctection-0.25/tests/mapper/test_prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_pubstruct.py` & `deepdoctection-0.25/tests/mapper/test_pubstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_tpstruct.py` & `deepdoctection-0.25/tests/mapper/test_tpstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_utils.py` & `deepdoctection-0.25/tests/mapper/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/mapper/test_xfundstruct.py` & `deepdoctection-0.25/tests/mapper/test_xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/__init__.py` & `deepdoctection-0.25/tests/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_anngen.py` & `deepdoctection-0.25/tests/pipe/test_anngen.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_cell.py` & `deepdoctection-0.25/tests/pipe/test_cell.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_common.py` & `deepdoctection-0.25/tests/pipe/test_common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_language.py` & `deepdoctection-0.25/tests/pipe/test_language.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from unittest.mock import MagicMock
 
 from pytest import mark
 
 from deepdoctection.datapoint import ContainerAnnotation, Image
 from deepdoctection.extern.base import DetectionResult
 from deepdoctection.pipe.language import LanguageDetectionService
-from deepdoctection.pipe.text import TextOrderService
-from deepdoctection.utils import CellType, LayoutType, PageType
+from deepdoctection.pipe.order import TextOrderService
+from deepdoctection.utils import LayoutType, PageType
 
 
 class TestLanguageDetectionService:
     """
     Test LanguageDetectionService
     """
 
@@ -39,36 +39,23 @@
         """
         setup necessary components
         """
 
         self._language_detector = MagicMock()
         self._text_order_service = TextOrderService(
             text_container=LayoutType.word,
-            floating_text_block_names=[LayoutType.title, LayoutType.text, LayoutType.list],
-            text_block_names=[
+            text_block_categories=[
                 LayoutType.title,
                 LayoutType.text,
                 LayoutType.list,
                 LayoutType.cell,
-                CellType.header,
-                CellType.body,
-            ],
-        )
-        self.language_detection_service = LanguageDetectionService(
-            self._language_detector,
-            text_container=LayoutType.word,
-            text_block_names=[
-                LayoutType.title,
-                LayoutType.text,
-                LayoutType.list,
-                LayoutType.cell,
-                CellType.header,
-                CellType.body,
             ],
+            floating_text_block_categories=[LayoutType.title, LayoutType.text, LayoutType.list],
         )
+        self.language_detection_service = LanguageDetectionService(self._language_detector)
 
     @mark.basic
     def test_pass_datapoint(
         self, dp_image_with_layout_and_word_annotations: Image, language_detect_result: DetectionResult
     ) -> None:
         """
         test pass datapoint
```

### Comparing `deepdoctection-0.24/tests/pipe/test_layout.py` & `deepdoctection-0.25/tests/pipe/test_layout.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_lm.py` & `deepdoctection-0.25/tests/pipe/test_lm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_refine.py` & `deepdoctection-0.25/tests/pipe/test_refine.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_registry.py` & `deepdoctection-0.25/tests/pipe/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_segment.py` & `deepdoctection-0.25/tests/pipe/test_segment.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/pipe/test_text.py` & `deepdoctection-0.25/tests/pipe/test_text.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from typing import List
 from unittest.mock import MagicMock
 
 from pytest import mark, raises
 
 from deepdoctection.datapoint import BoundingBox, Image, ImageAnnotation
 from deepdoctection.extern.base import DetectionResult, ObjectDetector, PdfMiner
-from deepdoctection.pipe.text import TextExtractionService, TextOrderService
-from deepdoctection.utils.settings import CellType, LayoutType, Relationships
+from deepdoctection.pipe.text import TextExtractionService
+from deepdoctection.utils.settings import LayoutType
 
 
 class TestTextExtractionService:
     """
     Test TextExtractionService2. In this setting, extraction will be tested when extract_from_category is None.
     """
 
@@ -196,59 +196,7 @@
         assert global_box_fta == word_box_global[3]
         local_box_fta = fourth_word_ann.image.get_embedding(second_table_ann.annotation_id)  # type: ignore
         assert local_box_fta == fourth_word_ann.bounding_box
         st_text_ann = second_table_ann.image.get_annotation(  # type: ignore
             annotation_ids=fourth_word_ann.annotation_id
         )[0]
         assert isinstance(st_text_ann, ImageAnnotation)
-
-
-class TestTextOrderService:
-    """
-    Test TextOrderService
-    """
-
-    @staticmethod
-    @mark.basic
-    def test_integration_pipeline_component(dp_image_with_layout_and_word_annotations: Image) -> None:
-        """
-        test integration_pipeline_component
-        """
-
-        # Arrange
-        text_order_service = TextOrderService(
-            text_container=LayoutType.word,
-            floating_text_block_names=[LayoutType.title, LayoutType.text, LayoutType.list],
-            text_block_names=[
-                LayoutType.title,
-                LayoutType.text,
-                LayoutType.list,
-                LayoutType.cell,
-                CellType.header,
-                CellType.body,
-            ],
-        )
-        dp_image = dp_image_with_layout_and_word_annotations
-
-        # Act
-        text_order_service.pass_datapoint(dp_image)
-
-        # Assert
-        layout_anns = dp_image.get_annotation(category_names=[LayoutType.title, LayoutType.text])
-        word_anns = dp_image.get_annotation(category_names=LayoutType.word)
-
-        # only need to check on layout_anns and word_anns, if sub cats have been added
-        # and numbers are correctly assigned
-
-        sub_cat = layout_anns[0].get_sub_category(Relationships.reading_order)
-        assert sub_cat.category_id == "1"
-        sub_cat = layout_anns[1].get_sub_category(Relationships.reading_order)
-        assert sub_cat.category_id == "2"
-
-        sub_cat = word_anns[0].get_sub_category(Relationships.reading_order)
-        assert sub_cat.category_id == "1"
-        sub_cat = word_anns[1].get_sub_category(Relationships.reading_order)
-        assert sub_cat.category_id == "2"
-        sub_cat = word_anns[2].get_sub_category(Relationships.reading_order)
-        assert sub_cat.category_id == "1"
-        sub_cat = word_anns[3].get_sub_category(Relationships.reading_order)
-        assert sub_cat.category_id == "2"
```

### Comparing `deepdoctection-0.24/tests/pipe/test_transform.py` & `deepdoctection-0.25/tests/pipe/test_transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/test_utils.py` & `deepdoctection-0.25/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/train/__init__.py` & `deepdoctection-0.25/tests/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/train/conftest.py` & `deepdoctection-0.25/tests/train/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/train/test_d2_frcnn_train.py` & `deepdoctection-0.25/tests/train/test_d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests/train/test_tp_frcnn_train.py` & `deepdoctection-0.25/tests/train/test_tp_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests_d2/__init__.py` & `deepdoctection-0.25/tests_d2/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests_d2/conftest.py` & `deepdoctection-0.25/tests_d2/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.24/tests_d2/test_d2detect.py` & `deepdoctection-0.25/tests_d2/test_d2detect.py`

 * *Files identical despite different names*

