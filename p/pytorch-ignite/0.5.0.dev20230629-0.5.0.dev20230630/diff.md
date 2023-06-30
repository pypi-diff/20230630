# Comparing `tmp/pytorch-ignite-0.5.0.dev20230629.tar.gz` & `tmp/pytorch-ignite-0.5.0.dev20230630.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-ignite-0.5.0.dev20230629.tar", last modified: Thu Jun 29 00:19:28 2023, max compression
+gzip compressed data, was "pytorch-ignite-0.5.0.dev20230630.tar", last modified: Fri Jun 30 00:17:01 2023, max compression
```

## Comparing `pytorch-ignite-0.5.0.dev20230629.tar` & `pytorch-ignite-0.5.0.dev20230630.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.924470 pytorch-ignite-0.5.0.dev20230629/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28342 2023-06-29 00:19:28.924470 pytorch-ignite-0.5.0.dev20230629/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27890 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.900470 pytorch-ignite-0.5.0.dev20230629/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 00:13:06.000000 pytorch-ignite-0.5.0.dev20230629/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.900470 pytorch-ignite-0.5.0.dev20230629/ignite/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/base/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.900470 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.904470 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/engines/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28561 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/engines/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/engines/tbptt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.904470 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    37618 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27453 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.908470 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/precision_recall_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.908470 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/roc_auc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.912470 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.912470 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    26478 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/xla.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    22584 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.912470 pytorch-ignite-0.5.0.dev20230629/ignite/engine/
--rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/engine/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)    54999 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/engine/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.916470 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44795 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/ema_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    65160 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/state_param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/handlers/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.920470 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/classification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/epoch_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/fbeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.920470 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/gan/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/gan/fid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/gan/inception_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/gan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/mean_pairwise_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    24263 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/metrics_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/multilabel_confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.924470 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/nlp/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/nlp/rouge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/psnr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/running_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/metrics/top_k_categorical_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/ignite/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:19:28.924470 pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28342 2023-06-29 00:19:28.000000 pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-29 00:19:28.000000 pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:19:28.000000 pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:19:28.000000 pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 00:19:28.000000 pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 00:19:28.000000 pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-29 00:19:28.924470 pytorch-ignite-0.5.0.dev20230629/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-29 00:12:21.000000 pytorch-ignite-0.5.0.dev20230629/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.701743 pytorch-ignite-0.5.0.dev20230630/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28342 2023-06-30 00:17:01.701743 pytorch-ignite-0.5.0.dev20230630/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27890 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.677743 pytorch-ignite-0.5.0.dev20230630/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 00:12:13.000000 pytorch-ignite-0.5.0.dev20230630/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.677743 pytorch-ignite-0.5.0.dev20230630/ignite/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/base/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.677743 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.677743 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/engines/tbptt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.681743 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37618 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27453 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.685743 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/precision_recall_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.689743 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/roc_auc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.689743 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.689743 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26478 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22584 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.693743 pytorch-ignite-0.5.0.dev20230630/ignite/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/engine/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54999 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.693743 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44795 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/ema_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65143 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/state_param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/handlers/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.697743 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/classification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/epoch_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/fbeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.697743 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/gan/fid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/gan/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/gan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/mean_pairwise_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27675 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/metrics_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/multilabel_confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.697743 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/nlp/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/nlp/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/running_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/metrics/top_k_categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/ignite/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:17:01.701743 pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28342 2023-06-30 00:17:01.000000 pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-30 00:17:01.000000 pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:17:01.000000 pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:17:01.000000 pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 00:17:01.000000 pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 00:17:01.000000 pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-30 00:17:01.701743 pytorch-ignite-0.5.0.dev20230630/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-30 00:11:44.000000 pytorch-ignite-0.5.0.dev20230630/setup.py
```

### Comparing `pytorch-ignite-0.5.0.dev20230629/LICENSE` & `pytorch-ignite-0.5.0.dev20230630/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/PKG-INFO` & `pytorch-ignite-0.5.0.dev20230630/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.dev20230629
+Version: 0.5.0.dev20230630
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.5.0.dev20230629/README.md` & `pytorch-ignite-0.5.0.dev20230630/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/base/mixins.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/base/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/engines/common.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/engines/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from ignite.contrib.handlers.base_logger import BaseLogger
 from ignite.contrib.metrics import GpuInfo
 from ignite.engine import Engine, Events
 from ignite.handlers import Checkpoint, DiskSaver, EarlyStopping, TerminateOnNan
 from ignite.handlers.checkpoint import BaseSaveHandler
 from ignite.handlers.param_scheduler import ParamScheduler
 from ignite.metrics import RunningAverage
+from ignite.metrics.metric import RunningBatchWise
 from ignite.utils import deprecated
 
 
 def setup_common_training_handlers(
     trainer: Engine,
     train_sampler: Optional[DistributedSampler] = None,
     to_save: Optional[Mapping] = None,
@@ -205,16 +206,16 @@
             else:
                 raise TypeError(
                     "Unhandled type of update_function's output. "
                     f"It should either mapping or sequence, but given {type(x)}"
                 )
 
         for i, n in enumerate(output_names):
-            RunningAverage(output_transform=partial(output_transform, index=i, name=n), epoch_bound=False).attach(
-                trainer, n
+            RunningAverage(output_transform=partial(output_transform, index=i, name=n)).attach(
+                trainer, n, usage=RunningBatchWise()
             )
 
     if with_pbars:
         if with_pbar_on_iters:
             ProgressBar(persist=False).attach(
                 trainer, metric_names="all", event_name=Events.ITERATION_COMPLETED(every=log_every_iters)
             )
```

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/engines/tbptt.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/engines/tbptt.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/__init__.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/base_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/clearml_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/lr_finder.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/mlflow_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/neptune_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/polyaxon_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/tensorboard_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/time_profilers.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/tqdm_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/visdom_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/handlers/wandb_logger.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/average_precision.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/cohen_kappa.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/gpu_info.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/precision_recall_curve.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/__init__.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/_base.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/canberra_metric.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/fractional_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/fractional_bias.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/manhattan_distance.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/maximum_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/mean_absolute_relative_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/mean_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/mean_normalized_bias.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/median_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/median_absolute_percentage_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/median_relative_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/r2_score.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/regression/wave_hedges_distance.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/contrib/metrics/roc_auc.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/contrib/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/distributed/auto.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/distributed/auto.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/__init__.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/base.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/horovod.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/horovod.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/native.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/native.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/distributed/comp_models/xla.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/distributed/comp_models/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/distributed/launcher.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/distributed/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/distributed/utils.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/engine/__init__.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/engine/deterministic.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/engine/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/engine/engine.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/engine/events.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/engine/events.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/engine/utils.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/__init__.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/checkpoint.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/early_stopping.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/ema_handler.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/ema_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/lr_finder.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/param_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1504,28 +1504,27 @@
             `state.output.param_history`. Is used if `save_history`
             is true. Default: None.
         save_history: Whether to save history or not. If true,
             history will be logged in `trainer`'s `state.output.param_history`.
             Default: False.
         param_group_index: `optimizer`'s parameters group
             to use.  Default: None. Use all `optimizer`'s paramater groups.
-        **scheduler_kwargs: Keyword arguments to be passed to the wrapped
-            `ReduceLROnPlateau`.
+        scheduler_kwargs: Keyword arguments to be passed to the wrapped ``ReduceLROnPlateau``.
 
     Examples:
 
-        .. code-block python
+        .. code-block:: python
 
-            # Metric 'metric-name' should surpass its best value by
+            # Metric "accuracy" should increase the best value by
             # more than 1 unit after at most 2 epochs, otherwise LR
             # would get multiplied by 0.5 .
 
             scheduler = ReduceLROnPlateauScheduler(
                 default_optimizer,
-                metric_name="metric-name", mode="max",
+                metric_name="accuracy", mode="max",
                 factor=0.5, patience=1, threshold_mode='abs',
                 threshold=1, trainer=trainer
             )
 
             metric = Accuracy()
             default_evaluator.attach(metric, "accuracy")
 
@@ -1534,18 +1533,18 @@
         .. include:: defaults.rst
             :start-after: :orphan:
 
         .. testcode::
 
             default_trainer = get_default_trainer()
 
-            # Metric `loss` should decrease more than
-            # a tenth of best loss after at most
+            # Metric "loss" should decrease more than
+            # 0.1 of best loss after at most
             # three iterations. Then best loss would get
-            # updated, otherwise lr is multiplied by 2
+            # updated, otherwise lr is multiplied by 0.5
 
             scheduler = ReduceLROnPlateauScheduler(
                 default_optimizer, "loss",
                 save_history=True, mode="min",
                 factor=0.5, patience=3, threshold_mode='rel',
                 threshold=0.1, trainer=default_trainer
             )
```

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/state_param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/state_param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/stores.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/stores.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/terminate_on_nan.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/time_limit.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/time_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/time_profilers.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/handlers/timing.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/handlers/timing.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/__init__.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/accumulation.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/accuracy.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/classification_report.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/confusion_matrix.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/epoch_metric.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/epoch_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/fbeta.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/fbeta.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/frequency.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/frequency.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/gan/fid.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/gan/fid.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/gan/inception_score.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/gan/inception_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/gan/utils.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/gan/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/loss.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/mean_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/mean_pairwise_distance.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/mean_pairwise_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/mean_squared_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/metric.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,24 @@
 
 import ignite.distributed as idist
 from ignite.engine import CallableEventWithFilter, Engine, Events
 
 if TYPE_CHECKING:
     from ignite.metrics.metrics_lambda import MetricsLambda
 
-__all__ = ["Metric", "MetricUsage", "EpochWise", "BatchWise", "BatchFiltered"]
+__all__ = [
+    "Metric",
+    "MetricUsage",
+    "EpochWise",
+    "BatchWise",
+    "BatchFiltered",
+    "RunningEpochWise",
+    "RunningBatchWise",
+    "SingleEpochRunningBatchWise",
+]
 
 
 class MetricUsage:
     """
     Base class for all usages of metrics.
 
     A usage of metric defines the events when a metric starts to compute, updates and completes.
@@ -27,14 +36,16 @@
             :meth:`~ignite.metrics.metric.Metric.started`.
         completed: event when the metric completes. This event will be associated to
             :meth:`~ignite.metrics.metric.Metric.completed`.
         iteration_completed: event when the metric updates. This event will be associated to
             :meth:`~ignite.metrics.metric.Metric.iteration_completed`.
     """
 
+    usage_name: str
+
     def __init__(self, started: Events, completed: Events, iteration_completed: CallableEventWithFilter) -> None:
         self.__started = started
         self.__completed = completed
         self.__iteration_completed = iteration_completed
 
     @property
     def STARTED(self) -> Events:
@@ -70,14 +81,41 @@
         super(EpochWise, self).__init__(
             started=Events.EPOCH_STARTED,
             completed=Events.EPOCH_COMPLETED,
             iteration_completed=Events.ITERATION_COMPLETED,
         )
 
 
+class RunningEpochWise(EpochWise):
+    """
+    Running epoch-wise usage of Metrics. It's the running version of the :class:`~.metrics.metric.EpochWise` metric
+    usage. A metric with such a usage most likely accompanies an :class:`~.metrics.metric.EpochWise` one to compute
+    a running measure of it e.g. running average.
+
+    Metric's methods are triggered on the following engine events:
+
+    - :meth:`~ignite.metrics.metric.Metric.started` on every ``STARTED``
+      (See :class:`~ignite.engine.events.Events`).
+    - :meth:`~ignite.metrics.metric.Metric.iteration_completed` on every ``EPOCH_COMPLETED``.
+    - :meth:`~ignite.metrics.metric.Metric.completed` on every ``EPOCH_COMPLETED``.
+
+    Attributes:
+        usage_name: usage name string
+    """
+
+    usage_name: str = "running_epoch_wise"
+
+    def __init__(self) -> None:
+        super(EpochWise, self).__init__(
+            started=Events.STARTED,
+            completed=Events.EPOCH_COMPLETED,
+            iteration_completed=Events.EPOCH_COMPLETED,
+        )
+
+
 class BatchWise(MetricUsage):
     """
     Batch-wise usage of Metrics.
 
     Metric's methods are triggered on the following engine events:
 
     - :meth:`~ignite.metrics.metric.Metric.started` on every ``ITERATION_STARTED``
@@ -95,14 +133,67 @@
         super(BatchWise, self).__init__(
             started=Events.ITERATION_STARTED,
             completed=Events.ITERATION_COMPLETED,
             iteration_completed=Events.ITERATION_COMPLETED,
         )
 
 
+class RunningBatchWise(BatchWise):
+    """
+    Running batch-wise usage of Metrics. It's the running version of the :class:`~.metrics.metric.EpochWise` metric
+    usage. A metric with such a usage could for example accompany a :class:`~.metrics.metric.BatchWise` one to compute
+    a running measure of it e.g. running average.
+
+    Metric's methods are triggered on the following engine events:
+
+    - :meth:`~ignite.metrics.metric.Metric.started` on every ``STARTED``
+      (See :class:`~ignite.engine.events.Events`).
+    - :meth:`~ignite.metrics.metric.Metric.iteration_completed` on every ``ITERATION_COMPLETED``.
+    - :meth:`~ignite.metrics.metric.Metric.completed` on every ``ITERATION_COMPLETED``.
+
+    Attributes:
+        usage_name: usage name string
+    """
+
+    usage_name: str = "running_batch_wise"
+
+    def __init__(self) -> None:
+        super(BatchWise, self).__init__(
+            started=Events.STARTED,
+            completed=Events.ITERATION_COMPLETED,
+            iteration_completed=Events.ITERATION_COMPLETED,
+        )
+
+
+class SingleEpochRunningBatchWise(BatchWise):
+    """
+    Running batch-wise usage of Metrics in a single epoch. It's like :class:`~.metrics.metric.RunningBatchWise` metric
+    usage with the difference that is used during a single epoch.
+
+    Metric's methods are triggered on the following engine events:
+
+    - :meth:`~ignite.metrics.metric.Metric.started` on every ``EPOCH_STARTED``
+      (See :class:`~ignite.engine.events.Events`).
+    - :meth:`~ignite.metrics.metric.Metric.iteration_completed` on every ``ITERATION_COMPLETED``.
+    - :meth:`~ignite.metrics.metric.Metric.completed` on every ``ITERATION_COMPLETED``.
+
+    Attributes:
+        usage_name: usage name string
+    """
+
+    usage_name: str = "single_epoch_running_batch_wise"
+
+    def __init__(self) -> None:
+        super(BatchWise, self).__init__(
+            started=Events.EPOCH_STARTED,
+            completed=Events.ITERATION_COMPLETED,
+            iteration_completed=Events.ITERATION_COMPLETED,
+        )
+
+
 class BatchFiltered(MetricUsage):
     """
     Batch filtered usage of Metrics. This usage is similar to epoch-wise but update event is filtered.
 
     Metric's methods are triggered on the following engine events:
 
     - :meth:`~ignite.metrics.metric.Metric.started` on every ``EPOCH_STARTED``
@@ -340,20 +431,24 @@
                 elif "cpu" not in result.device.type:
                     result = result.cpu()
 
             engine.state.metrics[name] = result
 
     def _check_usage(self, usage: Union[str, MetricUsage]) -> MetricUsage:
         if isinstance(usage, str):
-            if usage == EpochWise.usage_name:
-                usage = EpochWise()
-            elif usage == BatchWise.usage_name:
-                usage = BatchWise()
-            else:
-                raise ValueError(f"usage should be 'EpochWise.usage_name' or 'BatchWise.usage_name', get {usage}")
+            usages = [EpochWise, RunningEpochWise, BatchWise, RunningBatchWise, SingleEpochRunningBatchWise]
+            for usage_cls in usages:
+                if usage == usage_cls.usage_name:
+                    usage = usage_cls()
+                    break
+            if not isinstance(usage, MetricUsage):
+                raise ValueError(
+                    "Argument usage should be '(Running)EpochWise.usage_name' or "
+                    f"'((SingleEpoch)Running)BatchWise.usage_name', got {usage}"
+                )
         if not isinstance(usage, MetricUsage):
             raise TypeError(f"Unhandled usage type {type(usage)}")
         return usage
 
     def attach(self, engine: Engine, name: str, usage: Union[str, MetricUsage] = EpochWise()) -> None:
         """
         Attaches current metric to provided engine. On the end of engine's run, `engine.state.metrics` dictionary will
```

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/metrics_lambda.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/metrics_lambda.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/multilabel_confusion_matrix.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/multilabel_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/nlp/bleu.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/nlp/bleu.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/nlp/rouge.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/nlp/rouge.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/nlp/utils.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/precision.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/psnr.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/psnr.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/recall.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/root_mean_squared_error.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/ssim.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/metrics/top_k_categorical_accuracy.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/metrics/top_k_categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/ignite/utils.py` & `pytorch-ignite-0.5.0.dev20230630/ignite/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/pyproject.toml` & `pytorch-ignite-0.5.0.dev20230630/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/PKG-INFO` & `pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.dev20230629
+Version: 0.5.0.dev20230630
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.5.0.dev20230629/pytorch_ignite.egg-info/SOURCES.txt` & `pytorch-ignite-0.5.0.dev20230630/pytorch_ignite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/setup.cfg` & `pytorch-ignite-0.5.0.dev20230630/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230629/setup.py` & `pytorch-ignite-0.5.0.dev20230630/setup.py`

 * *Files identical despite different names*

