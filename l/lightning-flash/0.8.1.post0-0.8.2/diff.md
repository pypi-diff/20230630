# Comparing `tmp/lightning-flash-0.8.1.post0.tar.gz` & `tmp/lightning-flash-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lightning-flash-0.8.1.post0.tar", last modified: Thu Jan  5 06:11:08 2023, max compression
+gzip compressed data, was "lightning-flash-0.8.2.tar", last modified: Fri Jun 30 13:36:07 2023, max compression
```

## Comparing `lightning-flash-0.8.1.post0.tar` & `lightning-flash-0.8.2.tar`

### file list

```diff
@@ -1,414 +1,425 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/
--rw-r--r--   0 runner    (1001) docker     (122)    41086 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    11342 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    16150 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14237 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2188 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/assets/fish.jpg
--rw-r--r--   0 runner    (1001) docker     (122)   607310 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/assets/road.png
--rw-r--r--   0 runner    (1001) docker     (122)    31437 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/assets/starry_night.jpg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/audio/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/audio/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/classification/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    44165 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/classification/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6844 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/classification/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/classification/input_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/backbone.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    27780 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5659 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     4417 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/audio/speech_recognition/output_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7610 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)    12597 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6208 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/base_viz.py
--rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     7531 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/callback.py
--rw-r--r--   0 runner    (1001) docker     (122)    23256 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/data_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/data/io/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/io/classification_input.py
--rw-r--r--   0 runner    (1001) docker     (122)    12116 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/io/input.py
--rw-r--r--   0 runner    (1001) docker     (122)    31523 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/io/input_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/io/output.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/io/output_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/io/transform_predictions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/output.py
--rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/splits.py
--rw-r--r--   0 runner    (1001) docker     (122)     3895 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17108 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/data_frame.py
--rw-r--r--   0 runner    (1001) docker     (122)     5286 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/loading.py
--rw-r--r--   0 runner    (1001) docker     (122)     6749 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/samples.py
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utilities/sort.py
--rw-r--r--   0 runner    (1001) docker     (122)     5133 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10023 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/heads.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/integrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/integrations/fiftyone/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/fiftyone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4686 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/fiftyone/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/integrations/icevision/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/icevision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11623 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/icevision/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/icevision/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/icevision/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10545 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/icevision/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)     1889 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/icevision/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/integrations/labelstudio/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/labelstudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15182 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/labelstudio/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/labelstudio/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_forecasting/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4475 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_forecasting/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_forecasting/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_forecasting/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_tabular/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_tabular/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3516 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_tabular/backbones.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/integrations/transformers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/integrations/transformers/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    37727 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/optimizers/
--rw-r--r--   0 runner    (1001) docker     (122)      367 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7113 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/optimizers/lamb.py
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/optimizers/lars.py
--rw-r--r--   0 runner    (1001) docker     (122)     5831 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/optimizers/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/optimizers/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (122)    11436 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/serve/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/serve/_compat/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/_compat/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     9192 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/component.py
--rw-r--r--   0 runner    (1001) docker     (122)     5080 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/composition.py
--rw-r--r--   0 runner    (1001) docker     (122)    12094 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    33145 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)    27643 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/order.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/rewrite.py
--rw-r--r--   0 runner    (1001) docker     (122)    12298 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/task.py
--rw-r--r--   0 runner    (1001) docker     (122)     3263 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/dag/visualize.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)    15160 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/execution.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/flash_components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/serve/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6987 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/interfaces/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/interfaces/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/serve/interfaces/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/interfaces/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/
--rw-r--r--   0 runner    (1001) docker     (122)      702 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2740 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/bbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/label.py
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/number.py
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/repeated.py
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/types/text.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/serve/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    13696 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/core/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (122)     3634 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/embedder.py
--rw-r--r--   0 runner    (1001) docker     (122)    10394 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/flash_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    10245 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)      845 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/isinstance.py
--rw-r--r--   0 runner    (1001) docker     (122)    23474 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/providers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/stability.py
--rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/stages.py
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/core/utilities/url_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/graph/
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/backbones.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/graph/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/classification/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     9318 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/classification/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/classification/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/classification/input_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     5507 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/classification/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/collate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/graph/embedding/
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/graph/embedding/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21114 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/classification/backbones/
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/backbones/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)    15441 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/backbones/timm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/backbones/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/backbones/transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    60904 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/heads.py
--rw-r--r--   0 runner    (1001) docker     (122)     7616 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/input_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/classification/integrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/classification/integrations/baal/
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/integrations/baal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/integrations/baal/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/integrations/baal/dropout.py
--rw-r--r--   0 runner    (1001) docker     (122)     9183 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/integrations/baal/loop.py
--rw-r--r--   0 runner    (1001) docker     (122)     4997 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/integrations/learn2learn.py
--rw-r--r--   0 runner    (1001) docker     (122)     8131 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/classification/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/detection/
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4137 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/detection/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/detection/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    55288 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/detection/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     9372 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/detection/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/detection/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/detection/output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/embedding/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/embedding/heads/
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4605 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/heads/vissl_heads.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/embedding/losses/
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4254 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/losses/vissl_losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     7095 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/embedding/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3078 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/strategies/default.py
--rw-r--r--   0 runner    (1001) docker     (122)     2227 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/strategies/vissl_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/embedding/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/transforms/vissl_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/embedding/vissl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/vissl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7764 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/vissl/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3583 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/vissl/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/embedding/vissl/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/vissl/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/vissl/transforms/multicrop.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/embedding/vissl/transforms/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/backbones/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/backbones/fastface_backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1655 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     3441 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/input_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     7055 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/face_detection/output_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/instance_segmentation/
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/instance_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3026 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/instance_segmentation/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/instance_segmentation/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    22594 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/instance_segmentation/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3546 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/instance_segmentation/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/keypoint_detection/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/keypoint_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/keypoint_detection/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/keypoint_detection/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    14650 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/keypoint_detection/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/keypoint_detection/input_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     3420 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/keypoint_detection/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    29553 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/heads.py
--rw-r--r--   0 runner    (1001) docker     (122)     6518 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/input_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     8628 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4911 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4413 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/segmentation/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/image/style_transfer/
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/style_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/style_transfer/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/style_transfer/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    14199 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/style_transfer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/style_transfer/input_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     6306 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/style_transfer/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/image/style_transfer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/pointcloud/
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     4811 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/open3d_ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/open3d_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6684 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/open3d_ml/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/open3d_ml/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     9314 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/detection/open3d_ml/input.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/input.py
--rw-r--r--   0 runner    (1001) docker     (122)    10502 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/open3d_ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/open3d_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4163 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/open3d_ml/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/open3d_ml/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     6163 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/open3d_ml/sequences_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/setup_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/tabular/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/tabular/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/classification/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    28978 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/classification/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/classification/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/classification/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2961 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/classification/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/tabular/forecasting/
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/forecasting/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     8038 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/forecasting/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/forecasting/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/forecasting/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5182 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/input.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/tabular/regression/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/regression/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    25532 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/regression/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/regression/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     6572 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/tabular/regression/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/template/
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/template/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/template/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/template/classification/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/template/classification/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5555 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/template/classification/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      739 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5695 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/classification/backbones/
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/backbones/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/backbones/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    38754 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     5258 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/classification/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/embedding/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/embedding/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/embedding/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      897 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/ort_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/question_answering/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/question_answering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/question_answering/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     8760 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/question_answering/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    35396 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/question_answering/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6845 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/question_answering/input.py
--rw-r--r--   0 runner    (1001) docker     (122)    15267 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/question_answering/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/question_answering/output_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/core/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/core/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3144 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/core/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     8985 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/core/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/summarization/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/summarization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/summarization/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    20468 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/summarization/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4365 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/summarization/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/translation/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/translation/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    20619 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/translation/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4359 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/text/seq2seq/translation/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/video/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/flash/video/classification/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/video/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1925 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/video/classification/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    57593 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/video/classification/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    17393 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/video/classification/input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/video/classification/input_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/video/classification/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/flash/video/classification/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/lightning_flash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    16150 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/lightning_flash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12505 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/lightning_flash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/lightning_flash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/lightning_flash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/lightning_flash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     4330 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/lightning_flash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/lightning_flash.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_audio.txt
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_graph.txt
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_image.txt
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_image_extras.txt
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_image_extras_baal.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_pointcloud.txt
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_tabular.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_text.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_video.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/datatype_video_extras.txt
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)      423 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/serve.txt
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-01-05 06:11:08.000000 lightning-flash-0.8.1.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-01-05 06:11:05.000000 lightning-flash-0.8.1.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.998236 lightning-flash-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    42000 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11342 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15238 2023-06-30 13:36:06.998236 lightning-flash-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13353 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.946236 lightning-flash-0.8.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_audio.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_image.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_image_baal.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_image_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_image_segm.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_image_vissl.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_pointcloud.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_tabular.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_text.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/datatype_video.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/serve.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_audio.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_image.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_pointcloud.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_serve.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_tabular.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_text.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_video.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements/testing_vision.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 13:36:06.998236 lightning-flash-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     8900 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.942236 lightning-flash-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.946236 lightning-flash-0.8.2/src/flash/
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2190 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.946236 lightning-flash-0.8.2/src/flash/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)   108954 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/assets/example.wav
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/assets/fish.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)   607310 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/assets/road.png
+-rw-r--r--   0 runner    (1001) docker     (122)    31437 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/assets/starry_night.jpg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.946236 lightning-flash-0.8.2/src/flash/audio/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.946236 lightning-flash-0.8.2/src/flash/audio/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/classification/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44254 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/classification/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6800 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/classification/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/classification/input_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.950236 lightning-flash-0.8.2/src/flash/audio/speech_recognition/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/speech_recognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/speech_recognition/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/speech_recognition/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4664 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/speech_recognition/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27665 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/speech_recognition/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5671 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/speech_recognition/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4429 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/speech_recognition/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/audio/speech_recognition/output_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.950236 lightning-flash-0.8.2/src/flash/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7610 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12556 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.950236 lightning-flash-0.8.2/src/flash/core/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6215 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/base_viz.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/batch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7531 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23219 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/data_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/data/io/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/io/classification_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11990 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31298 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/io/input_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/io/output_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/io/transform_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/splits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3885 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/data/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17096 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utilities/classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utilities/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utilities/data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utilities/loading.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6749 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utilities/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utilities/samples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utilities/sort.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10019 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/heads.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/integrations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/integrations/fiftyone/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/fiftyone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4686 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/fiftyone/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/integrations/icevision/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/icevision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11623 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/icevision/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/icevision/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/icevision/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10556 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/icevision/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1889 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/icevision/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/integrations/labelstudio/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/labelstudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15137 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/labelstudio/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/labelstudio/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_forecasting/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4475 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_forecasting/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_forecasting/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_forecasting/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3159 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_tabular/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/pytorch_tabular/backbones.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.954236 lightning-flash-0.8.2/src/flash/core/integrations/transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/integrations/transformers/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37358 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.958236 lightning-flash-0.8.2/src/flash/core/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (122)      367 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7155 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/optimizers/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/optimizers/lars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5894 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/optimizers/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/optimizers/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11372 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2117 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.958236 lightning-flash-0.8.2/src/flash/core/serve/
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.958236 lightning-flash-0.8.2/src/flash/core/serve/_compat/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/_compat/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9181 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/composition.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12050 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.958236 lightning-flash-0.8.2/src/flash/core/serve/dag/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33810 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/dag/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/dag/order.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12763 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/dag/rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12823 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/dag/task.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3234 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/dag/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/dag/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/dag/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15139 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/execution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/flash_components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.958236 lightning-flash-0.8.2/src/flash/core/serve/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6969 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/interfaces/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/interfaces/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.958236 lightning-flash-0.8.2/src/flash/core/serve/interfaces/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/interfaces/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.962236 lightning-flash-0.8.2/src/flash/core/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      702 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2740 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/repeated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/types/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/serve/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11966 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.962236 lightning-flash-0.8.2/src/flash/core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3634 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10790 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/flash_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8857 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)      845 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/isinstance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22222 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/stability.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/stages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/core/utilities/url_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.962236 lightning-flash-0.8.2/src/flash/graph/
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/backbones.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.962236 lightning-flash-0.8.2/src/flash/graph/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/classification/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9333 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/classification/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/classification/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/classification/input_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5519 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/classification/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/collate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.962236 lightning-flash-0.8.2/src/flash/graph/embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/graph/embedding/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.962236 lightning-flash-0.8.2/src/flash/image/
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.962236 lightning-flash-0.8.2/src/flash/image/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20643 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.966236 lightning-flash-0.8.2/src/flash/image/classification/backbones/
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/backbones/clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15432 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/backbones/timm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/backbones/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/backbones/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60504 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/heads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7572 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/input_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.966236 lightning-flash-0.8.2/src/flash/image/classification/integrations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.966236 lightning-flash-0.8.2/src/flash/image/classification/integrations/baal/
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/integrations/baal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/integrations/baal/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/integrations/baal/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8335 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/integrations/baal/loop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4974 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/integrations/learn2learn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8131 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/classification/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.966236 lightning-flash-0.8.2/src/flash/image/detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4136 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/detection/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/detection/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55349 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/detection/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9338 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/detection/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/detection/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3671 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/detection/output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.966236 lightning-flash-0.8.2/src/flash/image/embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.966236 lightning-flash-0.8.2/src/flash/image/embedding/heads/
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/heads/vissl_heads.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.966236 lightning-flash-0.8.2/src/flash/image/embedding/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4254 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/losses/vissl_losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7119 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.966236 lightning-flash-0.8.2/src/flash/image/embedding/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3078 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/strategies/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2227 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/strategies/vissl_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.970236 lightning-flash-0.8.2/src/flash/image/embedding/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/transforms/vissl_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.970236 lightning-flash-0.8.2/src/flash/image/embedding/vissl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/vissl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7723 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/vissl/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3583 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/vissl/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.970236 lightning-flash-0.8.2/src/flash/image/embedding/vissl/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/vissl/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5135 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/vissl/transforms/multicrop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/embedding/vissl/transforms/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.974236 lightning-flash-0.8.2/src/flash/image/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.974236 lightning-flash-0.8.2/src/flash/image/face_detection/backbones/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/backbones/fastface_backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1655 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3434 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/input_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7055 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/face_detection/output_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.974236 lightning-flash-0.8.2/src/flash/image/instance_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/instance_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3026 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/instance_segmentation/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/instance_segmentation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22750 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/instance_segmentation/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3546 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/instance_segmentation/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.978236 lightning-flash-0.8.2/src/flash/image/keypoint_detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/keypoint_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2421 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/keypoint_detection/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/keypoint_detection/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14650 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/keypoint_detection/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/keypoint_detection/input_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3420 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/keypoint_detection/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.978236 lightning-flash-0.8.2/src/flash/image/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29391 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/heads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6518 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/input_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4911 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4413 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/segmentation/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.982236 lightning-flash-0.8.2/src/flash/image/style_transfer/
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/style_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/style_transfer/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/style_transfer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14197 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/style_transfer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/style_transfer/input_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/style_transfer/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/image/style_transfer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.982236 lightning-flash-0.8.2/src/flash/pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.982236 lightning-flash-0.8.2/src/flash/pointcloud/detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4819 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9353 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.982236 lightning-flash-0.8.2/src/flash/pointcloud/detection/open3d_ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/open3d_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/open3d_ml/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3341 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/open3d_ml/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9344 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/detection/open3d_ml/input.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.986236 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3724 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10410 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.986236 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/open3d_ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/open3d_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/open3d_ml/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/open3d_ml/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6109 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/pointcloud/segmentation/open3d_ml/sequences_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.986236 lightning-flash-0.8.2/src/flash/tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.986236 lightning-flash-0.8.2/src/flash/tabular/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/classification/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29038 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/classification/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4435 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/classification/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6930 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/classification/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/classification/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.986236 lightning-flash-0.8.2/src/flash/tabular/forecasting/
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/forecasting/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8046 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/forecasting/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/forecasting/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/forecasting/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5192 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/input.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.990236 lightning-flash-0.8.2/src/flash/tabular/regression/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/regression/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25564 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/regression/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/regression/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6391 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/tabular/regression/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.990236 lightning-flash-0.8.2/src/flash/template/
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.990236 lightning-flash-0.8.2/src/flash/template/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/template/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/template/classification/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10839 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/template/classification/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5555 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/template/classification/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.990236 lightning-flash-0.8.2/src/flash/text/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.990236 lightning-flash-0.8.2/src/flash/text/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.990236 lightning-flash-0.8.2/src/flash/text/classification/backbones/
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/backbones/clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/backbones/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38774 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5508 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5258 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/classification/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.994236 lightning-flash-0.8.2/src/flash/text/embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/embedding/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4600 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/embedding/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      897 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/ort_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.994236 lightning-flash-0.8.2/src/flash/text/question_answering/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/question_answering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/question_answering/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8760 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/question_answering/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35431 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/question_answering/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6802 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/question_answering/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15054 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/question_answering/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/question_answering/output_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.994236 lightning-flash-0.8.2/src/flash/text/seq2seq/
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.994236 lightning-flash-0.8.2/src/flash/text/seq2seq/core/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/core/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3139 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/core/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8997 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/core/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.994236 lightning-flash-0.8.2/src/flash/text/seq2seq/summarization/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/summarization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/summarization/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20927 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/summarization/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/summarization/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.998236 lightning-flash-0.8.2/src/flash/text/seq2seq/translation/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/translation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20676 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/translation/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/text/seq2seq/translation/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.998236 lightning-flash-0.8.2/src/flash/video/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.998236 lightning-flash-0.8.2/src/flash/video/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/video/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1925 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/video/classification/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57360 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/video/classification/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17303 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/video/classification/input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/video/classification/input_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/video/classification/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3488 2023-06-30 13:35:56.000000 lightning-flash-0.8.2/src/flash/video/classification/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:36:06.998236 lightning-flash-0.8.2/src/lightning_flash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15238 2023-06-30 13:36:06.000000 lightning-flash-0.8.2/src/lightning_flash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14096 2023-06-30 13:36:06.000000 lightning-flash-0.8.2/src/lightning_flash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 13:36:06.000000 lightning-flash-0.8.2/src/lightning_flash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-30 13:36:06.000000 lightning-flash-0.8.2/src/lightning_flash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 13:36:06.000000 lightning-flash-0.8.2/src/lightning_flash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     4184 2023-06-30 13:36:06.000000 lightning-flash-0.8.2/src/lightning_flash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-30 13:36:06.000000 lightning-flash-0.8.2/src/lightning_flash.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lightning-flash-0.8.1.post0/CHANGELOG.md` & `lightning-flash-0.8.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
+## [0.8.2] - 2023-06-30
+
+### Changed
+
+- Added GATE backbone for Tabular integrations ([#1559](https://github.com/Lightning-AI/lightning-flash/pull/1559))
+
+### Fixed
+
+- Fixed datamodule can't load files with square brackets in names ([#1501](https://github.com/Lightning-AI/lightning-flash/pull/1501))
+- Fixed channel dim selection on segmentation target ([#1509](https://github.com/Lightning-AI/lightning-flash/pull/1509))
+- Fixed used of `jsonargparse` avoiding reliance on non-public internal logic ([#1620](https://github.com/Lightning-AI/lightning-flash/pull/1620))
+- Compatibility with `pytorch-tabular>=1.0` ([#1545](https://github.com/Lightning-AI/lightning-flash/pull/1545))
+- Compatibility latest `numpy` ([#1595](https://github.com/Lightning-AI/lightning-flash/pull/1595))
+
 ## [0.8.1] - 2022-11-08
 
 ### Added
 
 - Added support for CLIP backbones to the `TextClassifier` and `ImageClassifier` tasks ([#1458](https://github.com/Lightning-AI/lightning-flash/pull/1458))
 
 ### Fixed
 
 - Fixed compatibility with `lightning==1.8.0` ([#1479](https://github.com/Lightning-AI/lightning-flash/pull/1479))
 - Fixed the error message to suggest installing `icevision`, if it's not found while loading data ([#1474](https://github.com/Lightning-AI/lightning-flash/pull/1474))
 - Fixed compatibility with `torchmetrics==0.10.0` ([#1469](https://github.com/Lightning-AI/lightning-flash/pull/1469))
+- Fixed type of `n_gram` from bool to int in TranslationTask ([#1486](https://github.com/Lightning-AI/lightning-flash/pull/1486))
 
 
 ## [0.8.0] - 2022-09-02
 
 ### Added
 
 - Added support for `from_tensors` for `VideoClassification` ([#1389](https://github.com/Lightning-AI/lightning-flash/pull/1389))
```

### Comparing `lightning-flash-0.8.1.post0/LICENSE` & `lightning-flash-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/PKG-INFO` & `lightning-flash-0.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-flash
-Version: 0.8.1.post0
+Version: 0.8.2
 Summary: Your PyTorch AI Factory - Flash enables you to easily configure and run complex AI recipes.
 Home-page: https://github.com/Lightning-AI/lightning-flash
 Download-URL: https://github.com/Lightning-AI/lightning-flash
 Author: PyTorchLightning et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-flash/issues
@@ -16,92 +16,80 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: base
 Provides-Extra: audio
 Provides-Extra: graph
 Provides-Extra: image
+Provides-Extra: image_baal
+Provides-Extra: image_extras
+Provides-Extra: image_segm
+Provides-Extra: image_vissl
 Provides-Extra: pointcloud
 Provides-Extra: tabular
 Provides-Extra: text
 Provides-Extra: video
-Provides-Extra: devel
 Provides-Extra: docs
-Provides-Extra: notebooks
 Provides-Extra: serve
 Provides-Extra: test
-Provides-Extra: image_extras
-Provides-Extra: image_extras_baal
-Provides-Extra: video_extras
 Provides-Extra: vision
 Provides-Extra: core
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/lightning-flash/raw/0.8.1.post0/docs/source/_static/images/logo.svg" width="400px">
+<img src="https://github.com/Lightning-AI/lightning-flash/raw/0.8.2/docs/source/_static/images/logo.svg" width="400px">
 
 
 **Your PyTorch AI Factory**
 
 ---
 
 <p align="center">
   <a href="#getting-started">Installation</a> •
   <a href="#flash-in-3-steps">Flash in 3 Steps</a> •
   <a href="https://lightning-flash.readthedocs.io/en/stable/?badge=stable">Docs</a> •
   <a href="#contribute">Contribute</a> •
   <a href="#community">Community</a> •
-  <a href="https://www.pytorchlightning.ai/">Website</a> •
+  <a href="https://www.lightning.ai/">Website</a> •
   <a href="#license">License</a>
 </p>
 
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning-flash)](https://pypi.org/project/lightning-flash/)
 [![PyPI Status](https://badge.fury.io/py/lightning-flash.svg)](https://badge.fury.io/py/lightning-flash)
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/pytorch-lightning/blob/master/LICENSE)
 
-![CI testing](https://github.com/Lightning-AI/lightning-flash/workflows/CI%20testing/badge.svg?tag=0.8.1.post0)
-[![codecov](https://codecov.io/gh/Lightning-AI/lightning-flash/release/0.8.1.post0/graph/badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-AI/lightning-flash)
+[![CI testing](https://github.com/Lightning-Universe/lightning-flash/actions/workflows/ci-testing.yml/badge.svg?event=push)](https://github.com/Lightning-Universe/lightning-flash/actions/workflows/ci-testing.yml)
+[![codecov](https://codecov.io/gh/Lightning-Universe/lightning-flash/release/0.8.2/graph/badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-Universe/lightning-flash)
 [![Documentation Status](https://readthedocs.org/projects/lightning-flash/badge/?version=latest)](https://lightning-flash.readthedocs.io/en/stable/?badge=stable)
 [![DOI](https://zenodo.org/badge/333857397.svg)](https://zenodo.org/badge/latestdoi/333857397)
 
 </div>
 
 ---
 
 <div align="center">
   Flash makes complex AI recipes for over 15 tasks across 7 data domains accessible to all.
   <br / >
   In a nutshell, Flash is the production grade research framework you always dreamed of but didn't have time to build.
 </div>
 
-
-## News
-
-- Sept 30: [Lightning Flash now supports Meta-Learning](https://devblog.pytorchlightning.ai/lightning-flash-now-supports-meta-learning-7c0ac8b1cde7)
-- Sept 9: [Lightning Flash 0.5](https://devblog.pytorchlightning.ai/flash-0-5-your-pytorch-ai-factory-81b172ff0d76)
-- Jul 12: Flash Task-a-thon community sprint with 25+ community members
-- Jul 1: [Lightning Flash 0.4](https://devblog.pytorchlightning.ai/lightning-flash-0-4-flash-serve-fiftyone-multi-label-text-classification-and-jit-support-97428276c06f)
-- Jun 22: [Ushering in the New Age of Video Understanding with PyTorch](https://medium.com/pytorch/ushering-in-the-new-age-of-video-understanding-with-pytorch-1d85078e8015)
-- May 24: [Lightning Flash 0.3](https://devblog.pytorchlightning.ai/lightning-flash-0-3-new-tasks-visualization-tools-data-pipeline-and-flash-registry-api-1e236ba9530)
-- May 20: [Video Understanding with PyTorch](https://towardsdatascience.com/video-understanding-made-simple-with-pytorch-video-and-lightning-flash-c7d65583c37e)
-- Feb 2: [Read our launch blogpost](https://pytorch-lightning.medium.com/introducing-lightning-flash-the-fastest-way-to-get-started-with-deep-learning-202f196b3b98)
-
 ## Getting Started
 
 From PyPI:
 
 ```bash
 pip install lightning-flash
 ```
@@ -109,15 +97,15 @@
 See [our installation guide](https://lightning-flash.readthedocs.io/en/latest/installation.html) for more options.
 
 ## Flash in 3 Steps
 
 ### Step 1. Load your data
 
 All data loading in Flash is performed via a `from_*` classmethod on a `DataModule`.
-Which `DataModule` to use and which `from_*` methods are available depends on the task you want to perform.
+To decide which `DataModule` to use and which `from_*` methods are available, it depends on the task you want to perform.
 For example, for image segmentation where your data is stored in folders, you would use the [`from_folders` method of the `SemanticSegmentationData` class](https://lightning-flash.readthedocs.io/en/latest/reference/semantic_segmentation.html#from-folders):
 
 ```py
 from flash.image import SemanticSegmentationData
 
 dm = SemanticSegmentationData.from_folders(
     train_folder="data/CameraRGB",
@@ -129,15 +117,15 @@
 
 ```
 
 ### Step 2: Configure your model
 
 Our tasks come loaded with pre-trained backbones and (where applicable) heads.
 You can view the available backbones to use with your task using [`available_backbones`](https://lightning-flash.readthedocs.io/en/latest/general/backbones.html).
-Once you've chosen, create the model:
+Once you've chosen one, create the model:
 
 ```py
 from flash.image import SemanticSegmentation
 
 print(SemanticSegmentation.available_heads())
 # ['deeplabv3', 'deeplabv3plus', 'fpn', ..., 'unetplusplus']
 
@@ -163,40 +151,44 @@
 
 ---
 
 ## PyTorch Recipes
 
 ### Make predictions with Flash!
 
-Serve in just 2 lines.
+Serve in just 2 lines:
 
 ```py
 from flash.image import SemanticSegmentation
 
 model = SemanticSegmentation.load_from_checkpoint("semantic_segmentation_model.pt")
 model.serve()
 ```
 
 or make predictions from raw data directly.
 
 ```py
+from flash import Trainer
+
 trainer = Trainer(strategy='ddp', accelerator="gpu", gpus=2)
 dm = SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
 predictions = trainer.predict(model, dm)
 ```
 
 ### Flash Training Strategies
 
 Training strategies are PyTorch SOTA Training Recipes which can be utilized with a given task.
 
 
-Check out this [example](https://github.com/Lightning-AI/lightning-flash/blob/master/flash_examples/integrations/learn2learn/image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/meta-learning.html) from [Learn2Learn](https://github.com/learnables/learn2learn).
+Check out this [example](https://github.com/Lightning-AI/lightning-flash/blob/master/examples/integrations/learn2learn/image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/meta-learning.html) from [Learn2Learn](https://github.com/learnables/learn2learn).
 This is particularly useful if you use this model in production and want to make sure the model adapts quickly to its new environment with minimal labelled data.
 
 ```py
+from flash.image import ImageClassifier
+
 model = ImageClassifier(
     backbone="resnet18",
     optimizer=torch.optim.Adam,
     optimizer_kwargs={"lr": 0.001},
     training_strategy="prototypicalnetworks",
     training_strategy_kwargs={
         "epoch_length": 10 * 16,
@@ -218,28 +210,32 @@
 * **[maml](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_maml.py)** : from Finn *et al.* 2017, [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks](https://arxiv.org/abs/1703.03400)
 * **[metaoptnet](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_metaoptnet.py)** : from Lee *et al.* 2019, [Meta-Learning with Differentiable Convex Optimization](https://arxiv.org/abs/1904.03758)
 * **[anil](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_anil.py)** : from Raghu *et al.* 2020, [Rapid Learning or Feature Reuse? Towards Understanding the Effectiveness of MAML](https://arxiv.org/abs/1909.09157)
 
 
 ### Flash Optimizers / Schedulers
 
-With Flash, swapping among 40+ optimizers and 15 + schedulers recipes are simple. Find the list of available optimizers, schedulers as follows:
+With Flash, swapping among 40+ optimizers and 15+ schedulers recipes are simple. Find the list of available optimizers, schedulers as follows:
 
 ```py
+from flash.image import ImageClassifier
+
 ImageClassifier.available_optimizers()
 # ['A2GradExp', ..., 'Yogi']
 
 ImageClassifier.available_schedulers()
 # ['CosineAnnealingLR', 'CosineAnnealingWarmRestarts', ..., 'polynomial_decay_schedule_with_warmup']
 ```
 
 Once you've chosen, create the model:
 
 ```py
-#### The optimizer of choice can be passed as a
+#### The optimizer of choice can be passed as
+from flash.image import ImageClassifier
+
 # - String value
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=None)
 
 # - Callable
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer=functools.partial(torch.optim.Adadelta, eps=0.5), lr_scheduler=None)
 
 # - Tuple[string, dict]: (The dict takes in the optimizer kwargs)
@@ -255,14 +251,16 @@
 # - Tuple[string, dict]: (The dict takes in the scheduler kwargs)
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=("StepLR", {"step_size": 10}))
 ```
 
 You can also register you own custom scheduler recipes beforeahand and use them shown as above:
 
 ```py
+from flash.image import ImageClassifier
+
 @ImageClassifier.lr_schedulers_registry
 def my_steplr_recipe(optimizer):
     return torch.optim.lr_scheduler.StepLR(optimizer, step_size=10)
 
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler="my_steplr_recipe")
 ```
 
@@ -314,30 +312,30 @@
 )
 
 ```
 
 ## Flash Zero - PyTorch Recipes from the Command Line!
 
 <div align="center">
-<img src="/https://github.com/Lightning-AI/lightning-flash/raw/0.8.1.post0/docs/source/_static/images/flash_zero.gif?raw=true" width="75%">
+<img src="/https://github.com/Lightning-AI/lightning-flash/raw/0.8.2/docs/source/_static/images/flash_zero.gif?raw=true" width="75%">
 </div>
 
 Flash Zero is a zero-code machine learning platform built
 directly into lightning-flash
-using the [`Lightning CLI`](https://pytorch-lightning.readthedocs.io/en/0.8.1.post0common/lightning_cli.html).
+using the [`Lightning CLI`](https://pytorch-lightning.readthedocs.io/en/0.8.2common/lightning_cli.html).
 
 To get started and view the available tasks, run:
 
-```py
+```bash
   flash --help
 ```
 
 For example, to train an image classifier for 10 epochs with a `resnet50` backbone on 2 GPUs using your own data, you can do:
 
-```py
+```bash
   flash image_classification --trainer.max_epochs 10 --trainer.gpus 2 --model.backbone resnet50 from_folders --train_folder {PATH_TO_DATA}
 ```
 
 ## Kaggle Notebook Examples
 
 - [🚢Titanic crash with Lightning⚡Flash](https://www.kaggle.com/jirkaborovec/titanic-crash-with-lightning-flash)
 - [🏠House 💵prices predictions with Lightning⚡Flash](https://www.kaggle.com/jirkaborovec/house-prices-predictions-with-lightning-flash)
```

#### html2text {}

```diff
@@ -1,161 +1,149 @@
-Metadata-Version: 2.1 Name: lightning-flash Version: 0.8.1.post0 Summary: Your
+Metadata-Version: 2.1 Name: lightning-flash Version: 0.8.2 Summary: Your
 PyTorch AI Factory - Flash enables you to easily configure and run complex AI
 recipes. Home-page: https://github.com/Lightning-AI/lightning-flash Download-
 URL: https://github.com/Lightning-AI/lightning-flash Author: PyTorchLightning
 et al. Author-email: name@pytorchlightning.ai License: Apache-2.0 Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning-flash/issues Project-
 URL: Documentation, https://lightning-flash.rtfd.io/en/latest/ Project-URL:
 Source Code, https://github.com/Lightning-AI/lightning-flash Keywords: deep
 learning,pytorch,AI Classifier: Environment :: Console Classifier: Natural
 Language :: English Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Image
 Recognition Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: audio Provides-Extra: graph Provides-Extra: image Provides-
-Extra: pointcloud Provides-Extra: tabular Provides-Extra: text Provides-Extra:
-video Provides-Extra: devel Provides-Extra: docs Provides-Extra: notebooks
-Provides-Extra: serve Provides-Extra: test Provides-Extra: image_extras
-Provides-Extra: image_extras_baal Provides-Extra: video_extras Provides-Extra:
-vision Provides-Extra: core Provides-Extra: all Provides-Extra: dev License-
-File: LICENSE
- [https://github.com/Lightning-AI/lightning-flash/raw/0.8.1.post0/docs/source/
-           _static/images/logo.svg] **Your PyTorch AI Factory** ---
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: base Provides-Extra: audio Provides-Extra: graph Provides-
+Extra: image Provides-Extra: image_baal Provides-Extra: image_extras Provides-
+Extra: image_segm Provides-Extra: image_vissl Provides-Extra: pointcloud
+Provides-Extra: tabular Provides-Extra: text Provides-Extra: video Provides-
+Extra: docs Provides-Extra: serve Provides-Extra: test Provides-Extra: vision
+Provides-Extra: core Provides-Extra: all Provides-Extra: dev License-File:
+LICENSE
+[https://github.com/Lightning-AI/lightning-flash/raw/0.8.2/docs/source/_static/
+               images/logo.svg] **Your PyTorch AI Factory** ---
   Installation â¢ Flash_in_3_Steps â¢ Docs â¢ Contribute â¢ Community â¢
                               Website â¢ License
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning-
   flash)](https://pypi.org/project/lightning-flash/) [![PyPI Status](https://
   badge.fury.io/py/lightning-flash.svg)](https://badge.fury.io/py/lightning-
 flash) [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)]
 (https://www.pytorchlightning.ai/community) [![license](https://img.shields.io/
 badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/pytorch-
- lightning/blob/master/LICENSE) ![CI testing](https://github.com/Lightning-AI/
- lightning-flash/workflows/CI%20testing/badge.svg?tag=0.8.1.post0) [![codecov]
-(https://codecov.io/gh/Lightning-AI/lightning-flash/release/0.8.1.post0/graph/
-  badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-AI/lightning-
-  flash) [![Documentation Status](https://readthedocs.org/projects/lightning-
-flash/badge/?version=latest)](https://lightning-flash.readthedocs.io/en/stable/
+  lightning/blob/master/LICENSE) [![CI testing](https://github.com/Lightning-
+          Universe/lightning-flash/actions/workflows/ci-testing.yml/
+ badge.svg?event=push)](https://github.com/Lightning-Universe/lightning-flash/
+actions/workflows/ci-testing.yml) [![codecov](https://codecov.io/gh/Lightning-
+   Universe/lightning-flash/release/0.8.2/graph/badge.svg?token=oLuUr9q1vt)]
+  (https://codecov.io/gh/Lightning-Universe/lightning-flash) [![Documentation
+        Status](https://readthedocs.org/projects/lightning-flash/badge/
+      ?version=latest)](https://lightning-flash.readthedocs.io/en/stable/
    ?badge=stable) [![DOI](https://zenodo.org/badge/333857397.svg)](https://
                      zenodo.org/badge/latestdoi/333857397)
 ---
     Flash makes complex AI recipes for over 15 tasks across 7 data domains
                               accessible to all.
  > In a nutshell, Flash is the production grade research framework you always
                    dreamed of but didn't have time to build.
-## News - Sept 30: [Lightning Flash now supports Meta-Learning](https://
-devblog.pytorchlightning.ai/lightning-flash-now-supports-meta-learning-
-7c0ac8b1cde7) - Sept 9: [Lightning Flash 0.5](https://
-devblog.pytorchlightning.ai/flash-0-5-your-pytorch-ai-factory-81b172ff0d76) -
-Jul 12: Flash Task-a-thon community sprint with 25+ community members - Jul 1:
-[Lightning Flash 0.4](https://devblog.pytorchlightning.ai/lightning-flash-0-4-
-flash-serve-fiftyone-multi-label-text-classification-and-jit-support-
-97428276c06f) - Jun 22: [Ushering in the New Age of Video Understanding with
-PyTorch](https://medium.com/pytorch/ushering-in-the-new-age-of-video-
-understanding-with-pytorch-1d85078e8015) - May 24: [Lightning Flash 0.3](https:
-//devblog.pytorchlightning.ai/lightning-flash-0-3-new-tasks-visualization-
-tools-data-pipeline-and-flash-registry-api-1e236ba9530) - May 20: [Video
-Understanding with PyTorch](https://towardsdatascience.com/video-understanding-
-made-simple-with-pytorch-video-and-lightning-flash-c7d65583c37e) - Feb 2: [Read
-our launch blogpost](https://pytorch-lightning.medium.com/introducing-
-lightning-flash-the-fastest-way-to-get-started-with-deep-learning-202f196b3b98)
 ## Getting Started From PyPI: ```bash pip install lightning-flash ``` See [our
 installation guide](https://lightning-flash.readthedocs.io/en/latest/
 installation.html) for more options. ## Flash in 3 Steps ### Step 1. Load your
 data All data loading in Flash is performed via a `from_*` classmethod on a
-`DataModule`. Which `DataModule` to use and which `from_*` methods are
-available depends on the task you want to perform. For example, for image
-segmentation where your data is stored in folders, you would use the
+`DataModule`. To decide which `DataModule` to use and which `from_*` methods
+are available, it depends on the task you want to perform. For example, for
+image segmentation where your data is stored in folders, you would use the
 [`from_folders` method of the `SemanticSegmentationData` class](https://
 lightning-flash.readthedocs.io/en/latest/reference/
 semantic_segmentation.html#from-folders): ```py from flash.image import
 SemanticSegmentationData dm = SemanticSegmentationData.from_folders
 ( train_folder="data/CameraRGB", train_target_folder="data/CameraSeg",
 val_split=0.1, image_size=(256, 256), num_classes=21, ) ``` ### Step 2:
 Configure your model Our tasks come loaded with pre-trained backbones and
 (where applicable) heads. You can view the available backbones to use with your
 task using [`available_backbones`](https://lightning-flash.readthedocs.io/en/
-latest/general/backbones.html). Once you've chosen, create the model: ```py
+latest/general/backbones.html). Once you've chosen one, create the model: ```py
 from flash.image import SemanticSegmentation print
 (SemanticSegmentation.available_heads()) # ['deeplabv3', 'deeplabv3plus',
 'fpn', ..., 'unetplusplus'] print(SemanticSegmentation.available_backbones
 ('fpn')) # ['densenet121', ..., 'xception'] # + 113 models print
 (SemanticSegmentation.available_pretrained_weights('efficientnet-b0')) #
 ['imagenet', 'advprop'] model = SemanticSegmentation( head="fpn",
 backbone='efficientnet-b0', pretrained="advprop", num_classes=dm.num_classes)
 ``` ### Step 3: Finetune! ```py from flash import Trainer trainer = Trainer
 (max_epochs=3) trainer.finetune(model, datamodule=datamodule,
 strategy="freeze") trainer.save_checkpoint("semantic_segmentation_model.pt")
 ``` --- ## PyTorch Recipes ### Make predictions with Flash! Serve in just 2
-lines. ```py from flash.image import SemanticSegmentation model =
+lines: ```py from flash.image import SemanticSegmentation model =
 SemanticSegmentation.load_from_checkpoint("semantic_segmentation_model.pt")
-model.serve() ``` or make predictions from raw data directly. ```py trainer =
-Trainer(strategy='ddp', accelerator="gpu", gpus=2) dm =
-SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
+model.serve() ``` or make predictions from raw data directly. ```py from flash
+import Trainer trainer = Trainer(strategy='ddp', accelerator="gpu", gpus=2) dm
+= SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
 predictions = trainer.predict(model, dm) ``` ### Flash Training Strategies
 Training strategies are PyTorch SOTA Training Recipes which can be utilized
 with a given task. Check out this [example](https://github.com/Lightning-AI/
-lightning-flash/blob/master/flash_examples/integrations/learn2learn/
+lightning-flash/blob/master/examples/integrations/learn2learn/
 image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4
 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/
 meta-learning.html) from [Learn2Learn](https://github.com/learnables/
 learn2learn). This is particularly useful if you use this model in production
 and want to make sure the model adapts quickly to its new environment with
-minimal labelled data. ```py model = ImageClassifier( backbone="resnet18",
-optimizer=torch.optim.Adam, optimizer_kwargs={"lr": 0.001},
-training_strategy="prototypicalnetworks", training_strategy_kwargs=
-{ "epoch_length": 10 * 16, "meta_batch_size": 4, "num_tasks": 200,
-"test_num_tasks": 2000, "ways": datamodule.num_classes, "shots": 1,
-"test_ways": 5, "test_shots": 1, "test_queries": 15, }, ) ``` In detail, the
-following methods are currently implemented: * **[prototypicalnetworks](https:/
-/github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/
-lightning/lightning_protonet.py)** : from Snell *et al.* 2017, [Prototypical
-Networks for Few-shot Learning](https://arxiv.org/abs/1703.05175) * **[maml]
-(https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/
-lightning/lightning_maml.py)** : from Finn *et al.* 2017, [Model-Agnostic Meta-
-Learning for Fast Adaptation of Deep Networks](https://arxiv.org/abs/
-1703.03400) * **[metaoptnet](https://github.com/learnables/learn2learn/blob/
-master/learn2learn/algorithms/lightning/lightning_metaoptnet.py)** : from Lee
-*et al.* 2019, [Meta-Learning with Differentiable Convex Optimization](https://
-arxiv.org/abs/1904.03758) * **[anil](https://github.com/learnables/learn2learn/
-blob/master/learn2learn/algorithms/lightning/lightning_anil.py)** : from Raghu
-*et al.* 2020, [Rapid Learning or Feature Reuse? Towards Understanding the
-Effectiveness of MAML](https://arxiv.org/abs/1909.09157) ### Flash Optimizers /
-Schedulers With Flash, swapping among 40+ optimizers and 15 + schedulers
-recipes are simple. Find the list of available optimizers, schedulers as
-follows: ```py ImageClassifier.available_optimizers() # ['A2GradExp', ...,
-'Yogi'] ImageClassifier.available_schedulers() # ['CosineAnnealingLR',
-'CosineAnnealingWarmRestarts', ..., 'polynomial_decay_schedule_with_warmup']
-``` Once you've chosen, create the model: ```py #### The optimizer of choice
-can be passed as a # - String value model = ImageClassifier
+minimal labelled data. ```py from flash.image import ImageClassifier model =
+ImageClassifier( backbone="resnet18", optimizer=torch.optim.Adam,
+optimizer_kwargs={"lr": 0.001}, training_strategy="prototypicalnetworks",
+training_strategy_kwargs={ "epoch_length": 10 * 16, "meta_batch_size": 4,
+"num_tasks": 200, "test_num_tasks": 2000, "ways": datamodule.num_classes,
+"shots": 1, "test_ways": 5, "test_shots": 1, "test_queries": 15, }, ) ``` In
+detail, the following methods are currently implemented: * **
+[prototypicalnetworks](https://github.com/learnables/learn2learn/blob/master/
+learn2learn/algorithms/lightning/lightning_protonet.py)** : from Snell *et al.*
+2017, [Prototypical Networks for Few-shot Learning](https://arxiv.org/abs/
+1703.05175) * **[maml](https://github.com/learnables/learn2learn/blob/master/
+learn2learn/algorithms/lightning/lightning_maml.py)** : from Finn *et al.*
+2017, [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks]
+(https://arxiv.org/abs/1703.03400) * **[metaoptnet](https://github.com/
+learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/
+lightning_metaoptnet.py)** : from Lee *et al.* 2019, [Meta-Learning with
+Differentiable Convex Optimization](https://arxiv.org/abs/1904.03758) * **
+[anil](https://github.com/learnables/learn2learn/blob/master/learn2learn/
+algorithms/lightning/lightning_anil.py)** : from Raghu *et al.* 2020, [Rapid
+Learning or Feature Reuse? Towards Understanding the Effectiveness of MAML]
+(https://arxiv.org/abs/1909.09157) ### Flash Optimizers / Schedulers With
+Flash, swapping among 40+ optimizers and 15+ schedulers recipes are simple.
+Find the list of available optimizers, schedulers as follows: ```py from
+flash.image import ImageClassifier ImageClassifier.available_optimizers() #
+['A2GradExp', ..., 'Yogi'] ImageClassifier.available_schedulers() #
+['CosineAnnealingLR', 'CosineAnnealingWarmRestarts', ...,
+'polynomial_decay_schedule_with_warmup'] ``` Once you've chosen, create the
+model: ```py #### The optimizer of choice can be passed as from flash.image
+import ImageClassifier # - String value model = ImageClassifier
 (backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=None) # -
 Callable model = ImageClassifier(backbone="resnet18", num_classes=2,
 optimizer=functools.partial(torch.optim.Adadelta, eps=0.5), lr_scheduler=None)
 # - Tuple[string, dict]: (The dict takes in the optimizer kwargs) model =
 ImageClassifier(backbone="resnet18", num_classes=2, optimizer=("Adadelta",
 {"epa": 0.5}), lr_scheduler=None) #### The scheduler of choice can be passed as
 a # - String value model = ImageClassifier(backbone="resnet18", num_classes=2,
 optimizer="Adam", lr_scheduler="constant_schedule") # - Callable model =
 ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
 lr_scheduler=functools.partial(CyclicLR, step_size_up=1500, mode='exp_range',
 gamma=0.5)) # - Tuple[string, dict]: (The dict takes in the scheduler kwargs)
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
 lr_scheduler=("StepLR", {"step_size": 10})) ``` You can also register you own
-custom scheduler recipes beforeahand and use them shown as above: ```py
-@ImageClassifier.lr_schedulers_registry def my_steplr_recipe(optimizer): return
-torch.optim.lr_scheduler.StepLR(optimizer, step_size=10) model =
-ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
-lr_scheduler="my_steplr_recipe") ``` ### Flash Transforms Flash includes some
-simple augmentations for each task by default, however, you will often want to
-override these and control your own augmentation recipe. To this end, Flash
-supports custom transformations with the [`InputTransform`](https://lightning-
-flash.readthedocs.io/en/stable/api/generated/
+custom scheduler recipes beforeahand and use them shown as above: ```py from
+flash.image import ImageClassifier @ImageClassifier.lr_schedulers_registry def
+my_steplr_recipe(optimizer): return torch.optim.lr_scheduler.StepLR(optimizer,
+step_size=10) model = ImageClassifier(backbone="resnet18", num_classes=2,
+optimizer="Adam", lr_scheduler="my_steplr_recipe") ``` ### Flash Transforms
+Flash includes some simple augmentations for each task by default, however, you
+will often want to override these and control your own augmentation recipe. To
+this end, Flash supports custom transformations with the [`InputTransform`]
+(https://lightning-flash.readthedocs.io/en/stable/api/generated/
 flash.core.data.io.input_transform.InputTransform.html). The `InputTransform`
 is like a callback for transforms, with hooks that can be used to apply
 transforms to samples or batches, on and off the device / accelerator. In
 addition, hooks can be specialized to apply transforms only to the input or
 target. With these hooks, complex transforms like MixUp can be implemented with
 ease. Here's an example (with an albumentations transform thrown in too!):
 ```py import torch import numpy as np import albumentations from flash import
@@ -168,22 +156,22 @@
 batch class MixUpInputTransform(InputTransform): def
 train_input_per_sample_transform(self): return AlbumentationsAdapter
 (albumentations.HorizontalFlip(p=0.5)) # This will be applied after
 transferring the batch to the device! def train_per_batch_transform_on_device
 (self): return mixup datamodule = ImageClassificationData.from_folders
 ( train_folder="data/train", transform=MixUpInputTransform, batch_size=2, ) ```
 ## Flash Zero - PyTorch Recipes from the Command Line!
-[/https://github.com/Lightning-AI/lightning-flash/raw/0.8.1.post0/docs/source/
+   [/https://github.com/Lightning-AI/lightning-flash/raw/0.8.2/docs/source/
                     _static/images/flash_zero.gif?raw=true]
 Flash Zero is a zero-code machine learning platform built directly into
 lightning-flash using the [`Lightning CLI`](https://pytorch-
-lightning.readthedocs.io/en/0.8.1.post0common/lightning_cli.html). To get
-started and view the available tasks, run: ```py flash --help ``` For example,
-to train an image classifier for 10 epochs with a `resnet50` backbone on 2 GPUs
-using your own data, you can do: ```py flash image_classification --
+lightning.readthedocs.io/en/0.8.2common/lightning_cli.html). To get started and
+view the available tasks, run: ```bash flash --help ``` For example, to train
+an image classifier for 10 epochs with a `resnet50` backbone on 2 GPUs using
+your own data, you can do: ```bash flash image_classification --
 trainer.max_epochs 10 --trainer.gpus 2 --model.backbone resnet50 from_folders -
 -train_folder {PATH_TO_DATA} ``` ## Kaggle Notebook Examples - [ð¢Titanic
 crash with Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/titanic-
 crash-with-lightning-flash) - [ð House ðµprices predictions with
 Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/house-prices-
 predictions-with-lightning-flash) - [Playing ðtabular with
 Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/playing-tabular-with-
```

### Comparing `lightning-flash-0.8.1.post0/README.md` & `lightning-flash-0.8.2/src/lightning_flash.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,95 @@
+Metadata-Version: 2.1
+Name: lightning-flash
+Version: 0.8.2
+Summary: Your PyTorch AI Factory - Flash enables you to easily configure and run complex AI recipes.
+Home-page: https://github.com/Lightning-AI/lightning-flash
+Download-URL: https://github.com/Lightning-AI/lightning-flash
+Author: PyTorchLightning et al.
+Author-email: name@pytorchlightning.ai
+License: Apache-2.0
+Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-flash/issues
+Project-URL: Documentation, https://lightning-flash.rtfd.io/en/latest/
+Project-URL: Source Code, https://github.com/Lightning-AI/lightning-flash
+Keywords: deep learning,pytorch,AI
+Classifier: Environment :: Console
+Classifier: Natural Language :: English
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: base
+Provides-Extra: audio
+Provides-Extra: graph
+Provides-Extra: image
+Provides-Extra: image_baal
+Provides-Extra: image_extras
+Provides-Extra: image_segm
+Provides-Extra: image_vissl
+Provides-Extra: pointcloud
+Provides-Extra: tabular
+Provides-Extra: text
+Provides-Extra: video
+Provides-Extra: docs
+Provides-Extra: serve
+Provides-Extra: test
+Provides-Extra: vision
+Provides-Extra: core
+Provides-Extra: all
+Provides-Extra: dev
+License-File: LICENSE
+
 <div align="center">
 
-<img src="docs/source/_static/images/logo.svg" width="400px">
+<img src="https://github.com/Lightning-AI/lightning-flash/raw/0.8.2/docs/source/_static/images/logo.svg" width="400px">
 
 
 **Your PyTorch AI Factory**
 
 ---
 
 <p align="center">
   <a href="#getting-started">Installation</a> •
   <a href="#flash-in-3-steps">Flash in 3 Steps</a> •
   <a href="https://lightning-flash.readthedocs.io/en/stable/?badge=stable">Docs</a> •
   <a href="#contribute">Contribute</a> •
   <a href="#community">Community</a> •
-  <a href="https://www.pytorchlightning.ai/">Website</a> •
+  <a href="https://www.lightning.ai/">Website</a> •
   <a href="#license">License</a>
 </p>
 
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning-flash)](https://pypi.org/project/lightning-flash/)
 [![PyPI Status](https://badge.fury.io/py/lightning-flash.svg)](https://badge.fury.io/py/lightning-flash)
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/pytorch-lightning/blob/master/LICENSE)
 
-![CI testing](https://github.com/Lightning-AI/lightning-flash/workflows/CI%20testing/badge.svg?branch=master&event=push)
-[![codecov](https://codecov.io/gh/Lightning-AI/lightning-flash/branch/master/graph/badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-AI/lightning-flash)
+[![CI testing](https://github.com/Lightning-Universe/lightning-flash/actions/workflows/ci-testing.yml/badge.svg?event=push)](https://github.com/Lightning-Universe/lightning-flash/actions/workflows/ci-testing.yml)
+[![codecov](https://codecov.io/gh/Lightning-Universe/lightning-flash/release/0.8.2/graph/badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-Universe/lightning-flash)
 [![Documentation Status](https://readthedocs.org/projects/lightning-flash/badge/?version=latest)](https://lightning-flash.readthedocs.io/en/stable/?badge=stable)
 [![DOI](https://zenodo.org/badge/333857397.svg)](https://zenodo.org/badge/latestdoi/333857397)
 
 </div>
 
 ---
 
 <div align="center">
   Flash makes complex AI recipes for over 15 tasks across 7 data domains accessible to all.
   <br / >
   In a nutshell, Flash is the production grade research framework you always dreamed of but didn't have time to build.
 </div>
 
-
-## News
-
-- Sept 30: [Lightning Flash now supports Meta-Learning](https://devblog.pytorchlightning.ai/lightning-flash-now-supports-meta-learning-7c0ac8b1cde7)
-- Sept 9: [Lightning Flash 0.5](https://devblog.pytorchlightning.ai/flash-0-5-your-pytorch-ai-factory-81b172ff0d76)
-- Jul 12: Flash Task-a-thon community sprint with 25+ community members
-- Jul 1: [Lightning Flash 0.4](https://devblog.pytorchlightning.ai/lightning-flash-0-4-flash-serve-fiftyone-multi-label-text-classification-and-jit-support-97428276c06f)
-- Jun 22: [Ushering in the New Age of Video Understanding with PyTorch](https://medium.com/pytorch/ushering-in-the-new-age-of-video-understanding-with-pytorch-1d85078e8015)
-- May 24: [Lightning Flash 0.3](https://devblog.pytorchlightning.ai/lightning-flash-0-3-new-tasks-visualization-tools-data-pipeline-and-flash-registry-api-1e236ba9530)
-- May 20: [Video Understanding with PyTorch](https://towardsdatascience.com/video-understanding-made-simple-with-pytorch-video-and-lightning-flash-c7d65583c37e)
-- Feb 2: [Read our launch blogpost](https://pytorch-lightning.medium.com/introducing-lightning-flash-the-fastest-way-to-get-started-with-deep-learning-202f196b3b98)
-
 ## Getting Started
 
 From PyPI:
 
 ```bash
 pip install lightning-flash
 ```
@@ -61,15 +97,15 @@
 See [our installation guide](https://lightning-flash.readthedocs.io/en/latest/installation.html) for more options.
 
 ## Flash in 3 Steps
 
 ### Step 1. Load your data
 
 All data loading in Flash is performed via a `from_*` classmethod on a `DataModule`.
-Which `DataModule` to use and which `from_*` methods are available depends on the task you want to perform.
+To decide which `DataModule` to use and which `from_*` methods are available, it depends on the task you want to perform.
 For example, for image segmentation where your data is stored in folders, you would use the [`from_folders` method of the `SemanticSegmentationData` class](https://lightning-flash.readthedocs.io/en/latest/reference/semantic_segmentation.html#from-folders):
 
 ```py
 from flash.image import SemanticSegmentationData
 
 dm = SemanticSegmentationData.from_folders(
     train_folder="data/CameraRGB",
@@ -81,15 +117,15 @@
 
 ```
 
 ### Step 2: Configure your model
 
 Our tasks come loaded with pre-trained backbones and (where applicable) heads.
 You can view the available backbones to use with your task using [`available_backbones`](https://lightning-flash.readthedocs.io/en/latest/general/backbones.html).
-Once you've chosen, create the model:
+Once you've chosen one, create the model:
 
 ```py
 from flash.image import SemanticSegmentation
 
 print(SemanticSegmentation.available_heads())
 # ['deeplabv3', 'deeplabv3plus', 'fpn', ..., 'unetplusplus']
 
@@ -115,40 +151,44 @@
 
 ---
 
 ## PyTorch Recipes
 
 ### Make predictions with Flash!
 
-Serve in just 2 lines.
+Serve in just 2 lines:
 
 ```py
 from flash.image import SemanticSegmentation
 
 model = SemanticSegmentation.load_from_checkpoint("semantic_segmentation_model.pt")
 model.serve()
 ```
 
 or make predictions from raw data directly.
 
 ```py
+from flash import Trainer
+
 trainer = Trainer(strategy='ddp', accelerator="gpu", gpus=2)
 dm = SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
 predictions = trainer.predict(model, dm)
 ```
 
 ### Flash Training Strategies
 
 Training strategies are PyTorch SOTA Training Recipes which can be utilized with a given task.
 
 
-Check out this [example](https://github.com/Lightning-AI/lightning-flash/blob/master/flash_examples/integrations/learn2learn/image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/meta-learning.html) from [Learn2Learn](https://github.com/learnables/learn2learn).
+Check out this [example](https://github.com/Lightning-AI/lightning-flash/blob/master/examples/integrations/learn2learn/image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/meta-learning.html) from [Learn2Learn](https://github.com/learnables/learn2learn).
 This is particularly useful if you use this model in production and want to make sure the model adapts quickly to its new environment with minimal labelled data.
 
 ```py
+from flash.image import ImageClassifier
+
 model = ImageClassifier(
     backbone="resnet18",
     optimizer=torch.optim.Adam,
     optimizer_kwargs={"lr": 0.001},
     training_strategy="prototypicalnetworks",
     training_strategy_kwargs={
         "epoch_length": 10 * 16,
@@ -170,28 +210,32 @@
 * **[maml](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_maml.py)** : from Finn *et al.* 2017, [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks](https://arxiv.org/abs/1703.03400)
 * **[metaoptnet](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_metaoptnet.py)** : from Lee *et al.* 2019, [Meta-Learning with Differentiable Convex Optimization](https://arxiv.org/abs/1904.03758)
 * **[anil](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_anil.py)** : from Raghu *et al.* 2020, [Rapid Learning or Feature Reuse? Towards Understanding the Effectiveness of MAML](https://arxiv.org/abs/1909.09157)
 
 
 ### Flash Optimizers / Schedulers
 
-With Flash, swapping among 40+ optimizers and 15 + schedulers recipes are simple. Find the list of available optimizers, schedulers as follows:
+With Flash, swapping among 40+ optimizers and 15+ schedulers recipes are simple. Find the list of available optimizers, schedulers as follows:
 
 ```py
+from flash.image import ImageClassifier
+
 ImageClassifier.available_optimizers()
 # ['A2GradExp', ..., 'Yogi']
 
 ImageClassifier.available_schedulers()
 # ['CosineAnnealingLR', 'CosineAnnealingWarmRestarts', ..., 'polynomial_decay_schedule_with_warmup']
 ```
 
 Once you've chosen, create the model:
 
 ```py
-#### The optimizer of choice can be passed as a
+#### The optimizer of choice can be passed as
+from flash.image import ImageClassifier
+
 # - String value
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=None)
 
 # - Callable
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer=functools.partial(torch.optim.Adadelta, eps=0.5), lr_scheduler=None)
 
 # - Tuple[string, dict]: (The dict takes in the optimizer kwargs)
@@ -207,14 +251,16 @@
 # - Tuple[string, dict]: (The dict takes in the scheduler kwargs)
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=("StepLR", {"step_size": 10}))
 ```
 
 You can also register you own custom scheduler recipes beforeahand and use them shown as above:
 
 ```py
+from flash.image import ImageClassifier
+
 @ImageClassifier.lr_schedulers_registry
 def my_steplr_recipe(optimizer):
     return torch.optim.lr_scheduler.StepLR(optimizer, step_size=10)
 
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler="my_steplr_recipe")
 ```
 
@@ -266,30 +312,30 @@
 )
 
 ```
 
 ## Flash Zero - PyTorch Recipes from the Command Line!
 
 <div align="center">
-<img src="/docs/source/_static/images/flash_zero.gif?raw=true" width="75%">
+<img src="/https://github.com/Lightning-AI/lightning-flash/raw/0.8.2/docs/source/_static/images/flash_zero.gif?raw=true" width="75%">
 </div>
 
 Flash Zero is a zero-code machine learning platform built
 directly into lightning-flash
-using the [`Lightning CLI`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_cli.html).
+using the [`Lightning CLI`](https://pytorch-lightning.readthedocs.io/en/0.8.2common/lightning_cli.html).
 
 To get started and view the available tasks, run:
 
-```py
+```bash
   flash --help
 ```
 
 For example, to train an image classifier for 10 epochs with a `resnet50` backbone on 2 GPUs using your own data, you can do:
 
-```py
+```bash
   flash image_classification --trainer.max_epochs 10 --trainer.gpus 2 --model.backbone resnet50 from_folders --train_folder {PATH_TO_DATA}
 ```
 
 ## Kaggle Notebook Examples
 
 - [🚢Titanic crash with Lightning⚡Flash](https://www.kaggle.com/jirkaborovec/titanic-crash-with-lightning-flash)
 - [🏠House 💵prices predictions with Lightning⚡Flash](https://www.kaggle.com/jirkaborovec/house-prices-predictions-with-lightning-flash)
```

#### html2text {}

```diff
@@ -1,136 +1,149 @@
-     [docs/source/_static/images/logo.svg] **Your PyTorch AI Factory** ---
+Metadata-Version: 2.1 Name: lightning-flash Version: 0.8.2 Summary: Your
+PyTorch AI Factory - Flash enables you to easily configure and run complex AI
+recipes. Home-page: https://github.com/Lightning-AI/lightning-flash Download-
+URL: https://github.com/Lightning-AI/lightning-flash Author: PyTorchLightning
+et al. Author-email: name@pytorchlightning.ai License: Apache-2.0 Project-URL:
+Bug Tracker, https://github.com/Lightning-AI/lightning-flash/issues Project-
+URL: Documentation, https://lightning-flash.rtfd.io/en/latest/ Project-URL:
+Source Code, https://github.com/Lightning-AI/lightning-flash Keywords: deep
+learning,pytorch,AI Classifier: Environment :: Console Classifier: Natural
+Language :: English Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Image
+Recognition Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: base Provides-Extra: audio Provides-Extra: graph Provides-
+Extra: image Provides-Extra: image_baal Provides-Extra: image_extras Provides-
+Extra: image_segm Provides-Extra: image_vissl Provides-Extra: pointcloud
+Provides-Extra: tabular Provides-Extra: text Provides-Extra: video Provides-
+Extra: docs Provides-Extra: serve Provides-Extra: test Provides-Extra: vision
+Provides-Extra: core Provides-Extra: all Provides-Extra: dev License-File:
+LICENSE
+[https://github.com/Lightning-AI/lightning-flash/raw/0.8.2/docs/source/_static/
+               images/logo.svg] **Your PyTorch AI Factory** ---
   Installation â¢ Flash_in_3_Steps â¢ Docs â¢ Contribute â¢ Community â¢
                               Website â¢ License
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning-
   flash)](https://pypi.org/project/lightning-flash/) [![PyPI Status](https://
   badge.fury.io/py/lightning-flash.svg)](https://badge.fury.io/py/lightning-
 flash) [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)]
 (https://www.pytorchlightning.ai/community) [![license](https://img.shields.io/
 badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/pytorch-
- lightning/blob/master/LICENSE) ![CI testing](https://github.com/Lightning-AI/
- lightning-flash/workflows/CI%20testing/badge.svg?branch=master&event=push) [!
-  [codecov](https://codecov.io/gh/Lightning-AI/lightning-flash/branch/master/
-    graph/badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-AI/
-  lightning-flash) [![Documentation Status](https://readthedocs.org/projects/
-lightning-flash/badge/?version=latest)](https://lightning-flash.readthedocs.io/
-   en/stable/?badge=stable) [![DOI](https://zenodo.org/badge/333857397.svg)]
-                (https://zenodo.org/badge/latestdoi/333857397)
+  lightning/blob/master/LICENSE) [![CI testing](https://github.com/Lightning-
+          Universe/lightning-flash/actions/workflows/ci-testing.yml/
+ badge.svg?event=push)](https://github.com/Lightning-Universe/lightning-flash/
+actions/workflows/ci-testing.yml) [![codecov](https://codecov.io/gh/Lightning-
+   Universe/lightning-flash/release/0.8.2/graph/badge.svg?token=oLuUr9q1vt)]
+  (https://codecov.io/gh/Lightning-Universe/lightning-flash) [![Documentation
+        Status](https://readthedocs.org/projects/lightning-flash/badge/
+      ?version=latest)](https://lightning-flash.readthedocs.io/en/stable/
+   ?badge=stable) [![DOI](https://zenodo.org/badge/333857397.svg)](https://
+                     zenodo.org/badge/latestdoi/333857397)
 ---
     Flash makes complex AI recipes for over 15 tasks across 7 data domains
                               accessible to all.
  > In a nutshell, Flash is the production grade research framework you always
                    dreamed of but didn't have time to build.
-## News - Sept 30: [Lightning Flash now supports Meta-Learning](https://
-devblog.pytorchlightning.ai/lightning-flash-now-supports-meta-learning-
-7c0ac8b1cde7) - Sept 9: [Lightning Flash 0.5](https://
-devblog.pytorchlightning.ai/flash-0-5-your-pytorch-ai-factory-81b172ff0d76) -
-Jul 12: Flash Task-a-thon community sprint with 25+ community members - Jul 1:
-[Lightning Flash 0.4](https://devblog.pytorchlightning.ai/lightning-flash-0-4-
-flash-serve-fiftyone-multi-label-text-classification-and-jit-support-
-97428276c06f) - Jun 22: [Ushering in the New Age of Video Understanding with
-PyTorch](https://medium.com/pytorch/ushering-in-the-new-age-of-video-
-understanding-with-pytorch-1d85078e8015) - May 24: [Lightning Flash 0.3](https:
-//devblog.pytorchlightning.ai/lightning-flash-0-3-new-tasks-visualization-
-tools-data-pipeline-and-flash-registry-api-1e236ba9530) - May 20: [Video
-Understanding with PyTorch](https://towardsdatascience.com/video-understanding-
-made-simple-with-pytorch-video-and-lightning-flash-c7d65583c37e) - Feb 2: [Read
-our launch blogpost](https://pytorch-lightning.medium.com/introducing-
-lightning-flash-the-fastest-way-to-get-started-with-deep-learning-202f196b3b98)
 ## Getting Started From PyPI: ```bash pip install lightning-flash ``` See [our
 installation guide](https://lightning-flash.readthedocs.io/en/latest/
 installation.html) for more options. ## Flash in 3 Steps ### Step 1. Load your
 data All data loading in Flash is performed via a `from_*` classmethod on a
-`DataModule`. Which `DataModule` to use and which `from_*` methods are
-available depends on the task you want to perform. For example, for image
-segmentation where your data is stored in folders, you would use the
+`DataModule`. To decide which `DataModule` to use and which `from_*` methods
+are available, it depends on the task you want to perform. For example, for
+image segmentation where your data is stored in folders, you would use the
 [`from_folders` method of the `SemanticSegmentationData` class](https://
 lightning-flash.readthedocs.io/en/latest/reference/
 semantic_segmentation.html#from-folders): ```py from flash.image import
 SemanticSegmentationData dm = SemanticSegmentationData.from_folders
 ( train_folder="data/CameraRGB", train_target_folder="data/CameraSeg",
 val_split=0.1, image_size=(256, 256), num_classes=21, ) ``` ### Step 2:
 Configure your model Our tasks come loaded with pre-trained backbones and
 (where applicable) heads. You can view the available backbones to use with your
 task using [`available_backbones`](https://lightning-flash.readthedocs.io/en/
-latest/general/backbones.html). Once you've chosen, create the model: ```py
+latest/general/backbones.html). Once you've chosen one, create the model: ```py
 from flash.image import SemanticSegmentation print
 (SemanticSegmentation.available_heads()) # ['deeplabv3', 'deeplabv3plus',
 'fpn', ..., 'unetplusplus'] print(SemanticSegmentation.available_backbones
 ('fpn')) # ['densenet121', ..., 'xception'] # + 113 models print
 (SemanticSegmentation.available_pretrained_weights('efficientnet-b0')) #
 ['imagenet', 'advprop'] model = SemanticSegmentation( head="fpn",
 backbone='efficientnet-b0', pretrained="advprop", num_classes=dm.num_classes)
 ``` ### Step 3: Finetune! ```py from flash import Trainer trainer = Trainer
 (max_epochs=3) trainer.finetune(model, datamodule=datamodule,
 strategy="freeze") trainer.save_checkpoint("semantic_segmentation_model.pt")
 ``` --- ## PyTorch Recipes ### Make predictions with Flash! Serve in just 2
-lines. ```py from flash.image import SemanticSegmentation model =
+lines: ```py from flash.image import SemanticSegmentation model =
 SemanticSegmentation.load_from_checkpoint("semantic_segmentation_model.pt")
-model.serve() ``` or make predictions from raw data directly. ```py trainer =
-Trainer(strategy='ddp', accelerator="gpu", gpus=2) dm =
-SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
+model.serve() ``` or make predictions from raw data directly. ```py from flash
+import Trainer trainer = Trainer(strategy='ddp', accelerator="gpu", gpus=2) dm
+= SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
 predictions = trainer.predict(model, dm) ``` ### Flash Training Strategies
 Training strategies are PyTorch SOTA Training Recipes which can be utilized
 with a given task. Check out this [example](https://github.com/Lightning-AI/
-lightning-flash/blob/master/flash_examples/integrations/learn2learn/
+lightning-flash/blob/master/examples/integrations/learn2learn/
 image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4
 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/
 meta-learning.html) from [Learn2Learn](https://github.com/learnables/
 learn2learn). This is particularly useful if you use this model in production
 and want to make sure the model adapts quickly to its new environment with
-minimal labelled data. ```py model = ImageClassifier( backbone="resnet18",
-optimizer=torch.optim.Adam, optimizer_kwargs={"lr": 0.001},
-training_strategy="prototypicalnetworks", training_strategy_kwargs=
-{ "epoch_length": 10 * 16, "meta_batch_size": 4, "num_tasks": 200,
-"test_num_tasks": 2000, "ways": datamodule.num_classes, "shots": 1,
-"test_ways": 5, "test_shots": 1, "test_queries": 15, }, ) ``` In detail, the
-following methods are currently implemented: * **[prototypicalnetworks](https:/
-/github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/
-lightning/lightning_protonet.py)** : from Snell *et al.* 2017, [Prototypical
-Networks for Few-shot Learning](https://arxiv.org/abs/1703.05175) * **[maml]
-(https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/
-lightning/lightning_maml.py)** : from Finn *et al.* 2017, [Model-Agnostic Meta-
-Learning for Fast Adaptation of Deep Networks](https://arxiv.org/abs/
-1703.03400) * **[metaoptnet](https://github.com/learnables/learn2learn/blob/
-master/learn2learn/algorithms/lightning/lightning_metaoptnet.py)** : from Lee
-*et al.* 2019, [Meta-Learning with Differentiable Convex Optimization](https://
-arxiv.org/abs/1904.03758) * **[anil](https://github.com/learnables/learn2learn/
-blob/master/learn2learn/algorithms/lightning/lightning_anil.py)** : from Raghu
-*et al.* 2020, [Rapid Learning or Feature Reuse? Towards Understanding the
-Effectiveness of MAML](https://arxiv.org/abs/1909.09157) ### Flash Optimizers /
-Schedulers With Flash, swapping among 40+ optimizers and 15 + schedulers
-recipes are simple. Find the list of available optimizers, schedulers as
-follows: ```py ImageClassifier.available_optimizers() # ['A2GradExp', ...,
-'Yogi'] ImageClassifier.available_schedulers() # ['CosineAnnealingLR',
-'CosineAnnealingWarmRestarts', ..., 'polynomial_decay_schedule_with_warmup']
-``` Once you've chosen, create the model: ```py #### The optimizer of choice
-can be passed as a # - String value model = ImageClassifier
+minimal labelled data. ```py from flash.image import ImageClassifier model =
+ImageClassifier( backbone="resnet18", optimizer=torch.optim.Adam,
+optimizer_kwargs={"lr": 0.001}, training_strategy="prototypicalnetworks",
+training_strategy_kwargs={ "epoch_length": 10 * 16, "meta_batch_size": 4,
+"num_tasks": 200, "test_num_tasks": 2000, "ways": datamodule.num_classes,
+"shots": 1, "test_ways": 5, "test_shots": 1, "test_queries": 15, }, ) ``` In
+detail, the following methods are currently implemented: * **
+[prototypicalnetworks](https://github.com/learnables/learn2learn/blob/master/
+learn2learn/algorithms/lightning/lightning_protonet.py)** : from Snell *et al.*
+2017, [Prototypical Networks for Few-shot Learning](https://arxiv.org/abs/
+1703.05175) * **[maml](https://github.com/learnables/learn2learn/blob/master/
+learn2learn/algorithms/lightning/lightning_maml.py)** : from Finn *et al.*
+2017, [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks]
+(https://arxiv.org/abs/1703.03400) * **[metaoptnet](https://github.com/
+learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/
+lightning_metaoptnet.py)** : from Lee *et al.* 2019, [Meta-Learning with
+Differentiable Convex Optimization](https://arxiv.org/abs/1904.03758) * **
+[anil](https://github.com/learnables/learn2learn/blob/master/learn2learn/
+algorithms/lightning/lightning_anil.py)** : from Raghu *et al.* 2020, [Rapid
+Learning or Feature Reuse? Towards Understanding the Effectiveness of MAML]
+(https://arxiv.org/abs/1909.09157) ### Flash Optimizers / Schedulers With
+Flash, swapping among 40+ optimizers and 15+ schedulers recipes are simple.
+Find the list of available optimizers, schedulers as follows: ```py from
+flash.image import ImageClassifier ImageClassifier.available_optimizers() #
+['A2GradExp', ..., 'Yogi'] ImageClassifier.available_schedulers() #
+['CosineAnnealingLR', 'CosineAnnealingWarmRestarts', ...,
+'polynomial_decay_schedule_with_warmup'] ``` Once you've chosen, create the
+model: ```py #### The optimizer of choice can be passed as from flash.image
+import ImageClassifier # - String value model = ImageClassifier
 (backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=None) # -
 Callable model = ImageClassifier(backbone="resnet18", num_classes=2,
 optimizer=functools.partial(torch.optim.Adadelta, eps=0.5), lr_scheduler=None)
 # - Tuple[string, dict]: (The dict takes in the optimizer kwargs) model =
 ImageClassifier(backbone="resnet18", num_classes=2, optimizer=("Adadelta",
 {"epa": 0.5}), lr_scheduler=None) #### The scheduler of choice can be passed as
 a # - String value model = ImageClassifier(backbone="resnet18", num_classes=2,
 optimizer="Adam", lr_scheduler="constant_schedule") # - Callable model =
 ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
 lr_scheduler=functools.partial(CyclicLR, step_size_up=1500, mode='exp_range',
 gamma=0.5)) # - Tuple[string, dict]: (The dict takes in the scheduler kwargs)
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
 lr_scheduler=("StepLR", {"step_size": 10})) ``` You can also register you own
-custom scheduler recipes beforeahand and use them shown as above: ```py
-@ImageClassifier.lr_schedulers_registry def my_steplr_recipe(optimizer): return
-torch.optim.lr_scheduler.StepLR(optimizer, step_size=10) model =
-ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
-lr_scheduler="my_steplr_recipe") ``` ### Flash Transforms Flash includes some
-simple augmentations for each task by default, however, you will often want to
-override these and control your own augmentation recipe. To this end, Flash
-supports custom transformations with the [`InputTransform`](https://lightning-
-flash.readthedocs.io/en/stable/api/generated/
+custom scheduler recipes beforeahand and use them shown as above: ```py from
+flash.image import ImageClassifier @ImageClassifier.lr_schedulers_registry def
+my_steplr_recipe(optimizer): return torch.optim.lr_scheduler.StepLR(optimizer,
+step_size=10) model = ImageClassifier(backbone="resnet18", num_classes=2,
+optimizer="Adam", lr_scheduler="my_steplr_recipe") ``` ### Flash Transforms
+Flash includes some simple augmentations for each task by default, however, you
+will often want to override these and control your own augmentation recipe. To
+this end, Flash supports custom transformations with the [`InputTransform`]
+(https://lightning-flash.readthedocs.io/en/stable/api/generated/
 flash.core.data.io.input_transform.InputTransform.html). The `InputTransform`
 is like a callback for transforms, with hooks that can be used to apply
 transforms to samples or batches, on and off the device / accelerator. In
 addition, hooks can be specialized to apply transforms only to the input or
 target. With these hooks, complex transforms like MixUp can be implemented with
 ease. Here's an example (with an albumentations transform thrown in too!):
 ```py import torch import numpy as np import albumentations from flash import
@@ -143,21 +156,22 @@
 batch class MixUpInputTransform(InputTransform): def
 train_input_per_sample_transform(self): return AlbumentationsAdapter
 (albumentations.HorizontalFlip(p=0.5)) # This will be applied after
 transferring the batch to the device! def train_per_batch_transform_on_device
 (self): return mixup datamodule = ImageClassificationData.from_folders
 ( train_folder="data/train", transform=MixUpInputTransform, batch_size=2, ) ```
 ## Flash Zero - PyTorch Recipes from the Command Line!
-             [/docs/source/_static/images/flash_zero.gif?raw=true]
+   [/https://github.com/Lightning-AI/lightning-flash/raw/0.8.2/docs/source/
+                    _static/images/flash_zero.gif?raw=true]
 Flash Zero is a zero-code machine learning platform built directly into
 lightning-flash using the [`Lightning CLI`](https://pytorch-
-lightning.readthedocs.io/en/stable/common/lightning_cli.html). To get started
-and view the available tasks, run: ```py flash --help ``` For example, to train
+lightning.readthedocs.io/en/0.8.2common/lightning_cli.html). To get started and
+view the available tasks, run: ```bash flash --help ``` For example, to train
 an image classifier for 10 epochs with a `resnet50` backbone on 2 GPUs using
-your own data, you can do: ```py flash image_classification --
+your own data, you can do: ```bash flash image_classification --
 trainer.max_epochs 10 --trainer.gpus 2 --model.backbone resnet50 from_folders -
 -train_folder {PATH_TO_DATA} ``` ## Kaggle Notebook Examples - [ð¢Titanic
 crash with Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/titanic-
 crash-with-lightning-flash) - [ð House ðµprices predictions with
 Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/house-prices-
 predictions-with-lightning-flash) - [Playing ðtabular with
 Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/playing-tabular-with-
```

### Comparing `lightning-flash-0.8.1.post0/flash/__about__.py` & `lightning-flash-0.8.2/src/flash/__about__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-__version__ = "0.8.1.post0"
+__version__ = "0.8.2"
 __author__ = "PyTorchLightning et al."
 __author_email__ = "name@pytorchlightning.ai"
 __license__ = "Apache-2.0"
-__copyright__ = f"Copyright (c) 2020-2022, {__author__}."
+__copyright__ = f"Copyright (c) 2020-2023, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/lightning-flash"
 __docs_url__ = "https://lightning-flash.readthedocs.io/en/stable/"
 __docs__ = "Your PyTorch AI Factory - Flash enables you to easily configure and run complex AI recipes."
 __long_doc__ = """
 Flash makes complex AI recipes for over 15 tasks across 7 data domains accessible to all.
 In a nutshell, Flash is the production grade research framework you always dreamed of but didn't have time to build.
 """
```

### Comparing `lightning-flash-0.8.1.post0/flash/__init__.py` & `lightning-flash-0.8.2/src/flash/image/style_transfer/input_transform.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,47 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Root package info."""
-import os
+from dataclasses import dataclass
+from typing import Callable
 
-from flash.__about__ import *  # noqa: F401 F403
-from flash.core.utilities.imports import _TORCH_AVAILABLE
-
-if _TORCH_AVAILABLE:
-
-    from flash.core.data.callback import FlashCallback
-    from flash.core.data.data_module import DataModule
-    from flash.core.data.io.input import DataKeys, Input
-    from flash.core.data.io.input_transform import InputTransform
-    from flash.core.data.io.output import Output
-    from flash.core.data.io.output_transform import OutputTransform
-    from flash.core.model import Task
-    from flash.core.trainer import Trainer
-    from flash.core.utilities.stages import RunningStage
-
-    _PACKAGE_ROOT = os.path.dirname(__file__)
-    ASSETS_ROOT = os.path.join(_PACKAGE_ROOT, "assets")
-    PROJECT_ROOT = os.path.dirname(_PACKAGE_ROOT)
-    _IS_TESTING = os.getenv("FLASH_TESTING", "0") == "1"
-
-    if _IS_TESTING:
-        from pytorch_lightning import seed_everything
-
-        seed_everything(42)
-
-    __all__ = [
-        "DataKeys",
-        "DataModule",
-        "FlashCallback",
-        "Input",
-        "InputTransform",
-        "Output",
-        "OutputTransform",
-        "RunningStage",
-        "Task",
-        "Trainer",
-    ]
+from flash.core.data.io.input import DataKeys
+from flash.core.data.io.input_transform import InputTransform
+from flash.core.data.transforms import ApplyToKeys
+from flash.core.utilities.imports import _TORCHVISION_AVAILABLE
+
+if _TORCHVISION_AVAILABLE:
+    from torchvision import transforms as T
+
+
+@dataclass
+class StyleTransferInputTransform(InputTransform):
+    image_size: int = 256
+
+    def per_sample_transform(self) -> Callable:
+        return ApplyToKeys(
+            DataKeys.INPUT, T.Compose([T.ToTensor(), T.Resize(self.image_size), T.CenterCrop(self.image_size)])
+        )
```

### Comparing `lightning-flash-0.8.1.post0/flash/__main__.py` & `lightning-flash-0.8.2/src/flash/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 def main():
     """The Lightning-Flash zero-code command line utility."""
 
 
 def register_command(command):
     @main.command(
         command.__name__,
-        context_settings=dict(
-            help_option_names=[],
-            ignore_unknown_options=True,
-        ),
+        context_settings={
+            "help_option_names": [],
+            "ignore_unknown_options": True,
+        },
     )
     @click.argument("cli_args", nargs=-1, type=click.UNPROCESSED)
     @functools.wraps(command)
     def wrapper(cli_args):
         with patch("sys.argv", [command.__name__] + list(cli_args)):
             command()
```

### Comparing `lightning-flash-0.8.1.post0/flash/assets/fish.jpg` & `lightning-flash-0.8.2/src/flash/assets/fish.jpg`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/assets/road.png` & `lightning-flash-0.8.2/src/flash/assets/road.png`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/assets/starry_night.jpg` & `lightning-flash-0.8.2/src/flash/assets/starry_night.jpg`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/audio/classification/cli.py` & `lightning-flash-0.8.2/src/flash/audio/classification/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/audio/classification/data.py` & `lightning-flash-0.8.2/src/flash/audio/classification/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,26 @@
 from flash.audio.classification.input_transform import AudioClassificationInputTransform
 from flash.core.data.callback import BaseDataFetcher
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import INPUT_TRANSFORM_TYPE
 from flash.core.data.utilities.classification import TargetFormatter
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.utilities.imports import _AUDIO_TESTING
+from flash.core.utilities.imports import _TOPIC_AUDIO_AVAILABLE, _TOPIC_IMAGE_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.image.classification.data import MatplotlibVisualization
 
 # Skip doctests if requirements aren't available
-if not _AUDIO_TESTING:
+if not _TOPIC_AUDIO_AVAILABLE or not _TOPIC_IMAGE_AVAILABLE:
     __doctest_skip__ = ["AudioClassificationData", "AudioClassificationData.*"]
 
 
 class AudioClassificationData(DataModule):
     """The ``AudioClassificationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
-    classmethods for loading data for audio classification."""
+    class methods for loading data for audio classification."""
 
     input_transform_cls = AudioClassificationInputTransform
 
     @classmethod
     def from_files(
         cls,
         train_files: Optional[Sequence[str]] = None,
@@ -139,19 +139,19 @@
         .. testcleanup::
 
             >>> import os
             >>> _ = [os.remove(f"spectrogram_{i}.png") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_spectrogram_{i}.png") for i in range(1, 4)]
         """
 
-        ds_kw = dict(
-            sampling_rate=sampling_rate,
-            n_fft=n_fft,
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "sampling_rate": sampling_rate,
+            "n_fft": n_fft,
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_files, train_targets, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_files, val_targets, **ds_kw),
@@ -273,19 +273,19 @@
         .. testcleanup::
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
         """
 
-        ds_kw = dict(
-            sampling_rate=sampling_rate,
-            n_fft=n_fft,
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "sampling_rate": sampling_rate,
+            "n_fft": n_fft,
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_folder, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_folder, **ds_kw),
@@ -308,16 +308,16 @@
         predict_data: Optional[Collection[np.ndarray]] = None,
         input_cls: Type[Input] = AudioClassificationNumpyInput,
         transform: INPUT_TRANSFORM_TYPE = AudioClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         target_formatter: Optional[TargetFormatter] = None,
         **data_module_kwargs: Any,
     ) -> "AudioClassificationData":
-        """Load the :class:`~flash.audio.classification.data.AudioClassificationData` from numpy arrays (or lists
-        of arrays) and corresponding lists of targets.
+        """Load the :class:`~flash.audio.classification.data.AudioClassificationData` from numpy arrays (or lists of
+        arrays) and corresponding lists of targets.
 
         The targets can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -363,17 +363,17 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
@@ -396,16 +396,16 @@
         predict_data: Optional[Collection[Tensor]] = None,
         input_cls: Type[Input] = AudioClassificationTensorInput,
         transform: INPUT_TRANSFORM_TYPE = AudioClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         target_formatter: Optional[TargetFormatter] = None,
         **data_module_kwargs: Any,
     ) -> "AudioClassificationData":
-        """Load the :class:`~flash.audio.classification.data.AudioClassificationData` from torch tensors (or lists
-        of tensors) and corresponding lists of targets.
+        """Load the :class:`~flash.audio.classification.data.AudioClassificationData` from torch tensors (or lists of
+        tensors) and corresponding lists of targets.
 
         The targets can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -451,17 +451,17 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
@@ -605,19 +605,19 @@
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> del train_data_frame
             >>> del predict_data_frame
         """
 
-        ds_kw = dict(
-            sampling_rate=sampling_rate,
-            n_fft=n_fft,
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "sampling_rate": sampling_rate,
+            "n_fft": n_fft,
+            "target_formatter": target_formatter,
+        }
 
         train_data = (train_data_frame, input_field, target_fields, train_images_root, train_resolver)
         val_data = (val_data_frame, input_field, target_fields, val_images_root, val_resolver)
         test_data = (test_data_frame, input_field, target_fields, test_images_root, test_resolver)
         predict_data = (predict_data_frame, input_field, None, predict_images_root, predict_resolver)
 
         train_input = input_cls(RunningStage.TRAINING, *train_data, **ds_kw)
@@ -852,19 +852,19 @@
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
 
-        ds_kw = dict(
-            sampling_rate=sampling_rate,
-            n_fft=n_fft,
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "sampling_rate": sampling_rate,
+            "n_fft": n_fft,
+            "target_formatter": target_formatter,
+        }
 
         train_data = (train_file, input_field, target_fields, train_images_root, train_resolver)
         val_data = (val_file, input_field, target_fields, val_images_root, val_resolver)
         test_data = (test_file, input_field, target_fields, test_images_root, test_resolver)
         predict_data = (predict_file, input_field, None, predict_images_root, predict_resolver)
 
         train_input = input_cls(RunningStage.TRAINING, *train_data, **ds_kw)
```

### Comparing `lightning-flash-0.8.1.post0/flash/audio/classification/input.py` & `lightning-flash-0.8.2/src/flash/audio/classification/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 from flash.core.data.io.classification_input import ClassificationInputMixin
 from flash.core.data.io.input import DataKeys, Input
 from flash.core.data.utilities.classification import MultiBinaryTargetFormatter, TargetFormatter
 from flash.core.data.utilities.data_frame import resolve_files, resolve_targets
 from flash.core.data.utilities.loading import (
     AUDIO_EXTENSIONS,
     IMG_EXTENSIONS,
+    NP_EXTENSIONS,
     load_data_frame,
     load_spectrogram,
-    NP_EXTENSIONS,
 )
-from flash.core.data.utilities.paths import filter_valid_files, make_dataset, PATH_TYPE
+from flash.core.data.utilities.paths import PATH_TYPE, filter_valid_files, make_dataset
 from flash.core.data.utilities.samples import to_samples
 from flash.core.utilities.imports import requires
 
 
 class AudioClassificationInput(Input, ClassificationInputMixin):
     @requires("audio")
     def load_sample(self, sample: Dict[str, Any]) -> Dict[str, Any]:
@@ -126,18 +126,15 @@
         root: Optional[PATH_TYPE] = None,
         resolver: Optional[Callable[[Optional[PATH_TYPE], Any], PATH_TYPE]] = None,
         sampling_rate: int = 16000,
         n_fft: int = 400,
         target_formatter: Optional[TargetFormatter] = None,
     ) -> List[Dict[str, Any]]:
         files = resolve_files(data_frame, input_key, root, resolver)
-        if target_keys is not None:
-            targets = resolve_targets(data_frame, target_keys)
-        else:
-            targets = None
+        targets = resolve_targets(data_frame, target_keys) if target_keys is not None else None
         result = super().load_data(
             files, targets, sampling_rate=sampling_rate, n_fft=n_fft, target_formatter=target_formatter
         )
 
         # If we had binary multi-class targets then we also know the labels (column names)
         if (
             self.training
```

### Comparing `lightning-flash-0.8.1.post0/flash/audio/classification/input_transform.py` & `lightning-flash-0.8.2/src/flash/audio/classification/input_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 if _TORCHAUDIO_AVAILABLE:
     from torchaudio import transforms as TAudio
 
 
 @dataclass
 class AudioClassificationInputTransform(InputTransform):
-
     spectrogram_size: Tuple[int, int] = (128, 128)
     time_mask_param: Optional[int] = None
     freq_mask_param: Optional[int] = None
 
     def train_per_sample_transform(self) -> Callable:
         transforms = []
         if self.time_mask_param is not None:
```

### Comparing `lightning-flash-0.8.1.post0/flash/audio/speech_recognition/__init__.py` & `lightning-flash-0.8.2/src/flash/audio/speech_recognition/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/audio/speech_recognition/backbone.py` & `lightning-flash-0.8.2/src/flash/audio/speech_recognition/backbone.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from functools import partial
 
 from flash.core.registry import ExternalRegistry, FlashRegistry
-from flash.core.utilities.imports import _AUDIO_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_AUDIO_AVAILABLE
 from flash.core.utilities.providers import _FAIRSEQ, _HUGGINGFACE
 
 SPEECH_RECOGNITION_BACKBONES = FlashRegistry("backbones")
 
-if _AUDIO_AVAILABLE:
+if _TOPIC_AUDIO_AVAILABLE:
     from transformers import AutoModelForCTC, Wav2Vec2ForCTC
 
     WAV2VEC_MODELS = ["facebook/wav2vec2-base-960h", "facebook/wav2vec2-large-960h-lv60"]
 
     for model_name in WAV2VEC_MODELS:
         SPEECH_RECOGNITION_BACKBONES(
             fn=partial(Wav2Vec2ForCTC.from_pretrained, model_name),
```

### Comparing `lightning-flash-0.8.1.post0/flash/audio/speech_recognition/cli.py` & `lightning-flash-0.8.2/src/flash/audio/speech_recognition/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/audio/speech_recognition/collate.py` & `lightning-flash-0.8.2/src/flash/audio/speech_recognition/collate.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Union
 
 from torch import Tensor
 
 from flash.core.data.io.input import DataKeys
-from flash.core.utilities.imports import _AUDIO_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_AUDIO_AVAILABLE
 
-if _AUDIO_AVAILABLE:
+if _TOPIC_AUDIO_AVAILABLE:
     from transformers import AutoProcessor
 else:
     AutoProcessor = object
 
 
 @dataclass
 class DataCollatorCTCWithPadding:
```

### Comparing `lightning-flash-0.8.1.post0/flash/audio/speech_recognition/data.py` & `lightning-flash-0.8.2/src/flash/audio/speech_recognition/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     SpeechRecognitionJSONInput,
     SpeechRecognitionPathsInput,
 )
 from flash.audio.speech_recognition.output_transform import SpeechRecognitionOutputTransform
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import INPUT_TRANSFORM_TYPE, InputTransform
-from flash.core.utilities.imports import _AUDIO_TESTING
+from flash.core.utilities.imports import _TOPIC_AUDIO_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 
 # Skip doctests if requirements aren't available
-if not _AUDIO_TESTING:
+if not _TOPIC_AUDIO_AVAILABLE:
     __doctest_skip__ = ["SpeechRecognitionData", "SpeechRecognitionData.*"]
 
 
 class SpeechRecognitionData(DataModule):
     """The ``SpeechRecognitionData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for speech recognition."""
 
@@ -52,16 +52,16 @@
         predict_files: Optional[Sequence[str]] = None,
         sampling_rate: int = 16000,
         input_cls: Type[Input] = SpeechRecognitionPathsInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "SpeechRecognitionData":
-        """Load the :class:`~flash.audio.speech_recognition.data.SpeechRecognitionData` from lists of audio files
-        and corresponding lists of targets.
+        """Load the :class:`~flash.audio.speech_recognition.data.SpeechRecognitionData` from lists of audio files and
+        corresponding lists of targets.
 
         The supported file extensions are: ``.aiff``, ``.au``, ``.avr``, ``.caf``, ``.flac``, ``.mat``, ``.mat4``,
         ``.mat5``, ``.mpc2k``, ``.ogg``, ``.paf``, ``.pvf``, ``.rf64``, ``.ircam``, ``.voc``, ``.w64``,
         ``.wav``, ``.nist``, and ``.wavex``.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
@@ -115,17 +115,15 @@
         .. testcleanup::
 
             >>> import os
             >>> _ = [os.remove(f"speech_{i}.wav") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_speech_{i}.wav") for i in range(1, 4)]
         """
 
-        ds_kw = dict(
-            sampling_rate=sampling_rate,
-        )
+        ds_kw = {"sampling_rate": sampling_rate}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_files, train_targets, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_files, val_targets, **ds_kw),
             input_cls(RunningStage.TESTING, test_files, test_targets, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_files, **ds_kw),
             transform=transform,
@@ -144,16 +142,16 @@
         predict_file: Optional[str] = None,
         sampling_rate: int = 16000,
         input_cls: Type[Input] = SpeechRecognitionCSVInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "SpeechRecognitionData":
-        """Load the :class:`~flash.audio.speech_recognition.data.SpeechRecognitionData` from CSV files containing
-        audio file paths and their corresponding targets.
+        """Load the :class:`~flash.audio.speech_recognition.data.SpeechRecognitionData` from CSV files containing audio
+        file paths and their corresponding targets.
 
         Input audio file paths will be extracted from the ``input_field`` column in the CSV files.
         The supported file extensions are: ``.aiff``, ``.au``, ``.avr``, ``.caf``, ``.flac``, ``.mat``, ``.mat4``,
         ``.mat5``, ``.mpc2k``, ``.ogg``, ``.paf``, ``.pvf``, ``.rf64``, ``.ircam``, ``.voc``, ``.w64``,
         ``.wav``, ``.nist``, and ``.wavex``.
         The targets will be extracted from the ``target_field`` in the CSV files.
         To learn how to customize the transforms applied for each stage, read our
@@ -302,18 +300,15 @@
             >>> import os
             >>> _ = [os.remove(f"speech_{i}.wav") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_speech_{i}.wav") for i in range(1, 4)]
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
 
-        ds_kw = dict(
-            input_key=input_field,
-            sampling_rate=sampling_rate,
-        )
+        ds_kw = {"input_key": input_field, "sampling_rate": sampling_rate}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, target_key=target_field, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, target_key=target_field, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, target_key=target_field, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -333,16 +328,16 @@
         sampling_rate: int = 16000,
         field: Optional[str] = None,
         input_cls: Type[Input] = SpeechRecognitionJSONInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "SpeechRecognitionData":
-        """Load the :class:`~flash.audio.speech_recognition.data.SpeechRecognitionData` from JSON files containing
-        audio file paths and their corresponding targets.
+        """Load the :class:`~flash.audio.speech_recognition.data.SpeechRecognitionData` from JSON files containing audio
+        file paths and their corresponding targets.
 
         Input audio file paths will be extracted from the ``input_field`` field in the JSON files.
         The supported file extensions are: ``.aiff``, ``.au``, ``.avr``, ``.caf``, ``.flac``, ``.mat``, ``.mat4``,
         ``.mat5``, ``.mpc2k``, ``.ogg``, ``.paf``, ``.pvf``, ``.rf64``, ``.ircam``, ``.voc``, ``.w64``,
         ``.wav``, ``.nist``, and ``.wavex``.
         The targets will be extracted from the ``target_field`` field in the JSON files.
         To learn how to customize the transforms applied for each stage, read our
@@ -426,19 +421,15 @@
             >>> import os
             >>> _ = [os.remove(f"speech_{i}.wav") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_speech_{i}.wav") for i in range(1, 4)]
             >>> os.remove("train_data.json")
             >>> os.remove("predict_data.json")
         """
 
-        ds_kw = dict(
-            input_key=input_field,
-            sampling_rate=sampling_rate,
-            field=field,
-        )
+        ds_kw = {"input_key": input_field, "sampling_rate": sampling_rate, "field": field}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, target_key=target_field, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, target_key=target_field, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, target_key=target_field, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -455,16 +446,15 @@
         predict_dataset: Optional[Dataset] = None,
         sampling_rate: int = 16000,
         input_cls: Type[Input] = SpeechRecognitionDatasetInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "SpeechRecognitionData":
-        """Load the :class:`~flash.audio.speech_recognition.data.SpeechRecognitionData` from PyTorch Dataset
-        objects.
+        """Load the :class:`~flash.audio.speech_recognition.data.SpeechRecognitionData` from PyTorch Dataset objects.
 
         The Dataset objects should be one of the following:
 
         * A PyTorch Dataset where the ``__getitem__`` returns a tuple: ``(file_path or , target)``
         * A PyTorch Dataset where the ``__getitem__`` returns a dict: ``{"input": file_path, "target": target}``
 
         The supported file extensions are: ``.aiff``, ``.au``, ``.avr``, ``.caf``, ``.flac``, ``.mat``, ``.mat4``,
@@ -577,17 +567,15 @@
         .. testcleanup::
 
             >>> import os
             >>> _ = [os.remove(f"speech_{i}.wav") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_speech_{i}.wav") for i in range(1, 4)]
         """
 
-        ds_kw = dict(
-            sampling_rate=sampling_rate,
-        )
+        ds_kw = {"sampling_rate": sampling_rate}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_dataset, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_dataset, **ds_kw),
             input_cls(RunningStage.TESTING, test_dataset, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_dataset, **ds_kw),
             transform=transform,
```

### Comparing `lightning-flash-0.8.1.post0/flash/audio/speech_recognition/input.py` & `lightning-flash-0.8.2/src/flash/audio/speech_recognition/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from torch.utils.data import Dataset
 
 import flash
 from flash.core.data.io.input import DataKeys, Input, ServeInput
 from flash.core.data.utilities.loading import AUDIO_EXTENSIONS, load_audio, load_data_frame
 from flash.core.data.utilities.paths import filter_valid_files, list_valid_files
 from flash.core.data.utilities.samples import to_sample, to_samples
-from flash.core.utilities.imports import _AUDIO_AVAILABLE, requires
+from flash.core.utilities.imports import _TOPIC_AUDIO_AVAILABLE, requires
 
-if _AUDIO_AVAILABLE:
+if _TOPIC_AUDIO_AVAILABLE:
     import librosa
     from datasets import Dataset as HFDataset
     from datasets import load_dataset
 else:
     HFDataset = object
```

### Comparing `lightning-flash-0.8.1.post0/flash/audio/speech_recognition/model.py` & `lightning-flash-0.8.2/src/flash/audio/speech_recognition/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 from flash.audio.speech_recognition.output_transform import SpeechRecognitionOutputTransform
 from flash.core.data.io.input import ServeInput
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.io.output import Output
 from flash.core.model import Task
 from flash.core.registry import FlashRegistry
 from flash.core.serve import Composition
-from flash.core.utilities.imports import _AUDIO_AVAILABLE, requires
+from flash.core.utilities.imports import _TOPIC_AUDIO_AVAILABLE, requires
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE, LR_SCHEDULER_TYPE, OPTIMIZER_TYPE
 
-if _AUDIO_AVAILABLE:
+if _TOPIC_AUDIO_AVAILABLE:
     from transformers import AutoProcessor
 
 
 class SpeechRecognition(Task):
     """The ``SpeechRecognition`` task is a :class:`~flash.Task` for converting speech to text. For more details, see
     :ref:`speech_recognition`.
```

### Comparing `lightning-flash-0.8.1.post0/flash/audio/speech_recognition/output_transform.py` & `lightning-flash-0.8.2/src/flash/audio/speech_recognition/output_transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,33 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any
 
 import torch
 
 from flash.core.data.io.output_transform import OutputTransform
-from flash.core.utilities.imports import _AUDIO_AVAILABLE, requires
+from flash.core.utilities.imports import _TOPIC_AUDIO_AVAILABLE, requires
 
-if _AUDIO_AVAILABLE:
+if _TOPIC_AUDIO_AVAILABLE:
     from transformers import Wav2Vec2CTCTokenizer
 
 
 class SpeechRecognitionOutputTransform(OutputTransform):
     def __init__(self, backbone: str):
         super().__init__()
 
         self.backbone = backbone
         self._tokenizer = Wav2Vec2CTCTokenizer.from_pretrained(self.backbone)
 
     @requires("audio")
     def per_batch_transform(self, batch: Any) -> Any:
         # converts logits into greedy transcription
         pred_ids = torch.argmax(batch, dim=-1)
-        transcriptions = self._tokenizer.batch_decode(pred_ids)
-        return transcriptions
+        return self._tokenizer.batch_decode(pred_ids)
 
     def __getstate__(self):  # TODO: Find out why this is being pickled
         state = self.__dict__.copy()
         state.pop("_tokenizer", None)
         return state
 
     def __setstate__(self, state):
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/adapter.py` & `lightning-flash-0.8.2/src/flash/core/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from abc import abstractmethod
 from typing import Any, Callable, Optional
 
 import torch.jit
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.utils.data import DataLoader, Sampler
 
 import flash
 from flash.core.data.io.input import InputBase
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.model import DatasetProcessor, ModuleWrapperBase, Task
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 
 
 class Adapter(DatasetProcessor, ModuleWrapperBase, nn.Module):
-    """The ``Adapter`` is a lightweight interface that can be used to encapsulate the logic from a particular
-    provider within a :class:`~flash.core.model.Task`."""
+    """The ``Adapter`` is a lightweight interface that can be used to encapsulate the logic from a particular provider
+    within a :class:`~flash.core.model.Task`."""
 
     @classmethod
     @abstractmethod
     def from_task(cls, task: "flash.Task", **kwargs) -> "Adapter":
         """Instantiate the adapter from the given :class:`~flash.core.model.Task`.
 
         This includes resolution / creation of backbones / heads and any other provider specific options.
@@ -63,16 +63,16 @@
 
 
 def identity_collate_fn(x):
     return x
 
 
 class AdapterTask(Task):
-    """The ``AdapterTask`` is a :class:`~flash.core.model.Task` which wraps an :class:`~flash.core.adapter.Adapter`
-    and forwards all of the hooks.
+    """The ``AdapterTask`` is a :class:`~flash.core.model.Task` which wraps an :class:`~flash.core.adapter.Adapter` and
+    forwards all of the hooks.
 
     Args:
         adapter: The :class:`~flash.core.adapter.Adapter` to wrap.
         kwargs: Keyword arguments to be passed to the base :class:`~flash.core.model.Task`.
     """
 
     def __init__(self, adapter: Adapter, **kwargs):
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/classification.py` & `lightning-flash-0.8.2/src/flash/core/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,38 +13,33 @@
 # limitations under the License.
 from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Union
 
 import torch
 import torch.nn.functional as F
 from pytorch_lightning.utilities import rank_zero_warn
 from torch import Tensor
-from torchmetrics import Accuracy, Metric
+from torchmetrics import Accuracy, F1Score, Metric
 
 from flash.core.adapter import AdapterTask
 from flash.core.data.io.input import DataKeys
 from flash.core.data.io.output import Output
 from flash.core.model import Task
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, _TM_GREATER_EQUAL_0_7_0, lazy_import, requires
+from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, lazy_import, requires
 from flash.core.utilities.providers import _FIFTYONE
 
 if _FIFTYONE_AVAILABLE:
     fol = lazy_import("fiftyone.core.labels")
     Classification = "fiftyone.core.labels.Classification"
     Classifications = "fiftyone.core.labels.Classifications"
 else:
     fol = None
     Classification = None
     Classifications = None
 
-if _TM_GREATER_EQUAL_0_7_0:
-    from torchmetrics import F1Score
-else:
-    from torchmetrics import F1 as F1Score
-
 
 CLASSIFICATION_OUTPUTS = FlashRegistry("outputs")
 
 
 def binary_cross_entropy_with_logits(x: Tensor, y: Tensor) -> Tensor:
     """Calls BCE with logits and cast the target one_hot (y) encoding to floating point precision."""
     return F.binary_cross_entropy_with_logits(x, y.float())
@@ -60,67 +55,67 @@
         multi_label: bool = False,
     ):
         self.num_classes = num_classes
         self.multi_label = multi_label
         self.labels = labels
 
         if metrics is None:
-            metrics = F1Score(num_classes) if (multi_label and num_classes) else Accuracy()
+            metrics = (
+                F1Score(num_labels=num_classes, task="multilabel", top_k=1)
+                if (multi_label and num_classes)
+                else Accuracy()
+            )
 
         if loss_fn is None:
             loss_fn = binary_cross_entropy_with_logits if multi_label else F.cross_entropy
 
         return metrics, loss_fn
 
     def to_metrics_format(self, x: Tensor) -> Tensor:
         if getattr(self, "multi_label", False):
             return torch.sigmoid(x)
         return torch.softmax(x, dim=1)
 
 
 class ClassificationTask(ClassificationMixin, Task):
-
     outputs: FlashRegistry = Task.outputs + CLASSIFICATION_OUTPUTS
 
     def __init__(
         self,
         *args,
         num_classes: Optional[int] = None,
         loss_fn: Optional[Callable] = None,
         metrics: Union[Metric, Mapping, Sequence, None] = None,
         multi_label: bool = False,
         labels: Optional[List[str]] = None,
         **kwargs,
     ) -> None:
-
         metrics, loss_fn = self._build(num_classes, labels, loss_fn, metrics, multi_label)
 
         super().__init__(
             *args,
             loss_fn=loss_fn,
             metrics=metrics,
             **kwargs,
         )
 
 
 class ClassificationAdapterTask(ClassificationMixin, AdapterTask):
-
     outputs: FlashRegistry = Task.outputs + CLASSIFICATION_OUTPUTS
 
     def __init__(
         self,
         *args,
         num_classes: Optional[int] = None,
         loss_fn: Optional[Callable] = None,
         metrics: Union[Metric, Mapping, Sequence, None] = None,
         multi_label: bool = False,
         labels: Optional[List[str]] = None,
         **kwargs,
     ) -> None:
-
         metrics, loss_fn = self._build(num_classes, labels, loss_fn, metrics, multi_label)
 
         super().__init__(
             *args,
             loss_fn=loss_fn,
             metrics=metrics,
             **kwargs,
@@ -147,16 +142,15 @@
     def multi_label(self) -> bool:
         return self._mutli_label
 
 
 @CLASSIFICATION_OUTPUTS(name="preds")
 class PredsClassificationOutput(ClassificationOutput):
     """A :class:`~flash.core.classification.ClassificationOutput` which gets the
-    :attr:`~flash.core.data.io.input.InputFormat.PREDS` from the sample.
-    """
+    :attr:`~flash.core.data.io.input.InputFormat.PREDS` from the sample."""
 
     def transform(self, sample: Any) -> Any:
         if isinstance(sample, Mapping) and DataKeys.PREDS in sample:
             sample = sample[DataKeys.PREDS]
         if not isinstance(sample, Tensor):
             sample = torch.tensor(sample)
         return sample
@@ -168,28 +162,27 @@
 
     def transform(self, sample: Any) -> Any:
         return super().transform(sample).tolist()
 
 
 @CLASSIFICATION_OUTPUTS(name="probabilities")
 class ProbabilitiesOutput(PredsClassificationOutput):
-    """A :class:`.Output` which applies a softmax to the model outputs (assumed to be logits) and converts to a
-    list."""
+    """A :class:`.Output` which applies a softmax to the model outputs (assumed to be logits) and converts to a list."""
 
     def transform(self, sample: Any) -> Any:
         sample = super().transform(sample)
         if self.multi_label:
             return torch.sigmoid(sample).tolist()
         return torch.softmax(sample, -1).tolist()
 
 
 @CLASSIFICATION_OUTPUTS(name="classes")
 class ClassesOutput(PredsClassificationOutput):
-    """A :class:`.Output` which applies an argmax to the model outputs (either logits or probabilities) and
-    converts to a list.
+    """A :class:`.Output` which applies an argmax to the model outputs (either logits or probabilities) and converts to
+    a list.
 
     Args:
         multi_label: If true, treats outputs as multi label logits.
         threshold: The threshold to use for multi_label classification.
     """
 
     def __init__(self, multi_label: bool = False, threshold: float = 0.5):
@@ -207,16 +200,16 @@
                     result.append(index)
             return result
         return torch.argmax(sample, -1).tolist()
 
 
 @CLASSIFICATION_OUTPUTS(name="labels")
 class LabelsOutput(ClassesOutput):
-    """A :class:`.Output` which converts the model outputs (either logits or probabilities) to the label of the
-    argmax classification.
+    """A :class:`.Output` which converts the model outputs (either logits or probabilities) to the label of the argmax
+    classification.
 
     Args:
         labels: A list of labels, assumed to map the class index to the label for that class.
         multi_label: If true, treats outputs as multi label logits.
         threshold: The threshold to use for multi_label classification.
     """
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/base_viz.py` & `lightning-flash-0.8.2/src/flash/core/data/base_viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Set, Tuple
 
-from lightning_utilities.core.overrides import is_overridden
+from pytorch_lightning.utilities.model_helpers import is_overridden
 
 from flash.core.data.callback import BaseDataFetcher
 from flash.core.data.utils import _CALLBACK_FUNCS
 from flash.core.utilities.stages import RunningStage
 
 
 class BaseVisualization(BaseDataFetcher):
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/batch.py` & `lightning-flash-0.8.2/src/flash/core/data/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Callable, List, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Callable, List
 
-from torch import nn, Tensor
+from torch import Tensor, nn
 
 from flash.core.data.utilities.classification import _is_list_like
 
 if TYPE_CHECKING:
     from flash.core.data.io.input import ServeInput
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/callback.py` & `lightning-flash-0.8.2/src/flash/core/data/callback.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/data_module.py` & `lightning-flash-0.8.2/src/flash/core/data/data_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 from torch.utils.data.sampler import Sampler
 
 import flash
 from flash.core.data.base_viz import BaseVisualization
 from flash.core.data.callback import BaseDataFetcher
 from flash.core.data.io.input import DataKeys, Input, IterableInput
 from flash.core.data.io.input_transform import (
+    InputTransform,
     create_device_input_transform_processor,
     create_or_configure_input_transform,
     create_worker_input_transform_processor,
-    InputTransform,
 )
 from flash.core.data.splits import SplitDataset
 from flash.core.data.utils import _STAGES_PREFIX
-from flash.core.utilities.imports import _CORE_TESTING
+from flash.core.utilities.imports import _TOPIC_CORE_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 
 # Skip doctests if requirements aren't available
-if not _CORE_TESTING:
+if not _TOPIC_CORE_AVAILABLE:
     __doctest_skip__ = ["DataModule"]
 
 
 class DatasetInput(Input):
     """The ``DatasetInput`` implements default behaviours for data sources which expect the input to
     :meth:`~flash.core.data.io.input.Input.load_data` to be a :class:`torch.utils.data.dataset.Dataset`
     """
@@ -99,15 +99,14 @@
     Alternatively, you can pass a sampler instance:
 
     .. doctest::
 
         >>> datamodule = DataModule(train_input, sampler=WeightedRandomSampler([0.1, 0.5], 2), batch_size=1)
         >>> print(datamodule.train_dataloader().sampler)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
         <torch.utils.data.sampler.WeightedRandomSampler object at ...>
-
     """
 
     input_transform_cls = InputTransform
 
     def __init__(
         self,
         train_input: Optional[Input] = None,
@@ -120,15 +119,14 @@
         val_split: Optional[float] = None,
         batch_size: Optional[int] = None,
         num_workers: int = 0,
         sampler: Optional[Union[Callable, Sampler, Type[Sampler]]] = None,
         pin_memory: bool = True,
         persistent_workers: bool = False,
     ) -> None:
-
         if not batch_size:
             raise TypeError("The `batch_size` should be provided to the DataModule on instantiation.")
 
         if flash._IS_TESTING and torch.cuda.is_available():
             batch_size = 16
 
         self.input_transform = create_or_configure_input_transform(
@@ -212,18 +210,15 @@
 
     def _train_dataloader(self) -> DataLoader:
         train_ds: Input = self._train_input
 
         input_transform = self._resolve_input_transform()
 
         shuffle: bool = False
-        if isinstance(train_ds, IterableDataset):
-            drop_last = False
-        else:
-            drop_last = len(train_ds) > self.batch_size
+        drop_last = False if isinstance(train_ds, IterableDataset) else len(train_ds) > self.batch_size
 
         if self.sampler is None:
             sampler = None
             shuffle = not isinstance(train_ds, IterableDataset)
         elif callable(self.sampler):
             sampler = self.sampler(train_ds)
         else:
@@ -459,15 +454,15 @@
         limit_nb_samples: int = None,
         figsize: Tuple[int, int] = (6.4, 4.8),
         reset: bool = True,
     ) -> None:
         """This function is used to handle transforms profiling for batch visualization."""
         # don't show in CI
         if os.getenv("FLASH_TESTING", "0") == "1":
-            return None
+            return
         iter_name = f"_{stage}_iter"
 
         if not hasattr(self, iter_name):
             self._reset_iterator(stage)
 
         # list of functions to visualise
         if isinstance(func_names, str):
@@ -557,16 +552,16 @@
         return self._get_property("multi_label")
 
     @staticmethod
     def _split_train_val(
         train_dataset: Dataset,
         val_split: float,
     ) -> Tuple[Any, Any]:
-        """Utility function for splitting the training dataset into a disjoint subset of training samples and
-        validation samples.
+        """Utility function for splitting the training dataset into a disjoint subset of training samples and validation
+        samples.
 
         Args:
             train_dataset: A instance of a :class:`torch.utils.data.Dataset`.
             val_split: A float between 0 and 1 determining the number fraction of samples that should go into the
                 validation split
 
         Returns:
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/io/classification_input.py` & `lightning-flash-0.8.2/src/flash/core/data/io/classification_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, List, Optional
 
 from flash.core.data.properties import Properties
-from flash.core.data.utilities.classification import get_target_formatter, TargetFormatter
+from flash.core.data.utilities.classification import TargetFormatter, get_target_formatter
 
 
 class ClassificationInputMixin(Properties):
     """The ``ClassificationInputMixin`` class provides utility methods for handling classification targets.
     :class:`~flash.core.data.io.input.Input` objects that extend ``ClassificationInputMixin`` should do the following:
 
     * In the ``load_data`` method, include a call to ``load_target_metadata``. This will determine the format of the
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/io/input.py` & `lightning-flash-0.8.2/src/flash/core/data/io/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,44 +9,40 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
 import os
-import sys
 from enum import Enum
-from typing import Any, cast, Dict, Iterable, List, Sequence, Tuple, Union
+from typing import Any, Dict, Iterable, List, Sequence, Tuple, Union, cast
 
 from pytorch_lightning.utilities.enums import LightningEnum
 from torch.utils.data import Dataset
 
 from flash.core.data.properties import Properties
 from flash.core.data.utils import _STAGES_PREFIX
 from flash.core.utilities.stages import RunningStage
 
-if sys.version_info < (3, 7):
-    from typing import GenericMeta
-else:
-    GenericMeta = type
+GenericMeta = type
 
 
 if not os.environ.get("READTHEDOCS", False):
     from torch.utils.data import IterableDataset
 else:
     # ReadTheDocs mocks the `IterableDataset` import so it's type cannot be used as a base for a metaclass, so we
     # replace it here.
     IterableDataset = object
 
 
 def _deepcopy_dict(nested_dict: Any) -> Any:
     """Utility to deepcopy a nested dict."""
     if not isinstance(nested_dict, Dict):
         return nested_dict
-    return {key: value for key, value in nested_dict.items()}
+    return dict(nested_dict.items())
 
 
 class InputFormat(LightningEnum):
     """The ``InputFormat`` enum contains the data source names used by all of the default ``from_*`` methods in
     :class:`~flash.core.data.data_module.DataModule`."""
 
     FOLDERS = "folders"
@@ -65,16 +61,15 @@
 
     # TODO: Create a FlashEnum class???
     def __hash__(self) -> int:
         return hash(self.value)
 
 
 class DataKeys(LightningEnum):
-    """The ``DataKeys`` enum contains the keys that are used by built-in data sources to refer to inputs and
-    targets."""
+    """The ``DataKeys`` enum contains the keys that are used by built-in data sources to refer to inputs and targets."""
 
     INPUT = "input"
     PREDS = "preds"
     TARGET = "target"
     METADATA = "metadata"
 
     # TODO: Create a FlashEnum class???
@@ -99,28 +94,28 @@
         len(data)
         return True
     except (TypeError, NotImplementedError):
         return False
 
 
 def _validate_input(input: "InputBase") -> None:
-    """Helper function to validate that the type of an ``InputBase.data`` is appropriate for the type of
-    ``InputBase`` being used.
+    """Helper function to validate that the type of an ``InputBase.data`` is appropriate for the type of ``InputBase``
+    being used.
 
     Args:
         input: The ``InputBase`` instance to validate.
 
     Raises:
         RuntimeError: If the ``input`` is of type ``Input`` and it's ``data`` attribute does not support ``len``.
         RuntimeError: If the ``input`` is of type ``IterableInput`` and it's ``data`` attribute does support ``len``.
     """
     if input.data is not None:
         if isinstance(input, Input) and not _has_len(input.data):
             raise RuntimeError("`Input.data` is not a sequence with a defined length. Use `IterableInput` instead.")
-        elif isinstance(input, IterableInput) and _has_len(input.data):
+        if isinstance(input, IterableInput) and _has_len(input.data):
             raise RuntimeError("`IterableInput.data` is a sequence with a defined length. Use `Input` instead.")
 
 
 def _wrap_init(class_dict: Dict[str, Any]) -> None:
     """Helper function to wrap the ``__init__`` (if present) from a class construction dict to apply the
     ``_validate_input`` function after instantiation. Modifies the dict inplace.
 
@@ -164,15 +159,14 @@
     Args:
         running_stage: The running stage for which the input will be used.
         *args: Any arguments that are to be passed to the ``load_data`` hook.
         **kwargs: Any additional keyword arguments to pass to the ``load_data`` hook.
     """
 
     def __init__(self, running_stage: RunningStage, *args: Any, **kwargs: Any) -> None:
-
         super().__init__(running_stage=running_stage)
 
         self.data = None
         if len(args) >= 1 and args[0] is not None:
             self.data = getattr(self, f"{_STAGES_PREFIX[running_stage]}_load_data")(*args, **kwargs)
 
     def _call_load_sample(self, sample: Any) -> Any:
@@ -188,17 +182,17 @@
                 else:
                     output_dict[key] = val
             return output_dict
         return sample_output
 
     @staticmethod
     def load_data(*args: Any, **kwargs: Any) -> Union[Sequence, Iterable]:
-        """The ``load_data`` hook should return a collection of samples. To reduce the memory footprint, these
-        samples should typically not have been loaded. For example, an input which loads images from disk would
-        only return the list of filenames here rather than the loaded images.
+        """The ``load_data`` hook should return a collection of samples. To reduce the memory footprint, these samples
+        should typically not have been loaded. For example, an input which loads images from disk would only return the
+        list of filenames here rather than the loaded images.
 
         Args:
             *args: Any arguments that the input requires.
             **kwargs: Any additional keyword arguments that the input requires.
         """
         return args[0]
 
@@ -236,16 +230,16 @@
             *args: Any arguments that the input requires.
             **kwargs: Any additional keyword arguments that the input requires.
         """
         return self.load_data(*args, **kwargs)
 
     @staticmethod
     def load_sample(sample: Dict[str, Any]) -> Any:
-        """The ``load_sample`` hook is called for each ``__getitem__`` or ``__next__`` call to the dataset with a
-        single sample from the output of the ``load_data`` hook as input.
+        """The ``load_sample`` hook is called for each ``__getitem__`` or ``__next__`` call to the dataset with a single
+        sample from the output of the ``load_data`` hook as input.
 
         Args:
             sample: A single sample from the output of the ``load_data`` hook.
         """
         return sample
 
     def train_load_sample(self, sample: Dict[str, Any]) -> Any:
@@ -269,16 +263,15 @@
 
         Args:
             sample: A single sample from the output of the ``load_data`` hook.
         """
         return self.load_sample(sample)
 
     def predict_load_sample(self, sample: Dict[str, Any]) -> Any:
-        """Override the ``predict_load_sample`` hook with data loading logic that is only required during
-        predicting.
+        """Override the ``predict_load_sample`` hook with data loading logic that is only required during predicting.
 
         Args:
             sample: A single sample from the output of the ``load_data`` hook.
         """
         return self.load_sample(sample)
 
     def __bool__(self):
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/io/input_transform.py` & `lightning-flash-0.8.2/src/flash/core/data/io/input_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from flash.core.data.utilities.collate import default_collate
 from flash.core.data.utils import _STAGES_PREFIX
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 
 
 class InputTransformPlacement(LightningEnum):
-
     PER_SAMPLE_TRANSFORM = "per_sample_transform"
     PER_BATCH_TRANSFORM = "per_batch_transform"
     COLLATE = "collate"
     PER_SAMPLE_TRANSFORM_ON_DEVICE = "per_sample_transform_on_device"
     PER_BATCH_TRANSFORM_ON_DEVICE = "per_batch_transform_on_device"
 
 
@@ -80,15 +79,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_sample_transform(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         pass
 
     def train_per_sample_transform(self) -> Callable:
         """Defines the transform to be applied on a single sample on cpu for the training stage.
 
@@ -118,15 +116,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_sample_transform(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_sample_transform()
 
     def test_per_sample_transform(self) -> Callable:
         """Defines the transform to be applied on a single sample on cpu for the testing stage.
 
@@ -156,15 +153,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_sample_transform(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_sample_transform()
 
     def serve_per_sample_transform(self) -> Callable:
         """Defines the transform to be applied on a single sample on cpu for the serving stage.
 
@@ -181,15 +177,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_sample_transform(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_sample_transform()
 
     ##################################
     # PER SAMPLE TRANSFORM ON DEVICE #
     ##################################
@@ -210,15 +205,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_sample_transform_on_device(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         pass
 
     def train_per_sample_transform_on_device(self) -> Callable:
         """Defines the transform to be applied on a single sample on device for the training stage.
 
@@ -248,15 +242,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_sample_transform_on_device(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_sample_transform_on_device()
 
     def test_per_sample_transform_on_device(self) -> Callable:
         """Defines the transform to be applied on a single sample on device for the testing stage.
 
@@ -286,15 +279,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_sample_transform_on_device(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_sample_transform_on_device()
 
     def serve_per_sample_transform_on_device(self) -> Callable:
         """Defines the transform to be applied on a single sample on device for the serving stage.
 
@@ -311,15 +303,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def serve_per_sample_transform_on_device(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_sample_transform_on_device()
 
     #######################
     # PER BATCH TRANSFORM #
     #######################
@@ -340,15 +331,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_batch_transform(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         pass
 
     def train_per_batch_transform(self) -> Callable:
         """Defines the transform to be applied on a batch of data on cpu for the training stage.
 
@@ -378,15 +368,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_batch_transform(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_batch_transform()
 
     def test_per_batch_transform(self) -> Callable:
         """Defines the transform to be applied on a batch of data on cpu for the testing stage.
 
@@ -416,15 +405,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_batch_transform(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_batch_transform()
 
     def serve_per_batch_transform(self) -> Callable:
         """Defines the transform to be applied on a batch of data on cpu for the serving stage.
 
@@ -441,15 +429,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_batch_transform(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_batch_transform()
 
     #################################
     # PER BATCH TRANSFORM ON DEVICE #
     #################################
@@ -470,15 +457,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_batch_transform_on_device(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         pass
 
     def train_per_batch_transform_on_device(self) -> Callable:
         """Defines the transform to be applied on a batch of data on device for the training stage.
 
@@ -508,15 +494,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_batch_transform_on_device(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_batch_transform_on_device()
 
     def test_per_batch_transform_on_device(self) -> Callable:
         """Defines the transform to be applied on a batch of data on device for the testing stage.
 
@@ -546,15 +531,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def per_batch_transform_on_device(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_batch_transform_on_device()
 
     def serve_per_batch_transform_on_device(self) -> Callable:
         """Defines the transform to be applied on a batch of data on device for the serving stage.
 
@@ -571,15 +555,14 @@
         .. code-block:: python
 
             from flash.core.data.transforms import ApplyToKeys
 
 
             class MyInputTransform(InputTransform):
                 def serve_per_batch_transform_on_device(self) -> Callable:
-
                     return ApplyToKeys("input", my_func)
         """
         return self.per_batch_transform_on_device()
 
     ###########
     # COLLATE #
     ###########
@@ -674,15 +657,14 @@
 
     def __resolve_transforms(self, running_stage: RunningStage) -> Optional[Dict[str, Callable]]:
         transforms = {}
         stage = _STAGES_PREFIX[running_stage]
 
         # iterate over all transforms hook name
         for transform_name in InputTransformPlacement:
-
             transform_name = transform_name.value
 
             method_name = f"{stage}_{transform_name}"
 
             # get associated transform
             try:
                 fn = getattr(self, method_name)()
@@ -723,15 +705,14 @@
         return f"{self.__class__.__name__}(" + f"transform={self._transform})"
 
 
 def create_or_configure_input_transform(
     transform: INPUT_TRANSFORM_TYPE,
     transform_kwargs: Optional[Dict] = None,
 ) -> Optional[InputTransform]:
-
     if not transform_kwargs:
         transform_kwargs = {}
 
     if isinstance(transform, InputTransform):
         return transform
 
     if inspect.isclass(transform) and issubclass(transform, InputTransform):
@@ -789,18 +770,15 @@
 
     def __call__(self, samples: Sequence[Any]) -> Any:
         if not self.on_device:
             for sample in samples:
                 self.callback.on_load_sample(sample, self.stage)
 
         if self.apply_per_sample_transform:
-            if not isinstance(samples, list):
-                list_samples = [samples]
-            else:
-                list_samples = samples
+            list_samples = [samples] if not isinstance(samples, list) else samples
 
             transformed_samples = [self.per_sample_transform(sample, self.stage) for sample in list_samples]
 
             for sample in transformed_samples:
                 if self.on_device:
                     self.callback.on_per_sample_transform_on_device(sample, self.stage)
                 else:
@@ -828,63 +806,60 @@
             f"\t(apply_per_sample_transform): {str(self.apply_per_sample_transform)}\n"
             f"\t(on_device): {str(self.on_device)}\n"
             f"\t(stage): {str(self.stage)}"
         )
 
 
 def __make_collates(input_transform: InputTransform, on_device: bool, collate: Callable) -> Tuple[Callable, Callable]:
-    """Returns the appropriate collate functions based on whether the transforms happen in a DataLoader worker or
-    on the device (main process)."""
+    """Returns the appropriate collate functions based on whether the transforms happen in a DataLoader worker or on the
+    device (main process)."""
     if on_device:
         return input_transform._identity, collate
     return collate, input_transform._identity
 
 
 def __configure_worker_and_device_collate_fn(
     running_stage: RunningStage, input_transform: InputTransform
 ) -> Tuple[Callable, Callable]:
-
     transform_for_stage: _InputTransformPerStage = input_transform._transform[running_stage]
 
     worker_collate_fn, device_collate_fn = __make_collates(
         input_transform, not transform_for_stage.collate_in_worker, input_transform._collate
     )
 
     return worker_collate_fn, device_collate_fn
 
 
 def create_worker_input_transform_processor(
     running_stage: RunningStage, input_transform: InputTransform
 ) -> _InputTransformProcessor:
-    """This utility is used to create the 2 `_InputTransformProcessor` objects which contain the transforms used as
-    the DataLoader `collate_fn`."""
+    """This utility is used to create the 2 `_InputTransformProcessor` objects which contain the transforms used as the
+    DataLoader `collate_fn`."""
     worker_collate_fn, _ = __configure_worker_and_device_collate_fn(
         running_stage=running_stage, input_transform=input_transform
     )
-    worker_input_transform_processor = _InputTransformProcessor(
+    return _InputTransformProcessor(
         input_transform,
         worker_collate_fn,
         input_transform._per_sample_transform,
         input_transform._per_batch_transform,
         running_stage,
     )
-    return worker_input_transform_processor
 
 
 def create_device_input_transform_processor(
     running_stage: RunningStage, input_transform: InputTransform
 ) -> _InputTransformProcessor:
     """This utility is used to create a `_InputTransformProcessor` object which contain the transforms used as the
     DataModule `on_after_batch_transfer` hook."""
     _, device_collate_fn = __configure_worker_and_device_collate_fn(
         running_stage=running_stage, input_transform=input_transform
     )
-    device_input_transform_processor = _InputTransformProcessor(
+    return _InputTransformProcessor(
         input_transform,
         device_collate_fn,
         input_transform._per_sample_transform_on_device,
         input_transform._per_batch_transform_on_device,
         running_stage,
         apply_per_sample_transform=device_collate_fn != input_transform._identity,
         on_device=True,
     )
-    return device_input_transform_processor
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/io/output.py` & `lightning-flash-0.8.2/src/flash/core/data/io/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from typing import Any
 
 import flash
 from flash.core.data.properties import Properties
 
 
 class Output(Properties):
-    """An :class:`.Output` encapsulates a single :meth:`~flash.core.data.io.output.Output.transform` method which
-    is used to convert the model output into the desired output format when predicting."""
+    """An :class:`.Output` encapsulates a single :meth:`~flash.core.data.io.output.Output.transform` method which is
+    used to convert the model output into the desired output format when predicting."""
 
     @classmethod
     @abstractmethod
     def from_task(cls, task: "flash.Task", **kwargs) -> "Output":
         """Instantiate the output from the given :class:`~flash.core.model.Task`."""
         return cls()
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/io/output_transform.py` & `lightning-flash-0.8.2/src/flash/core/data/io/output_transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 from typing import Any, Sequence
 
 from flash.core.data.batch import default_uncollate
 
 
 class OutputTransform:
-    """The :class:`~flash.core.data.io.output_transform.OutputTransform` encapsulates all the data processing logic
-    that should run after the model."""
+    """The :class:`~flash.core.data.io.output_transform.OutputTransform` encapsulates all the data processing logic that
+    should run after the model."""
 
     @staticmethod
     def per_batch_transform(batch: Any) -> Any:
         """Transforms to apply on a whole batch before uncollation to individual samples.
 
         Can involve both CPU and Device transforms as this is not applied in separate workers.
         """
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/io/transform_predictions.py` & `lightning-flash-0.8.2/src/flash/core/data/io/transform_predictions.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/output.py` & `lightning-flash-0.8.2/src/flash/core/data/output.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/properties.py` & `lightning-flash-0.8.2/src/flash/core/data/properties.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/splits.py` & `lightning-flash-0.8.2/src/flash/core/data/splits.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,26 +28,23 @@
         dataset: Any,
         indices: List[int],
         running_stage: Optional[RunningStage] = None,
         use_duplicated_indices: bool = False,
     ) -> None:
         kwargs = {}
         if running_stage is not None:
-            kwargs = dict(running_stage=running_stage)
+            kwargs = {"running_stage": running_stage}
         elif isinstance(dataset, Properties):
-            kwargs = dict(running_stage=dataset._running_stage)
+            kwargs = {"running_stage": dataset._running_stage}
         super().__init__(**kwargs)
 
         if not isinstance(indices, list):
             raise TypeError("indices should be a list")
 
-        if use_duplicated_indices:
-            indices = list(indices)
-        else:
-            indices = list(np.unique(indices))
+        indices = list(indices) if use_duplicated_indices else list(np.unique(indices))
 
         if np.max(indices) >= len(dataset) or np.min(indices) < 0:
             raise ValueError(f"`indices` should be within [0, {len(dataset) -1}].")
 
         self.dataset = dataset
         self.indices = indices
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/transforms.py` & `lightning-flash-0.8.2/src/flash/core/data/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,23 +49,23 @@
         if isinstance(x, dict):
             x_ = {self._mapping.get(key, key): np.array(value) for key, value in x.items() if key in self._mapping}
         else:
             x_ = {"image": x}
         x_ = self.transform(**x_)
         if isinstance(x, dict):
             x.update({self._mapping_rev.get(k, k): x_[k] for k in self._mapping_rev if k in x_})
-        else:
-            x = x_["image"]
-        return x
+            return x
+
+        return x_["image"]
 
 
 class ApplyToKeys(nn.Sequential):
-    """The ``ApplyToKeys`` class is an ``nn.Sequential`` which applies the given transforms to the given keys from
-    the input. When a single key is given, a single value will be passed to the transforms. When multiple keys are
-    given, the corresponding values will be passed to the transforms as a list.
+    """The ``ApplyToKeys`` class is an ``nn.Sequential`` which applies the given transforms to the given keys from the
+    input. When a single key is given, a single value will be passed to the transforms. When multiple keys are given,
+    the corresponding values will be passed to the transforms as a list.
 
     Args:
         keys: The key (``str``) or sequence of keys (``Sequence[str]``) to extract and forward to the transforms.
         args: The transforms, passed to the ``nn.Sequential`` super constructor.
     """
 
     def __init__(self, keys: Union[str, Sequence[str]], *args):
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/utilities/classification.py` & `lightning-flash-0.8.2/src/flash/core/data/utilities/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from dataclasses import dataclass
 from functools import reduce
-from typing import Any, cast, ClassVar, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, ClassVar, Dict, List, Optional, Tuple, Type, Union, cast
 
 import numpy as np
 import torch
 from torch import Tensor
 
 from flash.core.data.utilities.sort import sorted_alphanumeric
-from flash.core.utilities.imports import _CORE_TESTING
+from flash.core.utilities.imports import _TOPIC_CORE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _CORE_TESTING:
+if not _TOPIC_CORE_AVAILABLE:
     __doctest_skip__ = ["*"]
 
 
 def _is_list_like(x: Any) -> bool:
     try:
         _ = x[0]
         _ = len(x)
@@ -352,28 +352,27 @@
         target: A target that is one of: a single target, a list of targets, a comma delimited string.
     """
     if isinstance(target, str):
         target = _strip(target)
         # TODO: This could be a dangerous assumption if people happen to have a label that contains a comma or space
         if "," in target:
             return CommaDelimitedMultiLabelTargetFormatter
-        elif " " in target:
+        if " " in target:
             return SpaceDelimitedTargetFormatter
-        else:
-            return SingleLabelTargetFormatter
-    elif _is_list_like(target):
+        return SingleLabelTargetFormatter
+    if _is_list_like(target):
         if isinstance(target[0], str):
             return MultiLabelTargetFormatter
         target = _as_list(target)
         if len(target) > 1:
             if all(t == 0 or t == 1 for t in target):
                 if sum(target) == 1:
                     return SingleBinaryTargetFormatter
                 return MultiBinaryTargetFormatter
-            elif any(isinstance(t, float) for t in target):
+            if any(isinstance(t, float) for t in target):
                 return MultiSoftTargetFormatter
             return MultiNumericTargetFormatter
     return SingleNumericTargetFormatter
 
 
 _RESOLUTION_MAPPING: Dict[Type[TargetFormatter], List[Type[TargetFormatter]]] = {
     MultiBinaryTargetFormatter: [MultiNumericTargetFormatter, MultiSoftTargetFormatter],
@@ -381,25 +380,25 @@
     SingleLabelTargetFormatter: [CommaDelimitedMultiLabelTargetFormatter, SpaceDelimitedTargetFormatter],
     SingleNumericTargetFormatter: [SingleBinaryTargetFormatter, MultiNumericTargetFormatter],
 }
 
 
 def _resolve_target_formatter(a: Type[TargetFormatter], b: Type[TargetFormatter]) -> Type[TargetFormatter]:
     """The purpose of this resolution function is to enable reduction of the ``TargetFormatter`` type over multiple
-    targets. For example, if one target formatter type is ``CommaDelimitedMultiLabelTargetFormatter`` and the other
-    type is ``SingleLabelTargetFormatter``then their reduction will be ``CommaDelimitedMultiLabelTargetFormatter``.
+    targets. For example, if one target formatter type is ``CommaDelimitedMultiLabelTargetFormatter`` and the other type
+    is ``SingleLabelTargetFormatter``then their reduction will be ``CommaDelimitedMultiLabelTargetFormatter``.
 
     Raises:
         ValueError: If the two target formatters could not be resolved.
     """
     if a is b:
         return a
-    elif a in _RESOLUTION_MAPPING and b in _RESOLUTION_MAPPING[a]:
+    if a in _RESOLUTION_MAPPING and b in _RESOLUTION_MAPPING[a]:
         return b
-    elif b in _RESOLUTION_MAPPING and a in _RESOLUTION_MAPPING[b]:
+    if b in _RESOLUTION_MAPPING and a in _RESOLUTION_MAPPING[b]:
         return a
     raise ValueError(
         "Found inconsistent target formats. All targets should be either: single values, lists of values, or "
         "comma-delimited strings."
     )
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/utilities/collate.py` & `lightning-flash-0.8.2/src/flash/core/data/utilities/collate.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     return functools.partial(_wrap_collate, collate)
 
 
 _default_collate = wrap_collate(torch_default_collate)
 
 
 def default_collate(batch: List[Any]) -> Any:
-    """The :func:`flash.data.utilities.collate.default_collate` extends `torch.utils.data._utils.default_collate`
-    to first extract any metadata from the samples in the batch (in the ``"metadata"`` key). The list of metadata
-    entries will then be inserted into the collated result.
+    """The :func:`flash.data.utilities.collate.default_collate` extends `torch.utils.data._utils.default_collate` to
+    first extract any metadata from the samples in the batch (in the ``"metadata"`` key). The list of metadata entries
+    will then be inserted into the collated result.
 
     Args:
         batch: The list of samples to collate.
 
     Returns:
         The collated batch.
     """
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/utilities/data_frame.py` & `lightning-flash-0.8.2/src/flash/core/data/utilities/data_frame.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/utilities/loading.py` & `lightning-flash-0.8.2/src/flash/core/data/utilities/loading.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,25 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
+import glob
+import re
 from functools import partial
+from os import PathLike
+from typing import Union
+from urllib.parse import parse_qs, quote, urlencode, urlparse
 
 import fsspec
 import numpy as np
 import pandas as pd
 import torch
 
 from flash.core.data.utilities.paths import has_file_allowed_extension
-from flash.core.utilities.imports import _AUDIO_AVAILABLE, _TORCHVISION_AVAILABLE, Image
+from flash.core.utilities.imports import _TOPIC_AUDIO_AVAILABLE, _TORCHVISION_AVAILABLE, Image
 
-if _AUDIO_AVAILABLE:
+if _TOPIC_AUDIO_AVAILABLE:
     from torchaudio.transforms import Spectrogram
 
 if _TORCHVISION_AVAILABLE:
     from torchvision.datasets.folder import IMG_EXTENSIONS
 else:
     IMG_EXTENSIONS = (".jpg", ".jpeg", ".png", ".ppm", ".bmp", ".pgm", ".tif", ".tiff", ".webp")
 
@@ -135,17 +140,38 @@
         if has_file_allowed_extension(file_path, extensions):
             return loader
     raise ValueError(
         f"File: {file_path} has an unsupported extension. Supported extensions: " f"{list(sum(loaders.keys(), ()))}."
     )
 
 
+WINDOWS_FILE_PATH_RE = re.compile("^[a-zA-Z]:(\\\\[^\\\\]|/[^/]).*")
+
+
+def is_local_path(file_path: str) -> bool:
+    if WINDOWS_FILE_PATH_RE.fullmatch(file_path):
+        return True
+    return urlparse(file_path).scheme in ["", "file"]
+
+
+def escape_url(url: str) -> str:
+    parsed = urlparse(url)
+    return f"{parsed.scheme}://{parsed.netloc}{quote(parsed.path)}?{urlencode(parse_qs(parsed.query), doseq=True)}"
+
+
+def escape_file_path(file_path: Union[str, PathLike]) -> str:
+    file_path_str = str(file_path)
+    return glob.escape(file_path_str) if is_local_path(file_path_str) else escape_url(file_path_str)
+
+
 def load(file_path: str, loaders):
     loader = _get_loader(file_path, loaders)
-    with fsspec.open(file_path) as file:
+    # escaping file_path to avoid fsspec treating the path as a glob pattern
+    # fsspec ignores `expand=False` in read mode
+    with fsspec.open(escape_file_path(file_path)) as file:
         return loader(file)
 
 
 def load_image(file_path: str):
     """Load an image from a file.
 
     Args:
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/utilities/paths.py` & `lightning-flash-0.8.2/src/flash/core/data/utilities/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-from typing import Any, Callable, cast, List, Optional, Tuple, Union
+from typing import Any, Callable, List, Optional, Tuple, Union, cast
 
 from pytorch_lightning.utilities import rank_zero_warn
 
 from flash.core.data.utilities.sort import sorted_alphanumeric
 
 PATH_TYPE = Union[str, bytes, os.PathLike]
 
@@ -132,16 +132,16 @@
 
 
 def filter_valid_files(
     files: Union[PATH_TYPE, List[PATH_TYPE]],
     *additional_lists: List[Any],
     valid_extensions: Optional[Tuple[str, ...]] = None,
 ) -> Union[List[Any], Tuple[List[Any], ...]]:
-    """Filter the given list of files and any additional lists to include only the entries that contain a file with
-    a valid extension.
+    """Filter the given list of files and any additional lists to include only the entries that contain a file with a
+    valid extension.
 
     Args:
         files: The list of files to filter by.
         additional_lists: Any additional lists to be filtered together with files.
         valid_extensions: The tuple of valid file extensions.
 
     Returns:
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/utilities/samples.py` & `lightning-flash-0.8.2/src/flash/core/data/utilities/samples.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/utilities/sort.py` & `lightning-flash-0.8.2/src/flash/core/data/utilities/sort.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,13 @@
 
 
 def _alphanumeric_key(key: str) -> List[Union[int, str]]:
     return [_convert(c) for c in re.split("([0-9]+)", key)]
 
 
 def sorted_alphanumeric(iterable: Iterable[str]) -> Iterable[str]:
-    """Sort the given iterable in the way that humans expect. For example, given ``{"class_1", "class_11",
-    "class_2"}`` this returns ``["class_1", "class_2", "class_11"]``.
+    """Sort the given iterable in the way that humans expect. For example, given ``{"class_1", "class_11", "class_2"}``
+    this returns ``["class_1", "class_2", "class_11"]``.
 
-    Copied from:
-    https://blog.codinghorror.com/sorting-for-humans-natural-sort-order/
+    Copied from: https://blog.codinghorror.com/sorting-for-humans-natural-sort-order/
     """
     return sorted(iterable, key=_alphanumeric_key)
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/data/utils.py` & `lightning-flash-0.8.2/src/flash/core/data/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
 import requests
 import urllib3
 from pytorch_lightning.utilities.apply_func import apply_to_collection
 from torch import nn
 from tqdm.auto import tqdm as tq
 
-from flash.core.utilities.imports import _CORE_TESTING
+from flash.core.utilities.imports import _TOPIC_CORE_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 
 # Skip doctests if requirements aren't available
-if not _CORE_TESTING:
+if not _TOPIC_CORE_AVAILABLE:
     __doctest_skip__ = ["download_data"]
 
 _STAGES_PREFIX = {
     RunningStage.TRAINING: "train",
     RunningStage.TESTING: "test",
     RunningStage.VALIDATING: "val",
     RunningStage.PREDICTING: "predict",
@@ -84,16 +84,16 @@
         os.makedirs(path)
     local_filename = os.path.join(path, url.split("/")[-1])
     r = requests.get(url, stream=True, verify=False)
     file_size = int(r.headers["Content-Length"]) if "Content-Length" in r.headers else 0
     chunk_size = 1024
     num_bars = int(file_size / chunk_size)
     if verbose:
-        print(dict(file_size=file_size))
-        print(dict(num_bars=num_bars))
+        print({"file_size": file_size})
+        print({"num_bars": num_bars})
 
     if not os.path.exists(local_filename):
         with open(local_filename, "wb") as fp:
             for chunk in tq(
                 r.iter_content(chunk_size=chunk_size),
                 total=num_bars,
                 unit="KB",
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/finetuning.py` & `lightning-flash-0.8.2/src/flash/core/finetuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     # ReadTheDocs mocks the `LightningEnum` import to be a regular type, so we replace it with a plain Enum here.
     from enum import Enum
 
     LightningEnum = Enum
 
 
 class FinetuningStrategies(LightningEnum):
-    """The ``FinetuningStrategies`` enum contains the keys that are used internally by the ``FlashBaseFinetuning``
-    when choosing the strategy to perform."""
+    """The ``FinetuningStrategies`` enum contains the keys that are used internally by the ``FlashBaseFinetuning`` when
+    choosing the strategy to perform."""
 
     NO_FREEZE = "no_freeze"
     FREEZE = "freeze"
     FREEZE_UNFREEZE = "freeze_unfreeze"
     UNFREEZE_MILESTONES = "unfreeze_milestones"
 
     # TODO: Create a FlashEnum class???
@@ -213,16 +213,15 @@
         strategy_metadata: Tuple[Tuple[int, int], int],
         train_bn: bool = True,
     ):
         super().__init__(FinetuningStrategies.UNFREEZE_MILESTONES, strategy_metadata, train_bn)
 
 
 class FlashDeepSpeedFinetuning(FlashBaseFinetuning):
-    """FlashDeepSpeedFinetuning can be used to create a custom Flash Finetuning Callback which works with
-    DeepSpeed.
+    """FlashDeepSpeedFinetuning can be used to create a custom Flash Finetuning Callback which works with DeepSpeed.
 
     DeepSpeed cannot store and load its parameters when working with Lightning. So FlashDeepSpeedFinetuning overrides
     `_store` to not store its parameters.
     """
 
     def _store(
         self,
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/heads.py` & `lightning-flash-0.8.2/src/flash/core/heads.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/hooks.py` & `lightning-flash-0.8.2/src/flash/core/hooks.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/fiftyone/utils.py` & `lightning-flash-0.8.2/src/flash/core/integrations/fiftyone/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 def visualize(
     predictions: Union[List[Label], List[Dict[str, Label]]],
     filepaths: Optional[List[str]] = None,
     label_field: Optional[str] = "predictions",
     wait: Optional[bool] = False,
     **kwargs,
 ) -> Optional[Session]:
-    """Visualizes predictions from a model with a FiftyOne Output in the
-    :ref:`FiftyOne App <fiftyone:fiftyone-app>`.
+    """Visualizes predictions from a model with a FiftyOne Output in the :ref:`FiftyOne App <fiftyone:fiftyone-app>`.
 
     This method can be used in all of the following environments:
 
     -   **Local Python shell**: The App will launch in a new tab in your
         default web browser.
     -   **Remote Python shell**: Pass the ``remote=True`` option to this method
         and then follow the instructions printed to your remote shell to open
@@ -76,15 +75,15 @@
         labels = predictions
 
     if filepaths is None:
         raise ValueError("The `filepaths` argument is required if filepaths are not provided in `labels`.")
 
     dataset = fo.Dataset()
     if filepaths:
-        dataset.add_samples([fo.Sample(filepath=f, **{label_field: l}) for f, l in zip(filepaths, labels)])
+        dataset.add_samples([fo.Sample(filepath=fp, **{label_field: lb}) for fp, lb in zip(filepaths, labels)])
 
     session = fo.launch_app(dataset, **kwargs)
     if wait:
         session.wait()
 
     return session
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/icevision/adapter.py` & `lightning-flash-0.8.2/src/flash/core/integrations/icevision/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from torch import Tensor
 from torch.utils.data import DataLoader, Sampler
 
 import flash
 from flash.core.adapter import Adapter
 from flash.core.data.io.input import DataKeys, InputBase
-from flash.core.data.io.input_transform import create_worker_input_transform_processor, InputTransform
+from flash.core.data.io.input_transform import InputTransform, create_worker_input_transform_processor
 from flash.core.integrations.icevision.transforms import (
     from_icevision_predictions,
     from_icevision_record,
     to_icevision_record,
 )
 from flash.core.integrations.icevision.wrappers import wrap_icevision_adapter
 from flash.core.model import Task
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/icevision/backbones.py` & `lightning-flash-0.8.2/src/flash/core/integrations/icevision/backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/icevision/data.py` & `lightning-flash-0.8.2/src/flash/core/integrations/icevision/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 import inspect
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import numpy as np
 
 from flash.core.data.io.input import DataKeys, Input
-from flash.core.data.utilities.loading import IMG_EXTENSIONS, load_image, NP_EXTENSIONS
+from flash.core.data.utilities.loading import IMG_EXTENSIONS, NP_EXTENSIONS, load_image
 from flash.core.data.utilities.paths import list_valid_files
 from flash.core.integrations.icevision.transforms import from_icevision_record
 from flash.core.utilities.imports import _ICEVISION_AVAILABLE, requires
 
 if _ICEVISION_AVAILABLE:
     from icevision.core.record import BaseRecord
     from icevision.core.record_components import ClassMapRecordComponent, FilepathRecordComponent, tasks
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/icevision/transforms.py` & `lightning-flash-0.8.2/src/flash/core/integrations/icevision/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
-from torch import nn, Tensor
+from torch import Tensor, nn
 
 from flash.core.data.io.input import DataKeys
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.utilities.imports import (
     _ICEVISION_AVAILABLE,
     _ICEVISION_GREATER_EQUAL_0_11_0,
-    _IMAGE_AVAILABLE,
+    _TOPIC_IMAGE_AVAILABLE,
     requires,
 )
 
-if _IMAGE_AVAILABLE:
+if _TOPIC_IMAGE_AVAILABLE:
     from PIL import Image
 
 if _ICEVISION_AVAILABLE:
     from icevision.core import tasks
     from icevision.core.bbox import BBox
     from icevision.core.keypoints import KeyPoints
     from icevision.core.mask import Mask, MaskArray
@@ -279,15 +279,14 @@
         record = to_icevision_record(x)
         record = self.transform(record)
         return from_icevision_record(record)
 
 
 @dataclass
 class IceVisionInputTransform(InputTransform):
-
     image_size: int = 128
 
     @requires("image", "icevision")
     def per_sample_transform(self):
         return IceVisionTransformAdapter([*A.resize_and_pad(self.image_size), A.Normalize()])
 
     @requires("image", "icevision")
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/icevision/wrappers.py` & `lightning-flash-0.8.2/src/flash/core/integrations/icevision/wrappers.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/labelstudio/input.py` & `lightning-flash-0.8.2/src/flash/core/integrations/labelstudio/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     classes: Set
     data_types: Set
     tag_types: Set
 
 
 def _get_labels_from_sample(labels, classes):
     """Translate string labels to int."""
-    sorted_labels = sorted(list(classes))
+    sorted_labels = sorted(classes)
     return [sorted_labels.index(item) for item in labels] if isinstance(labels, list) else sorted_labels.index(labels)
 
 
 def _load_json_data(data, data_folder, multi_label=False):
     """Utility method to extract data from Label Studio json files."""
     results = []
     test_results = []
@@ -137,19 +137,18 @@
     def load_sample(self, sample: Mapping[str, Any] = None) -> Any:
         """Load 1 sample from dataset."""
         # all other data types
         # separate label from data
         label = _get_labels_from_sample(sample["label"], self.parameters.classes)
         # delete label from input data
         del sample["label"]
-        result = {
+        return {
             DataKeys.INPUT: sample,
             DataKeys.TARGET: label,
         }
-        return result
 
     @staticmethod
     def _split_train_test_data(data: Dict, multi_label: bool = False) -> List[Dict]:
         file_path = data.get("export_json", None)
 
         if not file_path:
             raise TypeError("The key `export_json` should be provided as a string.")
@@ -188,15 +187,16 @@
         if fs.exists(export_path):
             fs.delete(export_path)
         with fs.open(export_path, mode="w") as f:
             json.dump(raw_data, f)
 
     @staticmethod
     def _split_train_val_data(data: Dict, split: float = 0) -> List[Dict]:
-        assert split > 0 and split < 1
+        assert split > 0
+        assert split < 1
         file_path = data.get("export_json", None)
 
         if not file_path:
             raise TypeError("The key `export_json` should be provided as a string.")
 
         fs = get_filesystem(file_path)
         with fs.open(file_path) as f:
@@ -237,19 +237,18 @@
     Export data should point to image files"""
 
     def load_sample(self, sample: Mapping[str, Any] = None) -> Any:
         """Load 1 sample from dataset."""
         p = sample["file_upload"]
         # loading image
         image = load_image(p)
-        result = {
+        return {
             DataKeys.INPUT: image,
             DataKeys.TARGET: _get_labels_from_sample(sample["label"], self.parameters.classes),
         }
-        return result
 
 
 class LabelStudioTextClassificationInput(LabelStudioInput):
     """The ``LabelStudioTextInput`` expects the input to
     :meth:`~flash.core.data.io.input.Input.load_data` to be a json export from label studio.
     Export data should point to text data
     """
@@ -305,15 +304,14 @@
         """load_data produces a sequence or iterable of samples."""
         res = super().load_data(data, parameters=parameters)
         return self.convert_to_encodedvideo(res)
 
     def convert_to_encodedvideo(self, dataset):
         """Converting dataset to EncodedVideoDataset."""
         if len(dataset) > 0:
-
             from pytorchvideo.data import LabeledVideoDataset
 
             dataset = LabeledVideoDataset(
                 [
                     (
                         os.path.join(self._data_folder, sample["file_upload"]),
                         {"label": _get_labels_from_sample(sample["label"], self.parameters.classes)},
@@ -338,15 +336,14 @@
     train_data_folder: str = None,
     val_data_folder: str = None,
     test_data_folder: str = None,
     predict_data_folder: str = None,
     val_split: Optional[float] = None,
     multi_label: Optional[bool] = False,
 ):
-
     train_data = None
     val_data = None
     test_data = None
     predict_data = None
     data = {
         "data_folder": data_folder,
         "export_json": export_json,
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/labelstudio/visualizer.py` & `lightning-flash-0.8.2/src/flash/core/integrations/labelstudio/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,59 +43,58 @@
                     "task": task["id"],
                 }
                 if task.get("predictions"):
                     task["predictions"].append(temp)
                 else:
                     task["predictions"] = [temp]
             return _raw_data
-        else:
-            print("No export file provided, meta information is generated!")
-            final_results = []
-            for res in results:
-                temp = {
-                    "result": [res],
-                    "id": meta["max_predictions_id"],
-                    "model_version": "",
-                    "score": 0.0,
-                    "task": meta["max_predictions_id"],
-                }
-                task = {
-                    "id": meta["max_predictions_id"],
-                    "predictions": [temp],
-                    "data": {data_type: ""},
-                    "project": 1,
-                }
-                meta["max_predictions_id"] = meta["max_predictions_id"] + 1
-                final_results.append(task)
-            return final_results
+
+        print("No export file provided, meta information is generated!")
+        final_results = []
+        for res in results:
+            temp = {
+                "result": [res],
+                "id": meta["max_predictions_id"],
+                "model_version": "",
+                "score": 0.0,
+                "task": meta["max_predictions_id"],
+            }
+            task = {
+                "id": meta["max_predictions_id"],
+                "predictions": [temp],
+                "data": {data_type: ""},
+                "project": 1,
+            }
+            meta["max_predictions_id"] = meta["max_predictions_id"] + 1
+            final_results.append(task)
+        return final_results
 
     def _construct_result(self, pred):
         """Construction Label Studio result from data source and prediction values."""
         # get label
         if isinstance(pred, list):
             label = [list(self.parameters.classes)[p] for p in pred]
         else:
             label = list(self.parameters.classes)[pred]
         # get data type, if len(data_types) > 1 take first data type
         data_type = list(self.parameters.data_types)[0]
         # get tag type, if len(tag_types) > 1 take first tag
         tag_type = list(self.parameters.tag_types)[0]
-        js = {
+        return {
             "result": [
                 {
                     "id": "".join(
                         random.SystemRandom().choice(string.ascii_uppercase + string.ascii_lowercase + string.digits)
                         for _ in range(10)
                     ),
                     "from_name": "tag",
                     "to_name": data_type,
                     "type": tag_type,
                     "value": {tag_type: label if isinstance(label, list) else [label]},
                 }
             ]
         }
-        return js
 
 
 def launch_app(datamodule: DataModule) -> "App":
     """Creating instance of Visualizing App."""
     return App(datamodule)
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_forecasting/adapter.py` & `lightning-flash-0.8.2/src/flash/core/integrations/pytorch_forecasting/adapter.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_forecasting/backbones.py` & `lightning-flash-0.8.2/src/flash/core/integrations/pytorch_forecasting/backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_forecasting/transforms.py` & `lightning-flash-0.8.2/src/flash/core/integrations/pytorch_forecasting/transforms.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_tabular/adapter.py` & `lightning-flash-0.8.2/src/flash/core/integrations/pytorch_tabular/adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,33 +38,31 @@
         num_features: int,
         output_dim: int,
         backbone: str,
         loss_fn: Optional[Callable],
         metrics: Optional[Union[torchmetrics.Metric, List[torchmetrics.Metric]]],
         backbone_kwargs: Optional[Dict[str, Any]] = None,
     ) -> Adapter:
-
         backbone_kwargs = backbone_kwargs or {}
         parameters = {
             "embedding_dims": embedding_sizes,
             "categorical_cols": categorical_fields,
             "categorical_cardinality": cat_dims,
             "categorical_dim": len(categorical_fields),
             "continuous_dim": num_features - len(categorical_fields),
             "output_dim": output_dim,
+            "embedded_cat_dim": sum([embd_dim for _, embd_dim in embedding_sizes]),
         }
-        adapter = cls(
+        return cls(
             task_type,
             task.backbones.get(backbone)(
                 task_type=task_type, parameters=parameters, loss_fn=loss_fn, metrics=metrics, **backbone_kwargs
             ),
         )
 
-        return adapter
-
     def convert_batch(self, batch):
         new_batch = {
             "continuous": batch[DataKeys.INPUT][1],
             "categorical": batch[DataKeys.INPUT][0],
         }
         if DataKeys.TARGET in batch:
             new_batch["target"] = batch[DataKeys.TARGET].reshape(-1, 1)
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/pytorch_tabular/backbones.py` & `lightning-flash-0.8.2/src/flash/core/integrations/pytorch_tabular/backbones.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
 from flash.core.integrations.pytorch_tabular.adapter import PytorchTabularAdapter
 from flash.core.registry import FlashRegistry
 from flash.core.utilities.imports import _PYTORCHTABULAR_AVAILABLE
 from flash.core.utilities.providers import _PYTORCH_TABULAR
 
 if _PYTORCHTABULAR_AVAILABLE:
-    import pytorch_tabular.models as models
+    import pytorch_tabular
     from omegaconf import DictConfig, OmegaConf
     from pytorch_tabular.config import ModelConfig
     from pytorch_tabular.models import (
         AutoIntConfig,
         CategoryEmbeddingModelConfig,
         FTTransformerConfig,
+        GatedAdditiveTreeEnsembleConfig,
         NodeConfig,
         TabNetModelConfig,
         TabTransformerConfig,
     )
 
 
 PYTORCH_TABULAR_BACKBONES = FlashRegistry("backbones")
@@ -42,20 +43,20 @@
 if _PYTORCHTABULAR_AVAILABLE:
 
     def _read_parse_config(config, cls):
         if isinstance(config, str):
             if os.path.exists(config):
                 _config = OmegaConf.load(config)
                 if cls == ModelConfig:
-                    cls = getattr(getattr(models, _config._module_src), _config._config_name)
+                    cls = getattr(getattr(pytorch_tabular, _config._module_src), _config._config_name)
                 config = cls(
                     **{
                         k: v
                         for k, v in _config.items()
-                        if (k in cls.__dataclass_fields__.keys()) and cls.__dataclass_fields__[k].init
+                        if (k in cls.__dataclass_fields__) and cls.__dataclass_fields__[k].init
                     }
                 )
             else:
                 raise ValueError(f"{config} is not a valid path")
         config = OmegaConf.structured(config)
         return config
 
@@ -65,32 +66,36 @@
         parameters: DictConfig,
         loss_fn: Callable,
         metrics: Optional[Union[torchmetrics.Metric, List[torchmetrics.Metric]]],
         **model_kwargs,
     ):
         model_config = model_config_class(task=task_type, embedding_dims=parameters["embedding_dims"], **model_kwargs)
         model_config = _read_parse_config(model_config, ModelConfig)
-        model_callable = getattr(getattr(models, model_config._module_src), model_config._model_name)
+        model_callable = pytorch_tabular
+        for attr in model_config._module_src.split(".") + [model_config._model_name]:
+            model_callable = getattr(model_callable, attr)
         config = OmegaConf.merge(
             OmegaConf.create(parameters),
             OmegaConf.to_container(model_config),
         )
-        model = model_callable(config=config, custom_loss=loss_fn, custom_metrics=metrics)
-        return model
+        return model_callable(
+            config=config, custom_loss=loss_fn, custom_metrics=metrics, inferred_config=DictConfig(config)
+        )
 
     for model_config_class, name in zip(
         [
             TabNetModelConfig,
             TabTransformerConfig,
             FTTransformerConfig,
             AutoIntConfig,
             NodeConfig,
             CategoryEmbeddingModelConfig,
+            GatedAdditiveTreeEnsembleConfig,
         ],
-        ["tabnet", "tabtransformer", "fttransformer", "autoint", "node", "category_embedding"],
+        ["tabnet", "tabtransformer", "fttransformer", "autoint", "node", "category_embedding", "gate"],
     ):
         PYTORCH_TABULAR_BACKBONES(
             functools.partial(load_pytorch_tabular, model_config_class),
             name=name,
             providers=_PYTORCH_TABULAR,
             adapter=PytorchTabularAdapter,
         )
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/integrations/transformers/collate.py` & `lightning-flash-0.8.2/src/flash/core/integrations/transformers/collate.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 if _TRANSFORMERS_AVAILABLE:
     from transformers import AutoTokenizer
 
 
 @dataclass(unsafe_hash=True)
 class TransformersCollate:
-
     backbone: str
     tokenizer_kwargs: Optional[Dict[str, Any]] = field(default_factory=dict, hash=False)
 
     def __post_init__(self):
         tokenizer_kwargs = self.tokenizer_kwargs or {}
         self.tokenizer = AutoTokenizer.from_pretrained(self.backbone, use_fast=True, **tokenizer_kwargs)
 
@@ -43,8 +42,8 @@
                 tensor_sample[key] = torch.tensor(sample[key])
         return tensor_sample
 
     def tokenize(self, sample):
         raise NotImplementedError
 
     def __call__(self, samples):
-        return self.to_tensor(self.tokenize({key: [sample[key] for sample in samples] for key in samples[0].keys()}))
+        return self.to_tensor(self.tokenize({key: [sample[key] for sample in samples] for key in samples[0]}))
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/model.py` & `lightning-flash-0.8.2/src/flash/core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,52 +20,52 @@
 import pytorch_lightning as pl
 import torch
 import torchmetrics
 from pytorch_lightning import LightningModule, Trainer
 from pytorch_lightning.callbacks import Callback
 from pytorch_lightning.callbacks.finetuning import BaseFinetuning
 from pytorch_lightning.utilities.enums import LightningEnum
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.optim.lr_scheduler import _LRScheduler
 from torch.optim.optimizer import Optimizer
 from torch.utils.data import DataLoader, Sampler
 
 import flash
 from flash.core.data.io.input import InputBase, ServeInput
 from flash.core.data.io.input_transform import (
+    InputTransform,
     create_or_configure_input_transform,
     create_worker_input_transform_processor,
-    InputTransform,
 )
 from flash.core.data.io.output import Output
 from flash.core.data.io.output_transform import OutputTransform
 from flash.core.data.output import BASE_OUTPUTS
 from flash.core.data.utilities.collate import default_collate
 from flash.core.finetuning import _FINETUNING_STRATEGIES_REGISTRY
 from flash.core.hooks import FineTuningHooks
 from flash.core.optimizers.optimizers import _OPTIMIZERS_REGISTRY
 from flash.core.optimizers.schedulers import _SCHEDULERS_REGISTRY
 from flash.core.registry import FlashRegistry
 from flash.core.serve.composition import Composition
 from flash.core.utilities.apply_func import get_callable_dict
-from flash.core.utilities.imports import _CORE_TESTING, _PL_GREATER_EQUAL_1_5_0, requires
+from flash.core.utilities.imports import _TOPIC_CORE_AVAILABLE, requires
 from flash.core.utilities.providers import _HUGGINGFACE
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import (
     INPUT_TRANSFORM_TYPE,
     LOSS_FN_TYPE,
     LR_SCHEDULER_TYPE,
     METRICS_TYPE,
     MODEL_TYPE,
     OPTIMIZER_TYPE,
     OUTPUT_TRANSFORM_TYPE,
 )
 
 # Skip doctests if requirements aren't available
-if not _CORE_TESTING:
+if not _TOPIC_CORE_AVAILABLE:
     __doctest_skip__ = ["Task", "Task.*"]
 
 
 class ModuleWrapperBase:
     """The ``ModuleWrapperBase`` is a base for classes which wrap a ``LightningModule`` or an instance of
     ``ModuleWrapperBase``.
 
@@ -80,24 +80,23 @@
 
         self._children = []
 
     def __setattr__(self, key, value):
         if isinstance(value, (LightningModule, ModuleWrapperBase)):
             self._children.append(key)
         patched_attributes = ["_current_fx_name", "_current_hook_fx_name", "_results", "_data_pipeline_state"]
-        if isinstance(value, Trainer) or key in patched_attributes:
-            if hasattr(self, "_children"):
-                for child in self._children:
-                    setattr(getattr(self, child), key, value)
+        if (isinstance(value, Trainer) or key in patched_attributes) and hasattr(self, "_children"):
+            for child in self._children:
+                setattr(getattr(self, child), key, value)
         super().__setattr__(key, value)
 
 
 class DatasetProcessor:
-    """The ``DatasetProcessor`` mixin provides hooks for classes which need custom logic for producing the data
-    loaders for each running stage given the corresponding dataset."""
+    """The ``DatasetProcessor`` mixin provides hooks for classes which need custom logic for producing the data loaders
+    for each running stage given the corresponding dataset."""
 
     def __init__(self):
         super().__init__()
 
         self._collate_fn = default_collate
         self._input_transform = None
 
@@ -320,14 +319,21 @@
         lr_scheduler: The LR scheduler to use during training.
         metrics: Metrics to compute for training and evaluation. Can either be an metric from the `torchmetrics`
             package, a custom metric inheriting from `torchmetrics.Metric`, a callable function or a list/dict
             containing a combination of the aforementioned. In all cases, each metric needs to have the signature
             `metric(preds,target)` and return a single scalar tensor.
         output_transform: :class:`~flash.core.data.io.output_transform.OutputTransform` to use as the default for this
             task.
+
+    >>> Task()  # doctest: +ELLIPSIS
+    Task(
+      (train_metrics): ModuleDict()
+      (val_metrics): ModuleDict()
+      (test_metrics): ModuleDict()
+    )
     """
 
     optimizers_registry: FlashRegistry = _OPTIMIZERS_REGISTRY
     lr_schedulers_registry: FlashRegistry = _SCHEDULERS_REGISTRY
     finetuning_strategies: FlashRegistry = _FINETUNING_STRATEGIES_REGISTRY
     outputs: FlashRegistry = BASE_OUTPUTS
 
@@ -386,18 +392,14 @@
         y_hat = self.to_metrics_format(output[OutputKeys.OUTPUT])
 
         logs = {}
 
         for name, metric in metrics.items():
             if isinstance(metric, torchmetrics.metric.Metric):
                 metric(y_hat, y)
-                # PL 1.4.0 -> 1.4.9 tries to deepcopy the metric.
-                # Sometimes _forward_cache is not a leaf, so we convert it to one.
-                if not metric._forward_cache.is_leaf and not _PL_GREATER_EQUAL_1_5_0:
-                    metric._forward_cache = metric._forward_cache.clone().detach()
                 logs[name] = metric  # log the metric itself if it is of type Metric
             else:
                 logs[name] = metric(y_hat, y)
 
         if len(losses.values()) > 1:
             logs["total_loss"] = sum(losses.values())
             return logs["total_loss"], logs
@@ -429,38 +431,38 @@
         return x
 
     def forward(self, x: Any) -> Any:
         return self.model(x)
 
     def training_step(self, batch: Any, batch_idx: int) -> Any:
         output = self.step(batch, batch_idx, self.train_metrics)
-        log_kwargs = {"batch_size": output.get(OutputKeys.BATCH_SIZE, None)} if _PL_GREATER_EQUAL_1_5_0 else {}
+        log_kwargs = {"batch_size": output.get(OutputKeys.BATCH_SIZE, None)}
         self.log_dict(
             {f"train_{k}": v for k, v in output[OutputKeys.LOGS].items()},
             on_step=True,
             on_epoch=True,
             prog_bar=True,
             **log_kwargs,
         )
         return output[OutputKeys.LOSS]
 
     def validation_step(self, batch: Any, batch_idx: int) -> None:
         output = self.step(batch, batch_idx, self.val_metrics)
-        log_kwargs = {"batch_size": output.get(OutputKeys.BATCH_SIZE, None)} if _PL_GREATER_EQUAL_1_5_0 else {}
+        log_kwargs = {"batch_size": output.get(OutputKeys.BATCH_SIZE, None)}
         self.log_dict(
             {f"val_{k}": v for k, v in output[OutputKeys.LOGS].items()},
             on_step=False,
             on_epoch=True,
             prog_bar=True,
             **log_kwargs,
         )
 
     def test_step(self, batch: Any, batch_idx: int) -> None:
         output = self.step(batch, batch_idx, self.test_metrics)
-        log_kwargs = {"batch_size": output.get(OutputKeys.BATCH_SIZE, None)} if _PL_GREATER_EQUAL_1_5_0 else {}
+        log_kwargs = {"batch_size": output.get(OutputKeys.BATCH_SIZE, None)}
         self.log_dict(
             {f"test_{k}": v for k, v in output[OutputKeys.LOGS].items()},
             on_step=False,
             on_epoch=True,
             prog_bar=True,
             **log_kwargs,
         )
@@ -473,31 +475,29 @@
             batch = batch[0]
         elif isinstance(batch, list):
             # Todo: Understand why stack is needed
             batch = torch.stack(batch)
         return self(batch)
 
     def modules_to_freeze(self) -> Optional[nn.Module]:
-        """By default, we try to get the ``backbone`` attribute from the task and return it or ``None`` if not
-        present.
+        """By default, we try to get the ``backbone`` attribute from the task and return it or ``None`` if not present.
 
         Returns:
             The backbone ``Module`` to freeze or ``None`` if this task does not have a ``backbone`` attribute.
         """
         return getattr(self, "backbone", None)
 
     def _get_optimizer_class_from_registry(self, optimizer_key: str) -> Optimizer:
         if optimizer_key.lower() not in self.available_optimizers():
             raise KeyError(
                 f"Please provide a valid optimizer name and make sure it is registerd with the Optimizer registry."
                 f"\nUse `{self.__class__.__name__}.available_optimizers()` to list the available optimizers."
                 f"\nList of available Optimizers: {self.available_optimizers()}."
             )
-        optimizer_fn = self.optimizers_registry.get(optimizer_key.lower())
-        return optimizer_fn
+        return self.optimizers_registry.get(optimizer_key.lower())
 
     def configure_optimizers(self) -> Union[Optimizer, Tuple[List[Optimizer], List[_LRScheduler]]]:
         """Implement how optimizer and optionally learning rate schedulers should be configured."""
         optimizers_kwargs: Dict[str, Any] = {}
         if isinstance(self.optimizer, str):
             optimizer_fn = self._get_optimizer_class_from_registry(self.optimizer.lower())
         elif isinstance(self.optimizer, Callable):
@@ -539,15 +539,14 @@
         return optimizer
 
     def configure_finetune_callback(
         self,
         strategy: Union[str, Tuple[str, int], Tuple[str, Tuple[Tuple[int, int], int]], BaseFinetuning] = "no_freeze",
         train_bn: bool = True,
     ) -> List[BaseFinetuning]:
-
         if isinstance(strategy, BaseFinetuning):
             return [strategy]
 
         if isinstance(strategy, str):
             if strategy not in self.available_finetuning_strategies():
                 raise ValueError(
                     f"The `strategy` should be one of: {', '.join(self.available_finetuning_strategies())}."
@@ -569,16 +568,16 @@
                 "The `strategy` should be a ``pytorch_lightning.callbacks.BaseFinetuning`` callback or one of: "
                 f"{', '.join(self.available_finetuning_strategies())}."
             )
 
         return [finetuning_strategy_fn(**finetuning_strategy_metadata)]
 
     def as_embedder(self, layer: str):
-        """Convert this task to an embedder. Note that the parameters are not copied so that any optimization of
-        the embedder will also apply to the converted ``Task``.
+        """Convert this task to an embedder. Note that the parameters are not copied so that any optimization of the
+        embedder will also apply to the converted ``Task``.
 
         Args:
             layer: The layer to embed to. This should be one of the :meth:`~flash.core.model.Task.available_layers`.
         """
         from flash.core.utilities.embedder import Embedder  # Avoid circular import
 
         return Embedder(self, layer)
@@ -776,34 +775,37 @@
         else:
             raise TypeError(
                 f"`lr_scheduler` argument should be of type string or callable or tuple(string, dictionary)"
                 f" or tuple(string, dictionary, dictionary) but got {type(self.lr_scheduler)}."
             )
 
         # Providers part
-        if lr_scheduler_metadata is not None and "providers" in lr_scheduler_metadata.keys():
-            if lr_scheduler_metadata["providers"] == _HUGGINGFACE:
-                if lr_scheduler_data["name"] != "constant_schedule":
-                    num_training_steps: int = self.get_num_training_steps()
-                    num_warmup_steps: int = self._compute_warmup(
-                        num_training_steps=num_training_steps,
-                        num_warmup_steps=lr_scheduler_kwargs["num_warmup_steps"],
-                    )
-                    lr_scheduler_kwargs["num_warmup_steps"] = num_warmup_steps
-                    if lr_scheduler_data["name"] != "constant_schedule_with_warmup":
-                        lr_scheduler_kwargs["num_training_steps"] = num_training_steps
+        if (
+            lr_scheduler_metadata is not None
+            and "providers" in lr_scheduler_metadata
+            and lr_scheduler_metadata["providers"] == _HUGGINGFACE
+            and lr_scheduler_data["name"] != "constant_schedule"
+        ):
+            num_training_steps: int = self.get_num_training_steps()
+            num_warmup_steps: int = self._compute_warmup(
+                num_training_steps=num_training_steps,
+                num_warmup_steps=lr_scheduler_kwargs["num_warmup_steps"],
+            )
+            lr_scheduler_kwargs["num_warmup_steps"] = num_warmup_steps
+            if lr_scheduler_data["name"] != "constant_schedule_with_warmup":
+                lr_scheduler_kwargs["num_training_steps"] = num_training_steps
 
         # User can register a callable that returns a lr_scheduler_config
         # 1) If return value is an instance of _LR_Scheduler -> Add to current config and return the config.
         # 2) If return value is a dictionary, check for the lr_scheduler_config `only keys` and return the config.
         lr_scheduler: Union[_LRScheduler, Dict[str, Any]] = lr_scheduler_fn(optimizer, **lr_scheduler_kwargs)
 
         if isinstance(lr_scheduler, Dict):
             dummy_config = default_scheduler_config
-            if not all(config_key in dummy_config.keys() for config_key in lr_scheduler.keys()):
+            if not all(config_key in dummy_config for config_key in lr_scheduler):
                 raise ValueError(
                     f"Please make sure that your custom configuration outputs either an LR Scheduler or a scheduler"
                     f" configuration with keys belonging to {list(dummy_config.keys())}."
                 )
             # If all are present, return the config
             return lr_scheduler
 
@@ -811,14 +813,15 @@
         lr_scheduler_config["scheduler"] = lr_scheduler
         return lr_scheduler_config
 
     def configure_callbacks(self):
         # used only for CI
         if flash._IS_TESTING and torch.cuda.is_available():
             return [BenchmarkConvergenceCI()]
+        return None
 
     @requires("serve")
     def run_serve_sanity_check(
         self, serve_input: ServeInput, transform: INPUT_TRANSFORM_TYPE, transform_kwargs: Optional[Dict], output: Output
     ):
         from fastapi.testclient import TestClient
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/optimizers/lamb.py` & `lightning-flash-0.8.2/src/flash/core/optimizers/lamb.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 # References:
 #     - https://arxiv.org/pdf/1904.00962.pdf
 #     - https://github.com/pytorch/pytorch/blob/1.6/torch/optim/adam.py
 import math
 from typing import Tuple
 
 import torch
-from torch import nn
 from torch.optim.optimizer import Optimizer
 
-from flash.core.utilities.imports import _CORE_TESTING
+from flash.core.utilities.imports import _TOPIC_CORE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _CORE_TESTING:
+if not _TOPIC_CORE_AVAILABLE:
     __doctest_skip__ = ["LAMB"]
 
 
 class LAMB(Optimizer):
     r"""Extends ADAM in pytorch to incorporate LAMB algorithm from the paper: `Large batch optimization for deep
     learning: Training BERT in 76 minutes <https://arxiv.org/pdf/1904.00962.pdf>`_.
 
@@ -47,14 +46,15 @@
         exclude_from_layer_adaptation (bool, optional): layers which do not need LAMB
             layer adaptation (default: False)
         amsgrad (boolean, optional): whether to use the AMSGrad variant of this
             algorithm from the paper `On the Convergence of Adam and Beyond <https://arxiv.org/pdf/1904.09237.pdf>`_
             (default: False)
 
     Example:
+        >>> from torch import nn
         >>> model = nn.Linear(10, 1)
         >>> optimizer = LAMB(model.parameters(), lr=0.1)
         >>> optimizer.zero_grad()
         >>> # loss_fn(model(input), target).backward()
         >>> optimizer.step()
 
     .. warning::
@@ -69,32 +69,32 @@
         lr: float = 1e-3,
         betas: Tuple[float, float] = (0.9, 0.999),
         eps: float = 1e-6,
         weight_decay: float = 0,
         exclude_from_layer_adaptation: bool = False,
         amsgrad: bool = False,
     ):
-        if not 0.0 <= lr:
+        if not lr >= 0.0:
             raise ValueError(f"Invalid learning rate: {lr}")
-        if not 0.0 <= eps:
+        if not eps >= 0.0:
             raise ValueError(f"Invalid epsilon value: {eps}")
         if not 0.0 <= betas[0] < 1.0:
             raise ValueError(f"Invalid beta parameter at index 0: {betas[0]}")
         if not 0.0 <= betas[1] < 1.0:
             raise ValueError(f"Invalid beta parameter at index 1: {betas[1]}")
-        if not 0.0 <= weight_decay:
+        if not weight_decay >= 0.0:
             raise ValueError(f"Invalid weight_decay value: {weight_decay}")
-        defaults = dict(
-            lr=lr,
-            betas=betas,
-            eps=eps,
-            weight_decay=weight_decay,
-            exclude_from_layer_adaptation=exclude_from_layer_adaptation,
-            amsgrad=amsgrad,
-        )
+        defaults = {
+            "lr": lr,
+            "betas": betas,
+            "eps": eps,
+            "weight_decay": weight_decay,
+            "exclude_from_layer_adaptation": exclude_from_layer_adaptation,
+            "amsgrad": amsgrad,
+        }
         super().__init__(params, defaults)
 
     def __setstate__(self, state):
         super().__setstate__(state)
         for group in self.param_groups:
             group.setdefault("amsgrad", False)
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/optimizers/lars.py` & `lightning-flash-0.8.2/src/flash/core/optimizers/lars.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 #
 # Implemented by @ananyahjha93
 # also found at: https://github.com/gridai-labs/aavae/tree/main/src/optimizers
 # References:
 #     - https://arxiv.org/pdf/1708.03888.pdf
 #     - https://github.com/pytorch/pytorch/blob/master/torch/optim/sgd.py
 import torch
-from torch import nn
 from torch.optim.optimizer import Optimizer, required
 
-from flash.core.utilities.imports import _CORE_TESTING
+from flash.core.utilities.imports import _TOPIC_CORE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _CORE_TESTING:
+if not _TOPIC_CORE_AVAILABLE:
     __doctest_skip__ = ["LARS"]
 
 
 class LARS(Optimizer):
     r"""Extends SGD in PyTorch with LARS scaling.
 
     See the paper `Large batch training of Convolutional Networks <https://arxiv.org/pdf/1708.03888.pdf>`_
@@ -42,14 +41,15 @@
         weight_decay (float, optional): weight decay (L2 penalty) (default: 0)
         dampening (float, optional): dampening for momentum (default: 0)
         nesterov (bool, optional): enables Nesterov momentum (default: False)
         trust_coefficient (float, optional): trust coefficient for computing LR (default: 0.001)
         eps (float, optional): eps for division denominator (default: 1e-8)
 
     Example:
+        >>> from torch import nn
         >>> model = nn.Linear(10, 1)
         >>> optimizer = LARS(model.parameters(), lr=0.1, momentum=0.9)
         >>> optimizer.zero_grad()
         >>> # loss_fn(model(input), target).backward()
         >>> optimizer.step()
 
     .. note::
@@ -89,15 +89,21 @@
         if lr is not required and lr < 0.0:
             raise ValueError(f"Invalid learning rate: {lr}")
         if momentum < 0.0:
             raise ValueError(f"Invalid momentum value: {momentum}")
         if weight_decay < 0.0:
             raise ValueError(f"Invalid weight_decay value: {weight_decay}")
 
-        defaults = dict(lr=lr, momentum=momentum, dampening=dampening, weight_decay=weight_decay, nesterov=nesterov)
+        defaults = {
+            "lr": lr,
+            "momentum": momentum,
+            "dampening": dampening,
+            "weight_decay": weight_decay,
+            "nesterov": nesterov,
+        }
         if nesterov and (momentum <= 0 or dampening != 0):
             raise ValueError("Nesterov momentum requires a momentum and zero dampening")
 
         self.eps = eps
         self.trust_coefficient = trust_coefficient
 
         super().__init__(params, defaults)
@@ -133,31 +139,27 @@
                     continue
 
                 d_p = p.grad
                 p_norm = torch.norm(p.data)
                 g_norm = torch.norm(p.grad.data)
 
                 # lars scaling + weight decay part
-                if weight_decay != 0:
-                    if p_norm != 0 and g_norm != 0:
-                        lars_lr = p_norm / (g_norm + p_norm * weight_decay + self.eps)
-                        lars_lr *= self.trust_coefficient
+                if weight_decay != 0 and p_norm != 0 and g_norm != 0:
+                    lars_lr = p_norm / (g_norm + p_norm * weight_decay + self.eps)
+                    lars_lr *= self.trust_coefficient
 
-                        d_p = d_p.add(p, alpha=weight_decay)
-                        d_p *= lars_lr
+                    d_p = d_p.add(p, alpha=weight_decay)
+                    d_p *= lars_lr
 
                 # sgd part
                 if momentum != 0:
                     param_state = self.state[p]
                     if "momentum_buffer" not in param_state:
                         buf = param_state["momentum_buffer"] = torch.clone(d_p).detach()
                     else:
                         buf = param_state["momentum_buffer"]
                         buf.mul_(momentum).add_(d_p, alpha=1 - dampening)
-                    if nesterov:
-                        d_p = d_p.add(buf, alpha=momentum)
-                    else:
-                        d_p = buf
+                    d_p = d_p.add(buf, alpha=momentum) if nesterov else buf
 
                 p.add_(d_p, alpha=-group["lr"])
 
         return loss
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/optimizers/lr_scheduler.py` & `lightning-flash-0.8.2/src/flash/core/optimizers/lr_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,43 @@
 #
 # Implemented by @ananyahjha93
 # also found at: https://github.com/Lightning-AI/lightning-bolts/blob/master/pl_bolts/optimizers/lr_scheduler.py
 import math
 import warnings
 from typing import List
 
-from torch import nn
-from torch.optim import Adam, Optimizer
+from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 
-from flash.core.utilities.imports import _CORE_TESTING
+from flash.core.utilities.imports import _TOPIC_CORE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _CORE_TESTING:
+if not _TOPIC_CORE_AVAILABLE:
     __doctest_skip__ = ["LinearWarmupCosineAnnealingLR"]
 
 
 class LinearWarmupCosineAnnealingLR(_LRScheduler):
-    """Sets the learning rate of each parameter group to follow a linear warmup schedule between warmup_start_lr
-    and base_lr followed by a cosine annealing schedule between base_lr and eta_min.
+    """Sets the learning rate of each parameter group to follow a linear warmup schedule between warmup_start_lr and
+    base_lr followed by a cosine annealing schedule between base_lr and eta_min.
 
     .. warning::
         It is recommended to call :func:`.step()` for :class:`LinearWarmupCosineAnnealingLR`
         after each iteration as calling it after each epoch will keep the starting lr at
         warmup_start_lr for the first epoch which is 0 in most cases.
 
     .. warning::
         passing epoch to :func:`.step()` is being deprecated and comes with an EPOCH_DEPRECATION_WARNING.
         It calls the :func:`_get_closed_form_lr()` method for this scheduler instead of
         :func:`get_lr()`. Though this does not change the behavior of the scheduler, when passing
         epoch param to :func:`.step()`, the user should call the :func:`.step()` function before calling
         train and validation methods.
 
     Example:
+        >>> from torch import nn
+        >>> from torch.optim import Adam
         >>> layer = nn.Linear(10, 1)
         >>> optimizer = Adam(layer.parameters(), lr=0.02)
         >>> scheduler = LinearWarmupCosineAnnealingLR(optimizer, warmup_epochs=10, max_epochs=40)
         >>> #
         >>> # the default case
         >>> for epoch in range(40):
         ...     # train(...)
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/optimizers/optimizers.py` & `lightning-flash-0.8.2/src/flash/core/optimizers/optimizers.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/optimizers/schedulers.py` & `lightning-flash-0.8.2/src/flash/core/optimizers/schedulers.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import inspect
 from typing import Callable, List
 
 from torch.optim import lr_scheduler
 from torch.optim.lr_scheduler import (
-    _LRScheduler,
     CosineAnnealingLR,
     CosineAnnealingWarmRestarts,
     CyclicLR,
     MultiStepLR,
     ReduceLROnPlateau,
     StepLR,
+    _LRScheduler,
 )
 
 from flash.core.registry import FlashRegistry
 from flash.core.utilities.imports import _TORCH_AVAILABLE, _TRANSFORMERS_AVAILABLE
 from flash.core.utilities.providers import _HUGGINGFACE
 
 _SCHEDULERS_REGISTRY = FlashRegistry("scheduler")
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/registry.py` & `lightning-flash-0.8.2/src/flash/core/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,15 @@
     def __add__(self, other):
         registries = []
         if isinstance(self, ConcatRegistry):
             registries += self.registries
         else:
             registries += [self]
 
-        if isinstance(other, ConcatRegistry):
-            registries = other.registries + tuple(registries)
-        else:
-            registries = [other] + registries
+        registries = other.registries + tuple(registries) if isinstance(other, ConcatRegistry) else [other] + registries
 
         return ConcatRegistry(*registries)
 
     def __len__(self) -> int:
         return len(self.functions)
 
     def __contains__(self, key) -> bool:
@@ -118,18 +115,15 @@
         override: bool = False,
         metadata: Optional[Dict[str, Any]] = None,
     ):
         if not callable(fn):
             raise TypeError(f"You can only register a callable, found: {fn}")
 
         if name is None:
-            if hasattr(fn, "func"):
-                name = fn.func.__name__
-            else:
-                name = fn.__name__
+            name = fn.func.__name__ if hasattr(fn, "func") else fn.__name__
 
         if self._verbose:
             rank_zero_info(f"Registering: {fn.__name__} function with name: {name} and metadata: {metadata}")
 
         if "providers" in metadata:
             providers = metadata["providers"]
             fn = print_provider_info(name, providers, fn)
@@ -147,14 +141,15 @@
                 )
             self.functions.append(item)
 
     def _find_matching_index(self, item: _REGISTERED_FUNCTION) -> Optional[int]:
         for idx, fn in enumerate(self.functions):
             if all(fn[k] == item[k] for k in ("fn", "name", "metadata")):
                 return idx
+        return None
 
     def __call__(
         self,
         fn: Optional[Callable[..., Any]] = None,
         name: Optional[str] = None,
         override: bool = False,
         providers: Optional[Union[Provider, List[Provider]]] = None,
@@ -182,16 +177,15 @@
         return _register
 
     def available_keys(self) -> List[str]:
         return sorted(v["name"] for v in self.functions)
 
 
 class ExternalRegistry(FlashRegistry):
-    """The ``ExternalRegistry`` is a ``FlashRegistry`` that can point to an external provider via a getter
-    function.
+    """The ``ExternalRegistry`` is a ``FlashRegistry`` that can point to an external provider via a getter function.
 
     Args:
         getter: A function whose first argument is a key that can optionally take additional args and kwargs.
         providers: The provider(/s) of entries in this registry.
     """
 
     # Prevent users from trying to remove or register items
@@ -209,16 +203,16 @@
         super().__init__(name, verbose=verbose)
 
         self.getter = getter
         self.providers = providers if providers is None or isinstance(providers, list) else [providers]
         self.metadata = metadata
 
     def __contains__(self, item):
-        """Contains is always ``True`` for an ``ExternalRegistry`` as we can't know whether the getter will fail
-        without executing it."""
+        """Contains is always ``True`` for an ``ExternalRegistry`` as we can't know whether the getter will fail without
+        executing it."""
         return True
 
     def get(
         self,
         key: str,
         with_metadata: bool = False,
         strict: bool = True,
@@ -312,10 +306,11 @@
         override: bool = False,
         metadata: Optional[Dict[str, Any]] = None,
     ):
         """Register in the first available registry."""
         for registry in self.registries:
             if getattr(registry, "_register_function", None) is not None:
                 return registry._register_function(fn, name=name, override=override, metadata=metadata)
+        return None
 
     def available_keys(self) -> List[str]:
         return list(itertools.chain.from_iterable(registry.available_keys() for registry in self.registries))
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/regression.py` & `lightning-flash-0.8.2/src/flash/core/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     def __init__(
         self,
         *args,
         loss_fn: Optional[Callable] = None,
         metrics: Union[torchmetrics.Metric, Mapping, Sequence, None] = None,
         **kwargs,
     ) -> None:
-
         metrics, loss_fn = RegressionMixin._build(loss_fn, metrics)
 
         super().__init__(
             *args,
             loss_fn=loss_fn,
             metrics=metrics,
             **kwargs,
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/component.py` & `lightning-flash-0.8.2/src/flash/core/serve/component.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import wraps
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 from torch import nn
 
 from flash.core.serve.core import ParameterContainer, Servable
 from flash.core.serve.decorators import BoundMeta, UnboundMeta
-from flash.core.utilities.imports import _CYTOOLZ_AVAILABLE, _SERVE_AVAILABLE, requires
+from flash.core.utilities.imports import _CYTOOLZ_AVAILABLE, _TOPIC_SERVE_AVAILABLE, requires
 
 if _CYTOOLZ_AVAILABLE:
     from cytoolz import first, isiterable, valfilter
 else:
     first, isiterable, valfilter = None, None, None
 
 # ------------------- Validation Funcs and Pydantic Models --------------------
@@ -93,15 +93,15 @@
     if isiterable(args) and len(args) == 0:
         raise ValueError(f"Iterable args={args} must have length >= 1")
 
     if isinstance(args, (list, tuple)):
         if not all(isinstance(x, _Servable_t) for x in args):
             raise TypeError(f"One of arg in args={args} is not type {_Servable_t}")
     elif isinstance(args, dict):
-        if not all(isinstance(x, str) for x in args.keys()):
+        if not all(isinstance(x, str) for x in args):
             raise TypeError(f"One of keys in args={args.keys()} is not type {str}")
         if not all(isinstance(x, _Servable_t) for x in args.values()):
             raise TypeError(f"One of values in args={args} is not type {_Servable_t}")
     elif not isinstance(args, _Servable_t):
         raise TypeError(f"Args must be instance, list/tuple, or mapping of {_Servable_t}")
 
 
@@ -187,28 +187,26 @@
         klass = super().__call__(*args, **kwargs)
         klass._flashserve_meta_ = replace(klass._flashserve_meta_)
         _validate_exposed_input_parameters_valid(klass)
         klass.__flashserve_init__(*args, **kwargs)
         return klass
 
 
-if _SERVE_AVAILABLE:
+if _TOPIC_SERVE_AVAILABLE:
 
     class ModelComponent(metaclass=FlashServeMeta):
         """Represents a computation which is decorated by `@expose`.
 
-        A component is how we represent the main unit of work; it is a set of
-        evaluations which involve some input being passed through some set of
-        functions to generate some set of outputs.
-
-        To specify a component, we record things like: its name, source file
-        assets, configuration args, model source assets, etc. The
-        specification must be YAML serializable and loadable to/from a fully
-        initialized instance. It must contain the minimal set of information
-        necessary to find and initialize its dependencies (assets) and itself.
+        A component is how we represent the main unit of work; it is a set of evaluations which involve some input being
+        passed through some set of functions to generate some set of outputs.
+
+        To specify a component, we record things like: its name, source file assets, configuration args, model source
+        assets, etc. The specification must be YAML serializable and loadable to/from a fully initialized instance. It
+        must contain the minimal set of information necessary to find and initialize its dependencies (assets) and
+        itself.
         """
 
         _flashserve_meta_: Optional[Union[BoundMeta, UnboundMeta]] = None
 
         def __flashserve_init__(self, models, *, config=None):
             """Do a bunch of setup.
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/composition.py` & `lightning-flash-0.8.2/src/flash/core/serve/composition.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 else:
     concat, first = None, None
 
 
 def _parse_composition_kwargs(
     **kwargs: Union[ModelComponent, Endpoint]
 ) -> Tuple[Dict[str, ModelComponent], Dict[str, Endpoint]]:
-
     components, endpoints = {}, {}
     for k, v in kwargs.items():
         if isinstance(v, ModelComponent):
             components[k] = v
         elif isinstance(v, Endpoint):
             endpoints[k] = v
         else:
@@ -90,16 +89,16 @@
         self._uid_names_map = {v.uid: k for k, v in kwarg_comps.items()}
 
         self._connections = list(concat([c._flashserve_meta_.connections for c in kwarg_comps.values()]))
 
         if len(self._name_endpoints) == 0:
             comp = first(self.components.values())  # one element iterable
             ep_route = f"/{comp._flashserve_meta_.exposed.__name__}"
-            ep_inputs = {k: f"{comp.uid}.inputs.{k}" for k in asdict(comp.inputs).keys()}
-            ep_outputs = {k: f"{comp.uid}.outputs.{k}" for k in asdict(comp.outputs).keys()}
+            ep_inputs = {k: f"{comp.uid}.inputs.{k}" for k in asdict(comp.inputs)}
+            ep_outputs = {k: f"{comp.uid}.outputs.{k}" for k in asdict(comp.outputs)}
             ep = Endpoint(route=ep_route, inputs=ep_inputs, outputs=ep_outputs)
             self._name_endpoints[f"{comp._flashserve_meta_.exposed.__name__}_ENDPOINT"] = ep
 
         self._name_ep_protos = {}
         for ep_key, ep in self._name_endpoints.items():
             for ep_comp in itertools.chain(ep.inputs.values(), ep.outputs.values()):
                 uid, argtype, name = ep_comp.split(".")
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/core.py` & `lightning-flash-0.8.2/src/flash/core/serve/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch
 
 from flash.core.serve.types.base import BaseType
 from flash.core.serve.utils import download_file
 from flash.core.utilities.imports import _PYDANTIC_AVAILABLE, requires
 
 if _PYDANTIC_AVAILABLE:
-    from pydantic import FilePath, HttpUrl, parse_obj_as, ValidationError
+    from pydantic import FilePath, HttpUrl, ValidationError, parse_obj_as
 else:
     FilePath, HttpUrl, parse_obj_as, ValidationError = None, None, None, None
 
 # -------------------------------- Endpoint -----------------------------------
 
 
 @dataclass
@@ -59,15 +59,14 @@
             self.outputs[k] = str(v)
 
 
 # -------------------------------- Servable ---------------------------------
 
 
 class FlashServeScriptLoader:
-
     __slots__ = ("location", "instance")
 
     def __init__(self, location: FilePath):
         self.location = location
         self.instance = torch.jit.load(location)
 
     def __call__(self, *args, **kwargs):
@@ -113,18 +112,15 @@
             loc = args[-1]  # last element in args is always loc
             parsed = parse_obj_as(ServableValidArgs_T, tuple(args))
         except ValidationError:
             if args[0].__qualname__ != script_loader_cls.__qualname__:
                 raise
             parsed = [script_loader_cls, parse_obj_as(Union[HttpUrl, FilePath], loc)]
 
-        if isinstance(parsed[-1], Path):
-            f_path = loc
-        else:
-            f_path = download_file(loc, download_path=download_path)
+        f_path = loc if isinstance(parsed[-1], Path) else download_file(loc, download_path=download_path)
 
         if len(args) == 2 and args[0].__qualname__ != script_loader_cls.__qualname__:
             # if this is a class and path/url...
             klass = args[0]
             instance = klass.load_from_checkpoint(f_path)
         else:
             # if this is just a path/url
@@ -203,15 +199,15 @@
     position: str
     connections: List["Connection"] = field(default_factory=list, init=False, repr=False)
 
     def __str__(self):
         return f"{self.component_uid}.{self.position}.{self.name}"
 
     def __terminate_invalid_connection_request(self, other: "Parameter", dunder_meth_called: str) -> None:
-        """verify that components can be composed.
+        """Verify that components can be composed.
 
         Parameters
         ----------
         other
             object passed into the bitshift operator. We verify if is a
             ``Parameter`` class and that is not the type of the same component
         dunder_meth_called: str
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/dag/optimization.py` & `lightning-flash-0.8.2/src/flash/core/serve/dag/optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import math
 import numbers
 from enum import Enum
 
 from flash.core.serve.dag.task import flatten, get, get_dependencies, ishashable, istask, reverse_dict, subs, toposort
 from flash.core.serve.dag.utils import key_split
-from flash.core.serve.dag.utils_test import add, inc, mul
-from flash.core.utilities.imports import _SERVE_TESTING
+from flash.core.utilities.imports import _TOPIC_SERVE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _SERVE_TESTING:
+if not _TOPIC_SERVE_AVAILABLE:
     __doctest_skip__ = ["*"]
 
 
 def cull(dsk, keys):
     """Return new task graph with only the tasks required to calculate keys.
 
     In other words, remove unnecessary tasks from task graph.
     ``keys`` may be a single key or list of keys.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import add, inc
     >>> d = {'x': 1, 'y': (inc, 'x'), 'out': (add, 'x', 10)}
-    >>> dsk, dependencies = cull(d, 'out')  # doctest: +SKIP
-    >>> dsk  # doctest: +SKIP
-    {'x': 1, 'out': (add, 'x', 10)}
-    >>> dependencies  # doctest: +SKIP
-    {'x': set(), 'out': set(['x'])}
+    >>> dsk, dependencies = cull(d, 'out')
+    >>> dsk  # doctest: +ELLIPSIS
+    {'out': (<function add at ...>, 'x', 10), 'x': 1}
+    >>> dependencies
+    {'out': ['x'], 'x': []}
 
     Returns
     -------
     dsk: culled graph
     dependencies: Dict mapping {key: [deps]}.  Useful side effect to accelerate
         other optimizations, notably fuse.
     """
     if not isinstance(keys, (list, set)):
         keys = [keys]
 
     seen = set()
-    dependencies = dict()
+    dependencies = {}
     out = {}
     work = list(set(flatten(keys)))
 
     while work:
         new_work = []
         for k in work:
             dependencies_k = get_dependencies(dsk, k, as_list=True)  # fuse needs lists
@@ -92,24 +92,25 @@
         or not.  Renaming fused keys can keep the graph more understandable
         and comprehensive, but it comes at the cost of additional processing.
         If False, then the top-most key will be used.  For advanced usage, a
         func is also accepted, ``new_key = rename_keys(fused_key_list)``.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import inc
     >>> d = {'a': 1, 'b': (inc, 'a'), 'c': (inc, 'b')}
     >>> dsk, dependencies = fuse(d)
-    >>> dsk # doctest: +SKIP
-    {'a-b-c': (inc, (inc, 1)), 'c': 'a-b-c'}
+    >>> dsk  # doctest: +ELLIPSIS
+    {'c': 'a-b-c', 'a-b-c': (<function inc at ...>, (<function inc at ...>, 1))}
     >>> dsk, dependencies = fuse(d, rename_keys=False)
-    >>> dsk # doctest: +SKIP
-    {'c': (inc, (inc, 1))}
+    >>> dsk  # doctest: +ELLIPSIS
+    {'c': (<function inc at ...>, (<function inc at ...>, 1))}
     >>> dsk, dependencies = fuse(d, keys=['b'], rename_keys=False)
-    >>> dsk  # doctest: +SKIP
-    {'b': (inc, 1), 'c': (inc, 'b')}
+    >>> dsk  # doctest: +ELLIPSIS
+    {'b': (<function inc at ...>, 1), 'c': (<function inc at ...>, 'b')}
 
     Returns
     -------
     dsk: output graph with keys fused
     dependencies: dict mapping dependencies after fusion.  Useful side effect
         to accelerate other downstream optimizations.
     """
@@ -223,21 +224,22 @@
 
     Inlines all constants if ``inline_constants`` keyword is True. Note that
     the constant keys will remain in the graph, to remove them follow
     ``inline`` with ``cull``.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import add, inc
     >>> d = {'x': 1, 'y': (inc, 'x'), 'z': (add, 'x', 'y')}
-    >>> inline(d)  # doctest: +SKIP
-    {'x': 1, 'y': (inc, 1), 'z': (add, 1, 'y')}
-    >>> inline(d, keys='y')  # doctest: +SKIP
-    {'x': 1, 'y': (inc, 1), 'z': (add, 1, (inc, 1))}
-    >>> inline(d, keys='y', inline_constants=False)  # doctest: +SKIP
-    {'x': 1, 'y': (inc, 1), 'z': (add, 'x', (inc, 'x'))}
+    >>> inline(d)  # doctest: +ELLIPSIS
+    {'x': 1, 'y': (<function inc at ...>, 1), 'z': (<function add at ...>, 1, 'y')}
+    >>> inline(d, keys='y')  # doctest: +ELLIPSIS
+    {'x': 1, 'y': (<function inc at ...>, 1), 'z': (<function add at ...>, 1, (<function inc at ...>, 1))}
+    >>> inline(d, keys='y', inline_constants=False)  # doctest: +ELLIPSIS
+    {'x': 1, 'y': (<function inc at ...>, 'x'), 'z': (<function add at ...>, 'x', (<function inc at ...>, 'x'))}
     """
     if dependencies and isinstance(next(iter(dependencies.values())), list):
         dependencies = {k: set(v) for k, v in dependencies.items()}
 
     keys = _flat_set(keys)
 
     if dependencies is None:
@@ -270,31 +272,34 @@
 
 
 def inline_functions(dsk, output, fast_functions=None, inline_constants=False, dependencies=None):
     """Inline cheap functions into larger operations.
 
     Examples
     --------
-    >>> double = lambda x: x*2  # doctest: +SKIP
-    >>> dsk = {'out': (add, 'i', 'd'),  # doctest: +SKIP
+    >>> from flash.core.serve.dag.utils_test import add, inc
+    >>> double = lambda x: x*2
+    >>> dsk = {'out': (add, 'i', 'd'),
     ...        'i': (inc, 'x'),
     ...        'd': (double, 'y'),
     ...        'x': 1, 'y': 1}
-    >>> inline_functions(dsk, [], [inc])  # doctest: +SKIP
-    {'out': (add, (inc, 'x'), 'd'),
-     'd': (double, 'y'),
-     'x': 1, 'y': 1}
+    >>> inline_functions(dsk, [], [inc])  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
+    {'x': 1,
+     'out': (<function add at ...>, (<function inc at ...>, 'x'), 'd'),
+     'd': (<function <lambda> at ...>, 'y'),
+     'y': 1}
 
     Protect output keys.  In the example below ``i`` is not inlined because it
     is marked as an output key.
 
-    >>> inline_functions(dsk, ['i', 'out'], [inc, double])  # doctest: +SKIP
-    {'out': (add, 'i', (double, 'y')),
-     'i': (inc, 'x'),
-     'x': 1, 'y': 1}
+    >>> inline_functions(dsk, ['i', 'out'], [inc, double])  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
+    {'y': 1,
+     'out': (<function add at ...>, 'i', (<function <lambda> at ...>, 'y')),
+     'i': (<function inc at ...>, 'x'),
+     'x': 1}
     """
     if not fast_functions:
         return dsk
 
     output = set(output)
 
     fast_functions = set(fast_functions)
@@ -325,17 +330,18 @@
 
 
 def functions_of(task):
     """Set of functions contained within nested task.
 
     Examples
     --------
-    >>> task = (add, (mul, 1, 2), (inc, 3))  # doctest: +SKIP
-    >>> functions_of(task)  # doctest: +SKIP
-    set([add, mul, inc])
+    >>> from flash.core.serve.dag.utils_test import add, inc, mul
+    >>> task = (add, (mul, 1, 2), (inc, 3))
+    >>> sorted(functions_of(task), key=str)  # doctest: +ELLIPSIS
+    [<function add at ...>, <function inc at ...>, <function mul at ...>]
     """
     funcs = set()
 
     work = [task]
     sequence_types = {list, tuple}
 
     while work:
@@ -383,14 +389,15 @@
         first_name = key_split(first_key)
         names = {key_split(k) for k in it}
         names.discard(first_name)
         names = sorted(names)
         names.append(first_key[0])
         concatenated_name = "-".join(names)
         return (_enforce_max_key_limit(concatenated_name),) + first_key[1:]
+    return None
 
 
 # PEP-484 compliant singleton constant
 # https://www.python.org/dev/peps/pep-0484/#support-for-singleton-types-in-unions
 class Default(Enum):
     token = 0
 
@@ -489,18 +496,15 @@
         key_renamer = None
     elif not callable(rename_keys):
         raise TypeError("rename_keys must be a boolean or callable")
     else:
         key_renamer = rename_keys
     rename_keys = key_renamer is not None
 
-    if dependencies is None:
-        deps = {k: get_dependencies(dsk, k, as_list=True) for k in dsk}
-    else:
-        deps = dict(dependencies)
+    deps = {k: get_dependencies(dsk, k, as_list=True) for k in dsk} if dependencies is None else dict(dependencies)
 
     rdeps = {}
     for k, vals in deps.items():
         for v in vals:
             if v not in rdeps:
                 rdeps[v] = [k]
             else:
@@ -882,23 +886,22 @@
         self.name = name
 
     def __repr__(self):
         return self.name
 
     def __eq__(self, other):
         is_key = self.outkey == other.outkey and set(self.inkeys) == set(other.inkeys)
-        is_eq = type(self) is type(other) and self.name == other.name and is_key
-        return is_eq
+        return type(self) is type(other) and self.name == other.name and is_key
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __call__(self, *args):
         if not len(args) == len(self.inkeys):
             raise ValueError("Expected %d args, got %d" % (len(self.inkeys), len(args)))
         return get(self.dsk, self.outkey, dict(zip(self.inkeys, args)))
 
     def __reduce__(self):
         return SubgraphCallable, (self.dsk, self.outkey, self.inkeys, self.name)
 
     def __hash__(self):
-        return hash(tuple((self.outkey, tuple(self.inkeys), self.name)))
+        return hash((self.outkey, tuple(self.inkeys), self.name))
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/dag/order.py` & `lightning-flash-0.8.2/src/flash/core/serve/dag/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,20 +75,19 @@
     This relies on the regularity of graph constructors like dask.array to be a
     good proxy for ordering.  This is usually a good idea and a sane default.
 """
 
 from collections import defaultdict
 from math import log
 
-from flash.core.serve.dag.task import get_dependencies, get_deps, getcycle, reverse_dict
-from flash.core.serve.dag.utils_test import add, inc
-from flash.core.utilities.imports import _SERVE_TESTING
+from flash.core.serve.dag.task import get_dependencies, getcycle, reverse_dict
+from flash.core.utilities.imports import _TOPIC_SERVE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _SERVE_TESTING:
+if not _TOPIC_SERVE_AVAILABLE:
     __doctest_skip__ = ["*"]
 
 
 def order(dsk, dependencies=None):
     """Order nodes in the task graph.
 
     This produces an ordering over our tasks that we use to break ties when
@@ -103,14 +102,15 @@
     2.  Prefer tall branches with few dependents (start hard things first and
         try to avoid memory usage)
     3.  Prefer dependents that are dependencies of root nodes that have
         the smallest subgraph (do small goals that can terminate quickly)
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import add, inc
     >>> dsk = {'a': 1, 'b': 2, 'c': (inc, 'a'), 'd': (add, 'b', 'c')}
     >>> order(dsk)
     {'a': 0, 'c': 1, 'b': 2, 'd': 3}
     """
     if not dsk:
         return {}
 
@@ -363,15 +363,15 @@
                                 elif key < item_key:
                                     next_nodes[key].append(vals)
                                 else:
                                     later_nodes[key].append(vals)
                             if now_keys:
                                 # Run before `inner_stack` (change tactical goal!)
                                 inner_stacks_append(inner_stack)
-                                if 1 < len(now_keys):
+                                if len(now_keys) > 1:
                                     now_keys.sort(reverse=True)
                                 for key in now_keys:
                                     pool = dep_pools[key]
                                     if 1 < len(pool) < 100:
                                         pool.sort(key=dependents_key, reverse=True)
                                     inner_stacks_extend([dep] for dep in pool)
                                     seen_update(pool)
@@ -537,14 +537,16 @@
         |
         1   0
          \ /
           2
 
     Examples
     --------
+    >>> from flash.core.serve.dag.task import get_deps
+    >>> from flash.core.serve.dag.utils_test import add, inc
     >>> dsk = {'a1': 1, 'b1': (inc, 'a1'), 'b2': (inc, 'a1'), 'c1': (inc, 'b1')}
     >>> dependencies, dependents = get_deps(dsk)
     >>> _, total_dependencies = ndependencies(dependencies, dependents)
     >>> metrics = graph_metrics(dependencies, dependents, total_dependencies)
     >>> sorted(metrics.items())
     [('a1', (4, 2, 3, 1, 2)), ('b1', (2, 3, 3, 1, 1)), ('b2', (1, 2, 2, 0, 0)), ('c1', (1, 3, 3, 0, 0))]
 
@@ -611,14 +613,16 @@
     """Number of total data elements on which this key depends.
 
     For each key we return the number of tasks that must be run for us to run
     this task.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.task import get_deps
+    >>> from flash.core.serve.dag.utils_test import add, inc
     >>> dsk = {'a': 1, 'b': (inc, 'a'), 'c': (inc, 'b')}
     >>> dependencies, dependents = get_deps(dsk)
     >>> num_dependencies, total_dependencies = ndependencies(dependencies, dependents)
     >>> sorted(total_dependencies.items())
     [('a', 1), ('b', 2), ('c', 3)]
 
     Returns
@@ -654,15 +658,15 @@
 
 
 class StrComparable:
     """Wrap object so that it defaults to string comparison.
 
     When comparing two objects of different types Python fails
 
-    >>> 'a' < 1  # doctest: +SKIP
+    >>> 'a' < 1
     Traceback (most recent call last):
         ...
     TypeError: '<' not supported between instances of 'str' and 'int'
 
     This class wraps the object so that, when this would occur it instead
     compares the string representation
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/dag/rewrite.py` & `lightning-flash-0.8.2/src/flash/core/serve/dag/rewrite.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import deque
 
 from flash.core.serve.dag.task import istask, subs
-from flash.core.utilities.imports import _SERVE_TESTING
+from flash.core.utilities.imports import _TOPIC_SERVE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _SERVE_TESTING:
+if not _TOPIC_SERVE_AVAILABLE:
     __doctest_skip__ = ["*"]
 
 
 def head(task):
     """Return the top level node of a task."""
 
     if istask(task):
@@ -220,16 +220,16 @@
     ...         RewriteRule((f, (g, 'x'), 'y'),
     ...                     (h, 'x', 'y'),
     ...                     ('x', 'y')))
 
     >>> rs.rewrite((add, 2, 0))       # Apply ruleset to single task
     2
 
-    >>> rs.rewrite((f, (g, 'a', 3)))  # doctest: +SKIP
-    (h, 'a', 3)
+    >>> rs.rewrite((f, (g, 'a', 3)))  # doctest: +ELLIPSIS
+    (<function h at ...>, 'a', 3)
 
     >>> dsk = {'a': (add, 2, 0),      # Apply ruleset to full dask graph
     ...        'b': (f, (g, 'a', 3))}
 
     Attributes
     ----------
     rules : list
@@ -324,35 +324,37 @@
             or "top_level".
 
         Examples
         --------
         Suppose there was a function `add` that returned the sum of 2 numbers,
         and another function `double` that returned twice its input:
 
-        >>> add = lambda x, y: x + y
-        >>> double = lambda x: 2*x
+        >>> def add(x, y):
+        ...     return x + y
+        >>> def double(x):
+        ...     return 2*x
 
         Now suppose `double` was *significantly* faster than `add`, so
         you'd like to replace all expressions `(add, x, x)` with `(double,
         x)`, where `x` is a variable. This can be expressed as a rewrite rule:
 
         >>> rule = RewriteRule((add, 'x', 'x'), (double, 'x'), ('x',))
         >>> rs = RuleSet(rule)
 
         This can then be applied to terms to perform the rewriting:
 
         >>> term = (add, (add, 2, 2), (add, 2, 2))
-        >>> rs.rewrite(term)  # doctest: +SKIP
-        (double, (double, 2))
+        >>> rs.rewrite(term)  # doctest: +ELLIPSIS
+        (<function double at ...>, (<function double at ...>, 2))
 
         If we only wanted to apply this to the top level of the term, the
         `strategy` kwarg can be set to "top_level".
 
-        >>> rs.rewrite(term)  # doctest: +SKIP
-        (double, (add, 2, 2))
+        >>> rs.rewrite(term)  # doctest: +ELLIPSIS
+        (<function double at ...>, (<function double at ...>, 2))
         """
         return strategies[strategy](self, task)
 
 
 def _top_level(net, term):
     return net._rewrite(term)
 
@@ -403,16 +405,16 @@
             (S, N, matches) = stack.pop()
             restore_state_flag = True
         except Exception:
             return
 
 
 def _process_match(rule, syms):
-    """Process a match to determine if it is correct, and to find the correct substitution that will convert the
-    term into the pattern.
+    """Process a match to determine if it is correct, and to find the correct substitution that will convert the term
+    into the pattern.
 
     Parameters
     ----------
     rule : RewriteRule
     syms : iterable
         Iterable of subterms that match a corresponding variable.
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/dag/task.py` & `lightning-flash-0.8.2/src/flash/core/serve/dag/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections import defaultdict
 from typing import List, Sequence
 
-from flash.core.serve.dag.utils_test import add, inc
-from flash.core.utilities.imports import _SERVE_TESTING
+from flash.core.utilities.imports import _TOPIC_SERVE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _SERVE_TESTING:
+if not _TOPIC_SERVE_AVAILABLE:
     __doctest_skip__ = ["*"]
 
 no_default = "__no_default__"
 
 
 def ishashable(x):
     """Is x hashable?
@@ -25,18 +24,19 @@
         hash(x)
         return True
     except TypeError:
         return False
 
 
 def istask(x):
-    """Is x a runnable task?
-    A task is a tuple with a callable first argument
+    """Is x a runnable task? A task is a tuple with a callable first argument.
+
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import inc
     >>> istask((inc, 1))
     True
     >>> istask(1)
     False
     """
     return type(x) is tuple and x and callable(x[0])
 
@@ -61,14 +61,15 @@
 
 
 def _execute_task(arg, cache):
     """Do the actual work of collecting data and executing a function.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import add, inc
     >>> cache = {'x': 1, 'y': 2}  # Compute tasks against a cache
     >>> _execute_task((add, 'x', 1), cache)  # Compute task in naive manner
     2
     >>> _execute_task((add, (inc, 'x'), 1), cache)  # Support nested computation
     3
     >>> _execute_task('x', cache)  # Also grab data from cache
     1
@@ -107,14 +108,15 @@
     cache
         cache dict for fast in-memory lookups of previously computed results.
     sortkeys
         topologically sorted keys
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import inc
     >>> d = {'x': 1, 'y': (inc, 'x')}
     >>> get(d, 'x')
     1
     >>> get(d, 'y')
     2
     >>> get(d, 'y', sortkeys=['x', 'y'])
     2
@@ -137,25 +139,26 @@
 
 
 def get_dependencies(dsk, key=None, task=no_default, as_list=False):
     """Get the immediate tasks on which this task depends.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import add, inc
     >>> dsk = {'x': 1,
     ...        'y': (inc, 'x'),
     ...        'z': (add, 'x', 'y'),
     ...        'w': (inc, 'z'),
     ...        'a': (add, (inc, 'x'), 1)}
     >>> get_dependencies(dsk, 'x')
     set()
     >>> get_dependencies(dsk, 'y')
     {'x'}
-    >>> get_dependencies(dsk, 'z')  # doctest: +SKIP
-    {'x', 'y'}
+    >>> sorted(get_dependencies(dsk, 'z'))
+    ['x', 'y']
     >>> get_dependencies(dsk, 'w')  # Only direct dependencies
     {'z'}
     >>> get_dependencies(dsk, 'a')  # Ignore non-keys
     {'x'}
     >>> get_dependencies(dsk, task=(inc, 'x'))  # provide tasks directly
     {'x'}
     """
@@ -191,14 +194,15 @@
 
 
 def get_deps(dsk):
     """Get dependencies and dependents from task graph.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import inc
     >>> dsk = {'a': 1, 'b': (inc, 'a'), 'c': (inc, 'b')}
     >>> dependencies, dependents = get_deps(dsk)
     >>> dependencies
     {'a': set(), 'b': {'a'}, 'c': {'b'}}
     >>> dict(dependents)
     {'a': {'b'}, 'b': {'c'}, 'c': set()}
     """
@@ -230,16 +234,18 @@
                 yield item
 
 
 def reverse_dict(d):
     """
     >>> a, b, c = 'abc'
     >>> d = {a: [b, c], b: [c]}
-    >>> reverse_dict(d)  # doctest: +SKIP
-    {'a': set([]), 'b': set(['a']}, 'c': set(['a', 'b'])}
+    >>> dd = reverse_dict(d)
+    >>> from pprint import pprint
+    >>> pprint({k: sorted(v) for k, v in dd.items()})
+    {'a': [], 'b': ['a'], 'c': ['a', 'b']}
     """
     result = defaultdict(set)
     _add = set.add
     for k, vals in d.items():
         result[k]
         for val in vals:
             _add(result[val], k)
@@ -248,16 +254,17 @@
 
 
 def subs(task, key, val):
     """Perform a substitution on a task.
 
     Examples
     --------
-    >>> subs((inc, 'x'), 'x', 1)  # doctest: +SKIP
-    (inc, 1)
+    >>> from flash.core.serve.dag.utils_test import inc
+    >>> subs((inc, 'x'), 'x', 1)  # doctest: +ELLIPSIS
+    (<function inc at ...>, 1)
     """
     type_task = type(task)
     if not (type_task is tuple and task and callable(task[0])):  # istask(task):
         try:
             if type_task is type(key) and task == key:
                 return val
         except Exception:
@@ -365,31 +372,32 @@
 
 def getcycle(d, keys):
     """Return a list of nodes that form a cycle if graph is not a DAG. Returns an empty list if no cycle is found.
     ``keys`` may be a single key or list of keys.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import inc
     >>> d = {'x': (inc, 'z'), 'y': (inc, 'x'), 'z': (inc, 'y')}
     >>> getcycle(d, 'x')
     ['x', 'z', 'y', 'x']
 
     See Also
     --------
     isdag
     """
     return _toposort(d, keys=keys, returncycle=True)
 
 
 def isdag(d, keys):
-    """Does graph form a directed acyclic graph when calculating keys? ``keys`` may be a single key or list of
-    keys.
+    """Does graph form a directed acyclic graph when calculating keys? ``keys`` may be a single key or list of keys.
 
     Examples
     --------
+    >>> from flash.core.serve.dag.utils_test import inc
     >>> isdag({'x': 0, 'y': (inc, 'x')}, 'y')
     True
     >>> isdag({'x': (inc, 'y'), 'y': (inc, 'x')}, 'y')
     False
 
     See Also
     --------
@@ -418,13 +426,14 @@
 
 def quote(x):
     """Ensure that this value remains this value in a task graph Some values in task graph take on special meaning.
     Sometimes we want to ensure that our data is not interpreted but remains literal.
 
     Examples
     --------
-    >>> quote((add, 1, 2))  # doctest: +SKIP
+    >>> from flash.core.serve.dag.utils_test import add
+    >>> quote((add, 1, 2))
     (literal<type=tuple>,)
     """
     if istask(x) or type(x) is list or type(x) is dict:
         return (literal(x),)
     return x
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/dag/utils.py` & `lightning-flash-0.8.2/src/flash/core/serve/dag/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-"""
-NOTICE: Some methods in this file have been modified from their original source.
-"""
+"""NOTICE: Some methods in this file have been modified from their original source."""
 
 import functools
 import re
 from operator import methodcaller
 
-from flash.core.utilities.imports import _SERVE_TESTING
+from flash.core.utilities.imports import _TOPIC_SERVE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _SERVE_TESTING:
+if not _TOPIC_SERVE_AVAILABLE:
     __doctest_skip__ = ["*"]
 
 
 def funcname(func):
     """Get the name of a function."""
     # functools.partial
     if isinstance(func, functools.partial):
@@ -76,18 +74,15 @@
     """
     if type(s) is bytes:
         s = s.decode()
     if type(s) is tuple:
         s = s[0]
     try:
         words = s.split("-")
-        if not words[0][0].isalpha():
-            result = words[0].strip("_'()\"")
-        else:
-            result = words[0]
+        result = words[0].strip("_'()\"") if not words[0][0].isalpha() else words[0]
         for word in words[1:]:
             if word.isalpha() and not (len(word) == 8 and hex_pattern.match(word) is not None):
                 result += "-" + word
             else:
                 break
         if len(result) == 32 and re.match(r"[a-f0-9]{32}", result):
             return "data"
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/dag/visualize.py` & `lightning-flash-0.8.2/src/flash/core/serve/dag/visualize.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,10 +64,10 @@
         response_data=tc.ep_dsk_output_keys,
         no_optimization=no_optimization,
     )
     if fhandle is not None:
         data = g.pipe(format=format)
         fhandle.seek(0)
         fhandle.write(data)
-        return
+        return None
 
     return g
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/decorators.py` & `lightning-flash-0.8.2/src/flash/core/serve/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass, field, fields
 from functools import partial, wraps
 from keyword import iskeyword
 from types import FunctionType, MethodType
 from typing import Dict, List, Sequence, Tuple, Union
 from uuid import uuid4
 
-from flash.core.serve.core import Connection, make_param_dict, make_parameter_container, ParameterContainer, Servable
+from flash.core.serve.core import Connection, ParameterContainer, Servable, make_param_dict, make_parameter_container
 from flash.core.serve.types.base import BaseType
 from flash.core.serve.utils import fn_outputs_to_keyed_map
-from flash.core.utilities.imports import _CYTOOLZ_AVAILABLE, _SERVE_TESTING
+from flash.core.utilities.imports import _CYTOOLZ_AVAILABLE, _TOPIC_SERVE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _SERVE_TESTING:
+if not _TOPIC_SERVE_AVAILABLE:
     __doctest_skip__ = ["*"]
 
 if _CYTOOLZ_AVAILABLE:
     from cytoolz import compose
     from cytoolz import get as cytoolz_get
 else:
     compose, cytoolz_get = None, None
@@ -28,15 +28,14 @@
     exposed: Union[FunctionType, MethodType]
     inputs: Dict[str, BaseType]
     outputs: Dict[str, BaseType]
 
 
 @dataclass(unsafe_hash=True)
 class BoundMeta(UnboundMeta):
-
     models: Union[List["Servable"], Tuple["Servable", ...], Dict[str, "Servable"]]
     uid: str = field(default_factory=lambda: uuid4().hex, init=False)
     out_attr_dict: ParameterContainer = field(default=None, init=False)
     inp_attr_dict: ParameterContainer = field(default=None, init=False)
     dsk: Dict[str, tuple] = field(default_factory=dict, init=False)
 
     def __post_init__(self):
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/execution.py` & `lightning-flash-0.8.2/src/flash/core/serve/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from operator import attrgetter
-from typing import Dict, List, Set, Tuple, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, List, Set, Tuple
 
 from flash.core.serve.dag.optimization import cull, functions_of, inline_functions
 from flash.core.serve.dag.rewrite import RewriteRule, RuleSet
 from flash.core.serve.dag.task import flatten, get_deps, getcycle, isdag, toposort
 from flash.core.serve.dag.utils import funcname
 from flash.core.utilities.imports import _CYTOOLZ_AVAILABLE, _PYDANTIC_AVAILABLE
 
@@ -263,15 +263,15 @@
     for connection in connections:
         source_dsk = f"{connection.source_component}.outputs.{connection.source_key}"
         target_dsk = f"{connection.target_component}.inputs.{connection.target_key}"
         # value of target key is mapped one-to-one from value of source
         dsk_tgt_src_connections[target_dsk] = (identity, source_dsk)
 
     rewrite_ruleset = RuleSet()
-    for dsk_payload_target_serial in initial_task_dsk.payload_tasks_dsk.keys():
+    for dsk_payload_target_serial in initial_task_dsk.payload_tasks_dsk:
         dsk_payload_target, _serial_ident = dsk_payload_target_serial.rsplit(".", maxsplit=1)
         if _serial_ident != "serial":
             raise RuntimeError(
                 f"dsk_payload_target_serial={dsk_payload_target_serial}, "
                 f"dsk_payload_target={dsk_payload_target}, _serial_ident={_serial_ident}"
             )
         if dsk_payload_target in dsk_tgt_src_connections:
@@ -313,23 +313,22 @@
     _verify_no_cycles(inlined_culled_dsk, initial_task_dsk.output_keys, endpoint_protocol.name)
 
     # pe-run topological sort of tasks so it doesn't have to be
     # recomputed upon every request.
     toposort_keys = toposort(inlined_culled_dsk)
 
     # construct results
-    res = TaskComposition(
+    return TaskComposition(
         dsk=inlined_culled_dsk,
         sortkeys=toposort_keys,
         get_keys=initial_task_dsk.output_keys,
         ep_dsk_input_keys=initial_task_dsk.payload_dsk_map,
         ep_dsk_output_keys=initial_task_dsk.result_dsk_map,
         pre_optimization_dsk=initial_task_dsk.merged_dsk,
     )
-    return res
 
 
 def _verify_no_cycles(dsk: Dict[str, tuple], out_keys: List[str], endpoint_name: str):
     if not isdag(dsk, keys=out_keys):
         cycle = getcycle(dsk, keys=out_keys)
         raise RuntimeError(
             f"Cycle detected when attepting to build DAG for endpoint: "
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/flash_components.py` & `lightning-flash-0.8.2/src/flash/core/serve/flash_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch
 from torch import Tensor
 
 from flash.core.data.batch import _ServeInputProcessor
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import DataKeys
 from flash.core.data.io.output_transform import OutputTransform
-from flash.core.serve import expose, ModelComponent
+from flash.core.serve import ModelComponent, expose
 from flash.core.serve.types.base import BaseType
 from flash.core.trainer import Trainer
 from flash.core.utilities.stages import RunningStage
 
 
 class FlashInputs(BaseType):
     def __init__(
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/interfaces/http.py` & `lightning-flash-0.8.2/src/flash/core/serve/interfaces/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import base64
 import uuid
 from io import BytesIO
 from pathlib import Path
-from typing import Any, Callable, Dict, Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
 
 from flash.core.serve.dag.task import get
 from flash.core.serve.dag.visualize import visualize
 from flash.core.serve.execution import (
-    build_composition,
-    component_dag_content,
     ComponentJSON,
-    merged_dag_content,
     MergedJSON,
     TaskComposition,
+    build_composition,
+    component_dag_content,
+    merged_dag_content,
 )
 from flash.core.serve.interfaces.models import Alive, EndpointProtocol
 from flash.core.utilities.imports import _CYTOOLZ_AVAILABLE, _FASTAPI_AVAILABLE
 
 if _CYTOOLZ_AVAILABLE:
     from cytoolz import first
 else:
@@ -90,16 +90,15 @@
     def endpoint_visualization(request: Request):
         nonlocal dsk_composition, templates, no_optimization
         with BytesIO() as f:
             visualize(dsk_composition, fhandle=f, no_optimization=no_optimization)
             f.seek(0)
             raw = f.read()
         encoded = base64.b64encode(raw).decode("ascii")
-        res = templates.TemplateResponse("dag.html", {"request": request, "encoded_image": encoded})
-        return res
+        return templates.TemplateResponse("dag.html", {"request": request, "encoded_image": encoded})
 
     return endpoint_visualization
 
 
 def _build_dag_json(
     components: Dict[str, "ModelComponent"],
     ep_proto: Optional["EndpointProtocol"],
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/interfaces/models.py` & `lightning-flash-0.8.2/src/flash/core/serve/interfaces/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Dict, Optional, Tuple
 
 from flash.core.serve.component import ModelComponent
 from flash.core.serve.core import Endpoint
 from flash.core.serve.types import Repeated
-from flash.core.utilities.imports import _PYDANTIC_AVAILABLE, _SERVE_TESTING
+from flash.core.utilities.imports import _PYDANTIC_AVAILABLE, _TOPIC_SERVE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _SERVE_TESTING:
+if not _TOPIC_SERVE_AVAILABLE:
     __doctest_skip__ = ["EndpointProtocol.*"]
 
 if _PYDANTIC_AVAILABLE:
     from pydantic import BaseModel, create_model
 else:
     BaseModel, create_model = object, None
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/server.py` & `lightning-flash-0.8.2/src/flash/core/serve/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,13 +35,13 @@
         ----------
         host
             host address to run the server on
         port
             port number to expose the running server on
         """
         if FLASH_DISABLE_SERVE:
-            return
+            return None
 
         if not self.TESTING:  # pragma: no cover
             app = self.http_app()
             uvicorn.run(app, host=host, port=port)
         return self.http_app()
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/types/__init__.py` & `lightning-flash-0.8.2/src/flash/core/serve/types/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/types/base.py` & `lightning-flash-0.8.2/src/flash/core/serve/types/base.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/types/bbox.py` & `lightning-flash-0.8.2/src/flash/core/serve/types/bbox.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/types/image.py` & `lightning-flash-0.8.2/src/flash/core/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/types/label.py` & `lightning-flash-0.8.2/src/flash/core/serve/types/label.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/types/repeated.py` & `lightning-flash-0.8.2/src/flash/core/serve/types/repeated.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/types/table.py` & `lightning-flash-0.8.2/src/flash/core/serve/types/table.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/types/text.py` & `lightning-flash-0.8.2/src/flash/core/serve/types/text.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/serve/utils.py` & `lightning-flash-0.8.2/src/flash/core/serve/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Optional
 
 import requests
 from tqdm import tqdm
 
 
 def fn_outputs_to_keyed_map(serialize_fn_out_keys, fn_output) -> Dict[str, Any]:
-    """convert outputs of a function to a dict of `{result_name: values}`
+    """Convert outputs of a function to a dict of `{result_name: values}`
 
     accepts function outputs which are sequence, dict, or object.
     """
     if len(serialize_fn_out_keys) == 1:
         if not isinstance(fn_output, dict):
             fn_output = dict(zip(serialize_fn_out_keys, [fn_output]))
     elif not isinstance(fn_output, dict):
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/trainer.py` & `lightning-flash-0.8.2/src/flash/core/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,36 +8,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
-import math
 import warnings
 from argparse import ArgumentParser, Namespace
 from functools import wraps
 from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 from pytorch_lightning import LightningDataModule, LightningModule
 from pytorch_lightning import Trainer as PlTrainer
 from pytorch_lightning.accelerators.tpu import TPUAccelerator
 from pytorch_lightning.callbacks import BaseFinetuning
-from pytorch_lightning.utilities import rank_zero_info
 from pytorch_lightning.utilities.argparse import add_argparse_args, get_init_arguments_and_types, parse_env_variables
 from torch.utils.data import DataLoader
 
 import flash
 from flash.core.data.io.output import Output
 from flash.core.data.io.output_transform import OutputTransform
 from flash.core.data.io.transform_predictions import TransformPredictions
 from flash.core.model import Task
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _PL_GREATER_EQUAL_1_4_0, _PL_GREATER_EQUAL_1_5_0, _PL_GREATER_EQUAL_1_6_0
 
 
 def from_argparse_args(cls, args: Union[Namespace, ArgumentParser], **kwargs):
     """Modified version of :func:`pytorch_lightning.utilities.argparse.from_argparse_args` which populates
     ``valid_kwargs`` from :class:`pytorch_lightning.Trainer`."""
     if isinstance(args, ArgumentParser):
         args = cls.parse_argparser(args)
@@ -73,14 +70,20 @@
         # all args were already moved to kwargs
         return fn(self, **kwargs)
 
     return insert_env_defaults
 
 
 class Trainer(PlTrainer):
+    """Exteded Trainer for FLash tasks.
+
+    >>> Trainer()  # doctest: +ELLIPSIS
+    <...trainer.Trainer object at ...>
+    """
+
     @_defaults_from_env_vars
     def __init__(self, *args, **kwargs):
         if flash._IS_TESTING:
             if torch.cuda.is_available():
                 kwargs["gpus"] = -1
                 kwargs["limit_train_batches"] = 1.0
                 kwargs["limit_val_batches"] = 1.0
@@ -123,16 +126,16 @@
         model: LightningModule,
         train_dataloader: Optional[DataLoader] = None,
         val_dataloaders: Optional[Union[DataLoader, List[DataLoader]]] = None,
         datamodule: Optional[LightningDataModule] = None,
         strategy: Union[str, BaseFinetuning, Tuple[str, int], Tuple[str, Tuple[int, int]]] = "no_freeze",
         train_bn: bool = True,
     ):
-        r"""Runs the full optimization routine. Same as :meth:`pytorch_lightning.Trainer.fit`, but unfreezes layers
-        of the backbone throughout training layers of the backbone throughout training.
+        r"""Runs the full optimization routine. Same as :meth:`pytorch_lightning.Trainer.fit`, but unfreezes layers of
+        the backbone throughout training layers of the backbone throughout training.
 
         Args:
             model: Model to fit.
 
             train_dataloader: A PyTorch DataLoader with training samples. If the model has
                 a predefined train_dataloader method this will be skipped.
 
@@ -215,16 +218,15 @@
         finetuning_callback = model.configure_finetune_callback(strategy=strategy, train_bn=train_bn)
         if len(finetuning_callback) > 1:
             raise ValueError("Create a list with only 1 finetuning callback.")
         self.callbacks = self._merge_callbacks(self.callbacks, finetuning_callback)
 
     @staticmethod
     def _merge_callbacks(old_callbacks: List, new_callbacks: List) -> List:
-        """This function keeps only 1 instance of each callback type, extending new_callbacks with
-        old_callbacks."""
+        """This function keeps only 1 instance of each callback type, extending new_callbacks with old_callbacks."""
         if len(new_callbacks) == 0:
             return old_callbacks
         new_callbacks_types = {type(c) for c in new_callbacks}
         old_callbacks_types = {type(c) for c in old_callbacks}
         override_types = new_callbacks_types.intersection(old_callbacks_types)
         new_callbacks.extend(c for c in old_callbacks if type(c) not in override_types)
         return new_callbacks
@@ -242,62 +244,23 @@
         ``valid_kwargs`` from :class:`pytorch_lightning.Trainer`."""
         # the lightning trainer implementation does not support subclasses.
         # context: https://github.com/Lightning-AI/lightning-flash/issues/342#issuecomment-848892447
         return from_argparse_args(Trainer, args, **kwargs)
 
     @property
     def estimated_stepping_batches(self) -> Union[int, float]:
-        """Estimated stepping batches for the complete training inferred from DataLoaders, gradient accumulation
-        factor and distributed setup.
+        """Estimated stepping batches for the complete training inferred from DataLoaders, gradient accumulation factor
+        and distributed setup.
 
         Examples
         ________
 
         .. code-block:: python
 
             def configure_optimizers(self):
                 optimizer = ...
                 scheduler = torch.optim.lr_scheduler.OneCycleLR(
                     optimizer, max_lr=1e-3, total_steps=self.trainer.estimated_stepping_batches
                 )
                 return [optimizer], [scheduler]
         """
-        if _PL_GREATER_EQUAL_1_6_0:
-            return super().estimated_stepping_batches
-        # Copied from PL 1.6
-        accumulation_scheduler = self.accumulation_scheduler
-
-        if accumulation_scheduler.epochs != [0]:
-            raise ValueError(
-                "Estimated stepping batches cannot be computed with different"
-                " `accumulate_grad_batches` at different epochs."
-            )
-
-        # infinite training
-        if self.max_epochs == -1 and self.max_steps == -1:
-            return float("inf")
-
-        if self.train_dataloader is None:
-            rank_zero_info("Loading `train_dataloader` to estimate number of stepping batches.")
-            if _PL_GREATER_EQUAL_1_5_0:
-                self.reset_train_dataloader()
-            else:
-                self.reset_train_dataloader(self.lightning_module)
-
-        total_batches = self.num_training_batches
-
-        # iterable dataset
-        if total_batches == float("inf"):
-            return self.max_steps
-
-        if _PL_GREATER_EQUAL_1_4_0:
-            self.accumulate_grad_batches = accumulation_scheduler.get_accumulate_grad_batches(self.current_epoch)
-        else:
-            # Call the callback hook manually to guarantee that `self.accumulate_grad_batches` has been set
-            accumulation_scheduler.on_train_epoch_start(self, self.lightning_module)
-        effective_batch_size = self.accumulate_grad_batches
-        max_estimated_steps = math.ceil(total_batches / effective_batch_size) * max(self.max_epochs, 1)
-
-        max_estimated_steps = (
-            min(max_estimated_steps, self.max_steps) if self.max_steps not in [None, -1] else max_estimated_steps
-        )
-        return max_estimated_steps
+        return super().estimated_stepping_batches
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/apply_func.py` & `lightning-flash-0.8.2/src/flash/core/utilities/apply_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,7 +25,8 @@
         return nn.ModuleDict({get_callable_name(fn): fn})
     if isinstance(fn, Mapping):
         return fn
     if isinstance(fn, Sequence):
         return {get_callable_name(f): f for f in fn}
     if callable(fn):
         return {get_callable_name(fn): fn}
+    return None
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/compatibility.py` & `lightning-flash-0.8.2/src/flash/core/utilities/compatibility.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/embedder.py` & `lightning-flash-0.8.2/src/flash/core/utilities/embedder.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/flash_cli.py` & `lightning-flash-0.8.2/src/flash/core/utilities/flash_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,21 @@
 import inspect
 from argparse import Namespace
 from functools import wraps
 from inspect import Parameter, signature
 from typing import Any, Callable, Dict, List, Optional, Set, Type, Union
 
 import pytorch_lightning as pl
-from jsonargparse import ArgumentParser
-from jsonargparse.signatures import get_class_signature_functions
+from jsonargparse import ArgumentParser, class_from_function
+from lightning_utilities.core.overrides import is_overridden
 from pytorch_lightning import LightningModule, Trainer
-from pytorch_lightning.utilities.model_helpers import is_overridden
 
 import flash
 from flash.core.data.data_module import DataModule
 from flash.core.utilities.lightning_cli import (
-    class_from_function,
     LightningArgumentParser,
     LightningCLI,
     SaveConfigCallback,
 )
 from flash.core.utilities.stability import beta
 
 
@@ -103,23 +101,32 @@
 
     sig = sig.replace(parameters=parameters, return_annotation=cls)
     wrapper.__signature__ = sig
 
     return wrapper
 
 
+def get_class_signature_functions(classes):
+    signatures = []
+    for num, cls in enumerate(classes):
+        if cls.__new__ is not object.__new__ and not any(cls.__new__ is c.__new__ for c in classes[num + 1 :]):
+            signatures.append((cls, cls.__new__))
+        if not any(cls.__init__ is c.__init__ for c in classes[num + 1 :]):
+            signatures.append((cls, cls.__init__))
+    return signatures
+
+
 def get_overlapping_args(func_a, func_b) -> Set[str]:
     func_a = get_class_signature_functions([func_a])[0][1]
     func_b = get_class_signature_functions([func_b])[0][1]
     return set(inspect.signature(func_a).parameters.keys() & inspect.signature(func_b).parameters.keys())
 
 
 @beta("Flash Zero is currently in Beta.")
 class FlashCLI(LightningCLI):
-
     datamodule: DataModule
     config_init: Namespace
     model: LightningModule
 
     def __init__(
         self,
         model_class: Type[pl.LightningModule],
@@ -189,35 +196,37 @@
     def parse_arguments(self) -> None:
         with self.patch_default_subcommand():
             super().parse_arguments()
 
     def add_arguments_to_parser(self, parser) -> None:
         subcommands = parser.add_subcommands()
 
-        for function in vars(self.local_datamodule_class).keys():
+        for function in vars(self.local_datamodule_class):
             if not function.startswith("from"):
                 continue
-            if (
-                hasattr(DataModule, function) and is_overridden(function, self.local_datamodule_class, DataModule)
-            ) or not hasattr(DataModule, function):
-                if getattr(self.local_datamodule_class, function, None) is not None:
-                    self.add_subcommand_from_function(subcommands, getattr(self.local_datamodule_class, function))
+            _data_overwritten = hasattr(DataModule, function) and is_overridden(
+                function, self.local_datamodule_class, DataModule
+            )
+            if (_data_overwritten or not hasattr(DataModule, function)) and getattr(
+                self.local_datamodule_class, function, None
+            ) is not None:
+                self.add_subcommand_from_function(subcommands, getattr(self.local_datamodule_class, function))
 
         for datamodule_builder in self.additional_datamodule_builders:
             self.add_subcommand_from_function(subcommands, datamodule_builder)
 
         if self.default_datamodule_builder is not None:
             self.add_subcommand_from_function(subcommands, self.default_datamodule_builder)
 
         parser.set_defaults(self.default_arguments)
 
     def add_subcommand_from_function(self, subcommands, function, function_name=None):
         subcommand = ArgumentParser()
         if get_kwarg_name(function) == "data_module_kwargs":
-            datamodule_function = class_from_function(function, return_type=self.local_datamodule_class)
+            datamodule_function = class_from_function(function, self.local_datamodule_class)
             subcommand.add_class_arguments(
                 datamodule_function,
                 fail_untyped=False,
                 skip={
                     "self",
                     "train_dataset",
                     "val_dataset",
@@ -228,29 +237,31 @@
                     "test_input",
                     "predict_input",
                     "input",
                     "input_transform",
                 },
             )
         else:
-            datamodule_function = class_from_function(drop_kwargs(function), return_type=self.local_datamodule_class)
+            datamodule_function = class_from_function(drop_kwargs(function), self.local_datamodule_class)
             subcommand.add_class_arguments(datamodule_function, fail_untyped=False)
         subcommand_name = function_name or function.__name__
         subcommands.add_subcommand(subcommand_name, subcommand)
         self._subcommand_builders[subcommand_name] = function
 
     def instantiate_classes(self) -> None:
         """Instantiates the classes using settings from self.config."""
         sub_config = self.config.get("subcommand")
         self.datamodule = self._subcommand_builders[sub_config](**self.config.get(sub_config))
 
         for datamodule_attribute in self.datamodule_attributes:
-            if datamodule_attribute in self.config["model"]:
-                if getattr(self.datamodule, datamodule_attribute, None) is not None:
-                    self.config["model"][datamodule_attribute] = getattr(self.datamodule, datamodule_attribute)
+            if (
+                datamodule_attribute in self.config["model"]
+                and getattr(self.datamodule, datamodule_attribute, None) is not None
+            ):
+                self.config["model"][datamodule_attribute] = getattr(self.datamodule, datamodule_attribute)
         self.config_init = self.parser.instantiate_classes(self.config)
         self.model = self.config_init["model"]
         self.instantiate_trainer()
 
     def prepare_fit_kwargs(self):
         super().prepare_fit_kwargs()
         if self.finetune:
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/isinstance.py` & `lightning-flash-0.8.2/src/flash/core/utilities/isinstance.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/lightning_cli.py` & `lightning-flash-0.8.2/src/flash/core/utilities/lightning_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,41 @@
 # Adapted from the Lightning CLI:
 # https://github.com/Lightning-AI/lightning/blob/master/src/pytorch_lightning/utilities/cli.py
 import inspect
 import os
 import warnings
 from argparse import Namespace
-from functools import wraps
 from types import MethodType
-from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union, cast
 
 import torch
-from jsonargparse import ActionConfigFile, ArgumentParser, set_config_read_mode
-from jsonargparse.signatures import ClassFromFunctionBase
-from jsonargparse.typehints import ClassType
+from jsonargparse import ActionConfigFile, ArgumentParser, class_from_function, set_config_read_mode
+from pytorch_lightning import LightningDataModule, LightningModule, Trainer
 from pytorch_lightning.callbacks import Callback
-from pytorch_lightning.core.datamodule import LightningDataModule
-from pytorch_lightning.core.lightning import LightningModule
-from pytorch_lightning.trainer.trainer import Trainer
 from pytorch_lightning.utilities.cloud_io import get_filesystem
 from pytorch_lightning.utilities.model_helpers import is_overridden
 from pytorch_lightning.utilities.seed import seed_everything
 from torch.optim import Optimizer
 
 set_config_read_mode(fsspec_enabled=True)
 
 LRSchedulerTypeTuple = (torch.optim.lr_scheduler._LRScheduler, torch.optim.lr_scheduler.ReduceLROnPlateau)
 LRSchedulerType = Union[Type[torch.optim.lr_scheduler._LRScheduler], Type[torch.optim.lr_scheduler.ReduceLROnPlateau]]
 
 
-def class_from_function(
-    func: Callable[..., ClassType],
-    return_type: Optional[Type[ClassType]] = None,
-) -> Type[ClassType]:
-    """Creates a dynamic class which if instantiated is equivalent to calling func.
-
-    Args:
-        func: A function that returns an instance of a class. It must have a return type annotation.
-    """
-
-    @wraps(func)
-    def __new__(cls, *args, **kwargs):
-        return func(*args, **kwargs)
-
-    if return_type is None:
-        return_type = inspect.signature(func).return_annotation
-
-    if isinstance(return_type, str):
-        raise RuntimeError("Classmethod instantiation is not supported when the return type annotation is a string.")
-
-    class ClassFromFunction(return_type, ClassFromFunctionBase):  # type: ignore
-        pass
-
-    ClassFromFunction.__new__ = __new__  # type: ignore
-    ClassFromFunction.__doc__ = func.__doc__
-    ClassFromFunction.__name__ = func.__name__
-
-    return ClassFromFunction
-
-
 class LightningArgumentParser(ArgumentParser):
     """Extension of jsonargparse's ArgumentParser for pytorch-lightning."""
 
-    def __init__(self, *args: Any, parse_as_dict: bool = True, **kwargs: Any) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initialize argument parser that supports configuration file input.
 
-        For full details of accepted arguments see `ArgumentParser.__init__
-        <https://jsonargparse.readthedocs.io/en/stable/#jsonargparse.core.ArgumentParser.__init__>`_.
+        For full details of accepted arguments see
+        `ArgumentParser.__init__ <https://jsonargparse.readthedocs.io/en/stable/#jsonargparse.core.ArgumentParser.__init__>`_.
         """
-        super().__init__(*args, parse_as_dict=parse_as_dict, **kwargs)
+        super().__init__(*args, **kwargs)
         self.add_argument(
             "--config", action=ActionConfigFile, help="Path to a configuration file in json or yaml format."
         )
         self.callback_keys: List[str] = []
         self.optimizers_and_lr_schedulers: Dict[str, Tuple[Union[Type, Tuple[Type, ...]], str]] = {}
 
     def add_lightning_class_args(
@@ -93,15 +58,15 @@
             subclass_mode: Whether allow any subclass of the given class.
         """
         if callable(lightning_class) and not inspect.isclass(lightning_class):
             lightning_class = class_from_function(lightning_class)
 
         if inspect.isclass(lightning_class) and issubclass(
             cast(type, lightning_class),
-            (Trainer, LightningModule, LightningDataModule, Callback, ClassFromFunctionBase),
+            (Trainer, LightningModule, LightningDataModule, Callback),
         ):
             if issubclass(cast(type, lightning_class), Callback):
                 self.callback_keys.append(nested_key)
             if subclass_mode:
                 return self.add_subclass_arguments(lightning_class, nested_key, required=True)
             return self.add_class_arguments(
                 lightning_class,
@@ -243,19 +208,19 @@
         description: str = "pytorch-lightning trainer command line tool",
         env_prefix: str = "PL",
         env_parse: bool = False,
         parser_kwargs: Dict[str, Any] = None,
         subclass_mode_model: bool = False,
         subclass_mode_data: bool = False,
     ) -> None:
-        """Receives as input pytorch-lightning classes (or callables which return pytorch-lightning classes), which
-        are called / instantiated using a parsed configuration file and / or command line args and then runs
-        trainer.fit. Parsing of configuration from environment variables can be enabled by setting
-        ``env_parse=True``. A full configuration yaml would be parsed from ``PL_CONFIG`` if set. Individual
-        settings are so parsed from variables named for example ``PL_TRAINER__MAX_EPOCHS``.
+        """Receives as input pytorch-lightning classes (or callables which return pytorch-lightning classes), which are
+        called / instantiated using a parsed configuration file and / or command line args and then runs trainer.fit.
+        Parsing of configuration from environment variables can be enabled by setting ``env_parse=True``. A full
+        configuration yaml would be parsed from ``PL_CONFIG`` if set. Individual settings are so parsed from variables
+        named for example ``PL_TRAINER__MAX_EPOCHS``.
 
         Example, first implement the ``trainer.py`` tool as::
 
             from mymodels import MyModel
             from pytorch_lightning.utilities.cli import LightningCLI
             LightningCLI(MyModel)
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/providers.py` & `lightning-flash-0.8.2/src/flash/core/utilities/providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from dataclasses import dataclass
 
 PROVIDERS = []  #: testing
 
 
 @dataclass
 class Provider:
-
     name: str
     url: str
 
     def __post_init__(self):
         PROVIDERS.append(self)
 
     def __str__(self):
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/stability.py` & `lightning-flash-0.8.2/src/flash/core/utilities/stability.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,35 +13,35 @@
 # limitations under the License.
 import functools
 import inspect
 from typing import Callable, Type, Union
 
 from pytorch_lightning.utilities import rank_zero_warn
 
-from flash.core.utilities.imports import _CORE_TESTING
+from flash.core.utilities.imports import _TOPIC_CORE_AVAILABLE
 
 # Skip doctests if requirements aren't available
-if not _CORE_TESTING:
+if not _TOPIC_CORE_AVAILABLE:
     __doctest_skip__ = ["beta"]
 
 
-@functools.lru_cache()  # Trick to only warn once for each message
+@functools.lru_cache  # Trick to only warn once for each message
 def _raise_beta_warning(message: str, stacklevel: int = 6):
     rank_zero_warn(
         f"{message} The API and functionality may change without warning in future releases. "
         "More details: https://lightning-flash.readthedocs.io/en/latest/stability.html",
         stacklevel=stacklevel,
         category=UserWarning,
     )
 
 
 def beta(message: str = "This feature is currently in Beta."):
-    """The beta decorator is used to indicate that a particular feature is in Beta. A callable or type that has
-    been marked as beta will give a ``UserWarning`` when it is called or instantiated. This designation should be
-    used following the description given in :ref:`stability`.
+    """The beta decorator is used to indicate that a particular feature is in Beta. A callable or type that has been
+    marked as beta will give a ``UserWarning`` when it is called or instantiated. This designation should be used
+    following the description given in :ref:`stability`.
 
     Args:
         message: The message to include in the warning.
 
     Examples
     ________
```

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/stages.py` & `lightning-flash-0.8.2/src/flash/core/utilities/stages.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/types.py` & `lightning-flash-0.8.2/src/flash/core/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/core/utilities/url_error.py` & `lightning-flash-0.8.2/src/flash/core/utilities/url_error.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/graph/backbones.py` & `lightning-flash-0.8.2/src/flash/graph/backbones.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from functools import partial
 
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _GRAPH_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_GRAPH_AVAILABLE
 from flash.core.utilities.providers import _PYTORCH_GEOMETRIC
 
-if _GRAPH_AVAILABLE:
+if _TOPIC_GRAPH_AVAILABLE:
     from torch_geometric.nn.models import GAT, GCN, GIN, GraphSAGE
 
     MODELS = {"GCN": GCN, "GraphSAGE": GraphSAGE, "GAT": GAT, "GIN": GIN}
 else:
     MODELS = {}
 
 GRAPH_BACKBONES = FlashRegistry("backbones")
@@ -33,9 +33,9 @@
     hidden_channels: int = 512,
     num_layers: int = 4,
 ):
     model = MODELS[model_name]
     return model(in_channels, hidden_channels, num_layers)
 
 
-for model_name in MODELS.keys():
+for model_name in MODELS:
     GRAPH_BACKBONES(name=model_name, providers=_PYTORCH_GEOMETRIC)(partial(_load_graph_backbone, model_name))
```

### Comparing `lightning-flash-0.8.1.post0/flash/graph/classification/cli.py` & `lightning-flash-0.8.2/src/flash/graph/classification/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/graph/classification/data.py` & `lightning-flash-0.8.2/src/flash/graph/classification/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 from typing import Dict, Optional, Type
 
 from torch.utils.data import Dataset
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.utilities.classification import TargetFormatter
-from flash.core.utilities.imports import _GRAPH_TESTING
+from flash.core.utilities.imports import _TOPIC_GRAPH_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.graph.classification.input import GraphClassificationDatasetInput
 from flash.graph.classification.input_transform import GraphClassificationInputTransform
 
 # Skip doctests if requirements aren't available
-if not _GRAPH_TESTING:
+if not _TOPIC_GRAPH_AVAILABLE:
     __doctest_skip__ = ["GraphClassificationData", "GraphClassificationData.*"]
 
 
 class GraphClassificationData(DataModule):
     """The ``GraphClassificationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for graph classification."""
 
@@ -162,17 +162,17 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_dataset, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_dataset, **ds_kw),
```

### Comparing `lightning-flash-0.8.1.post0/flash/graph/classification/input.py` & `lightning-flash-0.8.2/src/flash/graph/classification/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 from torch.utils.data import Dataset
 
 from flash.core.data.io.classification_input import ClassificationInputMixin
 from flash.core.data.io.input import DataKeys, Input
 from flash.core.data.utilities.classification import TargetFormatter
 from flash.core.data.utilities.samples import to_sample
-from flash.core.utilities.imports import _GRAPH_AVAILABLE, requires
+from flash.core.utilities.imports import _TOPIC_GRAPH_AVAILABLE, requires
 
-if _GRAPH_AVAILABLE:
+if _TOPIC_GRAPH_AVAILABLE:
     from torch_geometric.data import Data, InMemoryDataset
 
 
 def _get_num_features(sample: Dict[str, Any]) -> Optional[int]:
     """Get the number of features per node in the given dataset."""
     data = sample[DataKeys.INPUT]
     data = data[0] if isinstance(data, tuple) else data
```

### Comparing `lightning-flash-0.8.1.post0/flash/graph/classification/input_transform.py` & `lightning-flash-0.8.2/src/flash/graph/classification/input_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 from dataclasses import dataclass
 from typing import Any, Callable, Dict
 
 from flash.core.data.io.input import DataKeys
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.utilities.samples import to_sample
-from flash.core.utilities.imports import _GRAPH_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_GRAPH_AVAILABLE
 from flash.graph.collate import _pyg_collate
 
-if _GRAPH_AVAILABLE:
+if _TOPIC_GRAPH_AVAILABLE:
     from torch_geometric.data import Data
     from torch_geometric.transforms import NormalizeFeatures
 else:
     Data = object
 
 
 @dataclass
```

### Comparing `lightning-flash-0.8.1.post0/flash/graph/classification/model.py` & `lightning-flash-0.8.2/src/flash/graph/classification/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from torch import nn, Tensor
-from torch.nn import functional as F
+from torch import Tensor, nn
 from torch.nn import Linear
+from torch.nn import functional as F
 
 from flash.core.classification import ClassificationTask
 from flash.core.data.io.input import DataKeys
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _GRAPH_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_GRAPH_AVAILABLE
 from flash.core.utilities.types import LOSS_FN_TYPE, LR_SCHEDULER_TYPE, METRICS_TYPE, OPTIMIZER_TYPE
 from flash.graph.backbones import GRAPH_BACKBONES
 from flash.graph.collate import _pyg_collate
 
-if _GRAPH_AVAILABLE:
+if _TOPIC_GRAPH_AVAILABLE:
     from torch_geometric.nn import global_add_pool, global_max_pool, global_mean_pool
 
     POOLING_FUNCTIONS = {"mean": global_mean_pool, "add": global_add_pool, "max": global_max_pool}
 else:
     POOLING_FUNCTIONS = {}
```

### Comparing `lightning-flash-0.8.1.post0/flash/graph/collate.py` & `lightning-flash-0.8.2/src/flash/graph/collate.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List
 
 from torch.utils.data.dataloader import default_collate
 
 from flash.core.data.io.input import DataKeys
-from flash.core.utilities.imports import _GRAPH_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_GRAPH_AVAILABLE
 
-if _GRAPH_AVAILABLE:
+if _TOPIC_GRAPH_AVAILABLE:
     from torch_geometric.data import Batch
 
 
 def _pyg_collate(samples: List[Dict[str, Any]]) -> Dict[str, Any]:
-    """Helper to collate PyTorch Geometric ``Data`` objects into PyTorch Geometric ``Batch`` objects whilst
-    preserving our dictionary format."""
+    """Helper to collate PyTorch Geometric ``Data`` objects into PyTorch Geometric ``Batch`` objects whilst preserving
+    our dictionary format."""
     inputs = Batch.from_data_list([sample[DataKeys.INPUT] for sample in samples])
     if DataKeys.TARGET in samples[0]:
         targets = default_collate([sample[DataKeys.TARGET] for sample in samples])
         return {DataKeys.INPUT: inputs, DataKeys.TARGET: targets}
     return {DataKeys.INPUT: inputs}
```

### Comparing `lightning-flash-0.8.1.post0/flash/graph/embedding/model.py` & `lightning-flash-0.8.2/src/flash/graph/embedding/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Callable, Dict, IO, Optional, Union
+from typing import IO, Any, Callable, Dict, Optional, Union
 
 import torch
-from torch import nn, Tensor
+from torch import Tensor, nn
 
 from flash.core.data.io.input import DataKeys
 from flash.core.model import Task
-from flash.graph.classification.model import GraphClassifier, POOLING_FUNCTIONS
+from flash.graph.classification.model import POOLING_FUNCTIONS, GraphClassifier
 from flash.graph.collate import _pyg_collate
 
 
 class GraphEmbedder(Task):
-    """The ``GraphEmbedder`` is a :class:`~flash.Task` for obtaining feature vectors (embeddings) from graphs. For
-    more details, see :ref:`graph_embedder`.
+    """The ``GraphEmbedder`` is a :class:`~flash.Task` for obtaining feature vectors (embeddings) from graphs. For more
+    details, see :ref:`graph_embedder`.
 
     Args:
         backbone: A model to use to extract image features.
         pooling_fn: The global pooling operation to use (one of: "max", "max", "add" or a callable).
     """
 
     required_extras: str = "graph"
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/__init__.py` & `lightning-flash-0.8.2/src/flash/image/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/adapters.py` & `lightning-flash-0.8.2/src/flash/image/classification/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,36 +17,32 @@
 from collections import defaultdict
 from functools import partial
 from typing import Any, Callable, List, Optional, Type
 
 import torch
 from lightning_utilities.core.rank_zero import WarningCache
 from pytorch_lightning import LightningModule
+from pytorch_lightning.strategies import DataParallelStrategy, DDPSpawnStrategy, DDPStrategy
 from pytorch_lightning.trainer.states import TrainerFn
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.utils.data import DataLoader, IterableDataset, Sampler
 
 import flash
 from flash.core.adapter import Adapter, AdapterTask
 from flash.core.data.io.input import DataKeys, InputBase
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.model import Task
 from flash.core.registry import FlashRegistry
 from flash.core.utilities.compatibility import accelerator_connector
-from flash.core.utilities.imports import _LEARN2LEARN_AVAILABLE, _PL_GREATER_EQUAL_1_6_0
+from flash.core.utilities.imports import _LEARN2LEARN_AVAILABLE
 from flash.core.utilities.providers import _LEARN2LEARN
 from flash.core.utilities.stability import beta
 from flash.core.utilities.url_error import catch_url_error
 from flash.image.classification.integrations.learn2learn import TaskDataParallel, TaskDistributedDataParallel
 
-if _PL_GREATER_EQUAL_1_6_0:
-    from pytorch_lightning.strategies import DataParallelStrategy, DDPSpawnStrategy, DDPStrategy
-else:
-    from pytorch_lightning.plugins import DataParallelPlugin, DDPPlugin, DDPSpawnPlugin
-
 warning_cache = WarningCache()
 
 
 if _LEARN2LEARN_AVAILABLE:
     import learn2learn as l2l
     from learn2learn.data.transforms import RemapLabels as Learn2LearnRemapLabels
 else:
@@ -75,15 +71,14 @@
         if self.head is None:
             return x
         return self.head(x)
 
 
 @beta("The Learn2Learn integration is currently in Beta.")
 class Learn2LearnAdapter(Adapter):
-
     required_extras: str = "image"
 
     def __init__(
         self,
         backbone: nn.Module,
         head: nn.Module,
         algorithm_cls: Type[LightningModule],
@@ -98,16 +93,16 @@
         test_shots: Optional[int] = None,
         test_queries: Optional[int] = None,
         test_num_task: Optional[int] = None,
         default_transforms_fn: Optional[Callable] = None,
         seed: int = 42,
         **algorithm_kwargs,
     ):
-        """The ``Learn2LearnAdapter`` is an :class:`~flash.core.adapter.Adapter` for integrating with `learn 2
-        learn` library (https://github.com/learnables/learn2learn).
+        """The ``Learn2LearnAdapter`` is an :class:`~flash.core.adapter.Adapter` for integrating with `learn 2 learn`
+        library (https://github.com/learnables/learn2learn).
 
         Args:
             task: Task to be used. This adapter should work with any Flash Classification task
             backbone: Feature extractor to be used.
             head: Predictive head.
             algorithm_cls: Algorithm class coming
                 from: https://github.com/learnables/learn2learn/tree/master/learn2learn/algorithms/lightning
@@ -212,15 +207,14 @@
     ):
         if trainer is None:
             raise ValueError(
                 "The Learn2Learn integration requires the `Trainer` to be passed to the `process_*_dataset` method."
             )
 
         if isinstance(dataset, InputBase):
-
             metadata = getattr(dataset, "data", None)
             if metadata is None or (metadata is not None and not isinstance(dataset.data, list)):
                 raise TypeError("Only dataset built out of metadata is supported.")
 
             labels_to_indices = self._labels_to_indices(dataset.data)
 
             if len(labels_to_indices) < ways:
@@ -239,18 +233,15 @@
             taskset = l2l.data.TaskDataset(
                 dataset=dataset,
                 task_transforms=transform_fn(dataset, ways=ways, shots=shots, queries=queries),
                 num_tasks=num_task,
                 task_collate=self._identity_task_collate_fn,
             )
 
-        if _PL_GREATER_EQUAL_1_6_0:
-            is_ddp_or_ddp_spawn = isinstance(trainer.strategy, (DDPStrategy, DDPSpawnStrategy))
-        else:
-            is_ddp_or_ddp_spawn = isinstance(trainer.training_type_plugin, (DDPPlugin, DDPSpawnPlugin))
+        is_ddp_or_ddp_spawn = isinstance(trainer.strategy, (DDPStrategy, DDPSpawnStrategy))
         if is_ddp_or_ddp_spawn:
             # when running in a distributed data parallel way,
             # we are actually sampling one task per device.
             dataset = TaskDistributedDataParallel(
                 taskset=taskset,
                 global_rank=trainer.global_rank,
                 world_size=trainer.world_size,
@@ -258,18 +249,15 @@
                 epoch_length=epoch_length,
                 seed=os.getenv("PL_GLOBAL_SEED", self.seed),
                 requires_divisible=trainer.training,
             )
             self.trainer.accumulated_grad_batches = self.meta_batch_size / trainer.world_size
         else:
             devices = 1
-            if _PL_GREATER_EQUAL_1_6_0:
-                is_data_parallel = isinstance(trainer.strategy, DataParallelStrategy)
-            else:
-                is_data_parallel = isinstance(trainer.training_type_plugin, DataParallelPlugin)
+            is_data_parallel = isinstance(trainer.strategy, DataParallelStrategy)
             if is_data_parallel:
                 # when using DP, we need to sample n tasks, so it can split across multiple devices.
                 devices = accelerator_connector(trainer).devices
             dataset = TaskDataParallel(taskset, epoch_length=epoch_length, devices=devices, collate_fn=None)
             self.trainer.accumulated_grad_batches = self.meta_batch_size / devices
 
         return dataset
@@ -459,15 +447,14 @@
         shuffle: bool = False,
         drop_last: bool = False,
         sampler: Optional[Sampler] = None,
         persistent_workers: bool = False,
         input_transform: Optional[InputTransform] = None,
         trainer: Optional["flash.Trainer"] = None,
     ) -> DataLoader:
-
         if not self._algorithm_has_validated:
             raise RuntimeError(
                 "This training strategy needs to be validated before it can be used for prediction."
                 " Call trainer.validate(...)."
             )
 
         return super().process_predict_dataset(
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/backbones/__init__.py` & `lightning-flash-0.8.2/src/flash/image/classification/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/backbones/clip.py` & `lightning-flash-0.8.2/src/flash/image/classification/backbones/clip.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/backbones/resnet.py` & `lightning-flash-0.8.2/src/flash/image/classification/backbones/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
         width_per_group: int = 64,
         replace_stride_with_dilation: Optional[List[bool]] = None,
         norm_layer: Optional[Callable[..., nn.Module]] = None,
         first_conv3x3: bool = False,
         remove_first_maxpool: bool = False,
         in_chans: int = 3,
     ) -> None:
-
         super().__init__()
 
         if norm_layer is None:
             norm_layer = nn.BatchNorm2d
         self._norm_layer = norm_layer
 
         self.inplanes = width_per_group * widen
@@ -311,15 +310,14 @@
     block: Type[Union[BasicBlock, Bottleneck]],
     layers: List[int],
     num_features: int,
     pretrained: Union[bool, str] = True,
     weights_paths: dict = {"supervised": None},
     **kwargs: Any,
 ) -> ResNet:
-
     pretrained_flag = (pretrained and isinstance(pretrained, bool)) or (pretrained == "supervised")
 
     backbone = ResNet(block, layers, **kwargs)
     device = next(backbone.parameters()).get_device()
 
     model_weights = None
     if pretrained_flag:
@@ -336,15 +334,15 @@
 
     if not pretrained_flag and isinstance(pretrained, str):
         if pretrained in weights_paths:
             model_weights = load_state_dict_from_url(
                 weights_paths[pretrained], map_location=torch.device("cpu") if device == -1 else torch.device(device)
             )
 
-            if "classy_state_dict" in model_weights.keys():
+            if "classy_state_dict" in model_weights:
                 model_weights = model_weights["classy_state_dict"]["base_model"]["model"]["trunk"]
                 model_weights = {
                     key.replace("_feature_blocks.", "") if "_feature_blocks." in key else key: val
                     for (key, val) in model_weights.items()
                 }
             else:
                 raise KeyError("Unrecognized state dict. Logic for loading the current state dict missing.")
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/backbones/timm.py` & `lightning-flash-0.8.2/src/flash/image/classification/backbones/timm.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         num_features = backbone.num_features
         return backbone, num_features
 
 
 def register_timm_backbones(register: FlashRegistry):
     if _TIMM_AVAILABLE:
         for model_name in timm.list_models():
-
             if model_name in TORCHVISION_MODELS:
                 continue
 
             register(
                 fn=catch_url_error(partial(_fn_timm, model_name)),
                 name=model_name,
                 namespace="vision",
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/backbones/torchvision.py` & `lightning-flash-0.8.2/src/flash/image/classification/backbones/torchvision.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/backbones/transformers.py` & `lightning-flash-0.8.2/src/flash/image/classification/backbones/transformers.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/cli.py` & `lightning-flash-0.8.2/src/flash/image/classification/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/data.py` & `lightning-flash-0.8.2/src/flash/image/classification/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 from flash.core.data.base_viz import BaseVisualization
 from flash.core.data.callback import BaseDataFetcher
 from flash.core.data.data_module import DataModule, DatasetInput
 from flash.core.data.io.input import DataKeys, Input
 from flash.core.data.io.input_transform import INPUT_TRANSFORM_TYPE
 from flash.core.data.utilities.classification import TargetFormatter
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.integrations.labelstudio.input import _parse_labelstudio_arguments, LabelStudioImageClassificationInput
+from flash.core.integrations.labelstudio.input import LabelStudioImageClassificationInput, _parse_labelstudio_arguments
 from flash.core.utilities.imports import (
     _FIFTYONE_AVAILABLE,
-    _IMAGE_EXTRAS_TESTING,
-    _IMAGE_TESTING,
     _MATPLOTLIB_AVAILABLE,
+    _TOPIC_IMAGE_AVAILABLE,
     Image,
     requires,
 )
 from flash.core.utilities.stages import RunningStage
 from flash.image.classification.input import (
     ImageClassificationCSVInput,
     ImageClassificationDataFrameInput,
@@ -43,38 +42,26 @@
     ImageClassificationFolderInput,
     ImageClassificationImageInput,
     ImageClassificationNumpyInput,
     ImageClassificationTensorInput,
 )
 from flash.image.classification.input_transform import ImageClassificationInputTransform
 
-if _FIFTYONE_AVAILABLE:
-    SampleCollection = "fiftyone.core.collections.SampleCollection"
-else:
-    SampleCollection = None
+SampleCollection = "fiftyone.core.collections.SampleCollection" if _FIFTYONE_AVAILABLE else None
 
 if _MATPLOTLIB_AVAILABLE:
     import matplotlib.pyplot as plt
 else:
     plt = None
 
 # Skip doctests if requirements aren't available
 __doctest_skip__ = []
-if not _IMAGE_TESTING:
-    __doctest_skip__ += [
-        "ImageClassificationData",
-        "ImageClassificationData.from_files",
-        "ImageClassificationData.from_folders",
-        "ImageClassificationData.from_numpy",
-        "ImageClassificationData.from_images",
-        "ImageClassificationData.from_tensors",
-        "ImageClassificationData.from_data_frame",
-        "ImageClassificationData.from_csv",
-    ]
-if not _IMAGE_EXTRAS_TESTING:
+if not _TOPIC_IMAGE_AVAILABLE:
+    __doctest_skip__ += ["ImageClassificationData", "ImageClassificationData.*"]
+if not _FIFTYONE_AVAILABLE:
     __doctest_skip__ += ["ImageClassificationData.from_fiftyone"]
 
 
 class ImageClassificationData(DataModule):
     """The ``ImageClassificationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for image classification."""
 
@@ -159,17 +146,17 @@
 
         .. testcleanup::
 
             >>> import os
             >>> _ = [os.remove(f"image_{i}.png") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_image_{i}.png") for i in range(1, 4)]
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_files, train_targets, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_files, val_targets, **ds_kw),
@@ -189,16 +176,15 @@
         predict_folder: Optional[str] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ImageClassificationFolderInput,
         transform: INPUT_TRANSFORM_TYPE = ImageClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ImageClassificationData":
-        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from folders containing
-        images.
+        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from folders containing images.
 
         The supported file extensions are: ``.jpg``, ``.jpeg``, ``.png``, ``.ppm``, ``.bmp``, ``.pgm``, ``.tif``,
         ``.tiff``, ``.webp``, and ``.npy``.
         For train, test, and validation data, the folders are expected to contain a sub-folder for each class.
         Here's the required structure:
 
         .. code-block::
@@ -280,17 +266,17 @@
 
         .. testcleanup::
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_folder, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_folder, **ds_kw),
@@ -313,16 +299,16 @@
         predict_data: Optional[Collection[np.ndarray]] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ImageClassificationNumpyInput,
         transform: INPUT_TRANSFORM_TYPE = ImageClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ImageClassificationData":
-        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from numpy arrays (or lists
-        of arrays) and corresponding lists of targets.
+        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from numpy arrays (or lists of
+        arrays) and corresponding lists of targets.
 
         The targets can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -366,17 +352,17 @@
             >>> model = ImageClassifier(backbone="resnet18", num_classes=datamodule.num_classes)
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
@@ -457,17 +443,17 @@
             >>> model = ImageClassifier(backbone="resnet18", num_classes=datamodule.num_classes)
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_images, train_targets, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_images, val_targets, **ds_kw),
@@ -490,16 +476,16 @@
         predict_data: Optional[Collection[Tensor]] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ImageClassificationTensorInput,
         transform: INPUT_TRANSFORM_TYPE = ImageClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ImageClassificationData":
-        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from torch tensors (or lists
-        of tensors) and corresponding lists of targets.
+        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from torch tensors (or lists of
+        tensors) and corresponding lists of targets.
 
         The targets can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -543,17 +529,17 @@
             >>> model = ImageClassifier(backbone="resnet18", num_classes=datamodule.num_classes)
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
@@ -682,17 +668,17 @@
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> del train_data_frame
             >>> del predict_data_frame
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_data = (train_data_frame, input_field, target_fields, train_images_root, train_resolver)
         val_data = (val_data_frame, input_field, target_fields, val_images_root, val_resolver)
         test_data = (test_data_frame, input_field, target_fields, test_images_root, test_resolver)
         predict_data = (predict_data_frame, input_field, None, predict_images_root, predict_resolver)
 
         train_input = input_cls(RunningStage.TRAINING, *train_data, **ds_kw)
@@ -727,16 +713,16 @@
         predict_resolver: Optional[Callable[[PATH_TYPE, Any], PATH_TYPE]] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ImageClassificationCSVInput,
         transform: INPUT_TRANSFORM_TYPE = ImageClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ImageClassificationData":
-        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from CSV files containing
-        image file paths and their corresponding targets.
+        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from CSV files containing image
+        file paths and their corresponding targets.
 
         Input images will be extracted from the ``input_field`` column in the CSV files.
         The supported file extensions are: ``.jpg``, ``.jpeg``, ``.png``, ``.ppm``, ``.bmp``, ``.pgm``, ``.tif``,
         ``.tiff``, ``.webp``, and ``.npy``.
         The targets will be extracted from the ``target_fields`` in the CSV files and can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
@@ -913,17 +899,17 @@
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_data = (train_file, input_field, target_fields, train_images_root, train_resolver)
         val_data = (val_file, input_field, target_fields, val_images_root, val_resolver)
         test_data = (test_file, input_field, target_fields, test_images_root, test_resolver)
         predict_data = (predict_file, input_field, None, predict_images_root, predict_resolver)
 
         train_input = input_cls(RunningStage.TRAINING, *train_data, **ds_kw)
@@ -950,16 +936,16 @@
         label_field: str = "ground_truth",
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ImageClassificationFiftyOneInput,
         transform: INPUT_TRANSFORM_TYPE = ImageClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs,
     ) -> "ImageClassificationData":
-        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from FiftyOne
-        ``SampleCollection`` objects.
+        """Load the :class:`~flash.image.classification.data.ImageClassificationData` from FiftyOne ``SampleCollection``
+        objects.
 
         The supported file extensions are: ``.jpg``, ``.jpeg``, ``.png``, ``.ppm``, ``.bmp``, ``.pgm``, ``.tif``,
         ``.tiff``, ``.webp``, and ``.npy``.
         The targets will be extracted from the ``label_field`` in the ``SampleCollection`` objects and can be in any
         of our :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
@@ -1032,17 +1018,17 @@
 
             >>> import os
             >>> _ = [os.remove(f"image_{i}.png") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_image_{i}.png") for i in range(1, 4)]
             >>> del train_dataset
             >>> del predict_dataset
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_dataset, label_field=label_field, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_dataset, label_field=label_field, **ds_kw),
@@ -1069,19 +1055,18 @@
         input_cls: Type[Input] = LabelStudioImageClassificationInput,
         transform: INPUT_TRANSFORM_TYPE = ImageClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         val_split: Optional[float] = None,
         multi_label: Optional[bool] = False,
         **data_module_kwargs: Any,
     ) -> "ImageClassificationData":
-        """Creates a :class:`~flash.core.data.data_module.DataModule` object
-        from the given export file and data directory using the
-        :class:`~flash.core.data.io.input.Input` of name
-        :attr:`~flash.core.data.io.input.InputFormat.FOLDERS`
-        from the passed or constructed :class:`~flash.core.data.io.input_transform.InputTransform`.
+        """Creates a :class:`~flash.core.data.data_module.DataModule` object from the given export file and data
+        directory using the :class:`~flash.core.data.io.input.Input` of name
+        :attr:`~flash.core.data.io.input.InputFormat.FOLDERS` from the passed or constructed
+        :class:`~flash.core.data.io.input_transform.InputTransform`.
 
         Args:
             export_json: path to label studio export file
             train_export_json: path to label studio export file for train set.(overrides export_json if specified)
             val_export_json: path to label studio export file for validation
             test_export_json: path to label studio export file for test
             predict_export_json: path to label studio export file for predict
@@ -1120,15 +1105,15 @@
             val_data_folder=val_data_folder,
             test_data_folder=test_data_folder,
             predict_data_folder=predict_data_folder,
             val_split=val_split,
             multi_label=multi_label,
         )
 
-        ds_kw = dict()
+        ds_kw = {}
 
         train_input = input_cls(RunningStage.TRAINING, train_data, **ds_kw)
         ds_kw["parameters"] = getattr(train_input, "parameters", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, **ds_kw),
@@ -1148,17 +1133,16 @@
         predict_dataset: Optional[Dataset] = None,
         input_cls: Type[Input] = DatasetInput,
         transform: INPUT_TRANSFORM_TYPE = ImageClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "DataModule":
         """Creates a :class:`~flash.core.data.data_module.DataModule` object from the given datasets using the
-        :class:`~flash.core.data.io.input.Input`
-        of name :attr:`~flash.core.data.io.input.InputFormat.DATASETS`
-        from the passed or constructed :class:`~flash.core.data.io.input_transform.InputTransform`.
+        :class:`~flash.core.data.io.input.Input` of name :attr:`~flash.core.data.io.input.InputFormat.DATASETS` from the
+        passed or constructed :class:`~flash.core.data.io.input_transform.InputTransform`.
 
         Args:
             train_dataset: Dataset used during training.
             val_dataset: Dataset used during validating.
             test_dataset: Dataset used during testing.
             predict_dataset: Dataset used during predicting.
             input_cls: Input class used to create the datasets.
@@ -1171,15 +1155,15 @@
 
         Examples::
 
             data_module = DataModule.from_datasets(
                 train_dataset=train_dataset,
             )
         """
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_dataset, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_dataset, **ds_kw),
             input_cls(RunningStage.TESTING, test_dataset, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_dataset, **ds_kw),
             transform=transform,
@@ -1199,15 +1183,15 @@
 class MatplotlibVisualization(BaseVisualization):
     """Process and show the image batch and its associated label using matplotlib."""
 
     max_cols: int = 4  # maximum number of columns we accept
     block_viz_window: bool = True  # parameter to allow user to block visualisation windows
 
     @staticmethod
-    @requires("image")
+    @requires("PIL")
     def _to_numpy(img: Union[np.ndarray, Tensor, Image.Image]) -> np.ndarray:
         out: np.ndarray
         if isinstance(img, np.ndarray):
             out = img
         elif isinstance(img, Image.Image):
             out = np.array(img)
         elif isinstance(img, Tensor):
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/heads.py` & `lightning-flash-0.8.2/src/flash/image/classification/heads.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/input.py` & `lightning-flash-0.8.2/src/flash/image/classification/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 import pandas as pd
 
 from flash.core.data.io.classification_input import ClassificationInputMixin
 from flash.core.data.io.input import DataKeys
 from flash.core.data.utilities.classification import MultiBinaryTargetFormatter, TargetFormatter
 from flash.core.data.utilities.data_frame import resolve_files, resolve_targets
 from flash.core.data.utilities.loading import load_data_frame
-from flash.core.data.utilities.paths import filter_valid_files, make_dataset, PATH_TYPE
+from flash.core.data.utilities.paths import PATH_TYPE, filter_valid_files, make_dataset
 from flash.core.data.utilities.samples import to_samples
 from flash.core.integrations.fiftyone.utils import FiftyOneLabelUtilities
 from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, lazy_import, requires
 from flash.image.data import (
+    IMG_EXTENSIONS,
+    NP_EXTENSIONS,
     ImageFilesInput,
     ImageInput,
     ImageNumpyInput,
     ImageTensorInput,
-    IMG_EXTENSIONS,
-    NP_EXTENSIONS,
 )
 
 if _FIFTYONE_AVAILABLE:
     fol = lazy_import("fiftyone.core.labels")
     SampleCollection = "fiftyone.core.collections.SampleCollection"
 else:
     fol = None
@@ -147,18 +147,15 @@
         input_key: str,
         target_keys: Optional[Union[str, List[str]]] = None,
         root: Optional[PATH_TYPE] = None,
         resolver: Optional[Callable[[Optional[PATH_TYPE], Any], PATH_TYPE]] = None,
         target_formatter: Optional[TargetFormatter] = None,
     ) -> List[Dict[str, Any]]:
         files = resolve_files(data_frame, input_key, root, resolver)
-        if target_keys is not None:
-            targets = resolve_targets(data_frame, target_keys)
-        else:
-            targets = None
+        targets = resolve_targets(data_frame, target_keys) if target_keys is not None else None
         result = super().load_data(files, targets, target_formatter=target_formatter)
 
         # If we had binary multi-class targets then we also know the labels (column names)
         if (
             self.training
             and isinstance(self.target_formatter, MultiBinaryTargetFormatter)
             and isinstance(target_keys, List)
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/input_transform.py` & `lightning-flash-0.8.2/src/flash/image/classification/input_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     def forward(self, x):
         return torch.from_numpy(self.transform(image=x.numpy())["image"])
 
 
 @dataclass
 class ImageClassificationInputTransform(InputTransform):
-
     image_size: Tuple[int, int] = (196, 196)
     mean: Union[float, Tuple[float, float, float]] = (0.485, 0.456, 0.406)
     std: Union[float, Tuple[float, float, float]] = (0.229, 0.224, 0.225)
 
     def per_sample_transform(self):
         return T.Compose(
             [
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/integrations/baal/data.py` & `lightning-flash-0.8.2/src/flash/image/classification/integrations/baal/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from flash.core.data.io.input import InputBase
 from flash.core.data.io.input_transform import create_worker_input_transform_processor
 from flash.core.utilities.imports import _BAAL_AVAILABLE, requires
 from flash.core.utilities.stages import RunningStage
 
 if _BAAL_AVAILABLE:
     from baal.active.dataset import ActiveLearningDataset
-    from baal.active.heuristics import AbstractHeuristic, BALD
+    from baal.active.heuristics import BALD, AbstractHeuristic
 else:
 
     class AbstractHeuristic:
         pass
 
     class BALD(AbstractHeuristic):
         pass
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/integrations/baal/dropout.py` & `lightning-flash-0.8.2/src/flash/image/classification/integrations/baal/dropout.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/integrations/baal/loop.py` & `lightning-flash-0.8.2/src/flash/image/classification/integrations/baal/loop.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,55 +7,42 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import contextlib
 from copy import deepcopy
 from typing import Any, Dict, Optional
 
 from pytorch_lightning import LightningModule
+from pytorch_lightning.loops import Loop
+from pytorch_lightning.loops.fit_loop import FitLoop
+from pytorch_lightning.trainer.connectors.data_connector import _DataLoaderSource
+from pytorch_lightning.trainer.progress import Progress
 from pytorch_lightning.trainer.states import TrainerFn, TrainerStatus
 from pytorch_lightning.utilities.model_helpers import is_overridden
 from torch import Tensor
 
 import flash
 from flash.core.data.utils import _STAGES_PREFIX
-from flash.core.utilities.imports import (
-    _PL_GREATER_EQUAL_1_4_0,
-    _PL_GREATER_EQUAL_1_5_0,
-    _PL_GREATER_EQUAL_1_6_0,
-    requires,
-)
+from flash.core.utilities.imports import requires
 from flash.core.utilities.stability import beta
 from flash.core.utilities.stages import RunningStage
 from flash.image.classification.integrations.baal.data import ActiveLearningDataModule
 from flash.image.classification.integrations.baal.dropout import InferenceMCDropoutTask
 
-if _PL_GREATER_EQUAL_1_4_0:
-    from pytorch_lightning.loops import Loop
-    from pytorch_lightning.loops.fit_loop import FitLoop
-    from pytorch_lightning.trainer.progress import Progress
-else:
-    Loop = object
-    FitLoop = object
-
-if not _PL_GREATER_EQUAL_1_5_0:
-    from pytorch_lightning.trainer.connectors.data_connector import _PatchDataLoader
-else:
-    from pytorch_lightning.trainer.connectors.data_connector import _DataLoaderSource
-
 
 @beta("The BaaL integration is currently in Beta.")
 class ActiveLearningLoop(Loop):
     max_epochs: int
     inference_model: InferenceMCDropoutTask
 
-    @requires("baal", (_PL_GREATER_EQUAL_1_4_0, "pytorch-lightning>=1.4.0"))
+    @requires("baal")
     def __init__(self, label_epoch_frequency: int, inference_iteration: int = 2, should_reset_weights: bool = True):
         """The `ActiveLearning Loop` describes the following training procedure. This loop is connected with the
         `ActiveLearningTrainer`
 
         Example::
 
             while unlabelled data or budget criteria not reached:
@@ -110,15 +97,14 @@
             if self.trainer.datamodule.has_test:
                 self._reset_dataloader_for_stage(RunningStage.TESTING)
         if self.trainer.datamodule.has_unlabelled_data:
             self._reset_dataloader_for_stage(RunningStage.PREDICTING)
         self.progress.increment_ready()
 
     def advance(self, *args: Any, **kwargs: Any) -> None:
-
         self.progress.increment_started()
 
         if self.trainer.datamodule.has_labelled_data:
             self.fit_loop.run()
 
         if self.trainer.datamodule.has_test:
             self._reset_testing()
@@ -157,20 +143,15 @@
 
     def __getattr__(self, key):
         if key not in self.__dict__:
             return getattr(self.fit_loop, key)
         return self.__dict__[key]
 
     def _connect(self, model: LightningModule):
-        if _PL_GREATER_EQUAL_1_6_0:
-            self.trainer.strategy.connect(model)
-        elif _PL_GREATER_EQUAL_1_5_0:
-            self.trainer.training_type_plugin.connect(model)
-        else:
-            self.trainer.accelerator.connect(model)
+        self.trainer.strategy.connect(model)
 
     def _reset_fitting(self):
         self.trainer.state.fn = TrainerFn.FITTING
         self.trainer.training = True
         self._connect(self._lightning_module)
         self.fit_loop.epoch_progress = Progress()
 
@@ -191,32 +172,23 @@
         dataloader = (
             getattr(self.trainer.datamodule, dataloader_name)
             if is_overridden(dataloader_name, self.trainer.datamodule)
             else None
         )
 
         if dataloader:
-            if _PL_GREATER_EQUAL_1_5_0:
-                setattr(
-                    self.trainer._data_connector,
-                    f"_{dataloader_name}_source",
-                    _DataLoaderSource(self.trainer.datamodule, dataloader_name),
-                )
-            else:
-                setattr(
-                    self.trainer.lightning_module,
-                    dataloader_name,
-                    _PatchDataLoader(dataloader(), running_state),
-                )
+            setattr(
+                self.trainer._data_connector,
+                f"_{dataloader_name}_source",
+                _DataLoaderSource(self.trainer.datamodule, dataloader_name),
+            )
             setattr(self.trainer, dataloader_name, None)
             # TODO: Resolve this within PyTorch Lightning.
-            try:
+            with contextlib.suppress(Exception):
                 getattr(self.trainer, f"reset_{dataloader_name}")(self.trainer.lightning_module)
-            except Exception:
-                pass
 
     def _teardown(self) -> None:
         self.trainer.train_dataloader = None
         self.trainer.val_dataloaders = None
         self.trainer.test_dataloaders = None
         self.trainer.predict_dataloaders = None
         # Hack
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/integrations/learn2learn.py` & `lightning-flash-0.8.2/src/flash/image/classification/integrations/learn2learn.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""
-Note: This file will be deleted once
-https://github.com/learnables/learn2learn/pull/257/files is merged within Learn2Learn.
-"""
+"""Note: This file will be deleted once https://github.com/learnables/learn2learn/pull/257/files is merged within
+Learn2Learn."""
 
 from typing import Any, Callable, Optional
 
 import pytorch_lightning as pl
 from torch.utils.data import IterableDataset
 from torch.utils.data._utils.worker import get_worker_info
 
@@ -137,10 +134,9 @@
     def __next__(self):
         if self.counter >= len(self):
             raise StopIteration
         task_descriptions = []
         for _ in range(self.worker_world_size):
             task_descriptions.append(self.taskset.sample_task_description())
 
-        data = self.taskset.get_task(task_descriptions[self.worker_rank])
         self.counter += 1
-        return data
+        return self.taskset.get_task(task_descriptions[self.worker_rank])
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/classification/model.py` & `lightning-flash-0.8.2/src/flash/image/classification/model.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/data.py` & `lightning-flash-0.8.2/src/flash/image/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from pathlib import Path
 from typing import Any, Dict, List
 
 import torch
 
 import flash
 from flash.core.data.io.input import DataKeys, Input, ServeInput
-from flash.core.data.utilities.loading import IMG_EXTENSIONS, load_image, NP_EXTENSIONS
-from flash.core.data.utilities.paths import filter_valid_files, PATH_TYPE
+from flash.core.data.utilities.loading import IMG_EXTENSIONS, NP_EXTENSIONS, load_image
+from flash.core.data.utilities.paths import PATH_TYPE, filter_valid_files
 from flash.core.data.utilities.samples import to_samples
 from flash.core.utilities.imports import _TORCHVISION_AVAILABLE, Image, requires
 
 if _TORCHVISION_AVAILABLE:
     from torchvision.transforms.functional import to_pil_image
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/detection/backbones.py` & `lightning-flash-0.8.2/src/flash/image/detection/backbones.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
                 f"mmdet_{model_type.__name__.split('.')[-1]}",
                 backbones=get_backbones(model_type),
                 adapter=IceVisionObjectDetectionAdapter,
                 providers=[_ICEVISION, _MMDET],
             )
 
     if module_available("effdet"):
-
         model_type = icevision_models.ross.efficientdet
         OBJECT_DETECTION_HEADS(
             partial(load_icevision_with_image_size, model_type),
             model_type.__name__.split(".")[-1],
             backbones=get_backbones(model_type),
             adapter=IceVisionObjectDetectionAdapter,
             providers=[_ICEVISION, _EFFDET],
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/detection/cli.py` & `lightning-flash-0.8.2/src/flash/image/detection/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ) -> ObjectDetectionData:
     """Downloads and loads the COCO 128 data set."""
     download_data("https://github.com/zhiqwang/yolov5-rt-stack/releases/download/v0.3.0/coco128.zip", "data/")
     return ObjectDetectionData.from_coco(
         train_folder="data/coco128/images/train2017/",
         train_ann_file="data/coco128/annotations/instances_train2017.json",
         val_split=val_split,
-        transform_kwargs=dict(image_size=(128, 128)) if transform_kwargs is None else transform_kwargs,
+        transform_kwargs={"image_size": (128, 128)} if transform_kwargs is None else transform_kwargs,
         batch_size=batch_size,
         **data_module_kwargs,
     )
 
 
 def object_detection():
     """Detect objects in images."""
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/detection/data.py` & `lightning-flash-0.8.2/src/flash/image/detection/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,45 +22,47 @@
 from flash.core.data.utilities.classification import TargetFormatter
 from flash.core.data.utilities.sort import sorted_alphanumeric
 from flash.core.integrations.icevision.data import IceVisionInput
 from flash.core.integrations.icevision.transforms import IceVisionInputTransform
 from flash.core.utilities.imports import (
     _FIFTYONE_AVAILABLE,
     _ICEVISION_AVAILABLE,
-    _IMAGE_EXTRAS_TESTING,
+    _TOPIC_IMAGE_AVAILABLE,
     Image,
     requires,
 )
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.image.detection.input import (
     ObjectDetectionFiftyOneInput,
     ObjectDetectionFilesInput,
     ObjectDetectionImageInput,
     ObjectDetectionNumpyInput,
     ObjectDetectionTensorInput,
 )
 
-if _FIFTYONE_AVAILABLE:
-    SampleCollection = "fiftyone.core.collections.SampleCollection"
-else:
-    SampleCollection = None
+SampleCollection = "fiftyone.core.collections.SampleCollection" if _FIFTYONE_AVAILABLE else None
 
 if _ICEVISION_AVAILABLE:
     from icevision.core import ClassMap
     from icevision.parsers import COCOBBoxParser, Parser, VIABBoxParser, VOCBBoxParser
 else:
     COCOBBoxParser = object
     VIABBoxParser = object
     VOCBBoxParser = object
     Parser = object
 
+__doctest_skip__ = []
 # Skip doctests if requirements aren't available
-if not _IMAGE_EXTRAS_TESTING:
-    __doctest_skip__ = ["ObjectDetectionData", "ObjectDetectionData.*"]
+if not _TOPIC_IMAGE_AVAILABLE:
+    __doctest_skip__ += ["ObjectDetectionData", "ObjectDetectionData.*"]
+
+
+if not _FIFTYONE_AVAILABLE:
+    __doctest_skip__ += ["ObjectDetectionData.from_fiftyone"]
 
 
 class ObjectDetectionData(DataModule):
     """The ``ObjectDetectionData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for object detection."""
 
     input_transform_cls = IceVisionInputTransform
@@ -80,16 +82,16 @@
         predict_files: Optional[Sequence[str]] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ObjectDetectionFilesInput,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ObjectDetectionData":
-        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data list of
-        image files, bounding boxes, and targets.
+        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data list of image
+        files, bounding boxes, and targets.
 
         The supported file extensions are: ``.jpg``, ``.jpeg``, ``.png``, ``.ppm``, ``.bmp``, ``.pgm``, ``.tif``,
         ``.tiff``, ``.webp``, and ``.npy``.
         The targets can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         The bounding boxes are expected to be dictionaries with integer values (representing pixels) and the following
         keys: ``xmin``, ``ymin``, ``width``, ``height``.
@@ -159,17 +161,17 @@
         .. testcleanup::
 
             >>> import os
             >>> _ = [os.remove(f"image_{i}.png") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_image_{i}.png") for i in range(1, 4)]
         """
 
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(
             RunningStage.TRAINING,
             train_files,
             train_targets,
             train_bboxes,
             **ds_kw,
@@ -213,16 +215,16 @@
         predict_data: Optional[Collection[np.ndarray]] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ObjectDetectionNumpyInput,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ObjectDetectionData":
-        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given from numpy
-        arrays (or lists of arrays) and corresponding lists of bounding boxes and targets.
+        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given from numpy arrays
+        (or lists of arrays) and corresponding lists of bounding boxes and targets.
 
         The targets can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         The bounding boxes are expected to be dictionaries with integer values (representing pixels) and the following
         keys: ``xmin``, ``ymin``, ``width``, ``height``.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
@@ -277,17 +279,17 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(
             RunningStage.TRAINING,
             train_data,
             train_targets,
             train_bboxes,
             **ds_kw,
@@ -331,16 +333,16 @@
         predict_images: Optional[List[Image.Image]] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ObjectDetectionImageInput,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ObjectDetectionData":
-        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given lists of PIL
-        images and corresponding lists of bounding boxes and targets.
+        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given lists of PIL images
+        and corresponding lists of bounding boxes and targets.
 
         The targets can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         The bounding boxes are expected to be dictionaries with integer values (representing pixels) and the following
         keys: ``xmin``, ``ymin``, ``width``, ``height``.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
@@ -400,17 +402,17 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(
             RunningStage.TRAINING,
             train_images,
             train_targets,
             train_bboxes,
             **ds_kw,
@@ -454,16 +456,16 @@
         predict_data: Optional[Collection[torch.Tensor]] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = ObjectDetectionTensorInput,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ObjectDetectionData":
-        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given from torch
-        tensors (or lists of tensors) and corresponding lists of bounding boxes and targets.
+        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given from torch tensors
+        (or lists of tensors) and corresponding lists of bounding boxes and targets.
 
         The targets can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         The bounding boxes are expected to be dictionaries with integer values (representing pixels) and the following
         keys: ``xmin``, ``ymin``, ``width``, ``height``.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
@@ -518,17 +520,17 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(
             RunningStage.TRAINING,
             train_data,
             train_targets,
             train_bboxes,
             **ds_kw,
@@ -572,16 +574,15 @@
         predict_folder: Optional[str] = None,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         parser: Optional[Union[Callable, Type[Parser]]] = None,
         input_cls: Type[Input] = IceVisionInput,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs,
     ) -> "ObjectDetectionData":
-
-        ds_kw = dict(parser=parser)
+        ds_kw = {"parser": parser}
 
         return cls(
             input_cls(
                 RunningStage.TRAINING,
                 train_folder,
                 train_ann_file,
                 parser_kwargs=train_parser_kwargs,
@@ -618,18 +619,16 @@
         test_ann_file: Optional[str] = None,
         predict_folder: Optional[str] = None,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         input_cls: Type[Input] = IceVisionInput,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ObjectDetectionData":
-        """.. _COCO: https://www.immersivelimit.com/tutorials/create-coco-annotations-from-scratch.
-
-        Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data folders
-        and annotation files in the `COCO JSON format <https://cocodataset.org/#format-data>`_.
+        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data folders and
+        annotation files in the `COCO JSON format <https://cocodataset.org/#format-data>`_.
 
         For help understanding and using the COCO format, take a look at this tutorial: `Create COCO annotations from
         scratch <COCO>`__.
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
@@ -732,14 +731,16 @@
 
         .. testcleanup::
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> os.remove("train_annotations.json")
+
+        .. _COCO: https://www.immersivelimit.com/tutorials/create-coco-annotations-from-scratch
         """
         return cls.from_icedata(
             train_folder=train_folder,
             train_ann_file=train_ann_file,
             val_folder=val_folder,
             val_ann_file=val_ann_file,
             test_folder=test_folder,
@@ -764,18 +765,16 @@
         test_ann_folder: Optional[str] = None,
         predict_folder: Optional[str] = None,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         input_cls: Type[Input] = IceVisionInput,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ObjectDetectionData":
-        """.. _PASCAL: http://host.robots.ox.ac.uk/pascal/VOC/
-
-        Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data folders
-        and annotation files in the `PASCAL VOC (Visual Object Challenge) XML format <PASCAL>`_.
+        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data folders and
+        annotation files in the `PASCAL VOC (Visual Object Challenge) XML format <PASCAL>`_.
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
             labels: A list of class labels. Note that the list should not include a label for the background class which
                 will be added automatically as class zero (additional labels will be sorted).
@@ -888,14 +887,16 @@
 
         .. testcleanup::
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> shutil.rmtree("train_annotations")
+
+        .. _PASCAL: http://host.robots.ox.ac.uk/pascal/VOC/
         """
         return cls.from_icedata(
             train_folder=train_folder,
             train_ann_file=train_ann_folder,
             val_folder=val_folder,
             val_ann_file=val_ann_folder,
             test_folder=test_folder,
@@ -921,18 +922,17 @@
         test_ann_file: Optional[str] = None,
         predict_folder: Optional[str] = None,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         input_cls: Type[Input] = IceVisionInput,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ObjectDetectionData":
-        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data folders
-        and annotation files in the VIA (`VGG Image Annotator <https://www.robots.ox.ac.uk/~vgg/software/via/>`_)
-        `JSON format <https://gitlab.com/vgg/via/-/blob/via-3.x.y/via-3.x.y/CodeDoc.md#structure-of-via-project-
-        json-file>`_.
+        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data folders and
+        annotation files in the VIA (`VGG Image Annotator <https://www.robots.ox.ac.uk/~vgg/software/via/>`_) `JSON
+        format <https://gitlab.com/vgg/via/-/blob/via-3.x.y/via-3.x.y/CodeDoc.md#structure-of-via-project- json-file>`_.
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
             labels: A list of class labels. Not that the list should not include a label for the background class which
                 will be added automatically as class zero (additional labels will be sorted).
@@ -1074,16 +1074,15 @@
         label_field: str = "ground_truth",
         iscrowd: str = "iscrowd",
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         input_cls: Type[Input] = ObjectDetectionFiftyOneInput,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "ObjectDetectionData":
-        """Load the :class:`~flash.image.detection.data.ObjectDetectionData` from FiftyOne ``SampleCollection``
-        objects.
+        """Load the :class:`~flash.image.detection.data.ObjectDetectionData` from FiftyOne ``SampleCollection`` objects.
 
         Targets will be extracted from the ``label_field`` in the ``SampleCollection`` objects.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
             train_dataset: The ``SampleCollection`` to use when training.
@@ -1161,15 +1160,15 @@
         .. testcleanup::
 
             >>> import os
             >>> _ = [os.remove(f"image_{i}.png") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_image_{i}.png") for i in range(1, 4)]
         """
 
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_dataset, label_field, iscrowd, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_dataset, label_field, iscrowd, **ds_kw),
             input_cls(RunningStage.TESTING, test_dataset, label_field, iscrowd, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_dataset, **ds_kw),
             transform=transform,
@@ -1182,16 +1181,16 @@
         cls,
         predict_folder: Optional[str] = None,
         predict_transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         input_cls: Type[Input] = IceVisionInput,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "DataModule":
-        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data folders
-        This is currently support only for the predicting stage.
+        """Creates a :class:`~flash.image.detection.data.ObjectDetectionData` object from the given data folders This is
+        currently support only for the predicting stage.
 
         Args:
             predict_folder: The folder containing the predict data.
             predict_transform: The dictionary of transforms to use during predicting which maps
             data_module_kwargs: The keywords arguments for creating the datamodule.
 
         Returns:
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/detection/input.py` & `lightning-flash-0.8.2/src/flash/image/detection/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, Hashable, List, Optional, Sequence
 
 from flash.core.data.io.classification_input import ClassificationInputMixin
 from flash.core.data.io.input import DataKeys
 from flash.core.data.utilities.classification import TargetFormatter
-from flash.core.data.utilities.paths import filter_valid_files, PATH_TYPE
+from flash.core.data.utilities.paths import PATH_TYPE, filter_valid_files
 from flash.core.data.utilities.samples import to_samples
 from flash.core.integrations.fiftyone.utils import FiftyOneLabelUtilities
 from flash.core.integrations.icevision.data import IceVisionInput
 from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, _ICEVISION_AVAILABLE, lazy_import, requires
 from flash.image.data import (
+    IMG_EXTENSIONS,
+    NP_EXTENSIONS,
     ImageFilesInput,
     ImageInput,
     ImageNumpyInput,
     ImageTensorInput,
-    IMG_EXTENSIONS,
-    NP_EXTENSIONS,
 )
 
 if _FIFTYONE_AVAILABLE:
     fol = lazy_import("fiftyone.core.labels")
     SampleCollection = "fiftyone.core.collections.SampleCollection"
 else:
     fol = None
@@ -215,16 +215,15 @@
     def _reformat_bbox(xmin, ymin, box_w, box_h, img_w, img_h):
         xmin *= img_w
         ymin *= img_h
         box_w *= img_w
         box_h *= img_h
         xmax = xmin + box_w
         ymax = ymin + box_h
-        output_bbox = [xmin, ymin, xmax, ymax]
-        return output_bbox
+        return [xmin, ymin, xmax, ymax]
 
 
 class ObjectDetectionFiftyOneInput(IceVisionInput):
     num_classes: int
     labels: list
 
     @requires("fiftyone")
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/detection/model.py` & `lightning-flash-0.8.2/src/flash/image/detection/model.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/detection/output.py` & `lightning-flash-0.8.2/src/flash/image/detection/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,18 +80,15 @@
                 (xmin / width).item(),
                 (ymin / height).item(),
                 (box_width / width).item(),
                 (box_height / height).item(),
             ]
 
             label = label.item()
-            if self._labels is not None:
-                label = self._labels[label]
-            else:
-                label = str(int(label))
+            label = self._labels[label] if self._labels is not None else str(int(label))
 
             detections.append(
                 fo.Detection(
                     label=label,
                     bounding_box=box,
                     confidence=confidence,
                 )
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/heads/vissl_heads.py` & `lightning-flash-0.8.2/src/flash/image/embedding/heads/vissl_heads.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         layers.append(nn.Linear(last_dim, self.dims[-1]))
         return nn.Sequential(*layers)
 
     def forward(self, x: Tensor) -> Tensor:
         return self.clf(x)
 
 
-if _VISSL_AVAILABLE:
+if _VISSL_AVAILABLE and "simclr_head" not in MODEL_HEADS_REGISTRY:
     SimCLRHead = register_model_head("simclr_head")(SimCLRHead)
 
 
 def simclr_head(
     num_features: int = 2048,
     embedding_dim: int = 128,
     dims: List[int] = [2048],
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/losses/vissl_losses.py` & `lightning-flash-0.8.2/src/flash/image/embedding/losses/vissl_losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from flash.core.registry import FlashRegistry
 from flash.core.utilities.imports import _VISSL_AVAILABLE
 
 if _VISSL_AVAILABLE:
     import vissl.losses  # noqa: F401
     from classy_vision.generic.distributed_util import set_cpu_device
-    from classy_vision.losses import ClassyLoss, LOSS_REGISTRY
+    from classy_vision.losses import LOSS_REGISTRY, ClassyLoss
     from vissl.config.attr_dict import AttrDict
 else:
     AttrDict = object
     ClassyLoss = object
 
 
 def _recursive_register(module):
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/model.py` & `lightning-flash-0.8.2/src/flash/image/embedding/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 _deprecated_backbones = {
     "resnet": "resnet50",
     "vision_transformer": "vit_small_patch16_224",
 }
 
 
 class ImageEmbedder(AdapterTask):
-    """The ``ImageEmbedder`` is a :class:`~flash.Task` for obtaining feature vectors (embeddings) from images. For
-    more details, see :ref:`image_embedder`.
+    """The ``ImageEmbedder`` is a :class:`~flash.Task` for obtaining feature vectors (embeddings) from images. For more
+    details, see :ref:`image_embedder`.
 
     Args:
         training_strategy: Training strategy from VISSL,
             select between 'simclr', 'swav', or 'barlow_twins'.
         head: projection head used for task, select between
             'simclr_head', 'swav_head', or 'barlow_twins_head'.
         pretraining_transform: transform applied to input image for pre-training SSL model.
@@ -131,17 +131,20 @@
         if pretraining_transform is not None:
             warnings.warn(
                 "Overriding any transforms from the `DataModule` with the pretraining transform: "
                 f"{pretraining_transform}."
             )
             self.input_transform = self.transforms.get(pretraining_transform)(**pretraining_transform_kwargs)
 
-        if "providers" in metadata["metadata"] and metadata["metadata"]["providers"].name == "Facebook Research/vissl":
-            if pretraining_transform is None:
-                raise ValueError("Correct pretraining_transform must be set to use VISSL")
+        if (
+            "providers" in metadata["metadata"]
+            and metadata["metadata"]["providers"].name == "Facebook Research/vissl"
+            and pretraining_transform is None
+        ):
+            raise ValueError("Correct pretraining_transform must be set to use VISSL")
 
     def forward(self, x: Tensor) -> Any:
         return self.model(x)
 
     def predict_step(self, batch: Any, batch_idx: int, dataloader_idx: int = 0) -> Any:
         return self(batch[DataKeys.INPUT])
 
@@ -156,16 +159,15 @@
 
     def on_train_batch_end(self, outputs: Any, batch: Any, batch_idx: int, *args) -> None:
         self.adapter.on_train_batch_end(outputs, batch, batch_idx, *args)
 
     @classmethod
     @requires("image", "vissl", "fairscale")
     def available_training_strategies(cls) -> List[str]:
-        """Get the list of available training strategies (passed to the ``training_strategy`` argument) for this
-        task.
+        """Get the list of available training strategies (passed to the ``training_strategy`` argument) for this task.
 
         Examples
         ________
 
         .. doctest::
 
             >>> from flash.image import ImageEmbedder
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/strategies/default.py` & `lightning-flash-0.8.2/src/flash/image/embedding/strategies/default.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/strategies/vissl_strategies.py` & `lightning-flash-0.8.2/src/flash/image/embedding/strategies/vissl_strategies.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/transforms/vissl_transforms.py` & `lightning-flash-0.8.2/src/flash/image/embedding/transforms/vissl_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,54 +28,50 @@
     crop_scales: Sequence[Sequence[float]] = [[0.4, 1]],
     gaussian_blur: bool = True,
     jitter_strength: float = 1.0,
     normalize: Optional[nn.Module] = None,
     collate_fn: Callable = simclr_collate_fn,
 ) -> partial:
     """For simclr and barlow twins."""
-    transform = partial(
+    return partial(
         StandardMultiCropSSLTransform,
         total_num_crops=total_num_crops,
         num_crops=num_crops,
         size_crops=size_crops,
         crop_scales=crop_scales,
         gaussian_blur=gaussian_blur,
         jitter_strength=jitter_strength,
         normalize=normalize,
         collate_fn=collate_fn,
     )
 
-    return transform
-
 
 def swav_transform(
     total_num_crops: int = 8,
     num_crops: Sequence[int] = [2, 6],
     size_crops: Sequence[int] = [224, 96],
     crop_scales: Sequence[Sequence[float]] = [[0.4, 1], [0.05, 0.4]],
     gaussian_blur: bool = True,
     jitter_strength: float = 1.0,
     normalize: Optional[nn.Module] = None,
     collate_fn: Callable = multicrop_collate_fn,
 ) -> partial:
     """For swav."""
-    transform = partial(
+    return partial(
         StandardMultiCropSSLTransform,
         total_num_crops=total_num_crops,
         num_crops=num_crops,
         size_crops=size_crops,
         crop_scales=crop_scales,
         gaussian_blur=gaussian_blur,
         jitter_strength=jitter_strength,
         normalize=normalize,
         collate_fn=collate_fn,
     )
 
-    return transform
-
 
 barlow_twins_transform = partial(simclr_transform, collate_fn=simclr_collate_fn)
 
 
 transforms = [
     "simclr_transform",
     "swav_transform",
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/vissl/adapter.py` & `lightning-flash-0.8.2/src/flash/image/embedding/vissl/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     def __init__(
         self,
         backbone: nn.Module,
         head: nn.Module,
         loss_fn: ClassyLoss,
         hooks: List[ClassyHook],
     ) -> None:
-
         Adapter.__init__(self)
 
         self.model_config = self.get_model_config_template()
         self.optimizer_config = AttrDict({})
 
         self.backbone = backbone
         self.head = [head] if not isinstance(head, list) else head
@@ -158,15 +157,15 @@
         if hasattr(self.loss_fn, "info_criterion"):
             self.loss_fn.info_criterion.use_gpu = use_gpu
         if hasattr(self.loss_fn, "swav_criterion"):
             self.loss_fn.swav_criterion.use_gpu = use_gpu
 
     @staticmethod
     def get_model_config_template():
-        cfg = AttrDict(
+        return AttrDict(
             {
                 "BASE_MODEL_NAME": "multi_input_output_model",
                 "SINGLE_PASS_EVERY_CROP": False,
                 "INPUT_TYPE": "rgb",
                 "MULTI_INPUT_HEAD_MAPPING": [],
                 "TRUNK": AttrDict({}),
                 "HEAD": AttrDict(
@@ -189,16 +188,14 @@
                         "USE_ACTIVATION_CHECKPOINTING": False,
                         "NUM_ACTIVATION_CHECKPOINTING_SPLITS": 2,
                     }
                 ),
             }
         )
 
-        return cfg
-
     def ssl_forward(self, batch) -> Any:
         model_output = self.vissl_base_model(batch)
 
         # vissl-specific
         if len(model_output) == 1:
             model_output = model_output[0]
 
@@ -208,17 +205,15 @@
         out = self.ssl_forward(batch[DataKeys.INPUT])
 
         if train:
             # call forward hook from VISSL (momentum updates)
             for hook in self.hooks:
                 hook.on_forward(self.vissl_task)
 
-        loss = self.loss_fn(out, target=None)
-
-        return loss
+        return self.loss_fn(out, target=None)
 
     def training_step(self, batch: Any, batch_idx: int) -> Any:
         loss = self.shared_step(batch)
         self.adapter_task.log_dict({"train_loss": loss.item()})
 
         return loss
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/vissl/hooks.py` & `lightning-flash-0.8.2/src/flash/image/embedding/vissl/hooks.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/vissl/transforms/multicrop.py` & `lightning-flash-0.8.2/src/flash/image/embedding/vissl/transforms/multicrop.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 
 if _TORCHVISION_AVAILABLE:
     import torchvision.transforms as pth_transforms
 
 
 @dataclass
 class StandardMultiCropSSLTransform(InputTransform):
-    """Convert a PIL image to Multi-resolution Crops. The input is a PIL image and output is the list of image
-    crops.
+    """Convert a PIL image to Multi-resolution Crops. The input is a PIL image and output is the list of image crops.
 
     This transform was proposed in SwAV - https://arxiv.org/abs/2006.09882
     This transform can act as a base transform class for SimCLR, SwAV, and Barlow Twins from VISSL.
 
     This transform has been modified from the ImgPilToMultiCrop code present at
     https://github.com/facebookresearch/vissl/blob/master/vissl/data/ssl_transforms/img_pil_to_multicrop.py
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/embedding/vissl/transforms/utilities.py` & `lightning-flash-0.8.2/src/flash/image/embedding/vissl/transforms/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/face_detection/backbones/fastface_backbones.py` & `lightning-flash-0.8.2/src/flash/image/face_detection/backbones/fastface_backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/face_detection/cli.py` & `lightning-flash-0.8.2/src/flash/image/face_detection/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/face_detection/data.py` & `lightning-flash-0.8.2/src/flash/image/face_detection/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,15 @@
         test_dataset: Optional[Dataset] = None,
         predict_dataset: Optional[Dataset] = None,
         input_cls: Type[Input] = FaceDetectionInput,
         transform: INPUT_TRANSFORM_TYPE = FaceDetectionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs,
     ) -> "FaceDetectionData":
-
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_dataset, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_dataset, **ds_kw),
             input_cls(RunningStage.TESTING, test_dataset, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_dataset, **ds_kw),
             transform=transform,
@@ -59,15 +58,14 @@
         cls,
         predict_files: Optional[Sequence[str]] = None,
         predict_transform: INPUT_TRANSFORM_TYPE = FaceDetectionInputTransform,
         input_cls: Type[Input] = ImageClassificationFilesInput,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "FaceDetectionData":
-
         return cls(
             predict_input=input_cls(RunningStage.PREDICTING, predict_files),
             transform=predict_transform,
             transform_kwargs=transform_kwargs,
             **data_module_kwargs,
         )
 
@@ -76,14 +74,13 @@
         cls,
         predict_folder: Optional[str] = None,
         predict_transform: INPUT_TRANSFORM_TYPE = FaceDetectionInputTransform,
         input_cls: Type[Input] = ImageClassificationFolderInput,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "FaceDetectionData":
-
         return cls(
             predict_input=input_cls(RunningStage.PREDICTING, predict_folder),
             transform=predict_transform,
             transform_kwargs=transform_kwargs,
             **data_module_kwargs,
         )
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/face_detection/input.py` & `lightning-flash-0.8.2/src/flash/image/face_detection/input.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/face_detection/input_transform.py` & `lightning-flash-0.8.2/src/flash/image/face_detection/input_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     samples = {key: [sample[key] for sample in samples] for key in samples[0]}
 
     images, scales, paddings = ff.utils.preprocess.prepare_batch(samples[DataKeys.INPUT], None, adaptive_batch=True)
 
     samples["scales"] = scales
     samples["paddings"] = paddings
 
-    if DataKeys.TARGET in samples.keys():
+    if DataKeys.TARGET in samples:
         targets = samples[DataKeys.TARGET]
 
         for i, (target, scale, padding) in enumerate(zip(targets, scales, paddings)):
             target["target_boxes"] *= scale
             target["target_boxes"][:, [0, 2]] += padding[0]
             target["target_boxes"][:, [1, 3]] += padding[1]
             targets[i]["target_boxes"] = target["target_boxes"]
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/face_detection/model.py` & `lightning-flash-0.8.2/src/flash/image/face_detection/model.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/face_detection/output_transform.py` & `lightning-flash-0.8.2/src/flash/image/face_detection/output_transform.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/instance_segmentation/backbones.py` & `lightning-flash-0.8.2/src/flash/image/instance_segmentation/backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/instance_segmentation/cli.py` & `lightning-flash-0.8.2/src/flash/image/instance_segmentation/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         train_folder=train_folder or data_dir,
         train_ann_file=train_ann_file,
         val_folder=val_folder,
         val_ann_file=val_ann_file,
         test_folder=test_folder,
         test_ann_file=test_ann_file,
         predict_folder=predict_folder,
-        transform_kwargs=dict(image_size=(128, 128)) if transform_kwargs is None else transform_kwargs,
+        transform_kwargs={"image_size": (128, 128)} if transform_kwargs is None else transform_kwargs,
         parser=parser,
         val_split=val_split,
         batch_size=batch_size,
         **data_module_kwargs,
     )
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/instance_segmentation/data.py` & `lightning-flash-0.8.2/src/flash/image/instance_segmentation/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from flash.core.data.io.input import DataKeys, Input
 from flash.core.data.io.output_transform import OutputTransform
 from flash.core.data.utilities.sort import sorted_alphanumeric
 from flash.core.integrations.icevision.data import IceVisionInput
 from flash.core.integrations.icevision.transforms import IceVisionInputTransform
 from flash.core.utilities.imports import (
     _ICEVISION_AVAILABLE,
-    _IMAGE_EXTRAS_TESTING,
+    _TOPIC_IMAGE_AVAILABLE,
     _TORCHVISION_AVAILABLE,
     _TORCHVISION_GREATER_EQUAL_0_9,
 )
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 
 if _ICEVISION_AVAILABLE:
@@ -47,27 +47,26 @@
     else:
 
         class InterpolationMode:
             NEAREST = "nearest"
 
 
 # Skip doctests if requirements aren't available
-if not _IMAGE_EXTRAS_TESTING:
+if not _TOPIC_IMAGE_AVAILABLE:
     __doctest_skip__ = ["InstanceSegmentationData", "InstanceSegmentationData.*"]
 
 
 class InstanceSegmentationOutputTransform(OutputTransform):
     def per_sample_transform(self, sample: Any) -> Any:
         resize = T.Resize(sample[DataKeys.METADATA]["size"], interpolation=InterpolationMode.NEAREST)
         sample[DataKeys.PREDS]["masks"] = [resize(tensor(mask)) for mask in sample[DataKeys.PREDS]["masks"]]
         return sample[DataKeys.PREDS]
 
 
 class InstanceSegmentationData(DataModule):
-
     input_transform_cls = IceVisionInputTransform
     output_transform_cls = InstanceSegmentationOutputTransform
 
     @classmethod
     def from_icedata(
         cls,
         train_folder: Optional[str] = None,
@@ -82,16 +81,15 @@
         predict_folder: Optional[str] = None,
         parser: Optional[Union[Callable, Type[Parser]]] = None,
         input_cls: Type[Input] = IceVisionInput,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs,
     ) -> "InstanceSegmentationData":
-
-        ds_kw = dict(parser=parser)
+        ds_kw = {"parser": parser}
 
         return cls(
             input_cls(
                 RunningStage.TRAINING,
                 train_folder,
                 train_ann_file,
                 parser_kwargs=train_parser_kwargs,
@@ -128,19 +126,19 @@
         test_ann_file: Optional[str] = None,
         predict_folder: Optional[str] = None,
         input_cls: Type[Input] = IceVisionInput,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ):
-        """Creates a :class:`~flash.image.instance_segmentation.data.InstanceSegmentationData` object from the
-        given data folders and annotation files in the `COCO JSON format <https://cocodataset.org/#format-data>`_.
+        """Creates a :class:`~flash.image.instance_segmentation.data.InstanceSegmentationData` object from the given
+        data folders and annotation files in the `COCO JSON format <https://cocodataset.org/#format-data>`_.
 
         For help understanding and using the COCO format, take a look at this tutorial: `Create COCO annotations from
-        scratch <COCO>`__.
+        scratch <COCO>`_.
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
             train_folder: The folder containing images to use when training.
             train_ann_file: The COCO format annotation file to use when training.
@@ -246,14 +244,16 @@
 
         .. testcleanup::
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> os.remove("train_annotations.json")
+
+        .. _COCO: https://www.immersivelimit.com/tutorials/create-coco-annotations-from-scratch
         """
         return cls.from_icedata(
             train_folder=train_folder,
             train_ann_file=train_ann_file,
             val_folder=val_folder,
             val_ann_file=val_ann_file,
             test_folder=test_folder,
@@ -281,17 +281,17 @@
         test_ann_folder: Optional[str] = None,
         predict_folder: Optional[str] = None,
         input_cls: Type[Input] = IceVisionInput,
         transform: INPUT_TRANSFORM_TYPE = IceVisionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ):
-        """Creates a :class:`~flash.image.instance_segmentation.data.InstanceSegmentationData` object from the
-        given data folders, mask folders, and annotation files in the `PASCAL VOC (Visual Object Challenge) XML
-        format <PASCAL>`_.
+        """Creates a :class:`~flash.image.instance_segmentation.data.InstanceSegmentationData` object from the given
+        data folders, mask folders, and annotation files in the `PASCAL VOC <PASCAL>`_ (Visual Object Challenge) XML
+        format.
 
         .. note:: All three arguments `*_folder`, `*_target_folder`, and `*_ann_folder` are needed to load data for a
             particular stage.
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
@@ -425,14 +425,16 @@
         .. testcleanup::
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("train_masks")
             >>> shutil.rmtree("predict_folder")
             >>> shutil.rmtree("train_annotations")
+
+        .. _PASCAL: http://host.robots.ox.ac.uk/pascal/VOC/
         """
         return cls.from_icedata(
             train_folder=train_folder,
             train_ann_file=train_ann_folder,
             train_parser_kwargs={"masks_dir": train_target_folder},
             val_folder=val_folder,
             val_ann_file=val_ann_folder,
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/instance_segmentation/model.py` & `lightning-flash-0.8.2/src/flash/image/instance_segmentation/model.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/keypoint_detection/backbones.py` & `lightning-flash-0.8.2/src/flash/image/keypoint_detection/backbones.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,16 @@
             pretrained=pretrained,
             metrics=metrics,
             image_size=image_size,
             **kwargs,
         )
 
 
-if _ICEVISION_AVAILABLE:
-    if _TORCHVISION_AVAILABLE:
-        model_type = icevision_models.torchvision.keypoint_rcnn
-        KEYPOINT_DETECTION_HEADS(
-            partial(load_icevision_ignore_image_size, model_type),
-            model_type.__name__.split(".")[-1],
-            backbones=get_backbones(model_type),
-            adapter=IceVisionKeypointDetectionAdapter,
-            providers=[_ICEVISION, _TORCHVISION],
-        )
+if _ICEVISION_AVAILABLE and _TORCHVISION_AVAILABLE:
+    model_type = icevision_models.torchvision.keypoint_rcnn
+    KEYPOINT_DETECTION_HEADS(
+        partial(load_icevision_ignore_image_size, model_type),
+        model_type.__name__.split(".")[-1],
+        backbones=get_backbones(model_type),
+        adapter=IceVisionKeypointDetectionAdapter,
+        providers=[_ICEVISION, _TORCHVISION],
+    )
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/keypoint_detection/cli.py` & `lightning-flash-0.8.2/src/flash/image/keypoint_detection/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         train_ann_file=train_ann_file,
         val_folder=val_folder,
         val_ann_file=val_ann_file,
         test_folder=test_folder,
         test_ann_file=test_ann_file,
         predict_folder=predict_folder,
         val_split=val_split,
-        transform_kwargs=dict(image_size=(128, 128)) if transform_kwargs is None else transform_kwargs,
+        transform_kwargs={"image_size": (128, 128)} if transform_kwargs is None else transform_kwargs,
         batch_size=batch_size,
         parser=parser,
         **data_module_kwargs,
     )
 
 
 def keypoint_detection():
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/keypoint_detection/data.py` & `lightning-flash-0.8.2/src/flash/image/keypoint_detection/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 # limitations under the License.
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.integrations.icevision.data import IceVisionInput
-from flash.core.utilities.imports import _ICEVISION_AVAILABLE, _IMAGE_EXTRAS_TESTING
+from flash.core.utilities.imports import _ICEVISION_AVAILABLE, _TOPIC_IMAGE_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.image.keypoint_detection.input_transform import KeypointDetectionInputTransform
 
 if _ICEVISION_AVAILABLE:
     from icevision.core import KeyPoints, KeypointsMetadata
     from icevision.parsers import COCOKeyPointsParser, Parser
 else:
     COCOKeyPointsParser = object
     Parser = object
     KeyPoints = object
 
 
 # Skip doctests if requirements aren't available
-if not _IMAGE_EXTRAS_TESTING:
+if not _TOPIC_IMAGE_AVAILABLE:
     __doctest_skip__ = ["KeypointDetectionData", "KeypointDetectionData.*"]
 
 
 class FlashCOCOKeyPointsParser(COCOKeyPointsParser):
     def __init__(
         self,
         annotations_filepath: Union[str, Path, dict],
@@ -81,16 +81,15 @@
         predict_folder: Optional[str] = None,
         parser: Optional[Union[Callable, Type[Parser]]] = None,
         input_cls: Type[Input] = IceVisionInput,
         transform: INPUT_TRANSFORM_TYPE = KeypointDetectionInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "KeypointDetectionData":
-
-        ds_kw = dict(parser=parser)
+        ds_kw = {"parser": parser}
 
         return cls(
             input_cls(
                 RunningStage.TRAINING,
                 train_folder,
                 train_ann_file,
                 parser_kwargs=train_parser_kwargs,
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/keypoint_detection/input_transform.py` & `lightning-flash-0.8.2/src/flash/image/keypoint_detection/input_transform.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/keypoint_detection/model.py` & `lightning-flash-0.8.2/src/flash/image/keypoint_detection/model.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/backbones.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/backbones.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 if _SEGMENTATION_MODELS_AVAILABLE:
     import segmentation_models_pytorch as smp
 
 SEMANTIC_SEGMENTATION_BACKBONES = FlashRegistry("backbones")
 
 if _SEGMENTATION_MODELS_AVAILABLE:
-
     ENCODERS = smp.encoders.get_encoder_names()
 
     def _load_smp_backbone(backbone: str, **_) -> str:
         return backbone
 
     for encoder_name in ENCODERS:
         short_name = encoder_name
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/cli.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/data.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import numpy as np
 from torch import Tensor
 
 from flash.core.data.callback import BaseDataFetcher
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
-from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, _IMAGE_EXTRAS_TESTING, _IMAGE_TESTING, lazy_import
+from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, _SEGMENTATION_MODELS_AVAILABLE, lazy_import
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.image.segmentation.input import (
     SemanticSegmentationFiftyOneInput,
     SemanticSegmentationFilesInput,
     SemanticSegmentationFolderInput,
     SemanticSegmentationNumpyInput,
@@ -37,23 +37,17 @@
     SampleCollection = "fiftyone.core.collections.SampleCollection"
 else:
     fo = None
     SampleCollection = object
 
 # Skip doctests if requirements aren't available
 __doctest_skip__ = []
-if not _IMAGE_TESTING:
-    __doctest_skip__ += [
-        "SemanticSegmentationData",
-        "SemanticSegmentationData.from_files",
-        "SemanticSegmentationData.from_folders",
-        "SemanticSegmentationData.from_numpy",
-        "SemanticSegmentationData.from_tensors",
-    ]
-if not _IMAGE_EXTRAS_TESTING:
+if not _SEGMENTATION_MODELS_AVAILABLE:
+    __doctest_skip__ += ["SemanticSegmentationData", "SemanticSegmentationData.*"]
+if not _FIFTYONE_AVAILABLE:
     __doctest_skip__ += ["SemanticSegmentationData.from_fiftyone"]
 
 
 class SemanticSegmentationData(DataModule):
     """The ``SemanticSegmentationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for semantic segmentation."""
 
@@ -145,18 +139,18 @@
 
             >>> import os
             >>> _ = [os.remove(f"image_{i}.png") for i in range(1, 4)]
             >>> _ = [os.remove(f"mask_{i}.npy") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_image_{i}.png") for i in range(1, 4)]
         """
 
-        ds_kw = dict(
-            num_classes=num_classes,
-            labels_map=labels_map,
-        )
+        ds_kw = {
+            "num_classes": num_classes,
+            "labels_map": labels_map,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_files, train_targets, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_files, val_targets, **ds_kw),
             input_cls(RunningStage.TESTING, test_files, test_targets, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_files, **ds_kw),
             transform=transform,
@@ -177,16 +171,16 @@
         input_cls: Type[Input] = SemanticSegmentationFolderInput,
         num_classes: Optional[int] = None,
         labels_map: Dict[int, Tuple[int, int, int]] = None,
         transform: INPUT_TRANSFORM_TYPE = SemanticSegmentationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "SemanticSegmentationData":
-        """Load the :class:`~flash.image.segmentation.data.SemanticSegmentationData` from folders containing image
-        files and folders containing mask files.
+        """Load the :class:`~flash.image.segmentation.data.SemanticSegmentationData` from folders containing image files
+        and folders containing mask files.
 
         The supported file extensions are: ``.jpg``, ``.jpeg``, ``.png``, ``.ppm``, ``.bmp``, ``.pgm``, ``.tif``,
         ``.tiff``, ``.webp``, and ``.npy``.
         For train, test, and validation data, the folders are expected to contain the images with a corresponding target
         folder which contains the mask in a file of the same name.
         For example, if your ``train_images`` folder (passed to the ``train_folder`` argument) looks like this:
 
@@ -286,18 +280,18 @@
 
             >>> import shutil
             >>> shutil.rmtree("train_images")
             >>> shutil.rmtree("train_masks")
             >>> shutil.rmtree("predict_folder")
         """
 
-        ds_kw = dict(
-            num_classes=num_classes,
-            labels_map=labels_map,
-        )
+        ds_kw = {
+            "num_classes": num_classes,
+            "labels_map": labels_map,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_folder, train_target_folder, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_folder, val_target_folder, **ds_kw),
             input_cls(RunningStage.TESTING, test_folder, test_target_folder, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_folder, **ds_kw),
             transform=transform,
@@ -318,16 +312,16 @@
         input_cls: Type[Input] = SemanticSegmentationNumpyInput,
         num_classes: Optional[int] = None,
         labels_map: Dict[int, Tuple[int, int, int]] = None,
         transform: INPUT_TRANSFORM_TYPE = SemanticSegmentationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "SemanticSegmentationData":
-        """Load the :class:`~flash.image.segmentation.data.SemanticSegmentationData` from numpy arrays containing
-        images (or lists of arrays) and corresponding numpy arrays containing masks (or lists of arrays).
+        """Load the :class:`~flash.image.segmentation.data.SemanticSegmentationData` from numpy arrays containing images
+        (or lists of arrays) and corresponding numpy arrays containing masks (or lists of arrays).
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
             train_data: The numpy array or list of arrays containing images to use when training.
             train_targets: The numpy array or list of arrays containing masks to use when training.
@@ -374,18 +368,18 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict(
-            num_classes=num_classes,
-            labels_map=labels_map,
-        )
+        ds_kw = {
+            "num_classes": num_classes,
+            "labels_map": labels_map,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
             input_cls(RunningStage.TESTING, test_data, test_targets, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_data, **ds_kw),
             transform=transform,
@@ -462,18 +456,18 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict(
-            num_classes=num_classes,
-            labels_map=labels_map,
-        )
+        ds_kw = {
+            "num_classes": num_classes,
+            "labels_map": labels_map,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
             input_cls(RunningStage.TESTING, test_data, test_targets, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_data, **ds_kw),
             transform=transform,
@@ -492,16 +486,16 @@
         num_classes: Optional[int] = None,
         labels_map: Dict[int, Tuple[int, int, int]] = None,
         transform: INPUT_TRANSFORM_TYPE = SemanticSegmentationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         label_field: str = "ground_truth",
         **data_module_kwargs: Any,
     ) -> "SemanticSegmentationData":
-        """Load the :class:`~flash.image.segmentation.data.SemanticSegmentationData` from FiftyOne
-        ``SampleCollection`` objects.
+        """Load the :class:`~flash.image.segmentation.data.SemanticSegmentationData` from FiftyOne ``SampleCollection``
+        objects.
 
         The supported file extensions are: ``.jpg``, ``.jpeg``, ``.png``, ``.ppm``, ``.bmp``, ``.pgm``, ``.tif``,
         ``.tiff``, ``.webp``, and ``.npy``.
         Mask image file paths will be extracted from the ``label_field`` in the ``SampleCollection`` objects.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/heads.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/heads.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         head: str,
         backbone: str,
         pretrained: Union[bool, str] = True,
         num_classes: int = 1,
         in_channels: int = 3,
         **kwargs,
     ) -> nn.Module:
-
         if head not in SMP_MODELS:
             raise NotImplementedError(f"{head} is not implemented! Supported heads -> {SMP_MODELS.keys()}")
 
         encoder_weights = None
         if isinstance(pretrained, str):
             encoder_weights = pretrained
         elif pretrained:
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/input.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 import os
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 from flash.core.data.io.input import DataKeys, Input
-from flash.core.data.utilities.loading import IMG_EXTENSIONS, load_image, NP_EXTENSIONS
-from flash.core.data.utilities.paths import filter_valid_files, PATH_TYPE
+from flash.core.data.utilities.loading import IMG_EXTENSIONS, NP_EXTENSIONS, load_image
+from flash.core.data.utilities.paths import PATH_TYPE, filter_valid_files
 from flash.core.data.utilities.samples import to_samples
 from flash.core.integrations.fiftyone.utils import FiftyOneLabelUtilities
 from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, lazy_import
 from flash.image.data import ImageFilesInput, ImageNumpyInput, ImageTensorInput
 from flash.image.segmentation.output import SegmentationLabelsOutput
 
 if _FIFTYONE_AVAILABLE:
@@ -90,15 +90,15 @@
             files = filter_valid_files(files, valid_extensions=IMG_EXTENSIONS + NP_EXTENSIONS)
         else:
             files, mask_files = filter_valid_files(files, mask_files, valid_extensions=IMG_EXTENSIONS + NP_EXTENSIONS)
         return to_samples(files, mask_files)
 
     def load_sample(self, sample: Dict[str, Any]) -> Dict[str, Any]:
         if DataKeys.TARGET in sample:
-            sample[DataKeys.TARGET] = np.array(load_image(sample[DataKeys.TARGET])).transpose((2, 0, 1))[:, :, 0]
+            sample[DataKeys.TARGET] = np.array(load_image(sample[DataKeys.TARGET])).transpose((2, 0, 1))[0, :, :]
         return super().load_sample(sample)
 
 
 class SemanticSegmentationFolderInput(SemanticSegmentationFilesInput):
     def load_data(
         self,
         folder: PATH_TYPE,
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/input_transform.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/input_transform.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/model.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Type, Union
 
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.nn import functional as F
 
 from flash.core.classification import ClassificationTask
 from flash.core.data.io.input import DataKeys, ServeInput
 from flash.core.data.io.output import Output
 from flash.core.data.io.output_transform import OutputTransform
 from flash.core.model import Task
 from flash.core.registry import FlashRegistry
 from flash.core.serve import Composition
 from flash.core.utilities.imports import (
-    _TM_GREATER_EQUAL_0_7_0,
     _TM_GREATER_EQUAL_0_10_0,
     _TORCHVISION_AVAILABLE,
     _TORCHVISION_GREATER_EQUAL_0_9,
     requires,
 )
 from flash.core.utilities.isinstance import _isinstance
 from flash.core.utilities.types import (
@@ -54,18 +53,16 @@
 
         class InterpolationMode:
             NEAREST = "nearest"
 
 
 if _TM_GREATER_EQUAL_0_10_0:
     from torchmetrics.classification import MulticlassJaccardIndex as JaccardIndex
-elif _TM_GREATER_EQUAL_0_7_0:
-    from torchmetrics import JaccardIndex
 else:
-    from torchmetrics import IoU as JaccardIndex
+    from torchmetrics import JaccardIndex
 
 
 class SemanticSegmentationOutputTransform(OutputTransform):
     def per_sample_transform(self, sample: Any) -> Any:
         resize = T.Resize(sample[DataKeys.METADATA]["size"], interpolation=InterpolationMode.NEAREST)
         sample[DataKeys.PREDS] = resize(sample[DataKeys.PREDS])
         sample[DataKeys.INPUT] = resize(sample[DataKeys.INPUT])
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/output.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,32 +50,32 @@
 
 
 SEMANTIC_SEGMENTATION_OUTPUTS = FlashRegistry("outputs")
 
 
 @SEMANTIC_SEGMENTATION_OUTPUTS(name="labels")
 class SegmentationLabelsOutput(Output):
-    """A :class:`.Output` which converts the model outputs to the label of the argmax classification per pixel in
-    the image for semantic segmentation tasks.
+    """A :class:`.Output` which converts the model outputs to the label of the argmax classification per pixel in the
+    image for semantic segmentation tasks.
 
     Args:
         labels_map: A dictionary that map the labels ids to pixel intensities.
         visualize: Whether to visualize the image labels.
     """
 
     @requires("image")
     def __init__(self, labels_map: Optional[Dict[int, Tuple[int, int, int]]] = None, visualize: bool = False):
         super().__init__()
         self.labels_map = labels_map
         self.visualize = visualize
 
     @staticmethod
     def labels_to_image(img_labels: Tensor, labels_map: Dict[int, Tuple[int, int, int]]) -> Tensor:
-        """Function that given an image with labels ids and their pixel intensity mapping, creates an RGB
-        representation for visualisation purposes."""
+        """Function that given an image with labels ids and their pixel intensity mapping, creates an RGB representation
+        for visualisation purposes."""
         assert len(img_labels.shape) == 2, img_labels.shape
         H, W = img_labels.shape
         out = torch.empty(3, H, W, dtype=torch.uint8)
         for label_id, label_val in labels_map.items():
             mask = img_labels == label_id
             for i in range(3):
                 out[i].masked_fill_(mask, label_val[i])
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/segmentation/viz.py` & `lightning-flash-0.8.2/src/flash/image/segmentation/viz.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/style_transfer/backbones.py` & `lightning-flash-0.8.2/src/flash/image/style_transfer/backbones.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from flash.core.utilities.providers import _PYSTICHE
 
 STYLE_TRANSFER_BACKBONES = FlashRegistry("backbones")
 
 __all__ = ["STYLE_TRANSFER_BACKBONES"]
 
 if _PYSTICHE_AVAILABLE:
-
     from pystiche import enc
 
     MLE_FN_PATTERN = re.compile(r"^(?P<name>\w+?)_multi_layer_encoder$")
 
     for mle_fn in dir(enc):
         match = MLE_FN_PATTERN.match(mle_fn)
         if not match:
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/style_transfer/cli.py` & `lightning-flash-0.8.2/src/flash/image/style_transfer/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/image/style_transfer/data.py` & `lightning-flash-0.8.2/src/flash/image/style_transfer/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 from typing import Any, Collection, Dict, Optional, Sequence, Type
 
 import numpy as np
 from torch import Tensor
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
-from flash.core.utilities.imports import _IMAGE_TESTING
 from flash.core.utilities.stability import beta
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.image.classification.input import ImageClassificationFilesInput, ImageClassificationFolderInput
 from flash.image.data import ImageNumpyInput, ImageTensorInput
 from flash.image.style_transfer.input_transform import StyleTransferInputTransform
 
 # Skip doctests if requirements aren't available
-if not _IMAGE_TESTING:
-    __doctest_skip__ = ["StyleTransferData", "StyleTransferData.*"]
+# if not _TOPIC_IMAGE_AVAILABLE:
+# skipping as there are some connection/download issues
+__doctest_skip__ = ["StyleTransferData", "StyleTransferData.*"]
 
 
 @beta("Style transfer is currently in Beta.")
 class StyleTransferData(DataModule):
-    """The ``StyleTransferData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
-    classmethods for loading data for image style transfer."""
+    """The ``StyleTransferData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of classmethods
+    for loading data for image style transfer."""
 
     input_transform_cls = StyleTransferInputTransform
 
     @classmethod
     def from_files(
         cls,
         train_files: Optional[Sequence[str]] = None,
@@ -201,16 +201,15 @@
         train_data: Optional[Collection[np.ndarray]] = None,
         predict_data: Optional[Collection[np.ndarray]] = None,
         input_cls: Type[Input] = ImageNumpyInput,
         transform: INPUT_TRANSFORM_TYPE = StyleTransferInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any
     ) -> "StyleTransferData":
-        """Load the :class:`~flash.image.style_transfer.data.StyleTransferData` from numpy arrays (or lists of
-        arrays).
+        """Load the :class:`~flash.image.style_transfer.data.StyleTransferData` from numpy arrays (or lists of arrays).
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
             train_data: The numpy array or list of arrays to use when training.
             predict_data: The numpy array or list of arrays to use when predicting.
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/style_transfer/input_transform.py` & `lightning-flash-0.8.2/src/flash/text/input.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,28 +7,19 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from dataclasses import dataclass
-from typing import Callable
+from typing import Any, Dict
 
-from flash.core.data.io.input import DataKeys
-from flash.core.data.io.input_transform import InputTransform
-from flash.core.data.transforms import ApplyToKeys
-from flash.core.utilities.imports import _TORCHVISION_AVAILABLE
+from flash.core.data.io.input import DataKeys, ServeInput
 
-if _TORCHVISION_AVAILABLE:
-    from torchvision import transforms as T
 
+class TextDeserializer(ServeInput):
+    def serve_load_sample(self, text: str) -> Dict[str, Any]:
+        return {DataKeys.INPUT: text}
 
-@dataclass
-class StyleTransferInputTransform(InputTransform):
-
-    image_size: int = 256
-
-    def per_sample_transform(self) -> Callable:
-        return ApplyToKeys(
-            DataKeys.INPUT, T.Compose([T.ToTensor(), T.Resize(self.image_size), T.CenterCrop(self.image_size)])
-        )
+    @property
+    def example_input(self) -> str:
+        return "An example input"
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/style_transfer/model.py` & `lightning-flash-0.8.2/src/flash/image/style_transfer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, cast, List, NoReturn, Optional, Sequence, Tuple, Union
+from typing import Any, List, NoReturn, Optional, Sequence, Tuple, Union, cast
 
-from torch import nn, Tensor
+from torch import Tensor, nn
 
 from flash.core.data.io.input import DataKeys
 from flash.core.model import Task
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _IMAGE_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_IMAGE_AVAILABLE
 from flash.core.utilities.stability import beta
 from flash.core.utilities.types import LR_SCHEDULER_TYPE, OPTIMIZER_TYPE
 from flash.image.style_transfer import STYLE_TRANSFER_BACKBONES
 
-if _IMAGE_AVAILABLE:
+if _TOPIC_IMAGE_AVAILABLE:
     import pystiche.demo
     from pystiche import enc, loss
     from pystiche.image import read_image
 else:
 
     class enc:
         Encoder = None
```

### Comparing `lightning-flash-0.8.1.post0/flash/image/style_transfer/utils.py` & `lightning-flash-0.8.2/src/flash/image/style_transfer/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/backbones.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/cli.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/data.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     PointCloudObjectDetectionDataFormat,
     PointCloudObjectDetectorFoldersInput,
 )
 
 
 @beta("Point cloud object detection is currently in Beta.")
 class PointCloudObjectDetectorData(DataModule):
-
     input_transform_cls = InputTransform
 
     @classmethod
     def from_folders(
         cls,
         train_folder: Optional[str] = None,
         val_folder: Optional[str] = None,
@@ -45,21 +44,20 @@
         calibrations_folder_name: Optional[str] = "calibs",
         data_format: Optional[BaseDataFormat] = PointCloudObjectDetectionDataFormat.KITTI,
         input_cls: Type[Input] = PointCloudObjectDetectorFoldersInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "PointCloudObjectDetectorData":
-
-        ds_kw = dict(
-            scans_folder_name=scans_folder_name,
-            labels_folder_name=labels_folder_name,
-            calibrations_folder_name=calibrations_folder_name,
-            data_format=data_format,
-        )
+        ds_kw = {
+            "scans_folder_name": scans_folder_name,
+            "labels_folder_name": labels_folder_name,
+            "calibrations_folder_name": calibrations_folder_name,
+            "data_format": data_format,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_folder, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_folder, **ds_kw),
             input_cls(RunningStage.TESTING, test_folder, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_folder, **ds_kw),
             transform=transform,
@@ -76,21 +74,20 @@
         calibrations_folder_name: Optional[str] = "calibs",
         data_format: Optional[BaseDataFormat] = PointCloudObjectDetectionDataFormat.KITTI,
         input_cls: Type[Input] = PointCloudObjectDetectorFoldersInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "PointCloudObjectDetectorData":
-
-        ds_kw = dict(
-            scans_folder_name=scans_folder_name,
-            labels_folder_name=labels_folder_name,
-            calibrations_folder_name=calibrations_folder_name,
-            data_format=data_format,
-        )
+        ds_kw = {
+            "scans_folder_name": scans_folder_name,
+            "labels_folder_name": labels_folder_name,
+            "calibrations_folder_name": calibrations_folder_name,
+            "data_format": data_format,
+        }
 
         return cls(
             predict_input=input_cls(RunningStage.PREDICTING, predict_files, **ds_kw),
             transform=transform,
             transform_kwargs=transform_kwargs,
             **data_module_kwargs,
         )
@@ -103,16 +100,15 @@
         test_dataset: Optional[Dataset] = None,
         predict_dataset: Optional[Dataset] = None,
         input_cls: Type[Input] = PointCloudObjectDetectorDatasetInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "PointCloudObjectDetectorData":
-
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_dataset, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_dataset, **ds_kw),
             input_cls(RunningStage.TESTING, test_dataset, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_dataset, **ds_kw),
             transform=transform,
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/datasets.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_POINTCLOUD_AVAILABLE
 from flash.pointcloud.segmentation.datasets import executor
 
-if _POINTCLOUD_AVAILABLE:
+if _TOPIC_POINTCLOUD_AVAILABLE:
     from open3d.ml.datasets import KITTI
 
 _OBJECT_DETECTION_DATASET = FlashRegistry("dataset")
 
 
 @_OBJECT_DETECTION_DATASET
 def kitti(dataset_path, download, **kwargs):
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/input.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/input.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/model.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import sys
 from typing import Any, Dict, Optional, Tuple, Union
 
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.utils.data import DataLoader, Sampler
 
 import flash
 from flash.core.data.io.input import DataKeys, InputBase
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.utilities.collate import wrap_collate
 from flash.core.model import Task
@@ -65,15 +65,14 @@
         lr_scheduler: LR_SCHEDULER_TYPE = None,
         metrics: METRICS_TYPE = None,
         learning_rate: Optional[float] = None,
         lambda_loss_cls: float = 1.0,
         lambda_loss_bbox: float = 1.0,
         lambda_loss_dir: float = 1.0,
     ):
-
         super().__init__(
             model=None,
             loss_fn=loss_fn,
             optimizer=optimizer,
             lr_scheduler=lr_scheduler,
             metrics=metrics,
             learning_rate=learning_rate,
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/open3d_ml/app.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/open3d_ml/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 # limitations under the License.
 import numpy as np
 from torch.utils.data.dataset import Dataset
 
 import flash
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import DataKeys
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE
-
-if _POINTCLOUD_AVAILABLE:
+from flash.core.utilities.imports import _TOPIC_POINTCLOUD_AVAILABLE
 
+if _TOPIC_POINTCLOUD_AVAILABLE:
     from open3d._ml3d.vis.visualizer import LabelLUT, Visualizer
     from open3d.visualization import gui
 
     class Visualizer(Visualizer):
         def visualize_dataset(self, dataset, split, indices=None, width=1024, height=768):
             """Visualize a dataset.
 
@@ -99,15 +98,14 @@
                 self._update_geometry()
                 self.setup_camera()
 
             self._load_geometries(self._objects.data_names, on_done_ui)
             gui.Application.instance.run()
 
     class VizDataset(Dataset):
-
         name = "VizDataset"
 
         def __init__(self, dataset):
             self.dataset = dataset
             self.label_to_names = getattr(dataset, "label_to_names", {})
             self.path_list = getattr(dataset, "path_list", [])
             self.color_map = getattr(dataset, "color_map", {})
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/open3d_ml/backbones.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/open3d_ml/backbones.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 from abc import ABC
 from typing import Callable
 
 import torch
 from pytorch_lightning.utilities.cloud_io import load as pl_load
 
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_POINTCLOUD_AVAILABLE
 from flash.core.utilities.providers import _OPEN3D_ML
 from flash.core.utilities.url_error import catch_url_error
 
 ROOT_URL = "https://storage.googleapis.com/open3d-releases/model-zoo/"
 
-if _POINTCLOUD_AVAILABLE:
+if _TOPIC_POINTCLOUD_AVAILABLE:
     import open3d
     import open3d.ml as _ml3d
     from open3d._ml3d.torch.dataloaders.concat_batcher import ConcatBatcher, ObjectDetectBatch
     from open3d._ml3d.torch.models.point_pillars import PointPillars
     from open3d.ml.torch.dataloaders import DefaultBatcher
 else:
     ObjectDetectBatch = ABC
@@ -46,16 +46,15 @@
         return self
 
     def __len__(self):
         return self.num_batches
 
 
 def register_open_3d_ml(register: FlashRegistry):
-    if _POINTCLOUD_AVAILABLE:
-
+    if _TOPIC_POINTCLOUD_AVAILABLE:
         CONFIG_PATH = os.path.join(os.path.dirname(open3d.__file__), "_ml3d/configs")
 
         def get_collate_fn(model) -> Callable:
             batcher_name = model.cfg.batcher
             if batcher_name == "DefaultBatcher":
                 batcher = DefaultBatcher()
             elif batcher_name == "ConcatBatcher":
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/detection/open3d_ml/input.py` & `lightning-flash-0.8.2/src/flash/pointcloud/detection/open3d_ml/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import os
 from os.path import basename, dirname, exists, isdir, isfile, join
 from typing import Any, Dict, List, Optional, Type, Union
 
 import yaml
 
 from flash.core.data.io.input import BaseDataFormat, Input
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_POINTCLOUD_AVAILABLE
 
-if _POINTCLOUD_AVAILABLE:
-    from open3d._ml3d.datasets.kitti import DataProcessing, KITTI
+if _TOPIC_POINTCLOUD_AVAILABLE:
+    from open3d._ml3d.datasets.kitti import KITTI, DataProcessing
 
 
 class PointCloudObjectDetectionDataFormat(BaseDataFormat):
     KITTI = "kitti"
 
 
 class BasePointCloudObjectDetectorLoader:
@@ -149,24 +149,24 @@
         return [{"scan_path": scan_path, "calibration_path": clean_fn(scan_path)} for scan_path in scan_paths]
 
     def predict_load_data(self, data, dataset: Input):
         if (isinstance(data, str) and isfile(data)) or (isinstance(data, list) and all(isfile(p) for p in data)):
             return self.load_files(data, dataset)
         if isinstance(data, str) and isdir(data):
             raise NotImplementedError
+        return None
 
     def predict_load_sample(self, metadata: Dict[str, str]):
         metadata, attr = self.load_sample(metadata, has_label=False)
         # hack to prevent manipulation of labels
         attr["split"] = "test"
         return metadata, attr
 
 
 class PointCloudObjectDetectorFoldersInput(Input):
-
     loaders: Dict[PointCloudObjectDetectionDataFormat, Type[BasePointCloudObjectDetectorLoader]] = {
         PointCloudObjectDetectionDataFormat.KITTI: KITTIPointCloudObjectDetectorLoader
     }
 
     def _get_loader(
         self, data_format: Optional[BaseDataFormat] = None, image_size: tuple = (375, 1242), **loader_kwargs: Any
     ) -> BasePointCloudObjectDetectorLoader:
@@ -225,15 +225,14 @@
         **loader_kwargs: Any,
     ) -> Any:
         self._validate_predict_data(data)
         self.loader = self._get_loader(data_format, image_size, **loader_kwargs)
         return self.loader.predict_load_data(data, self)
 
     def predict_load_sample(self, metadata: Dict[str, str]) -> Any:
-
         data, metadata = self.loader.predict_load_sample(metadata)
 
         input_transform_fn = getattr(self, "input_transform_fn", None)
         if input_transform_fn:
             data = input_transform_fn(data, metadata)
 
         transform_fn = getattr(self, "transform_fn", None)
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/backbones.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/cli.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/data.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,31 +22,29 @@
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.pointcloud.segmentation.input import PointCloudSegmentationDatasetInput, PointCloudSegmentationFoldersInput
 
 
 @beta("Point cloud segmentation is currently in Beta.")
 class PointCloudSegmentationData(DataModule):
-
     input_transform_cls = InputTransform
 
     @classmethod
     def from_folders(
         cls,
         train_folder: Optional[str] = None,
         val_folder: Optional[str] = None,
         test_folder: Optional[str] = None,
         predict_folder: Optional[str] = None,
         input_cls: Type[Input] = PointCloudSegmentationFoldersInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "PointCloudSegmentationData":
-
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_folder, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_folder, **ds_kw),
             input_cls(RunningStage.TESTING, test_folder, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_folder, **ds_kw),
             transform=transform,
@@ -59,16 +57,15 @@
         cls,
         predict_files: Optional[List[str]] = None,
         input_cls: Type[Input] = PointCloudSegmentationFoldersInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "PointCloudSegmentationData":
-
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             predict_input=input_cls(RunningStage.PREDICTING, predict_files, **ds_kw),
             transform=transform,
             transform_kwargs=transform_kwargs,
             **data_module_kwargs,
         )
@@ -81,16 +78,15 @@
         test_dataset: Optional[Dataset] = None,
         predict_dataset: Optional[Dataset] = None,
         input_cls: Type[Input] = PointCloudSegmentationDatasetInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "PointCloudSegmentationData":
-
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_dataset, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_dataset, **ds_kw),
             input_cls(RunningStage.TESTING, test_dataset, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_dataset, **ds_kw),
             transform=transform,
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/datasets.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_POINTCLOUD_AVAILABLE
 
-if _POINTCLOUD_AVAILABLE:
+if _TOPIC_POINTCLOUD_AVAILABLE:
     from open3d.ml.datasets import Lyft, SemanticKITTI
 
 _SEGMENTATION_DATASET = FlashRegistry("dataset")
 
 
 def executor(download_script, preprocess_script, dataset_path, name):
     if not os.path.exists(os.path.join(dataset_path, name)):
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/input.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/input.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/model.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,39 +10,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, Iterable, Optional, Tuple, Union
 
 import torch
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.nn import functional as F
 from torch.utils.data import DataLoader, Sampler
 
 import flash
 from flash.core.classification import ClassificationTask
 from flash.core.data.io.input import DataKeys, InputBase
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.utilities.collate import wrap_collate
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE, _TM_GREATER_EQUAL_0_7_0, _TM_GREATER_EQUAL_0_10_0
+from flash.core.utilities.imports import _TM_GREATER_EQUAL_0_10_0, _TOPIC_POINTCLOUD_AVAILABLE
 from flash.core.utilities.stability import beta
 from flash.core.utilities.types import LOSS_FN_TYPE, LR_SCHEDULER_TYPE, METRICS_TYPE, OPTIMIZER_TYPE
 from flash.pointcloud.segmentation.backbones import POINTCLOUD_SEGMENTATION_BACKBONES
 
-if _POINTCLOUD_AVAILABLE:
+if _TOPIC_POINTCLOUD_AVAILABLE:
     from open3d._ml3d.torch.modules.losses.semseg_loss import filter_valid_label
     from open3d.ml.torch.dataloaders import TorchDataloader
 
 if _TM_GREATER_EQUAL_0_10_0:
     from torchmetrics.classification import MulticlassJaccardIndex as JaccardIndex
-elif _TM_GREATER_EQUAL_0_7_0:
-    from torchmetrics import JaccardIndex
 else:
-    from torchmetrics import IoU as JaccardIndex
+    from torchmetrics import JaccardIndex
 
 
 @beta("Point cloud segmentation is currently in Beta.")
 class PointCloudSegmentation(ClassificationTask):
     """The ``PointCloudClassifier`` is a :class:`~flash.core.classification.ClassificationTask` that classifies
     pointcloud data.
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/open3d_ml/app.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/open3d_ml/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import torch
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import DataKeys
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE
-
-if _POINTCLOUD_AVAILABLE:
+from flash.core.utilities.imports import _TOPIC_POINTCLOUD_AVAILABLE
 
+if _TOPIC_POINTCLOUD_AVAILABLE:
     from open3d._ml3d.torch.dataloaders import TorchDataloader
     from open3d._ml3d.vis.visualizer import LabelLUT
     from open3d._ml3d.vis.visualizer import Visualizer as Open3dVisualizer
 
 else:
-
     Open3dVisualizer = object
 
 
 class Visualizer(Open3dVisualizer):
     def visualize_dataset(self, dataset, split, indices=None, width=1024, height=768):
         """Visualize a dataset.
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/open3d_ml/backbones.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/open3d_ml/backbones.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 import os
 from typing import Callable
 
 import torch
 from pytorch_lightning.utilities.cloud_io import load as pl_load
 
 from flash.core.registry import FlashRegistry
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_POINTCLOUD_AVAILABLE
 from flash.core.utilities.providers import _OPEN3D_ML
 from flash.core.utilities.url_error import catch_url_error
 
 ROOT_URL = "https://storage.googleapis.com/open3d-releases/model-zoo/"
 
 
 def register_open_3d_ml(register: FlashRegistry):
-    if _POINTCLOUD_AVAILABLE:
+    if _TOPIC_POINTCLOUD_AVAILABLE:
         import open3d
         import open3d.ml as _ml3d
         from open3d._ml3d.torch.dataloaders import ConcatBatcher, DefaultBatcher
         from open3d._ml3d.torch.models import RandLANet
 
         CONFIG_PATH = os.path.join(os.path.dirname(open3d.__file__), "_ml3d/configs")
```

### Comparing `lightning-flash-0.8.1.post0/flash/pointcloud/segmentation/open3d_ml/sequences_dataset.py` & `lightning-flash-0.8.2/src/flash/pointcloud/segmentation/open3d_ml/sequences_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 import os
 from os.path import basename, dirname, exists, isdir, isfile, join, split
 
 import numpy as np
 import yaml
 from torch.utils.data import Dataset
 
-from flash.core.utilities.imports import _POINTCLOUD_AVAILABLE
-
-if _POINTCLOUD_AVAILABLE:
+from flash.core.utilities.imports import _TOPIC_POINTCLOUD_AVAILABLE
 
+if _TOPIC_POINTCLOUD_AVAILABLE:
     from open3d._ml3d.datasets.utils import DataProcessing
     from open3d._ml3d.utils.config import Config
 
 
 class SequencesDataset(Dataset):
     meta: dict
     split: str
@@ -40,15 +39,14 @@
         cache_dir="./logs/cache",
         use_cache=False,
         num_points=65536,
         ignored_label_inds=[0],
         predicting=False,
         **kwargs,
     ):
-
         super().__init__()
 
         self.name = "Dataset"
         self.ignored_label_inds = ignored_label_inds
 
         kwargs["cache_dir"] = cache_dir
         kwargs["use_cache"] = use_cache
@@ -145,42 +143,38 @@
         return data
 
     def get_data(self, idx):
         pc_path = self.path_list[idx]
         points = DataProcessing.load_pc_kitti(pc_path)
 
         folder, file = split(pc_path)
-        if self.predicting:
-            label_path = join(folder, file[:-4] + ".label")
-        else:
-            label_path = join(folder, "../labels", file[:-4] + ".label")
+        label_path = (
+            join(folder, file[:-4] + ".label") if self.predicting else join(folder, "../labels", file[:-4] + ".label")
+        )
         if not exists(label_path):
             labels = np.zeros(np.shape(points)[0], dtype=np.int32)
             if self.split not in ["test", "all"]:
                 raise FileNotFoundError(f" Label file {label_path} not found")
 
         else:
             labels = DataProcessing.load_label_kitti(label_path, self.remap_lut_val).astype(np.int32)
 
-        data = {
+        return {
             "point": points[:, 0:3],
             "feat": None,
             "label": labels,
         }
 
-        return data
-
     def get_attr(self, idx):
         pc_path = self.path_list[idx]
         folder, file = split(pc_path)
         _, seq = split(split(folder)[0])
         name = f"{seq}_{file[:-4]}"
 
         pc_path = str(pc_path)
-        attr = {"idx": idx, "name": name, "path": pc_path, "split": self.split}
-        return attr
+        return {"idx": idx, "name": name, "path": pc_path, "split": self.split}
 
     def __len__(self):
         return len(self.path_list)
 
     def get_split(self, *_):
         return self
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/classification/cli.py` & `lightning-flash-0.8.2/src/flash/tabular/classification/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/classification/data.py` & `lightning-flash-0.8.2/src/flash/tabular/classification/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Type, Union
 
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import INPUT_TRANSFORM_TYPE, InputTransform
 from flash.core.data.utilities.classification import TargetFormatter
-from flash.core.utilities.imports import _PANDAS_AVAILABLE, _TABULAR_TESTING
+from flash.core.utilities.imports import _PANDAS_AVAILABLE, _TOPIC_TABULAR_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.tabular.classification.input import (
     TabularClassificationCSVInput,
     TabularClassificationDataFrameInput,
     TabularClassificationDictInput,
     TabularClassificationListInput,
 )
@@ -28,15 +28,15 @@
 
 if _PANDAS_AVAILABLE:
     from pandas.core.frame import DataFrame
 else:
     DataFrame = object
 
 # Skip doctests if requirements aren't available
-if not _TABULAR_TESTING:
+if not _TOPIC_TABULAR_AVAILABLE:
     __doctest_skip__ = ["TabularClassificationData", "TabularClassificationData.*"]
 
 
 class TabularClassificationData(TabularData):
     """The ``TabularClassificationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for tabular classification."""
 
@@ -53,16 +53,16 @@
         predict_data_frame: Optional[DataFrame] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = TabularClassificationDataFrameInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TabularClassificationData":
-        """Creates a :class:`~flash.tabular.classification.data.TabularClassificationData` object from the given
-        data frames.
+        """Creates a :class:`~flash.tabular.classification.data.TabularClassificationData` object from the given data
+        frames.
 
         .. note::
 
             The ``categorical_fields``, ``numerical_fields``, and ``target_fields`` do not need to be provided if
             ``parameters`` are passed instead. These can be obtained from the
             :attr:`~flash.tabular.data.TabularData.parameters` attribute of the
             :class:`~flash.tabular.data.TabularData` object that contains your training data.
@@ -153,21 +153,21 @@
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            categorical_fields=categorical_fields,
-            numerical_fields=numerical_fields,
-            target_fields=target_fields,
-            parameters=parameters,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "categorical_fields": categorical_fields,
+            "numerical_fields": numerical_fields,
+            "target_fields": target_fields,
+            "parameters": parameters,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data_frame, **ds_kw)
         ds_kw["parameters"] = train_input.parameters if train_input else parameters
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
@@ -192,16 +192,16 @@
         predict_file: Optional[str] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = TabularClassificationCSVInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TabularClassificationData":
-        """Creates a :class:`~flash.tabular.classification.data.TabularClassificationData` object from the given
-        CSV files.
+        """Creates a :class:`~flash.tabular.classification.data.TabularClassificationData` object from the given CSV
+        files.
 
         .. note::
 
             The ``categorical_fields``, ``numerical_fields``, and ``target_fields`` do not need to be provided if
             ``parameters`` are passed instead. These can be obtained from the
             :attr:`~flash.tabular.data.TabularData.parameters` attribute of the
             :class:`~flash.tabular.data.TabularData` object that contains your training data.
@@ -355,21 +355,21 @@
 
         .. testcleanup::
 
             >>> import os
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            categorical_fields=categorical_fields,
-            numerical_fields=numerical_fields,
-            target_fields=target_fields,
-            parameters=parameters,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "categorical_fields": categorical_fields,
+            "numerical_fields": numerical_fields,
+            "target_fields": target_fields,
+            "parameters": parameters,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_file, **ds_kw)
         ds_kw["parameters"] = train_input.parameters if train_input else parameters
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
@@ -491,21 +491,21 @@
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            categorical_fields=categorical_fields,
-            numerical_fields=numerical_fields,
-            target_fields=target_fields,
-            parameters=parameters,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "categorical_fields": categorical_fields,
+            "numerical_fields": numerical_fields,
+            "target_fields": target_fields,
+            "parameters": parameters,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_dict, **ds_kw)
         ds_kw["parameters"] = train_input.parameters if train_input else parameters
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
@@ -530,16 +530,16 @@
         predict_list: Optional[List[Union[tuple, dict]]] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = TabularClassificationListInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TabularClassificationData":
-        """Creates a :class:`~flash.tabular.classification.data.TabularClassificationData` object from the given
-        data (in the form of list of a tuple or a dictionary).
+        """Creates a :class:`~flash.tabular.classification.data.TabularClassificationData` object from the given data
+        (in the form of list of a tuple or a dictionary).
 
         .. note::
             The ``categorical_fields``, ``numerical_fields``, and ``target_fields`` do not need to be provided if
             ``parameters`` are passed instead. These can be obtained from the
             :attr:`~flash.tabular.data.TabularData.parameters` attribute of the
             :class:`~flash.tabular.data.TabularData` object that contains your training data.
 
@@ -629,21 +629,21 @@
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            categorical_fields=categorical_fields,
-            numerical_fields=numerical_fields,
-            target_fields=target_fields,
-            parameters=parameters,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "categorical_fields": categorical_fields,
+            "numerical_fields": numerical_fields,
+            "target_fields": target_fields,
+            "parameters": parameters,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_list, **ds_kw)
         ds_kw["parameters"] = train_input.parameters if train_input else parameters
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/classification/input.py` & `lightning-flash-0.8.2/src/flash/tabular/classification/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     ):
         cat_vars, num_vars = self.preprocess(data_frame, categorical_fields, numerical_fields, parameters)
 
         if not self.predicting:
             targets = resolve_targets(data_frame, target_fields)
             self.load_target_metadata(targets, target_formatter=target_formatter)
             return [{DataKeys.INPUT: (c, n), DataKeys.TARGET: t} for c, n, t in zip(cat_vars, num_vars, targets)]
-        else:
-            return [{DataKeys.INPUT: (c, n)} for c, n in zip(cat_vars, num_vars)]
+
+        return [{DataKeys.INPUT: (c, n)} for c, n in zip(cat_vars, num_vars)]
 
     def load_sample(self, sample: Dict[str, Any]) -> Any:
         if DataKeys.TARGET in sample:
             sample[DataKeys.TARGET] = self.format_target(sample[DataKeys.TARGET])
         return sample
 
 
@@ -62,14 +62,15 @@
         parameters: Dict[str, Any] = None,
         target_formatter: Optional[TargetFormatter] = None,
     ):
         if file is not None:
             return super().load_data(
                 load_data_frame(file), categorical_fields, numerical_fields, target_fields, parameters, target_formatter
             )
+        return None
 
 
 class TabularClassificationDictInput(TabularClassificationDataFrameInput):
     def load_data(
         self,
         data: Dict[str, Union[Any, List[Any]]],
         categorical_fields: Optional[Union[str, List[str]]] = None,
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/classification/model.py` & `lightning-flash-0.8.2/src/flash/tabular/classification/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 from flash.core.classification import ClassificationAdapterTask
 from flash.core.data.io.input import ServeInput
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.io.output import Output
 from flash.core.integrations.pytorch_tabular.backbones import PYTORCH_TABULAR_BACKBONES
 from flash.core.registry import FlashRegistry
 from flash.core.serve import Composition
-from flash.core.utilities.imports import _TABULAR_TESTING, requires
+from flash.core.utilities.imports import _TOPIC_TABULAR_AVAILABLE, requires
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE, LR_SCHEDULER_TYPE, METRICS_TYPE, OPTIMIZER_TYPE
 from flash.tabular.input import TabularDeserializer
 
 # Skip doctests if requirements aren't available
-if not _TABULAR_TESTING:
+if not _TOPIC_TABULAR_AVAILABLE:
     __doctest_skip__ = ["TabularClassifier", "TabularClassifier.*"]
 
 
 class TabularClassifier(ClassificationAdapterTask):
     """The ``TabularClassifier`` is a :class:`~flash.Task` for classifying tabular data. For more details, see
     :ref:`tabular_classification`.
 
@@ -98,61 +98,57 @@
             lr_scheduler=lr_scheduler,
             learning_rate=learning_rate,
             labels=labels,
         )
 
     @property
     def data_parameters(self) -> Dict[str, Any]:
-        """Get the parameters computed from the training data used to create this
-        :class:`~flash.tabular.classification.TabularClassifier`. Use these parameters to load data for
-        evaluation / prediction.
-
-        Examples
-        ________
-
-        .. doctest::
-
-            >>> import flash
-            >>> from flash.core.data.utils import download_data
-            >>> from flash.tabular import TabularClassificationData, TabularClassifier
-            >>> download_data("https://pl-flash-data.s3.amazonaws.com/titanic.zip", "./data")
-            >>> model = TabularClassifier.load_from_checkpoint(
-            ...     "https://flash-weights.s3.amazonaws.com/0.7.0/tabular_classification_model.pt"
-            ... )
-            >>> datamodule = TabularClassificationData.from_csv(
-            ...     predict_file="data/titanic/predict.csv",
-            ...     parameters=model.data_parameters,
-            ...     batch_size=8,
-            ... )
-            >>> trainer = flash.Trainer()
-            >>> trainer.predict(
-            ...     model,
-            ...     datamodule=datamodule,
-            ...     output="classes",
-            ... )  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
+        r"""Get the parameters computed from the training data used to create this
+        :class:`~flash.tabular.classification.TabularClassifier`. Use these parameters to load data for evaluation /
+        prediction.
+
+        Example::
+
+            import flash
+            from flash.core.data.utils import download_data
+            from flash.tabular import TabularClassificationData, TabularClassifier
+            download_data("https://pl-flash-data.s3.amazonaws.com/titanic.zip", "./data")
+            model = TabularClassifier.load_from_checkpoint(
+                "https://flash-weights.s3.amazonaws.com/0.7.0/tabular_classification_model.pt"
+            )
+            datamodule = TabularClassificationData.from_csv(
+                predict_file="data/titanic/predict.csv",
+                parameters=model.data_parameters,
+                batch_size=8,
+            )
+            trainer = flash.Trainer()
+            trainer.predict(
+                model,
+                datamodule=datamodule,
+                output="classes",
+            )
             Predicting...
         """
         return self._data_parameters
 
     @staticmethod
     def _ci_benchmark_fn(history: List[Dict[str, Any]]):
         """This function is used only for debugging usage with CI."""
         assert history[-1]["valid_accuracy"] > 0.6, history[-1]["valid_accuracy"]
 
     @classmethod
     def from_data(cls, datamodule, **kwargs) -> "TabularClassifier":
-        model = cls(
+        return cls(
             parameters=datamodule.parameters,
             embedding_sizes=datamodule.embedding_sizes,
             cat_dims=datamodule.cat_dims,
             num_features=datamodule.num_features,
             num_classes=datamodule.num_classes,
             **kwargs,
         )
-        return model
 
     @requires("serve")
     def serve(
         self,
         host: str = "127.0.0.1",
         port: int = 8000,
         sanity_check: bool = True,
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/classification/utils.py` & `lightning-flash-0.8.2/src/flash/tabular/classification/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 
 def _generate_codes(df: DataFrame, cat_cols: List) -> dict:
     tmp = df.copy()
     for col in cat_cols:
         tmp[col] = tmp[col].astype("category").cat.as_ordered()
 
     # list of categories for each column (always a column for None)
-    codes = {col: list(tmp[col].cat.categories) for col in cat_cols}
-
-    return codes
+    return {col: list(tmp[col].cat.categories) for col in cat_cols}
 
 
 def _categorize(df: DataFrame, cat_cols: List, codes) -> DataFrame:
     # apply codes to each column
     for col in cat_cols:
         df[col] = pd.Categorical(df[col], categories=codes[col], ordered=True)
     df[cat_cols] = df[cat_cols].apply(lambda x: x.cat.codes)
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/data.py` & `lightning-flash-0.8.2/src/flash/tabular/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.io.output_transform import OutputTransform
 
 
 class TabularData(DataModule):
-
     input_transform_cls = InputTransform
     output_transform_cls = OutputTransform
 
     @property
     def parameters(self) -> Optional[Dict[str, Any]]:
         """The parameters dictionary created from the train data when constructing the ``TabularData`` object."""
         return getattr(self.train_dataset, "parameters", None)
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/forecasting/cli.py` & `lightning-flash-0.8.2/src/flash/tabular/forecasting/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/forecasting/data.py` & `lightning-flash-0.8.2/src/flash/tabular/forecasting/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 
 from torch.utils.data.sampler import Sampler
 
 from flash.core.data.callback import BaseDataFetcher
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import INPUT_TRANSFORM_TYPE, InputTransform
-from flash.core.utilities.imports import _PANDAS_AVAILABLE, _TABULAR_TESTING
+from flash.core.utilities.imports import _PANDAS_AVAILABLE, _TOPIC_TABULAR_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.tabular.forecasting.input import TabularForecastingDataFrameInput
 
 if _PANDAS_AVAILABLE:
     from pandas.core.frame import DataFrame
 else:
     DataFrame = object
 
 
 # Skip doctests if requirements aren't available
-if not _TABULAR_TESTING:
+if not _TOPIC_TABULAR_AVAILABLE:
     __doctest_skip__ = ["TabularForecastingData", "TabularForecastingData.*"]
 
 
 class TabularForecastingData(DataModule):
     """The ``TabularForecastingData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for tabular forecasting."""
 
@@ -65,16 +65,15 @@
         batch_size: Optional[int] = None,
         num_workers: int = 0,
         sampler: Optional[Type[Sampler]] = None,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **input_kwargs: Any,
     ) -> "TabularForecastingData":
-        """Creates a :class:`~flash.tabular.forecasting.data.TabularForecastingData` object from the given data
-        frames.
+        """Creates a :class:`~flash.tabular.forecasting.data.TabularForecastingData` object from the given data frames.
 
         .. note::
 
             The ``time_idx``, ``target``, and ``group_ids`` do not need to be provided if ``parameters`` are passed
             instead. These can be obtained from the
             :attr:`~flash.tabular.forecasting.data.TabularForecastingData.parameters` attribute of the
             :class:`~flash.tabular.forecasting.data.TabularForecastingData` object that contains your training data.
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/forecasting/input.py` & `lightning-flash-0.8.2/src/flash/tabular/forecasting/input.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/forecasting/model.py` & `lightning-flash-0.8.2/src/flash/tabular/forecasting/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from flash.core.integrations.pytorch_forecasting.adapter import PyTorchForecastingAdapter
 from flash.core.integrations.pytorch_forecasting.backbones import PYTORCH_FORECASTING_BACKBONES
 from flash.core.registry import FlashRegistry
 from flash.core.utilities.types import LR_SCHEDULER_TYPE, OPTIMIZER_TYPE
 
 
 class TabularForecaster(AdapterTask):
-
     backbones: FlashRegistry = FlashRegistry("backbones") + PYTORCH_FORECASTING_BACKBONES
     required_extras: str = "tabular"
 
     def __init__(
         self,
         parameters: Dict[str, Any],
         backbone: str,
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/input.py` & `lightning-flash-0.8.2/src/flash/tabular/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,25 @@
 
     @staticmethod
     def compute_parameters(
         train_data_frame: DataFrame,
         numerical_fields: List[str],
         categorical_fields: List[str],
     ) -> Dict[str, Any]:
-
         mean, std = _compute_normalization(train_data_frame, numerical_fields)
 
         codes = _generate_codes(train_data_frame, categorical_fields)
 
-        return dict(
-            mean=mean,
-            std=std,
-            codes=codes,
-            numerical_fields=numerical_fields,
-            categorical_fields=categorical_fields,
-        )
+        return {
+            "mean": mean,
+            "std": std,
+            "codes": codes,
+            "numerical_fields": numerical_fields,
+            "categorical_fields": categorical_fields,
+        }
 
     def preprocess(
         self,
         df: DataFrame,
         categorical_fields: Optional[List[str]] = None,
         numerical_fields: Optional[List[str]] = None,
         parameters: Dict[str, Any] = None,
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/regression/cli.py` & `lightning-flash-0.8.2/src/flash/tabular/regression/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/regression/data.py` & `lightning-flash-0.8.2/src/flash/tabular/regression/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Type, Union
 
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import INPUT_TRANSFORM_TYPE, InputTransform
-from flash.core.utilities.imports import _PANDAS_AVAILABLE, _TABULAR_TESTING
+from flash.core.utilities.imports import _PANDAS_AVAILABLE, _TOPIC_TABULAR_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.tabular.data import TabularData
 from flash.tabular.regression.input import (
     TabularRegressionCSVInput,
     TabularRegressionDataFrameInput,
     TabularRegressionDictInput,
     TabularRegressionListInput,
@@ -27,15 +27,15 @@
 
 if _PANDAS_AVAILABLE:
     from pandas.core.frame import DataFrame
 else:
     DataFrame = object
 
 # Skip doctests if requirements aren't available
-if not _TABULAR_TESTING:
+if not _TOPIC_TABULAR_AVAILABLE:
     __doctest_skip__ = ["TabularRegressionData", "TabularRegressionData.*"]
 
 
 class TabularRegressionData(TabularData):
     """The ``TabularRegressionData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for tabular regression."""
 
@@ -51,16 +51,15 @@
         test_data_frame: Optional[DataFrame] = None,
         predict_data_frame: Optional[DataFrame] = None,
         input_cls: Type[Input] = TabularRegressionDataFrameInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TabularRegressionData":
-        """Creates a :class:`~flash.tabular.regression.data.TabularRegressionData` object from the given data
-        frames.
+        """Creates a :class:`~flash.tabular.regression.data.TabularRegressionData` object from the given data frames.
 
         .. note::
 
             The ``categorical_fields``, ``numerical_fields``, and ``target_field`` do not need to be provided if
             ``parameters`` are passed instead. These can be obtained from the
             :attr:`~flash.tabular.data.TabularData.parameters` attribute of the
             :class:`~flash.tabular.data.TabularData` object that contains your training data.
@@ -144,20 +143,20 @@
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
-        ds_kw = dict(
-            categorical_fields=categorical_fields,
-            numerical_fields=numerical_fields,
-            target_field=target_field,
-            parameters=parameters,
-        )
+        ds_kw = {
+            "categorical_fields": categorical_fields,
+            "numerical_fields": numerical_fields,
+            "target_field": target_field,
+            "parameters": parameters,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data_frame, **ds_kw)
         ds_kw["parameters"] = train_input.parameters if train_input else parameters
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data_frame, **ds_kw),
@@ -331,20 +330,20 @@
 
         .. testcleanup::
 
             >>> import os
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
-        ds_kw = dict(
-            categorical_fields=categorical_fields,
-            numerical_fields=numerical_fields,
-            target_field=target_field,
-            parameters=parameters,
-        )
+        ds_kw = {
+            "categorical_fields": categorical_fields,
+            "numerical_fields": numerical_fields,
+            "target_field": target_field,
+            "parameters": parameters,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_file, **ds_kw)
         ds_kw["parameters"] = train_input.parameters if train_input else parameters
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
@@ -367,16 +366,15 @@
         test_dict: Optional[Dict[str, List[Any]]] = None,
         predict_dict: Optional[Dict[str, List[Any]]] = None,
         input_cls: Type[Input] = TabularRegressionDictInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TabularRegressionData":
-        """Creates a :class:`~flash.tabular.regression.data.TabularRegressionData` object from the given
-        dictionary.
+        """Creates a :class:`~flash.tabular.regression.data.TabularRegressionData` object from the given dictionary.
 
         .. note::
 
             The ``categorical_fields``, ``numerical_fields``, and ``target_field`` do not need to be provided if
             ``parameters`` are passed instead. These can be obtained from the
             :attr:`~flash.tabular.data.TabularData.parameters` attribute of the
             :class:`~flash.tabular.data.TabularData` object that contains your training data.
@@ -458,20 +456,20 @@
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
-        ds_kw = dict(
-            categorical_fields=categorical_fields,
-            numerical_fields=numerical_fields,
-            target_field=target_field,
-            parameters=parameters,
-        )
+        ds_kw = {
+            "categorical_fields": categorical_fields,
+            "numerical_fields": numerical_fields,
+            "target_field": target_field,
+            "parameters": parameters,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_dict, **ds_kw)
         ds_kw["parameters"] = train_input.parameters if train_input else parameters
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_dict, **ds_kw),
@@ -494,16 +492,16 @@
         test_list: List[Union[tuple, dict]] = None,
         predict_list: List[Union[tuple, dict]] = None,
         input_cls: Type[Input] = TabularRegressionListInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TabularRegressionData":
-        """Creates a :class:`~flash.tabular.regression.data.TabularRegressionData` object from the given data (in
-        the form of list of a tuple or a dictionary).
+        """Creates a :class:`~flash.tabular.regression.data.TabularRegressionData` object from the given data (in the
+        form of list of a tuple or a dictionary).
 
         .. note::
 
             The ``categorical_fields``, ``numerical_fields``, and ``target_field`` do not need to be provided if
             ``parameters`` are passed instead. These can be obtained from the
             :attr:`~flash.tabular.data.TabularData.parameters` attribute of the
             :class:`~flash.tabular.data.TabularData` object that contains your training data.
@@ -587,20 +585,20 @@
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
-        ds_kw = dict(
-            categorical_fields=categorical_fields,
-            numerical_fields=numerical_fields,
-            target_field=target_field,
-            parameters=parameters,
-        )
+        ds_kw = {
+            "categorical_fields": categorical_fields,
+            "numerical_fields": numerical_fields,
+            "target_field": target_field,
+            "parameters": parameters,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_list, **ds_kw)
         ds_kw["parameters"] = train_input.parameters if train_input else parameters
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_list, **ds_kw),
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/regression/input.py` & `lightning-flash-0.8.2/src/flash/tabular/regression/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         parameters: Dict[str, Any] = None,
     ):
         cat_vars, num_vars = self.preprocess(data_frame, categorical_fields, numerical_fields, parameters)
 
         if not self.predicting:
             targets = data_frame[target_field].to_numpy().astype(np.float32)
             return [{DataKeys.INPUT: (c, n), DataKeys.TARGET: t} for c, n, t in zip(cat_vars, num_vars, targets)]
-        else:
-            return [{DataKeys.INPUT: (c, n)} for c, n in zip(cat_vars, num_vars)]
+
+        return [{DataKeys.INPUT: (c, n)} for c, n in zip(cat_vars, num_vars)]
 
 
 class TabularRegressionCSVInput(TabularRegressionDataFrameInput):
     def load_data(
         self,
         file: Optional[str],
         categorical_fields: Optional[Union[str, List[str]]] = None,
@@ -53,14 +53,15 @@
         target_field: Optional[str] = None,
         parameters: Dict[str, Any] = None,
     ):
         if file is not None:
             return super().load_data(
                 load_data_frame(file), categorical_fields, numerical_fields, target_field, parameters
             )
+        return None
 
 
 class TabularRegressionDictInput(TabularRegressionDataFrameInput):
     def load_data(
         self,
         data: Dict[str, List[Any]],
         categorical_fields: Optional[Union[str, List[str]]] = None,
```

### Comparing `lightning-flash-0.8.1.post0/flash/tabular/regression/model.py` & `lightning-flash-0.8.2/src/flash/tabular/regression/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 from flash.core.data.io.input import ServeInput
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.io.output import Output
 from flash.core.integrations.pytorch_tabular.backbones import PYTORCH_TABULAR_BACKBONES
 from flash.core.registry import FlashRegistry
 from flash.core.regression import RegressionAdapterTask
 from flash.core.serve import Composition
-from flash.core.utilities.imports import _TABULAR_TESTING, requires
+from flash.core.utilities.imports import _TOPIC_TABULAR_AVAILABLE, requires
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE, LR_SCHEDULER_TYPE, METRICS_TYPE, OPTIMIZER_TYPE
 from flash.tabular.input import TabularDeserializer
 
 # Skip doctests if requirements aren't available
-if not _TABULAR_TESTING:
+if not _TOPIC_TABULAR_AVAILABLE:
     __doctest_skip__ = ["TabularRegressor", "TabularRegressor.*"]
 
 
 class TabularRegressor(RegressionAdapterTask):
     """The ``TabularRegressor`` is a :class:`~flash.Task` for classifying tabular data. For more details, see
     :ref:`tabular_classification`.
 
@@ -94,54 +94,49 @@
             optimizer=optimizer,
             lr_scheduler=lr_scheduler,
             learning_rate=learning_rate,
         )
 
     @property
     def data_parameters(self) -> Dict[str, Any]:
-        """Get the parameters computed from the training data used to create this
-        :class:`~flash.tabular.regression.TabularRegressor`. Use these parameters to load data for
-        evaluation / prediction.
-
-        Examples
-        ________
-
-        .. doctest::
-
-            >>> import flash
-            >>> from flash.core.data.utils import download_data
-            >>> from flash.tabular import TabularRegressionData, TabularRegressor
-            >>> download_data("https://pl-flash-data.s3.amazonaws.com/SeoulBikeData.csv", "./data")
-            >>> model = TabularRegressor.load_from_checkpoint(
-            ...     "https://flash-weights.s3.amazonaws.com/0.7.0/tabular_regression_model.pt"
-            ... )
-            >>> datamodule = TabularRegressionData.from_csv(
-            ...     predict_file="data/SeoulBikeData.csv",
-            ...     parameters=model.data_parameters,
-            ...     batch_size=8,
-            ... )
-            >>> trainer = flash.Trainer()
-            >>> trainer.predict(
-            ...     model,
-            ...     datamodule=datamodule,
-            ... )  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-            Predicting...
+        r"""Get the parameters computed from the training data used to create this
+        :class:`~flash.tabular.regression.TabularRegressor`. Use these parameters to load data for evaluation /
+        prediction.
+
+        Example::
+
+            import flash
+            from flash.core.data.utils import download_data
+            from flash.tabular import TabularRegressionData, TabularRegressor
+            download_data("https://pl-flash-data.s3.amazonaws.com/SeoulBikeData.csv", "./data")
+            model = TabularRegressor.load_from_checkpoint(
+                "https://flash-weights.s3.amazonaws.com/0.7.0/tabular_regression_model.pt"
+            )
+            datamodule = TabularRegressionData.from_csv(
+                predict_file="data/SeoulBikeData.csv",
+                parameters=model.data_parameters,
+                batch_size=8,
+            )
+            trainer = flash.Trainer()
+            trainer.predict(
+                model,
+                datamodule=datamodule,
+            )
         """
         return self._data_parameters
 
     @classmethod
     def from_data(cls, datamodule, **kwargs) -> "TabularRegressor":
-        model = cls(
+        return cls(
             parameters=datamodule.parameters,
             embedding_sizes=datamodule.embedding_sizes,
             cat_dims=datamodule.cat_dims,
             num_features=datamodule.num_features,
             **kwargs
         )
-        return model
 
     @requires("serve")
     def serve(
         self,
         host: str = "127.0.0.1",
         port: int = 8000,
         sanity_check: bool = True,
```

### Comparing `lightning-flash-0.8.1.post0/flash/template/classification/backbones.py` & `lightning-flash-0.8.2/src/flash/template/classification/backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/template/classification/data.py` & `lightning-flash-0.8.2/src/flash/template/classification/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,16 +132,16 @@
         test_targets: Optional[Sequence[Any]] = None,
         predict_data: Optional[Collection[np.ndarray]] = None,
         input_cls: Type[Input] = TemplateNumpyClassificationInput,
         transform: INPUT_TRANSFORM_TYPE = TemplateInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TemplateData":
-        """This is our custom ``from_*`` method. It expects numpy ``Array`` objects and targets as input and
-        creates the ``TemplateData`` with them.
+        """This is our custom ``from_*`` method. It expects numpy ``Array`` objects and targets as input and creates the
+        ``TemplateData`` with them.
 
         Args:
             train_data: The numpy ``Array`` containing the train data.
             train_targets: The sequence of train targets.
             val_data: The numpy ``Array`` containing the validation data.
             val_targets: The sequence of validation targets.
             test_data: The numpy ``Array`` containing the test data.
@@ -153,15 +153,15 @@
             data_module_kwargs: Additional keyword arguments to provide to the
               :class:`~flash.core.data.data_module.DataModule` constructor.
 
         Returns:
             The constructed data module.
         """
 
-        ds_kw = dict()
+        ds_kw = {}
 
         train_input = input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw)
         target_formatter = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, val_targets, target_formatter=target_formatter, **ds_kw),
@@ -197,15 +197,15 @@
             transform_kwargs: Dict of keyword arguments to be provided when instantiating the transforms.
             data_module_kwargs: Additional keyword arguments to provide to the
               :class:`~flash.core.data.data_module.DataModule` constructor.
 
         Returns:
             The constructed data module.
         """
-        ds_kw = dict()
+        ds_kw = {}
 
         train_input = input_cls(RunningStage.TRAINING, train_bunch, **ds_kw)
         target_formatter = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_bunch, target_formatter=target_formatter, **ds_kw),
@@ -224,22 +224,21 @@
         n_fts_test = getattr(self.test_dataset, "num_features", None)
         return n_fts_train or n_fts_val or n_fts_test
 
     # OPTIONAL - Everything from this point onwards is an optional extra
 
     @staticmethod
     def configure_data_fetcher(*args, **kwargs) -> BaseDataFetcher:
-        """We can, *optionally*, provide a data visualization callback using the ``configure_data_fetcher``
-        method."""
+        """We can, *optionally*, provide a data visualization callback using the ``configure_data_fetcher`` method."""
         return TemplateVisualization(*args, **kwargs)
 
 
 class TemplateVisualization(BaseVisualization):
-    """The ``TemplateVisualization`` class is a :class:`~flash.core.data.callbacks.BaseVisualization` that just
-    prints the data.
+    """The ``TemplateVisualization`` class is a :class:`~flash.core.data.callbacks.BaseVisualization` that just prints
+    the data.
 
     If you want to provide a visualization with your task, you can override these hooks.
     """
 
     def show_load_sample(
         self,
         samples: List[Any],
```

### Comparing `lightning-flash-0.8.1.post0/flash/template/classification/model.py` & `lightning-flash-0.8.2/src/flash/template/classification/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from torch import nn, Tensor
+from torch import Tensor, nn
 
 from flash.core.classification import ClassificationTask
 from flash.core.data.io.input import DataKeys
 from flash.core.registry import FlashRegistry
 from flash.core.utilities.types import LOSS_FN_TYPE, LR_SCHEDULER_TYPE, METRICS_TYPE, OPTIMIZER_TYPE
 from flash.template.classification.backbones import TEMPLATE_BACKBONES
 
 
 class TemplateSKLearnClassifier(ClassificationTask):
-    """The ``TemplateSKLearnClassifier`` is a :class:`~flash.core.classification.ClassificationTask` that
-    classifies tabular data from scikit-learn.
+    """The ``TemplateSKLearnClassifier`` is a :class:`~flash.core.classification.ClassificationTask` that classifies
+    tabular data from scikit-learn.
 
     Args:
         num_features: The number of features (elements) in the input data.
         num_classes: The number of classes (outputs) for this :class:`~flash.core.model.Task`.
         backbone: The backbone name (or a tuple of ``nn.Module``, output size) to use.
         backbone_kwargs: Any additional kwargs to pass to the backbone constructor.
         loss_fn: The loss function to use. If ``None``, a default will be selected by the
@@ -102,16 +102,16 @@
         """For the test step, we just extract the :attr:`~flash.core.data.io.input.DataKeys.INPUT` and
         :attr:`~flash.core.data.io.input.DataKeys.TARGET` keys from the input and forward them to the
         :meth:`~flash.core.model.Task.test_step`."""
         batch = (batch[DataKeys.INPUT], batch[DataKeys.TARGET])
         return super().test_step(batch, batch_idx)
 
     def predict_step(self, batch: Any, batch_idx: int, dataloader_idx: int = 0) -> Any:
-        """For the predict step, we just extract the :attr:`~flash.core.data.io.input.DataKeys.INPUT` key from the
-        input and forward it to the :meth:`~flash.core.model.Task.predict_step`."""
+        """For the predict step, we just extract the :attr:`~flash.core.data.io.input.DataKeys.INPUT` key from the input
+        and forward it to the :meth:`~flash.core.model.Task.predict_step`."""
         batch = batch[DataKeys.INPUT]
         return super().predict_step(batch, batch_idx, dataloader_idx=dataloader_idx)
 
     def forward(self, x) -> Tensor:
         """First call the backbone, then the model head."""
         x = self.backbone(x)
         return self.head(x)
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/__init__.py` & `lightning-flash-0.8.2/src/flash/text/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/adapters.py` & `lightning-flash-0.8.2/src/flash/text/classification/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
     def predict_step(self, batch: Any, batch_idx: int, dataloader_idx: int = 0) -> Any:
         return self(batch)
 
 
 @dataclass
 class GenericCollate:
-
     tokenizer: Callable[[str], Any]
 
     @staticmethod
     def to_tensor(sample: Dict[str, Any]) -> Dict[str, Any]:
         tensor_sample = {}
         for key in sample:
             if key is DataKeys.METADATA:
@@ -102,19 +101,18 @@
         return tensor_sample
 
     def tokenize(self, sample):
         sample[DataKeys.INPUT] = self.tokenizer(sample[DataKeys.INPUT])
         return sample
 
     def __call__(self, samples):
-        return self.to_tensor(self.tokenize({key: [sample[key] for sample in samples] for key in samples[0].keys()}))
+        return self.to_tensor(self.tokenize({key: [sample[key] for sample in samples] for key in samples[0]}))
 
 
 class GenericAdapter(Adapter):
-
     heads: FlashRegistry = CLASSIFIER_HEADS
 
     def __init__(self, backbone, num_classes: int, max_length: int = 128, head="linear"):
         super().__init__()
 
         self.backbone, tokenizer, num_features = backbone()
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/backbones/clip.py` & `lightning-flash-0.8.2/src/flash/text/classification/backbones/clip.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/backbones/huggingface.py` & `lightning-flash-0.8.2/src/flash/text/classification/backbones/huggingface.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,13 @@
     model = AutoModelForSequenceClassification.from_pretrained(backbone, num_labels=num_classes)
     return model, backbone
 
 
 HUGGINGFACE_BACKBONES = FlashRegistry("backbones")
 
 if _TRANSFORMERS_AVAILABLE:
-
     HUGGINGFACE_BACKBONES = ExternalRegistry(
         getter=load_hugingface,
         name="backbones",
         providers=_HUGGINGFACE,
         adapter=HuggingFaceAdapter,
     )
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/cli.py` & `lightning-flash-0.8.2/src/flash/text/classification/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/collate.py` & `lightning-flash-0.8.2/src/flash/text/classification/collate.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from flash.core.data.io.input import DataKeys
 from flash.core.integrations.transformers.collate import TransformersCollate
 
 
 @dataclass(unsafe_hash=True)
 class TextClassificationCollate(TransformersCollate):
-
     max_length: int = 128
 
     def tokenize(self, sample):
         tokenized_sample = self.tokenizer(
             sample[DataKeys.INPUT], max_length=self.max_length, truncation=True, padding="max_length"
         )
         tokenized_sample = tokenized_sample.data
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/data.py` & `lightning-flash-0.8.2/src/flash/text/classification/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 from pandas.core.frame import DataFrame
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.utilities.classification import TargetFormatter
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.integrations.labelstudio.input import _parse_labelstudio_arguments, LabelStudioTextClassificationInput
-from flash.core.utilities.imports import _TEXT_AVAILABLE, _TEXT_TESTING
+from flash.core.integrations.labelstudio.input import LabelStudioTextClassificationInput, _parse_labelstudio_arguments
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.text.classification.input import (
     TextClassificationCSVInput,
     TextClassificationDataFrameInput,
     TextClassificationInput,
     TextClassificationJSONInput,
     TextClassificationListInput,
     TextClassificationParquetInput,
 )
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from datasets import Dataset
 else:
     Dataset = object
 
 # Skip doctests if requirements aren't available
-if not _TEXT_TESTING:
+if not _TOPIC_TEXT_AVAILABLE:
     __doctest_skip__ = ["TextClassificationData", "TextClassificationData.*"]
 
 
 class TextClassificationData(DataModule):
     """The ``TextClassificationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for text classification."""
 
@@ -207,19 +207,19 @@
             Predicting...
 
         .. testcleanup::
 
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            input_key=input_field,
-            target_keys=target_fields,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "input_key": input_field,
+            "target_keys": target_fields,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_file, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
@@ -329,20 +329,20 @@
             Predicting...
 
         .. testcleanup::
 
             >>> os.remove("train_data.json")
             >>> os.remove("predict_data.json")
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            input_key=input_field,
-            target_keys=target_fields,
-            field=field,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "input_key": input_field,
+            "target_keys": target_fields,
+            "field": field,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_file, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
@@ -364,16 +364,16 @@
         predict_file: Optional[PATH_TYPE] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = TextClassificationParquetInput,
         transform: Optional[Dict[str, Callable]] = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TextClassificationData":
-        """Load the :class:`~flash.text.classification.data.TextClassificationData` from PARQUET files containing
-        text snippets and their corresponding targets.
+        """Load the :class:`~flash.text.classification.data.TextClassificationData` from PARQUET files containing text
+        snippets and their corresponding targets.
 
         Input text snippets will be extracted from the ``input_field`` column in the PARQUET files.
         The targets will be extracted from the ``target_fields`` in the PARQUET files and can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
@@ -452,19 +452,19 @@
             Predicting...
 
         .. testcleanup::
 
             >>> os.remove("train_data.parquet")
             >>> os.remove("predict_data.parquet")
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            input_key=input_field,
-            target_keys=target_fields,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "input_key": input_field,
+            "target_keys": target_fields,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_file, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
@@ -555,19 +555,19 @@
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            input_key=input_field,
-            target_keys=target_fields,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "input_key": input_field,
+            "target_keys": target_fields,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_hf_dataset, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_hf_dataset, **ds_kw),
@@ -589,16 +589,16 @@
         predict_data_frame: Optional[DataFrame] = None,
         target_formatter: Optional[TargetFormatter] = None,
         input_cls: Type[Input] = TextClassificationDataFrameInput,
         transform: Optional[Dict[str, Callable]] = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TextClassificationData":
-        """Load the :class:`~flash.text.classification.data.TextClassificationData` from Pandas ``DataFrame``
-        objects containing text snippets and their corresponding targets.
+        """Load the :class:`~flash.text.classification.data.TextClassificationData` from Pandas ``DataFrame`` objects
+        containing text snippets and their corresponding targets.
 
         Input text snippets will be extracted from the ``input_field`` column in the ``DataFrame`` objects.
         The targets will be extracted from the ``target_fields`` in the ``DataFrame`` objects and can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
@@ -659,19 +659,19 @@
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-            input_key=input_field,
-            target_keys=target_fields,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+            "input_key": input_field,
+            "target_keys": target_fields,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data_frame, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data_frame, **ds_kw),
@@ -745,17 +745,17 @@
             >>> model = TextClassifier(num_classes=datamodule.num_classes, backbone="prajjwal1/bert-tiny")
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
-        ds_kw = dict(
-            target_formatter=target_formatter,
-        )
+        ds_kw = {
+            "target_formatter": target_formatter,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw)
         ds_kw["target_formatter"] = getattr(train_input, "target_formatter", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
@@ -782,19 +782,18 @@
         input_cls: Type[Input] = LabelStudioTextClassificationInput,
         transform: Optional[Dict[str, Callable]] = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         val_split: Optional[float] = None,
         multi_label: Optional[bool] = False,
         **data_module_kwargs: Any,
     ) -> "TextClassificationData":
-        """Creates a :class:`~flash.core.data.data_module.DataModule` object
-        from the given export file and data directory using the
-        :class:`~flash.core.data.io.input.Input` of name
-        :attr:`~flash.core.data.io.input.InputFormat.FOLDERS`
-        from the passed or constructed :class:`~flash.core.data.io.input_transform.InputTransform`.
+        """Creates a :class:`~flash.core.data.data_module.DataModule` object from the given export file and data
+        directory using the :class:`~flash.core.data.io.input.Input` of name
+        :attr:`~flash.core.data.io.input.InputFormat.FOLDERS` from the passed or constructed
+        :class:`~flash.core.data.io.input_transform.InputTransform`.
 
         Args:
             export_json: path to label studio export file
             train_export_json: path to label studio export file for train set, overrides export_json if specified
             val_export_json: path to label studio export file for validation
             test_export_json: path to label studio export file for test
             predict_export_json: path to label studio export file for predict
@@ -825,15 +824,15 @@
             val_data_folder=val_data_folder,
             test_data_folder=test_data_folder,
             predict_data_folder=predict_data_folder,
             val_split=val_split,
             multi_label=multi_label,
         )
 
-        ds_kw = dict()
+        ds_kw = {}
 
         train_input = input_cls(RunningStage.TRAINING, train_data, **ds_kw)
         ds_kw["parameters"] = getattr(train_input, "parameters", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, **ds_kw),
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/input.py` & `lightning-flash-0.8.2/src/flash/text/classification/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import pandas as pd
 
 from flash.core.data.io.classification_input import ClassificationInputMixin
 from flash.core.data.io.input import DataKeys, Input
 from flash.core.data.utilities.classification import MultiBinaryTargetFormatter, TargetFormatter
 from flash.core.data.utilities.loading import load_data_frame
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.utilities.imports import _TEXT_AVAILABLE, requires
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE, requires
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from datasets import Dataset, load_dataset
 else:
     Dataset = object
 
 
 class TextClassificationInput(Input, ClassificationInputMixin):
     @staticmethod
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/classification/model.py` & `lightning-flash-0.8.2/src/flash/text/classification/model.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/embedding/model.py` & `lightning-flash-0.8.2/src/flash/text/embedding/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 
 import torch
 from pytorch_lightning import Callback
 from torch import Tensor
 
 from flash.core.model import Task
 from flash.core.registry import FlashRegistry, print_provider_info
-from flash.core.utilities.imports import _TEXT_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE
 from flash.core.utilities.providers import _SENTENCE_TRANSFORMERS
 from flash.text.classification.collate import TextClassificationCollate
 from flash.text.embedding.backbones import HUGGINGFACE_BACKBONES
 from flash.text.ort_callback import ORTCallback
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from sentence_transformers.models import Pooling
 
     Pooling = print_provider_info("Pooling", _SENTENCE_TRANSFORMERS, Pooling)
 
 logger = logging.getLogger(__name__)
 
 
 class TextEmbedder(Task):
-    """The ``TextEmbedder`` is a :class:`~flash.Task` for generating sentence embeddings, training and validation.
-    For more details, see `embeddings`.
+    """The ``TextEmbedder`` is a :class:`~flash.Task` for generating sentence embeddings, training and validation. For
+    more details, see `embeddings`.
 
     You can change the backbone to any question answering model from `UKPLab/sentence-transformers
     <https://github.com/UKPLab/sentence-transformers>`_ using the ``backbone``
     argument.
 
     Args:
         backbone: backbone model to use for the task.
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/ort_callback.py` & `lightning-flash-0.8.2/src/flash/text/ort_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/question_answering/cli.py` & `lightning-flash-0.8.2/src/flash/text/question_answering/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/question_answering/collate.py` & `lightning-flash-0.8.2/src/flash/text/question_answering/collate.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/question_answering/data.py` & `lightning-flash-0.8.2/src/flash/text/question_answering/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 from typing import Any, Dict, Optional, Type
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.utilities.imports import _TEXT_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.text.question_answering.input import (
     QuestionAnsweringCSVInput,
     QuestionAnsweringDictionaryInput,
     QuestionAnsweringJSONInput,
     QuestionAnsweringSQuADInput,
 )
 
 # Skip doctests if requirements aren't available
-if not _TEXT_AVAILABLE:
+if not _TOPIC_TEXT_AVAILABLE:
     __doctest_skip__ = ["QuestionAnsweringData", "QuestionAnsweringData.*"]
 
 
 class QuestionAnsweringData(DataModule):
     """The ``QuestionAnsweringData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for extractive question answering."""
 
@@ -205,19 +205,19 @@
 
         .. testcleanup::
 
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
 
-        ds_kw = dict(
-            question_column_name=question_column_name,
-            context_column_name=context_column_name,
-            answer_column_name=answer_column_name,
-        )
+        ds_kw = {
+            "question_column_name": question_column_name,
+            "context_column_name": context_column_name,
+            "answer_column_name": answer_column_name,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -349,20 +349,20 @@
 
         .. testcleanup::
 
             >>> os.remove("train_data.json")
             >>> os.remove("predict_data.json")
         """
 
-        ds_kw = dict(
-            field=field,
-            question_column_name=question_column_name,
-            context_column_name=context_column_name,
-            answer_column_name=answer_column_name,
-        )
+        ds_kw = {
+            "field": field,
+            "question_column_name": question_column_name,
+            "context_column_name": context_column_name,
+            "answer_column_name": answer_column_name,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -631,19 +631,19 @@
         .. testcleanup::
 
             >>> import os
             >>> os.remove("train_data.json")
             >>> os.remove("predict_data.json")
         """
 
-        ds_kw = dict(
-            question_column_name=question_column_name,
-            context_column_name=context_column_name,
-            answer_column_name=answer_column_name,
-        )
+        ds_kw = {
+            "question_column_name": question_column_name,
+            "context_column_name": context_column_name,
+            "answer_column_name": answer_column_name,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -662,16 +662,16 @@
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         question_column_name: str = "question",
         context_column_name: str = "context",
         answer_column_name: str = "answer",
         **data_module_kwargs: Any,
     ) -> "QuestionAnsweringData":
-        """Load the :class:`~flash.text.question_answering.data.QuestionAnsweringData` from Python dictionary
-        objects containing questions, contexts and their corresponding answers.
+        """Load the :class:`~flash.text.question_answering.data.QuestionAnsweringData` from Python dictionary objects
+        containing questions, contexts and their corresponding answers.
 
         Question snippets will be extracted from the ``question_column_name`` field in the dictionaries.
         Context snippets will be extracted from the ``context_column_name`` field in the dictionaries.
         Answer snippets will be extracted from the ``answer_column_name`` field in the dictionaries.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
@@ -744,19 +744,19 @@
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
 
-        ds_kw = dict(
-            question_column_name=question_column_name,
-            context_column_name=context_column_name,
-            answer_column_name=answer_column_name,
-        )
+        ds_kw = {
+            "question_column_name": question_column_name,
+            "context_column_name": context_column_name,
+            "answer_column_name": answer_column_name,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_data, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_data, **ds_kw),
             input_cls(RunningStage.TESTING, test_data, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_data, **ds_kw),
             transform=transform,
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/question_answering/input.py` & `lightning-flash-0.8.2/src/flash/text/question_answering/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from pathlib import Path
 from typing import Any, Dict
 
 import flash
 from flash.core.data.io.input import Input
 from flash.core.data.utilities.loading import load_data_frame
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.utilities.imports import _TEXT_AVAILABLE, requires
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE, requires
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from datasets import Dataset, load_dataset
 else:
     Dataset = object
 
 
 class QuestionAnsweringInputBase(Input):
     def _reshape_answer_column(self, sample: Any):
@@ -49,23 +49,22 @@
         question_column_name: str = "question",
         context_column_name: str = "context",
         answer_column_name: str = "answer",
     ) -> Dataset:
         column_names = hf_dataset.column_names
 
         if self.training or self.validating or self.testing:
-            if answer_column_name == "answer":
-                if "answer" not in column_names:
-                    if "answer_text" in column_names and "answer_start" in column_names:
-                        hf_dataset = hf_dataset.map(self._reshape_answer_column, batched=False)
-                    else:
-                        raise KeyError(
-                            """Dataset must contain either \"answer\" key as dict type or "answer_text" and
+            if answer_column_name == "answer" and "answer" not in column_names:
+                if "answer_text" in column_names and "answer_start" in column_names:
+                    hf_dataset = hf_dataset.map(self._reshape_answer_column, batched=False)
+                else:
+                    raise KeyError(
+                        """Dataset must contain either \"answer\" key as dict type or "answer_text" and
                             "answer_start" as string and integer types."""
-                        )
+                    )
             if not isinstance(hf_dataset[answer_column_name][0], Dict):
                 raise TypeError(
                     f'{answer_column_name} column should be of type dict with keys "text" and "answer_start"'
                 )
 
             if answer_column_name in column_names and answer_column_name != "answer":
                 hf_dataset = hf_dataset.rename_column(answer_column_name, "answer")
@@ -74,15 +73,15 @@
             hf_dataset = hf_dataset.rename_column(question_column_name, "question")
 
         if context_column_name in column_names and context_column_name != "context":
             hf_dataset = hf_dataset.rename_column(context_column_name, "context")
 
         if flash._IS_TESTING:
             # NOTE: must subset in this way to return a Dataset
-            hf_dataset = [sample for sample in hf_dataset][:40]
+            hf_dataset = list(hf_dataset)[:40]
 
         return hf_dataset
 
 
 class QuestionAnsweringCSVInput(QuestionAnsweringInputBase):
     @requires("text")
     def load_data(
@@ -162,15 +161,15 @@
                     titles.append(title)
                     contexts.append(context)
                     questions.append(question)
 
                     if not self.predicting:
                         _answer_starts = [answer["answer_start"] for answer in qa["answers"]]
                         _answers = [answer["text"] for answer in qa["answers"]]
-                        answers.append(dict(text=_answers, answer_start=_answer_starts))
+                        answers.append({"text": _answers, "answer_start": _answer_starts})
 
         data = {"id": ids, "title": titles, "context": contexts, "question": questions}
         if not self.predicting:
             data["answer"] = answers
 
         return super().load_data(
             data,
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/question_answering/model.py` & `lightning-flash-0.8.2/src/flash/text/question_answering/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,38 +28,38 @@
 from torch import Tensor
 from torch.nn import Module
 from torchmetrics.text.rouge import ROUGEScore
 
 from flash.core.data.io.input import DataKeys
 from flash.core.model import Task
 from flash.core.registry import ExternalRegistry, FlashRegistry
-from flash.core.utilities.imports import _TEXT_AVAILABLE, _TM_GREATER_EQUAL_0_7_0
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE
 from flash.core.utilities.providers import _HUGGINGFACE
 from flash.core.utilities.types import LR_SCHEDULER_TYPE, METRICS_TYPE, OPTIMIZER_TYPE
 from flash.text.ort_callback import ORTCallback
 from flash.text.question_answering.collate import TextQuestionAnsweringCollate
 from flash.text.question_answering.output_transform import QuestionAnsweringOutputTransform
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from transformers import AutoModelForQuestionAnswering
 
     HUGGINGFACE_BACKBONES = ExternalRegistry(
         AutoModelForQuestionAnswering.from_pretrained,
         "backbones",
         _HUGGINGFACE,
     )
 else:
     AutoModelForQuestionAnswering = None
 
     HUGGINGFACE_BACKBONES = FlashRegistry("backbones")
 
 
 class QuestionAnsweringTask(Task):
-    """The ``QuestionAnsweringTask`` is a :class:`~flash.Task` for extractive question answering. For more details,
-    see `question_answering`.
+    """The ``QuestionAnsweringTask`` is a :class:`~flash.Task` for extractive question answering. For more details, see
+    `question_answering`.
 
     You can change the backbone to any question answering model from `HuggingFace/transformers
     <https://huggingface.co/transformers/model_doc/auto.html#automodelforquestionanswering>`_ using the ``backbone``
     argument.
 
     .. note:: When changing the backbone, make sure you pass in the same backbone to the :class:`~flash.Task` and the
         :class:`~flash.core.data.data_module.DataModule` object! Since this is a QuestionAnswering task, make sure you
@@ -140,26 +140,17 @@
         self.enable_ort = enable_ort
         self.n_best_size = n_best_size
         self.version_2_with_negative = version_2_with_negative
         self.max_target_length = max_target_length
         self.null_score_diff_threshold = null_score_diff_threshold
         self._initialize_model_specific_parameters()
 
-        if _TM_GREATER_EQUAL_0_7_0:
-            self.rouge = ROUGEScore(
-                use_stemmer=use_stemmer,
-            )
-        else:
-            self.rouge = ROUGEScore(
-                True,
-                use_stemmer=use_stemmer,
-            )
+        self.rouge = ROUGEScore(use_stemmer=use_stemmer)
 
     def _generate_answers(self, pred_start_logits, pred_end_logits, examples):
-
         all_predictions = collections.OrderedDict()
         if self.version_2_with_negative:
             scores_diff_json = collections.OrderedDict()
 
         for example_index, example in enumerate(examples):
             min_null_prediction = None
             prelim_predictions = []
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/question_answering/output_transform.py` & `lightning-flash-0.8.2/src/flash/text/question_answering/output_transform.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/core/collate.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/core/collate.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/core/input.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/core/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 from typing import List, Optional
 
 import flash
 from flash.core.data.io.input import DataKeys, Input
 from flash.core.data.utilities.loading import load_data_frame
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.utilities.imports import _TEXT_AVAILABLE, requires
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE, requires
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from datasets import Dataset, load_dataset
 else:
     Dataset = object
 
 
 class Seq2SeqInputBase(Input):
     @requires("text")
@@ -41,15 +41,15 @@
             hf_dataset = hf_dataset.rename_column(input_key, DataKeys.INPUT)
 
         if target_key in hf_dataset.column_names and target_key != DataKeys.TARGET:
             hf_dataset = hf_dataset.rename_column(target_key, DataKeys.TARGET)
 
         if flash._IS_TESTING:
             # NOTE: must subset in this way to return a Dataset
-            hf_dataset = [sample for sample in hf_dataset][:40]
+            hf_dataset = list(hf_dataset)[:40]
 
         return hf_dataset
 
 
 class Seq2SeqCSVInput(Seq2SeqInputBase):
     @requires("text")
     def load_data(
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/core/model.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 from flash.core.data.io.input import DataKeys, ServeInput
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.io.output import Output
 from flash.core.data.io.output_transform import OutputTransform
 from flash.core.model import Task
 from flash.core.registry import ExternalRegistry, FlashRegistry
 from flash.core.serve import Composition
-from flash.core.utilities.imports import _TEXT_AVAILABLE, requires
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE, requires
 from flash.core.utilities.providers import _HUGGINGFACE
 from flash.core.utilities.types import (
     INPUT_TRANSFORM_TYPE,
     LOSS_FN_TYPE,
     LR_SCHEDULER_TYPE,
     METRICS_TYPE,
     OPTIMIZER_TYPE,
 )
 from flash.text.input import TextDeserializer
 from flash.text.ort_callback import ORTCallback
 from flash.text.seq2seq.core.collate import TextSeq2SeqCollate
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from transformers import AutoModelForSeq2SeqLM
 
     HUGGINGFACE_BACKBONES = ExternalRegistry(
         AutoModelForSeq2SeqLM.from_pretrained,
         "backbones",
         _HUGGINGFACE,
     )
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/summarization/cli.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/summarization/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/summarization/data.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/summarization/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,44 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import os
 from typing import Any, Dict, List, Optional, Type
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.utilities.imports import _TEXT_AVAILABLE, _TEXT_TESTING
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.text.seq2seq.core.input import Seq2SeqCSVInput, Seq2SeqInputBase, Seq2SeqJSONInput, Seq2SeqListInput
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from datasets import Dataset
 else:
     Dataset = object
 
+__doctest_skip__ = []
 # Skip doctests if requirements aren't available
-if not _TEXT_TESTING:
-    __doctest_skip__ = ["SummarizationData", "SummarizationData.*"]
+if not _TOPIC_TEXT_AVAILABLE:
+    __doctest_skip__ += ["SummarizationData", "SummarizationData.*"]
+
+# some strange crash for out of memory with pt 1.11
+if os.name == "nt":
+    __doctest_skip__ += ["SummarizationData.from_lists", "SummarizationData.from_json"]
 
 
 class SummarizationData(DataModule):
-    """The ``SummarizationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
-    classmethods for loading data for text summarization."""
+    """The ``SummarizationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of classmethods
+    for loading data for text summarization."""
 
     input_transform_cls = InputTransform
 
     @classmethod
     def from_csv(
         cls,
         input_field: str,
@@ -48,16 +54,16 @@
         test_file: Optional[PATH_TYPE] = None,
         predict_file: Optional[PATH_TYPE] = None,
         input_cls: Type[Input] = Seq2SeqCSVInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "SummarizationData":
-        """Load the :class:`~flash.text.seq2seq.summarization.data.SummarizationData` from CSV files containing
-        input text snippets and their corresponding target text snippets.
+        """Load the :class:`~flash.text.seq2seq.summarization.data.SummarizationData` from CSV files containing input
+        text snippets and their corresponding target text snippets.
 
         Input text snippets will be extracted from the ``input_field`` column in the CSV files.
         Target text snippets will be extracted from the ``target_field`` column in the CSV files.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -116,15 +122,15 @@
             >>> datamodule = SummarizationData.from_csv(
             ...     "texts",
             ...     "summaries",
             ...     train_file="train_data.csv",
             ...     predict_file="predict_data.csv",
             ...     batch_size=2,
             ... )
-            >>> model = SummarizationTask()
+            >>> model = SummarizationTask(backbone="JulesBelveze/t5-small-headline-generator")
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
 
         .. testcleanup::
@@ -169,31 +175,31 @@
             >>> datamodule = SummarizationData.from_csv(
             ...     "texts",
             ...     "summaries",
             ...     train_file="train_data.tsv",
             ...     predict_file="predict_data.tsv",
             ...     batch_size=2,
             ... )
-            >>> model = SummarizationTask()
+            >>> model = SummarizationTask(backbone="JulesBelveze/t5-small-headline-generator")
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
 
         .. testcleanup::
 
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
 
-        ds_kw = dict(
-            input_key=input_field,
-            target_key=target_field,
-        )
+        ds_kw = {
+            "input_key": input_field,
+            "target_key": target_field,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -212,16 +218,16 @@
         predict_file: Optional[PATH_TYPE] = None,
         input_cls: Type[Input] = Seq2SeqJSONInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         field: Optional[str] = None,
         **data_module_kwargs: Any,
     ) -> "SummarizationData":
-        """Load the :class:`~flash.text.seq2seq.summarization.data.SummarizationData` from JSON files containing
-        input text snippets and their corresponding target text snippets.
+        """Load the :class:`~flash.text.seq2seq.summarization.data.SummarizationData` from JSON files containing input
+        text snippets and their corresponding target text snippets.
 
         Input text snippets will be extracted from the ``input_field`` column in the JSON files.
         Target text snippets will be extracted from the ``target_field`` column in the JSON files.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -278,32 +284,32 @@
             ...     "texts",
             ...     "summaries",
             ...     train_file="train_data.json",
             ...     predict_file="predict_data.json",
             ...     batch_size=2,
             ... )  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Downloading...
-            >>> model = SummarizationTask()
+            >>> model = SummarizationTask(backbone="JulesBelveze/t5-small-headline-generator")
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
 
         .. testcleanup::
 
             >>> os.remove("train_data.json")
             >>> os.remove("predict_data.json")
         """
 
-        ds_kw = dict(
-            input_key=input_field,
-            target_key=target_field,
-            field=field,
-        )
+        ds_kw = {
+            "input_key": input_field,
+            "target_key": target_field,
+            "field": field,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -371,31 +377,31 @@
             >>> datamodule = SummarizationData.from_hf_datasets(
             ...     "texts",
             ...     "summaries",
             ...     train_hf_dataset=train_data,
             ...     predict_hf_dataset=predict_data,
             ...     batch_size=2,
             ... )  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-            >>> model = SummarizationTask()
+            >>> model = SummarizationTask(backbone="JulesBelveze/t5-small-headline-generator")
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
 
-        ds_kw = dict(
-            input_key=input_field,
-            target_key=target_field,
-        )
+        ds_kw = {
+            "input_key": input_field,
+            "target_key": target_field,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_hf_dataset, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_hf_dataset, **ds_kw),
             input_cls(RunningStage.TESTING, test_hf_dataset, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_hf_dataset, **ds_kw),
             transform=transform,
@@ -414,16 +420,16 @@
         test_targets: Optional[List[str]] = None,
         predict_data: Optional[List[str]] = None,
         input_cls: Type[Input] = Seq2SeqListInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "SummarizationData":
-        """Load the :class:`~flash.text.seq2seq.summarization.data.SummarizationData` from lists of input text
-        snippets and corresponding lists of target text snippets.
+        """Load the :class:`~flash.text.seq2seq.summarization.data.SummarizationData` from lists of input text snippets
+        and corresponding lists of target text snippets.
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
             train_data: The list of input text snippets to use when training.
             train_targets: The list of target text snippets to use when training.
@@ -450,23 +456,23 @@
             >>> from flash.text import SummarizationTask, SummarizationData
             >>> datamodule = SummarizationData.from_lists(
             ...     train_data=["A long paragraph", "A news article"],
             ...     train_targets=["A short paragraph", "A news headline"],
             ...     predict_data=["A movie review", "A book chapter"],
             ...     batch_size=2,
             ... )  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-            >>> model = SummarizationTask()
+            >>> model = SummarizationTask(backbone="JulesBelveze/t5-small-headline-generator")
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
             input_cls(RunningStage.TESTING, test_data, test_targets, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_data, **ds_kw),
             transform=transform,
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/summarization/model.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/summarization/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Union
 
 from torch import Tensor
 from torchmetrics.text.rouge import ROUGEScore
 
-from flash.core.utilities.imports import _TM_GREATER_EQUAL_0_7_0
 from flash.core.utilities.types import LOSS_FN_TYPE, LR_SCHEDULER_TYPE, METRICS_TYPE, OPTIMIZER_TYPE
 from flash.text.seq2seq.core.model import Seq2SeqTask
 
 
 class SummarizationTask(Seq2SeqTask):
     """The ``SummarizationTask`` is a :class:`~flash.Task` for Seq2Seq text summarization. For more details, see
     :ref:`summarization`.
@@ -72,23 +71,15 @@
             optimizer=optimizer,
             lr_scheduler=lr_scheduler,
             metrics=metrics,
             learning_rate=learning_rate,
             num_beams=num_beams,
             enable_ort=enable_ort,
         )
-        if _TM_GREATER_EQUAL_0_7_0:
-            self.rouge = ROUGEScore(
-                use_stemmer=use_stemmer,
-            )
-        else:
-            self.rouge = ROUGEScore(
-                True,
-                use_stemmer=use_stemmer,
-            )
+        self.rouge = ROUGEScore(use_stemmer=use_stemmer)
 
     @property
     def task(self) -> str:
         return "summarization"
 
     def compute_metrics(self, generated_tokens: Tensor, batch: Dict, prefix: str) -> None:
         tgt_lns = self.decode(batch["labels"])
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/translation/cli.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/translation/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/translation/data.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/translation/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,36 +9,38 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Type
 
+import torch
+
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import InputTransform
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.utilities.imports import _TEXT_AVAILABLE, _TEXT_TESTING
+from flash.core.utilities.imports import _TOPIC_TEXT_AVAILABLE
 from flash.core.utilities.stages import RunningStage
 from flash.core.utilities.types import INPUT_TRANSFORM_TYPE
 from flash.text.seq2seq.core.input import Seq2SeqCSVInput, Seq2SeqInputBase, Seq2SeqJSONInput, Seq2SeqListInput
 
-if _TEXT_AVAILABLE:
+if _TOPIC_TEXT_AVAILABLE:
     from datasets import Dataset
 else:
     Dataset = object
 
 # Skip doctests if requirements aren't available
-if not _TEXT_TESTING:
+if not _TOPIC_TEXT_AVAILABLE or not torch.cuda.is_available():
     __doctest_skip__ = ["TranslationData", "TranslationData.*"]
 
 
 class TranslationData(DataModule):
-    """The ``TranslationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
-    classmethods for loading data for text translation."""
+    """The ``TranslationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of classmethods
+    for loading data for text translation."""
 
     input_transform_cls = InputTransform
 
     @classmethod
     def from_csv(
         cls,
         input_field: str,
@@ -48,16 +50,16 @@
         test_file: Optional[PATH_TYPE] = None,
         predict_file: Optional[PATH_TYPE] = None,
         input_cls: Type[Input] = Seq2SeqCSVInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TranslationData":
-        """Load the :class:`~flash.text.seq2seq.translation.data.TranslationData` from CSV files containing input
-        text snippets and their corresponding target text snippets.
+        """Load the :class:`~flash.text.seq2seq.translation.data.TranslationData` from CSV files containing input text
+        snippets and their corresponding target text snippets.
 
         Input text snippets will be extracted from the ``input_field`` column in the CSV files.
         Target text snippets will be extracted from the ``target_field`` column in the CSV files.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -180,18 +182,18 @@
 
         .. testcleanup::
 
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
 
-        ds_kw = dict(
-            input_key=input_field,
-            target_key=target_field,
-        )
+        ds_kw = {
+            "input_key": input_field,
+            "target_key": target_field,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -210,16 +212,16 @@
         predict_file: Optional[PATH_TYPE] = None,
         input_cls: Type[Input] = Seq2SeqJSONInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         field: Optional[str] = None,
         **data_module_kwargs: Any,
     ) -> "TranslationData":
-        """Load the :class:`~flash.text.seq2seq.translation.data.TranslationData` from JSON files containing input
-        text snippets and their corresponding target text snippets.
+        """Load the :class:`~flash.text.seq2seq.translation.data.TranslationData` from JSON files containing input text
+        snippets and their corresponding target text snippets.
 
         Input text snippets will be extracted from the ``input_field`` column in the JSON files.
         Target text snippets will be extracted from the ``target_field`` column in the JSON files.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -288,19 +290,19 @@
 
         .. testcleanup::
 
             >>> os.remove("train_data.json")
             >>> os.remove("predict_data.json")
         """
 
-        ds_kw = dict(
-            input_key=input_field,
-            target_key=target_field,
-            field=field,
-        )
+        ds_kw = {
+            "input_key": input_field,
+            "target_key": target_field,
+            "field": field,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_file, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_file, **ds_kw),
             input_cls(RunningStage.TESTING, test_file, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_file, **ds_kw),
             transform=transform,
@@ -318,16 +320,16 @@
         test_hf_dataset: Optional[Dataset] = None,
         predict_hf_dataset: Optional[Dataset] = None,
         input_cls: Type[Input] = Seq2SeqInputBase,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TranslationData":
-        """Load the :class:`~flash.text.seq2seq.translation.data.TranslationData` from Hugging Face ``Dataset``
-        objects containing input text snippets and their corresponding target text snippets.
+        """Load the :class:`~flash.text.seq2seq.translation.data.TranslationData` from Hugging Face ``Dataset`` objects
+        containing input text snippets and their corresponding target text snippets.
 
         Input text snippets will be extracted from the ``input_field`` column in the ``Dataset`` objects.
         Target text snippets will be extracted from the ``target_field`` column in the ``Dataset`` objects.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
@@ -381,18 +383,18 @@
 
         .. testcleanup::
 
             >>> del train_data
             >>> del predict_data
         """
 
-        ds_kw = dict(
-            input_key=input_field,
-            target_key=target_field,
-        )
+        ds_kw = {
+            "input_key": input_field,
+            "target_key": target_field,
+        }
 
         return cls(
             input_cls(RunningStage.TRAINING, train_hf_dataset, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_hf_dataset, **ds_kw),
             input_cls(RunningStage.TESTING, test_hf_dataset, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_hf_dataset, **ds_kw),
             transform=transform,
@@ -411,16 +413,16 @@
         test_targets: Optional[List[str]] = None,
         predict_data: Optional[List[str]] = None,
         input_cls: Type[Input] = Seq2SeqListInput,
         transform: INPUT_TRANSFORM_TYPE = InputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "TranslationData":
-        """Load the :class:`~flash.text.seq2seq.translation.data.TranslationData` from lists of input text snippets
-        and corresponding lists of target text snippets.
+        """Load the :class:`~flash.text.seq2seq.translation.data.TranslationData` from lists of input text snippets and
+        corresponding lists of target text snippets.
 
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
         Args:
             train_data: The list of input text snippets to use when training.
             train_targets: The list of target text snippets to use when training.
@@ -455,15 +457,15 @@
             >>> trainer = Trainer(fast_dev_run=True)
             >>> trainer.fit(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Training...
             >>> trainer.predict(model, datamodule=datamodule)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             Predicting...
         """
 
-        ds_kw = dict()
+        ds_kw = {}
 
         return cls(
             input_cls(RunningStage.TRAINING, train_data, train_targets, **ds_kw),
             input_cls(RunningStage.VALIDATING, val_data, val_targets, **ds_kw),
             input_cls(RunningStage.TESTING, test_data, test_targets, **ds_kw),
             input_cls(RunningStage.PREDICTING, predict_data, **ds_kw),
             transform=transform,
```

### Comparing `lightning-flash-0.8.1.post0/flash/text/seq2seq/translation/model.py` & `lightning-flash-0.8.2/src/flash/text/seq2seq/translation/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, Optional, Union
 
 from torchmetrics import BLEUScore
 
-from flash.core.utilities.imports import _TM_GREATER_EQUAL_0_7_0
 from flash.core.utilities.types import LOSS_FN_TYPE, LR_SCHEDULER_TYPE, METRICS_TYPE, OPTIMIZER_TYPE
 from flash.text.seq2seq.core.model import Seq2SeqTask
 
 
 class TranslationTask(Seq2SeqTask):
     """The ``TranslationTask`` is a :class:`~flash.Task` for Seq2Seq text translation. For more details, see
     :ref:`translation`.
@@ -88,14 +87,11 @@
 
     def compute_metrics(self, generated_tokens, batch, prefix):
         reference_corpus = self.decode(batch["labels"])
         # wrap targets in list as score expects a list of potential references
         reference_corpus = [[reference] for reference in reference_corpus]
 
         translate_corpus = self.decode(generated_tokens)
-        translate_corpus = [line for line in translate_corpus]
+        translate_corpus = list(translate_corpus)
 
-        if _TM_GREATER_EQUAL_0_7_0:
-            result = self.bleu(translate_corpus, reference_corpus)
-        else:
-            result = self.bleu(reference_corpus, translate_corpus)
+        result = self.bleu(translate_corpus, reference_corpus)
         self.log(f"{prefix}_bleu_score", result, on_step=False, on_epoch=True, prog_bar=True)
```

### Comparing `lightning-flash-0.8.1.post0/flash/video/classification/cli.py` & `lightning-flash-0.8.2/src/flash/video/classification/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/video/classification/data.py` & `lightning-flash-0.8.2/src/flash/video/classification/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,16 @@
 from torch.utils.data import Sampler
 
 from flash.core.data.data_module import DataModule
 from flash.core.data.io.input import Input
 from flash.core.data.io.input_transform import INPUT_TRANSFORM_TYPE
 from flash.core.data.utilities.classification import TargetFormatter
 from flash.core.data.utilities.paths import PATH_TYPE
-from flash.core.integrations.labelstudio.input import _parse_labelstudio_arguments, LabelStudioVideoClassificationInput
-from flash.core.utilities.imports import (
-    _FIFTYONE_AVAILABLE,
-    _PYTORCHVIDEO_AVAILABLE,
-    _VIDEO_EXTRAS_TESTING,
-    _VIDEO_TESTING,
-    requires,
-)
+from flash.core.integrations.labelstudio.input import LabelStudioVideoClassificationInput, _parse_labelstudio_arguments
+from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, _PYTORCHVIDEO_AVAILABLE, _TOPIC_VIDEO_AVAILABLE, requires
 from flash.core.utilities.stages import RunningStage
 from flash.video.classification.input import (
     VideoClassificationCSVInput,
     VideoClassificationCSVPredictInput,
     VideoClassificationDataFrameInput,
     VideoClassificationDataFramePredictInput,
     VideoClassificationFiftyOneInput,
@@ -42,36 +36,26 @@
     VideoClassificationFoldersInput,
     VideoClassificationPathsPredictInput,
     VideoClassificationTensorsInput,
     VideoClassificationTensorsPredictInput,
 )
 from flash.video.classification.input_transform import VideoClassificationInputTransform
 
-if _FIFTYONE_AVAILABLE:
-    SampleCollection = "fiftyone.core.collections.SampleCollection"
-else:
-    SampleCollection = None
+SampleCollection = "fiftyone.core.collections.SampleCollection" if _FIFTYONE_AVAILABLE else None
 
 if _PYTORCHVIDEO_AVAILABLE:
     from pytorchvideo.data.clip_sampling import ClipSampler
 else:
     ClipSampler = None
 
 # Skip doctests if requirements aren't available
 __doctest_skip__ = []
-if not _VIDEO_TESTING:
-    __doctest_skip__ += [
-        "VideoClassificationData",
-        "VideoClassificationData.from_files",
-        "VideoClassificationData.from_folders",
-        "VideoClassificationData.from_data_frame",
-        "VideoClassificationData.from_csv",
-        "VideoClassificationData.from_tensors",
-    ]
-if not _VIDEO_EXTRAS_TESTING:
+if not _TOPIC_VIDEO_AVAILABLE:
+    __doctest_skip__ += ["VideoClassificationData", "VideoClassificationData.*"]
+if not _FIFTYONE_AVAILABLE:
     __doctest_skip__ += ["VideoClassificationData.from_fiftyone"]
 
 
 class VideoClassificationData(DataModule):
     """The ``VideoClassificationData`` class is a :class:`~flash.core.data.data_module.DataModule` with a set of
     classmethods for loading data for video classification."""
 
@@ -172,21 +156,21 @@
 
         .. testcleanup::
 
             >>> import os
             >>> _ = [os.remove(f"video_{i}.mp4") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_video_{i}.mp4") for i in range(1, 4)]
         """
-        ds_kw = dict(
-            clip_sampler=clip_sampler,
-            clip_duration=clip_duration,
-            clip_sampler_kwargs=clip_sampler_kwargs,
-            decode_audio=decode_audio,
-            decoder=decoder,
-        )
+        ds_kw = {
+            "clip_sampler": clip_sampler,
+            "clip_duration": clip_duration,
+            "clip_sampler_kwargs": clip_sampler_kwargs,
+            "decode_audio": decode_audio,
+            "decoder": decoder,
+        }
 
         train_input = input_cls(
             RunningStage.TRAINING,
             train_files,
             train_targets,
             video_sampler=video_sampler,
             target_formatter=target_formatter,
@@ -234,16 +218,15 @@
         decoder: str = "pyav",
         input_cls: Type[Input] = VideoClassificationFoldersInput,
         predict_input_cls: Type[Input] = VideoClassificationPathsPredictInput,
         transform: INPUT_TRANSFORM_TYPE = VideoClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs,
     ) -> "VideoClassificationData":
-        """Load the :class:`~flash.video.classification.data.VideoClassificationData` from folders containing
-        videos.
+        """Load the :class:`~flash.video.classification.data.VideoClassificationData` from folders containing videos.
 
         The supported file extensions are: ``.mp4``, and ``.avi``.
         For train, test, and validation data, the folders are expected to contain a sub-folder for each class.
         Here's the required structure:
 
         .. code-block::
 
@@ -338,21 +321,21 @@
 
         .. testcleanup::
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
         """
-        ds_kw = dict(
-            clip_sampler=clip_sampler,
-            clip_duration=clip_duration,
-            clip_sampler_kwargs=clip_sampler_kwargs,
-            decode_audio=decode_audio,
-            decoder=decoder,
-        )
+        ds_kw = {
+            "clip_sampler": clip_sampler,
+            "clip_duration": clip_duration,
+            "clip_sampler_kwargs": clip_sampler_kwargs,
+            "decode_audio": decode_audio,
+            "decoder": decoder,
+        }
 
         train_input = input_cls(
             RunningStage.TRAINING,
             train_folder,
             video_sampler=video_sampler,
             target_formatter=target_formatter,
             **ds_kw,
@@ -521,21 +504,21 @@
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> del train_data_frame
             >>> del predict_data_frame
         """
-        ds_kw = dict(
-            clip_sampler=clip_sampler,
-            clip_duration=clip_duration,
-            clip_sampler_kwargs=clip_sampler_kwargs,
-            decode_audio=decode_audio,
-            decoder=decoder,
-        )
+        ds_kw = {
+            "clip_sampler": clip_sampler,
+            "clip_duration": clip_duration,
+            "clip_sampler_kwargs": clip_sampler_kwargs,
+            "decode_audio": decode_audio,
+            "decoder": decoder,
+        }
 
         train_data = (train_data_frame, input_field, target_fields, train_videos_root, train_resolver)
         val_data = (val_data_frame, input_field, target_fields, val_videos_root, val_resolver)
         test_data = (test_data_frame, input_field, target_fields, test_videos_root, test_resolver)
         predict_data = (predict_data_frame, input_field, predict_videos_root, predict_resolver)
 
         train_input = input_cls(
@@ -711,16 +694,16 @@
         decoder: str = "pyav",
         input_cls: Type[Input] = VideoClassificationCSVInput,
         predict_input_cls: Type[Input] = VideoClassificationCSVPredictInput,
         transform: INPUT_TRANSFORM_TYPE = VideoClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs: Any,
     ) -> "VideoClassificationData":
-        """Load the :class:`~flash.video.classification.data.VideoClassificationData` from CSV files containing
-        video file paths and their corresponding targets.
+        """Load the :class:`~flash.video.classification.data.VideoClassificationData` from CSV files containing video
+        file paths and their corresponding targets.
 
         Input video file paths will be extracted from the ``input_field`` column in the CSV files.
         The supported file extensions are: ``.mp4``, and ``.avi``.
         The targets will be extracted from the ``target_fields`` in the CSV files and can be in any of our
         :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
@@ -919,21 +902,21 @@
 
             >>> import shutil
             >>> shutil.rmtree("train_folder")
             >>> shutil.rmtree("predict_folder")
             >>> os.remove("train_data.tsv")
             >>> os.remove("predict_data.tsv")
         """
-        ds_kw = dict(
-            clip_sampler=clip_sampler,
-            clip_duration=clip_duration,
-            clip_sampler_kwargs=clip_sampler_kwargs,
-            decode_audio=decode_audio,
-            decoder=decoder,
-        )
+        ds_kw = {
+            "clip_sampler": clip_sampler,
+            "clip_duration": clip_duration,
+            "clip_sampler_kwargs": clip_sampler_kwargs,
+            "decode_audio": decode_audio,
+            "decoder": decoder,
+        }
 
         train_data = (train_file, input_field, target_fields, train_videos_root, train_resolver)
         val_data = (val_file, input_field, target_fields, val_videos_root, val_resolver)
         test_data = (test_file, input_field, target_fields, test_videos_root, test_resolver)
         predict_data = (predict_file, input_field, predict_videos_root, predict_resolver)
 
         train_input = input_cls(
@@ -985,16 +968,16 @@
         label_field: str = "ground_truth",
         input_cls: Type[Input] = VideoClassificationFiftyOneInput,
         predict_input_cls: Type[Input] = VideoClassificationFiftyOnePredictInput,
         transform: INPUT_TRANSFORM_TYPE = VideoClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs,
     ) -> "VideoClassificationData":
-        """Load the :class:`~flash.video.classification.data.VideoClassificationData` from FiftyOne
-        ``SampleCollection`` objects.
+        """Load the :class:`~flash.video.classification.data.VideoClassificationData` from FiftyOne ``SampleCollection``
+        objects.
 
         The supported file extensions are: ``.mp4``, and ``.avi``.
         The targets will be extracted from the ``label_field`` in the ``SampleCollection`` objects and can be in any
         of our :ref:`supported classification target formats <formatting_classification_targets>`.
         To learn how to customize the transforms applied for each stage, read our
         :ref:`customizing transforms guide <customizing_transforms>`.
 
@@ -1076,21 +1059,21 @@
 
             >>> import os
             >>> _ = [os.remove(f"video_{i}.mp4") for i in range(1, 4)]
             >>> _ = [os.remove(f"predict_video_{i}.mp4") for i in range(1, 4)]
             >>> del train_dataset
             >>> del predict_dataset
         """
-        ds_kw = dict(
-            clip_sampler=clip_sampler,
-            clip_duration=clip_duration,
-            clip_sampler_kwargs=clip_sampler_kwargs,
-            decode_audio=decode_audio,
-            decoder=decoder,
-        )
+        ds_kw = {
+            "clip_sampler": clip_sampler,
+            "clip_duration": clip_duration,
+            "clip_sampler_kwargs": clip_sampler_kwargs,
+            "decode_audio": decode_audio,
+            "decoder": decoder,
+        }
 
         train_input = input_cls(
             RunningStage.TRAINING,
             train_dataset,
             video_sampler=video_sampler,
             label_field=label_field,
             target_formatter=target_formatter,
@@ -1144,19 +1127,18 @@
         decode_audio: bool = False,
         decoder: str = "pyav",
         input_cls: Type[Input] = LabelStudioVideoClassificationInput,
         transform: INPUT_TRANSFORM_TYPE = VideoClassificationInputTransform,
         transform_kwargs: Optional[Dict] = None,
         **data_module_kwargs,
     ) -> "VideoClassificationData":
-        """Creates a :class:`~flash.core.data.data_module.DataModule` object
-        from the given export file and data directory using the
-        :class:`~flash.core.data.io.input.Input` of name
-        :attr:`~flash.core.data.io.input.InputFormat.FOLDERS`
-        from the passed or constructed :class:`~flash.core.data.io.input_transform.InputTransform`.
+        """Creates a :class:`~flash.core.data.data_module.DataModule` object from the given export file and data
+        directory using the :class:`~flash.core.data.io.input.Input` of name
+        :attr:`~flash.core.data.io.input.InputFormat.FOLDERS` from the passed or constructed
+        :class:`~flash.core.data.io.input_transform.InputTransform`.
 
         Args:
             export_json: path to label studio export file
             train_export_json: path to label studio export file for train set. (overrides export_json if specified)
             val_export_json: path to label studio export file for validation
             test_export_json: path to label studio export file for test
             predict_export_json: path to label studio export file for predict
@@ -1202,22 +1184,22 @@
             val_data_folder=val_data_folder,
             test_data_folder=test_data_folder,
             predict_data_folder=predict_data_folder,
             val_split=val_split,
             multi_label=multi_label,
         )
 
-        ds_kw = dict(
-            clip_sampler=clip_sampler,
-            clip_duration=clip_duration,
-            clip_sampler_kwargs=clip_sampler_kwargs,
-            video_sampler=video_sampler,
-            decode_audio=decode_audio,
-            decoder=decoder,
-        )
+        ds_kw = {
+            "clip_sampler": clip_sampler,
+            "clip_duration": clip_duration,
+            "clip_sampler_kwargs": clip_sampler_kwargs,
+            "video_sampler": video_sampler,
+            "decode_audio": decode_audio,
+            "decoder": decoder,
+        }
 
         train_input = input_cls(RunningStage.TRAINING, train_data, **ds_kw)
         ds_kw["parameters"] = getattr(train_input, "parameters", None)
 
         return cls(
             train_input,
             input_cls(RunningStage.VALIDATING, val_data, **ds_kw),
```

### Comparing `lightning-flash-0.8.1.post0/flash/video/classification/input.py` & `lightning-flash-0.8.2/src/flash/video/classification/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 import pandas as pd
 import torch
 from torch.utils.data import Sampler
 
 from flash.core.data.io.classification_input import ClassificationInputMixin
 from flash.core.data.io.input import DataKeys, Input, IterableInput
-from flash.core.data.utilities.classification import _is_list_like, MultiBinaryTargetFormatter, TargetFormatter
+from flash.core.data.utilities.classification import MultiBinaryTargetFormatter, TargetFormatter, _is_list_like
 from flash.core.data.utilities.data_frame import resolve_files, resolve_targets
 from flash.core.data.utilities.loading import load_data_frame
-from flash.core.data.utilities.paths import list_valid_files, make_dataset, PATH_TYPE
+from flash.core.data.utilities.paths import PATH_TYPE, list_valid_files, make_dataset
 from flash.core.integrations.fiftyone.utils import FiftyOneLabelUtilities
 from flash.core.utilities.imports import _FIFTYONE_AVAILABLE, _PYTORCHVIDEO_AVAILABLE, lazy_import, requires
 
 if _FIFTYONE_AVAILABLE:
     fol = lazy_import("fiftyone.core.labels")
     SampleCollection = "fiftyone.core.collections.SampleCollection"
 else:
@@ -389,26 +389,24 @@
         )
 
 
 class VideoClassificationTensorsPredictInput(Input):
     def predict_load_data(self, data: Union[torch.Tensor, List[Any], Any]):
         if _is_list_like(data):
             return data
-        else:
-            if not isinstance(data, torch.Tensor):
-                raise TypeError(f"Expected either a list/tuple of torch.Tensor or torch.Tensor, but got: {type(data)}.")
-            if data.ndim == 5:
-                return list(data)
-            elif data.ndim == 4:
-                return [data]
-            else:
-                raise ValueError(
-                    f"Got dimension of the input tensor: {data.ndim},"
-                    " for stack of tensors - dimension should be 5 or for a single tensor, dimension should be 4."
-                )
+        if not isinstance(data, torch.Tensor):
+            raise TypeError(f"Expected either a list/tuple of torch.Tensor or torch.Tensor, but got: {type(data)}.")
+        if data.ndim == 5:
+            return list(data)
+        if data.ndim == 4:
+            return [data]
+        raise ValueError(
+            f"Got dimension of the input tensor: {data.ndim},"
+            " for stack of tensors - dimension should be 5 or for a single tensor, dimension should be 4."
+        )
 
     def predict_load_sample(self, sample: torch.Tensor) -> Dict[str, Any]:
         return {
             DataKeys.INPUT: sample,
             "video_index": 0,
         }
```

### Comparing `lightning-flash-0.8.1.post0/flash/video/classification/input_transform.py` & `lightning-flash-0.8.2/src/flash/video/classification/input_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 def normalize(x: Tensor) -> Tensor:
     return x / 255.0
 
 
 @requires("video")
 @dataclass
 class VideoClassificationInputTransform(InputTransform):
-
     image_size: int = 244
     temporal_sub_sample: int = 8
     mean: Tensor = torch.tensor([0.45, 0.45, 0.45])
     std: Tensor = torch.tensor([0.225, 0.225, 0.225])
     data_format: str = "BCTHW"
     same_on_frame: bool = False
```

### Comparing `lightning-flash-0.8.1.post0/flash/video/classification/model.py` & `lightning-flash-0.8.2/src/flash/video/classification/model.py`

 * *Files identical despite different names*

### Comparing `lightning-flash-0.8.1.post0/flash/video/classification/utils.py` & `lightning-flash-0.8.2/src/flash/video/classification/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional, Tuple, Type
 
 import torch
 
-from flash.core.utilities.imports import _VIDEO_AVAILABLE
+from flash.core.utilities.imports import _TOPIC_VIDEO_AVAILABLE
 
-if _VIDEO_AVAILABLE:
+if _TOPIC_VIDEO_AVAILABLE:
     from pytorchvideo.data.utils import MultiProcessSampler
 else:
     MultiProcessSampler = None
 
 
 class LabeledVideoTensorDataset(torch.utils.data.IterableDataset):
     """LabeledVideoTensorDataset handles a direct tensor input data."""
@@ -57,24 +57,22 @@
 
         # Reuse previously stored video if there are still clips to be sampled from
         # the last loaded video.
         video_index = next(self._video_sampler_iter)
         video_tensor, info_dict = self._labeled_videos[video_index]
         self._loaded_video_label = (video_tensor, info_dict, video_index)
 
-        sample_dict = {
+        return {
             "video": self._loaded_video_label[0],
             "video_name": f"video{video_index}",
             "video_index": video_index,
             "label": info_dict,
             "video_label": info_dict,
         }
 
-        return sample_dict
-
     def __iter__(self):
         self._video_sampler_iter = None  # Reset video sampler
 
         # If we're in a PyTorch DataLoader multiprocessing context, we need to use the
         # same seed for each worker's RandomSampler generator. The workers at each
         # __iter__ call are created from the unique value: worker_info.seed - worker_info.id,
         # which we can use for this seed.
```

### Comparing `lightning-flash-0.8.1.post0/lightning_flash.egg-info/PKG-INFO` & `lightning-flash-0.8.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,47 @@
-Metadata-Version: 2.1
-Name: lightning-flash
-Version: 0.8.1.post0
-Summary: Your PyTorch AI Factory - Flash enables you to easily configure and run complex AI recipes.
-Home-page: https://github.com/Lightning-AI/lightning-flash
-Download-URL: https://github.com/Lightning-AI/lightning-flash
-Author: PyTorchLightning et al.
-Author-email: name@pytorchlightning.ai
-License: Apache-2.0
-Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-flash/issues
-Project-URL: Documentation, https://lightning-flash.rtfd.io/en/latest/
-Project-URL: Source Code, https://github.com/Lightning-AI/lightning-flash
-Keywords: deep learning,pytorch,AI
-Classifier: Environment :: Console
-Classifier: Natural Language :: English
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: audio
-Provides-Extra: graph
-Provides-Extra: image
-Provides-Extra: pointcloud
-Provides-Extra: tabular
-Provides-Extra: text
-Provides-Extra: video
-Provides-Extra: devel
-Provides-Extra: docs
-Provides-Extra: notebooks
-Provides-Extra: serve
-Provides-Extra: test
-Provides-Extra: image_extras
-Provides-Extra: image_extras_baal
-Provides-Extra: video_extras
-Provides-Extra: vision
-Provides-Extra: core
-Provides-Extra: all
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/lightning-flash/raw/0.8.1.post0/docs/source/_static/images/logo.svg" width="400px">
+<img src="docs/source/_static/images/logo.svg" width="400px">
 
 
 **Your PyTorch AI Factory**
 
 ---
 
 <p align="center">
   <a href="#getting-started">Installation</a> •
   <a href="#flash-in-3-steps">Flash in 3 Steps</a> •
   <a href="https://lightning-flash.readthedocs.io/en/stable/?badge=stable">Docs</a> •
   <a href="#contribute">Contribute</a> •
   <a href="#community">Community</a> •
-  <a href="https://www.pytorchlightning.ai/">Website</a> •
+  <a href="https://www.lightning.ai/">Website</a> •
   <a href="#license">License</a>
 </p>
 
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning-flash)](https://pypi.org/project/lightning-flash/)
 [![PyPI Status](https://badge.fury.io/py/lightning-flash.svg)](https://badge.fury.io/py/lightning-flash)
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/pytorch-lightning/blob/master/LICENSE)
 
-![CI testing](https://github.com/Lightning-AI/lightning-flash/workflows/CI%20testing/badge.svg?tag=0.8.1.post0)
-[![codecov](https://codecov.io/gh/Lightning-AI/lightning-flash/release/0.8.1.post0/graph/badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-AI/lightning-flash)
+[![CI testing](https://github.com/Lightning-Universe/lightning-flash/actions/workflows/ci-testing.yml/badge.svg?event=push)](https://github.com/Lightning-Universe/lightning-flash/actions/workflows/ci-testing.yml)
+[![codecov](https://codecov.io/gh/Lightning-Universe/lightning-flash/branch/master/graph/badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-Universe/lightning-flash)
 [![Documentation Status](https://readthedocs.org/projects/lightning-flash/badge/?version=latest)](https://lightning-flash.readthedocs.io/en/stable/?badge=stable)
 [![DOI](https://zenodo.org/badge/333857397.svg)](https://zenodo.org/badge/latestdoi/333857397)
 
 </div>
 
 ---
 
 <div align="center">
   Flash makes complex AI recipes for over 15 tasks across 7 data domains accessible to all.
   <br / >
   In a nutshell, Flash is the production grade research framework you always dreamed of but didn't have time to build.
 </div>
 
-
-## News
-
-- Sept 30: [Lightning Flash now supports Meta-Learning](https://devblog.pytorchlightning.ai/lightning-flash-now-supports-meta-learning-7c0ac8b1cde7)
-- Sept 9: [Lightning Flash 0.5](https://devblog.pytorchlightning.ai/flash-0-5-your-pytorch-ai-factory-81b172ff0d76)
-- Jul 12: Flash Task-a-thon community sprint with 25+ community members
-- Jul 1: [Lightning Flash 0.4](https://devblog.pytorchlightning.ai/lightning-flash-0-4-flash-serve-fiftyone-multi-label-text-classification-and-jit-support-97428276c06f)
-- Jun 22: [Ushering in the New Age of Video Understanding with PyTorch](https://medium.com/pytorch/ushering-in-the-new-age-of-video-understanding-with-pytorch-1d85078e8015)
-- May 24: [Lightning Flash 0.3](https://devblog.pytorchlightning.ai/lightning-flash-0-3-new-tasks-visualization-tools-data-pipeline-and-flash-registry-api-1e236ba9530)
-- May 20: [Video Understanding with PyTorch](https://towardsdatascience.com/video-understanding-made-simple-with-pytorch-video-and-lightning-flash-c7d65583c37e)
-- Feb 2: [Read our launch blogpost](https://pytorch-lightning.medium.com/introducing-lightning-flash-the-fastest-way-to-get-started-with-deep-learning-202f196b3b98)
-
 ## Getting Started
 
 From PyPI:
 
 ```bash
 pip install lightning-flash
 ```
@@ -109,15 +49,15 @@
 See [our installation guide](https://lightning-flash.readthedocs.io/en/latest/installation.html) for more options.
 
 ## Flash in 3 Steps
 
 ### Step 1. Load your data
 
 All data loading in Flash is performed via a `from_*` classmethod on a `DataModule`.
-Which `DataModule` to use and which `from_*` methods are available depends on the task you want to perform.
+To decide which `DataModule` to use and which `from_*` methods are available, it depends on the task you want to perform.
 For example, for image segmentation where your data is stored in folders, you would use the [`from_folders` method of the `SemanticSegmentationData` class](https://lightning-flash.readthedocs.io/en/latest/reference/semantic_segmentation.html#from-folders):
 
 ```py
 from flash.image import SemanticSegmentationData
 
 dm = SemanticSegmentationData.from_folders(
     train_folder="data/CameraRGB",
@@ -129,15 +69,15 @@
 
 ```
 
 ### Step 2: Configure your model
 
 Our tasks come loaded with pre-trained backbones and (where applicable) heads.
 You can view the available backbones to use with your task using [`available_backbones`](https://lightning-flash.readthedocs.io/en/latest/general/backbones.html).
-Once you've chosen, create the model:
+Once you've chosen one, create the model:
 
 ```py
 from flash.image import SemanticSegmentation
 
 print(SemanticSegmentation.available_heads())
 # ['deeplabv3', 'deeplabv3plus', 'fpn', ..., 'unetplusplus']
 
@@ -163,40 +103,44 @@
 
 ---
 
 ## PyTorch Recipes
 
 ### Make predictions with Flash!
 
-Serve in just 2 lines.
+Serve in just 2 lines:
 
 ```py
 from flash.image import SemanticSegmentation
 
 model = SemanticSegmentation.load_from_checkpoint("semantic_segmentation_model.pt")
 model.serve()
 ```
 
 or make predictions from raw data directly.
 
 ```py
+from flash import Trainer
+
 trainer = Trainer(strategy='ddp', accelerator="gpu", gpus=2)
 dm = SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
 predictions = trainer.predict(model, dm)
 ```
 
 ### Flash Training Strategies
 
 Training strategies are PyTorch SOTA Training Recipes which can be utilized with a given task.
 
 
-Check out this [example](https://github.com/Lightning-AI/lightning-flash/blob/master/flash_examples/integrations/learn2learn/image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/meta-learning.html) from [Learn2Learn](https://github.com/learnables/learn2learn).
+Check out this [example](https://github.com/Lightning-AI/lightning-flash/blob/master/examples/integrations/learn2learn/image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/meta-learning.html) from [Learn2Learn](https://github.com/learnables/learn2learn).
 This is particularly useful if you use this model in production and want to make sure the model adapts quickly to its new environment with minimal labelled data.
 
 ```py
+from flash.image import ImageClassifier
+
 model = ImageClassifier(
     backbone="resnet18",
     optimizer=torch.optim.Adam,
     optimizer_kwargs={"lr": 0.001},
     training_strategy="prototypicalnetworks",
     training_strategy_kwargs={
         "epoch_length": 10 * 16,
@@ -218,28 +162,32 @@
 * **[maml](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_maml.py)** : from Finn *et al.* 2017, [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks](https://arxiv.org/abs/1703.03400)
 * **[metaoptnet](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_metaoptnet.py)** : from Lee *et al.* 2019, [Meta-Learning with Differentiable Convex Optimization](https://arxiv.org/abs/1904.03758)
 * **[anil](https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/lightning_anil.py)** : from Raghu *et al.* 2020, [Rapid Learning or Feature Reuse? Towards Understanding the Effectiveness of MAML](https://arxiv.org/abs/1909.09157)
 
 
 ### Flash Optimizers / Schedulers
 
-With Flash, swapping among 40+ optimizers and 15 + schedulers recipes are simple. Find the list of available optimizers, schedulers as follows:
+With Flash, swapping among 40+ optimizers and 15+ schedulers recipes are simple. Find the list of available optimizers, schedulers as follows:
 
 ```py
+from flash.image import ImageClassifier
+
 ImageClassifier.available_optimizers()
 # ['A2GradExp', ..., 'Yogi']
 
 ImageClassifier.available_schedulers()
 # ['CosineAnnealingLR', 'CosineAnnealingWarmRestarts', ..., 'polynomial_decay_schedule_with_warmup']
 ```
 
 Once you've chosen, create the model:
 
 ```py
-#### The optimizer of choice can be passed as a
+#### The optimizer of choice can be passed as
+from flash.image import ImageClassifier
+
 # - String value
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=None)
 
 # - Callable
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer=functools.partial(torch.optim.Adadelta, eps=0.5), lr_scheduler=None)
 
 # - Tuple[string, dict]: (The dict takes in the optimizer kwargs)
@@ -255,14 +203,16 @@
 # - Tuple[string, dict]: (The dict takes in the scheduler kwargs)
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=("StepLR", {"step_size": 10}))
 ```
 
 You can also register you own custom scheduler recipes beforeahand and use them shown as above:
 
 ```py
+from flash.image import ImageClassifier
+
 @ImageClassifier.lr_schedulers_registry
 def my_steplr_recipe(optimizer):
     return torch.optim.lr_scheduler.StepLR(optimizer, step_size=10)
 
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler="my_steplr_recipe")
 ```
 
@@ -314,30 +264,30 @@
 )
 
 ```
 
 ## Flash Zero - PyTorch Recipes from the Command Line!
 
 <div align="center">
-<img src="/https://github.com/Lightning-AI/lightning-flash/raw/0.8.1.post0/docs/source/_static/images/flash_zero.gif?raw=true" width="75%">
+<img src="/docs/source/_static/images/flash_zero.gif?raw=true" width="75%">
 </div>
 
 Flash Zero is a zero-code machine learning platform built
 directly into lightning-flash
-using the [`Lightning CLI`](https://pytorch-lightning.readthedocs.io/en/0.8.1.post0common/lightning_cli.html).
+using the [`Lightning CLI`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_cli.html).
 
 To get started and view the available tasks, run:
 
-```py
+```bash
   flash --help
 ```
 
 For example, to train an image classifier for 10 epochs with a `resnet50` backbone on 2 GPUs using your own data, you can do:
 
-```py
+```bash
   flash image_classification --trainer.max_epochs 10 --trainer.gpus 2 --model.backbone resnet50 from_folders --train_folder {PATH_TO_DATA}
 ```
 
 ## Kaggle Notebook Examples
 
 - [🚢Titanic crash with Lightning⚡Flash](https://www.kaggle.com/jirkaborovec/titanic-crash-with-lightning-flash)
 - [🏠House 💵prices predictions with Lightning⚡Flash](https://www.kaggle.com/jirkaborovec/house-prices-predictions-with-lightning-flash)
```

#### html2text {}

```diff
@@ -1,161 +1,124 @@
-Metadata-Version: 2.1 Name: lightning-flash Version: 0.8.1.post0 Summary: Your
-PyTorch AI Factory - Flash enables you to easily configure and run complex AI
-recipes. Home-page: https://github.com/Lightning-AI/lightning-flash Download-
-URL: https://github.com/Lightning-AI/lightning-flash Author: PyTorchLightning
-et al. Author-email: name@pytorchlightning.ai License: Apache-2.0 Project-URL:
-Bug Tracker, https://github.com/Lightning-AI/lightning-flash/issues Project-
-URL: Documentation, https://lightning-flash.rtfd.io/en/latest/ Project-URL:
-Source Code, https://github.com/Lightning-AI/lightning-flash Keywords: deep
-learning,pytorch,AI Classifier: Environment :: Console Classifier: Natural
-Language :: English Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Image
-Recognition Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: audio Provides-Extra: graph Provides-Extra: image Provides-
-Extra: pointcloud Provides-Extra: tabular Provides-Extra: text Provides-Extra:
-video Provides-Extra: devel Provides-Extra: docs Provides-Extra: notebooks
-Provides-Extra: serve Provides-Extra: test Provides-Extra: image_extras
-Provides-Extra: image_extras_baal Provides-Extra: video_extras Provides-Extra:
-vision Provides-Extra: core Provides-Extra: all Provides-Extra: dev License-
-File: LICENSE
- [https://github.com/Lightning-AI/lightning-flash/raw/0.8.1.post0/docs/source/
-           _static/images/logo.svg] **Your PyTorch AI Factory** ---
+     [docs/source/_static/images/logo.svg] **Your PyTorch AI Factory** ---
   Installation â¢ Flash_in_3_Steps â¢ Docs â¢ Contribute â¢ Community â¢
                               Website â¢ License
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning-
   flash)](https://pypi.org/project/lightning-flash/) [![PyPI Status](https://
   badge.fury.io/py/lightning-flash.svg)](https://badge.fury.io/py/lightning-
 flash) [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)]
 (https://www.pytorchlightning.ai/community) [![license](https://img.shields.io/
 badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/pytorch-
- lightning/blob/master/LICENSE) ![CI testing](https://github.com/Lightning-AI/
- lightning-flash/workflows/CI%20testing/badge.svg?tag=0.8.1.post0) [![codecov]
-(https://codecov.io/gh/Lightning-AI/lightning-flash/release/0.8.1.post0/graph/
-  badge.svg?token=oLuUr9q1vt)](https://codecov.io/gh/Lightning-AI/lightning-
-  flash) [![Documentation Status](https://readthedocs.org/projects/lightning-
-flash/badge/?version=latest)](https://lightning-flash.readthedocs.io/en/stable/
+  lightning/blob/master/LICENSE) [![CI testing](https://github.com/Lightning-
+          Universe/lightning-flash/actions/workflows/ci-testing.yml/
+ badge.svg?event=push)](https://github.com/Lightning-Universe/lightning-flash/
+actions/workflows/ci-testing.yml) [![codecov](https://codecov.io/gh/Lightning-
+   Universe/lightning-flash/branch/master/graph/badge.svg?token=oLuUr9q1vt)]
+  (https://codecov.io/gh/Lightning-Universe/lightning-flash) [![Documentation
+        Status](https://readthedocs.org/projects/lightning-flash/badge/
+      ?version=latest)](https://lightning-flash.readthedocs.io/en/stable/
    ?badge=stable) [![DOI](https://zenodo.org/badge/333857397.svg)](https://
                      zenodo.org/badge/latestdoi/333857397)
 ---
     Flash makes complex AI recipes for over 15 tasks across 7 data domains
                               accessible to all.
  > In a nutshell, Flash is the production grade research framework you always
                    dreamed of but didn't have time to build.
-## News - Sept 30: [Lightning Flash now supports Meta-Learning](https://
-devblog.pytorchlightning.ai/lightning-flash-now-supports-meta-learning-
-7c0ac8b1cde7) - Sept 9: [Lightning Flash 0.5](https://
-devblog.pytorchlightning.ai/flash-0-5-your-pytorch-ai-factory-81b172ff0d76) -
-Jul 12: Flash Task-a-thon community sprint with 25+ community members - Jul 1:
-[Lightning Flash 0.4](https://devblog.pytorchlightning.ai/lightning-flash-0-4-
-flash-serve-fiftyone-multi-label-text-classification-and-jit-support-
-97428276c06f) - Jun 22: [Ushering in the New Age of Video Understanding with
-PyTorch](https://medium.com/pytorch/ushering-in-the-new-age-of-video-
-understanding-with-pytorch-1d85078e8015) - May 24: [Lightning Flash 0.3](https:
-//devblog.pytorchlightning.ai/lightning-flash-0-3-new-tasks-visualization-
-tools-data-pipeline-and-flash-registry-api-1e236ba9530) - May 20: [Video
-Understanding with PyTorch](https://towardsdatascience.com/video-understanding-
-made-simple-with-pytorch-video-and-lightning-flash-c7d65583c37e) - Feb 2: [Read
-our launch blogpost](https://pytorch-lightning.medium.com/introducing-
-lightning-flash-the-fastest-way-to-get-started-with-deep-learning-202f196b3b98)
 ## Getting Started From PyPI: ```bash pip install lightning-flash ``` See [our
 installation guide](https://lightning-flash.readthedocs.io/en/latest/
 installation.html) for more options. ## Flash in 3 Steps ### Step 1. Load your
 data All data loading in Flash is performed via a `from_*` classmethod on a
-`DataModule`. Which `DataModule` to use and which `from_*` methods are
-available depends on the task you want to perform. For example, for image
-segmentation where your data is stored in folders, you would use the
+`DataModule`. To decide which `DataModule` to use and which `from_*` methods
+are available, it depends on the task you want to perform. For example, for
+image segmentation where your data is stored in folders, you would use the
 [`from_folders` method of the `SemanticSegmentationData` class](https://
 lightning-flash.readthedocs.io/en/latest/reference/
 semantic_segmentation.html#from-folders): ```py from flash.image import
 SemanticSegmentationData dm = SemanticSegmentationData.from_folders
 ( train_folder="data/CameraRGB", train_target_folder="data/CameraSeg",
 val_split=0.1, image_size=(256, 256), num_classes=21, ) ``` ### Step 2:
 Configure your model Our tasks come loaded with pre-trained backbones and
 (where applicable) heads. You can view the available backbones to use with your
 task using [`available_backbones`](https://lightning-flash.readthedocs.io/en/
-latest/general/backbones.html). Once you've chosen, create the model: ```py
+latest/general/backbones.html). Once you've chosen one, create the model: ```py
 from flash.image import SemanticSegmentation print
 (SemanticSegmentation.available_heads()) # ['deeplabv3', 'deeplabv3plus',
 'fpn', ..., 'unetplusplus'] print(SemanticSegmentation.available_backbones
 ('fpn')) # ['densenet121', ..., 'xception'] # + 113 models print
 (SemanticSegmentation.available_pretrained_weights('efficientnet-b0')) #
 ['imagenet', 'advprop'] model = SemanticSegmentation( head="fpn",
 backbone='efficientnet-b0', pretrained="advprop", num_classes=dm.num_classes)
 ``` ### Step 3: Finetune! ```py from flash import Trainer trainer = Trainer
 (max_epochs=3) trainer.finetune(model, datamodule=datamodule,
 strategy="freeze") trainer.save_checkpoint("semantic_segmentation_model.pt")
 ``` --- ## PyTorch Recipes ### Make predictions with Flash! Serve in just 2
-lines. ```py from flash.image import SemanticSegmentation model =
+lines: ```py from flash.image import SemanticSegmentation model =
 SemanticSegmentation.load_from_checkpoint("semantic_segmentation_model.pt")
-model.serve() ``` or make predictions from raw data directly. ```py trainer =
-Trainer(strategy='ddp', accelerator="gpu", gpus=2) dm =
-SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
+model.serve() ``` or make predictions from raw data directly. ```py from flash
+import Trainer trainer = Trainer(strategy='ddp', accelerator="gpu", gpus=2) dm
+= SemanticSegmentationData.from_folders(predict_folder="data/CameraRGB")
 predictions = trainer.predict(model, dm) ``` ### Flash Training Strategies
 Training strategies are PyTorch SOTA Training Recipes which can be utilized
 with a given task. Check out this [example](https://github.com/Lightning-AI/
-lightning-flash/blob/master/flash_examples/integrations/learn2learn/
+lightning-flash/blob/master/examples/integrations/learn2learn/
 image_classification_imagenette_mini.py) where the `ImageClassifier` supports 4
 [Meta Learning Algorithms](https://lilianweng.github.io/lil-log/2018/11/30/
 meta-learning.html) from [Learn2Learn](https://github.com/learnables/
 learn2learn). This is particularly useful if you use this model in production
 and want to make sure the model adapts quickly to its new environment with
-minimal labelled data. ```py model = ImageClassifier( backbone="resnet18",
-optimizer=torch.optim.Adam, optimizer_kwargs={"lr": 0.001},
-training_strategy="prototypicalnetworks", training_strategy_kwargs=
-{ "epoch_length": 10 * 16, "meta_batch_size": 4, "num_tasks": 200,
-"test_num_tasks": 2000, "ways": datamodule.num_classes, "shots": 1,
-"test_ways": 5, "test_shots": 1, "test_queries": 15, }, ) ``` In detail, the
-following methods are currently implemented: * **[prototypicalnetworks](https:/
-/github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/
-lightning/lightning_protonet.py)** : from Snell *et al.* 2017, [Prototypical
-Networks for Few-shot Learning](https://arxiv.org/abs/1703.05175) * **[maml]
-(https://github.com/learnables/learn2learn/blob/master/learn2learn/algorithms/
-lightning/lightning_maml.py)** : from Finn *et al.* 2017, [Model-Agnostic Meta-
-Learning for Fast Adaptation of Deep Networks](https://arxiv.org/abs/
-1703.03400) * **[metaoptnet](https://github.com/learnables/learn2learn/blob/
-master/learn2learn/algorithms/lightning/lightning_metaoptnet.py)** : from Lee
-*et al.* 2019, [Meta-Learning with Differentiable Convex Optimization](https://
-arxiv.org/abs/1904.03758) * **[anil](https://github.com/learnables/learn2learn/
-blob/master/learn2learn/algorithms/lightning/lightning_anil.py)** : from Raghu
-*et al.* 2020, [Rapid Learning or Feature Reuse? Towards Understanding the
-Effectiveness of MAML](https://arxiv.org/abs/1909.09157) ### Flash Optimizers /
-Schedulers With Flash, swapping among 40+ optimizers and 15 + schedulers
-recipes are simple. Find the list of available optimizers, schedulers as
-follows: ```py ImageClassifier.available_optimizers() # ['A2GradExp', ...,
-'Yogi'] ImageClassifier.available_schedulers() # ['CosineAnnealingLR',
-'CosineAnnealingWarmRestarts', ..., 'polynomial_decay_schedule_with_warmup']
-``` Once you've chosen, create the model: ```py #### The optimizer of choice
-can be passed as a # - String value model = ImageClassifier
+minimal labelled data. ```py from flash.image import ImageClassifier model =
+ImageClassifier( backbone="resnet18", optimizer=torch.optim.Adam,
+optimizer_kwargs={"lr": 0.001}, training_strategy="prototypicalnetworks",
+training_strategy_kwargs={ "epoch_length": 10 * 16, "meta_batch_size": 4,
+"num_tasks": 200, "test_num_tasks": 2000, "ways": datamodule.num_classes,
+"shots": 1, "test_ways": 5, "test_shots": 1, "test_queries": 15, }, ) ``` In
+detail, the following methods are currently implemented: * **
+[prototypicalnetworks](https://github.com/learnables/learn2learn/blob/master/
+learn2learn/algorithms/lightning/lightning_protonet.py)** : from Snell *et al.*
+2017, [Prototypical Networks for Few-shot Learning](https://arxiv.org/abs/
+1703.05175) * **[maml](https://github.com/learnables/learn2learn/blob/master/
+learn2learn/algorithms/lightning/lightning_maml.py)** : from Finn *et al.*
+2017, [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks]
+(https://arxiv.org/abs/1703.03400) * **[metaoptnet](https://github.com/
+learnables/learn2learn/blob/master/learn2learn/algorithms/lightning/
+lightning_metaoptnet.py)** : from Lee *et al.* 2019, [Meta-Learning with
+Differentiable Convex Optimization](https://arxiv.org/abs/1904.03758) * **
+[anil](https://github.com/learnables/learn2learn/blob/master/learn2learn/
+algorithms/lightning/lightning_anil.py)** : from Raghu *et al.* 2020, [Rapid
+Learning or Feature Reuse? Towards Understanding the Effectiveness of MAML]
+(https://arxiv.org/abs/1909.09157) ### Flash Optimizers / Schedulers With
+Flash, swapping among 40+ optimizers and 15+ schedulers recipes are simple.
+Find the list of available optimizers, schedulers as follows: ```py from
+flash.image import ImageClassifier ImageClassifier.available_optimizers() #
+['A2GradExp', ..., 'Yogi'] ImageClassifier.available_schedulers() #
+['CosineAnnealingLR', 'CosineAnnealingWarmRestarts', ...,
+'polynomial_decay_schedule_with_warmup'] ``` Once you've chosen, create the
+model: ```py #### The optimizer of choice can be passed as from flash.image
+import ImageClassifier # - String value model = ImageClassifier
 (backbone="resnet18", num_classes=2, optimizer="Adam", lr_scheduler=None) # -
 Callable model = ImageClassifier(backbone="resnet18", num_classes=2,
 optimizer=functools.partial(torch.optim.Adadelta, eps=0.5), lr_scheduler=None)
 # - Tuple[string, dict]: (The dict takes in the optimizer kwargs) model =
 ImageClassifier(backbone="resnet18", num_classes=2, optimizer=("Adadelta",
 {"epa": 0.5}), lr_scheduler=None) #### The scheduler of choice can be passed as
 a # - String value model = ImageClassifier(backbone="resnet18", num_classes=2,
 optimizer="Adam", lr_scheduler="constant_schedule") # - Callable model =
 ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
 lr_scheduler=functools.partial(CyclicLR, step_size_up=1500, mode='exp_range',
 gamma=0.5)) # - Tuple[string, dict]: (The dict takes in the scheduler kwargs)
 model = ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
 lr_scheduler=("StepLR", {"step_size": 10})) ``` You can also register you own
-custom scheduler recipes beforeahand and use them shown as above: ```py
-@ImageClassifier.lr_schedulers_registry def my_steplr_recipe(optimizer): return
-torch.optim.lr_scheduler.StepLR(optimizer, step_size=10) model =
-ImageClassifier(backbone="resnet18", num_classes=2, optimizer="Adam",
-lr_scheduler="my_steplr_recipe") ``` ### Flash Transforms Flash includes some
-simple augmentations for each task by default, however, you will often want to
-override these and control your own augmentation recipe. To this end, Flash
-supports custom transformations with the [`InputTransform`](https://lightning-
-flash.readthedocs.io/en/stable/api/generated/
+custom scheduler recipes beforeahand and use them shown as above: ```py from
+flash.image import ImageClassifier @ImageClassifier.lr_schedulers_registry def
+my_steplr_recipe(optimizer): return torch.optim.lr_scheduler.StepLR(optimizer,
+step_size=10) model = ImageClassifier(backbone="resnet18", num_classes=2,
+optimizer="Adam", lr_scheduler="my_steplr_recipe") ``` ### Flash Transforms
+Flash includes some simple augmentations for each task by default, however, you
+will often want to override these and control your own augmentation recipe. To
+this end, Flash supports custom transformations with the [`InputTransform`]
+(https://lightning-flash.readthedocs.io/en/stable/api/generated/
 flash.core.data.io.input_transform.InputTransform.html). The `InputTransform`
 is like a callback for transforms, with hooks that can be used to apply
 transforms to samples or batches, on and off the device / accelerator. In
 addition, hooks can be specialized to apply transforms only to the input or
 target. With these hooks, complex transforms like MixUp can be implemented with
 ease. Here's an example (with an albumentations transform thrown in too!):
 ```py import torch import numpy as np import albumentations from flash import
@@ -168,22 +131,21 @@
 batch class MixUpInputTransform(InputTransform): def
 train_input_per_sample_transform(self): return AlbumentationsAdapter
 (albumentations.HorizontalFlip(p=0.5)) # This will be applied after
 transferring the batch to the device! def train_per_batch_transform_on_device
 (self): return mixup datamodule = ImageClassificationData.from_folders
 ( train_folder="data/train", transform=MixUpInputTransform, batch_size=2, ) ```
 ## Flash Zero - PyTorch Recipes from the Command Line!
-[/https://github.com/Lightning-AI/lightning-flash/raw/0.8.1.post0/docs/source/
-                    _static/images/flash_zero.gif?raw=true]
+             [/docs/source/_static/images/flash_zero.gif?raw=true]
 Flash Zero is a zero-code machine learning platform built directly into
 lightning-flash using the [`Lightning CLI`](https://pytorch-
-lightning.readthedocs.io/en/0.8.1.post0common/lightning_cli.html). To get
-started and view the available tasks, run: ```py flash --help ``` For example,
-to train an image classifier for 10 epochs with a `resnet50` backbone on 2 GPUs
-using your own data, you can do: ```py flash image_classification --
+lightning.readthedocs.io/en/stable/common/lightning_cli.html). To get started
+and view the available tasks, run: ```bash flash --help ``` For example, to
+train an image classifier for 10 epochs with a `resnet50` backbone on 2 GPUs
+using your own data, you can do: ```bash flash image_classification --
 trainer.max_epochs 10 --trainer.gpus 2 --model.backbone resnet50 from_folders -
 -train_folder {PATH_TO_DATA} ``` ## Kaggle Notebook Examples - [ð¢Titanic
 crash with Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/titanic-
 crash-with-lightning-flash) - [ð House ðµprices predictions with
 Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/house-prices-
 predictions-with-lightning-flash) - [Playing ðtabular with
 Lightningâ¡Flash](https://www.kaggle.com/jirkaborovec/playing-tabular-with-
```

