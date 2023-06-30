# Comparing `tmp/lightning-bolts-0.6.0.post1.tar.gz` & `tmp/lightning-bolts-0.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-bolts-0.6.0.post1.tar", last modified: Tue Nov  8 15:53:20 2022, max compression
+gzip compressed data, was "lightning-bolts-0.7.0rc0.tar", last modified: Thu Jun 29 15:23:05 2023, max compression
```

## Comparing `lightning-bolts-0.6.0.post1.tar` & `lightning-bolts-0.7.0rc0.tar`

### file list

```diff
@@ -1,232 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)    18856 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    11349 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      778 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6992 2022-11-08 15:53:20.925768 lightning-bolts-0.6.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5433 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.905767 lightning-bolts-0.6.0.post1/lightning_bolts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6992 2022-11-08 15:53:20.000000 lightning-bolts-0.6.0.post1/lightning_bolts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7583 2022-11-08 15:53:20.000000 lightning-bolts-0.6.0.post1/lightning_bolts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-08 15:53:20.000000 lightning-bolts-0.6.0.post1/lightning_bolts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-08 15:53:20.000000 lightning-bolts-0.6.0.post1/lightning_bolts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2022-11-08 15:53:20.000000 lightning-bolts-0.6.0.post1/lightning_bolts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-08 15:53:20.000000 lightning-bolts-0.6.0.post1/lightning_bolts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.905767 lightning-bolts-0.6.0.post1/pl_bolts/
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.905767 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/byol_updates.py
--rw-r--r--   0 runner    (1001) docker     (122)    11070 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/data_monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5628 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/knn_online.py
--rw-r--r--   0 runner    (1001) docker     (122)     5222 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/printing.py
--rw-r--r--   0 runner    (1001) docker     (122)     3453 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/sparseml.py
--rw-r--r--   0 runner    (1001) docker     (122)     6569 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/ssl_online.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/torch_ort.py
--rw-r--r--   0 runner    (1001) docker     (122)     3491 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.909767 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/verification/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/verification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5180 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/verification/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     9315 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/verification/batch_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.909767 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/vision/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6180 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/vision/confused_logit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3581 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/vision/image_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/callbacks/vision/sr_image_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.909767 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/
--rw-r--r--   0 runner    (1001) docker     (122)     1868 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4978 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/async_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (122)     3125 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/binary_emnist_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     3297 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/binary_mnist_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/cifar10_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     7337 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/cityscapes_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     7283 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/emnist_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)    10469 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/experience_source.py
--rw-r--r--   0 runner    (1001) docker     (122)     3411 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/fashion_mnist_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     9496 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/imagenet_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/kitti_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     3697 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/mnist_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6345 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/sklearn_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/sr_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     5443 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/ssl_imagenet_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)    11803 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/stl10_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6755 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/vision_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6557 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datamodules/vocdetection_datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.909767 lightning-bolts-0.6.0.post1/pl_bolts/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/array_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2608 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     8402 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/cifar10_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5969 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/dummy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2991 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/emnist_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     8205 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/imagenet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4044 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/kitti_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2792 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/mnist_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/sr_celeba_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/sr_dataset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/sr_mnist_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/sr_stl10_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4066 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/ssl_amdim_datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     4188 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/losses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/losses/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4328 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/losses/rl.py
--rw-r--r--   0 runner    (1001) docker     (122)    13036 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/losses/self_supervised_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/metrics/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/metrics/object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_ae/
--rw-r--r--   0 runner    (1001) docker     (122)      801 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_ae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5991 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_ae/basic_ae_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_vae/
--rw-r--r--   0 runner    (1001) docker     (122)      762 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7251 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_vae/basic_vae_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    10725 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/components/
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/components/_supported_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3314 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/components/torchvision_backbones.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (122)      223 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/faster_rcnn/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     6947 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/faster_rcnn/faster_rcnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/retinanet/
--rw-r--r--   0 runner    (1001) docker     (122)      213 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/retinanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1692 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/retinanet/backbones.py
--rw-r--r--   0 runner    (1001) docker     (122)     5534 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/retinanet/retinanet_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/yolo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9806 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/yolo/yolo_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    23885 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/yolo/yolo_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    26658 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/detection/yolo/yolo_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/basic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6570 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/basic/basic_gan_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/basic/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/dcgan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/dcgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3431 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/dcgan/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     7782 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/dcgan/dcgan_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.913767 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/pix2pix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4717 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/pix2pix/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     2890 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/pix2pix/pix2pix_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.917767 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/srgan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/srgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/srgan/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     9036 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/srgan/srgan_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     5564 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/gans/srgan/srresnet_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     3285 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/mnist_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.917767 lightning-bolts-0.6.0.post1/pl_bolts/models/regression/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5438 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/regression/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     6024 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/regression/logistic_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.917767 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/
--rw-r--r--   0 runner    (1001) docker     (122)      713 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11148 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/advantage_actor_critic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.917767 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6432 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/agents.py
--rw-r--r--   0 runner    (1001) docker     (122)     1772 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2208 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/distributions.py
--rw-r--r--   0 runner    (1001) docker     (122)     7103 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/gym_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)    10969 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15069 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/networks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/double_dqn_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    14822 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/dqn_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/dueling_dqn_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3583 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/noisy_dqn_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5174 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/per_dqn_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    14384 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/ppo_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    10482 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/reinforce_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    14677 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/sac_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/rl/vanilla_policy_gradient_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.917767 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/
--rw-r--r--   0 runner    (1001) docker     (122)     1335 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.917767 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/
--rw-r--r--   0 runner    (1001) docker     (122)      664 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11329 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/amdim_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     4447 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/networks.py
--rw-r--r--   0 runner    (1001) docker     (122)     8020 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.917767 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/byol/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/byol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8711 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/byol/byol_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/byol/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.917767 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/
--rw-r--r--   0 runner    (1001) docker     (122)      670 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1922 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/cpc_finetuner.py
--rw-r--r--   0 runner    (1001) docker     (122)     9129 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/cpc_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     6952 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/networks.py
--rw-r--r--   0 runner    (1001) docker     (122)    11053 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/moco/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/moco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/moco/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)    14452 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/moco/moco2_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     6506 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/moco/transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)    14117 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/resnets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simclr/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simclr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5327 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simclr/simclr_finetuner.py
--rw-r--r--   0 runner    (1001) docker     (122)    15309 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simclr/simclr_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     5333 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simclr/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simsiam/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simsiam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9386 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simsiam/simsiam_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     4654 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/ssl_finetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5052 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     4428 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/swav_finetuner.py
--rw-r--r--   0 runner    (1001) docker     (122)    19543 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/swav_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    11355 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/swav_resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5721 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/
--rw-r--r--   0 runner    (1001) docker     (122)      368 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/image_gpt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/image_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3672 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/image_gpt/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (122)     8603 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/image_gpt/igpt_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/pixel_cnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4978 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4092 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/models/vision/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/optimizers/
--rw-r--r--   0 runner    (1001) docker     (122)      229 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5466 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/optimizers/lars.py
--rw-r--r--   0 runner    (1001) docker     (122)     5694 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/optimizers/lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/transforms/dataset_normalizations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/transforms/self_supervised/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/transforms/self_supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/transforms/self_supervised/ssl_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/pl_bolts/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5522 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/arguments.py
--rw-r--r--   0 runner    (1001) docker     (122)      802 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/pretrained_weights.py
--rw-r--r--   0 runner    (1001) docker     (122)      514 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/self_supervised.py
--rw-r--r--   0 runner    (1001) docker     (122)     4135 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/semi_supervised.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/shaping.py
--rw-r--r--   0 runner    (1001) docker     (122)     3688 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/stability.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     1397 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/pl_bolts/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-08 15:53:20.921768 lightning-bolts-0.6.0.post1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/requirements/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/requirements/loggers.txt
--rw-r--r--   0 runner    (1001) docker     (122)      171 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/requirements/models.txt
--rw-r--r--   0 runner    (1001) docker     (122)      297 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      975 2022-11-08 15:53:20.925768 lightning-bolts-0.6.0.post1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     6205 2022-11-08 15:53:17.000000 lightning-bolts-0.6.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.902854 lightning-bolts-0.7.0rc0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/requirements/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/requirements/loggers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/requirements/models.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7788 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.898854 lightning-bolts-0.7.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.902854 lightning-bolts-0.7.0rc0/src/lightning_bolts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-29 15:23:05.000000 lightning-bolts-0.7.0rc0/src/lightning_bolts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-29 15:23:05.000000 lightning-bolts-0.7.0rc0/src/lightning_bolts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:23:05.000000 lightning-bolts-0.7.0rc0/src/lightning_bolts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:23:05.000000 lightning-bolts-0.7.0rc0/src/lightning_bolts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-29 15:23:05.000000 lightning-bolts-0.7.0rc0/src/lightning_bolts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 15:23:05.000000 lightning-bolts-0.7.0rc0/src/lightning_bolts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.902854 lightning-bolts-0.7.0rc0/src/pl_bolts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.902854 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/byol_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/data_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/knn_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/sparseml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/ssl_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/torch_ort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.906854 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/verification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/verification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/verification/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/verification/batch_gradient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.906854 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/vision/confused_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/vision/image_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/vision/sr_image_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.906854 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/async_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/binary_emnist_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/binary_mnist_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/cifar10_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/cityscapes_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/emnist_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/experience_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/fashion_mnist_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/imagenet_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/kitti_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/mnist_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/sklearn_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/sr_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/ssl_imagenet_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/stl10_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/vision_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/vocdetection_datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/array_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/cifar10_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/dummy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/emnist_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/imagenet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/kitti_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/mnist_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/sr_celeba_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/sr_dataset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/sr_mnist_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/sr_stl10_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/ssl_amdim_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/losses/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12930 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/losses/self_supervised_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/metrics/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_ae/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_ae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_ae/basic_ae_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_vae/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_vae/basic_vae_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/components/_supported_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/components/torchvision_backbones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/faster_rcnn/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/faster_rcnn/faster_rcnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.910854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/retinanet/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/retinanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/retinanet/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/retinanet/retinanet_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.914854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22268 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/darknet_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24288 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17893 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/target_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82191 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/torch_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30238 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/yolo_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.914854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.914854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/basic/basic_gan_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/basic/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.914854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/dcgan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/dcgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/dcgan/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/dcgan/dcgan_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.914854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/pix2pix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/pix2pix/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/pix2pix/pix2pix_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.914854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/srgan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/srgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/srgan/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/srgan/srgan_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/srgan/srresnet_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/mnist_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.914854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/regression/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/regression/logistic_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.914854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/advantage_actor_critic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/gym_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/double_dqn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14806 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/dqn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/dueling_dqn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/noisy_dqn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/per_dqn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/ppo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/reinforce_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14675 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/sac_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/vanilla_policy_gradient_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11162 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/amdim_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/byol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/byol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/byol/byol_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/byol/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/cpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/cpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/cpc/cpc_finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/cpc/cpc_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/cpc/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/moco/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/moco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/moco/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/moco/moco2_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/resnets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simclr/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simclr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simclr/simclr_finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simclr/simclr_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simsiam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simsiam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simsiam/simsiam_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/ssl_finetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.918854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/swav_finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19534 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/swav_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/swav_resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/image_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/image_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/image_gpt/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/image_gpt/igpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/pixel_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/src/pl_bolts/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/optimizers/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/optimizers/lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/dataset_normalizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/amdim_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/cpc_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/moco_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/simclr_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/ssl_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/swav_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:23:05.922854 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/pretrained_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/self_supervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/semi_supervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-29 15:23:03.000000 lightning-bolts-0.7.0rc0/src/pl_bolts/utils/warnings.py
```

### Comparing `lightning-bolts-0.6.0.post1/CHANGELOG.md` & `lightning-bolts-0.7.0rc0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,36 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [unReleased] - 2022-MM-DD
+
+### Added
+
+
+### Changed
+
+- Improved YOLO model includes YOLOv4, YOLOv5, and YOLOX networks and training algorithms ([#552](https://github.com/PyTorchLightning/pytorch-lightning-bolts/pull/817))
+
+
+- Bumped support of min python version to py3.8 ([#1021](https://github.com/PyTorchLightning/pytorch-lightning-bolts/pull/1021))
+
+
+### Deprecated
+
+
+### Removed
+
+
+### Fixed
+
+
+
 ## [0.6.0] - 2022-11-02
 
 ### Added
 
 - Updated SparseML callback for latest PyTorch Lightning ([#822](https://github.com/Lightning-AI/lightning-bolts/pull/822))
 - Updated torch version to v1.10.X ([#815](https://github.com/Lightning-AI/lightning-bolts/pull/815))
 - Dataset specific args method to CIFAR10, ImageNet, MNIST, and STL10 ([#890](https://github.com/Lightning-AI/lightning-bolts/pull/890))
```

### Comparing `lightning-bolts-0.6.0.post1/LICENSE` & `lightning-bolts-0.7.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/MANIFEST.in` & `lightning-bolts-0.7.0rc0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/PKG-INFO` & `lightning-bolts-0.7.0rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-bolts
-Version: 0.6.0.post1
+Version: 0.7.0rc0
 Summary: Lightning Bolts is a community contribution for ML researchers.
 Home-page: https://github.com/Lightning-AI/lightning-bolts
 Download-URL: https://github.com/PyTorchLightning/lightning-bolts
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PyTorchLightning/lightning-bolts/issues
@@ -17,53 +17,54 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: loggers
 Provides-Extra: models
 Provides-Extra: test
+Provides-Extra: typing
 Provides-Extra: extra
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/lightning-bolts/raw/0.6.0.post1/docs/source/_images/logos/bolts_logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/lightning-bolts/raw/0.7.0.rc0/docs/source/_images/logos/bolts_logo.png" width="400px">
 
 **Deep Learning components for extending PyTorch Lightning**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#install">Installation</a> •
   <a href="https://lightning-bolts.readthedocs.io/en/latest/">Latest Docs</a> •
-  <a href="https://lightning-bolts.readthedocs.io/en/0.6.0.post1">Stable Docs</a> •
+  <a href="https://lightning-bolts.readthedocs.io/en/0.7.0.rc0">Stable Docs</a> •
   <a href="#what-is-bolts">About</a> •
   <a href="#team">Community</a> •
-  <a href="https://www.pytorchlightning.ai/">Website</a> •
-  <a href="https://www.grid.ai/">Grid AI</a> •
+  <a href="https://www.lightning.ai/">Website</a> •
   <a href="#license">License</a>
 </p>
 
 [![PyPI Status](https://badge.fury.io/py/lightning-bolts.svg)](https://badge.fury.io/py/lightning-bolts)
 [![PyPI Status](https://pepy.tech/badge/lightning-bolts)](https://pepy.tech/project/lightning-bolts)
-[![Build Status](https://dev.azure.com/Lightning-AI/lightning%20Bolts/_apis/build/status/Lightning-AI.lightning-bolts?branchName=master)](https://dev.azure.com/Lightning-AI/lightning%20Bolts/_build?definitionId=31&_a=summary&repositoryFilter=13&branchFilter=4923%2C4923)
-[![codecov](https://codecov.io/gh/Lightning-AI/lightning-bolts/release/0.6.0.post1/graph/badge.svg?token=O8p0qhvj90)](https://codecov.io/gh/Lightning-AI/lightning-bolts)
+[![Build Status](https://dev.azure.com/Lightning-AI/compatibility/_apis/build/status%2Fprojects%2FLightning-Universe.Bolts?branchName=master)](https://dev.azure.com/Lightning-AI/compatibility/_build/latest?definitionId=51&branchName=master)
+[![codecov](https://codecov.io/gh/Lightning-Universe/lightning-bolts/release/0.7.0.rc0/graph/badge.svg?token=O8p0qhvj90)](https://codecov.io/gh/Lightning-Universe/lightning-bolts)
 
 [![Documentation Status](https://readthedocs.org/projects/lightning-bolts/badge/?version=latest)](https://lightning-bolts.readthedocs.io/en/latest/)
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/PytorchLightning/lightning-bolts/blob/master/LICENSE)
+[![DOI](https://zenodo.org/badge/250025410.svg)](https://zenodo.org/badge/latestdoi/250025410)
 
 </div>
 
 ______________________________________________________________________
 
 ## Getting Started
 
@@ -75,33 +76,28 @@
 
 <details>
   <summary>Other installations</summary>
 
 Install bleeding-edge (no guarantees)
 
 ```bash
-pip install git+https://github.com/PytorchLightning/lightning-bolts.git@master --upgrade
+pip install https://github.com/Lightning-Universe/lightning-bolts/archive/refs/heads/master.zip
 ```
 
 To install all optional dependencies
 
 ```bash
 pip install lightning-bolts["extra"]
 ```
 
 </details>
 
-## What is Bolts
+## What is Bolts?
 
-Bolts provides a variety of components to extend PyTorch Lightning such as callbacks & datasets, for applied research and production.
-
-## News
-
-- Sept 22: [Leverage Sparsity for Faster Inference with Lightning Flash and SparseML](https://devblog.pytorchlightning.ai/leverage-sparsity-for-faster-inference-with-lightning-flash-and-sparseml-cdda1165622b)
-- Aug 26: [Fine-tune Transformers Faster with Lightning Flash and Torch ORT](https://devblog.pytorchlightning.ai/fine-tune-transformers-faster-with-lightning-flash-and-torch-ort-ec2d53789dc3)
+Bolts package provides a variety of components to extend PyTorch Lightning, such as callbacks & datasets, for applied research and production.
 
 #### Example 1: Accelerate Lightning Training with the Torch ORT Callback
 
 Torch ORT converts your model into an optimized ONNX graph, speeding up training & inference when using NVIDIA or AMD GPUs. See the [documentation](https://lightning-bolts.readthedocs.io/en/latest/callbacks/torch_ort.html) for more details.
 
 ```python
 from pytorch_lightning import LightningModule, Trainer
@@ -143,25 +139,25 @@
 model = VisionModel()
 trainer = Trainer(gpus=1, callbacks=SparseMLCallback(recipe_path="recipe.yaml"))
 trainer.fit(model)
 ```
 
 ## Are specific research implementations supported?
 
-We'd like to encourage users to contribute general components that will help a broad range of problems, however components that help specifics domains will also be welcomed!
+We'd like to encourage users to contribute general components that will help a broad range of problems; however, components that help specific domains will also be welcomed!
 
-For example a callback to help train SSL models would be a great contribution, however the next greatest SSL model from your latest paper would be a good contribution to [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash).
+For example, a callback to help train SSL models would be a great contribution; however, the next greatest SSL model from your latest paper would be a good contribution to [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash).
 
-Use [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash) to train, predict and serve state-of-the-art models for applied research. We suggest looking at our [VISSL](https://lightning-flash.readthedocs.io/en/latest/integrations/vissl.html) Flash integration for SSL based tasks.
+Use [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash) to train, predict and serve state-of-the-art models for applied research. We suggest looking at our [VISSL](https://lightning-flash.readthedocs.io/en/latest/integrations/vissl.html) Flash integration for SSL-based tasks.
 
 ## Contribute!
 
 Bolts is supported by the PyTorch Lightning team and the PyTorch Lightning community!
 
 Join our Slack and/or read our [CONTRIBUTING](./.github/CONTRIBUTING.md) guidelines to get help becoming a contributor!
 
 ______________________________________________________________________
 
 ## License
 
 Please observe the Apache 2.0 license that is listed in this repository.
-In addition the Lightning framework is Patent Pending.
+In addition, the Lightning framework is Patent Pending.
```

### Comparing `lightning-bolts-0.6.0.post1/README.md` & `lightning-bolts-0.7.0rc0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 <p align="center">
   <a href="#install">Installation</a> •
   <a href="https://lightning-bolts.readthedocs.io/en/latest/">Latest Docs</a> •
   <a href="https://lightning-bolts.readthedocs.io/en/stable/">Stable Docs</a> •
   <a href="#what-is-bolts">About</a> •
   <a href="#team">Community</a> •
-  <a href="https://www.pytorchlightning.ai/">Website</a> •
-  <a href="https://www.grid.ai/">Grid AI</a> •
+  <a href="https://www.lightning.ai/">Website</a> •
   <a href="#license">License</a>
 </p>
 
 [![PyPI Status](https://badge.fury.io/py/lightning-bolts.svg)](https://badge.fury.io/py/lightning-bolts)
 [![PyPI Status](https://pepy.tech/badge/lightning-bolts)](https://pepy.tech/project/lightning-bolts)
-[![Build Status](https://dev.azure.com/Lightning-AI/lightning%20Bolts/_apis/build/status/Lightning-AI.lightning-bolts?branchName=master)](https://dev.azure.com/Lightning-AI/lightning%20Bolts/_build?definitionId=31&_a=summary&repositoryFilter=13&branchFilter=4923%2C4923)
-[![codecov](https://codecov.io/gh/Lightning-AI/lightning-bolts/branch/master/graph/badge.svg?token=O8p0qhvj90)](https://codecov.io/gh/Lightning-AI/lightning-bolts)
+[![Build Status](https://dev.azure.com/Lightning-AI/compatibility/_apis/build/status%2Fprojects%2FLightning-Universe.Bolts?branchName=master)](https://dev.azure.com/Lightning-AI/compatibility/_build/latest?definitionId=51&branchName=master)
+[![codecov](https://codecov.io/gh/Lightning-Universe/lightning-bolts/branch/master/graph/badge.svg?token=O8p0qhvj90)](https://codecov.io/gh/Lightning-Universe/lightning-bolts)
 
 [![Documentation Status](https://readthedocs.org/projects/lightning-bolts/badge/?version=latest)](https://lightning-bolts.readthedocs.io/en/latest/)
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/PytorchLightning/lightning-bolts/blob/master/LICENSE)
+[![DOI](https://zenodo.org/badge/250025410.svg)](https://zenodo.org/badge/latestdoi/250025410)
 
 </div>
 
 ______________________________________________________________________
 
 ## Getting Started
 
@@ -40,33 +40,28 @@
 
 <details>
   <summary>Other installations</summary>
 
 Install bleeding-edge (no guarantees)
 
 ```bash
-pip install git+https://github.com/PytorchLightning/lightning-bolts.git@master --upgrade
+pip install https://github.com/Lightning-Universe/lightning-bolts/archive/refs/heads/master.zip
 ```
 
 To install all optional dependencies
 
 ```bash
 pip install lightning-bolts["extra"]
 ```
 
 </details>
 
-## What is Bolts
+## What is Bolts?
 
-Bolts provides a variety of components to extend PyTorch Lightning such as callbacks & datasets, for applied research and production.
-
-## News
-
-- Sept 22: [Leverage Sparsity for Faster Inference with Lightning Flash and SparseML](https://devblog.pytorchlightning.ai/leverage-sparsity-for-faster-inference-with-lightning-flash-and-sparseml-cdda1165622b)
-- Aug 26: [Fine-tune Transformers Faster with Lightning Flash and Torch ORT](https://devblog.pytorchlightning.ai/fine-tune-transformers-faster-with-lightning-flash-and-torch-ort-ec2d53789dc3)
+Bolts package provides a variety of components to extend PyTorch Lightning, such as callbacks & datasets, for applied research and production.
 
 #### Example 1: Accelerate Lightning Training with the Torch ORT Callback
 
 Torch ORT converts your model into an optimized ONNX graph, speeding up training & inference when using NVIDIA or AMD GPUs. See the [documentation](https://lightning-bolts.readthedocs.io/en/latest/callbacks/torch_ort.html) for more details.
 
 ```python
 from pytorch_lightning import LightningModule, Trainer
@@ -108,25 +103,25 @@
 model = VisionModel()
 trainer = Trainer(gpus=1, callbacks=SparseMLCallback(recipe_path="recipe.yaml"))
 trainer.fit(model)
 ```
 
 ## Are specific research implementations supported?
 
-We'd like to encourage users to contribute general components that will help a broad range of problems, however components that help specifics domains will also be welcomed!
+We'd like to encourage users to contribute general components that will help a broad range of problems; however, components that help specific domains will also be welcomed!
 
-For example a callback to help train SSL models would be a great contribution, however the next greatest SSL model from your latest paper would be a good contribution to [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash).
+For example, a callback to help train SSL models would be a great contribution; however, the next greatest SSL model from your latest paper would be a good contribution to [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash).
 
-Use [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash) to train, predict and serve state-of-the-art models for applied research. We suggest looking at our [VISSL](https://lightning-flash.readthedocs.io/en/latest/integrations/vissl.html) Flash integration for SSL based tasks.
+Use [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash) to train, predict and serve state-of-the-art models for applied research. We suggest looking at our [VISSL](https://lightning-flash.readthedocs.io/en/latest/integrations/vissl.html) Flash integration for SSL-based tasks.
 
 ## Contribute!
 
 Bolts is supported by the PyTorch Lightning team and the PyTorch Lightning community!
 
 Join our Slack and/or read our [CONTRIBUTING](./.github/CONTRIBUTING.md) guidelines to get help becoming a contributor!
 
 ______________________________________________________________________
 
 ## License
 
 Please observe the Apache 2.0 license that is listed in this repository.
-In addition the Lightning framework is Patent Pending.
+In addition, the Lightning framework is Patent Pending.
```

### Comparing `lightning-bolts-0.6.0.post1/lightning_bolts.egg-info/PKG-INFO` & `lightning-bolts-0.7.0rc0/src/lightning_bolts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-bolts
-Version: 0.6.0.post1
+Version: 0.7.0rc0
 Summary: Lightning Bolts is a community contribution for ML researchers.
 Home-page: https://github.com/Lightning-AI/lightning-bolts
 Download-URL: https://github.com/PyTorchLightning/lightning-bolts
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PyTorchLightning/lightning-bolts/issues
@@ -17,53 +17,54 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: loggers
 Provides-Extra: models
 Provides-Extra: test
+Provides-Extra: typing
 Provides-Extra: extra
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/lightning-bolts/raw/0.6.0.post1/docs/source/_images/logos/bolts_logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/lightning-bolts/raw/0.7.0.rc0/docs/source/_images/logos/bolts_logo.png" width="400px">
 
 **Deep Learning components for extending PyTorch Lightning**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#install">Installation</a> •
   <a href="https://lightning-bolts.readthedocs.io/en/latest/">Latest Docs</a> •
-  <a href="https://lightning-bolts.readthedocs.io/en/0.6.0.post1">Stable Docs</a> •
+  <a href="https://lightning-bolts.readthedocs.io/en/0.7.0.rc0">Stable Docs</a> •
   <a href="#what-is-bolts">About</a> •
   <a href="#team">Community</a> •
-  <a href="https://www.pytorchlightning.ai/">Website</a> •
-  <a href="https://www.grid.ai/">Grid AI</a> •
+  <a href="https://www.lightning.ai/">Website</a> •
   <a href="#license">License</a>
 </p>
 
 [![PyPI Status](https://badge.fury.io/py/lightning-bolts.svg)](https://badge.fury.io/py/lightning-bolts)
 [![PyPI Status](https://pepy.tech/badge/lightning-bolts)](https://pepy.tech/project/lightning-bolts)
-[![Build Status](https://dev.azure.com/Lightning-AI/lightning%20Bolts/_apis/build/status/Lightning-AI.lightning-bolts?branchName=master)](https://dev.azure.com/Lightning-AI/lightning%20Bolts/_build?definitionId=31&_a=summary&repositoryFilter=13&branchFilter=4923%2C4923)
-[![codecov](https://codecov.io/gh/Lightning-AI/lightning-bolts/release/0.6.0.post1/graph/badge.svg?token=O8p0qhvj90)](https://codecov.io/gh/Lightning-AI/lightning-bolts)
+[![Build Status](https://dev.azure.com/Lightning-AI/compatibility/_apis/build/status%2Fprojects%2FLightning-Universe.Bolts?branchName=master)](https://dev.azure.com/Lightning-AI/compatibility/_build/latest?definitionId=51&branchName=master)
+[![codecov](https://codecov.io/gh/Lightning-Universe/lightning-bolts/release/0.7.0.rc0/graph/badge.svg?token=O8p0qhvj90)](https://codecov.io/gh/Lightning-Universe/lightning-bolts)
 
 [![Documentation Status](https://readthedocs.org/projects/lightning-bolts/badge/?version=latest)](https://lightning-bolts.readthedocs.io/en/latest/)
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/PytorchLightning/lightning-bolts/blob/master/LICENSE)
+[![DOI](https://zenodo.org/badge/250025410.svg)](https://zenodo.org/badge/latestdoi/250025410)
 
 </div>
 
 ______________________________________________________________________
 
 ## Getting Started
 
@@ -75,33 +76,28 @@
 
 <details>
   <summary>Other installations</summary>
 
 Install bleeding-edge (no guarantees)
 
 ```bash
-pip install git+https://github.com/PytorchLightning/lightning-bolts.git@master --upgrade
+pip install https://github.com/Lightning-Universe/lightning-bolts/archive/refs/heads/master.zip
 ```
 
 To install all optional dependencies
 
 ```bash
 pip install lightning-bolts["extra"]
 ```
 
 </details>
 
-## What is Bolts
+## What is Bolts?
 
-Bolts provides a variety of components to extend PyTorch Lightning such as callbacks & datasets, for applied research and production.
-
-## News
-
-- Sept 22: [Leverage Sparsity for Faster Inference with Lightning Flash and SparseML](https://devblog.pytorchlightning.ai/leverage-sparsity-for-faster-inference-with-lightning-flash-and-sparseml-cdda1165622b)
-- Aug 26: [Fine-tune Transformers Faster with Lightning Flash and Torch ORT](https://devblog.pytorchlightning.ai/fine-tune-transformers-faster-with-lightning-flash-and-torch-ort-ec2d53789dc3)
+Bolts package provides a variety of components to extend PyTorch Lightning, such as callbacks & datasets, for applied research and production.
 
 #### Example 1: Accelerate Lightning Training with the Torch ORT Callback
 
 Torch ORT converts your model into an optimized ONNX graph, speeding up training & inference when using NVIDIA or AMD GPUs. See the [documentation](https://lightning-bolts.readthedocs.io/en/latest/callbacks/torch_ort.html) for more details.
 
 ```python
 from pytorch_lightning import LightningModule, Trainer
@@ -143,25 +139,25 @@
 model = VisionModel()
 trainer = Trainer(gpus=1, callbacks=SparseMLCallback(recipe_path="recipe.yaml"))
 trainer.fit(model)
 ```
 
 ## Are specific research implementations supported?
 
-We'd like to encourage users to contribute general components that will help a broad range of problems, however components that help specifics domains will also be welcomed!
+We'd like to encourage users to contribute general components that will help a broad range of problems; however, components that help specific domains will also be welcomed!
 
-For example a callback to help train SSL models would be a great contribution, however the next greatest SSL model from your latest paper would be a good contribution to [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash).
+For example, a callback to help train SSL models would be a great contribution; however, the next greatest SSL model from your latest paper would be a good contribution to [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash).
 
-Use [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash) to train, predict and serve state-of-the-art models for applied research. We suggest looking at our [VISSL](https://lightning-flash.readthedocs.io/en/latest/integrations/vissl.html) Flash integration for SSL based tasks.
+Use [Lightning Flash](https://github.com/PyTorchLightning/lightning-flash) to train, predict and serve state-of-the-art models for applied research. We suggest looking at our [VISSL](https://lightning-flash.readthedocs.io/en/latest/integrations/vissl.html) Flash integration for SSL-based tasks.
 
 ## Contribute!
 
 Bolts is supported by the PyTorch Lightning team and the PyTorch Lightning community!
 
 Join our Slack and/or read our [CONTRIBUTING](./.github/CONTRIBUTING.md) guidelines to get help becoming a contributor!
 
 ______________________________________________________________________
 
 ## License
 
 Please observe the Apache 2.0 license that is listed in this repository.
-In addition the Lightning framework is Patent Pending.
+In addition, the Lightning framework is Patent Pending.
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/__about__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 
-__version__ = "0.6.0.post1"
+__version__ = "0.7.0.rc0"
 __author__ = "Lightning AI et al."
 __author_email__ = "pytorch@lightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2020-{time.strftime('%Y')}, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/lightning-bolts"
 __docs__ = "Lightning Bolts is a community contribution for ML researchers."
 __long_doc__ = """
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/byol_updates.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/byol_updates.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/data_monitor.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/data_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 from typing import Any, Dict, List, Optional, Sequence, Union
 
 import numpy as np
 import torch
 from pytorch_lightning import Callback, LightningModule, Trainer
-from pytorch_lightning.loggers import LightningLoggerBase, TensorBoardLogger, WandbLogger
+from pytorch_lightning.loggers import TensorBoardLogger, WandbLogger
 from pytorch_lightning.utilities import rank_zero_warn
 from pytorch_lightning.utilities.apply_func import apply_to_collection
 from torch import Tensor, nn
 from torch.nn import Module
 from torch.utils.hooks import RemovableHandle
 
 from pl_bolts.utils import _WANDB_AVAILABLE
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
+# Backward compatibility for Lightning Logger
+try:
+    from pytorch_lightning.loggers import Logger
+except ImportError:
+    from pytorch_lightning.loggers import LightningLoggerBase as Logger
+
 if _WANDB_AVAILABLE:
     import wandb
 else:  # pragma: no cover
     warn_missing_pkg("wandb")
 
 
 @under_review()
 class DataMonitorBase(Callback):
-
     supported_loggers = (
         TensorBoardLogger,
         WandbLogger,
     )
 
-    def __init__(self, log_every_n_steps: int = None):
+    def __init__(self, log_every_n_steps: int = None) -> None:
         """Base class for monitoring data histograms in a LightningModule. This requires a logger configured in the
         Trainer, otherwise no data is logged. The specific class that inherits from this base defines what data
         gets collected.
 
         Args:
             log_every_n_steps: The interval at which histograms should be logged. This defaults to the
                 interval defined in the Trainer. Use this to override the Trainer default.
@@ -93,39 +98,38 @@
 
         if isinstance(logger, WandbLogger):
             if not _WANDB_AVAILABLE:  # pragma: no cover
                 raise ModuleNotFoundError("You want to use `wandb` which is not installed yet.")
 
             logger.experiment.log(data={name: wandb.Histogram(tensor)}, commit=False)
 
-    def _is_logger_available(self, logger: LightningLoggerBase) -> bool:
+    def _is_logger_available(self, logger: Logger) -> bool:
         available = True
         if not logger:
             rank_zero_warn("Cannot log histograms because Trainer has no logger.")
             available = False
         if not isinstance(logger, self.supported_loggers):
             rank_zero_warn(
                 f"{self.__class__.__name__} does not support logging with {logger.__class__.__name__}."
-                f" Supported loggers are: {', '.join(map(lambda x: str(x.__name__), self.supported_loggers))}"
+                f" Supported loggers are: {', '.join((str(x.__name__) for x in self.supported_loggers))}"
             )
             available = False
         return available
 
 
 @under_review()
 class ModuleDataMonitor(DataMonitorBase):
-
     GROUP_NAME_INPUT = "input"
     GROUP_NAME_OUTPUT = "output"
 
     def __init__(
         self,
         submodules: Optional[Union[bool, List[str]]] = None,
         log_every_n_steps: int = None,
-    ):
+    ) -> None:
         """
         Args:
             submodules: If `True`, logs the in- and output histograms of every submodule in the
                 LightningModule, including the root module itself.
                 This parameter can also take a list of names of specifc submodules (see example below).
                 Default: `None`, logs only the in- and output of the root module.
             log_every_n_steps: The interval at which histograms should be logged. This defaults to the
@@ -189,24 +193,23 @@
         output_group_name = f"{self.GROUP_NAME_OUTPUT}/{module_name}" if module_name else self.GROUP_NAME_OUTPUT
 
         def hook(_: Module, inp: Sequence, out: Sequence) -> None:
             inp = inp[0] if len(inp) == 1 else inp
             self.log_histograms(inp, group=input_group_name)
             self.log_histograms(out, group=output_group_name)
 
-        handle = module.register_forward_hook(hook)
-        return handle
+        # handler
+        return module.register_forward_hook(hook)
 
 
 @under_review()
 class TrainingDataMonitor(DataMonitorBase):
-
     GROUP_NAME = "training_step"
 
-    def __init__(self, log_every_n_steps: int = None):
+    def __init__(self, log_every_n_steps: int = None) -> None:
         """Callback that logs the histogram of values in the batched data passed to `training_step`.
 
         Args:
             log_every_n_steps: The interval at which histograms should be logged. This defaults to the
                 interval defined in the Trainer. Use this to override the Trainer default.
 
         Example:
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/knn_online.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/knn_online.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Tuple, Union
 
 import torch
 from pytorch_lightning import Callback, LightningModule, Trainer
 from pytorch_lightning.accelerators import Accelerator
 from torch import Tensor
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class KNNOnlineEvaluator(Callback):
     """Weighted KNN online evaluator for self-supervised learning.
@@ -52,33 +52,33 @@
             feature_bank: (N, D) the bank of N known vectors with dim=D
             target_bank: (N, ) the bank of N known vectors' labels
 
         Returns:
             (B, ) the predicted labels of B query vectors
         """
 
-        B = query_feature.shape[0]
+        dim_b = query_feature.shape[0]
 
         # compute cos similarity between each feature vector and feature bank ---> [B, N]
         sim_matrix = query_feature @ feature_bank.T
         # [B, K]
         sim_weight, sim_indices = sim_matrix.topk(k=self.k, dim=-1)
         # [B, K]
-        sim_labels = torch.gather(target_bank.expand(B, -1), dim=-1, index=sim_indices)
+        sim_labels = torch.gather(target_bank.expand(dim_b, -1), dim=-1, index=sim_indices)
         sim_weight = (sim_weight / self.temperature).exp()
 
         # counts for each class
-        one_hot_label = torch.zeros(B * self.k, self.num_classes, device=sim_labels.device)
+        one_hot_label = torch.zeros(dim_b * self.k, self.num_classes, device=sim_labels.device)
         # [B*K, C]
         one_hot_label = one_hot_label.scatter(dim=-1, index=sim_labels.view(-1, 1), value=1.0)
         # weighted score ---> [B, C]
-        pred_scores = torch.sum(one_hot_label.view(B, -1, self.num_classes) * sim_weight.unsqueeze(dim=-1), dim=1)
+        pred_scores = torch.sum(one_hot_label.view(dim_b, -1, self.num_classes) * sim_weight.unsqueeze(dim=-1), dim=1)
 
-        pred_labels = pred_scores.argsort(dim=-1, descending=True)
-        return pred_labels
+        # pred_labels
+        return pred_scores.argsort(dim=-1, descending=True)
 
     def to_device(self, batch: Tensor, device: Union[str, torch.device]) -> Tuple[Tensor, Tensor]:
         # get the labeled batch
         if self.dataset == "stl10":
             labeled_batch = batch[1]
             batch = labeled_batch
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/printing.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/printing.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,16 @@
     marked_values = {}
     s = "│".join(f"{{{h}:{pad}{fcode}}}" for h, pad, fcode in zip_longest(marked_keys, pads, fcodes))
     lines = [headline, underline]
     for d in dicts:
         none_keys = [k for k, v in d.items() if v is None]
         if skip_none_lines and none_keys:
             continue
-        elif replace_values:
-            for k in d.keys():
+        if replace_values:
+            for k in d:
                 if k in replace_values and d[k] in replace_values[k]:
                     d[k] = replace_values[k][d[k]]
                 if d[k] is None:
                     raise ValueError(f"bad or no mapping for key '{k}' is None. Use skip or change replace mapping.")
         elif none_keys:
             raise ValueError(f"keys {none_keys} are None in {d}. Do skip or use replace mapping.")
         for h in convert_headers:
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/sparseml.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/sparseml.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """Enables SparseML aware training. Requires a recipe to run during training.
 
     Args:
         recipe_path: Path to a SparseML compatible yaml recipe.
             More information at https://docs.neuralmagic.com/sparseml/source/recipes.html
     """
 
-    def __init__(self, recipe_path: str):
+    def __init__(self, recipe_path: str) -> None:
         if not _SPARSEML_AVAILABLE:
             if not _PL_GREATER_EQUAL_1_4_5:
                 raise MisconfigurationException("SparseML requires PyTorch Lightning 1.4.5 or greater.")
             if not _TORCH_MAX_VERSION_SPARSEML:
                 raise MisconfigurationException("SparseML requires PyTorch version lower than 1.11.0.")
             raise MisconfigurationException("SparseML has not be installed, install with pip install sparseml")
         self.manager = ScheduledModifierManager.from_yaml(recipe_path)
@@ -61,15 +61,15 @@
     @staticmethod
     def export_to_sparse_onnx(
         model: LightningModule, output_dir: str, sample_batch: Optional[torch.Tensor] = None, **export_kwargs: Any
     ) -> None:
         """Exports the model to ONNX format."""
         with model._prevent_trainer_and_dataloaders_deepcopy():
             exporter = ModuleExporter(model, output_dir=output_dir)
-            sample_batch = sample_batch if sample_batch is not None else model.example_input_array
+            sample_batch = sample_batch if sample_batch is not None else model.example_input_array  # type: ignore[assignment] # noqa: E501
             if sample_batch is None:
                 raise MisconfigurationException(
                     "To export the model, a sample batch must be passed via "
                     "``SparseMLCallback.export_to_sparse_onnx(model, output_dir, sample_batch=sample_batch)`` "
                     "or an ``example_input_array`` property within the LightningModule"
                 )
             exporter.export_onnx(sample_batch=sample_batch, **export_kwargs)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/ssl_online.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/ssl_online.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import contextmanager
 from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import torch
 from pytorch_lightning import Callback, LightningModule, Trainer
 from pytorch_lightning.utilities import rank_zero_warn
 from torch import Tensor, nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 from torch.optim import Optimizer
 from torchmetrics.functional import accuracy
 
 from pl_bolts.models.self_supervised.evaluator import SSLEvaluator
 from pl_bolts.utils.stability import under_review
 
 
@@ -36,15 +36,15 @@
     def __init__(
         self,
         z_dim: int,
         drop_p: float = 0.2,
         hidden_dim: Optional[int] = None,
         num_classes: Optional[int] = None,
         dataset: Optional[str] = None,
-    ):
+    ) -> None:
         """
         Args:
             z_dim: Representation dimension
             drop_p: Dropout probability
             hidden_dim: Hidden dimension for the fine-tune MLP
         """
         super().__init__()
@@ -81,21 +81,21 @@
         accel = (
             trainer.accelerator_connector
             if hasattr(trainer, "accelerator_connector")
             else trainer._accelerator_connector
         )
         if accel.is_distributed:
             if accel.use_ddp:
-                from torch.nn.parallel import DistributedDataParallel as DDP
+                from torch.nn.parallel import DistributedDataParallel
 
-                self.online_evaluator = DDP(self.online_evaluator, device_ids=[pl_module.device])
+                self.online_evaluator = DistributedDataParallel(self.online_evaluator, device_ids=[pl_module.device])
             elif accel.use_dp:
-                from torch.nn.parallel import DataParallel as DP
+                from torch.nn.parallel import DataParallel
 
-                self.online_evaluator = DP(self.online_evaluator, device_ids=[pl_module.device])
+                self.online_evaluator = DataParallel(self.online_evaluator, device_ids=[pl_module.device])
             else:
                 rank_zero_warn(
                     "Does not support this type of distributed accelerator. The online evaluator will not sync."
                 )
 
         self.optimizer = torch.optim.Adam(self.online_evaluator.parameters(), lr=1e-4)
 
@@ -119,24 +119,23 @@
         return x, y
 
     def shared_step(
         self,
         pl_module: LightningModule,
         batch: Sequence,
     ):
-        with torch.no_grad():
-            with set_training(pl_module, False):
-                x, y = self.to_device(batch, pl_module.device)
-                representations = pl_module(x).flatten(start_dim=1)
+        with torch.no_grad(), set_training(pl_module, False):
+            x, y = self.to_device(batch, pl_module.device)
+            representations = pl_module(x).flatten(start_dim=1)
 
         # forward pass
         mlp_logits = self.online_evaluator(representations)  # type: ignore[operator]
         mlp_loss = F.cross_entropy(mlp_logits, y)
 
-        acc = accuracy(mlp_logits.softmax(-1), y)
+        acc = accuracy(mlp_logits.softmax(-1), y, task="multiclass", num_classes=self.num_classes)
 
         return acc, mlp_loss
 
     def on_train_batch_end(
         self,
         trainer: Trainer,
         pl_module: LightningModule,
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/torch_ort.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/torch_ort.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/variational.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/variational.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self,
         interpolate_epoch_interval: int = 20,
         range_start: int = -5,
         range_end: int = 5,
         steps: int = 11,
         num_samples: int = 2,
         normalize: bool = True,
-    ):
+    ) -> None:
         """
         Args:
             interpolate_epoch_interval: default 20
             range_start: default -5
             range_end: default 5
             steps: number of step between start and end
             num_samples: default 2
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/verification/base.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/verification/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class VerificationBase:
     """Base class for model verification.
 
-    All verifications should run with any :class:`torch.nn.Module` unless otherwise stated.
+    All verifications should run with any
+    :class: `torch.nn.Module` unless otherwise stated.
     """
 
-    def __init__(self, model: nn.Module):
+    def __init__(self, model: nn.Module) -> None:
         """
         Arguments:
             model: The model to run verification for.
         """
         super().__init__()
         self.model = model
 
@@ -96,19 +97,16 @@
             warn: If ``True``, prints a warning message when verification fails. Default: ``True``.
             error: If ``True``, prints an error message when verification fails. Default: ``False``.
         """
         self._raise_warning = warn
         self._raise_error = error
 
     def message(self, *args: Any, **kwargs: Any) -> str:
-        """
-        The message to be printed when the model does not pass the verification.
-        If the message for warning and error differ, override the
-        :meth:`warning_message` and :meth:`error_message`
-        methods directly.
+        """The message to be printed when the model does not pass the verification. If the message for warning and
+        error differ, override the :meth:`warning_message` and :meth:`error_message` methods directly.
 
         Arguments:
             *args: Any positional arguments that are needed to construct the message.
             **kwargs: Any keyword arguments that are needed to construct the message.
 
         Returns:
             The message as a string.
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/verification/batch_gradient.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/verification/batch_gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     def __init__(
         self,
         input_mapping: Optional[Callable] = None,
         output_mapping: Optional[Callable] = None,
         sample_idx: int = 0,
         **kwargs: Any,
-    ):
+    ) -> None:
         """
         Arguments:
             input_mapping: An optional input mapping that returns all batched tensors in a input collection.
                 See :meth:`BatchGradientVerification.check` for more information.
             output_mapping: An optional output mapping that combines all batched tensors in the output
                 collection into one big batch. See :meth:`BatchGradientVerification.check` for more information.
             sample_idx: The index of the batch sample to run the test for.
@@ -110,20 +110,19 @@
         """
         super().__init__(**kwargs)
         self._input_mapping = input_mapping
         self._output_mapping = output_mapping
         self._sample_idx = sample_idx
 
     def message(self, *args: Any, **kwargs: Any) -> str:
-        message = (
+        return (
             "Your model is mixing data across the batch dimension."
             " This can lead to wrong gradient updates in the optimizer."
             " Check the operations that reshape and permute tensor dimensions in your model."
         )
-        return message
 
     def on_train_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
         verification = BatchGradientVerification(pl_module)
         result = verification.check(
             input_array=pl_module.example_input_array,
             input_mapping=self._input_mapping,
             output_mapping=self._output_mapping,
@@ -185,16 +184,15 @@
     """
     if isinstance(data, Tensor):
         return data
 
     batches = default_input_mapping(data)
     # cannot use .flatten(1) because of tensors with shape (B, )
     batches = [batch.view(batch.size(0), -1).float() for batch in batches]
-    combined = torch.cat(batches, 1)  # combined batch has shape (B, N)
-    return combined
+    return torch.cat(batches, 1)  # combined batch has shape (B, N)
 
 
 @under_review()
 def collect_tensors(data: Any) -> List[Tensor]:
     """Filters all tensors in a collection and returns them in a list."""
     tensors = []
 
@@ -215,15 +213,14 @@
     Args:
         model: A model which has layers that need to be set to eval mode.
         layer_types: The list of class objects for which all layers of that type will be set to eval mode.
     """
     to_revert = []
     try:
         for module in model.modules():
-            if isinstance(module, tuple(layer_types)):
-                if module.training:
-                    module.eval()
-                    to_revert.append(module)
+            if isinstance(module, tuple(layer_types)) and module.training:
+                module.eval()
+                to_revert.append(module)
         yield
     finally:
         for module in to_revert:
             module.train()
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/vision/confused_logit.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/vision/confused_logit.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def __init__(
         self,
         top_k: int,
         min_logit_value: float = 5.0,
         logging_batch_interval: int = 20,
         max_logit_difference: float = 0.1,
-    ):
+    ) -> None:
         """
         Args:
             top_k: How many "offending" images we should plot
             projection_factor: How much to multiply the input image to make it look more like this logit label
             min_logit_value: Only consider logit values above this threshold
             logging_batch_interval: How frequently to inspect/potentially plot something
             max_logit_difference: When the top 2 logits are within this threshold we consider them confused
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/vision/image_generation.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/vision/image_generation.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/callbacks/vision/sr_image_logger.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/callbacks/vision/sr_image_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple
 
 import pytorch_lightning as pl
 import torch
-import torch.nn.functional as F
+import torch.nn.functional as F  # noqa: N812
 from pytorch_lightning import Callback
 
 from pl_bolts.utils import _TORCHVISION_AVAILABLE
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _TORCHVISION_AVAILABLE:
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/async_dataloader.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/async_dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import re
 from queue import Queue
 from threading import Thread
 from typing import Any, Optional, Union
 
 import torch
 from torch import Tensor
-from torch._six import string_classes
 from torch.utils.data import DataLoader, Dataset
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class AsynchronousLoader:
@@ -81,15 +80,15 @@
             if elem_type.__name__ == "ndarray" and self.np_str_obj_array_pattern.search(sample.dtype.str) is not None:
                 return self.load_instance(sample)
             return self.load_instance(torch.as_tensor(sample))
         elif isinstance(sample, container_abcs.Mapping):
             return {key: self.load_instance(sample[key]) for key in sample}
         elif isinstance(sample, tuple) and hasattr(sample, "_fields"):  # namedtuple
             return elem_type(*(self.load_instance(d) for d in sample))
-        elif isinstance(sample, container_abcs.Sequence) and not isinstance(sample, string_classes):
+        elif isinstance(sample, container_abcs.Sequence) and not isinstance(sample, str):
             return [self.load_instance(s) for s in sample]
         else:
             return sample
 
     def __iter__(self) -> "AsynchronousLoader":
         # We don't want to run the thread more than once
         # Start a new thread if we are at the beginning of a new epoch, and our current worker is dead
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/binary_emnist_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/binary_emnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/binary_mnist_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/binary_mnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/cifar10_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/cifar10_datamodule.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,13 +175,13 @@
             num_samples: number of examples per selected class/label
             labels: list selected CIFAR10 classes/labels
         """
         super().__init__(data_dir, val_split, num_workers, *args, **kwargs)
 
         self.num_samples = num_samples  # type: ignore[misc]
         self.labels = sorted(labels) if labels is not None else set(range(10))
-        self.extra_args = dict(num_samples=self.num_samples, labels=self.labels)
+        self.extra_args = {"num_samples": self.num_samples, "labels": self.labels}
 
     @property
     def num_classes(self) -> int:
         """Return number of classes."""
         return len(self.labels)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/cityscapes_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/cityscapes_datamodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,23 +138,22 @@
             target_type=self.target_type,
             mode=self.quality_mode,
             transform=transforms,
             target_transform=target_transforms,
             **self.extra_args,
         )
 
-        loader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def val_dataloader(self) -> DataLoader:
         """Cityscapes val set."""
         transforms = self.val_transforms or self._default_transforms()
         target_transforms = self.target_transforms or self._default_target_transforms()
 
         dataset = Cityscapes(
@@ -163,23 +162,22 @@
             target_type=self.target_type,
             mode=self.quality_mode,
             transform=transforms,
             target_transform=target_transforms,
             **self.extra_args,
         )
 
-        loader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
             drop_last=self.drop_last,
         )
-        return loader
 
     def test_dataloader(self) -> DataLoader:
         """Cityscapes test set."""
         transforms = self.test_transforms or self._default_transforms()
         target_transforms = self.target_transforms or self._default_target_transforms()
 
         dataset = Cityscapes(
@@ -187,33 +185,28 @@
             split="test",
             target_type=self.target_type,
             mode=self.quality_mode,
             transform=transforms,
             target_transform=target_transforms,
             **self.extra_args,
         )
-        loader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def _default_transforms(self) -> Callable:
-        cityscapes_transforms = transform_lib.Compose(
+        return transform_lib.Compose(
             [
                 transform_lib.ToTensor(),
                 transform_lib.Normalize(
                     mean=[0.28689554, 0.32513303, 0.28389177], std=[0.18696375, 0.19017339, 0.18720214]
                 ),
             ]
         )
-        return cityscapes_transforms
 
     def _default_target_transforms(self) -> Callable:
-        cityscapes_target_transforms = transform_lib.Compose(
-            [transform_lib.ToTensor(), transform_lib.Lambda(lambda t: t.squeeze())]
-        )
-        return cityscapes_target_transforms
+        return transform_lib.Compose([transform_lib.ToTensor(), transform_lib.Lambda(lambda t: t.squeeze())])
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/emnist_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/emnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/experience_source.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/experience_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,15 @@
     generated is defined the Lightning model itself
     """
 
     def __init__(self, generate_batch: Callable) -> None:
         self.generate_batch = generate_batch
 
     def __iter__(self) -> Iterator:
-        iterator = self.generate_batch()
-        return iterator
+        return self.generate_batch()  # iterator
 
 
 # Experience Sources
 @under_review()
 class BaseExperienceSource(ABC):
     """Simplest form of the experience source."""
 
@@ -99,15 +98,14 @@
         """
         while True:
             # get actions for all envs
             actions = self.env_actions(device)
 
             # step through each env
             for env_idx, (env, action) in enumerate(zip(self.pool, actions)):
-
                 exp = self.env_step(env_idx, env, action)
                 history = self.histories[env_idx]
                 history.append(exp)
                 self.states[env_idx] = exp.new_state
 
                 self.update_history_queue(env_idx, exp, history)
 
@@ -188,17 +186,15 @@
             Experience tuple
         """
         next_state, r, is_done, _ = env.step(action[0])
 
         self.cur_rewards[env_idx] += r
         self.cur_steps[env_idx] += 1
 
-        exp = Experience(state=self.states[env_idx], action=action[0], reward=r, done=is_done, new_state=next_state)
-
-        return exp
+        return Experience(state=self.states[env_idx], action=action[0], reward=r, done=is_done, new_state=next_state)
 
     def update_env_stats(self, env_idx: int) -> None:
         """To be called at the end of the history tail generation during the termination state. Updates the stats
         tracked for all environments.
 
         Args:
             env_idx: index of the environment used to update stats
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/fashion_mnist_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/fashion_mnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/imagenet_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/imagenet_datamodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,26 +124,26 @@
         self._verify_splits(self.data_dir, "val")
 
         for split in ["train", "val"]:
             files = os.listdir(os.path.join(self.data_dir, split))
             if "meta.bin" not in files:
                 raise FileNotFoundError(
                     """
-                no meta.bin present. Imagenet is no longer automatically downloaded by PyTorch.
-                To get imagenet:
-                1. download yourself from http://www.image-net.org/challenges/LSVRC/2012/downloads
-                2. download the devkit (ILSVRC2012_devkit_t12.tar.gz)
-                3. generate the meta.bin file using the devkit
-                4. copy the meta.bin file into both train and val split folders
-
-                To generate the meta.bin do the following:
-
-                from pl_bolts.datasets import UnlabeledImagenet
-                path = '/path/to/folder/with/ILSVRC2012_devkit_t12.tar.gz/'
-                UnlabeledImagenet.generate_meta_bins(path)
+    no meta.bin present. Imagenet is no longer automatically downloaded by PyTorch.
+    To get imagenet:
+
+    1. download the devkit (https://image-net.org/data/ILSVRC/2012/ILSVRC2012_devkit_t12.tar.gz)
+    2. generate the meta.bin file using the devkit
+    3. copy the meta.bin file into both train and val split folders
+
+    To generate the meta.bin do the following:
+
+    from pl_bolts.datasets import UnlabeledImagenet
+    path = '/path/to/folder/with/ILSVRC2012_devkit_t12.tar.gz/'
+    UnlabeledImagenet.generate_meta_bins(path)
                 """
                 )
 
     def train_dataloader(self) -> DataLoader:
         """Uses the train split of imagenet2012 and puts away a portion of it for the validation split."""
         transforms = self.train_transform() if self.train_transforms is None else self.train_transforms
 
@@ -220,25 +220,23 @@
                 transform_lib.ToTensor(),
                 transform_lib.Normalize(
                     mean=[0.485, 0.456, 0.406],
                     std=[0.229, 0.224, 0.225]
                 ),
             ])
         """
-        preprocessing = transform_lib.Compose(
+        return transform_lib.Compose(
             [
                 transform_lib.RandomResizedCrop(self.image_size),
                 transform_lib.RandomHorizontalFlip(),
                 transform_lib.ToTensor(),
                 imagenet_normalization(),
             ]
         )
 
-        return preprocessing
-
     def val_transform(self) -> Callable:
         """The standard imagenet transforms for validation.
 
         .. code-block:: python
 
             transform_lib.Compose([
                 transform_lib.Resize(self.image_size + 32),
@@ -247,23 +245,22 @@
                 transform_lib.Normalize(
                     mean=[0.485, 0.456, 0.406],
                     std=[0.229, 0.224, 0.225]
                 ),
             ])
         """
 
-        preprocessing = transform_lib.Compose(
+        return transform_lib.Compose(
             [
                 transform_lib.Resize(self.image_size + 32),
                 transform_lib.CenterCrop(self.image_size),
                 transform_lib.ToTensor(),
                 imagenet_normalization(),
             ]
         )
-        return preprocessing
 
     @staticmethod
     def add_dataset_specific_args(parent_parser: ArgumentParser) -> ArgumentParser:
         parser = ArgumentParser(parents=[parent_parser], add_help=False)
 
         parser.add_argument("--data_dir", type=str, default=".")
         parser.add_argument("--num_workers", type=int, default=0)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/kitti_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/kitti_datamodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     from torchvision import transforms
 else:  # pragma: no cover
     warn_missing_pkg("torchvision")
 
 
 @under_review()
 class KittiDataModule(LightningDataModule):
-
     name = "kitti"
 
     def __init__(
         self,
         data_dir: Optional[str] = None,
         val_split: float = 0.2,
         test_split: float = 0.1,
@@ -91,49 +90,45 @@
         train_len = len(kitti_dataset) - val_len - test_len
 
         self.trainset, self.valset, self.testset = random_split(
             kitti_dataset, lengths=[train_len, val_len, test_len], generator=torch.Generator().manual_seed(self.seed)
         )
 
     def train_dataloader(self) -> DataLoader:
-        loader = DataLoader(
+        return DataLoader(
             self.trainset,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def val_dataloader(self) -> DataLoader:
-        loader = DataLoader(
+        return DataLoader(
             self.valset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def test_dataloader(self) -> DataLoader:
-        loader = DataLoader(
+        return DataLoader(
             self.testset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def _default_transforms(self) -> Callable:
-        kitti_transforms = transforms.Compose(
+        return transforms.Compose(
             [
                 transforms.ToTensor(),
                 transforms.Normalize(
                     mean=[0.35675976, 0.37380189, 0.3764753], std=[0.32064945, 0.32098866, 0.32325324]
                 ),
             ]
         )
-        return kitti_transforms
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/mnist_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/mnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/sklearn_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/sklearn_datamodule.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,61 +8,66 @@
 from pl_bolts.utils import _SKLEARN_AVAILABLE
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _SKLEARN_AVAILABLE:
     from sklearn.utils import shuffle as sk_shuffle
 else:  # pragma: no cover
-    warn_missing_pkg("sklearn")
+    warn_missing_pkg("sklearn", pypi_name="scikit-learn")
 
 
 @under_review()
 class SklearnDataset(Dataset):
     """Mapping between numpy (or sklearn) datasets to PyTorch datasets.
 
+    Args:
+        X: Numpy ndarray
+        y: Numpy ndarray
+        x_transform: Any transform that works with Numpy arrays
+        y_transform: Any transform that works with Numpy arrays
+
     Example:
         >>> from sklearn.datasets import load_diabetes
         >>> from pl_bolts.datamodules import SklearnDataset
         ...
         >>> X, y = load_diabetes(return_X_y=True)
         >>> dataset = SklearnDataset(X, y)
         >>> len(dataset)
         442
     """
 
-    def __init__(self, X: np.ndarray, y: np.ndarray, X_transform: Any = None, y_transform: Any = None) -> None:
-        """
-        Args:
-            X: Numpy ndarray
-            y: Numpy ndarray
-            X_transform: Any transform that works with Numpy arrays
-            y_transform: Any transform that works with Numpy arrays
-        """
+    def __init__(
+        self,
+        X: np.ndarray,  # noqa: N803
+        y: np.ndarray,
+        x_transform: Any = None,
+        y_transform: Any = None,
+    ) -> None:
         super().__init__()
-        self.X = X
-        self.Y = y
-        self.X_transform = X_transform
-        self.y_transform = y_transform
+        self.data = X
+        self.labels = y
+        self.data_transform = x_transform
+        self.labels_transform = y_transform
 
     def __len__(self) -> int:
-        return len(self.X)
+        return len(self.data)
 
     def __getitem__(self, idx) -> Tuple[np.ndarray, np.ndarray]:
-        x = self.X[idx].astype(np.float32)
-        y = self.Y[idx]
+        x = self.data[idx].astype(np.float32)
+        y = self.labels[idx]
 
         # Do not convert integer to float for classification data
         if not ((y.dtype == np.int32) or (y.dtype == np.int64)):
             y = y.astype(np.float32)
 
-        if self.X_transform:
-            x = self.X_transform(x)
+        if self.data_transform:
+            x = self.data_transform(x)
 
-        if self.y_transform:
-            y = self.y_transform(y)
+        if self.labels_transform:
+            y = self.labels_transform(y)
 
         return x, y
 
 
 @under_review()
 class SklearnDataModule(LightningDataModule):
     """Automatically generates the train, validation and test splits for a Numpy dataset. They are set up as
@@ -96,15 +101,15 @@
         2
     """
 
     name = "sklearn"
 
     def __init__(
         self,
-        X,
+        X,  # noqa: N803
         y,
         x_val=None,
         y_val=None,
         x_test=None,
         y_test=None,
         val_split=0.2,
         test_split=0.1,
@@ -113,25 +118,24 @@
         shuffle=True,
         batch_size: int = 16,
         pin_memory=True,
         drop_last=False,
         *args,
         **kwargs,
     ) -> None:
-
         super().__init__(*args, **kwargs)
         self.num_workers = num_workers
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.pin_memory = pin_memory
         self.drop_last = drop_last
 
         # shuffle x and y
         if shuffle and _SKLEARN_AVAILABLE:
-            X, y = sk_shuffle(X, y, random_state=random_state)
+            X, y = sk_shuffle(X, y, random_state=random_state)  # noqa: N806
         elif shuffle and not _SKLEARN_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError(
                 "You want to use shuffle function from `scikit-learn` which is not installed yet."
             )
 
         val_split = 0 if x_val is not None or y_val is not None else val_split
         test_split = 0 if x_test is not None or y_test is not None else test_split
@@ -140,58 +144,61 @@
         if hold_out_split > 0:
             val_split = val_split / hold_out_split
             hold_out_size = math.floor(len(X) * hold_out_split)
             x_holdout, y_holdout = X[:hold_out_size], y[:hold_out_size]
             test_i_start = int(val_split * hold_out_size)
             x_val_hold_out, y_val_holdout = x_holdout[:test_i_start], y_holdout[:test_i_start]
             x_test_hold_out, y_test_holdout = x_holdout[test_i_start:], y_holdout[test_i_start:]
-            X, y = X[hold_out_size:], y[hold_out_size:]
+            X, y = X[hold_out_size:], y[hold_out_size:]  # noqa: N806
 
         # if don't have x_val and y_val create split from X
         if x_val is None and y_val is None and val_split > 0:
             x_val, y_val = x_val_hold_out, y_val_holdout
 
         # if don't have x_test, y_test create split from X
         if x_test is None and y_test is None and test_split > 0:
             x_test, y_test = x_test_hold_out, y_test_holdout
 
         self._init_datasets(X, y, x_val, y_val, x_test, y_test)
 
     def _init_datasets(
-        self, X: np.ndarray, y: np.ndarray, x_val: np.ndarray, y_val: np.ndarray, x_test: np.ndarray, y_test: np.ndarray
+        self,
+        x: np.ndarray,
+        y: np.ndarray,
+        x_val: np.ndarray,
+        y_val: np.ndarray,
+        x_test: np.ndarray,
+        y_test: np.ndarray,
     ) -> None:
-        self.train_dataset = SklearnDataset(X, y)
+        self.train_dataset = SklearnDataset(x, y)
         self.val_dataset = SklearnDataset(x_val, y_val)
         self.test_dataset = SklearnDataset(x_test, y_test)
 
     def train_dataloader(self) -> DataLoader:
-        loader = DataLoader(
+        return DataLoader(
             self.train_dataset,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def val_dataloader(self) -> DataLoader:
-        loader = DataLoader(
+        return DataLoader(
             self.val_dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def test_dataloader(self) -> DataLoader:
-        loader = DataLoader(
+        return DataLoader(
             self.test_dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/sr_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/sr_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/ssl_imagenet_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/ssl_imagenet_datamodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     from torchvision import transforms as transform_lib
 else:  # pragma: no cover
     warn_missing_pkg("torchvision")
 
 
 @under_review()
 class SSLImagenetDataModule(LightningDataModule):  # pragma: no cover
-
     name = "imagenet"
 
     def __init__(
         self,
         data_dir: str,
         meta_dir: Optional[str] = None,
         num_workers: int = 0,
@@ -92,60 +91,56 @@
         dataset = UnlabeledImagenet(
             self.data_dir,
             num_imgs_per_class=num_images_per_class,
             meta_dir=self.meta_dir,
             split="train",
             transform=transforms,
         )
-        loader: DataLoader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def val_dataloader(self, num_images_per_class: int = 50, add_normalize: bool = False) -> DataLoader:
         transforms = self._default_transforms() if self.val_transforms is None else self.val_transforms
 
         dataset = UnlabeledImagenet(
             self.data_dir,
             num_imgs_per_class_val_split=num_images_per_class,
             meta_dir=self.meta_dir,
             split="val",
             transform=transforms,
         )
-        loader: DataLoader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def test_dataloader(self, num_images_per_class: int, add_normalize: bool = False) -> DataLoader:
         transforms = self._default_transforms() if self.test_transforms is None else self.test_transforms
 
         dataset = UnlabeledImagenet(
             self.data_dir,
             num_imgs_per_class=num_images_per_class,
             meta_dir=self.meta_dir,
             split="test",
             transform=transforms,
         )
-        loader: DataLoader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def _default_transforms(self) -> Callable:
-        transforms = transform_lib.Compose([transform_lib.ToTensor(), imagenet_normalization()])
-        return transforms
+        return transform_lib.Compose([transform_lib.ToTensor(), imagenet_normalization()])
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/stl10_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/stl10_datamodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,23 +118,22 @@
         dataset = STL10(self.data_dir, split="unlabeled", download=False, transform=transforms)
         train_length = len(dataset)
         dataset_train, _ = random_split(
             dataset,
             [train_length - self.unlabeled_val_split, self.unlabeled_val_split],
             generator=torch.Generator().manual_seed(self.seed),
         )
-        loader = DataLoader(
+        return DataLoader(
             dataset_train,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def train_dataloader_mixed(self) -> DataLoader:
         """Loads a portion of the 'unlabeled' training data and 'train' (labeled) data. both portions have a subset
         removed for validation via `unlabeled_val_split` and `train_val_split`
 
         Args:
 
@@ -156,23 +155,22 @@
         labeled_dataset, _ = random_split(
             labeled_dataset,
             [labeled_length - self.train_val_split, self.train_val_split],
             generator=torch.Generator().manual_seed(self.seed),
         )
 
         dataset = ConcatDataset(unlabeled_dataset, labeled_dataset)
-        loader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def val_dataloader(self) -> DataLoader:
         """Loads a portion of the 'unlabeled' training data set aside for validation.
 
         The val dataset = (unlabeled - train_val_split)
 
         Args:
@@ -185,23 +183,22 @@
         dataset = STL10(self.data_dir, split="unlabeled", download=False, transform=transforms)
         train_length = len(dataset)
         _, dataset_val = random_split(
             dataset,
             [train_length - self.unlabeled_val_split, self.unlabeled_val_split],
             generator=torch.Generator().manual_seed(self.seed),
         )
-        loader = DataLoader(
+        return DataLoader(
             dataset_val,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def val_dataloader_mixed(self) -> DataLoader:
         """Loads a portion of the 'unlabeled' training data set aside for validation along with the portion of the
         'train' dataset to be used for validation.
 
         unlabeled_val = (unlabeled - train_val_split)
 
@@ -228,87 +225,82 @@
         _, labeled_dataset = random_split(
             labeled_dataset,
             [labeled_length - self.train_val_split, self.train_val_split],
             generator=torch.Generator().manual_seed(self.seed),
         )
 
         dataset = ConcatDataset(unlabeled_dataset, labeled_dataset)
-        loader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def test_dataloader(self) -> DataLoader:
         """Loads the test split of STL10.
 
         Args:
             batch_size: the batch size
             transforms: the transforms
         """
         transforms = self._default_transforms() if self.test_transforms is None else self.test_transforms
 
         dataset = STL10(self.data_dir, split="test", download=False, transform=transforms)
-        loader = DataLoader(
+        return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def train_dataloader_labeled(self) -> DataLoader:
         transforms = self._default_transforms() if self.val_transforms is None else self.val_transforms
 
         dataset = STL10(self.data_dir, split="train", download=False, transform=transforms)
         train_length = len(dataset)
         dataset_train, _ = random_split(
             dataset,
             [train_length - self.train_val_split, self.train_val_split],
             generator=torch.Generator().manual_seed(self.seed),
         )
-        loader = DataLoader(
+        return DataLoader(
             dataset_train,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def val_dataloader_labeled(self) -> DataLoader:
         transforms = self._default_transforms() if self.val_transforms is None else self.val_transforms
         dataset = STL10(self.data_dir, split="train", download=False, transform=transforms)
         labeled_length = len(dataset)
         _, labeled_val = random_split(
             dataset,
             [labeled_length - self.train_val_split, self.train_val_split],
             generator=torch.Generator().manual_seed(self.seed),
         )
 
-        loader = DataLoader(
+        return DataLoader(
             labeled_val,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             drop_last=self.drop_last,
             pin_memory=self.pin_memory,
         )
-        return loader
 
     def _default_transforms(self) -> Callable:
-        data_transforms = transform_lib.Compose([transform_lib.ToTensor(), stl10_normalization()])
-        return data_transforms
+        return transform_lib.Compose([transform_lib.ToTensor(), stl10_normalization()])
 
     @staticmethod
     def add_dataset_specific_args(parent_parser: ArgumentParser) -> ArgumentParser:
         parser = ArgumentParser(parents=[parent_parser], add_help=False)
 
         parser.add_argument("--data_dir", type=str, default=".")
         parser.add_argument("--num_workers", type=int, default=0)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/vision_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/vision_datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import torch
 from pytorch_lightning import LightningDataModule
 from torch.utils.data import DataLoader, Dataset, random_split
 
 
 class VisionDataModule(LightningDataModule):
-
     EXTRA_ARGS: dict = {}
     name: str = ""
     #: Dataset class to use
     dataset_cls: type
     #: A tuple describing the shape of the data
     dims: tuple
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datamodules/vocdetection_datamodule.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datamodules/vocdetection_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/array_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/array_dataset.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/base_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/base_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.types import TArrays
 
 
 @under_review()
 class LightDataset(ABC, Dataset):
-
     data: Tensor
     targets: Tensor
     normalize: tuple
     dir_path: str
     cache_folder_name: str
     DATASET_NAME = "light"
 
@@ -54,15 +53,15 @@
         return data, targets
 
     def _download_from_url(self, base_url: str, data_folder: str, file_name: str):
         url = urllib.parse.urljoin(base_url, file_name)
         logging.info(f"Downloading {url}")
         fpath = os.path.join(data_folder, file_name)
         try:
-            urllib.request.urlretrieve(url, fpath)
+            urllib.request.urlretrieve(url, fpath)  # noqa: S310
         except HTTPError as err:
             raise RuntimeError(f"Failed download from {url}") from err
 
 
 @dataclass
 class DataModel:
     """Data model dataclass.
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/cifar10_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/cifar10_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     TEST_FILE_NAME = "test.pt"
     DATASET_NAME = "CIFAR10"
     labels = set(range(10))
     relabel = False
 
     def __init__(
         self, data_dir: str = ".", train: bool = True, transform: Optional[Callable] = None, download: bool = True
-    ):
+    ) -> None:
         super().__init__()
         self.dir_path = data_dir
         self.train = train  # training set or test set
         self.transform = transform
 
         if not _PIL_AVAILABLE:
             raise ImportError("You want to use PIL.Image for loading but it is not installed yet.")
@@ -109,15 +109,15 @@
     def _check_exists(cls, data_folder: str, file_names: Sequence[str]) -> bool:
         if isinstance(file_names, str):
             file_names = [file_names]
         return all(os.path.isfile(os.path.join(data_folder, fname)) for fname in file_names)
 
     def _unpickle(self, path_folder: str, file_name: str) -> Tuple[Tensor, Tensor]:
         with open(os.path.join(path_folder, file_name), "rb") as fo:
-            pkl = pickle.load(fo, encoding="bytes")
+            pkl = pickle.load(fo, encoding="bytes")  # noqa: S301
         return torch.tensor(pkl[b"data"]), torch.tensor(pkl[b"labels"])
 
     def _extract_archive_save_torch(self, download_path):
         # extract achieve
         with tarfile.open(os.path.join(download_path, self.FILE_NAME), "r:gz") as tar:
             safe_extract_tarfile(tar, path=download_path)
         # this is internal path in the archive
@@ -180,15 +180,15 @@
         data_dir: str = ".",
         train: bool = True,
         transform: Optional[Callable] = None,
         download: bool = False,
         num_samples: int = 100,
         labels: Optional[Sequence] = (1, 5, 8),
         relabel: bool = True,
-    ):
+    ) -> None:
         """
         Args:
             data_dir: Root directory of dataset where ``CIFAR10/processed/training.pt``
                 and  ``CIFAR10/processed/test.pt`` exist.
             train: If ``True``, creates dataset from ``training.pt``,
                 otherwise from ``test.pt``.
             download: If true, downloads the dataset from the internet and
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/dummy_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/dummy_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,29 @@
         >>> x, y = batch
         >>> x.size()
         torch.Size([7, 1, 28, 28])
         >>> y.size()
         torch.Size([7, 1])
     """
 
-    def __init__(self, *shapes, num_samples: int = 10000):
+    def __init__(self, *shapes, num_samples: int = 10000) -> None:
         """
         Args:
             *shapes: list of shapes
             num_samples: how many samples to use in this dataset
         """
         super().__init__()
         self.shapes = shapes
 
         if num_samples < 1:
             raise ValueError("Provide an argument greater than 0 for `num_samples`")
 
         self.num_samples = num_samples
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.num_samples
 
     def __getitem__(self, idx: int):
         sample = []
         for shape in self.shapes:
             spl = torch.rand(*shape)
             sample.append(spl)
@@ -62,30 +62,30 @@
         torch.Size([7, 1, 4])
         >>> y['labels'].size()
         torch.Size([7, 1])
     """
 
     def __init__(
         self, img_shape: tuple = (3, 256, 256), num_boxes: int = 1, num_classes: int = 2, num_samples: int = 10000
-    ):
+    ) -> None:
         """
         Args:
             *shapes: list of shapes
             num_samples: how many samples to use in this dataset
         """
         super().__init__()
         if num_samples < 1:
             raise ValueError("Provide an argument greater than 0 for `num_samples`")
 
         self.img_shape = img_shape
         self.num_samples = num_samples
         self.num_boxes = num_boxes
         self.num_classes = num_classes
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.num_samples
 
     def _random_bbox(self):
         c, h, w = self.img_shape
         xs = torch.randint(w, (2,))
         ys = torch.randint(h, (2,))
         return [min(xs), min(ys), max(xs), max(ys)]
@@ -108,15 +108,15 @@
         >>> batch = next(iter(dl))
         >>> len(batch['a']),len(batch['a'][0])
         (7, 10)
         >>> len(batch['b']),len(batch['b'][0])
         (7, 10)
     """
 
-    def __init__(self, size: int, num_samples: int = 250):
+    def __init__(self, size: int, num_samples: int = 250) -> None:
         """
         Args:
             size: integer representing the length of a feature_vector
             num_samples: number of samples
         """
         if num_samples < 1:
             raise ValueError("Provide an argument greater than 0 for `num_samples`")
@@ -129,15 +129,15 @@
         self.data_b = torch.randn(num_samples, size)
 
     def __getitem__(self, index):
         a = self.data_a[index]
         b = self.data_b[index]
         return {"a": a, "b": b}
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.len
 
 
 class RandomDictStringDataset(Dataset):
     """Generate a dummy dataset with in dict structure with strings as indexes.
 
     Example:
@@ -148,30 +148,30 @@
         >>> batch = next(iter(dl))
         >>> batch['id']
         ['0', '1', '2', '3', '4', '5', '6']
         >>> len(batch['x'])
         7
     """
 
-    def __init__(self, size: int, num_samples: int = 250):
+    def __init__(self, size: int, num_samples: int = 250) -> None:
         """
         Args:
             size: tuple
             num_samples: number of samples
         """
         if num_samples < 1:
             raise ValueError("Provide an argument greater than 0 for `num_samples`")
 
         self.len = num_samples
         self.data = torch.randn(num_samples, size)
 
     def __getitem__(self, index):
         return {"id": str(index), "x": self.data[index]}
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.len
 
 
 class RandomDataset(Dataset):
     """Generate a dummy dataset.
 
     Example:
@@ -180,24 +180,24 @@
         >>> ds = RandomDataset(10)
         >>> dl = DataLoader(ds, batch_size=7)
         >>> batch = next(iter(dl))
         >>> len(batch),len(batch[0])
         (7, 10)
     """
 
-    def __init__(self, size: int, num_samples: int = 250):
+    def __init__(self, size: int, num_samples: int = 250) -> None:
         """
         Args:
             size: tuple
             num_samples: number of samples
         """
         if num_samples < 1:
             raise ValueError("Provide an argument greater than 0 for `num_samples`")
 
         self.len = num_samples
         self.data = torch.randn(num_samples, size)
 
     def __getitem__(self, index):
         return self.data[index]
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.len
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/emnist_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/emnist_dataset.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/imagenet_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/imagenet_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 else:  # pragma: no cover
     warn_missing_pkg("torchvision")
     ImageNet = object
 
 
 @under_review()
 class UnlabeledImagenet(ImageNet):
-    """Official train set gets split into train, val. (using nb_imgs_per_val_class for each class). Official
+    """Official train set gets split into train, val. (using num_imgs_per_val_class for each class). Official
     validation becomes test set.
 
     Within each class, we further allow limiting the number of samples per class (for semi-sup lng)
     """
 
     def __init__(
         self,
         root,
         split: str = "train",
         num_classes: int = -1,
         num_imgs_per_class: int = -1,
         num_imgs_per_class_val_split: int = 50,
         meta_dir=None,
         **kwargs,
-    ):
+    ) -> None:
         """
         Args:
             root: path of dataset
             split:
             num_classes: Sets the limit of classes
             num_imgs_per_class: Limits the number of images per class
             num_imgs_per_class_val_split: How many images per class to generate the val split
@@ -80,24 +80,23 @@
             train, val = self.partition_train_set(self.imgs, num_imgs_per_class_val_split)
             if original_split == "train":
                 self.imgs = train
             if original_split == "val":
                 self.imgs = val
 
         # limit the number of images in train or test set since the limit was already applied to the val set
-        if split in ["train", "test"]:
-            if num_imgs_per_class != -1:
-                clean_imgs = []
-                cts = {x: 0 for x in range(len(self.classes))}
-                for img_name, idx in self.imgs:
-                    if cts[idx] < num_imgs_per_class:
-                        clean_imgs.append((img_name, idx))
-                        cts[idx] += 1
+        if split in ["train", "test"] and num_imgs_per_class != -1:
+            clean_imgs = []
+            cts = {x: 0 for x in range(len(self.classes))}
+            for img_name, idx in self.imgs:
+                if cts[idx] < num_imgs_per_class:
+                    clean_imgs.append((img_name, idx))
+                    cts[idx] += 1
 
-                self.imgs = clean_imgs
+            self.imgs = clean_imgs
 
         # limit the number of classes
         if num_classes != -1:
             # choose the classes at random (but deterministic)
             ok_classes = list(range(num_classes))
             np.random.seed(1234)
             np.random.shuffle(ok_classes)
@@ -123,21 +122,21 @@
         self.classes = [wnid_to_classes[wnid] for wnid in self.wnids]
         self.class_to_idx = {cls: idx for clss, idx in zip(self.classes, idcs) for cls in clss}
 
         # update the root data
         self.samples = self.imgs
         self.targets = [s[1] for s in self.imgs]
 
-    def partition_train_set(self, imgs, nb_imgs_in_val):
+    def partition_train_set(self, imgs, num_imgs_in_val):
         val = []
         train = []
 
         cts = {x: 0 for x in range(len(self.classes))}
         for img_name, idx in imgs:
-            if cts[idx] < nb_imgs_in_val:
+            if cts[idx] < num_imgs_in_val:
                 val.append((img_name, idx))
                 cts[idx] += 1
             else:
                 train.append((img_name, idx))
 
         return train, val
 
@@ -202,16 +201,16 @@
     def parse_meta_mat(devkit_root):
         metafile = os.path.join(devkit_root, "data", "meta.mat")
         meta = sio.loadmat(metafile, squeeze_me=True)["synsets"]
         nums_children = list(zip(*meta))[4]
         meta = [meta[idx] for idx, num_children in enumerate(nums_children) if num_children == 0]
         idcs, wnids, classes = list(zip(*meta))[:3]
         classes = [tuple(clss.split(", ")) for clss in classes]
-        idx_to_wnid = {idx: wnid for idx, wnid in zip(idcs, wnids)}
-        wnid_to_classes = {wnid: clss for wnid, clss in zip(wnids, classes)}
+        idx_to_wnid = dict(zip(idcs, wnids))
+        wnid_to_classes = dict(zip(wnids, classes))
         return idx_to_wnid, wnid_to_classes
 
     def parse_val_groundtruth_txt(devkit_root):
         file = os.path.join(devkit_root, "data", "ILSVRC2012_validation_ground_truth.txt")
         with open(file) as txtfh:
             val_idcs = txtfh.readlines()
         return [int(val_idx) for val_idx in val_idcs]
@@ -235,10 +234,8 @@
         extract_archive(os.path.join(root, file), tmp_dir)
 
         devkit_root = os.path.join(tmp_dir, "ILSVRC2012_devkit_t12")
         idx_to_wnid, wnid_to_classes = parse_meta_mat(devkit_root)
         val_idcs = parse_val_groundtruth_txt(devkit_root)
         val_wnids = [idx_to_wnid[idx] for idx in val_idcs]
 
-        META_FILE = "meta.bin"
-
-        torch.save((wnid_to_classes, val_wnids), os.path.join(root, META_FILE))
+        torch.save((wnid_to_classes, val_wnids), os.path.join(root, "meta.bin"))
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/kitti_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/kitti_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     def __init__(
         self,
         data_dir: str,
         img_size: tuple = (1242, 376),
         valid_labels: Tuple[int] = DEFAULT_VALID_LABELS,
         transform: Optional[Callable] = None,
-    ):
+    ) -> None:
         if not _PIL_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `PIL` which is not installed yet.")
 
         self.img_size = img_size
         self.valid_labels = valid_labels
         self.void_labels = tuple(label for label in KITTI_LABELS if label not in self.valid_labels)
         self.ignore_index = 250
@@ -92,11 +92,11 @@
             mask[mask == validc] = self.class_map[validc]
         # remove extra idxs from updated dataset
         mask[mask > 33] = self.ignore_index
         return mask
 
     def get_filenames(self, path: str):
         """Returns a list of absolute paths to images inside given `path`"""
-        files_list = list()
+        files_list = []
         for filename in os.listdir(path):
             files_list.append(os.path.join(path, filename))
         return files_list
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/mnist_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/mnist_dataset.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/sr_celeba_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/sr_celeba_dataset.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/sr_dataset_mixin.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/sr_dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/sr_mnist_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/sr_mnist_dataset.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/sr_stl10_dataset.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/sr_stl10_dataset.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/ssl_amdim_datasets.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/ssl_amdim_datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,72 +15,69 @@
 
 
 @under_review()
 class SSLDatasetMixin(ABC):
     @classmethod
     def generate_train_val_split(cls, examples, labels, pct_val):
         """Splits dataset uniformly across classes."""
-        nb_classes = len(set(labels))
+        num_classes = len(set(labels))
 
-        nb_val_images = int(len(examples) * pct_val) // nb_classes
+        num_val_images = int(len(examples) * pct_val) // num_classes
 
         val_x = []
         val_y = []
         train_x = []
         train_y = []
 
-        cts = {x: 0 for x in range(nb_classes)}
+        cts = {x: 0 for x in range(num_classes)}
         for img, class_idx in zip(examples, labels):
-
             # allow labeled
-            if cts[class_idx] < nb_val_images:
+            if cts[class_idx] < num_val_images:
                 val_x.append(img)
                 val_y.append(class_idx)
                 cts[class_idx] += 1
             else:
                 train_x.append(img)
                 train_y.append(class_idx)
 
         val_x = np.stack(val_x)
         train_x = np.stack(train_x)
         return val_x, val_y, train_x, train_y
 
     @classmethod
-    def select_nb_imgs_per_class(cls, examples, labels, nb_imgs_in_val):
+    def select_num_imgs_per_class(cls, examples, labels, num_imgs_in_val):
         """Splits a dataset into two parts.
 
-        The labeled split has nb_imgs_in_val per class
+        The labeled split has num_imgs_in_val per class
         """
-        nb_classes = len(set(labels))
+        num_classes = len(set(labels))
 
-        # def partition_train_set(self, imgs, nb_imgs_in_val):
+        # def partition_train_set(self, imgs, num_imgs_in_val):
         labeled = []
         labeled_y = []
         unlabeled = []
         unlabeled_y = []
 
-        cts = {x: 0 for x in range(nb_classes)}
+        cts = {x: 0 for x in range(num_classes)}
         for img_name, class_idx in zip(examples, labels):
-
             # allow labeled
-            if cts[class_idx] < nb_imgs_in_val:
+            if cts[class_idx] < num_imgs_in_val:
                 labeled.append(img_name)
                 labeled_y.append(class_idx)
                 cts[class_idx] += 1
             else:
                 unlabeled.append(img_name)
                 unlabeled_y.append(class_idx)
 
         labeled = np.stack(labeled)
 
         return labeled, labeled_y
 
     @classmethod
     def deterministic_shuffle(cls, x, y):
-
         n = len(x)
         idxs = list(range(0, n))
         np.random.seed(1234)
         np.random.shuffle(idxs)
 
         x = x[idxs]
 
@@ -96,40 +93,40 @@
     def __init__(
         self,
         root: str,
         split: str = "val",
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         download: bool = False,
-        nb_labeled_per_class: Optional[int] = None,
+        num_labeled_per_class: Optional[int] = None,
         val_pct: float = 0.10,
-    ):
+    ) -> None:
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `torchvision` which is not installed yet.")
 
-        if nb_labeled_per_class == -1:
-            nb_labeled_per_class = None
+        if num_labeled_per_class == -1:
+            num_labeled_per_class = None
 
         # use train for all of these splits
         train = split in ("val", "train", "train+unlabeled")
         super(SSLDatasetMixin, self).__init__(root, train, transform, target_transform, download)
 
         # modify only for val, train
         if split != "test":
             # limit nb of examples per class
-            X_test, y_test, X_train, y_train = self.generate_train_val_split(self.data, self.targets, val_pct)
+            data_test, lbs_test, data_train, lbs_train = self.generate_train_val_split(self.data, self.targets, val_pct)
 
             # shuffle idxs representing the data
-            X_train, y_train = self.deterministic_shuffle(X_train, y_train)
-            X_test, y_test = self.deterministic_shuffle(X_test, y_test)
+            data_train, lbs_train = self.deterministic_shuffle(data_train, lbs_train)
+            data_test, lbs_test = self.deterministic_shuffle(data_test, lbs_test)
 
             if split == "val":
-                self.data = X_test
-                self.targets = y_test
+                self.data = data_test
+                self.targets = lbs_test
 
             else:
-                self.data = X_train
-                self.targets = y_train
+                self.data = data_train
+                self.targets = lbs_train
 
             # limit the number of items per class
-            if nb_labeled_per_class is not None:
-                self.data, self.targets = self.select_nb_imgs_per_class(self.data, self.targets, nb_labeled_per_class)
+            if num_labeled_per_class is not None:
+                self.data, self.targets = self.select_num_imgs_per_class(self.data, self.targets, num_labeled_per_class)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/datasets/utils.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/losses/rl.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/losses/rl.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/losses/self_supervised_learning.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/losses/self_supervised_learning.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,24 +19,22 @@
     # Negative similarity
     mask = ~torch.eye(n_samples, device=sim.device).bool()
     neg = sim.masked_select(mask).view(n_samples, -1).sum(dim=-1)
 
     # Positive similarity :
     pos = torch.exp(torch.sum(out_1 * out_2, dim=-1) / temperature)
     pos = torch.cat([pos, pos], dim=0)
-    loss = -torch.log(pos / neg).mean()
-
-    return loss
+    return -torch.log(pos / neg).mean()
 
 
 @under_review()
 class CPCTask(nn.Module):
     """Loss used in CPC."""
 
-    def __init__(self, num_input_channels, target_dim=64, embed_scale=0.1):
+    def __init__(self, num_input_channels, target_dim=64, embed_scale=0.1) -> None:
         super().__init__()
         self.target_dim = target_dim
         self.embed_scale = embed_scale
 
         self.target_cnn = torch.nn.Conv2d(num_input_channels, self.target_dim, kernel_size=1)
         self.pred_cnn = torch.nn.Conv2d(num_input_channels, self.target_dim, kernel_size=1)
         self.context_cnn = PixelCNN(num_input_channels)
@@ -63,24 +61,23 @@
         n = b * (h - i - 1) * w
         b1 = torch.arange(n) // ((h - i - 1) * w)
         c1 = torch.arange(n) % ((h - i - 1) * w)
         labels = b1 * h * w + (i + 1) * w + c1
         labels = labels.to(logits.device)
         labels = labels.long()
 
-        loss = nn.functional.cross_entropy(logits, labels)
-        return loss
+        return nn.functional.cross_entropy(logits, labels)
 
-    def forward(self, Z):
+    def forward(self, z):
         losses = []
 
-        context = self.context_cnn(Z)
-        targets = self.target_cnn(Z)
+        context = self.context_cnn(z)
+        targets = self.target_cnn(z)
 
-        _, _, h, w = Z.shape
+        _, _, h, w = z.shape
 
         # future prediction
         preds = self.pred_cnn(context)
         for steps_to_ignore in range(h - 1):
             for i in range(steps_to_ignore + 1, h):
                 loss = self.compute_loss_h(targets, preds, i)
                 if not torch.isnan(loss):
@@ -90,79 +87,76 @@
         return loss
 
 
 @under_review()
 class AmdimNCELoss(nn.Module):
     """Compute the NCE scores for predicting r_src->r_trg."""
 
-    def __init__(self, tclip):
+    def __init__(self, tclip) -> None:
         super().__init__()
         self.tclip = tclip
 
     def forward(self, anchor_representations, positive_representations, mask_mat):
         """
         Args:
             anchor_representations: (batch_size, emb_dim)
-            positive_representations: (emb_dim, n_batch * w* h) (ie: nb_feat_vectors x embedding_dim)
+            positive_representations: (emb_dim, n_batch * w* h) (ie: num_feat_vectors x embedding_dim)
             mask_mat: (n_batch_gpu, n_batch)
 
         Output:
             raw_scores: (n_batch_gpu, n_locs)
             nce_scores: (n_batch_gpu, n_locs)
             lgt_reg : scalar
         """
         r_src = anchor_representations
         r_trg = positive_representations
 
         # RKHS = embedding dim
         batch_size, emb_dim = r_src.size()
-        nb_feat_vectors = r_trg.size(1) // batch_size
+        num_feat_vectors = r_trg.size(1) // batch_size
 
-        # (b, b) -> (b, b, nb_feat_vectors)
+        # (b, b) -> (b, b, num_feat_vectors)
         # all zeros with ones in diagonal tensor... (ie: b1 b1 are all 1s, b1 b2 are all zeros)
-        mask_pos = mask_mat.unsqueeze(dim=2).expand(-1, -1, nb_feat_vectors).float()
+        mask_pos = mask_mat.unsqueeze(dim=2).expand(-1, -1, num_feat_vectors).float()
 
         # negative mask
         mask_neg = 1.0 - mask_pos
 
         # -------------------------------
         # ALL SCORES COMPUTATION
         # compute src->trg raw scores for batch
-        # (b, dim) x (dim, nb_feats*b) -> (b, b, nb_feats)
+        # (b, dim) x (dim, num_feats*b) -> (b, b, num_feats)
         # vector for each img in batch times all the vectors of all images in batch
         raw_scores = torch.mm(r_src, r_trg).float()
-        raw_scores = raw_scores.reshape(batch_size, batch_size, nb_feat_vectors)
+        raw_scores = raw_scores.reshape(batch_size, batch_size, num_feat_vectors)
 
         # -----------------------
         # STABILITY TRICKS
         # trick 1: weighted regularization term
         raw_scores = raw_scores / emb_dim**0.5
         lgt_reg = 5e-2 * (raw_scores**2.0).mean()
 
         # trick 2: tanh clip
         raw_scores = tanh_clip(raw_scores, clip_val=self.tclip)
-        """
-        pos_scores includes scores for all the positive samples
-        neg_scores includes scores for all the negative samples, with
-        scores for positive samples set to the min score (-self.tclip here)
-        """
+        """pos_scores includes scores for all the positive samples neg_scores includes scores for all the negative
+        samples, with scores for positive samples set to the min score (-self.tclip here)"""
         # ----------------------
         # EXTRACT POSITIVE SCORES
         # use the index mask to pull all the diagonals which are b1 x b1
-        # (batch_size, nb_feat_vectors)
+        # (batch_size, num_feat_vectors)
         pos_scores = (mask_pos * raw_scores).sum(dim=1)
 
         # ----------------------
         # EXTRACT NEGATIVE SCORES
         # pull everything except diagonal and apply clipping
-        # (batch_size, batch_size, nb_feat_vectors)
+        # (batch_size, batch_size, num_feat_vectors)
         # diagonals have - clip vals. everything else has actual negative stores
         neg_scores = (mask_neg * raw_scores) - (self.tclip * mask_pos)
 
-        # (batch_size, batch_size * nb_feat_vectors) -> (batch_size, batch_size, nb_feat_vectors)
+        # (batch_size, batch_size * num_feat_vectors) -> (batch_size, batch_size, num_feat_vectors)
         neg_scores = neg_scores.reshape(batch_size, -1)
         mask_neg = mask_neg.reshape(batch_size, -1)
 
         # ---------------------
         # STABLE SOFTMAX
         # max for each row of negative samples
         # will use max in safe softmax
@@ -214,15 +208,15 @@
         task = FeatureMapContrastiveTask('01, 02')
 
         # will compare the following:
         # 01: (pos_0, anc_1), (anc_0, pos_1)
         # 02: (pos_0, anc_2), (anc_0, pos_2)
     """
 
-    def __init__(self, comparisons: str = "00, 11", tclip: float = 10.0, bidirectional: bool = True):
+    def __init__(self, comparisons: str = "00, 11", tclip: float = 10.0, bidirectional: bool = True) -> None:
         """
         Args:
             comparisons: groupings of feature map indices to compare (zero indexed, 'r' means random) ex: '00, 1r'
             tclip: stability clipping value
             bidirectional: if true, does the comparison both ways
         """
         super().__init__()
@@ -272,16 +266,15 @@
         if masks is not None:
             # subsample from conv-ish r_cnv to get a single vector
             mask_idx = torch.randint(0, masks.size(0), (n_batch,), device=r_cnv.device)
             mask = masks[mask_idx]
             r_cnv = torch.masked_select(r_cnv, mask)
 
         # flatten features for use as globals in glb->lcl nce cost
-        r_vec = r_cnv.reshape(n_batch, feat_dim)
-        return r_vec
+        return r_cnv.reshape(n_batch, feat_dim)
 
     def __cache_dimension_masks(self, *args):
         # cache masks for each feature map we'll need
         if len(self.masks) == 0:
             for m1 in args:
                 batch_size, emb_dim, h, w = m1.size()
 
@@ -333,16 +326,15 @@
         """
         assert len(anchor_maps) == len(self.map_indexes), f"expected each input to have {len(self.map_indexes)} tensors"
 
         self.__cache_dimension_masks(*(anchor_maps + positive_maps))
 
         regularizer = 0
         losses = []
-        for (ai, pi) in self.map_indexes:
-
+        for ai, pi in self.map_indexes:
             # choose a random map
             if ai == -1:
                 ai = np.random.randint(0, len(anchor_maps))
             if pi == -1:
                 pi = np.random.randint(0, len(anchor_maps))
 
             # pull out the maps
@@ -368,13 +360,9 @@
             losses.append(map_loss.mean())
 
         return torch.stack(losses), regularizer
 
 
 @under_review()
 def tanh_clip(x, clip_val=10.0):
-    """soft clip values to the range [-clip_val, +clip_val]"""
-    if clip_val is not None:
-        x_clip = clip_val * torch.tanh((1.0 / clip_val) * x)
-    else:
-        x_clip = x
-    return x_clip
+    """Soft clip values to the range [-clip_val, +clip_val]"""
+    return clip_val * torch.tanh(1.0 / clip_val * x) if clip_val is not None else x
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/metrics/aggregation.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/metrics/aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 
 def accuracy(preds, labels):
     preds = preds.float()
     max_lgt = torch.max(preds, 1)[1]
     num_correct = (max_lgt == labels).sum().item()
     num_correct = torch.tensor(num_correct).float()
-    acc = num_correct / len(labels)
-
-    return acc
+    return num_correct / len(labels)
 
 
 def precision_at_k(output, target, top_k=(1,)):
     """Computes the accuracy over the k top predictions for the specified values of k."""
     with torch.no_grad():
         maxk = max(top_k)
         batch_size = target.size(0)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_ae/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_ae/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-AE Template
-============
+"""AE Template.
 
 This is a basic template for implementing an Autoencoder in PyTorch Lightning.
 
 A default encoder and decoder have been provided but can easily be replaced by custom models.
 
 This template uses the CIFAR10 dataset but image data of any dimension can be fed in as long as the image
  width and image height are even values. For other types of data, such as sound, it will be necessary
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_ae/basic_ae_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_ae/basic_ae_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import urllib.parse
 from argparse import ArgumentParser
 
 import torch
 from pytorch_lightning import LightningModule, Trainer
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts import _HTTPS_AWS_HUB
 from pl_bolts.models.autoencoders.components import (
     resnet18_decoder,
     resnet18_encoder,
     resnet50_decoder,
     resnet50_encoder,
@@ -41,15 +41,15 @@
         enc_type: str = "resnet18",
         first_conv: bool = False,
         maxpool1: bool = False,
         enc_out_dim: int = 512,
         latent_dim: int = 256,
         lr: float = 1e-4,
         **kwargs,
-    ):
+    ) -> None:
         """
         Args:
             input_height: height of the images
             enc_type: option between resnet18 or resnet50
             first_conv: use standard kernel_size 7, stride 2 at start or
                 replace it with kernel_size 3, stride 1 conv
             maxpool1: use standard maxpool to reduce spatial dim of feat by a factor of 2
@@ -97,16 +97,15 @@
             raise KeyError(str(checkpoint_name) + " not present in pretrained weights.")
 
         return self.load_from_checkpoint(AE.pretrained_urls[checkpoint_name], strict=False)
 
     def forward(self, x):
         feats = self.encoder(x)
         z = self.fc(feats)
-        x_hat = self.decoder(z)
-        return x_hat
+        return self.decoder(z)
 
     def step(self, batch, batch_idx):
         x, y = batch
 
         feats = self.encoder(x)
         z = self.fc(feats)
         x_hat = self.decoder(z)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_vae/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_vae/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-"""
-VAE Template
-============
+"""VAE Template.
 
 This is a basic template for implementing a Variational Autoencoder in PyTorch Lightning.
 
 A default encoder and decoder have been provided but can easily be replaced by custom models.
 
-This template uses the CIFAR10 dataset but image data of any dimension can be fed in as long as the image
- width and image height are even values. For other types of data, such as sound, it will be necessary
- to change the Encoder and Decoder.
+This template uses the CIFAR10 dataset but image data of any dimension can be fed in as long as the image  width and
+image height are even values. For other types of data, such as sound, it will be necessary  to change the Encoder and
+Decoder.
 
-The default encoder is a resnet18 backbone followed by linear layers which map representations
- to mu and var. The default decoder mirrors the encoder architecture and is similar to an inverted
- resnet18. The model also assumes a Gaussian prior and a Gaussian approximate posterior distribution.
+The default encoder is a resnet18 backbone followed by linear layers which map representations  to mu and var. The
+default decoder mirrors the encoder architecture and is similar to an inverted  resnet18. The model also assumes a
+Gaussian prior and a Gaussian approximate posterior distribution.
 """
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/basic_vae/basic_vae_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/basic_vae/basic_vae_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import urllib.parse
 from argparse import ArgumentParser
 
 import torch
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts import _HTTPS_AWS_HUB
 from pl_bolts.models.autoencoders.components import (
     resnet18_decoder,
     resnet18_encoder,
     resnet50_decoder,
     resnet50_encoder,
@@ -46,15 +46,15 @@
         first_conv: bool = False,
         maxpool1: bool = False,
         enc_out_dim: int = 512,
         kl_coeff: float = 0.1,
         latent_dim: int = 256,
         lr: float = 1e-4,
         **kwargs,
-    ):
+    ) -> None:
         """
         Args:
             input_height: height of the images
             enc_type: option between resnet18 or resnet50
             first_conv: use standard kernel_size 7, stride 2 at start or
                 replace it with kernel_size 3, stride 1 conv
             maxpool1: use standard maxpool to reduce spatial dim of feat by a factor of 2
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/autoencoders/components.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/autoencoders/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import torch
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class Interpolate(nn.Module):
     """nn.Module wrapper for F.interpolate."""
 
-    def __init__(self, size=None, scale_factor=None):
+    def __init__(self, size=None, scale_factor=None) -> None:
         super().__init__()
         self.size, self.scale_factor = size, scale_factor
 
     def forward(self, x):
         return F.interpolate(x, size=self.size, scale_factor=self.scale_factor)
 
 
@@ -27,35 +27,35 @@
 def conv1x1(in_planes, out_planes, stride=1):
     """1x1 convolution."""
     return nn.Conv2d(in_planes, out_planes, kernel_size=1, stride=stride, bias=False)
 
 
 @under_review()
 def resize_conv3x3(in_planes, out_planes, scale=1):
-    """upsample + 3x3 convolution with padding to avoid checkerboard artifact."""
+    """Upsample + 3x3 convolution with padding to avoid checkerboard artifact."""
     if scale == 1:
         return conv3x3(in_planes, out_planes)
     return nn.Sequential(Interpolate(scale_factor=scale), conv3x3(in_planes, out_planes))
 
 
 @under_review()
 def resize_conv1x1(in_planes, out_planes, scale=1):
-    """upsample + 1x1 convolution with padding to avoid checkerboard artifact."""
+    """Upsample + 1x1 convolution with padding to avoid checkerboard artifact."""
     if scale == 1:
         return conv1x1(in_planes, out_planes)
     return nn.Sequential(Interpolate(scale_factor=scale), conv1x1(in_planes, out_planes))
 
 
 @under_review()
 class EncoderBlock(nn.Module):
     """ResNet block, copied from https://github.com/pytorch/vision/blob/master/torchvision/models/resnet.py#L35."""
 
     expansion = 1
 
-    def __init__(self, inplanes, planes, stride=1, downsample=None):
+    def __init__(self, inplanes, planes, stride=1, downsample=None) -> None:
         super().__init__()
         self.conv1 = conv3x3(inplanes, planes, stride)
         self.bn1 = nn.BatchNorm2d(planes)
         self.relu = nn.ReLU(inplace=True)
         self.conv2 = conv3x3(planes, planes)
         self.bn2 = nn.BatchNorm2d(planes)
         self.downsample = downsample
@@ -82,15 +82,15 @@
 @under_review()
 class EncoderBottleneck(nn.Module):
     """ResNet bottleneck, copied from
     https://github.com/pytorch/vision/blob/master/torchvision/models/resnet.py#L75."""
 
     expansion = 4
 
-    def __init__(self, inplanes, planes, stride=1, downsample=None):
+    def __init__(self, inplanes, planes, stride=1, downsample=None) -> None:
         super().__init__()
         width = planes  # this needs to change if we want wide resnets
         self.conv1 = conv1x1(inplanes, width)
         self.bn1 = nn.BatchNorm2d(width)
         self.conv2 = conv3x3(width, width, stride)
         self.bn2 = nn.BatchNorm2d(width)
         self.conv3 = conv1x1(width, planes * self.expansion)
@@ -123,15 +123,15 @@
 
 @under_review()
 class DecoderBlock(nn.Module):
     """ResNet block, but convs replaced with resize convs, and channel increase is in second conv, not first."""
 
     expansion = 1
 
-    def __init__(self, inplanes, planes, scale=1, upsample=None):
+    def __init__(self, inplanes, planes, scale=1, upsample=None) -> None:
         super().__init__()
         self.conv1 = resize_conv3x3(inplanes, inplanes)
         self.bn1 = nn.BatchNorm2d(inplanes)
         self.relu = nn.ReLU(inplace=True)
         self.conv2 = resize_conv3x3(inplanes, planes, scale)
         self.bn2 = nn.BatchNorm2d(planes)
         self.upsample = upsample
@@ -157,15 +157,15 @@
 
 @under_review()
 class DecoderBottleneck(nn.Module):
     """ResNet bottleneck, but convs replaced with resize convs."""
 
     expansion = 4
 
-    def __init__(self, inplanes, planes, scale=1, upsample=None):
+    def __init__(self, inplanes, planes, scale=1, upsample=None) -> None:
         super().__init__()
         width = planes  # this needs to change if we want wide resnets
         self.conv1 = resize_conv1x1(inplanes, width)
         self.bn1 = nn.BatchNorm2d(width)
         self.conv2 = resize_conv3x3(width, width, scale)
         self.bn2 = nn.BatchNorm2d(width)
         self.conv3 = conv1x1(width, planes * self.expansion)
@@ -194,15 +194,15 @@
         out += identity
         out = self.relu(out)
         return out
 
 
 @under_review()
 class ResNetEncoder(nn.Module):
-    def __init__(self, block, layers, first_conv=False, maxpool1=False):
+    def __init__(self, block, layers, first_conv=False, maxpool1=False) -> None:
         super().__init__()
 
         self.inplanes = 64
         self.first_conv = first_conv
         self.maxpool1 = maxpool1
 
         if self.first_conv:
@@ -256,15 +256,15 @@
         return x
 
 
 @under_review()
 class ResNetDecoder(nn.Module):
     """Resnet in reverse order."""
 
-    def __init__(self, block, layers, latent_dim, input_height, first_conv=False, maxpool1=False):
+    def __init__(self, block, layers, latent_dim, input_height, first_conv=False, maxpool1=False) -> None:
         super().__init__()
 
         self.expansion = block.expansion
         self.inplanes = 512 * block.expansion
         self.first_conv = first_conv
         self.maxpool1 = maxpool1
         self.input_height = input_height
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/detection/components/_supported_models.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/components/_supported_models.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/detection/components/torchvision_backbones.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/components/torchvision_backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/detection/faster_rcnn/backbones.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/faster_rcnn/backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/detection/faster_rcnn/faster_rcnn_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/faster_rcnn/faster_rcnn_module.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         num_classes: int = 91,
         backbone: Optional[Union[str, torch.nn.Module]] = None,
         fpn: bool = True,
         pretrained: bool = False,
         pretrained_backbone: bool = True,
         trainable_backbone_layers: int = 3,
         **kwargs: Any,
-    ):
+    ) -> None:
         """
         Args:
             learning_rate: the learning rate
             num_classes: number of detection classes (including background)
             backbone: Pretained backbone CNN architecture or torch.nn.Module instance.
             fpn: If True, creates a Feature Pyramind Network on top of Resnet based CNNs.
             pretrained: if true, returns a model pre-trained on COCO train2017
@@ -109,17 +109,16 @@
             self.model = torchvision_FasterRCNN(backbone_model, num_classes=num_classes, **kwargs)
 
     def forward(self, x):
         self.model.eval()
         return self.model(x)
 
     def training_step(self, batch, batch_idx):
-
         images, targets = batch
-        targets = [{k: v for k, v in t.items()} for t in targets]
+        targets = [dict(t.items()) for t in targets]
 
         # fasterrcnn takes both images and targets for training, returns
         loss_dict = self.model(images, targets)
         loss = sum(loss for loss in loss_dict.values())
         return {"loss": loss, "log": loss_dict}
 
     def validation_step(self, batch, batch_idx):
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/detection/retinanet/backbones.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/retinanet/backbones.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/detection/retinanet/retinanet_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/retinanet/retinanet_module.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from pl_bolts.models.detection.retinanet import create_retinanet_backbone
 from pl_bolts.utils import _TORCHVISION_AVAILABLE, _TORCHVISION_LESS_THAN_0_13
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _TORCHVISION_AVAILABLE:
-
     from torchvision.models.detection.retinanet import RetinaNet as torchvision_RetinaNet
     from torchvision.models.detection.retinanet import RetinaNetHead, retinanet_resnet50_fpn
     from torchvision.ops import box_iou
 else:  # pragma: no cover
     warn_missing_pkg("torchvision")
 
 
@@ -44,15 +43,15 @@
         num_classes: int = 91,
         backbone: Optional[str] = None,
         fpn: bool = True,
         pretrained: bool = False,
         pretrained_backbone: bool = True,
         trainable_backbone_layers: int = 3,
         **kwargs: Any,
-    ):
+    ) -> None:
         """
         Args:
             learning_rate: the learning rate
             num_classes: number of detection classes (including background)
             backbone: Pretained backbone CNN architecture.
             fpn: If True, creates a Feature Pyramind Network on top of Resnet based CNNs.
             pretrained: if true, returns a model pre-trained on COCO train2017
@@ -93,17 +92,16 @@
             self.model = torchvision_RetinaNet(backbone_model, num_classes=num_classes, **kwargs)
 
     def forward(self, x):
         self.model.eval()
         return self.model(x)
 
     def training_step(self, batch, batch_idx):
-
         images, targets = batch
-        targets = [{k: v for k, v in t.items()} for t in targets]
+        targets = [dict(t.items()) for t in targets]
 
         # fasterrcnn takes both images and targets for training, returns
         loss_dict = self.model(images, targets)
         loss = sum(loss for loss in loss_dict.values())
         self.log("loss", loss, prog_bar=True)
         return loss
 
@@ -133,15 +131,18 @@
             momentum=0.9,
             weight_decay=0.005,
         )
 
 
 @under_review()
 def cli_main():
-    from pytorch_lightning.utilities.cli import LightningCLI
+    try:  # Backward compatibility for Lightning CLI
+        from pytorch_lightning.cli import LightningCLI  # PL v1.9+
+    except ImportError:
+        from pytorch_lightning.utilities.cli import LightningCLI  # PL v1.8
 
     from pl_bolts.datamodules import VOCDetectionDataModule
 
     LightningCLI(RetinaNet, VOCDetectionDataModule, seed_everything_default=42)
 
 
 if __name__ == "__main__":
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/detection/yolo/yolo_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/detection/yolo/yolo_module.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,613 +1,618 @@
-import logging
-from typing import Any, Dict, List, Optional, Tuple, Type
+from copy import copy
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
-import numpy as np
 import torch
 import torch.nn as nn
 from pytorch_lightning import LightningModule
-from pytorch_lightning.utilities import rank_zero_info
+from pytorch_lightning.utilities.cli import LightningCLI
+from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch import Tensor, optim
 
-from pl_bolts.models.detection.yolo.yolo_layers import DetectionLayer, RouteLayer, ShortcutLayer
+# It seems to be impossible to avoid mypy errors if using import instead of getattr().
+# See https://github.com/python/mypy/issues/8823
+try:
+    LRScheduler: Any = getattr(optim.lr_scheduler, "LRScheduler")
+except AttributeError:
+    LRScheduler = getattr(optim.lr_scheduler, "_LRScheduler")
+
+from pl_bolts.datamodules import VOCDetectionDataModule
+from pl_bolts.datamodules.vocdetection_datamodule import Compose
 from pl_bolts.optimizers.lr_scheduler import LinearWarmupCosineAnnealingLR
-from pl_bolts.utils import _TORCHVISION_AVAILABLE
-from pl_bolts.utils.stability import under_review
+from pl_bolts.utils import _TORCHMETRICS_DETECTION_AVAILABLE, _TORCHVISION_AVAILABLE
 from pl_bolts.utils.warnings import warn_missing_pkg
 
+from .darknet_network import DarknetNetwork
+from .torch_networks import YOLOV4Network
+from .types import BATCH, IMAGES, PRED, TARGET, TARGETS
+
+if _TORCHMETRICS_DETECTION_AVAILABLE:
+    try:
+        from torchmetrics.detection import MeanAveragePrecision
+
+        _MEAN_AVERAGE_PRECISION_AVAILABLE = True
+    except ImportError:
+        _MEAN_AVERAGE_PRECISION_AVAILABLE = False
+else:
+    _MEAN_AVERAGE_PRECISION_AVAILABLE = False
+
 if _TORCHVISION_AVAILABLE:
-    from torchvision.ops import nms
-    from torchvision.transforms import functional as F
+    from torchvision.ops import batched_nms
+    from torchvision.transforms import functional as T  # noqa: N812
 else:
     warn_missing_pkg("torchvision")
 
-log = logging.getLogger(__name__)
 
-
-@under_review()
 class YOLO(LightningModule):
-    """PyTorch Lightning implementation of YOLOv3 and YOLOv4.
+    """PyTorch Lightning implementation of YOLO that supports the most important features of YOLOv3, YOLOv4,
+    YOLOv5, YOLOv7, Scaled-YOLOv4, and YOLOX.
+
+    *YOLOv3 paper*: `Joseph Redmon and Ali Farhadi <https://arxiv.org/abs/1804.02767>`__
 
-    *YOLOv3 paper*: `Joseph Redmon and Ali Farhadi <https://arxiv.org/abs/1804.02767>`_
+    *YOLOv4 paper*: `Alexey Bochkovskiy, Chien-Yao Wang, and Hong-Yuan Mark Liao <https://arxiv.org/abs/2004.10934>`__
 
-    *YOLOv4 paper*: `Alexey Bochkovskiy, Chien-Yao Wang, and Hong-Yuan Mark Liao <https://arxiv.org/abs/2004.10934>`_
+    *YOLOv7 paper*: `Chien-Yao Wang, Alexey Bochkovskiy, and Hong-Yuan Mark Liao <https://arxiv.org/abs/2207.02696>`__
 
-    *Implementation*: `Seppo Enarvi <https://github.com/senarvi>`_
+    *Scaled-YOLOv4 paper*: `Chien-Yao Wang, Alexey Bochkovskiy, and Hong-Yuan Mark Liao
+    <https://arxiv.org/abs/2011.08036>`__
 
-    The network architecture can be read from a Darknet configuration file using the
-    :class:`~pl_bolts.models.detection.yolo.yolo_config.YOLOConfiguration` class, or created by
-    some other means, and provided as a list of PyTorch modules.
+    *YOLOX paper*: `Zheng Ge, Songtao Liu, Feng Wang, Zeming Li, and Jian Sun <https://arxiv.org/abs/2107.08430>`__
 
-    The input from the data loader is expected to be a list of images. Each image is a tensor with
-    shape ``[channels, height, width]``. The images from a single batch will be stacked into a
-    single tensor, so the sizes have to match. Different batches can have different image sizes, as
-    long as the size is divisible by the ratio in which the network downsamples the input.
+    *Implementation*: `Seppo Enarvi <https://github.com/senarvi>`__
 
-    During training, the model expects both the input tensors and a list of targets. *Each target is
-    a dictionary containing*:
+    The network architecture can be written in PyTorch, or read from a Darknet configuration file using the
+    :class:`~.darknet_network.DarknetNetwork` class. ``DarknetNetwork`` is also able to read weights that have been
+    saved by Darknet. See the :class:`~.yolo_module.CLIYOLO` command-line application for an example of how to specify
+    a network architecture.
+
+    The input is expected to be a list of images. Each image is a tensor with shape ``[channels, height, width]``. The
+    images from a single batch will be stacked into a single tensor, so the sizes have to match. Different batches can
+    have different image sizes, as long as the size is divisible by the ratio in which the network downsamples the
+    input.
+
+    During training, the model expects both the image tensors and a list of targets. It's possible to train a model
+    using one integer class label per box, but the YOLO model supports also multiple labels per box. For multi-label
+    training, simply use a boolean matrix that indicates which classes are assigned to which boxes, in place of the
+    class labels. *Each target is a dictionary containing the following tensors*:
 
     - boxes (``FloatTensor[N, 4]``): the ground-truth boxes in `(x1, y1, x2, y2)` format
-    - labels (``Int64Tensor[N]``): the class label for each ground-truth box
+    - labels (``Int64Tensor[N]`` or ``BoolTensor[N, classes]``): the class label or a boolean class mask for each
+      ground-truth box
 
-    :func:`~pl_bolts.models.detection.yolo.yolo_module.YOLO.forward` method returns all
-    predictions from all detection layers in all images in one tensor with shape
-    ``[images, predictors, classes + 5]``. The coordinates are scaled to the input image size.
-    During training it also returns a dictionary containing the classification, box overlap, and
-    confidence losses.
-
-    During inference, the model requires only the input tensors.
-    :func:`~pl_bolts.models.detection.yolo.yolo_module.YOLO.infer` method filters and processes the
-    predictions. *The processed output includes the following tensors*:
+    :func:`~.yolo_module.YOLO.forward` method returns all predictions from all detection layers in one tensor with shape
+    ``[N, anchors, classes + 5]``, where ``anchors`` is the total number of anchors in all detection layers. The
+    coordinates are scaled to the input image size. During training it also returns a dictionary containing the
+    classification, box overlap, and confidence losses.
+
+    During inference, the model requires only the image tensor. :func:`~.yolo_module.YOLO.infer` method filters and
+    processes the predictions. If a prediction has a high score for more than one class, it will be duplicated. *The
+    processed output is returned in a dictionary containing the following tensors*:
 
     - boxes (``FloatTensor[N, 4]``): predicted bounding box `(x1, y1, x2, y2)` coordinates in image space
     - scores (``FloatTensor[N]``): detection confidences
-    - labels (``Int64Tensor[N]``): the predicted labels for each image
-
-    Weights can be loaded from a Darknet model file using ``load_darknet_weights()``.
-
-    CLI command::
+    - labels (``Int64Tensor[N]``): the predicted labels for each object
 
-        # PascalVOC
-        wget https://raw.githubusercontent.com/AlexeyAB/darknet/master/cfg/yolov4-tiny-3l.cfg
-        python yolo_module.py --config yolov4-tiny-3l.cfg --data_dir . --gpus 8 --batch_size 8
+    Args:
+        network: A module that represents the network layers. This can be obtained from a Darknet configuration using
+            :func:`~.darknet_network.DarknetNetwork`, or it can be defined as PyTorch code.
+        optimizer: Which optimizer class to use for training.
+        optimizer_params: Parameters to pass to the optimizer constructor. Weight decay will be applied only to
+            convolutional layer weights.
+        lr_scheduler: Which learning rate scheduler class to use for training.
+        lr_scheduler_params: Parameters to pass to the learning rate scheduler constructor.
+        confidence_threshold: Postprocessing will remove bounding boxes whose confidence score is not higher than this
+            threshold.
+        nms_threshold: Non-maximum suppression will remove bounding boxes whose IoU with a higher confidence box is
+            higher than this threshold, if the predicted categories are equal.
+        detections_per_image: Keep at most this number of highest-confidence detections per image.
     """
 
     def __init__(
         self,
-        network: nn.ModuleList,
+        network: nn.Module,
         optimizer: Type[optim.Optimizer] = optim.SGD,
-        optimizer_params: Dict[str, Any] = {"lr": 0.001, "momentum": 0.9, "weight_decay": 0.0005},
-        lr_scheduler: Type[optim.lr_scheduler._LRScheduler] = LinearWarmupCosineAnnealingLR,
-        lr_scheduler_params: Dict[str, Any] = {"warmup_epochs": 1, "max_epochs": 300, "warmup_start_lr": 0.0},
+        optimizer_params: Optional[Dict[str, Any]] = None,
+        lr_scheduler: Type[LRScheduler] = LinearWarmupCosineAnnealingLR,
+        lr_scheduler_params: Optional[Dict[str, Any]] = None,
         confidence_threshold: float = 0.2,
         nms_threshold: float = 0.45,
-        max_predictions_per_image: int = -1,
+        detections_per_image: int = 300,
     ) -> None:
-        """
-        Args:
-            network: A list of network modules. This can be obtained from a Darknet configuration
-                using the :func:`~pl_bolts.models.detection.yolo.yolo_config.YOLOConfiguration.get_network`
-                method.
-            optimizer: Which optimizer class to use for training.
-            optimizer_params: Parameters to pass to the optimizer constructor.
-            lr_scheduler: Which learning rate scheduler class to use for training.
-            lr_scheduler_params: Parameters to pass to the learning rate scheduler constructor.
-            confidence_threshold: Postprocessing will remove bounding boxes whose
-                confidence score is not higher than this threshold.
-            nms_threshold: Non-maximum suppression will remove bounding boxes whose IoU with a higher
-                confidence box is higher than this threshold, if the predicted categories are equal.
-            max_predictions_per_image: If non-negative, keep at most this number of
-                highest-confidence predictions per image.
-        """
         super().__init__()
 
         if not _TORCHVISION_AVAILABLE:
             raise ModuleNotFoundError("YOLO model uses `torchvision`, which is not installed yet.")  # pragma: no-cover
 
         self.network = network
         self.optimizer_class = optimizer
-        self.optimizer_params = optimizer_params
+        if optimizer_params is not None:
+            self.optimizer_params = optimizer_params
+        else:
+            self.optimizer_params = {"lr": 0.01, "momentum": 0.9, "weight_decay": 0.0005}
         self.lr_scheduler_class = lr_scheduler
-        self.lr_scheduler_params = lr_scheduler_params
+        if lr_scheduler_params is not None:
+            self.lr_scheduler_params = lr_scheduler_params
+        else:
+            self.lr_scheduler_params = {"warmup_epochs": 5, "max_epochs": 300, "warmup_start_lr": 0.0}
         self.confidence_threshold = confidence_threshold
         self.nms_threshold = nms_threshold
-        self.max_predictions_per_image = max_predictions_per_image
+        self.detections_per_image = detections_per_image
+
+        if _MEAN_AVERAGE_PRECISION_AVAILABLE:
+            self._val_map = MeanAveragePrecision()
+            self._test_map = MeanAveragePrecision()
 
     def forward(
-        self, images: Tensor, targets: Optional[List[Dict[str, Tensor]]] = None
-    ) -> Tuple[Tensor, Dict[str, Tensor]]:
+        self, images: Union[Tensor, IMAGES], targets: Optional[TARGETS] = None
+    ) -> Union[Tensor, Tuple[Tensor, Tensor]]:
         """Runs a forward pass through the network (all layers listed in ``self.network``), and if training targets
         are provided, computes the losses from the detection layers.
 
-        Detections are concatenated from the detection layers. Each image will produce
-        `N * num_anchors * grid_height * grid_width` detections, where `N` depends on the number of
-        detection layers. For one detection layer `N = 1`, and each detection layer increases it by
-        a number that depends on the size of the feature map on that layer. For example, if the
-        feature map is twice as wide and high as the grid, the layer will add four times more
-        features.
+        Detections are concatenated from the detection layers. Each detection layer will produce a number of detections
+        that depends on the size of the feature map and the number of anchors per feature map cell.
 
         Args:
-            images: Images to be processed. Tensor of size
-                ``[batch_size, num_channels, height, width]``.
-            targets: If set, computes losses from detection layers against these targets. A list of
+            images: A tensor of size ``[batch_size, channels, height, width]`` containing a batch of images or a list of
+                image tensors.
+            targets: If given, computes losses from detection layers against these targets. A list of target
                 dictionaries, one for each image.
 
         Returns:
-            detections (:class:`~torch.Tensor`), losses (Dict[str, :class:`~torch.Tensor`]):
-            Detections, and if targets were provided, a dictionary of losses. Detections are shaped
-            ``[batch_size, num_predictors, num_classes + 5]``, where ``num_predictors`` is the
-            total number of cells in all detection layers times the number of boxes predicted by
-            one cell. The predicted box coordinates are in `(x1, y1, x2, y2)` format and scaled to
-            the input image size.
-        """
-        outputs = []  # Outputs from all layers
-        detections = []  # Outputs from detection layers
-        losses = []  # Losses from detection layers
-        hits = []  # Number of targets each detection layer was responsible for
-
-        image_height = images.shape[2]
-        image_width = images.shape[3]
-        image_size = torch.tensor([image_width, image_height], device=images.device)
-
-        x = images
-        for module in self.network:
-            if isinstance(module, (RouteLayer, ShortcutLayer)):
-                x = module(x, outputs)
-            elif isinstance(module, DetectionLayer):
-                if targets is None:
-                    x = module(x, image_size)
-                    detections.append(x)
-                else:
-                    x, layer_losses, layer_hits = module(x, image_size, targets)
-                    detections.append(x)
-                    losses.append(layer_losses)
-                    hits.append(layer_hits)
-            else:
-                x = module(x)
-
-            outputs.append(x)
+            detections (:class:`~torch.Tensor`), losses (:class:`~torch.Tensor`): Detections, and if targets were
+            provided, a dictionary of losses. Detections are shaped ``[batch_size, anchors, classes + 5]``, where
+            ``anchors`` is the feature map size (width * height) times the number of anchors per cell. The predicted box
+            coordinates are in `(x1, y1, x2, y2)` format and scaled to the input image size.
+        """
+        self.validate_batch(images, targets)
+        images_tensor = images if isinstance(images, Tensor) else torch.stack(images)
+        detections, losses, hits = self.network(images_tensor, targets)
 
         detections = torch.cat(detections, 1)
         if targets is None:
             return detections
 
         total_hits = sum(hits)
-        num_targets = sum(len(image_targets["boxes"]) for image_targets in targets)
-        if total_hits != num_targets:
-            log.warning(
-                f"{num_targets} training targets were matched a total of {total_hits} times by detection layers. "
-                "Anchors may have been configured incorrectly."
-            )
         for layer_idx, layer_hits in enumerate(hits):
-            hit_rate = torch.true_divide(layer_hits, total_hits) if total_hits > 0 else 1.0
-            self.log(f"layer_{layer_idx}_hit_rate", hit_rate, sync_dist=False)
-
-        def total_loss(loss_name):
-            """Returns the sum of the loss over detection layers."""
-            loss_tuple = tuple(layer_losses[loss_name] for layer_losses in losses)
-            return torch.stack(loss_tuple).sum()
+            hit_rate: Union[Tensor, float] = torch.true_divide(layer_hits, total_hits) if total_hits > 0 else 1.0
+            self.log(f"layer_{layer_idx}_hit_rate", hit_rate, sync_dist=True, batch_size=len(images))
 
-        losses = {loss_name: total_loss(loss_name) for loss_name in losses[0].keys()}
+        losses = torch.stack(losses).sum(0)
         return detections, losses
 
-    def configure_optimizers(self) -> Tuple[List, List]:
-        """Constructs the optimizer and learning rate scheduler."""
-        optimizer = self.optimizer_class(self.parameters(), **self.optimizer_params)
+    def configure_optimizers(self) -> Tuple[List[optim.Optimizer], List[LRScheduler]]:
+        """Constructs the optimizer and learning rate scheduler based on ``self.optimizer_params`` and
+        ``self.lr_scheduler_params``.
+
+        If weight decay is specified, it will be applied only to convolutional layer weights, as they contain much more
+        parameters than the biases and batch normalization parameters. Regularizing all parameters could lead to
+        underfitting.
+        """
+        if ("weight_decay" in self.optimizer_params) and (self.optimizer_params["weight_decay"] != 0):
+            defaults = copy(self.optimizer_params)
+            weight_decay = defaults.pop("weight_decay")
+
+            default_group = []
+            wd_group = []
+            for name, tensor in self.named_parameters():
+                if not tensor.requires_grad:
+                    continue
+                if name.endswith(".conv.weight"):
+                    wd_group.append(tensor)
+                else:
+                    default_group.append(tensor)
+
+            params = [
+                {"params": default_group, "weight_decay": 0.0},
+                {"params": wd_group, "weight_decay": weight_decay},
+            ]
+            optimizer = self.optimizer_class(params, **defaults)
+        else:
+            optimizer = self.optimizer_class(self.parameters(), **self.optimizer_params)
         lr_scheduler = self.lr_scheduler_class(optimizer, **self.lr_scheduler_params)
         return [optimizer], [lr_scheduler]
 
-    def training_step(self, batch: Tuple[List[Tensor], List[Dict[str, Tensor]]], batch_idx: int) -> Dict[str, Tensor]:
+    def training_step(self, batch: BATCH, batch_idx: int) -> STEP_OUTPUT:
         """Computes the training loss.
 
         Args:
-            batch: A tuple of images and targets. Images is a list of 3-dimensional tensors.
-                Targets is a list of dictionaries that contain ground-truth boxes, labels, etc.
-            batch_idx: The index of this batch.
+            batch: A tuple of images and targets. Images is a list of 3-dimensional tensors. Targets is a list of target
+                dictionaries.
+            batch_idx: Index of the current batch.
 
         Returns:
             A dictionary that includes the training loss in 'loss'.
         """
-        images, targets = self._validate_batch(batch)
+        images, targets = batch
         _, losses = self(images, targets)
-        total_loss = torch.stack(tuple(losses.values())).sum()
 
-        # sync_dist=True is broken in some versions of Lightning and may cause the sum of the loss
-        # across GPUs to be returned.
-        for name, value in losses.items():
-            self.log(f"train/{name}_loss", value, prog_bar=True, sync_dist=False)
-        self.log("train/total_loss", total_loss, sync_dist=False)
+        self.log("train/overlap_loss", losses[0], prog_bar=True, sync_dist=True)
+        self.log("train/confidence_loss", losses[1], prog_bar=True, sync_dist=True)
+        self.log("train/class_loss", losses[2], prog_bar=True, sync_dist=True)
+        self.log("train/total_loss", losses.sum(), sync_dist=True)
 
-        return {"loss": total_loss}
+        return {"loss": losses.sum()}
 
-    def validation_step(self, batch: Tuple[List[Tensor], List[Dict[str, Tensor]]], batch_idx: int):
+    def validation_step(self, batch: BATCH, batch_idx: int) -> Optional[STEP_OUTPUT]:
         """Evaluates a batch of data from the validation set.
 
         Args:
-            batch: A tuple of images and targets. Images is a list of 3-dimensional tensors.
-                Targets is a list of dictionaries that contain ground-truth boxes, labels, etc.
-            batch_idx: The index of this batch
+            batch: A tuple of images and targets. Images is a list of 3-dimensional tensors. Targets is a list of target
+                dictionaries.
+            batch_idx: Index of the current batch.
         """
-        images, targets = self._validate_batch(batch)
+        images, targets = batch
         detections, losses = self(images, targets)
-        detections = self._split_detections(detections)
-        detections = self._filter_detections(detections)
-        total_loss = torch.stack(tuple(losses.values())).sum()
-
-        for name, value in losses.items():
-            self.log(f"val/{name}_loss", value, sync_dist=True)
-        self.log("val/total_loss", total_loss, sync_dist=True)
 
-    def test_step(self, batch: Tuple[List[Tensor], List[Dict[str, Tensor]]], batch_idx: int):
+        self.log("val/overlap_loss", losses[0], sync_dist=True, batch_size=len(images))
+        self.log("val/confidence_loss", losses[1], sync_dist=True, batch_size=len(images))
+        self.log("val/class_loss", losses[2], sync_dist=True, batch_size=len(images))
+        self.log("val/total_loss", losses.sum(), sync_dist=True, batch_size=len(images))
+
+        if _MEAN_AVERAGE_PRECISION_AVAILABLE:
+            detections = self.process_detections(detections)
+            targets = self.process_targets(targets)
+            self._val_map.update(detections, targets)
+
+    def on_validation_epoch_end(self) -> None:
+        # When continuing training from a checkpoint, it may happen that epoch_end is called without detections. In this
+        # case the metrics cannot be computed.
+        if (not _MEAN_AVERAGE_PRECISION_AVAILABLE) or (not self._val_map.detections):
+            return
+
+        map_scores = self._val_map.compute()
+        map_scores = {"val/" + k: v for k, v in map_scores.items()}
+        self.log_dict(map_scores, sync_dist=True)
+        self._val_map.reset()
+
+    def test_step(self, batch: BATCH, batch_idx: int) -> Optional[STEP_OUTPUT]:
         """Evaluates a batch of data from the test set.
 
         Args:
-            batch: A tuple of images and targets. Images is a list of 3-dimensional tensors.
-                Targets is a list of dictionaries that contain ground-truth boxes, labels, etc.
-            batch_idx: The index of this batch.
+            batch: A tuple of images and targets. Images is a list of 3-dimensional tensors. Targets is a list of target
+                dictionaries.
+            batch_idx: Index of the current batch.
         """
-        images, targets = self._validate_batch(batch)
+        images, targets = batch
         detections, losses = self(images, targets)
-        detections = self._split_detections(detections)
-        detections = self._filter_detections(detections)
-        total_loss = torch.stack(tuple(losses.values())).sum()
-
-        for name, value in losses.items():
-            self.log(f"test/{name}_loss", value, sync_dist=True)
-        self.log("test/total_loss", total_loss, sync_dist=True)
 
-    def infer(self, image: Tensor) -> Tuple[Tensor, Tensor, Tensor]:
+        self.log("test/overlap_loss", losses[0], sync_dist=True)
+        self.log("test/confidence_loss", losses[1], sync_dist=True)
+        self.log("test/class_loss", losses[2], sync_dist=True)
+        self.log("test/total_loss", losses.sum(), sync_dist=True)
+
+        if _MEAN_AVERAGE_PRECISION_AVAILABLE:
+            detections = self.process_detections(detections)
+            targets = self.process_targets(targets)
+            self._test_map.update(detections, targets)
+
+    def on_test_epoch_end(self) -> None:
+        # When continuing training from a checkpoint, it may happen that epoch_end is called without detections. In this
+        # case the metrics cannot be computed.
+        if (not _MEAN_AVERAGE_PRECISION_AVAILABLE) or (not self._test_map.detections):
+            return
+
+        map_scores = self._test_map.compute()
+        map_scores = {"test/" + k: v for k, v in map_scores.items()}
+        self.log_dict(map_scores, sync_dist=True)
+        self._test_map.reset()
+
+    def predict_step(self, batch: BATCH, batch_idx: int, dataloader_idx: int = 0) -> List[PRED]:
+        """Feeds a batch of images to the network and returns the detected bounding boxes, confidence scores, and
+        class labels.
+
+        If a prediction has a high score for more than one class, it will be duplicated.
+
+        Args:
+            batch: A tuple of images and targets. Images is a list of 3-dimensional tensors. Targets is a list of target
+                dictionaries.
+            batch_idx: Index of the current batch.
+            dataloader_idx: Index of the current dataloader.
+
+        Returns:
+            A list of dictionaries containing tensors "boxes", "scores", and "labels". "boxes" is a matrix of detected
+            bounding box `(x1, y1, x2, y2)` coordinates. "scores" is a vector of confidence scores for the bounding box
+            detections. "labels" is a vector of predicted class labels.
+        """
+        images, _ = batch
+        detections = self(images)
+        detections = self.process_detections(detections)
+        return detections
+
+    def infer(self, image: Tensor) -> PRED:
         """Feeds an image to the network and returns the detected bounding boxes, confidence scores, and class
         labels.
 
+        If a prediction has a high score for more than one class, it will be duplicated.
+
         Args:
             image: An input image, a tensor of uint8 values sized ``[channels, height, width]``.
 
         Returns:
-            boxes (:class:`~torch.Tensor`), confidences (:class:`~torch.Tensor`), labels (:class:`~torch.Tensor`):
-            A matrix of detected bounding box `(x1, y1, x2, y2)` coordinates, a vector of
-            confidences for the bounding box detections, and a vector of predicted class labels.
+            A dictionary containing tensors "boxes", "scores", and "labels". "boxes" is a matrix of detected bounding
+            box `(x1, y1, x2, y2)` coordinates. "scores" is a vector of confidence scores for the bounding box
+            detections. "labels" is a vector of predicted class labels.
         """
-        if not isinstance(image, torch.Tensor):
-            image = F.to_tensor(image)
+        if not isinstance(image, Tensor):
+            image = T.to_tensor(image)
 
+        was_training = self.training
         self.eval()
-        detections = self(image.unsqueeze(0))
-        detections = self._split_detections(detections)
-        detections = self._filter_detections(detections)
-        boxes = detections["boxes"][0]
-        scores = detections["scores"][0]
-        labels = detections["labels"][0]
-        return boxes, scores, labels
-
-    def load_darknet_weights(self, weight_file):
-        """Loads weights to layer modules from a pretrained Darknet model.
-
-        One may want to continue training from the pretrained weights, on a dataset with a
-        different number of object categories. The number of kernels in the convolutional layers
-        just before each detection layer depends on the number of output classes. The Darknet
-        solution is to truncate the weight file and stop reading weights at the first incompatible
-        layer. For this reason the function silently leaves the rest of the layers unchanged, when
-        the weight file ends.
+
+        detections = self([image])
+        detections = self.process_detections(detections)
+        detections = detections[0]
+
+        if was_training:
+            self.train()
+        return detections
+
+    def process_detections(self, preds: Tensor) -> List[PRED]:
+        """Splits the detection tensor returned by a forward pass into a list of prediction dictionaries, and
+        filters them based on confidence threshold, non-maximum suppression (NMS), and maximum number of
+        predictions.
+
+        If for any single detection there are multiple categories whose score is above the confidence threshold, the
+        detection will be duplicated to create one detection for each category. NMS processes one category at a time,
+        iterating over the bounding boxes in descending order of confidence score, and removes lower scoring boxes that
+        have an IoU greater than the NMS threshold with a higher scoring box.
+
+        The returned detections are sorted by descending confidence. The items of the dictionaries are as follows:
+        - boxes (``Tensor[batch_size, N, 4]``): detected bounding box `(x1, y1, x2, y2)` coordinates
+        - scores (``Tensor[batch_size, N]``): detection confidences
+        - labels (``Int64Tensor[batch_size, N]``): the predicted class IDs
 
         Args:
-            weight_file: A file object containing model weights in the Darknet binary format.
+            preds: A tensor of detected bounding boxes and their attributes.
+
+        Returns:
+            Filtered detections. A list of prediction dictionaries, one for each image.
         """
-        version = np.fromfile(weight_file, count=3, dtype=np.int32)
-        images_seen = np.fromfile(weight_file, count=1, dtype=np.int64)
-        rank_zero_info(
-            f"Loading weights from Darknet model version {version[0]}.{version[1]}.{version[2]} "
-            f"that has been trained on {images_seen[0]} images."
-        )
-
-        def read(tensor):
-            """Reads the contents of ``tensor`` from the current position of ``weight_file``.
-
-            If there's no more data in ``weight_file``, returns without error.
-            """
-            x = np.fromfile(weight_file, count=tensor.numel(), dtype=np.float32)
-            if x.shape[0] == 0:
-                return
-            x = torch.from_numpy(x).view_as(tensor)
-            with torch.no_grad():
-                tensor.copy_(x)
-
-        for module in self.network:
-            # Weights are loaded only to convolutional layers
-            if not isinstance(module, nn.Sequential):
-                continue
-
-            conv = module[0]
-            assert isinstance(conv, nn.Conv2d)
-
-            # Convolution may be followed by batch normalization, in which case we read the batch
-            # normalization parameters and not the convolution bias.
-            if len(module) > 1 and isinstance(module[1], nn.BatchNorm2d):
-                bn = module[1]
-                read(bn.bias)
-                read(bn.weight)
-                read(bn.running_mean)
-                read(bn.running_var)
-            else:
-                read(conv.bias)
-
-            read(conv.weight)
-
-    def _validate_batch(
-        self, batch: Tuple[List[Tensor], List[Dict[str, Tensor]]]
-    ) -> Tuple[Tensor, List[Dict[str, Tensor]]]:
-        """Reads a batch of data, validates the format, and stacks the images into a single tensor.
+
+        def process(boxes: Tensor, confidences: Tensor, classprobs: Tensor) -> Dict[str, Any]:
+            scores = classprobs * confidences[:, None]
+
+            # Select predictions with high scores. If a prediction has a high score for more than one class, it will be
+            # duplicated.
+            idxs, labels = (scores > self.confidence_threshold).nonzero().T
+            boxes = boxes[idxs]
+            scores = scores[idxs, labels]
+
+            keep = batched_nms(boxes, scores, labels, self.nms_threshold)
+            keep = keep[: self.detections_per_image]
+            return {"boxes": boxes[keep], "scores": scores[keep], "labels": labels[keep]}
+
+        return [process(p[..., :4], p[..., 4], p[..., 5:]) for p in preds]
+
+    def process_targets(self, targets: TARGETS) -> List[TARGET]:
+        """Duplicates multi-label targets to create one target for each label.
 
         Args:
-            batch: The batch of data read by the :class:`~torch.utils.data.DataLoader`.
+            targets: List of target dictionaries. Each dictionary must contain "boxes" and "labels". "labels" is either
+                a one-dimensional list of class IDs, or a two-dimensional boolean class map.
 
         Returns:
-            The input batch with images stacked into a single tensor.
+            Single-label targets. A list of target dictionaries, one for each image.
         """
-        images, targets = batch
 
+        def process(boxes: Tensor, labels: Tensor, **other: Any) -> Dict[str, Any]:
+            if labels.ndim == 2:
+                idxs, labels = labels.nonzero().T
+                boxes = boxes[idxs]
+            return {"boxes": boxes, "labels": labels, **other}
+
+        return [process(**t) for t in targets]
+
+    def validate_batch(self, images: Union[Tensor, IMAGES], targets: Optional[TARGETS]) -> None:
+        """Validates the format of a batch of data.
+
+        Args:
+            images: A tensor containing a batch of images or a list of image tensors.
+            targets: A list of target dictionaries or ``None``. If a list is provided, there should be as many target
+                dictionaries as there are images.
+        """
+        if not isinstance(images, Tensor):
+            if not isinstance(images, (tuple, list)):
+                raise TypeError(f"Expected images to be a Tensor, tuple, or a list, got {type(images).__name__}.")
+            if not images:
+                raise ValueError("No images in batch.")
+            shape = images[0].shape
+            for image in images:
+                if not isinstance(image, Tensor):
+                    raise ValueError(f"Expected image to be of type Tensor, got {type(image).__name__}.")
+                if image.shape != shape:
+                    raise ValueError(f"Images with different shapes in one batch: {shape} and {image.shape}")
+
+        if targets is None:
+            if self.training:
+                raise ValueError("Targets should be given in training mode.")
+            return
+
+        if not isinstance(targets, (tuple, list)):
+            raise TypeError(f"Expected targets to be a tuple or a list, got {type(images).__name__}.")
         if len(images) != len(targets):
             raise ValueError(f"Got {len(images)} images, but targets for {len(targets)} images.")
 
-        for image in images:
-            if not isinstance(image, Tensor):
-                raise ValueError(f"Expected image to be of type Tensor, got {type(image)}.")
-
         for target in targets:
+            if "boxes" not in target:
+                raise ValueError("Target dictionary doesn't contain boxes.")
             boxes = target["boxes"]
             if not isinstance(boxes, Tensor):
-                raise ValueError(f"Expected target boxes to be of type Tensor, got {type(boxes)}.")
-            if (len(boxes.shape) != 2) or (boxes.shape[-1] != 4):
+                raise TypeError(f"Expected target boxes to be of type Tensor, got {type(boxes).__name__}.")
+            if (boxes.ndim != 2) or (boxes.shape[-1] != 4):
                 raise ValueError(f"Expected target boxes to be tensors of shape [N, 4], got {list(boxes.shape)}.")
+            if "labels" not in target:
+                raise ValueError("Target dictionary doesn't contain labels.")
             labels = target["labels"]
             if not isinstance(labels, Tensor):
-                raise ValueError(f"Expected target labels to be of type Tensor, got {type(labels)}.")
-            if len(labels.shape) != 1:
-                raise ValueError(f"Expected target labels to be tensors of shape [N], got {list(labels.shape)}.")
-
-        images = torch.stack(images)
-        return images, targets
-
-    def _split_detections(self, detections: Tensor) -> Dict[str, Tensor]:
-        """Splits the detection tensor returned by a forward pass into a dictionary.
-
-        The fields of the dictionary are as follows:
-            - boxes (``Tensor[batch_size, N, 4]``): detected bounding box `(x1, y1, x2, y2)` coordinates
-            - scores (``Tensor[batch_size, N]``): detection confidences
-            - classprobs (``Tensor[batch_size, N]``): probabilities of the best classes
-            - labels (``Int64Tensor[batch_size, N]``): the predicted labels for each image
+                raise ValueError(f"Expected target labels to be of type Tensor, got {type(labels).__name__}.")
+            if (labels.ndim < 1) or (labels.ndim > 2) or (len(labels) != len(boxes)):
+                raise ValueError(
+                    f"Expected target labels to be tensors of shape [N] or [N, num_classes], got {list(labels.shape)}."
+                )
 
-        Args:
-            detections: A tensor of detected bounding boxes and their attributes.
 
-        Returns:
-            A dictionary of detection results.
-        """
-        boxes = detections[..., :4]
-        scores = detections[..., 4]
-        classprobs = detections[..., 5:]
-        classprobs, labels = torch.max(classprobs, -1)
-        return {"boxes": boxes, "scores": scores, "classprobs": classprobs, "labels": labels}
-
-    def _filter_detections(self, detections: Dict[str, Tensor]) -> Dict[str, List[Tensor]]:
-        """Filters detections based on confidence threshold. Then for every class performs non-maximum suppression
-        (NMS). NMS iterates the bounding boxes that predict this class in descending order of confidence score, and
-        removes lower scoring boxes that have an IoU greater than the NMS threshold with a higher scoring box.
-        Finally the detections are sorted by descending confidence and possible truncated to the maximum number of
-        predictions.
+class CLIYOLO(YOLO):
+    """A subclass of YOLO that can be easily configured using LightningCLI.
+
+    Either loads a Darknet configuration file, or constructs a YOLOv4 network. This is just an example of how to use the
+    model. Various other network architectures from ``torch_networks.py`` can be used. Note that if you change the
+    resolution of the input images, you should also scale the prior shapes (a.k.a. anchors). They are specified in the
+    Darknet configuration file or provided in the network constructor parameters.
 
-        Args:
-            detections: All detections. A dictionary of tensors, each containing the predictions
-                from all images.
+    CLI command::
 
-        Returns:
-            Filtered detections. A dictionary of lists, each containing a tensor per image.
-        """
-        boxes = detections["boxes"]
-        scores = detections["scores"]
-        classprobs = detections["classprobs"]
-        labels = detections["labels"]
-
-        out_boxes = []
-        out_scores = []
-        out_classprobs = []
-        out_labels = []
-
-        for img_boxes, img_scores, img_classprobs, img_labels in zip(boxes, scores, classprobs, labels):
-            # Select detections with high confidence score.
-            selected = img_scores > self.confidence_threshold
-            img_boxes = img_boxes[selected]
-            img_scores = img_scores[selected]
-            img_classprobs = img_classprobs[selected]
-            img_labels = img_labels[selected]
-
-            img_out_boxes = boxes.new_zeros((0, 4))
-            img_out_scores = scores.new_zeros(0)
-            img_out_classprobs = classprobs.new_zeros(0)
-            img_out_labels = labels.new_zeros(0)
-
-            # Iterate through the unique object classes detected in the image and perform non-maximum
-            # suppression for the objects of the class in question.
-            for cls_label in labels.unique():
-                selected = img_labels == cls_label
-                cls_boxes = img_boxes[selected]
-                cls_scores = img_scores[selected]
-                cls_classprobs = img_classprobs[selected]
-                cls_labels = img_labels[selected]
-
-                # NMS will crash if there are too many boxes.
-                cls_boxes = cls_boxes[:100000]
-                cls_scores = cls_scores[:100000]
-                selected = nms(cls_boxes, cls_scores, self.nms_threshold)
-
-                img_out_boxes = torch.cat((img_out_boxes, cls_boxes[selected]))
-                img_out_scores = torch.cat((img_out_scores, cls_scores[selected]))
-                img_out_classprobs = torch.cat((img_out_classprobs, cls_classprobs[selected]))
-                img_out_labels = torch.cat((img_out_labels, cls_labels[selected]))
-
-            # Sort by descending confidence and limit the maximum number of predictions.
-            indices = torch.argsort(img_out_scores, descending=True)
-            if self.max_predictions_per_image >= 0:
-                indices = indices[: self.max_predictions_per_image]
-            out_boxes.append(img_out_boxes[indices])
-            out_scores.append(img_out_scores[indices])
-            out_classprobs.append(img_out_classprobs[indices])
-            out_labels.append(img_out_labels[indices])
-
-        return {"boxes": out_boxes, "scores": out_scores, "classprobs": out_classprobs, "labels": out_labels}
-
-
-@under_review()
-class Resize:
-    """Rescales the image and target to given dimensions.
+        # Darknet network configuration
+        wget https://raw.githubusercontent.com/AlexeyAB/darknet/master/cfg/yolov4-tiny-3l.cfg
+        python yolo_module.py fit \
+            --model.network_config yolov4-tiny-3l.cfg \
+            --data.batch_size 8 \
+            --data.num_workers 4 \
+            --trainer.accelerator gpu \
+            --trainer.devices 8 \
+            --trainer.accumulate_grad_batches 2 \
+            --trainer.gradient_clip_val 5.0 \
+            --trainer.max_epochs=100
+
+        # YOLOv4
+        python yolo_module.py fit \
+            --data.batch_size 8 \
+            --data.num_workers 4 \
+            --trainer.accelerator gpu \
+            --trainer.devices 8 \
+            --trainer.accumulate_grad_batches 2 \
+            --trainer.gradient_clip_val 5.0 \
+            --trainer.max_epochs=100
 
     Args:
-        output_size (tuple or int): Desired output size. If tuple (height, width), the output is
-            matched to ``output_size``. If int, the smaller of the image edges is matched to
-            ``output_size``, keeping the aspect ratio the same.
+        network_config: Path to a Darknet configuration file that defines the network architecture. If not given, a
+            YOLOv4 network will be constructed.
+        matching_algorithm: Which algorithm to use for matching targets to anchors. "simota" (the SimOTA matching rule
+            from YOLOX), "size" (match those prior shapes, whose width and height relative to the target is below given
+            ratio), "iou" (match all prior shapes that give a high enough IoU), or "maxiou" (match the prior shape that
+            gives the highest IoU, default).
+        matching_threshold: Threshold for "size" and "iou" matching algorithms.
+        spatial_range: The "simota" matching algorithm will restrict to anchors that are within an `N × N` grid cell
+            area centered at the target, where `N` is the value of this parameter.
+        size_range: The "simota" matching algorithm will restrict to anchors whose dimensions are no more than `N` and
+            no less than `1/N` times the target dimensions, where `N` is the value of this parameter.
+        ignore_bg_threshold: If a predictor is not responsible for predicting any target, but the corresponding anchor
+            has IoU with some target greater than this threshold, the predictor will not be taken into account when
+            calculating the confidence loss.
+        overlap_func: A function for calculating the pairwise overlaps between two sets of boxes. Valid values are
+            "iou", "giou", "diou", and "ciou".
+        predict_overlap: Balance between binary confidence targets and predicting the overlap. 0.0 means that target
+            confidence is one if there's an object, and 1.0 means that the target confidence is the output of
+            ``overlap_func``.
+        overlap_loss_multiplier: Overlap loss will be scaled by this value.
+        confidence_loss_multiplier: Confidence loss will be scaled by this value.
+        class_loss_multiplier: Classification loss will be scaled by this value.
     """
 
-    def __init__(self, output_size: tuple) -> None:
-        self.output_size = output_size
+    def __init__(
+        self,
+        network_config: Optional[str] = None,
+        darknet_weights: Optional[str] = None,
+        matching_algorithm: Optional[str] = None,
+        matching_threshold: Optional[float] = None,
+        spatial_range: float = 5.0,
+        size_range: float = 4.0,
+        ignore_bg_threshold: Optional[float] = None,
+        overlap_func: Optional[str] = None,
+        predict_overlap: Optional[float] = None,
+        overlap_loss_multiplier: Optional[float] = None,
+        confidence_loss_multiplier: Optional[float] = None,
+        class_loss_multiplier: Optional[float] = None,
+        **kwargs: Any,
+    ) -> None:
+        if network_config is not None:
+            network: nn.Module = DarknetNetwork(
+                network_config,
+                darknet_weights,
+                matching_algorithm=matching_algorithm,
+                matching_threshold=matching_threshold,
+                spatial_range=spatial_range,
+                size_range=size_range,
+                ignore_bg_threshold=ignore_bg_threshold,
+                overlap_func=overlap_func,
+                predict_overlap=predict_overlap,
+                overlap_loss_multiplier=overlap_loss_multiplier,
+                confidence_loss_multiplier=confidence_loss_multiplier,
+                class_loss_multiplier=class_loss_multiplier,
+            )
+        else:
+            # We need to set some defaults, since we don't get the default values from a configuration file.
+            if ignore_bg_threshold is None:
+                ignore_bg_threshold = 0.7
+            if overlap_func is None:
+                overlap_func = "ciou"
+            if overlap_loss_multiplier is None:
+                overlap_loss_multiplier = 5.0
+            if confidence_loss_multiplier is None:
+                confidence_loss_multiplier = 1.0
+            if class_loss_multiplier is None:
+                class_loss_multiplier = 1.0
+
+            network = YOLOV4Network(
+                num_classes=21,  # The number of classes in Pascal VOC dataset.
+                matching_algorithm=matching_algorithm,
+                matching_threshold=matching_threshold,
+                spatial_range=spatial_range,
+                size_range=size_range,
+                ignore_bg_threshold=ignore_bg_threshold,
+                overlap_func=overlap_func,
+                predict_overlap=predict_overlap,
+                overlap_loss_multiplier=overlap_loss_multiplier,
+                confidence_loss_multiplier=confidence_loss_multiplier,
+                class_loss_multiplier=class_loss_multiplier,
+            )
+        super().__init__(**kwargs, network=network)
+
+
+class ResizedVOCDetectionDataModule(VOCDetectionDataModule):
+    """A subclass of ``VOCDetectionDataModule`` that resizes the images to a specific size. YOLO expectes the image
+    size to be divisible by the ratio in which the network downsamples the image.
+
+    Args:
+        width: Resize images to this width.
+        height: Resize images to this height.
+    """
+
+    def __init__(self, width: int = 608, height: int = 608, **kwargs: Any):
+        super().__init__(**kwargs)
+        self.image_size = (height, width)
+
+    def default_transforms(self) -> Callable:
+        transforms = [
+            lambda image, target: (T.to_tensor(image), target),
+            self._resize,
+        ]
+        if self.normalize:
+            transforms += [
+                lambda image, target: (
+                    T.normalize(image, mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+                    target,
+                )
+            ]
+        return Compose(transforms)
+
+    def _resize(self, image: Tensor, target: TARGET) -> Tuple[Tensor, TARGET]:
+        """Rescales the image and target to ``self.image_size``.
 
-    def __call__(self, image: Tensor, target: Dict[str, Any]):
-        """
         Args:
-            tensor: Tensor image to be resized.
+            tensor: Image tensor to be resized.
             target: Dictionary of detection targets.
 
         Returns:
-            Resized Tensor image.
+            Resized image tensor.
         """
+        device = target["boxes"].device
         height, width = image.shape[-2:]
-        original_size = torch.tensor([height, width])
-        scale_y, scale_x = torch.tensor(self.output_size) / original_size
-        scale = torch.tensor([scale_x, scale_y, scale_x, scale_y], device=target["boxes"].device)
-        image = F.resize(image, self.output_size)
+        original_size = torch.tensor([height, width], device=device)
+        scale_y, scale_x = torch.tensor(self.image_size, device=device) / original_size
+        scale = torch.tensor([scale_x, scale_y, scale_x, scale_y], device=device)
+        image = T.resize(image, self.image_size)
         target["boxes"] = target["boxes"] * scale
         return image, target
 
 
-@under_review()
-def run_cli():
-    from argparse import ArgumentParser
-
-    from pytorch_lightning import Trainer, seed_everything
-
-    from pl_bolts.datamodules import VOCDetectionDataModule
-    from pl_bolts.datamodules.vocdetection_datamodule import Compose
-    from pl_bolts.models.detection.yolo.yolo_config import YOLOConfiguration
-
-    seed_everything(42)
-
-    parser = ArgumentParser()
-    parser.add_argument(
-        "--config",
-        type=str,
-        metavar="PATH",
-        required=True,
-        help="read model configuration from PATH",
-    )
-    parser.add_argument(
-        "--darknet-weights",
-        type=str,
-        metavar="PATH",
-        help="read the initial model weights from PATH in Darknet format",
-    )
-    parser.add_argument(
-        "--lr",
-        type=float,
-        metavar="LR",
-        default=0.0013,
-        help="learning rate after the warmup period",
-    )
-    parser.add_argument(
-        "--momentum",
-        type=float,
-        metavar="GAMMA",
-        default=0.9,
-        help="if nonzero, the optimizer uses momentum with factor GAMMA",
-    )
-    parser.add_argument(
-        "--weight-decay",
-        type=float,
-        metavar="LAMBDA",
-        default=0.0005,
-        help="if nonzero, the optimizer uses weight decay (L2 penalty) with factor LAMBDA",
-    )
-    parser.add_argument(
-        "--warmup-epochs",
-        type=int,
-        metavar="N",
-        default=1,
-        help="learning rate warmup period is N epochs",
-    )
-    parser.add_argument(
-        "--max-epochs",
-        type=int,
-        metavar="N",
-        default=300,
-        help="train at most N epochs",
-    )
-    parser.add_argument(
-        "--initial-lr",
-        type=float,
-        metavar="LR",
-        default=0.0,
-        help="learning rate before the warmup period",
-    )
-    parser.add_argument(
-        "--confidence-threshold",
-        type=float,
-        metavar="THRESHOLD",
-        default=0.001,
-        help="keep predictions only if the confidence is above THRESHOLD",
-    )
-    parser.add_argument(
-        "--nms-threshold",
-        type=float,
-        metavar="THRESHOLD",
-        default=0.45,
-        help="non-maximum suppression removes predicted boxes that have IoU greater than "
-        "THRESHOLD with a higher scoring box",
-    )
-    parser.add_argument(
-        "--max-predictions-per-image",
-        type=int,
-        metavar="N",
-        default=100,
-        help="keep at most N best predictions",
-    )
-
-    parser = VOCDetectionDataModule.add_argparse_args(parser)
-    parser = Trainer.add_argparse_args(parser)
-    args = parser.parse_args()
-
-    config = YOLOConfiguration(args.config)
-
-    transforms = [lambda image, target: (F.to_tensor(image), target), Resize((config.height, config.width))]
-    transforms = Compose(transforms)
-    datamodule = VOCDetectionDataModule.from_argparse_args(args, train_transforms=transforms, val_transforms=transforms)
-
-    optimizer_params = {"lr": args.lr, "momentum": args.momentum, "weight_decay": args.weight_decay}
-    lr_scheduler_params = {
-        "warmup_epochs": args.warmup_epochs,
-        "max_epochs": args.max_epochs,
-        "warmup_start_lr": args.initial_lr,
-    }
-    model = YOLO(
-        network=config.get_network(),
-        optimizer_params=optimizer_params,
-        lr_scheduler_params=lr_scheduler_params,
-        confidence_threshold=args.confidence_threshold,
-        nms_threshold=args.nms_threshold,
-        max_predictions_per_image=args.max_predictions_per_image,
-    )
-    if args.darknet_weights is not None:
-        with open(args.darknet_weights) as weight_file:
-            model.load_darknet_weights(weight_file)
-
-    trainer = Trainer.from_argparse_args(args)
-    trainer.fit(model, datamodule=datamodule)
-
-
 if __name__ == "__main__":
-    run_cli()
+    LightningCLI(CLIYOLO, ResizedVOCDetectionDataModule, seed_everything_default=42)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/basic/basic_gan_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/basic/basic_gan_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from argparse import ArgumentParser
 
 import torch
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from pytorch_lightning.callbacks.progress import TQDMProgressBar
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.models.gans.basic.components import Discriminator, Generator
 
 
 class GAN(LightningModule):
     """Vanilla GAN implementation.
 
@@ -33,15 +33,15 @@
         self,
         input_channels: int,
         input_height: int,
         input_width: int,
         latent_dim: int = 32,
         learning_rate: float = 0.0002,
         **kwargs
-    ):
+    ) -> None:
         """
         Args:
             input_channels: number of channels of an image
             input_height: image height
             input_width: image width
             latent_dim: emb dim for encoder
             learning_rate: the learning rate
@@ -53,20 +53,18 @@
         self.img_dim = (input_channels, input_height, input_width)
 
         # networks
         self.generator = self.init_generator(self.img_dim)
         self.discriminator = self.init_discriminator(self.img_dim)
 
     def init_generator(self, img_dim):
-        generator = Generator(latent_dim=self.hparams.latent_dim, img_shape=img_dim)
-        return generator
+        return Generator(latent_dim=self.hparams.latent_dim, img_shape=img_dim)
 
     def init_discriminator(self, img_dim):
-        discriminator = Discriminator(img_shape=img_dim)
-        return discriminator
+        return Discriminator(img_shape=img_dim)
 
     def forward(self, z):
         """Generates an image given input noise z.
 
         Example::
 
             z = torch.rand(batch_size, latent_dim)
@@ -79,64 +77,50 @@
         # sample noise
         z = torch.randn(x.shape[0], self.hparams.latent_dim, device=self.device)
         y = torch.ones(x.size(0), 1, device=self.device)
 
         # generate images
         generated_imgs = self(z)
 
-        D_output = self.discriminator(generated_imgs)
-
         # ground truth result (ie: all real)
-        g_loss = F.binary_cross_entropy(D_output, y)
-
-        return g_loss
+        return F.binary_cross_entropy(self.discriminator(generated_imgs), y)
 
     def discriminator_loss(self, x):
         # train discriminator on real
         b = x.size(0)
         x_real = x
         y_real = torch.ones(b, 1, device=self.device)
 
         # calculate real score
-        D_output = self.discriminator(x_real)
-        D_real_loss = F.binary_cross_entropy(D_output, y_real)
+        real_loss = F.binary_cross_entropy(self.discriminator(x_real), y_real)
 
         # train discriminator on fake
         z = torch.randn(b, self.hparams.latent_dim, device=self.device)
         x_fake = self(z)
         y_fake = torch.zeros(b, 1, device=self.device)
 
         # calculate fake score
-        D_output = self.discriminator(x_fake)
-        D_fake_loss = F.binary_cross_entropy(D_output, y_fake)
+        fake_loss = F.binary_cross_entropy(self.discriminator(x_fake), y_fake)
 
         # gradient backprop & optimize ONLY D's parameters
-        D_loss = D_real_loss + D_fake_loss
-
-        return D_loss
+        return real_loss + fake_loss
 
     def training_step(self, batch, batch_idx, optimizer_idx):
         x, _ = batch
-
         # train generator
-        result = None
         if optimizer_idx == 0:
-            result = self.generator_step(x)
-
+            return self.generator_step(x)
         # train discriminator
         if optimizer_idx == 1:
-            result = self.discriminator_step(x)
-
-        return result
+            return self.discriminator_step(x)
+        return None
 
     def generator_step(self, x):
         g_loss = self.generator_loss(x)
-
-        # log to prog bar on each step AND for the full epoch
-        # use the generator loss for checkpointing
+        # log to prog bar on each step AND for the full epoch use the generator loss for checkpointing
         self.log("g_loss", g_loss, on_epoch=True, prog_bar=True)
         return g_loss
 
     def discriminator_step(self, x):
         # Measure discriminator's ability to classify real from generated samples
         d_loss = self.discriminator_loss(x)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/basic/components.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/basic/components.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import torch
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 
 class Generator(nn.Module):
-    def __init__(self, latent_dim, img_shape, hidden_dim=256):
+    def __init__(self, latent_dim, img_shape, hidden_dim=256) -> None:
         super().__init__()
         feats = int(np.prod(img_shape))
         self.img_shape = img_shape
         self.fc1 = nn.Linear(latent_dim, hidden_dim)
         self.fc2 = nn.Linear(self.fc1.out_features, self.fc1.out_features * 2)
         self.fc3 = nn.Linear(self.fc2.out_features, self.fc2.out_features * 2)
         self.fc4 = nn.Linear(self.fc3.out_features, feats)
@@ -21,15 +21,15 @@
         z = F.leaky_relu(self.fc3(z), 0.2)
         img = torch.tanh(self.fc4(z))
         img = img.view(img.size(0), *self.img_shape)
         return img
 
 
 class Discriminator(nn.Module):
-    def __init__(self, img_shape, hidden_dim=1024):
+    def __init__(self, img_shape, hidden_dim=1024) -> None:
         super().__init__()
         in_dim = int(np.prod(img_shape))
         self.fc1 = nn.Linear(in_dim, hidden_dim)
         self.fc2 = nn.Linear(self.fc1.out_features, self.fc1.out_features // 2)
         self.fc3 = nn.Linear(self.fc2.out_features, self.fc2.out_features // 2)
         self.fc4 = nn.Linear(self.fc3.out_features, 1)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/dcgan/components.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/dcgan/components.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/dcgan/dcgan_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/dcgan/dcgan_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,33 +134,28 @@
         real_loss = self.criterion(real_pred, real_gt)
 
         # Train with fake
         fake_pred = self._get_fake_pred(real)
         fake_gt = torch.zeros_like(fake_pred)
         fake_loss = self.criterion(fake_pred, fake_gt)
 
-        disc_loss = real_loss + fake_loss
-
-        return disc_loss
+        # disc_loss
+        return real_loss + fake_loss
 
     def _get_gen_loss(self, real: Tensor) -> Tensor:
         # Train with fake
         fake_pred = self._get_fake_pred(real)
         fake_gt = torch.ones_like(fake_pred)
-        gen_loss = self.criterion(fake_pred, fake_gt)
-
-        return gen_loss
+        return self.criterion(fake_pred, fake_gt)
 
     def _get_fake_pred(self, real: Tensor) -> Tensor:
         batch_size = len(real)
         noise = self._get_noise(batch_size, self.hparams.latent_dim)
         fake = self(noise)
-        fake_pred = self.discriminator(fake)
-
-        return fake_pred
+        return self.discriminator(fake)
 
     def _get_noise(self, n_samples: int, latent_dim: int) -> Tensor:
         return torch.randn(n_samples, latent_dim, device=self.device)
 
     @staticmethod
     def add_model_specific_args(parent_parser: ArgumentParser) -> ArgumentParser:
         parser = ArgumentParser(parents=[parent_parser], add_help=False)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/pix2pix/components.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/pix2pix/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class UpSampleConv(nn.Module):
     def __init__(
         self, in_channels, out_channels, kernel=4, strides=2, padding=1, activation=True, batchnorm=True, dropout=False
-    ):
+    ) -> None:
         super().__init__()
         self.activation = activation
         self.batchnorm = batchnorm
         self.dropout = dropout
 
         self.deconv = nn.ConvTranspose2d(in_channels, out_channels, kernel, strides, padding)
 
@@ -33,15 +33,17 @@
         if self.dropout:
             x = self.drop(x)
         return x
 
 
 @under_review()
 class DownSampleConv(nn.Module):
-    def __init__(self, in_channels, out_channels, kernel=4, strides=2, padding=1, activation=True, batchnorm=True):
+    def __init__(
+        self, in_channels, out_channels, kernel=4, strides=2, padding=1, activation=True, batchnorm=True
+    ) -> None:
         """Paper details:
 
         - C64-C128-C256-C512-C512-C512-C512-C512
         - All convolutions are 4×4 spatial filters applied with stride 2
         - Convolutions in the encoder downsample by a factor of 2
         """
         super().__init__()
@@ -63,15 +65,15 @@
         if self.activation:
             x = self.act(x)
         return x
 
 
 @under_review()
 class Generator(nn.Module):
-    def __init__(self, in_channels, out_channels):
+    def __init__(self, in_channels, out_channels) -> None:
         """Paper details:
 
         - Encoder: C64-C128-C256-C512-C512-C512-C512-C512
         - All convolutions are 4×4 spatial filters applied with stride 2
         - Convolutions in the encoder downsample by a factor of 2
         - Decoder: CD512-CD1024-CD1024-C1024-C1024-C512 -C256-C128
         """
@@ -125,23 +127,22 @@
         # print(x.shape)
         x = self.final_conv(x)
         return self.tanh(x)
 
 
 @under_review()
 class PatchGAN(nn.Module):
-    def __init__(self, input_channels):
+    def __init__(self, input_channels) -> None:
         super().__init__()
         self.d1 = DownSampleConv(input_channels, 64, batchnorm=False)
         self.d2 = DownSampleConv(64, 128)
         self.d3 = DownSampleConv(128, 256)
         self.d4 = DownSampleConv(256, 512)
         self.final = nn.Conv2d(512, 1, kernel_size=1)
 
     def forward(self, x, y):
         x = torch.cat([x, y], axis=1)
         x0 = self.d1(x)
         x1 = self.d2(x0)
         x2 = self.d3(x1)
         x3 = self.d4(x2)
-        xn = self.final(x3)
-        return xn
+        return self.final(x3)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/pix2pix/pix2pix_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/pix2pix/pix2pix_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     if isinstance(m, nn.BatchNorm2d):
         torch.nn.init.normal_(m.weight, 0.0, 0.02)
         torch.nn.init.constant_(m.bias, 0)
 
 
 @under_review()
 class Pix2Pix(LightningModule):
-    def __init__(self, in_channels, out_channels, learning_rate=0.0002, lambda_recon=200):
-
+    def __init__(self, in_channels, out_channels, learning_rate=0.0002, lambda_recon=200) -> None:
         super().__init__()
         self.save_hyperparameters()
 
         self.gen = Generator(in_channels, out_channels)
         self.patch_gan = PatchGAN(in_channels + out_channels)
 
         # intializing weights
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/srgan/components.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/srgan/components.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/srgan/srgan_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/srgan/srgan_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Any, List, Optional, Tuple
 from warnings import warn
 
 import pytorch_lightning as pl
 import torch
-import torch.nn.functional as F
+import torch.nn.functional as F  # noqa: N812
 
 from pl_bolts.callbacks import SRImageLoggerCallback
 from pl_bolts.datamodules import TVTDataModule
 from pl_bolts.datasets.utils import prepare_sr_datasets
 from pl_bolts.models.gans.srgan.components import SRGANDiscriminator, SRGANGenerator, VGG19FeatureExtractor
 from pl_bolts.utils.stability import under_review
 
@@ -133,45 +133,39 @@
     def _disc_loss(self, hr_image: torch.Tensor, lr_image: torch.Tensor) -> torch.Tensor:
         real_pred = self.discriminator(hr_image)
         real_loss = self._adv_loss(real_pred, ones=True)
 
         _, fake_pred = self._fake_pred(lr_image)
         fake_loss = self._adv_loss(fake_pred, ones=False)
 
-        disc_loss = 0.5 * (real_loss + fake_loss)
-
-        return disc_loss
+        return 0.5 * (real_loss + fake_loss)
 
     def _gen_loss(self, hr_image: torch.Tensor, lr_image: torch.Tensor) -> torch.Tensor:
         fake, fake_pred = self._fake_pred(lr_image)
 
         perceptual_loss = self._perceptual_loss(hr_image, fake)
         adv_loss = self._adv_loss(fake_pred, ones=True)
         content_loss = self._content_loss(hr_image, fake)
 
-        gen_loss = 0.006 * perceptual_loss + 0.001 * adv_loss + content_loss
-
-        return gen_loss
+        return 0.006 * perceptual_loss + 0.001 * adv_loss + content_loss
 
     def _fake_pred(self, lr_image: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         fake = self(lr_image)
         fake_pred = self.discriminator(fake)
         return fake, fake_pred
 
     @staticmethod
     def _adv_loss(pred: torch.Tensor, ones: bool) -> torch.Tensor:
         target = torch.ones_like(pred) if ones else torch.zeros_like(pred)
-        adv_loss = F.binary_cross_entropy_with_logits(pred, target)
-        return adv_loss
+        return F.binary_cross_entropy_with_logits(pred, target)
 
     def _perceptual_loss(self, hr_image: torch.Tensor, fake: torch.Tensor) -> torch.Tensor:
         real_features = self.vgg_feature_extractor(hr_image)
         fake_features = self.vgg_feature_extractor(fake)
-        perceptual_loss = self._content_loss(real_features, fake_features)
-        return perceptual_loss
+        return self._content_loss(real_features, fake_features)
 
     @staticmethod
     def _content_loss(hr_image: torch.Tensor, fake: torch.Tensor) -> torch.Tensor:
         return F.mse_loss(hr_image, fake)
 
     @staticmethod
     def add_model_specific_args(parent_parser: ArgumentParser) -> ArgumentParser:
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/gans/srgan/srresnet_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/gans/srgan/srresnet_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Adapted from: https://github.com/https-deeplearning-ai/GANs-Public."""
 from argparse import ArgumentParser
 from typing import Any, Tuple
 
 import pytorch_lightning as pl
 import torch
-import torch.nn.functional as F
+import torch.nn.functional as F  # noqa: N812
 
 from pl_bolts.callbacks import SRImageLoggerCallback
 from pl_bolts.datamodules import TVTDataModule
 from pl_bolts.datasets.utils import prepare_sr_datasets
 from pl_bolts.models.gans.srgan.components import SRGANGenerator
 from pl_bolts.utils.stability import under_review
 
@@ -94,16 +94,15 @@
         loss = self._loss(batch)
         self.log("loss/test", loss, sync_dist=True)
         return loss
 
     def _loss(self, batch: Tuple[torch.Tensor, torch.Tensor]) -> torch.Tensor:
         hr_image, lr_image = batch
         fake = self(lr_image)
-        loss = F.mse_loss(hr_image, fake)
-        return loss
+        return F.mse_loss(hr_image, fake)
 
     @staticmethod
     def add_model_specific_args(parent_parser: ArgumentParser) -> ArgumentParser:
         parser = ArgumentParser(parents=[parent_parser], add_help=False)
         parser.add_argument("--feature_maps", default=64, type=int)
         parser.add_argument("--learning_rate", default=1e-4, type=float)
         parser.add_argument("--num_res_blocks", default=16, type=int)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/mnist_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/mnist_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser
 from typing import Any
 
 import torch
 from pytorch_lightning import LightningModule, Trainer
 from torch import Tensor
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.utils import _TORCHVISION_AVAILABLE
 
 
 class LitMNIST(LightningModule):
     """PyTorch Lightning implementation of a two-layer MNIST classification module.
 
@@ -23,15 +23,14 @@
         model = LitMNIST()
 
         trainer = Trainer()
         trainer.fit(model, datamodule=datamodule)
     """
 
     def __init__(self, hidden_dim: int = 128, learning_rate: float = 1e-3, **kwargs: Any) -> None:
-
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `torchvision` which is not installed yet.")
 
         super().__init__()
         self.save_hyperparameters()
 
         self.l1 = torch.nn.Linear(28 * 28, self.hparams.hidden_dim)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/regression/linear_regression.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/regression/linear_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser
 from typing import Any, Dict, List, Tuple, Type
 
 import torch
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from torch import Tensor, nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 from torch.optim import Adam
 from torch.optim.optimizer import Optimizer
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
@@ -42,16 +42,15 @@
         super().__init__()
         self.save_hyperparameters()
         self.optimizer = optimizer
 
         self.linear = nn.Linear(in_features=self.hparams.input_dim, out_features=self.hparams.output_dim, bias=bias)
 
     def forward(self, x: Tensor) -> Tensor:
-        y_hat = self.linear(x)
-        return y_hat
+        return self.linear(x)
 
     def training_step(self, batch: Tuple[Tensor, Tensor], batch_idx: int) -> Dict[str, Tensor]:
         x, y = batch
 
         # flatten any input
         x = x.view(x.size(0), -1)
 
@@ -134,16 +133,16 @@
     args = parser.parse_args()
 
     # model
     model = LinearRegression(input_dim=10, l1_strength=1, l2_strength=1)
     # model = LinearRegression(**vars(args))
 
     # data
-    X, y = load_diabetes(return_X_y=True)  # these are numpy arrays
-    loaders = SklearnDataModule(X, y, batch_size=args.batch_size)
+    data, y = load_diabetes(return_X_y=True)  # these are numpy arrays
+    loaders = SklearnDataModule(data, y, batch_size=args.batch_size)
 
     # train
     trainer = Trainer.from_argparse_args(args)
     trainer.fit(model, train_dataloaders=loaders.train_dataloader(), val_dataloaders=loaders.val_dataloader())
 
 
 if __name__ == "__main__":
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/advantage_actor_critic_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/advantage_actor_critic_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,16 +217,15 @@
         logprobs = logprobs[range(self.hparams.batch_size), actions]
         actor_loss = -(logprobs * advs).mean()
 
         # critic loss
         critic_loss = self.hparams.critic_beta * torch.square(targets - values).mean()
 
         # total loss (weighted sum)
-        total_loss = actor_loss + critic_loss - entropy
-        return total_loss
+        return actor_loss + critic_loss - entropy
 
     def training_step(self, batch: Tuple[Tensor, Tensor], batch_idx: int) -> OrderedDict:
         """Perform one actor-critic update using a batch of data.
 
         Args:
             batch: a batch of (states, actions, returns)
         """
@@ -251,16 +250,15 @@
         """Initialize Adam optimizer."""
         optimizer = optim.Adam(self.net.parameters(), lr=self.hparams.lr)
         return [optimizer]
 
     def _dataloader(self) -> DataLoader:
         """Initialize the Replay Buffer dataset used for retrieving experiences."""
         dataset = ExperienceSourceDataset(self.train_batch)
-        dataloader = DataLoader(dataset=dataset, batch_size=self.hparams.batch_size)
-        return dataloader
+        return DataLoader(dataset=dataset, batch_size=self.hparams.batch_size)
 
     def train_dataloader(self) -> DataLoader:
         """Get train loader."""
         return self._dataloader()
 
     def get_device(self, batch) -> str:
         """Retrieve device currently being used by minibatch."""
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/agents.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/agents.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 """
 from abc import ABC
 from typing import List
 
 import numpy as np
 import torch
 from torch import Tensor, nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class Agent(ABC):
     """Basic agent that always returns 0."""
 
-    def __init__(self, net: nn.Module):
+    def __init__(self, net: nn.Module) -> None:
         self.net = net
 
     def __call__(self, state: Tensor, device: str, *args, **kwargs) -> List[int]:
         """Using the given network, decide what action to carry.
 
         Args:
             state: current state of the environment
@@ -40,15 +40,15 @@
     def __init__(
         self,
         net: nn.Module,
         action_space: int,
         eps_start: float = 1.0,
         eps_end: float = 0.2,
         eps_frames: float = 1000,
-    ):
+    ) -> None:
         super().__init__(net)
         self.action_space = action_space
         self.eps_start = eps_start
         self.epsilon = eps_start
         self.eps_end = eps_end
         self.eps_frames = eps_frames
 
@@ -62,30 +62,19 @@
 
         Returns:
             action defined by policy
         """
         if not isinstance(state, list):
             state = [state]
 
-        if np.random.random() < self.epsilon:
-            action = self.get_random_action(state)
-        else:
-            action = self.get_action(state, device)
-
-        return action
-
-    def get_random_action(self, state: Tensor) -> int:
-        """returns a random action."""
-        actions = []
-
-        for i in range(len(state)):
-            action = np.random.randint(0, self.action_space)
-            actions.append(action)
+        return self.get_random_action(state) if np.random.random() < self.epsilon else self.get_action(state, device)
 
-        return actions
+    def get_random_action(self, state: Tensor) -> list:
+        """Returns a random action."""
+        return [np.random.randint(0, self.action_space) for i in range(len(state))]
 
     def get_action(self, state: Tensor, device: torch.device):
         """Returns the best action based on the Q values of the network.
 
         Args:
             state: current state of the environment
             device: the device used for the current batch
@@ -130,17 +119,15 @@
         states = torch.tensor(states, device=device)
 
         # get the logits and pass through softmax for probability distribution
         probabilities = F.softmax(self.net(states)).squeeze(dim=-1)
         prob_np = probabilities.data.cpu().numpy()
 
         # take the numpy values and randomly select action based on prob distribution
-        actions = [np.random.choice(len(prob), p=prob) for prob in prob_np]
-
-        return actions
+        return [np.random.choice(len(prob), p=prob) for prob in prob_np]
 
 
 @under_review()
 class ActorCriticAgent(Agent):
     """Actor-Critic based agent that returns an action based on the networks policy."""
 
     def __call__(self, states: Tensor, device: str) -> List[int]:
@@ -160,17 +147,15 @@
             states = torch.tensor(states, device=device)
 
         logprobs, _ = self.net(states)
         probabilities = logprobs.exp().squeeze(dim=-1)
         prob_np = probabilities.data.cpu().numpy()
 
         # take the numpy values and randomly select action based on prob distribution
-        actions = [np.random.choice(len(prob), p=prob) for prob in prob_np]
-
-        return actions
+        return [np.random.choice(len(prob), p=prob) for prob in prob_np]
 
 
 @under_review()
 class SoftActorCriticAgent(Agent):
     """Actor-Critic based agent that returns a continuous action based on the policy."""
 
     def __call__(self, states: Tensor, device: str) -> List[float]:
@@ -186,17 +171,15 @@
         if not isinstance(states, list):
             states = [states]
 
         if not isinstance(states, Tensor):
             states = torch.tensor(states, device=device)
 
         dist = self.net(states)
-        actions = [a for a in dist.sample().cpu().numpy()]
-
-        return actions
+        return list(dist.sample().cpu().numpy())
 
     def get_action(self, states: Tensor, device: str) -> List[float]:
         """Get the action greedily (without sampling)
 
         Args:
             states: current state of the environment
             device: the device used for the current batch
@@ -206,10 +189,8 @@
         """
         if not isinstance(states, list):
             states = [states]
 
         if not isinstance(states, Tensor):
             states = torch.tensor(states, device=device)
 
-        actions = [self.net.get_action(states).cpu().numpy()]
-
-        return actions
+        return [self.net.get_action(states).cpu().numpy()]
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/cli.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/distributions.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import torch
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class TanhMultivariateNormal(torch.distributions.MultivariateNormal):
-    """The distribution of X is an affine of tanh applied on a normal distribution.
+    """The distribution of X is an affine of tanh applied on a normal distribution::
 
     X = action_scale * tanh(Z) + action_bias
     Z ~ Normal(mean, variance)
+
     """
 
-    def __init__(self, action_bias, action_scale, **kwargs):
+    def __init__(self, action_bias, action_scale, **kwargs) -> None:
         super().__init__(**kwargs)
 
         self.action_bias = action_bias
         self.action_scale = action_scale
 
     def rsample_with_z(self, sample_shape=torch.Size()):
         """Samples X using reparametrization trick with the intermediate variable Z.
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/gym_wrappers.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/gym_wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,73 +24,73 @@
     warn_missing_pkg("cv2", pypi_name="opencv-python")
 
 
 @under_review()
 class ToTensor(Wrapper):
     """For environments where the user need to press FIRE for the game to start."""
 
-    def __init__(self, env=None):
+    def __init__(self, env=None) -> None:
         if not _GYM_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `gym` which is not installed yet.")
 
         super().__init__(env)
 
     def step(self, action):
         """Take 1 step and cast to tensor."""
         state, reward, done, info = self.env.step(action)
         return torch.tensor(state), torch.tensor(reward), done, info
 
     def reset(self):
-        """reset the env and cast to tensor."""
+        """Reset the env and cast to tensor."""
         return torch.tensor(self.env.reset())
 
 
 @under_review()
 class FireResetEnv(Wrapper):
     """For environments where the user need to press FIRE for the game to start."""
 
-    def __init__(self, env=None):
+    def __init__(self, env=None) -> None:
         if not _GYM_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `gym` which is not installed yet.")
 
         super().__init__(env)
         assert env.unwrapped.get_action_meanings()[1] == "FIRE"
         assert len(env.unwrapped.get_action_meanings()) >= 3
 
     def step(self, action):
         """Take 1 step."""
         return self.env.step(action)
 
     def reset(self):
-        """reset the env."""
+        """Reset the env."""
         self.env.reset()
         obs, _, done, _ = self.env.step(1)
         if done:
             self.env.reset()
         obs, _, done, _ = self.env.step(2)
         if done:
             self.env.reset()
         return obs
 
 
 @under_review()
 class MaxAndSkipEnv(Wrapper):
     """Return only every `skip`-th frame."""
 
-    def __init__(self, env=None, skip=4):
+    def __init__(self, env=None, skip=4) -> None:
         if not _GYM_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `gym` which is not installed yet.")
 
         super().__init__(env)
         # most recent raw observations (for max pooling across time steps)
         self._obs_buffer = collections.deque(maxlen=2)
         self._skip = skip
 
     def step(self, action):
-        """take 1 step."""
+        """Take 1 step."""
         total_reward = 0.0
         done = None
         for _ in range(self._skip):
             obs, reward, done, info = self.env.step(action)
             self._obs_buffer.append(obs)
             total_reward += reward
             if done:
@@ -107,116 +107,116 @@
         obs = self.env.reset()
         self._obs_buffer.append(obs)
         return obs
 
 
 @under_review()
 class ProcessFrame84(ObservationWrapper):
-    """preprocessing images from env."""
+    """Preprocessing images from env."""
 
-    def __init__(self, env=None):
+    def __init__(self, env=None) -> None:
         if not _OPENCV_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("This class uses OpenCV which it is not installed yet.")
 
         super().__init__(env)
         self.observation_space = gym.spaces.Box(low=0, high=255, shape=(84, 84, 1), dtype=np.uint8)
 
     def observation(self, obs):
-        """preprocess the obs."""
+        """Preprocess the obs."""
         return ProcessFrame84.process(obs)
 
     @staticmethod
     def process(frame):
-        """image preprocessing, formats to 84x84."""
+        """Image preprocessing, formats to 84x84."""
         if frame.size == 210 * 160 * 3:
             img = np.reshape(frame, [210, 160, 3]).astype(np.float32)
         elif frame.size == 250 * 160 * 3:
             img = np.reshape(frame, [250, 160, 3]).astype(np.float32)
         else:
-            assert False, "Unknown resolution."
+            raise RuntimeError("Unknown resolution.")
         img = img[:, :, 0] * 0.299 + img[:, :, 1] * 0.587 + img[:, :, 2] * 0.114
         resized_screen = cv2.resize(img, (84, 110), interpolation=cv2.INTER_AREA)
         x_t = resized_screen[18:102, :]
         x_t = np.reshape(x_t, [84, 84, 1])
         return x_t.astype(np.uint8)
 
 
 @under_review()
 class ImageToPyTorch(ObservationWrapper):
-    """converts image to pytorch format."""
+    """Converts image to pytorch format."""
 
-    def __init__(self, env):
+    def __init__(self, env) -> None:
         if not _OPENCV_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("This class uses OpenCV which it is not installed yet.")
 
         super().__init__(env)
         old_shape = self.observation_space.shape
         new_shape = (old_shape[-1], old_shape[0], old_shape[1])
         self.observation_space = gym.spaces.Box(low=0.0, high=1.0, shape=new_shape, dtype=np.float32)
 
     @staticmethod
     def observation(observation):
-        """convert observation."""
+        """Convert observation."""
         return np.moveaxis(observation, 2, 0)
 
 
 @under_review()
 class ScaledFloatFrame(ObservationWrapper):
-    """scales the pixels."""
+    """Scales the pixels."""
 
     @staticmethod
     def observation(obs):
         return np.array(obs).astype(np.float32) / 255.0
 
 
 @under_review()
 class BufferWrapper(ObservationWrapper):
     """Wrapper for image stacking."""
 
-    def __init__(self, env, n_steps, dtype=np.float32):
+    def __init__(self, env, n_steps, dtype=np.float32) -> None:
         super().__init__(env)
         self.dtype = dtype
         self.buffer = None
         old_space = env.observation_space
         self.observation_space = gym.spaces.Box(
             old_space.low.repeat(n_steps, axis=0),
             old_space.high.repeat(n_steps, axis=0),
             dtype=dtype,
         )
 
     def reset(self):
-        """reset env."""
+        """Reset env."""
         self.buffer = np.zeros_like(self.observation_space.low, dtype=self.dtype)
         return self.observation(self.env.reset())
 
     def observation(self, observation):
-        """convert observation."""
+        """Convert observation."""
         self.buffer[:-1] = self.buffer[1:]
         self.buffer[-1] = observation
         return self.buffer
 
 
 @under_review()
 class DataAugmentation(ObservationWrapper):
     """Carries out basic data augmentation on the env observations.
 
     - ToTensor
     - GrayScale
     - RandomCrop
     """
 
-    def __init__(self, env=None):
+    def __init__(self, env=None) -> None:
         if not _GYM_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `gym` which is not installed yet.")
 
         super().__init__(env)
         self.observation_space = gym.spaces.Box(low=0, high=255, shape=(84, 84, 1), dtype=np.uint8)
 
     def observation(self, obs):
-        """preprocess the obs."""
+        """Preprocess the obs."""
         return ProcessFrame84.process(obs)
 
 
 @under_review()
 def make_environment(env_name):
     """Convert environment with wrappers."""
     env = gym_make(env_name)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/memory.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         return total_reward
 
 
 @under_review()
 class MeanBuffer:
     """Stores a deque of items and calculates the mean."""
 
-    def __init__(self, capacity):
+    def __init__(self, capacity) -> None:
         self.capacity = capacity
         self.deque = collections.deque(maxlen=capacity)
         self.sum = 0.0
 
     def add(self, val: float) -> None:
         """Add to the buffer."""
         if len(self.deque) == self.capacity:
@@ -215,15 +215,15 @@
 @under_review()
 class PERBuffer(ReplayBuffer):
     """simple list based Prioritized Experience Replay Buffer Based on implementation found here:
 
     https://github.com/Shmuma/ptan/blob/master/ptan/experience.py#L371
     """
 
-    def __init__(self, buffer_size, prob_alpha=0.6, beta_start=0.4, beta_frames=100000):
+    def __init__(self, buffer_size, prob_alpha=0.6, beta_start=0.4, beta_frames=100000) -> None:
         super().__init__(capacity=buffer_size)
         self.beta_start = beta_start
         self.beta = beta_start
         self.beta_frames = beta_frames
         self.prob_alpha = prob_alpha
         self.capacity = buffer_size
         self.pos = 0
@@ -270,18 +270,15 @@
         Args:
             batch_size: size of sample
 
         Returns:
             sample of experiences chosen with ranked probability
         """
         # get list of priority rankings
-        if len(self.buffer) == self.capacity:
-            prios = self.priorities
-        else:
-            prios = self.priorities[: self.pos]
+        prios = self.priorities if len(self.buffer) == self.capacity else self.priorities[: self.pos]
 
         # probability to the power of alpha to weight how important that probability it, 0 = normal distirbution
         probs = prios**self.prob_alpha
         probs /= probs.sum()
 
         # choise sample of indices based on the priority prob distribution
         indices = np.random.choice(len(self.buffer), batch_size, p=probs)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/common/networks.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/common/networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import math
 from typing import Tuple
 
 import numpy as np
 import torch
 from torch import FloatTensor, Tensor, nn
 from torch.distributions import Categorical, Normal
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.models.rl.common.distributions import TanhMultivariateNormal
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class CNN(nn.Module):
     """Simple MLP network."""
 
-    def __init__(self, input_shape: Tuple[int], n_actions: int):
+    def __init__(self, input_shape: Tuple[int], n_actions: int) -> None:
         """
         Args:
             input_shape: observation shape of the environment
             n_actions: number of discrete actions available in the environment
         """
         super().__init__()
 
@@ -59,15 +59,15 @@
         return self.head(conv_out)
 
 
 @under_review()
 class MLP(nn.Module):
     """Simple MLP network."""
 
-    def __init__(self, input_shape: Tuple[int], n_actions: int, hidden_size: int = 128):
+    def __init__(self, input_shape: Tuple[int], n_actions: int, hidden_size: int = 128) -> None:
         """
         Args:
             input_shape: observation shape of the environment
             n_actions: number of discrete actions available in the environment
             hidden_size: size of hidden layers
         """
         super().__init__()
@@ -96,15 +96,15 @@
     def __init__(
         self,
         input_shape: Tuple[int],
         n_actions: int,
         hidden_size: int = 128,
         action_bias: int = 0,
         action_scale: int = 1,
-    ):
+    ) -> None:
         """
         Args:
             input_shape: observation shape of the environment
             n_actions: dimension of actions in the environment
             hidden_size: size of hidden layers
             action_bias: the center of the action space
             action_scale: the scale of the action space
@@ -148,15 +148,15 @@
         return self.action_scale * torch.tanh(batch_mean) + self.action_bias
 
 
 @under_review()
 class ActorCriticMLP(nn.Module):
     """MLP network with heads for actor and critic."""
 
-    def __init__(self, input_shape: Tuple[int], n_actions: int, hidden_size: int = 128):
+    def __init__(self, input_shape: Tuple[int], n_actions: int, hidden_size: int = 128) -> None:
         """
         Args:
             input_shape: observation shape of the environment
             n_actions: number of discrete actions available in the environment
             hidden_size: size of hidden layers
         """
         super().__init__()
@@ -180,15 +180,15 @@
         return a, c
 
 
 @under_review()
 class DuelingMLP(nn.Module):
     """MLP network with duel heads for val and advantage."""
 
-    def __init__(self, input_shape: Tuple[int], n_actions: int, hidden_size: int = 128):
+    def __init__(self, input_shape: Tuple[int], n_actions: int, hidden_size: int = 128) -> None:
         """
         Args:
             input_shape: observation shape of the environment
             n_actions: number of discrete actions available in the environment
             hidden_size: size of hidden layers
         """
         super().__init__()
@@ -212,16 +212,15 @@
         Args:
             x: input to network
 
         Returns:
             Q value
         """
         adv, val = self.adv_val(input_x)
-        q_val = val + (adv - adv.mean(dim=1, keepdim=True))
-        return q_val
+        return val + (adv - adv.mean(dim=1, keepdim=True))
 
     def adv_val(self, input_x) -> Tuple[Tensor, Tensor]:
         """Gets the advantage and value by passing out of the base network through the value and advantage heads.
 
         Args:
             input_x: input to network
 
@@ -233,15 +232,15 @@
         return self.fc_adv(base_out), self.fc_val(base_out)
 
 
 @under_review()
 class DuelingCNN(nn.Module):
     """CNN network with duel heads for val and advantage."""
 
-    def __init__(self, input_shape: Tuple[int], n_actions: int, _: int = 128):
+    def __init__(self, input_shape: Tuple[int], n_actions: int, _: int = 128) -> None:
         """
         Args:
             input_shape: observation shape of the environment
             n_actions: number of discrete actions available in the environment
             hidden_size: size of hidden layers
         """
         super().__init__()
@@ -281,16 +280,15 @@
         Args:
             input_x: input to network
 
         Returns:
             Q value
         """
         adv, val = self.adv_val(input_x)
-        q_val = val + (adv - adv.mean(dim=1, keepdim=True))
-        return q_val
+        return val + (adv - adv.mean(dim=1, keepdim=True))
 
     def adv_val(self, input_x):
         """Gets the advantage and value by passing out of the base network through the value and advantage heads.
 
         Args:
             input_x: input to network
 
@@ -302,15 +300,15 @@
         return self.head_adv(base_out), self.head_val(base_out)
 
 
 @under_review()
 class NoisyCNN(nn.Module):
     """CNN with Noisy Linear layers for exploration."""
 
-    def __init__(self, input_shape: Tuple[int], n_actions: int):
+    def __init__(self, input_shape: Tuple[int], n_actions: int) -> None:
         """
         Args:
             input_shape: observation shape of the environment
             n_actions: number of discrete actions available in the environment
         """
         super().__init__()
 
@@ -360,15 +358,15 @@
 class NoisyLinear(nn.Linear):
     """Noisy Layer using Independent Gaussian Noise.
 
     based on https://github.com/PacktPublishing/Deep-Reinforcement-Learning-Hands-On-Second-Edition/blob/master/
     Chapter08/lib/dqn_extra.py#L19
     """
 
-    def __init__(self, in_features: int, out_features: int, sigma_init: float = 0.017, bias: bool = True):
+    def __init__(self, in_features: int, out_features: int, sigma_init: float = 0.017, bias: bool = True) -> None:
         """
         Args:
             in_features: number of inputs
             out_features: number of outputs
             sigma_init: initial fill value of noisy weights
             bias: flag to include bias to linear layer
         """
@@ -384,15 +382,15 @@
             self.sigma_bias = nn.Parameter(bias)
             epsilon_bias = torch.zeros(out_features)
             self.register_buffer("epsilon_bias", epsilon_bias)
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
-        """initializes or resets the paramseter of the layer."""
+        """Initializes or resets the paramseter of the layer."""
         std = math.sqrt(3 / self.in_features)
         self.weight.data.uniform_(-std, std)
         self.bias.data.uniform_(-std, std)
 
     def forward(self, input_x: Tensor) -> Tensor:
         """Forward pass of the layer.
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/double_dqn_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/double_dqn_model.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/dqn_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/dqn_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         warm_start_size: int = 10000,
         avg_reward_len: int = 100,
         min_episode_reward: int = -21,
         seed: int = 123,
         batches_per_epoch: int = 1000,
         n_steps: int = 1,
         **kwargs,
-    ):
+    ) -> None:
         """
         Args:
             env: gym environment tag
             eps_start: starting value of epsilon for the epsilon-greedy exploration
             eps_end: final value of epsilon for the epsilon-greedy exploration
             eps_last_frame: the final frame in for the decrease of epsilon. At this frame espilon = eps_end
             sync_rate: the number of iterations between syncing up the target network with the train network
@@ -203,16 +203,15 @@
 
         Args:
             x: environment state
 
         Returns:
             q values
         """
-        output = self.net(x)
-        return output
+        return self.net(x)
 
     def train_batch(
         self,
     ) -> Tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
         """Contains the logic for generating a new batch of data to be passed to the DataLoader.
 
         Returns:
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/dueling_dqn_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/dueling_dqn_model.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/noisy_dqn_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/noisy_dqn_model.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/per_dqn_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/per_dqn_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,21 @@
                 episode_reward = 0
 
             samples, indices, weights = self.buffer.sample(self.batch_size)
 
             states, actions, rewards, dones, new_states = samples
 
             for idx, _ in enumerate(dones):
-                yield (states[idx], actions[idx], rewards[idx], dones[idx], new_states[idx],), indices[
+                yield (
+                    states[idx],
+                    actions[idx],
+                    rewards[idx],
+                    dones[idx],
+                    new_states[idx],
+                ), indices[
                     idx
                 ], weights[idx]
 
     def training_step(self, batch, _) -> OrderedDict:
         """Carries out a single step through the environment to update the replay buffer. Then calculates loss
         based on the minibatch recieved.
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/ppo_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/ppo_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,41 +49,41 @@
         gamma: float = 0.99,
         lam: float = 0.95,
         lr_actor: float = 3e-4,
         lr_critic: float = 1e-3,
         max_episode_len: float = 200,
         batch_size: int = 512,
         steps_per_epoch: int = 2048,
-        nb_optim_iters: int = 4,
+        num_optim_iters: int = 4,
         clip_ratio: float = 0.2,
         **kwargs: Any,
     ) -> None:
         """
         Args:
             env: gym environment tag
             gamma: discount factor
             lam: advantage discount factor (lambda in the paper)
             lr_actor: learning rate of actor network
             lr_critic: learning rate of critic network
             max_episode_len: maximum number interactions (actions) in an episode
             batch_size:  batch_size when training network- can simulate number of policy updates performed per epoch
             steps_per_epoch: how many action-state pairs to rollout for trajectory collection per epoch
-            nb_optim_iters: how many steps of gradient descent to perform on each batch
+            num_optim_iters: how many steps of gradient descent to perform on each batch
             clip_ratio: hyperparameter for clipping in the policy objective
         """
         super().__init__()
 
         if not _GYM_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("This Module requires gym environment which is not installed yet.")
 
         # Hyperparameters
         self.lr_actor = lr_actor
         self.lr_critic = lr_critic
         self.steps_per_epoch = steps_per_epoch
-        self.nb_optim_iters = nb_optim_iters
+        self.num_optim_iters = num_optim_iters
         self.batch_size = batch_size
         self.gamma = gamma
         self.lam = lam
         self.max_episode_len = max_episode_len
         self.clip_ratio = clip_ratio
         self.save_hyperparameters()
 
@@ -167,17 +167,15 @@
         Returns:
             list of advantages
         """
         rews = rewards + [last_value]
         vals = values + [last_value]
         # GAE
         delta = [rews[i] + self.gamma * vals[i + 1] - vals[i] for i in range(len(rews) - 1)]
-        adv = self.discount_rewards(delta, self.gamma * self.lam)
-
-        return adv
+        return self.discount_rewards(delta, self.gamma * self.lam)
 
     def generate_trajectory_samples(self) -> Tuple[List[Tensor], List[Tensor], List[Tensor]]:
         """Contains the logic for generating trajectory data to train policy and value network.
 
         Yield:
            Tuple of Lists containing tensors for states, actions, log probs, qvals and advantage
         """
@@ -248,33 +246,31 @@
 
                 # if epoch ended abruptly, exlude last cut-short episode to prevent stats skewness
                 epoch_rewards = self.epoch_rewards
                 if not done:
                     epoch_rewards = epoch_rewards[:-1]
 
                 total_epoch_reward = sum(epoch_rewards)
-                nb_episodes = len(epoch_rewards)
+                num_episodes = len(epoch_rewards)
 
-                self.avg_ep_reward = total_epoch_reward / nb_episodes
-                self.avg_ep_len = (self.steps_per_epoch - steps_before_cutoff) / nb_episodes
+                self.avg_ep_reward = total_epoch_reward / num_episodes
+                self.avg_ep_len = (self.steps_per_epoch - steps_before_cutoff) / num_episodes
 
                 self.epoch_rewards.clear()
 
     def actor_loss(self, state, action, logp_old, adv) -> Tensor:
         pi, _ = self.actor(state)
         logp = self.actor.get_log_prob(pi, action)
         ratio = torch.exp(logp - logp_old)
         clip_adv = torch.clamp(ratio, 1 - self.clip_ratio, 1 + self.clip_ratio) * adv
-        loss_actor = -(torch.min(ratio * adv, clip_adv)).mean()
-        return loss_actor
+        return -(torch.min(ratio * adv, clip_adv)).mean()
 
     def critic_loss(self, state, qval) -> Tensor:
         value = self.critic(state)
-        loss_critic = (qval - value).pow(2).mean()
-        return loss_critic
+        return (qval - value).pow(2).mean()
 
     def training_step(self, batch: Tuple[Tensor, Tensor], batch_idx, optimizer_idx):
         """Carries out a single update to actor and critic network from a batch of replay buffer.
 
         Args:
             batch: batch of replay buffer/trajectory data
             batch_idx: not used
@@ -313,24 +309,23 @@
         """Initialize Adam optimizer."""
         optimizer_actor = torch.optim.Adam(self.actor.parameters(), lr=self.lr_actor)
         optimizer_critic = torch.optim.Adam(self.critic.parameters(), lr=self.lr_critic)
 
         return optimizer_actor, optimizer_critic
 
     def optimizer_step(self, *args, **kwargs):
-        """Run ``nb_optim_iters`` number of iterations of gradient descent on actor and critic for each data
+        """Run ``num_optim_iters`` number of iterations of gradient descent on actor and critic for each data
         sample."""
-        for _ in range(self.nb_optim_iters):
+        for _ in range(self.num_optim_iters):
             super().optimizer_step(*args, **kwargs)
 
     def _dataloader(self) -> DataLoader:
         """Initialize the Replay Buffer dataset used for retrieving experiences."""
         dataset = ExperienceSourceDataset(self.generate_trajectory_samples)
-        dataloader = DataLoader(dataset=dataset, batch_size=self.batch_size)
-        return dataloader
+        return DataLoader(dataset=dataset, batch_size=self.batch_size)
 
     def train_dataloader(self) -> DataLoader:
         """Get train loader."""
         return self._dataloader()
 
     @staticmethod
     def add_model_specific_args(parent_parser):  # pragma: no cover
@@ -345,15 +340,15 @@
         parser.add_argument(
             "--steps_per_epoch",
             type=int,
             default=2048,
             help="how many action-state pairs to rollout for trajectory collection per epoch",
         )
         parser.add_argument(
-            "--nb_optim_iters", type=int, default=4, help="how many steps of gradient descent to perform on each batch"
+            "--num_optim_iters", type=int, default=4, help="how many steps of gradient descent to perform on each batch"
         )
         parser.add_argument(
             "--clip_ratio", type=float, default=0.2, help="hyperparameter for clipping in the policy objective"
         )
 
         return parser
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/reinforce_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/reinforce_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,15 @@
 
         Args:
             x: environment state
 
         Returns:
             q values
         """
-        output = self.net(x)
-        return output
+        return self.net(x)
 
     def calc_qvals(self, rewards: List[float]) -> List[float]:
         """Calculate the discounted rewards of all rewards in list.
 
         Args:
             rewards: list of rewards from latest batch
 
@@ -169,15 +168,14 @@
         """Contains the logic for generating a new batch of data to be passed to the DataLoader.
 
         Yield:
             yields a tuple of Lists containing tensors for states, actions and rewards of the batch.
         """
 
         while True:
-
             action = self.agent(self.state, self.device)
 
             next_state, reward, done, _ = self.env.step(action[0])
 
             self.batch_states.append(self.state)
             self.batch_actions.append(action[0])
             self.cur_rewards.append(reward)
@@ -210,17 +208,15 @@
 
     def loss(self, states, actions, scaled_rewards) -> Tensor:
         logits = self.net(states)
 
         # policy loss
         log_prob = log_softmax(logits, dim=1)
         log_prob_actions = scaled_rewards * log_prob[range(len(log_prob)), actions]
-        loss = -log_prob_actions.mean()
-
-        return loss
+        return -log_prob_actions.mean()
 
     def training_step(self, batch: Tuple[Tensor, Tensor], _) -> OrderedDict:
         """Carries out a single step through the environment to update the replay buffer. Then calculates loss
         based on the minibatch recieved.
 
         Args:
             batch: current mini batch of replay data
@@ -252,16 +248,15 @@
         """Initialize Adam optimizer."""
         optimizer = optim.Adam(self.net.parameters(), lr=self.lr)
         return [optimizer]
 
     def _dataloader(self) -> DataLoader:
         """Initialize the Replay Buffer dataset used for retrieving experiences."""
         dataset = ExperienceSourceDataset(self.train_batch)
-        dataloader = DataLoader(dataset=dataset, batch_size=self.batch_size)
-        return dataloader
+        return DataLoader(dataset=dataset, batch_size=self.batch_size)
 
     def train_dataloader(self) -> DataLoader:
         """Get train loader."""
         return self._dataloader()
 
     def get_device(self, batch) -> str:
         """Retrieve device currently being used by minibatch."""
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/sac_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/sac_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, List, Tuple
 
 import numpy as np
 import torch
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from pytorch_lightning.callbacks import ModelCheckpoint
 from torch import Tensor, optim
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 from torch.optim.optimizer import Optimizer
 from torch.utils.data import DataLoader
 
 from pl_bolts.datamodules.experience_source import Experience, ExperienceSourceDataset
 from pl_bolts.models.rl.common.agents import SoftActorCriticAgent
 from pl_bolts.models.rl.common.memory import MultiStepBuffer
 from pl_bolts.models.rl.common.networks import MLP, ContinuousMLP
@@ -44,15 +44,15 @@
         warm_start_size: int = 10000,
         avg_reward_len: int = 100,
         min_episode_reward: int = -21,
         seed: int = 123,
         batches_per_epoch: int = 10000,
         n_steps: int = 1,
         **kwargs,
-    ):
+    ) -> None:
         super().__init__()
 
         # Environment
         self.env = gym.make(env)
         self.test_env = gym.make(env)
 
         self.obs_shape = self.env.observation_space.shape
@@ -164,16 +164,15 @@
 
         Args:
             x: environment state
 
         Returns:
             q values
         """
-        output = self.policy(x).sample()
-        return output
+        return self.policy(x).sample()
 
     def train_batch(
         self,
     ) -> Tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
         """Contains the logic for generating a new batch of data to be passed to the DataLoader.
 
         Returns:
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/rl/vanilla_policy_gradient_model.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/rl/vanilla_policy_gradient_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,28 +115,26 @@
 
         Args:
             x: environment state
 
         Returns:
             q values
         """
-        output = self.net(x)
-        return output
+        return self.net(x)
 
     def train_batch(
         self,
     ) -> Tuple[List[Tensor], List[Tensor], List[Tensor]]:
         """Contains the logic for generating a new batch of data to be passed to the DataLoader.
 
         Returns:
             yields a tuple of Lists containing tensors for states, actions and rewards of the batch.
         """
 
         while True:
-
             action = self.agent(self.state, self.device)
 
             next_state, reward, done, _ = self.env.step(action[0])
 
             self.episode_rewards.append(reward)
             self.batch_actions.append(action)
             self.batch_states.append(self.state)
@@ -199,17 +197,15 @@
 
         # entropy loss
         prob = softmax(logits, dim=1)
         entropy = -(prob * log_prob).sum(dim=1).mean()
         entropy_loss = -self.entropy_beta * entropy
 
         # total loss
-        loss = policy_loss + entropy_loss
-
-        return loss
+        return policy_loss + entropy_loss
 
     def training_step(self, batch: Tuple[Tensor, Tensor], _) -> OrderedDict:
         """Carries out a single step through the environment to update the replay buffer. Then calculates loss
         based on the minibatch recieved.
 
         Args:
             batch: current mini batch of replay data
@@ -240,16 +236,15 @@
         """Initialize Adam optimizer."""
         optimizer = optim.Adam(self.net.parameters(), lr=self.lr)
         return [optimizer]
 
     def _dataloader(self) -> DataLoader:
         """Initialize the Replay Buffer dataset used for retrieving experiences."""
         dataset = ExperienceSourceDataset(self.train_batch)
-        dataloader = DataLoader(dataset=dataset, batch_size=self.batch_size)
-        return dataloader
+        return DataLoader(dataset=dataset, batch_size=self.batch_size)
 
     def train_dataloader(self) -> DataLoader:
         """Get train loader."""
         return self._dataloader()
 
     def get_device(self, batch) -> str:
         """Retrieve device currently being used by minibatch."""
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pl_bolts.models.self_supervised.amdim.amdim_module import AMDIM
 from pl_bolts.models.self_supervised.amdim.networks import AMDIMEncoder
-from pl_bolts.models.self_supervised.amdim.transforms import (
+from pl_bolts.transforms.self_supervised.amdim_transforms import (
     AMDIMEvalTransformsCIFAR10,
     AMDIMEvalTransformsImageNet128,
     AMDIMEvalTransformsSTL10,
     AMDIMTrainTransformsCIFAR10,
     AMDIMTrainTransformsImageNet128,
     AMDIMTrainTransformsSTL10,
 )
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/amdim_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/amdim_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,53 +14,52 @@
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 def generate_power_seq(lr, nb):
     half = int(nb / 2)
     coefs = [2**pow for pow in range(half, -half - 1, -1)]
-    lrs = [lr * coef for coef in coefs]
-    return lrs
+    return [lr * coef for coef in coefs]
 
 
 # CIFAR 10
 LEARNING_RATE_CIFAR = 2e-4
 DATASET_CIFAR10 = {
     "dataset": "cifar10",
     "ndf": 320,
     "n_rkhs": 1280,
     "depth": 10,
     "image_height": 32,
     "batch_size": 200,
-    "nb_classes": 10,
+    "num_classes": 10,
     "lr_options": generate_power_seq(LEARNING_RATE_CIFAR, 11),
 }
 
 # stl-10
 LEARNING_RATE_STL = 2e-4
 DATASET_STL10 = {
     "dataset": "stl10",
     "ndf": 192,
     "n_rkhs": 1536,
     "depth": 8,
     "image_height": 64,
     "batch_size": 200,
-    "nb_classes": 10,
+    "num_classes": 10,
     "lr_options": generate_power_seq(LEARNING_RATE_STL, 11),
 }
 
 LEARNING_RATE_IMAGENET = 2e-4
 DATASET_IMAGENET2012 = {
     "dataset": "imagenet2012",
     "ndf": 320,
     "n_rkhs": 2560,
     "depth": 10,
     "image_height": 128,
     "batch_size": 200,
-    "nb_classes": 1000,
+    "num_classes": 1000,
     "lr_options": generate_power_seq(LEARNING_RATE_IMAGENET, 11),
 }
 
 
 @under_review()
 class AMDIM(LightningModule):
     """PyTorch Lightning implementation of Augmented Multiscale Deep InfoMax (AMDIM_)
@@ -100,15 +99,15 @@
         tclip: int = 20.0,
         learning_rate: int = 2e-4,
         data_dir: str = "",
         num_classes: int = 10,
         batch_size: int = 200,
         num_workers: int = 16,
         **kwargs,
-    ):
+    ) -> None:
         """
         Args:
             datamodule: A LightningDatamodule
             encoder: an encoder string or model
             image_channels: 3
             image_height: pixels
             encoder_feature_dim: Called `ndf` in the paper, this is the representation size for the encoder.
@@ -182,25 +181,23 @@
         # ------------------
         # FEATURE EXTRACTION
         # extract features from various blocks for each image
         # _x1 are from image 1
         # _x2 from image 2
         r1_x1, r5_x1, r7_x1, r1_x2, r5_x2, r7_x2 = self.forward(img_1, img_2)
 
-        result = {
+        return {
             "r1_x1": r1_x1,
             "r5_x1": r5_x1,
             "r7_x1": r7_x1,
             "r1_x2": r1_x2,
             "r5_x2": r5_x2,
             "r7_x2": r7_x2,
         }
 
-        return result
-
     def training_step_end(self, outputs):
         r1_x1 = outputs["r1_x1"]
         r5_x1 = outputs["r5_x1"]
         r7_x1 = outputs["r7_x1"]
         r1_x2 = outputs["r1_x2"]
         r5_x2 = outputs["r5_x2"]
         r7_x2 = outputs["r7_x2"]
@@ -210,92 +207,84 @@
         unsupervised_loss = loss.sum() + lgt_reg
 
         # ------------------
         # FULL LOSS
         total_loss = unsupervised_loss
 
         tensorboard_logs = {"train_nce_loss": total_loss}
-        result = {"loss": total_loss, "log": tensorboard_logs}
-
-        return result
+        return {"loss": total_loss, "log": tensorboard_logs}
 
     def validation_step(self, batch, batch_nb):
         [img_1, img_2], labels = batch
 
         # generate features
         r1_x1, r5_x1, r7_x1, r1_x2, r5_x2, r7_x2 = self.forward(img_1, img_2)
 
         # Contrastive task
         loss, lgt_reg = self.contrastive_task((r1_x1, r5_x1, r7_x1), (r1_x2, r5_x2, r7_x2))
         unsupervised_loss = loss.sum() + lgt_reg
 
-        result = {"val_nce": unsupervised_loss}
-        return result
+        return {"val_nce": unsupervised_loss}
 
     def validation_epoch_end(self, outputs):
         val_nce = 0
         for output in outputs:
             val_nce += output["val_nce"]
 
         val_nce = val_nce / len(outputs)
         tensorboard_logs = {"val_nce": val_nce}
         return {"val_loss": val_nce, "log": tensorboard_logs}
 
     def configure_optimizers(self):
-        opt = optim.Adam(
-            params=self.parameters(), lr=self.hparams.learning_rate, betas=(0.8, 0.999), weight_decay=1e-5, eps=1e-7
-        )
-
         # if self.hparams.datamodule in ['cifar10', 'stl10', 'cifar100']:
         #     lr_scheduler = MultiStepLR(opt, milestones=[250, 280], gamma=0.2)
         # else:
         #     lr_scheduler = MultiStepLR(opt, milestones=[30, 45], gamma=0.2)
-
-        return opt  # [opt], [lr_scheduler]
+        return optim.Adam(
+            params=self.parameters(), lr=self.hparams.learning_rate, betas=(0.8, 0.999), weight_decay=1e-5, eps=1e-7
+        )
 
     def train_dataloader(self):
-        kwargs = dict(nb_classes=self.hparams.nb_classes) if self.hparams.datamodule == "imagenet2012" else {}
+        kwargs = {"num_classes": self.hparams.num_classes} if self.hparams.datamodule == "imagenet2012" else {}
         dataset = AMDIMPretraining.get_dataset(self.hparams.datamodule, self.hparams.data_dir, split="train", **kwargs)
 
         # LOADER
-        loader = DataLoader(
+        return DataLoader(
             dataset=dataset,
             batch_size=self.hparams.batch_size,
             pin_memory=True,
             drop_last=True,
             num_workers=self.hparams.num_workers,
         )
-        return loader
 
     def val_dataloader(self):
-        kwargs = dict(nb_classes=self.hparams.nb_classes) if self.hparams.datamodule == "imagenet2012" else {}
+        kwargs = {"num_classes": self.hparams.num_classes} if self.hparams.datamodule == "imagenet2012" else {}
         dataset = AMDIMPretraining.get_dataset(self.hparams.datamodule, self.hparams.data_dir, split="val", **kwargs)
 
         # LOADER
-        loader = DataLoader(
+        return DataLoader(
             dataset=dataset,
             batch_size=self.hparams.batch_size,
             pin_memory=True,
             drop_last=True,
             num_workers=self.hparams.num_workers,
         )
-        return loader
 
     @staticmethod
     def add_model_specific_args(parent_parser):
         parser = ArgumentParser(parents=[parent_parser], add_help=False)
         parser.add_argument("--datamodule", type=str, default="cifar10")
 
-        DATASETS = {"cifar10": DATASET_CIFAR10, "stl10": DATASET_STL10, "imagenet2012": DATASET_IMAGENET2012}
+        datasets = {"cifar10": DATASET_CIFAR10, "stl10": DATASET_STL10, "imagenet2012": DATASET_IMAGENET2012}
 
         (args, _) = parser.parse_known_args()
-        dataset = DATASETS[args.datamodule]
+        dataset = datasets[args.datamodule]
 
         # dataset options
-        parser.add_argument("--num_classes", default=dataset["nb_classes"], type=int)
+        parser.add_argument("--num_classes", default=dataset["num_classes"], type=int)
 
         # network params
         parser.add_argument("--tclip", type=float, default=20.0, help="soft clipping range for NCE scores")
         parser.add_argument("--use_bn", type=int, default=0)
         parser.add_argument("--encoder_feature_dim", type=int, default=dataset["ndf"], help="feature size for encoder")
         parser.add_argument(
             "--embedding_fx_dim",
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/datasets.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from torch.utils.data import random_split
 
 from pl_bolts.datasets import CIFAR10Mixed, UnlabeledImagenet
-from pl_bolts.models.self_supervised.amdim import transforms as amdim_transforms
+from pl_bolts.transforms.self_supervised import amdim_transforms
 from pl_bolts.utils import _TORCHVISION_AVAILABLE
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _TORCHVISION_AVAILABLE:
     from torchvision.datasets import STL10
 else:  # pragma: no cover
@@ -17,44 +17,41 @@
 @under_review()
 class AMDIMPretraining:
     """For pretraining we use the train transform for both train and val."""
 
     @staticmethod
     def cifar10(dataset_root, split: str = "train"):
         assert split in ("train", "val")
-        dataset = CIFAR10Mixed(
+        return CIFAR10Mixed(
             root=dataset_root,
             split=split,
             transform=amdim_transforms.AMDIMTrainTransformsCIFAR10(),
             download=True,
         )
-        return dataset
 
     @staticmethod
     def cifar10_tiny(dataset_root, split: str = "train"):
         assert split in ("train", "val")
-        dataset = CIFAR10Mixed(
+        return CIFAR10Mixed(
             root=dataset_root,
             split=split,
             transform=amdim_transforms.AMDIMTrainTransformsCIFAR10(),
             download=True,
-            nb_labeled_per_class=50,
+            num_labeled_per_class=50,
         )
-        return dataset
 
     @staticmethod
-    def imagenet(dataset_root, nb_classes, split: str = "train"):
+    def imagenet(dataset_root, num_classes, split: str = "train"):
         assert split in ("train", "val")
-        dataset = UnlabeledImagenet(
+        return UnlabeledImagenet(
             dataset_root,
-            nb_classes=nb_classes,
+            num_classes=num_classes,
             split=split,
             transform=amdim_transforms.AMDIMTrainTransformsImageNet128(),
         )
-        return dataset
 
     @staticmethod
     def stl(dataset_root, split: Optional[str] = None):
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError(
                 "You want to use STL10 dataset loaded from `torchvision` which is not installed yet."
             )
@@ -80,21 +77,20 @@
 class AMDIMPatchesPretraining:
     """For pretraining we use the train transform for both train and val."""
 
     @staticmethod
     def cifar10(dataset_root, patch_size, patch_overlap, split: str = "train"):
         assert split in ("train", "val")
         train_transform = amdim_transforms.TransformsC10Patches(patch_size=patch_size, patch_overlap=patch_overlap)
-        dataset = CIFAR10Mixed(
+        return CIFAR10Mixed(
             root=dataset_root,
             split=split,
             transform=train_transform,
             download=True,
         )
-        return dataset
 
     @staticmethod
     def stl(dataset_root, patch_size, patch_overlap, split: Optional[str] = None):
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError(
                 "You want to use STL10 dataset loaded from `torchvision` which is not installed yet."
             )
@@ -106,17 +102,16 @@
             download=True,
         )
         tng_split, val_split = random_split(dataset, [95000, 5000])
 
         return tng_split, val_split
 
     @staticmethod
-    def imagenet(dataset_root, nb_classes, patch_size, patch_overlap, split: str = "train"):
+    def imagenet(dataset_root, num_classes, patch_size, patch_overlap, split: str = "train"):
         assert split in ("train", "val")
         train_transform = amdim_transforms.TransformsImageNet128Patches(patch_size=patch_size, overlap=patch_overlap)
-        dataset = UnlabeledImagenet(
+        return UnlabeledImagenet(
             dataset_root,
-            nb_classes=nb_classes,
+            num_classes=num_classes,
             split=split,
             transform=train_transform,
         )
-        return dataset
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/networks.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/amdim/networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 
 import numpy as np
 import torch
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class AMDIMEncoder(nn.Module):
     def __init__(
@@ -15,15 +15,15 @@
         dummy_batch,
         num_channels=3,
         encoder_feature_dim=64,
         embedding_fx_dim=512,
         conv_block_depth=3,
         encoder_size=32,
         use_bn=False,
-    ):
+    ) -> None:
         super().__init__()
         # NDF = encoder hidden feat size
         # RKHS = output dim
         n_depth = conv_block_depth
         ndf = encoder_feature_dim
         self.ndf = encoder_feature_dim
         n_rkhs = embedding_fx_dim
@@ -123,16 +123,15 @@
         layer_acts = [x]
         for _, layer in enumerate(self.layer_list):
             layer_in = layer_acts[-1]
             layer_out = layer(layer_in)
             layer_acts.append(layer_out)
 
         # remove input from the returned list of activations
-        return_acts = layer_acts[1:]
-        return return_acts
+        return layer_acts[1:]
 
     def forward(self, x):
         # compute activations in all layers for x
         activations = self._forward_acts(x)
 
         # gather rkhs embeddings from certain layers
         # last feature map with (b, d, 1, 1) (ie: last network out)
@@ -147,15 +146,15 @@
         r7 = self.rkhs_block_7(r7)
 
         return r1, r5, r7
 
 
 @under_review()
 class Conv3x3(nn.Module):
-    def __init__(self, n_in, n_out, n_kern, n_stride, n_pad, use_bn=True, pad_mode="constant"):
+    def __init__(self, n_in, n_out, n_kern, n_stride, n_pad, use_bn=True, pad_mode="constant") -> None:
         super().__init__()
         assert pad_mode in ["constant", "reflect"]
         self.n_pad = (n_pad, n_pad, n_pad, n_pad)
         self.pad_mode = pad_mode
         self.conv = nn.Conv2d(n_in, n_out, n_kern, n_stride, 0, bias=(not use_bn))
         self.relu = nn.ReLU(inplace=True)
         self.bn = MaybeBatchNorm2d(n_out, True, use_bn)
@@ -165,41 +164,39 @@
             # maybe pad the input
             x = F.pad(x, self.n_pad, mode=self.pad_mode)
         # always apply conv
         x = self.conv(x)
         # maybe apply batchnorm
         x = self.bn(x)
         # always apply relu
-        out = self.relu(x)
-        return out
+        return self.relu(x)
 
 
 @under_review()
 class ConvResBlock(nn.Module):
-    def __init__(self, n_in, n_out, width, stride, pad, depth, use_bn):
+    def __init__(self, n_in, n_out, width, stride, pad, depth, use_bn) -> None:
         super().__init__()
         layer_list = [ConvResNxN(n_in, n_out, width, stride, pad, use_bn)]
         for i in range(depth - 1):
             layer_list.append(ConvResNxN(n_out, n_out, 1, 1, 0, use_bn))
         self.layer_list = nn.Sequential(*layer_list)
 
     def init_weights(self, init_scale=1.0):
         """Do a fixup-ish init for each ConvResNxN in this block."""
         for m in self.layer_list:
             m.init_weights(init_scale)
 
     def forward(self, x):
         # run forward pass through the list of ConvResNxN layers
-        x_out = self.layer_list(x)
-        return x_out
+        return self.layer_list(x)
 
 
 @under_review()
 class ConvResNxN(nn.Module):
-    def __init__(self, n_in, n_out, width, stride, pad, use_bn=False):
+    def __init__(self, n_in, n_out, width, stride, pad, use_bn=False) -> None:
         super().__init__()
         self.n_in = n_in
         self.n_out = n_out
         self.width = width
         self.stride = stride
         self.pad = pad
         self.relu1 = nn.ReLU(inplace=True)
@@ -230,48 +227,47 @@
         if self.n_out < self.n_in:
             h3 = self.conv3(x)
         elif self.n_in == self.n_out:
             h3 = F.avg_pool2d(x, self.width, self.stride, self.pad)
         else:
             h3_pool = F.avg_pool2d(x, self.width, self.stride, self.pad)
             h3 = F.pad(h3_pool, (0, 0, 0, 0, 0, self.n_grow))
-        h23 = h2 + h3
-        return h23
+        return h2 + h3
 
 
 @under_review()
 class MaybeBatchNorm2d(nn.Module):
-    def __init__(self, n_ftr, affine, use_bn):
+    def __init__(self, n_ftr, affine, use_bn) -> None:
         super().__init__()
         self.bn = nn.BatchNorm2d(n_ftr, affine=affine)
         self.use_bn = use_bn
 
     def forward(self, x):
         if self.use_bn:
             x = self.bn(x)
         return x
 
 
 @under_review()
 class NopNet(nn.Module):
-    def __init__(self, norm_dim=None):
+    def __init__(self, norm_dim=None) -> None:
         super().__init__()
         self.norm_dim = norm_dim
 
     def forward(self, x):
         if self.norm_dim is not None:
             x_norms = torch.sum(x**2.0, dim=self.norm_dim, keepdim=True)
             x_norms = torch.sqrt(x_norms + 1e-6)
             x = x / x_norms
         return x
 
 
 @under_review()
 class FakeRKHSConvNet(nn.Module):
-    def __init__(self, n_input, n_output, use_bn=False):
+    def __init__(self, n_input, n_output, use_bn=False) -> None:
         super().__init__()
         self.conv1 = nn.Conv2d(n_input, n_output, kernel_size=1, stride=1, padding=0, bias=False)
         self.bn1 = MaybeBatchNorm2d(n_output, True, use_bn)
         self.relu1 = nn.ReLU(inplace=True)
         self.conv2 = nn.Conv2d(n_output, n_output, kernel_size=1, stride=1, padding=0, bias=False)
         self.bn_out = MaybeBatchNorm2d(n_output, True, True)
         self.shortcut = nn.Conv2d(n_input, n_output, kernel_size=1, stride=1, padding=0, bias=True)
@@ -290,9 +286,8 @@
         self.conv1.weight.data.mul_(init_scale)
         # initialize second conv in res branch
         # -- set to 0, like fixup/zero init
         nn.init.constant_(self.conv2.weight, 0.0)
 
     def forward(self, x):
         h_res = self.conv2(self.relu1(self.bn1(self.conv1(x))))
-        h = self.bn_out(h_res + self.shortcut(x))
-        return h
+        return self.bn_out(h_res + self.shortcut(x))
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/amdim/transforms.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/moco_transforms.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,260 +1,259 @@
-from pl_bolts.transforms.self_supervised import RandomTranslateWithReflect
-from pl_bolts.utils import _TORCHVISION_AVAILABLE
+import random
+from typing import Callable, List, Tuple, Union
+
+from torch import Tensor
+
+from pl_bolts.transforms.dataset_normalizations import (
+    cifar10_normalization,
+    imagenet_normalization,
+    stl10_normalization,
+)
+from pl_bolts.utils import _PIL_AVAILABLE, _TORCHVISION_AVAILABLE
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _TORCHVISION_AVAILABLE:
     from torchvision import transforms
 else:  # pragma: no cover
     warn_missing_pkg("torchvision")
 
+if _PIL_AVAILABLE:
+    from PIL import ImageFilter
+else:  # pragma: no cover
+    warn_missing_pkg("PIL", pypi_name="Pillow")
 
-@under_review()
-class AMDIMTrainTransformsCIFAR10:
-    """Transforms applied to AMDIM.
 
-    Transforms::
+@under_review()
+class MoCoTrainTransforms:
+    normalization: type
+    """MoCo training transforms.
 
-        img_jitter,
-        col_jitter,
-        rnd_gray,
-        transforms.ToTensor(),
-        normalize
+    Args:
 
     Example::
-
-        x = torch.rand(5, 3, 32, 32)
-
-        transform = AMDIMTrainTransformsCIFAR10()
-        (view1, view2) = transform(x)
     """
 
-    def __init__(self):
-        if not _TORCHVISION_AVAILABLE:  # pragma: no cover
-            raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
-
-        # flipping image along vertical axis
-        self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
+    def __init__(self, size: int, normalize: Union[str, Callable]) -> None:
+        if isinstance(normalize, str):
+            self.normalize = normalize
+        else:
+            self.normalize = normalize
 
-        # image augmentation functions
-        normalize = transforms.Normalize(
-            mean=[x / 255.0 for x in [125.3, 123.0, 113.9]],
-            std=[x / 255.0 for x in [63.0, 62.1, 66.7]],
+        self.train_transform = transforms.Compose(
+            [
+                transforms.RandomResizedCrop(size, scale=(0.2, 1.0)),
+                transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8),  # not strengthened
+                transforms.RandomGrayscale(p=0.2),
+                transforms.RandomApply([GaussianBlur([0.1, 2.0])], p=0.5),
+                transforms.RandomHorizontalFlip(),
+                transforms.ToTensor(),
+                normalize(),
+            ]
         )
-        col_jitter = transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.2)], p=0.8)
-        img_jitter = transforms.RandomApply([RandomTranslateWithReflect(4)], p=0.8)
-        rnd_gray = transforms.RandomGrayscale(p=0.25)
-
-        self.transforms = transforms.Compose([img_jitter, col_jitter, rnd_gray, transforms.ToTensor(), normalize])
-
-    def __call__(self, inp):
-        inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        out2 = self.transforms(inp)
-        return out1, out2
+
+    def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        q = self.train_transform(x)
+        k = self.train_transform(x)
+        return q, k
 
 
 @under_review()
-class AMDIMEvalTransformsCIFAR10:
-    """Transforms applied to AMDIM.
+class MoCo2TrainCIFAR10Transforms:
+    """MoCo v2 transforms.
+
+    Args:
+        size (int, optional): input size. Defaults to 32.
 
-    Transforms::
+    Transform::
 
-        transforms.ToTensor(),
-        normalize
+        RandomResizedCrop(size=self.input_size)
 
     Example::
 
-        x = torch.rand(5, 3, 32, 32)
+        from pl_bolts.transforms.self_supervised.MoCo_transforms import MoCo2TrainCIFAR10Transforms
 
-        transform = AMDIMEvalTransformsCIFAR10()
-        (view1, view2) = transform(x)
+        transform = MoCo2TrainCIFAR10Transforms(input_size=32)
+        x = sample()
+        (xi, xj) = transform(x)
+
+    MoCo 2 augmentation:
+
+    https://arxiv.org/pdf/2003.04297.pdf
     """
 
-    def __init__(self):
+    def __init__(self, size: int = 32) -> None:
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
 
-        # flipping image along vertical axis
-        self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
-        normalize = transforms.Normalize(
-            mean=[x / 255.0 for x in [125.3, 123.0, 113.9]],
-            std=[x / 255.0 for x in [63.0, 62.1, 66.7]],
+        # image augmentation functions
+        self.train_transform = transforms.Compose(
+            [
+                transforms.RandomResizedCrop(size, scale=(0.2, 1.0)),
+                transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8),  # not strengthened
+                transforms.RandomGrayscale(p=0.2),
+                transforms.RandomApply([GaussianBlur([0.1, 2.0])], p=0.5),
+                transforms.RandomHorizontalFlip(),
+                transforms.ToTensor(),
+                cifar10_normalization(),
+            ]
         )
 
-        # transform for testing
-        self.transforms = transforms.Compose([transforms.ToTensor(), normalize])
-
-    def __call__(self, inp):
-        inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        return out1
+    def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        q = self.train_transform(x)
+        k = self.train_transform(x)
+        return q, k
 
 
 @under_review()
-class AMDIMTrainTransformsSTL10:
-    """Transforms applied to AMDIM.
+class MoCo2EvalCIFAR10Transforms:
+    """MoCo 2 augmentation:
 
-    Transforms::
+    https://arxiv.org/pdf/2003.04297.pdf
+    """
 
-        img_jitter,
-        col_jitter,
-        rnd_gray,
-        transforms.ToTensor(),
-        normalize
+    def __init__(self, size: int = 32) -> None:
+        if not _TORCHVISION_AVAILABLE:  # pragma: no cover
+            raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
 
-    Example::
+        self.test_transform = transforms.Compose(
+            [
+                transforms.Resize(size + 12),
+                transforms.CenterCrop(size),
+                transforms.ToTensor(),
+                cifar10_normalization(),
+            ]
+        )
 
-        x = torch.rand(5, 3, 64, 64)
+    def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        q = self.test_transform(x)
+        k = self.test_transform(x)
+        return q, k
 
-        transform = AMDIMTrainTransformsSTL10()
-        (view1, view2) = transform(x)
+
+@under_review()
+class MoCo2TrainImagenetTransforms:
+    """MoCo 2 augmentation:
+
+    https://arxiv.org/pdf/2003.04297.pdf
     """
 
-    def __init__(self, height=64):
+    def __init__(self, size: int = 224) -> None:
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
 
-        # flipping image along vertical axis
-        self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
-        normalize = transforms.Normalize(mean=(0.43, 0.42, 0.39), std=(0.27, 0.26, 0.27))
         # image augmentation functions
-        col_jitter = transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.2)], p=0.8)
-        rnd_gray = transforms.RandomGrayscale(p=0.25)
-        rand_crop = transforms.RandomResizedCrop(height, scale=(0.3, 1.0), ratio=(0.7, 1.4), interpolation=3)
-
-        self.transforms = transforms.Compose([rand_crop, col_jitter, rnd_gray, transforms.ToTensor(), normalize])
-
-    def __call__(self, inp):
-        inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        out2 = self.transforms(inp)
-        return out1, out2
-
-
-@under_review()
-class AMDIMEvalTransformsSTL10:
-    """Transforms applied to AMDIM.
-
-    Transforms::
+        self.train_transform = transforms.Compose(
+            [
+                transforms.RandomResizedCrop(size, scale=(0.2, 1.0)),
+                transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8),  # not strengthened
+                transforms.RandomGrayscale(p=0.2),
+                transforms.RandomApply([GaussianBlur([0.1, 2.0])], p=0.5),
+                transforms.RandomHorizontalFlip(),
+                transforms.ToTensor(),
+                imagenet_normalization(),
+            ]
+        )
 
-        transforms.Resize(height + 6, interpolation=3),
-        transforms.CenterCrop(height),
-        transforms.ToTensor(),
-        normalize
+    def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        q = self.train_transform(x)
+        k = self.train_transform(x)
+        return q, k
 
-    Example::
 
-        x = torch.rand(5, 3, 64, 64)
+@under_review()
+class MoCo2EvalImagenetTransforms:
+    """Transforms for MoCo during training step.
 
-        transform = AMDIMTrainTransformsSTL10()
-        view1 = transform(x)
+    https://arxiv.org/pdf/2003.04297.pdf
     """
 
-    def __init__(self, height=64):
+    def __init__(self, size: int = 128) -> None:
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
 
-        # flipping image along vertical axis
-        self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
-        normalize = transforms.Normalize(mean=(0.43, 0.42, 0.39), std=(0.27, 0.26, 0.27))
-        transforms.RandomResizedCrop(height, scale=(0.3, 1.0), ratio=(0.7, 1.4), interpolation=3)
-
-        self.transforms = transforms.Compose(
+        self.test_transform = transforms.Compose(
             [
-                transforms.Resize(height + 6, interpolation=3),
-                transforms.CenterCrop(height),
+                transforms.Resize(size + 32),
+                transforms.CenterCrop(size),
                 transforms.ToTensor(),
-                normalize,
+                imagenet_normalization(),
             ]
         )
 
-    def __call__(self, inp):
-        inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        return out1
+    def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        q = self.test_transform(x)
+        k = self.test_transform(x)
+        return q, k
 
 
 @under_review()
-class AMDIMTrainTransformsImageNet128:
-    """Transforms applied to AMDIM.
-
-    Transforms::
+class MoCo2TrainSTL10Transforms:
+    """MoCo 2 augmentation:
 
-        img_jitter,
-        col_jitter,
-        rnd_gray,
-        transforms.ToTensor(),
-        normalize
-
-    Example::
-
-        x = torch.rand(5, 3, 128, 128)
-
-        transform = AMDIMTrainTransformsSTL10()
-        (view1, view2) = transform(x)
+    https://arxiv.org/pdf/2003.04297.pdf
     """
 
-    def __init__(self, height=128):
+    def __init__(self, size: int = 64) -> None:
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
 
         # image augmentation functions
-        self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
-        rand_crop = transforms.RandomResizedCrop(height, scale=(0.3, 1.0), ratio=(0.7, 1.4), interpolation=3)
-        col_jitter = transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8)
-        rnd_gray = transforms.RandomGrayscale(p=0.25)
-        post_transform = transforms.Compose(
+        self.train_transform = transforms.Compose(
             [
+                transforms.RandomResizedCrop(size, scale=(0.2, 1.0)),
+                transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8),  # not strengthened
+                transforms.RandomGrayscale(p=0.2),
+                transforms.RandomApply([GaussianBlur([0.1, 2.0])], p=0.5),
+                transforms.RandomHorizontalFlip(),
                 transforms.ToTensor(),
-                transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+                stl10_normalization(),
             ]
         )
-        self.transforms = transforms.Compose([rand_crop, col_jitter, rnd_gray, post_transform])
 
-    def __call__(self, inp):
-        inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        out2 = self.transforms(inp)
-        return out1, out2
+    def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        q = self.train_transform(x)
+        k = self.train_transform(x)
+        return q, k
 
 
 @under_review()
-class AMDIMEvalTransformsImageNet128:
-    """Transforms applied to AMDIM.
-
-    Transforms::
-
-        transforms.Resize(height + 6, interpolation=3),
-        transforms.CenterCrop(height),
-        transforms.ToTensor(),
-        normalize
-
-    Example::
+class MoCo2EvalSTL10Transforms:
+    """MoCo 2 augmentation:
 
-        x = torch.rand(5, 3, 128, 128)
-
-        transform = AMDIMEvalTransformsImageNet128()
-        view1 = transform(x)
+    https://arxiv.org/pdf/2003.04297.pdf
     """
 
-    def __init__(self, height=128):
+    def __init__(self, size: int = 64) -> None:
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
 
-        # image augmentation functions
-        self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
-        post_transform = transforms.Compose(
+        self.test_augmentation = transforms.Compose(
             [
+                transforms.Resize(size + 11),
+                transforms.CenterCrop(size),
                 transforms.ToTensor(),
-                transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+                stl10_normalization(),
             ]
         )
-        self.transforms = transforms.Compose(
-            [transforms.Resize(height + 18, interpolation=3), transforms.CenterCrop(height), post_transform]
-        )
 
-    def __call__(self, inp):
-        inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        return out1
+    def __call__(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        q = self.test_augmentation(x)
+        k = self.test_augmentation(x)
+        return q, k
+
+
+@under_review()
+class GaussianBlur:
+    """Gaussian blur augmentation in SimCLR https://arxiv.org/abs/2002.05709."""
+
+    def __init__(self, sigma: List[float] = [0.1, 2.0]) -> None:
+        if not _PIL_AVAILABLE:  # pragma: no cover
+            raise ModuleNotFoundError(
+                "You want to use `Pillow` which is not installed yet, install it with `pip install Pillow`."
+            )
+        self.sigma = sigma
+
+    def __call__(self, x):
+        sigma = random.uniform(self.sigma[0], self.sigma[1])  # noqa: S311
+        x = x.filter(ImageFilter.GaussianBlur(radius=sigma))
+        return x
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/byol/byol_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/byol/byol_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from argparse import ArgumentParser
 from copy import deepcopy
 from typing import Any, Union
 
 import torch
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from torch import Tensor
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 from torch.optim import Adam
 
 from pl_bolts.callbacks.byol_updates import BYOLMAWeightUpdate
 from pl_bolts.models.self_supervised.byol.models import MLP, SiameseArm
 from pl_bolts.optimizers.lr_scheduler import LinearWarmupCosineAnnealingLR
 
 
@@ -70,15 +70,14 @@
         base_encoder: Union[str, torch.nn.Module] = "resnet50",
         encoder_out_dim: int = 2048,
         projector_hidden_dim: int = 4096,
         projector_out_dim: int = 256,
         initial_tau: float = 0.996,
         **kwargs: Any,
     ) -> None:
-
         super().__init__()
         self.save_hyperparameters(ignore="base_encoder")
 
         self.online_network = SiameseArm(base_encoder, encoder_out_dim, projector_hidden_dim, projector_out_dim)
         self.target_network = deepcopy(self.online_network)
         self.predictor = MLP(projector_out_dim, projector_hidden_dim, projector_out_dim)
 
@@ -133,16 +132,15 @@
             v_online (Tensor): Online network view
             v_target (Tensor): Target network view
         """
         _, z1 = self.online_network(v_online)
         h1 = self.predictor(z1)
         with torch.no_grad():
             _, z2 = self.target_network(v_target)
-        loss = -2 * F.cosine_similarity(h1, z2).mean()
-        return loss
+        return -2 * F.cosine_similarity(h1, z2).mean()
 
     def configure_optimizers(self):
         optimizer = Adam(self.parameters(), lr=self.hparams.learning_rate, weight_decay=self.hparams.weight_decay)
         scheduler = LinearWarmupCosineAnnealingLR(
             optimizer, warmup_epochs=self.hparams.warmup_epochs, max_epochs=self.hparams.max_epochs
         )
         return [optimizer], [scheduler]
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/byol/models.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/byol/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         output_dim (int, optional): Output dimension. Defaults to 256.
 
     Note:
         Default values for input, hidden, and output dimensions are based on values used in BYOL.
     """
 
     def __init__(self, input_dim: int = 2048, hidden_dim: int = 4096, output_dim: int = 256) -> None:
-
         super().__init__()
 
         self.model = nn.Sequential(
             nn.Linear(input_dim, hidden_dim, bias=False),
             nn.BatchNorm1d(hidden_dim),
             nn.ReLU(inplace=True),
             nn.Linear(hidden_dim, output_dim, bias=True),
@@ -49,15 +48,14 @@
     def __init__(
         self,
         encoder: Union[str, nn.Module] = "resnet50",
         encoder_out_dim: int = 2048,
         projector_hidden_dim: int = 4096,
         projector_out_dim: int = 256,
     ) -> None:
-
         super().__init__()
 
         if isinstance(encoder, str):
             self.encoder = torchvision_ssl_encoder(encoder)
         else:
             self.encoder = encoder
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/cpc_finetuner.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/cpc/cpc_finetuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from argparse import ArgumentParser
 
 from pytorch_lightning import Trainer, seed_everything
 
 from pl_bolts.models.self_supervised import CPC_v2, SSLFineTuner
-from pl_bolts.models.self_supervised.cpc.transforms import (
+from pl_bolts.transforms.self_supervised.cpc_transforms import (
     CPCEvalTransformsCIFAR10,
     CPCEvalTransformsSTL10,
     CPCTrainTransformsCIFAR10,
     CPCTrainTransformsSTL10,
 )
 from pl_bolts.utils.stability import under_review
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/cpc_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/cpc/cpc_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-"""
-CPC V2
-======
-"""
+"""CPC V2."""
 import math
 from argparse import ArgumentParser
 from typing import Optional
 
 import torch
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from pytorch_lightning.utilities import rank_zero_warn
 from torch import optim
 
 from pl_bolts.datamodules.stl10_datamodule import STL10DataModule
 from pl_bolts.losses.self_supervised_learning import CPCTask
 from pl_bolts.models.self_supervised.cpc.networks import cpc_resnet101
-from pl_bolts.models.self_supervised.cpc.transforms import (
+from pl_bolts.transforms.self_supervised.cpc_transforms import (
     CPCEvalTransformsCIFAR10,
     CPCEvalTransformsImageNet128,
     CPCEvalTransformsSTL10,
     CPCTrainTransformsCIFAR10,
     CPCTrainTransformsImageNet128,
     CPCTrainTransformsSTL10,
 )
@@ -26,28 +23,28 @@
 from pl_bolts.utils.self_supervised import torchvision_ssl_encoder
 from pl_bolts.utils.stability import under_review
 
 __all__ = ["CPC_v2"]
 
 
 @under_review()
-class CPC_v2(LightningModule):
+class CPC_v2(LightningModule):  # noqa: N801
     def __init__(
         self,
         encoder_name: str = "cpc_encoder",
         patch_size: int = 8,
         patch_overlap: int = 4,
         online_ft: bool = True,
         task: str = "cpc",
         num_workers: int = 4,
         num_classes: int = 10,
         learning_rate: float = 1e-4,
         pretrained: Optional[str] = None,
         **kwargs,
-    ):
+    ) -> None:
         """
         Args:
             encoder_name: A string for any of the resnets in torchvision, or the original CPC encoder,
                 or a custon nn.Module encoder
             patch_size: How big to make the image patches
             patch_overlap: How much overlap each patch should have
             online_ft: If True, enables a 1024-unit MLP to fine-tune online
@@ -66,15 +63,15 @@
         if pretrained:
             self.hparams.dataset = pretrained
             self.online_evaluator = True
 
         self.encoder = self.init_encoder()
 
         # info nce loss
-        c, h = self.__compute_final_nb_c(patch_size)
+        c, h = self.__compute_final_num_c(patch_size)
         self.contrastive_task = CPCTask(num_input_channels=c, target_dim=64, embed_scale=0.1)
 
         self.z_dim = c * h * h
         self.num_classes = num_classes
 
         if pretrained:
             self.load_pretrained(encoder_name)
@@ -91,52 +88,48 @@
         dummy_batch = torch.zeros((2, 3, self.hparams.patch_size, self.hparams.patch_size))
 
         encoder_name = self.hparams.encoder_name
         if encoder_name == "cpc_encoder":
             return cpc_resnet101(dummy_batch)
         return torchvision_ssl_encoder(encoder_name, return_all_feature_maps=self.hparams.task == "amdim")
 
-    def __compute_final_nb_c(self, patch_size):
+    def __compute_final_num_c(self, patch_size):
         dummy_batch = torch.zeros((2 * 49, 3, patch_size, patch_size))
         dummy_batch = self.encoder(dummy_batch)
 
         # other encoders return a list
         if self.hparams.encoder_name != "cpc_encoder":
             dummy_batch = dummy_batch[0]
 
         dummy_batch = self.__recover_z_shape(dummy_batch, 2)
         b, c, h, w = dummy_batch.size()
         return c, h
 
-    def __recover_z_shape(self, Z, b):
+    def __recover_z_shape(self, z, b):
         # recover shape
-        Z = Z.squeeze(-1)
-        nb_patches = int(math.sqrt(Z.size(0) // b))
-        Z = Z.view(b, -1, Z.size(1))
-        Z = Z.permute(0, 2, 1).contiguous()
-        Z = Z.view(b, -1, nb_patches, nb_patches)
+        z = z.squeeze(-1)
+        num_patches = int(math.sqrt(z.size(0) // b))
+        z = z.view(b, -1, z.size(1))
+        z = z.permute(0, 2, 1).contiguous()
+        return z.view(b, -1, num_patches, num_patches)
 
-        return Z
-
-    def forward(self, img_1):
+    def forward(self, img):
         # put all patches on the batch dim for simultaneous processing
-        b, _, c, w, h = img_1.size()
-        img_1 = img_1.view(-1, c, w, h)
+        b, _, c, w, h = img.size()
+        img = img.view(-1, c, w, h)
 
         # Z are the latent vars
-        Z = self.encoder(img_1)
+        z = self.encoder(img)
 
         # non cpc resnets return a list
         if self.hparams.encoder_name != "cpc_encoder":
-            Z = Z[0]
-
-        # (?) -> (b, -1, nb_feats, nb_feats)
-        Z = self.__recover_z_shape(Z, b)
+            z = z[0]
 
-        return Z
+        # (?) -> (b, -1, num_feats, num_feats)
+        return self.__recover_z_shape(z, b)
 
     def training_step(self, batch, batch_nb):
         # calculate loss
         nce_loss = self.shared_step(batch)
 
         # result
         self.log("train_nce_loss", nce_loss)
@@ -151,23 +144,22 @@
         return nce_loss
 
     def shared_step(self, batch):
         if isinstance(self.datamodule, STL10DataModule):
             # unlabeled batch
             batch = batch[0]
 
-        img_1, y = batch
+        img, y = batch
 
         # generate features
         # Latent features
-        Z = self(img_1)
+        z = self(img)
 
         # infoNCE loss
-        nce_loss = self.contrastive_task(Z)
-        return nce_loss
+        return self.contrastive_task(z)
 
     def configure_optimizers(self):
         opt = optim.Adam(
             params=self.parameters(),
             lr=self.hparams.learning_rate,
             betas=(0.8, 0.999),
             weight_decay=1e-5,
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/networks.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/cpc/networks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class CPCResNet(nn.Module):
     def __init__(
@@ -12,15 +12,15 @@
         block,
         layers,
         zero_init_residual=False,
         groups=1,
         width_per_group=64,
         replace_stride_with_dilation=None,
         norm_layer=None,
-    ):
+    ) -> None:
         super().__init__()
         if norm_layer is None:
             norm_layer = nn.LayerNorm
         self._norm_layer = norm_layer
         self.trainer = None
         self.experiment = None
         self.batch_size = None
@@ -151,15 +151,15 @@
         stride=1,
         downsample_conv=None,
         groups=1,
         base_width=64,
         dilation=1,
         norm_layer=None,
         expansion=4,
-    ):
+    ) -> None:
         super().__init__()
         width = int(planes * (base_width / 64.0)) * groups
         # Both self.conv2 and self.downsample layers downsample the input when stride != 1
         self.conv1 = conv1x1(inplanes, width)
         self.conv2 = conv3x3(width, width, stride, groups, dilation)
         self.conv3 = conv1x1(width, planes * expansion)
         self.relu = nn.ReLU(inplace=True)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/cpc/transforms.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/cpc_transforms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from torch import Tensor
+from torchvision.transforms import InterpolationMode
+
 from pl_bolts.transforms.self_supervised import Patchify, RandomTranslateWithReflect
 from pl_bolts.utils import _TORCHVISION_AVAILABLE
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _TORCHVISION_AVAILABLE:
     from torchvision import transforms
@@ -29,15 +32,15 @@
         CIFAR10(..., transforms=CPCTrainTransformsCIFAR10())
 
         # in a DataModule
         module = CIFAR10DataModule(PATH)
         train_loader = module.train_dataloader(batch_size=32, transforms=CPCTrainTransformsCIFAR10())
     """
 
-    def __init__(self, patch_size=8, overlap=4):
+    def __init__(self, patch_size: int = 8, overlap: int = 4) -> None:
         """
         Args:
             patch_size: size of patches when cutting up the image into overlapping patches
             overlap: how much to overlap patches
         """
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
@@ -61,18 +64,17 @@
                 rnd_gray,
                 transforms.ToTensor(),
                 normalize,
                 Patchify(patch_size=patch_size, overlap_size=overlap),
             ]
         )
 
-    def __call__(self, inp):
+    def __call__(self, inp: Tensor) -> Tensor:
         inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        return out1
+        return self.transforms(inp)
 
 
 @under_review()
 class CPCEvalTransformsCIFAR10:
     """Transforms used for CPC:
 
     Transforms::
@@ -88,15 +90,15 @@
         CIFAR10(..., transforms=CPCEvalTransformsCIFAR10())
 
         # in a DataModule
         module = CIFAR10DataModule(PATH)
         train_loader = module.train_dataloader(batch_size=32, transforms=CPCEvalTransformsCIFAR10())
     """
 
-    def __init__(self, patch_size: int = 8, overlap: int = 4):
+    def __init__(self, patch_size: int = 8, overlap: int = 4) -> None:
         """
         Args:
             patch_size: size of patches when cutting up the image into overlapping patches
             overlap: how much to overlap patches
         """
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
@@ -115,17 +117,16 @@
             [
                 transforms.ToTensor(),
                 normalize,
                 Patchify(patch_size=patch_size, overlap_size=overlap),
             ]
         )
 
-    def __call__(self, inp):
-        out1 = self.transforms(inp)
-        return out1
+    def __call__(self, inp: Tensor) -> Tensor:
+        return self.transforms(inp)
 
 
 @under_review()
 class CPCTrainTransformsSTL10:
     """Transforms used for CPC:
 
     Transforms::
@@ -144,15 +145,15 @@
         STL10(..., transforms=CPCTrainTransformsSTL10())
 
         # in a DataModule
         module = STL10DataModule(PATH)
         train_loader = module.train_dataloader(batch_size=32, transforms=CPCTrainTransformsSTL10())
     """
 
-    def __init__(self, patch_size: int = 16, overlap: int = 8):
+    def __init__(self, patch_size: int = 16, overlap: int = 8) -> None:
         """
         Args:
             patch_size: size of patches when cutting up the image into overlapping patches
             overlap: how much to overlap patches
         """
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
@@ -162,31 +163,32 @@
         self.overlap = overlap
         self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
         normalize = transforms.Normalize(mean=(0.43, 0.42, 0.39), std=(0.27, 0.26, 0.27))
 
         # image augmentation functions
         col_jitter = transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.2)], p=0.8)
         rnd_gray = transforms.RandomGrayscale(p=0.25)
-        rand_crop = transforms.RandomResizedCrop(64, scale=(0.3, 1.0), ratio=(0.7, 1.4), interpolation=3)
+        rand_crop = transforms.RandomResizedCrop(
+            64, scale=(0.3, 1.0), ratio=(0.7, 1.4), interpolation=InterpolationMode.BICUBIC
+        )
 
         self.transforms = transforms.Compose(
             [
                 rand_crop,
                 col_jitter,
                 rnd_gray,
                 transforms.ToTensor(),
                 normalize,
                 Patchify(patch_size=patch_size, overlap_size=overlap),
             ]
         )
 
-    def __call__(self, inp):
+    def __call__(self, inp: Tensor) -> Tensor:
         inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        return out1
+        return self.transforms(inp)
 
 
 @under_review()
 class CPCEvalTransformsSTL10:
     """Transforms used for CPC:
 
     Transforms::
@@ -202,15 +204,15 @@
         STL10(..., transforms=CPCEvalTransformsSTL10())
 
         # in a DataModule
         module = STL10DataModule(PATH)
         train_loader = module.train_dataloader(batch_size=32, transforms=CPCEvalTransformsSTL10())
     """
 
-    def __init__(self, patch_size: int = 16, overlap: int = 8):
+    def __init__(self, patch_size: int = 16, overlap: int = 8) -> None:
         """
         Args:
             patch_size: size of patches when cutting up the image into overlapping patches
             overlap: how much to overlap patches
         """
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
@@ -219,25 +221,24 @@
         self.patch_size = patch_size
         self.overlap = overlap
         self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
         normalize = transforms.Normalize(mean=(0.43, 0.42, 0.39), std=(0.27, 0.26, 0.27))
 
         self.transforms = transforms.Compose(
             [
-                transforms.Resize(70, interpolation=3),
+                transforms.Resize(70, interpolation=InterpolationMode.BICUBIC),
                 transforms.CenterCrop(64),
                 transforms.ToTensor(),
                 normalize,
                 Patchify(patch_size=patch_size, overlap_size=overlap),
             ]
         )
 
-    def __call__(self, inp):
-        out1 = self.transforms(inp)
-        return out1
+    def __call__(self, inp: Tensor) -> Tensor:
+        return self.transforms(inp)
 
 
 @under_review()
 class CPCTrainTransformsImageNet128:
     """Transforms used for CPC:
 
     Transforms::
@@ -253,45 +254,46 @@
         Imagenet(..., transforms=CPCTrainTransformsImageNet128())
 
         # in a DataModule
         module = ImagenetDataModule(PATH)
         train_loader = module.train_dataloader(batch_size=32, transforms=CPCTrainTransformsImageNet128())
     """
 
-    def __init__(self, patch_size: int = 32, overlap: int = 16):
+    def __init__(self, patch_size: int = 32, overlap: int = 16) -> None:
         """
         Args:
             patch_size: size of patches when cutting up the image into overlapping patches
             overlap: how much to overlap patches
         """
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
 
         # image augmentation functions
         self.patch_size = patch_size
         self.overlap = overlap
         self.flip_lr = transforms.RandomHorizontalFlip(p=0.5)
-        rand_crop = transforms.RandomResizedCrop(128, scale=(0.3, 1.0), ratio=(0.7, 1.4), interpolation=3)
+        rand_crop = transforms.RandomResizedCrop(
+            128, scale=(0.3, 1.0), ratio=(0.7, 1.4), interpolation=InterpolationMode.BICUBIC
+        )
         col_jitter = transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8)
         rnd_gray = transforms.RandomGrayscale(p=0.25)
 
         post_transform = transforms.Compose(
             [
                 transforms.ToTensor(),
                 transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
                 Patchify(patch_size=patch_size, overlap_size=overlap),
             ]
         )
 
         self.transforms = transforms.Compose([rand_crop, col_jitter, rnd_gray, post_transform])
 
-    def __call__(self, inp):
+    def __call__(self, inp: Tensor) -> Tensor:
         inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        return out1
+        return self.transforms(inp)
 
 
 @under_review()
 class CPCEvalTransformsImageNet128:
     """Transforms used for CPC:
 
     Transforms::
@@ -307,15 +309,15 @@
         Imagenet(..., transforms=CPCEvalTransformsImageNet128())
 
         # in a DataModule
         module = ImagenetDataModule(PATH)
         train_loader = module.train_dataloader(batch_size=32, transforms=CPCEvalTransformsImageNet128())
     """
 
-    def __init__(self, patch_size: int = 32, overlap: int = 16):
+    def __init__(self, patch_size: int = 32, overlap: int = 16) -> None:
         """
         Args:
             patch_size: size of patches when cutting up the image into overlapping patches
             overlap: how much to overlap patches
         """
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
@@ -328,14 +330,17 @@
             [
                 transforms.ToTensor(),
                 transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
                 Patchify(patch_size=patch_size, overlap_size=overlap),
             ]
         )
         self.transforms = transforms.Compose(
-            [transforms.Resize(146, interpolation=3), transforms.CenterCrop(128), post_transform]
+            [
+                transforms.Resize(146, interpolation=InterpolationMode.BICUBIC),
+                transforms.CenterCrop(128),
+                post_transform,
+            ]
         )
 
-    def __call__(self, inp):
+    def __call__(self, inp: Tensor) -> Tensor:
         inp = self.flip_lr(inp)
-        out1 = self.transforms(inp)
-        return out1
+        return self.transforms(inp)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/evaluator.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from torch import nn
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class SSLEvaluator(nn.Module):
-    def __init__(self, n_input, n_classes, n_hidden=512, p=0.1):
+    def __init__(self, n_input, n_classes, n_hidden=512, p=0.1) -> None:
         super().__init__()
         self.n_input = n_input
         self.n_classes = n_classes
         self.n_hidden = n_hidden
         if n_hidden is None:
             # use linear classifier
             self.block_forward = nn.Sequential(Flatten(), nn.Dropout(p=p), nn.Linear(n_input, n_classes, bias=True))
@@ -22,18 +22,17 @@
                 nn.BatchNorm1d(n_hidden),
                 nn.ReLU(inplace=True),
                 nn.Dropout(p=p),
                 nn.Linear(n_hidden, n_classes, bias=True),
             )
 
     def forward(self, x):
-        logits = self.block_forward(x)
-        return logits
+        return self.block_forward(x)
 
 
 @under_review()
 class Flatten(nn.Module):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
 
     def forward(self, input_tensor):
         return input_tensor.view(input_tensor.size(0), -1)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/moco/callbacks.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/moco/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pytorch_lightning import Callback
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class MocoLRScheduler(Callback):
-    def __init__(self, initial_lr=0.03, use_cosine_scheduler=False, schedule=(120, 160), max_epochs=200):
+    def __init__(self, initial_lr=0.03, use_cosine_scheduler=False, schedule=(120, 160), max_epochs=200) -> None:
         super().__init__()
         self.lr = initial_lr
         self.use_cosine_scheduler = use_cosine_scheduler
         self.schedule = schedule
         self.max_epochs = max_epochs
 
     def on_train_epoch_start(self, trainer, pl_module):
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/moco/moco2_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/moco/moco2_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-"""Adapted from: https://github.com/facebookresearch/moco.
+# Original work is: Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved.
+# This implementation is: Copyright (c) PyTorch Lightning, Inc. and its affiliates. All Rights Reserved
+#
+# This implementation is licensed under Attribution-NonCommercial 4.0 International;
+# You may not use this file except in compliance with the License.
+#
+# You may obtain a copy of the License from the LICENSE file present in this folder.
+"""MoCo2.
 
-Original work is: Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved
-This implementation is: Copyright (c) PyTorch Lightning, Inc. and its affiliates. All Rights Reserved
-
-This implementation is licensed under Attribution-NonCommercial 4.0 International;
-You may not use this file except in compliance with the License.
-
-You may obtain a copy of the License from the LICENSE file present in this folder.
+Adapted from https: //github.com/facebookresearch/moco.
 """
 from argparse import ArgumentParser
 from typing import Union
 
 import torch
 from pytorch_lightning import LightningModule, Trainer
 from pytorch_lightning.strategies import DDPStrategy
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.metrics import mean, precision_at_k
-from pl_bolts.models.self_supervised.moco.transforms import (
-    Moco2EvalCIFAR10Transforms,
-    Moco2EvalImagenetTransforms,
-    Moco2EvalSTL10Transforms,
-    Moco2TrainCIFAR10Transforms,
-    Moco2TrainImagenetTransforms,
-    Moco2TrainSTL10Transforms,
+from pl_bolts.transforms.self_supervised.moco_transforms import (
+    MoCo2EvalCIFAR10Transforms,
+    MoCo2EvalImagenetTransforms,
+    MoCo2EvalSTL10Transforms,
+    MoCo2TrainCIFAR10Transforms,
+    MoCo2TrainImagenetTransforms,
+    MoCo2TrainSTL10Transforms,
 )
 from pl_bolts.utils import _TORCHVISION_AVAILABLE
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _TORCHVISION_AVAILABLE:
     import torchvision
 else:  # pragma: no cover
     warn_missing_pkg("torchvision")
 
 
 @under_review()
-class Moco_v2(LightningModule):
+class Moco_v2(LightningModule):  # noqa: N801
     """PyTorch Lightning implementation of `Moco <https://arxiv.org/abs/2003.04297>`_
 
     Paper authors: Xinlei Chen, Haoqi Fan, Ross Girshick, Kaiming He.
 
     Code adapted from `facebookresearch/moco <https://github.com/facebookresearch/moco>`_ to Lightning by:
 
         - `William Falcon <https://github.com/williamFalcon>`_
@@ -79,15 +80,15 @@
         weight_decay: float = 1e-4,
         data_dir: str = "./",
         batch_size: int = 256,
         use_mlp: bool = False,
         num_workers: int = 8,
         *args,
         **kwargs
-    ):
+    ) -> None:
         """
         Args:
             base_encoder: torchvision model name or torch.nn.Module
             emb_dim: feature dimension (default: 128)
             num_negatives: queue size; number of negative keys (default: 65536)
             encoder_momentum: moco momentum of updating key encoder (default: 0.999)
             softmax_temperature: softmax temperature (default: 0.07)
@@ -221,15 +222,14 @@
 
         # compute query features
         q = self.encoder_q(img_q)  # queries: NxC
         q = nn.functional.normalize(q, dim=1)
 
         # compute key features
         with torch.no_grad():  # no gradient to keys
-
             # shuffle for making use of BN
             if self._use_ddp(self.trainer):
                 img_k, idx_unshuffle = self._batch_shuffle_ddp(img_k)
 
             k = self.encoder_k(img_k)  # keys: NxC
             k = nn.functional.normalize(k, dim=1)
 
@@ -289,16 +289,15 @@
         output, target, keys = self(img_q=img_1, img_k=img_2, queue=self.val_queue)
         self._dequeue_and_enqueue(keys, queue=self.val_queue, queue_ptr=self.val_queue_ptr)  # dequeue and enqueue
 
         loss = F.cross_entropy(output, target.long())
 
         acc1, acc5 = precision_at_k(output, target, top_k=(1, 5))
 
-        results = {"val_loss": loss, "val_acc1": acc1, "val_acc5": acc5}
-        return results
+        return {"val_loss": loss, "val_acc1": acc1, "val_acc5": acc5}
 
     def validation_epoch_end(self, outputs):
         val_loss = mean(outputs, "val_loss")
         val_acc1 = mean(outputs, "val_acc1")
         val_acc5 = mean(outputs, "val_acc5")
 
         log = {"val_loss": val_loss, "val_acc1": val_acc1, "val_acc5": val_acc5}
@@ -349,16 +348,15 @@
     """Performs all_gather operation on the provided tensors.
 
     *** Warning ***: torch.distributed.all_gather has no gradient.
     """
     tensors_gather = [torch.ones_like(tensor) for _ in range(torch.distributed.get_world_size())]
     torch.distributed.all_gather(tensors_gather, tensor, async_op=False)
 
-    output = torch.cat(tensors_gather, dim=0)
-    return output
+    return torch.cat(tensors_gather, dim=0)
 
 
 @under_review()
 def cli_main():
     from pl_bolts.datamodules import CIFAR10DataModule, SSLImagenetDataModule, STL10DataModule
 
     parser = ArgumentParser()
@@ -368,28 +366,28 @@
 
     # model args
     parser = Moco_v2.add_model_specific_args(parser)
     args = parser.parse_args()
 
     if args.dataset == "cifar10":
         datamodule = CIFAR10DataModule.from_argparse_args(args)
-        datamodule.train_transforms = Moco2TrainCIFAR10Transforms()
-        datamodule.val_transforms = Moco2EvalCIFAR10Transforms()
+        datamodule.train_transforms = MoCo2TrainCIFAR10Transforms()
+        datamodule.val_transforms = MoCo2EvalCIFAR10Transforms()
 
     elif args.dataset == "stl10":
         datamodule = STL10DataModule.from_argparse_args(args)
         datamodule.train_dataloader = datamodule.train_dataloader_mixed
         datamodule.val_dataloader = datamodule.val_dataloader_mixed
-        datamodule.train_transforms = Moco2TrainSTL10Transforms()
-        datamodule.val_transforms = Moco2EvalSTL10Transforms()
+        datamodule.train_transforms = MoCo2TrainSTL10Transforms()
+        datamodule.val_transforms = MoCo2EvalSTL10Transforms()
 
     elif args.dataset == "imagenet2012":
         datamodule = SSLImagenetDataModule.from_argparse_args(args)
-        datamodule.train_transforms = Moco2TrainImagenetTransforms()
-        datamodule.val_transforms = Moco2EvalImagenetTransforms()
+        datamodule.train_transforms = MoCo2TrainImagenetTransforms()
+        datamodule.val_transforms = MoCo2EvalImagenetTransforms()
 
     else:
         # replace with your own dataset, otherwise CIFAR-10 will be used by default if `None` passed in
         datamodule = None
 
     model = Moco_v2(**args.__dict__)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/moco/transforms.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/simclr_transforms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,205 +1,187 @@
-import random
+from typing import Callable, Tuple, Union
 
-from pl_bolts.transforms.dataset_normalizations import (
-    cifar10_normalization,
-    imagenet_normalization,
-    stl10_normalization,
-)
-from pl_bolts.utils import _PIL_AVAILABLE, _TORCHVISION_AVAILABLE
-from pl_bolts.utils.stability import under_review
+from torch import Tensor
+
+from pl_bolts.utils import _TORCHVISION_AVAILABLE
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _TORCHVISION_AVAILABLE:
     from torchvision import transforms
 else:  # pragma: no cover
     warn_missing_pkg("torchvision")
 
-if _PIL_AVAILABLE:
-    from PIL import ImageFilter
-else:  # pragma: no cover
-    warn_missing_pkg("PIL", pypi_name="Pillow")
-
 
-@under_review()
-class Moco2TrainCIFAR10Transforms:
-    """Moco 2 augmentation:
-
-    https://arxiv.org/pdf/2003.04297.pdf
-    """
+class SimCLRTrainDataTransform:
+    """Transforms for SimCLR during training step of the pre-training stage.
 
-    def __init__(self, height: int = 32):
-        if not _TORCHVISION_AVAILABLE:  # pragma: no cover
-            raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
+    Args:
+        input_height (int, optional): expected output size of image. Defaults to 224.
+        gaussian_blur (bool, optional): applies Gaussian blur if True. Defaults to True.
+        jitter_strength (float, optional): color jitter multiplier. Defaults to 1.0.
+        normalize (Callable, optional): optional transform to normalize. Defaults to None.
 
-        # image augmentation functions
-        self.train_transform = transforms.Compose(
-            [
-                transforms.RandomResizedCrop(height, scale=(0.2, 1.0)),
-                transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8),  # not strengthened
-                transforms.RandomGrayscale(p=0.2),
-                transforms.RandomApply([GaussianBlur([0.1, 2.0])], p=0.5),
-                transforms.RandomHorizontalFlip(),
-                transforms.ToTensor(),
-                cifar10_normalization(),
-            ]
-        )
+    Transform::
 
-    def __call__(self, inp):
-        q = self.train_transform(inp)
-        k = self.train_transform(inp)
-        return q, k
+        RandomResizedCrop(size=self.input_height)
+        RandomHorizontalFlip()
+        RandomApply([color_jitter], p=0.8)
+        RandomGrayscale(p=0.2)
+        RandomApply([GaussianBlur(kernel_size=int(0.1 * self.input_height))], p=0.5)
+        transforms.ToTensor()
 
+    Example::
 
-@under_review()
-class Moco2EvalCIFAR10Transforms:
-    """Moco 2 augmentation:
+        from pl_bolts.transforms.self_supervised.simclr_transforms import SimCLRTrainDataTransform
 
-    https://arxiv.org/pdf/2003.04297.pdf
+        transform = SimCLRTrainDataTransform(input_height=32)
+        x = sample()
+        (xi, xj, xk) = transform(x) # xk is only for the online evaluator if used
     """
 
-    def __init__(self, height: int = 32):
+    def __init__(
+        self,
+        input_height: int = 224,
+        gaussian_blur: bool = True,
+        jitter_strength: float = 1.0,
+        normalize: Union[None, Callable] = None,
+    ) -> None:
         if not _TORCHVISION_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
 
-        self.test_transform = transforms.Compose(
-            [
-                transforms.Resize(height + 12),
-                transforms.CenterCrop(height),
-                transforms.ToTensor(),
-                cifar10_normalization(),
-            ]
+        self.jitter_strength = jitter_strength
+        self.input_height = input_height
+        self.gaussian_blur = gaussian_blur
+        self.normalize = normalize
+
+        self.color_jitter = transforms.ColorJitter(
+            0.8 * self.jitter_strength,
+            0.8 * self.jitter_strength,
+            0.8 * self.jitter_strength,
+            0.2 * self.jitter_strength,
         )
 
-    def __call__(self, inp):
-        q = self.test_transform(inp)
-        k = self.test_transform(inp)
-        return q, k
+        data_transforms = [
+            transforms.RandomResizedCrop(size=self.input_height),
+            transforms.RandomHorizontalFlip(p=0.5),
+            transforms.RandomApply([self.color_jitter], p=0.8),
+            transforms.RandomGrayscale(p=0.2),
+        ]
 
+        if self.gaussian_blur:
+            kernel_size = int(0.1 * self.input_height)
+            if kernel_size % 2 == 0:
+                kernel_size += 1
 
-@under_review()
-class Moco2TrainSTL10Transforms:
-    """Moco 2 augmentation:
+            data_transforms.append(transforms.RandomApply([transforms.GaussianBlur(kernel_size=kernel_size)], p=0.5))
 
-    https://arxiv.org/pdf/2003.04297.pdf
-    """
+        self.data_transforms = transforms.Compose(data_transforms)
 
-    def __init__(self, height: int = 64):
-        if not _TORCHVISION_AVAILABLE:  # pragma: no cover
-            raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
+        if normalize is None:
+            self.final_transform = transforms.ToTensor()
+        else:
+            self.final_transform = transforms.Compose([transforms.ToTensor(), normalize])
 
-        # image augmentation functions
-        self.train_transform = transforms.Compose(
-            [
-                transforms.RandomResizedCrop(height, scale=(0.2, 1.0)),
-                transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8),  # not strengthened
-                transforms.RandomGrayscale(p=0.2),
-                transforms.RandomApply([GaussianBlur([0.1, 2.0])], p=0.5),
-                transforms.RandomHorizontalFlip(),
-                transforms.ToTensor(),
-                stl10_normalization(),
-            ]
+        self.train_transform = transforms.Compose([self.data_transforms, self.final_transform])
+
+        # add online train transform of the size of global view
+        self.online_transform = transforms.Compose(
+            [transforms.RandomResizedCrop(self.input_height), transforms.RandomHorizontalFlip(), self.final_transform]
         )
 
-    def __call__(self, inp):
-        q = self.train_transform(inp)
-        k = self.train_transform(inp)
-        return q, k
+    def __call__(self, sample: Tensor) -> Tuple[Tensor, Tensor, Tensor]:
+        xi = self.train_transform(sample)
+        xj = self.train_transform(sample)
+        return xi, xj, self.online_transform(sample)
 
 
-@under_review()
-class Moco2EvalSTL10Transforms:
-    """Moco 2 augmentation:
+class SimCLREvalDataTransform(SimCLRTrainDataTransform):
+    """Transforms for SimCLR during the validation step of the pre-training stage.
 
-    https://arxiv.org/pdf/2003.04297.pdf
-    """
+    Args:
+        input_height (int, optional): expected output size of image. Defaults to 224.
+        gaussian_blur (bool, optional): applies Gaussian blur if True. Defaults to True.
+        jitter_strength (float, optional): color jitter multiplier. Defaults to 1.0.
+        normalize (Callable, optional): optional transform to normalize. Defaults to None.
 
-    def __init__(self, height: int = 64):
-        if not _TORCHVISION_AVAILABLE:  # pragma: no cover
-            raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
-
-        self.test_augmentation = transforms.Compose(
-            [
-                transforms.Resize(height + 11),
-                transforms.CenterCrop(height),
-                transforms.ToTensor(),
-                stl10_normalization(),
-            ]
-        )
+    Transform::
 
-    def __call__(self, inp):
-        q = self.test_augmentation(inp)
-        k = self.test_augmentation(inp)
-        return q, k
+        Resize(input_height + 10, interpolation=3)
+        transforms.CenterCrop(input_height),
+        transforms.ToTensor()
 
+    Example::
 
-@under_review()
-class Moco2TrainImagenetTransforms:
-    """Moco 2 augmentation:
+        from pl_bolts.transforms.self_supervised.simclr_transforms import SimCLREvalDataTransform
 
-    https://arxiv.org/pdf/2003.04297.pdf
+        transform = SimCLREvalDataTransform(input_height=32)
+        x = sample()
+        (xi, xj, xk) = transform(x) # xk is only for the online evaluator if used
     """
 
-    def __init__(self, height: int = 128):
-        if not _TORCHVISION_AVAILABLE:  # pragma: no cover
-            raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
+    def __init__(
+        self,
+        input_height: int = 224,
+        gaussian_blur: bool = True,
+        jitter_strength: float = 1.0,
+        normalize: Union[None, Callable] = None,
+    ) -> None:
+        super().__init__(
+            normalize=normalize, input_height=input_height, gaussian_blur=gaussian_blur, jitter_strength=jitter_strength
+        )
 
-        # image augmentation functions
-        self.train_transform = transforms.Compose(
+        # replace online transform with eval time transform
+        self.online_transform = transforms.Compose(
             [
-                transforms.RandomResizedCrop(height, scale=(0.2, 1.0)),
-                transforms.RandomApply([transforms.ColorJitter(0.4, 0.4, 0.4, 0.1)], p=0.8),  # not strengthened
-                transforms.RandomGrayscale(p=0.2),
-                transforms.RandomApply([GaussianBlur([0.1, 2.0])], p=0.5),
-                transforms.RandomHorizontalFlip(),
-                transforms.ToTensor(),
-                imagenet_normalization(),
+                transforms.Resize(int(self.input_height + 0.1 * self.input_height)),
+                transforms.CenterCrop(self.input_height),
+                self.final_transform,
             ]
         )
 
-    def __call__(self, inp):
-        q = self.train_transform(inp)
-        k = self.train_transform(inp)
-        return q, k
 
+class SimCLRFinetuneTransform(SimCLRTrainDataTransform):
+    """Transforms for SimCLR during the fine-tuning stage.
+
+    Args:
+        input_height (int, optional): expected output size of image. Defaults to 224.
+        jitter_strength (float, optional): color jitter multiplier. Defaults to 1.0.
+        normalize (Callable, optional): optional transform to normalize. Defaults to None.
+        eval_transform (bool, optional): if True, uses validation transforms.
+            Otherwise uses training transforms. Defaults to False.
 
-@under_review()
-class Moco2EvalImagenetTransforms:
-    """Moco 2 augmentation:
+    Transform::
 
-    https://arxiv.org/pdf/2003.04297.pdf
+        Resize(input_height + 10, interpolation=3)
+        transforms.CenterCrop(input_height),
+        transforms.ToTensor()
+
+    Example::
+
+        from pl_bolts.transforms.self_supervised.simclr_transforms import SimCLREvalDataTransform
+
+        transform = SimCLREvalDataTransform(input_height=32)
+        x = sample()
+        xk = transform(x)
     """
 
-    def __init__(self, height: int = 128):
-        if not _TORCHVISION_AVAILABLE:  # pragma: no cover
-            raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
+    def __init__(
+        self,
+        input_height: int = 224,
+        jitter_strength: float = 1.0,
+        normalize: Union[None, Callable] = None,
+        eval_transform: bool = False,
+    ) -> None:
+        super().__init__(
+            input_height=input_height, gaussian_blur=False, jitter_strength=jitter_strength, normalize=normalize
+        )
 
-        self.test_transform = transforms.Compose(
-            [
-                transforms.Resize(height + 32),
-                transforms.CenterCrop(height),
-                transforms.ToTensor(),
-                imagenet_normalization(),
+        if eval_transform:
+            self.data_transforms = [
+                transforms.Resize(int(self.input_height + 0.1 * self.input_height)),
+                transforms.CenterCrop(self.input_height),
             ]
-        )
 
-    def __call__(self, inp):
-        q = self.test_transform(inp)
-        k = self.test_transform(inp)
-        return q, k
-
-
-@under_review()
-class GaussianBlur:
-    """Gaussian blur augmentation in SimCLR https://arxiv.org/abs/2002.05709."""
-
-    def __init__(self, sigma=(0.1, 2.0)):
-        if not _PIL_AVAILABLE:  # pragma: no cover
-            raise ModuleNotFoundError(
-                "You want to use `Pillow` which is not installed yet, install it with `pip install Pillow`."
-            )
-        self.sigma = sigma
-
-    def __call__(self, x):
-        sigma = random.uniform(self.sigma[0], self.sigma[1])
-        x = x.filter(ImageFilter.GaussianBlur(radius=sigma))
-        return x
+        self.transform = transforms.Compose([self.data_transforms, self.final_transform])
+
+    def __call__(self, sample: Tensor) -> Tensor:
+        return self.transform(sample)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/resnets.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/resnets.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 @under_review()
 class BasicBlock(nn.Module):
     expansion = 1
 
     def __init__(
         self, inplanes, planes, stride=1, downsample=None, groups=1, base_width=64, dilation=1, norm_layer=None
-    ):
+    ) -> None:
         super().__init__()
         if norm_layer is None:
             norm_layer = nn.BatchNorm2d
         if groups != 1 or base_width != 64:
             raise ValueError("BasicBlock only supports groups=1 and base_width=64")
         if dilation > 1:
             raise NotImplementedError("Dilation > 1 not supported in BasicBlock")
@@ -95,15 +95,15 @@
 
 @under_review()
 class Bottleneck(nn.Module):
     expansion = 4
 
     def __init__(
         self, inplanes, planes, stride=1, downsample=None, groups=1, base_width=64, dilation=1, norm_layer=None
-    ):
+    ) -> None:
         super().__init__()
         if norm_layer is None:
             norm_layer = nn.BatchNorm2d
         width = int(planes * (base_width / 64.0)) * groups
         # Both self.conv2 and self.downsample layers downsample the input when stride != 1
         self.conv1 = conv1x1(inplanes, width)
         self.bn1 = norm_layer(width)
@@ -149,15 +149,15 @@
         groups=1,
         width_per_group=64,
         replace_stride_with_dilation=None,
         norm_layer=None,
         return_all_feature_maps=False,
         first_conv=True,
         maxpool1=True,
-    ):
+    ) -> None:
         super().__init__()
         if norm_layer is None:
             norm_layer = nn.BatchNorm2d
         self._norm_layer = norm_layer
         self.return_all_feature_maps = return_all_feature_maps
 
         self.inplanes = 64
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simclr/simclr_finetuner.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simclr/simclr_finetuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from argparse import ArgumentParser
 
 from pytorch_lightning import Trainer, seed_everything
 
 from pl_bolts.models.self_supervised.simclr.simclr_module import SimCLR
-from pl_bolts.models.self_supervised.simclr.transforms import SimCLRFinetuneTransform
 from pl_bolts.models.self_supervised.ssl_finetuner import SSLFineTuner
 from pl_bolts.transforms.dataset_normalizations import (
     cifar10_normalization,
     imagenet_normalization,
     stl10_normalization,
 )
+from pl_bolts.transforms.self_supervised.simclr_transforms import SimCLRFinetuneTransform
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 def cli_main():  # pragma: no cover
     from pl_bolts.datamodules import CIFAR10DataModule, ImagenetDataModule, STL10DataModule
 
@@ -123,15 +123,15 @@
 
     trainer = Trainer(
         gpus=args.gpus,
         num_nodes=1,
         precision=16,
         max_epochs=args.num_epochs,
         accelerator="ddp",
-        sync_batchnorm=True if args.gpus > 1 else False,
+        sync_batchnorm=args.gpus > 1,
     )
 
     trainer.fit(tuner, dm)
     trainer.test(datamodule=dm)
 
 
 if __name__ == "__main__":
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simclr/simclr_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simclr/simclr_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from argparse import ArgumentParser
 
 import torch
 from pytorch_lightning import LightningModule, Trainer
 from pytorch_lightning.callbacks import LearningRateMonitor, ModelCheckpoint
 from torch import Tensor, nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.models.self_supervised.resnets import resnet18, resnet50
 from pl_bolts.optimizers.lars import LARS
 from pl_bolts.optimizers.lr_scheduler import linear_warmup_decay
 from pl_bolts.transforms.dataset_normalizations import (
     cifar10_normalization,
     imagenet_normalization,
@@ -39,15 +39,15 @@
         idx_from = torch.distributed.get_rank() * ctx.batch_size
         idx_to = (torch.distributed.get_rank() + 1) * ctx.batch_size
         return grad_input[idx_from:idx_to]
 
 
 @under_review()
 class Projection(nn.Module):
-    def __init__(self, input_dim=2048, hidden_dim=2048, output_dim=128):
+    def __init__(self, input_dim=2048, hidden_dim=2048, output_dim=128) -> None:
         super().__init__()
         self.output_dim = output_dim
         self.input_dim = input_dim
         self.hidden_dim = hidden_dim
 
         self.model = nn.Sequential(
             nn.Linear(self.input_dim, self.hidden_dim),
@@ -81,15 +81,15 @@
         optimizer: str = "adam",
         exclude_bn_bias: bool = False,
         start_lr: float = 0.0,
         learning_rate: float = 1e-3,
         final_lr: float = 0.0,
         weight_decay: float = 1e-6,
         **kwargs
-    ):
+    ) -> None:
         """
         Args:
             batch_size: the batch size
             num_samples: num samples in the dataset
             warmup_epochs: epochs to warmup the lr for
             lr: the optimizer learning rate
             opt_weight_decay: the optimizer weight decay
@@ -153,17 +153,15 @@
         h1 = self(img1)
         h2 = self(img2)
 
         # get z representations
         z1 = self.projection(h1)
         z2 = self.projection(h2)
 
-        loss = self.nt_xent_loss(z1, z2, self.temperature)
-
-        return loss
+        return self.nt_xent_loss(z1, z2, self.temperature)
 
     def training_step(self, batch, batch_idx):
         loss = self.shared_step(batch)
 
         self.log("train_loss", loss, on_step=True, on_epoch=False)
         return loss
 
@@ -176,15 +174,15 @@
     def exclude_from_wt_decay(self, named_params, weight_decay, skip_list=("bias", "bn")):
         params = []
         excluded_params = []
 
         for name, param in named_params:
             if not param.requires_grad:
                 continue
-            elif any(layer_name in name for layer_name in skip_list):
+            if any(layer_name in name for layer_name in skip_list):
                 excluded_params.append(param)
             else:
                 params.append(param)
 
         return [
             {"params": params, "weight_decay": weight_decay},
             {
@@ -255,17 +253,15 @@
         row_sub = Tensor(neg.shape).fill_(math.e ** (1 / temperature)).to(neg.device)
         neg = torch.clamp(neg - row_sub, min=eps)  # clamp for numerical stability
 
         # Positive similarity, pos becomes [2 * batch_size]
         pos = torch.exp(torch.sum(out_1 * out_2, dim=-1) / temperature)
         pos = torch.cat([pos, pos], dim=0)
 
-        loss = -torch.log(pos / (neg + eps)).mean()
-
-        return loss
+        return -torch.log(pos / (neg + eps)).mean()
 
     @staticmethod
     def add_model_specific_args(parent_parser):
         parser = ArgumentParser(parents=[parent_parser], add_help=False)
 
         # model params
         parser.add_argument("--arch", default="resnet50", type=str, help="convnet architecture")
@@ -304,15 +300,15 @@
         return parser
 
 
 @under_review()
 def cli_main():
     from pl_bolts.callbacks.ssl_online import SSLOnlineEvaluator
     from pl_bolts.datamodules import CIFAR10DataModule, ImagenetDataModule, STL10DataModule
-    from pl_bolts.models.self_supervised.simclr.transforms import SimCLREvalDataTransform, SimCLRTrainDataTransform
+    from pl_bolts.transforms.self_supervised.simclr_transforms import SimCLREvalDataTransform, SimCLRTrainDataTransform
 
     parser = ArgumentParser()
 
     # model args
     parser = SimCLR.add_model_specific_args(parser)
     args = parser.parse_args()
 
@@ -411,15 +407,15 @@
 
     trainer = Trainer(
         max_epochs=args.max_epochs,
         max_steps=None if args.max_steps == -1 else args.max_steps,
         gpus=args.gpus,
         num_nodes=args.num_nodes,
         accelerator="ddp" if args.gpus > 1 else None,
-        sync_batchnorm=True if args.gpus > 1 else False,
+        sync_batchnorm=args.gpus > 1,
         precision=32 if args.fp32 else 16,
         callbacks=callbacks,
         fast_dev_run=args.fast_dev_run,
     )
 
     trainer.fit(model, datamodule=dm)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simclr/transforms.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/swav_transforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,157 +1,169 @@
+from typing import List, Tuple
+
+from torch import Tensor
+
 from pl_bolts.utils import _TORCHVISION_AVAILABLE
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _TORCHVISION_AVAILABLE:
     from torchvision import transforms
 else:  # pragma: no cover
     warn_missing_pkg("torchvision")
 
 
-class SimCLRTrainDataTransform:
-    """Transforms for SimCLR during training step of the pre-training stage.
-
-    Transform::
-
-        RandomResizedCrop(size=self.input_height)
-        RandomHorizontalFlip()
-        RandomApply([color_jitter], p=0.8)
-        RandomGrayscale(p=0.2)
-        RandomApply([GaussianBlur(kernel_size=int(0.1 * self.input_height))], p=0.5)
-        transforms.ToTensor()
-
-    Example::
-
-        from pl_bolts.models.self_supervised.simclr.transforms import SimCLRTrainDataTransform
-
-        transform = SimCLRTrainDataTransform(input_height=32)
-        x = sample()
-        (xi, xj, xk) = transform(x) # xk is only for the online evaluator if used
-    """
-
+class SwAVTrainDataTransform:
     def __init__(
-        self, input_height: int = 224, gaussian_blur: bool = True, jitter_strength: float = 1.0, normalize=None
+        self,
+        normalize=None,
+        size_crops: Tuple[int] = (96, 36),
+        num_crops: Tuple[int] = (2, 4),
+        min_scale_crops: Tuple[float] = (0.33, 0.10),
+        max_scale_crops: Tuple[float] = (1, 0.33),
+        gaussian_blur: bool = True,
+        jitter_strength: float = 1.0,
     ) -> None:
-
-        if not _TORCHVISION_AVAILABLE:  # pragma: no cover
-            raise ModuleNotFoundError("You want to use `transforms` from `torchvision` which is not installed yet.")
-
         self.jitter_strength = jitter_strength
-        self.input_height = input_height
         self.gaussian_blur = gaussian_blur
-        self.normalize = normalize
+
+        if len(size_crops) != len(num_crops):
+            raise AssertionError("len(size_crops) should equal len(num_crops).")
+        if len(min_scale_crops) != len(num_crops):
+            raise AssertionError("len(min_scale_crops) should equal len(num_crops).")
+        if len(max_scale_crops) != len(num_crops):
+            raise AssertionError("len(max_scale_crops) should equal len(num_crops).")
+
+        self.size_crops = size_crops
+        self.num_crops = num_crops
+        self.min_scale_crops = min_scale_crops
+        self.max_scale_crops = max_scale_crops
 
         self.color_jitter = transforms.ColorJitter(
             0.8 * self.jitter_strength,
             0.8 * self.jitter_strength,
             0.8 * self.jitter_strength,
             0.2 * self.jitter_strength,
         )
 
-        data_transforms = [
-            transforms.RandomResizedCrop(size=self.input_height),
-            transforms.RandomHorizontalFlip(p=0.5),
-            transforms.RandomApply([self.color_jitter], p=0.8),
-            transforms.RandomGrayscale(p=0.2),
-        ]
+        transform = []
+        color_transform = [transforms.RandomApply([self.color_jitter], p=0.8), transforms.RandomGrayscale(p=0.2)]
 
         if self.gaussian_blur:
-            kernel_size = int(0.1 * self.input_height)
+            kernel_size = int(0.1 * self.size_crops[0])
             if kernel_size % 2 == 0:
                 kernel_size += 1
 
-            data_transforms.append(transforms.RandomApply([transforms.GaussianBlur(kernel_size=kernel_size)], p=0.5))
+            # Resort to torchvision gaussian blur instead of custom implementation
+            color_transform.append(transforms.RandomApply([transforms.GaussianBlur(kernel_size=kernel_size)], p=0.5))
 
-        self.data_transforms = transforms.Compose(data_transforms)
+        self.color_transform = transforms.Compose(color_transform)
 
         if normalize is None:
             self.final_transform = transforms.ToTensor()
         else:
             self.final_transform = transforms.Compose([transforms.ToTensor(), normalize])
 
-        self.train_transform = transforms.Compose([self.data_transforms, self.final_transform])
+        for i in range(len(self.size_crops)):
+            random_resized_crop = transforms.RandomResizedCrop(
+                self.size_crops[i],
+                scale=(self.min_scale_crops[i], self.max_scale_crops[i]),
+            )
+
+            transform.extend(
+                [
+                    transforms.Compose(
+                        [
+                            random_resized_crop,
+                            transforms.RandomHorizontalFlip(p=0.5),
+                            self.color_transform,
+                            self.final_transform,
+                        ]
+                    )
+                ]
+                * self.num_crops[i]
+            )
+
+        self.transform = transform
 
         # add online train transform of the size of global view
-        self.online_transform = transforms.Compose(
-            [transforms.RandomResizedCrop(self.input_height), transforms.RandomHorizontalFlip(), self.final_transform]
+        online_train_transform = transforms.Compose(
+            [transforms.RandomResizedCrop(self.size_crops[0]), transforms.RandomHorizontalFlip(), self.final_transform]
         )
 
-    def __call__(self, sample):
-        transform = self.train_transform
-
-        xi = transform(sample)
-        xj = transform(sample)
-
-        return xi, xj, self.online_transform(sample)
-
-
-class SimCLREvalDataTransform(SimCLRTrainDataTransform):
-    """Transforms for SimCLR during the validation step of the pre-training stage.
+        self.transform.append(online_train_transform)
 
-    Transform::
+    def __call__(self, sample: Tensor) -> List[Tensor]:
+        return [transform(sample) for transform in self.transform]
 
-        Resize(input_height + 10, interpolation=3)
-        transforms.CenterCrop(input_height),
-        transforms.ToTensor()
-
-    Example::
-
-        from pl_bolts.models.self_supervised.simclr.transforms import SimCLREvalDataTransform
-
-        transform = SimCLREvalDataTransform(input_height=32)
-        x = sample()
-        (xi, xj, xk) = transform(x) # xk is only for the online evaluator if used
-    """
 
+class SwAVEvalDataTransform(SwAVTrainDataTransform):
     def __init__(
-        self, input_height: int = 224, gaussian_blur: bool = True, jitter_strength: float = 1.0, normalize=None
-    ):
+        self,
+        normalize=None,
+        size_crops: Tuple[int] = (96, 36),
+        num_crops: Tuple[int] = (2, 4),
+        min_scale_crops: Tuple[float] = (0.33, 0.10),
+        max_scale_crops: Tuple[float] = (1, 0.33),
+        gaussian_blur: bool = True,
+        jitter_strength: float = 1.0,
+    ) -> None:
         super().__init__(
-            normalize=normalize, input_height=input_height, gaussian_blur=gaussian_blur, jitter_strength=jitter_strength
+            normalize=normalize,
+            size_crops=size_crops,
+            num_crops=num_crops,
+            min_scale_crops=min_scale_crops,
+            max_scale_crops=max_scale_crops,
+            gaussian_blur=gaussian_blur,
+            jitter_strength=jitter_strength,
         )
 
-        # replace online transform with eval time transform
-        self.online_transform = transforms.Compose(
+        input_height = self.size_crops[0]  # get global view crop
+        test_transform = transforms.Compose(
             [
-                transforms.Resize(int(self.input_height + 0.1 * self.input_height)),
-                transforms.CenterCrop(self.input_height),
+                transforms.Resize(int(input_height + 0.1 * input_height)),
+                transforms.CenterCrop(input_height),
                 self.final_transform,
             ]
         )
 
+        # replace last transform to eval transform in self.transform list
+        self.transform[-1] = test_transform
 
-class SimCLRFinetuneTransform(SimCLRTrainDataTransform):
-    """Transforms for SimCLR during the fine-tuning stage.
-
-    Transform::
-
-        Resize(input_height + 10, interpolation=3)
-        transforms.CenterCrop(input_height),
-        transforms.ToTensor()
-
-    Example::
-
-        from pl_bolts.models.self_supervised.simclr.transforms import SimCLREvalDataTransform
-
-        transform = SimCLREvalDataTransform(input_height=32)
-        x = sample()
-        xk = transform(x)
-    """
 
+class SwAVFinetuneTransform:
     def __init__(
         self, input_height: int = 224, jitter_strength: float = 1.0, normalize=None, eval_transform: bool = False
     ) -> None:
+        self.jitter_strength = jitter_strength
+        self.input_height = input_height
+        self.normalize = normalize
 
-        super().__init__(
-            normalize=normalize, input_height=input_height, gaussian_blur=None, jitter_strength=jitter_strength
+        self.color_jitter = transforms.ColorJitter(
+            0.8 * self.jitter_strength,
+            0.8 * self.jitter_strength,
+            0.8 * self.jitter_strength,
+            0.2 * self.jitter_strength,
         )
 
-        if eval_transform:
-            self.data_transforms = [
+        if not eval_transform:
+            data_transforms = [
+                transforms.RandomResizedCrop(size=self.input_height),
+                transforms.RandomHorizontalFlip(p=0.5),
+                transforms.RandomApply([self.color_jitter], p=0.8),
+                transforms.RandomGrayscale(p=0.2),
+            ]
+        else:
+            data_transforms = [
                 transforms.Resize(int(self.input_height + 0.1 * self.input_height)),
                 transforms.CenterCrop(self.input_height),
             ]
 
-        self.transform = transforms.Compose([self.data_transforms, self.final_transform])
+        if normalize is None:
+            final_transform = transforms.ToTensor()
+        else:
+            final_transform = transforms.Compose([transforms.ToTensor(), normalize])
+
+        data_transforms.append(final_transform)
+        self.transform = transforms.Compose(data_transforms)
 
-    def __call__(self, sample):
+    def __call__(self, sample: Tensor) -> Tensor:
         return self.transform(sample)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/simsiam/simsiam_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/simsiam/simsiam_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser
 from copy import deepcopy
 from typing import Any, Dict, List, Union
 
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
+import torch.nn.functional as F  # noqa: N812
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from torch import Tensor
 
 from pl_bolts.models.self_supervised.byol.models import MLP, SiameseArm
 from pl_bolts.optimizers.lr_scheduler import LinearWarmupCosineAnnealingLR
 
 
@@ -71,15 +71,14 @@
         encoder_out_dim: int = 2048,
         projector_hidden_dim: int = 2048,
         projector_out_dim: int = 2048,
         predictor_hidden_dim: int = 512,
         exclude_bn_bias: bool = False,
         **kwargs,
     ) -> None:
-
         super().__init__()
         self.save_hyperparameters(ignore="base_encoder")
 
         self.online_network = SiameseArm(base_encoder, encoder_out_dim, projector_hidden_dim, projector_out_dim)
         self.target_network = deepcopy(self.online_network)
         self.predictor = MLP(projector_out_dim, predictor_hidden_dim, projector_out_dim)
 
@@ -124,16 +123,15 @@
             v_online (Tensor): Online network view
             v_target (Tensor): Target network view
         """
         _, z1 = self.online_network(v_online)
         h1 = self.predictor(z1)
         with torch.no_grad():
             _, z2 = self.target_network(v_target)
-        loss = -0.5 * F.cosine_similarity(h1, z2).mean()
-        return loss
+        return -0.5 * F.cosine_similarity(h1, z2).mean()
 
     def configure_optimizers(self):
         """Configure optimizer and learning rate scheduler."""
         if self.hparams.exclude_bn_bias:
             params = self.exclude_from_weight_decay(self.named_parameters(), weight_decay=self.hparams.weight_decay)
         else:
             params = self.parameters()
@@ -155,15 +153,15 @@
         """Exclude parameters from weight decay."""
         params = []
         excluded_params = []
 
         for name, param in named_params:
             if not param.requires_grad:
                 continue
-            elif param.ndim == 1 or name in skip_list:
+            if param.ndim == 1 or name in skip_list:
                 excluded_params.append(param)
             else:
                 params.append(param)
 
         return [
             {"params": params, "weight_decay": weight_decay},
             {"params": excluded_params, "weight_decay": 0.0},
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/ssl_finetuner.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/ssl_finetuner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Tuple
 
 import torch
 from pytorch_lightning import LightningModule
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 from torchmetrics import Accuracy
 
 from pl_bolts.models.self_supervised import SSLEvaluator
 
 
 class SSLFineTuner(LightningModule):
     """Finetunes a self-supervised learning backbone using the standard evaluation protocol of a singler layer MLP
@@ -50,15 +50,15 @@
         learning_rate: float = 0.1,
         weight_decay: float = 1e-6,
         nesterov: bool = False,
         scheduler_type: str = "cosine",
         decay_epochs: Tuple = (60, 80),
         gamma: float = 0.1,
         final_lr: float = 0.0,
-    ):
+    ) -> None:
         """
         Args:
             backbone: a pretrained model
             in_features: feature dim of backbone outputs
             num_classes: classes of the dataset
             hidden_dim: dim of the MLP (1024 default used in self-supervised literature)
         """
@@ -74,17 +74,17 @@
         self.epochs = epochs
         self.final_lr = final_lr
 
         self.backbone = backbone
         self.linear_layer = SSLEvaluator(n_input=in_features, n_classes=num_classes, p=dropout, n_hidden=hidden_dim)
 
         # metrics
-        self.train_acc = Accuracy()
-        self.val_acc = Accuracy(compute_on_step=False)
-        self.test_acc = Accuracy(compute_on_step=False)
+        self.train_acc = Accuracy(task="multiclass", num_classes=num_classes)
+        self.val_acc = Accuracy(task="multiclass", num_classes=num_classes, compute_on_step=False)
+        self.test_acc = Accuracy(task="multiclass", num_classes=num_classes, compute_on_step=False)
 
     def on_train_epoch_start(self) -> None:
         self.backbone.eval()
 
     def training_step(self, batch, batch_idx):
         loss, logits, y = self.shared_step(batch)
         acc = self.train_acc(logits.softmax(-1), y)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pl_bolts.models.self_supervised.swav.loss import SWAVLoss
 from pl_bolts.models.self_supervised.swav.swav_module import SwAV
 from pl_bolts.models.self_supervised.swav.swav_resnet import resnet18, resnet50
-from pl_bolts.models.self_supervised.swav.transforms import (
+from pl_bolts.transforms.self_supervised.swav_transforms import (
     SwAVEvalDataTransform,
     SwAVFinetuneTransform,
     SwAVTrainDataTransform,
 )
 
 __all__ = [
     "SwAV",
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/loss.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/loss.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 
 
 class SWAVLoss(nn.Module):
     def __init__(
         self,
         temperature: float,
         crops_for_assign: tuple,
-        nmb_crops: tuple,
+        num_crops: tuple,
         sinkhorn_iterations: int,
         epsilon: float,
         gpus: int,
         num_nodes: int,
-    ):
+    ) -> None:
         """Implementation for SWAV loss function.
 
         Args:
             temperature:  loss temperature
             crops_for_assign: list of crop ids for computing assignment
-            nmb_crops: number of global and local crops, ex: [2, 6]
+            num_crops: number of global and local crops, ex: [2, 6]
             sinkhorn_iterations: iterations for sinkhorn normalization
             epsilon: epsilon val for swav assignments
             gpus: number of gpus per node used in training, passed to SwAV module
                 to manage the queue and select distributed sinkhorn
             num_nodes:  num_nodes: number of nodes to train on
         """
         super().__init__()
         self.temperature = temperature
         self.crops_for_assign = crops_for_assign
         self.softmax = nn.Softmax(dim=1)
         self.sinkhorn_iterations = sinkhorn_iterations
         self.epsilon = epsilon
-        self.nmb_crops = nmb_crops
+        self.num_crops = num_crops
         self.gpus = gpus
         self.num_nodes = num_nodes
         if self.gpus * self.num_nodes > 1:
             self.assignment_fn = self.distributed_sinkhorn
         else:
             self.assignment_fn = self.sinkhorn
 
@@ -59,73 +59,73 @@
 
                 # Time to use the queue
                 if queue is not None:
                     if use_queue or not torch.all(queue[i, -1, :] == 0):
                         use_queue = True
                         out = torch.cat((torch.mm(queue[i], prototype_weights.t()), out))
                     # fill the queue
-                    queue[i, batch_size:] = self.queue[i, :-batch_size].clone()  # type: ignore
+                    queue[i, batch_size:] = self.queue[i, :-batch_size].clone()  # type: ignore[index]
                     queue[i, :batch_size] = embedding[crop_id * batch_size : (crop_id + 1) * batch_size]
                 # get assignments
                 q = torch.exp(out / self.epsilon).t()
                 q = self.assignment_fn(q, self.sinkhorn_iterations)[-batch_size:]
 
             # cluster assignment prediction
             subloss = 0
-            for v in np.delete(np.arange(np.sum(self.nmb_crops)), crop_id):
+            for v in np.delete(np.arange(np.sum(self.num_crops)), crop_id):
                 p = self.softmax(output[batch_size * v : batch_size * (v + 1)] / self.temperature)
                 subloss -= torch.mean(torch.sum(q * torch.log(p), dim=1))
-            loss += subloss / (np.sum(self.nmb_crops) - 1)
+            loss += subloss / (np.sum(self.num_crops) - 1)
         loss /= len(self.crops_for_assign)  # type: ignore
         return loss, queue, use_queue
 
-    def sinkhorn(self, Q: torch.Tensor, nmb_iters: int) -> torch.Tensor:
+    def sinkhorn(self, q: torch.Tensor, num_iters: int) -> torch.Tensor:
         """Implementation of Sinkhorn clustering."""
         with torch.no_grad():
-            sum_Q = torch.sum(Q)
-            Q /= sum_Q
+            sum_q = torch.sum(q)
+            q /= sum_q
 
-            K, B = Q.shape
+            dim_k, dim_b = q.shape
 
             if self.gpus > 0:
-                u = torch.zeros(K).cuda()
-                r = torch.ones(K).cuda() / K
-                c = torch.ones(B).cuda() / B
+                # u = torch.zeros(K).cuda()
+                r = torch.ones(dim_k).cuda() / dim_k
+                c = torch.ones(dim_b).cuda() / dim_b
             else:
-                u = torch.zeros(K)
-                r = torch.ones(K) / K
-                c = torch.ones(B) / B
+                # u = torch.zeros(K)
+                r = torch.ones(dim_k) / dim_k
+                c = torch.ones(dim_b) / dim_b
 
-            for _ in range(nmb_iters):
-                u = torch.sum(Q, dim=1)
+            for _ in range(num_iters):
+                u = torch.sum(q, dim=1)
 
-                Q *= (r / u).unsqueeze(1)
-                Q *= (c / torch.sum(Q, dim=0)).unsqueeze(0)
+                q *= (r / u).unsqueeze(1)
+                q *= (c / torch.sum(q, dim=0)).unsqueeze(0)
 
-            return (Q / torch.sum(Q, dim=0, keepdim=True)).t().float()
+            return (q / torch.sum(q, dim=0, keepdim=True)).t().float()
 
-    def distributed_sinkhorn(self, Q: torch.Tensor, nmb_iters: int) -> torch.Tensor:
+    def distributed_sinkhorn(self, q: torch.Tensor, num_iters: int) -> torch.Tensor:
         """Implementation of Distributed Sinkhorn."""
         with torch.no_grad():
-            sum_Q = torch.sum(Q)
-            dist.all_reduce(sum_Q)
-            Q /= sum_Q
+            sum_q = torch.sum(q)
+            dist.all_reduce(sum_q)
+            q /= sum_q
 
             if self.gpus > 0:
-                u = torch.zeros(Q.shape[0]).cuda(non_blocking=True)
-                r = torch.ones(Q.shape[0]).cuda(non_blocking=True) / Q.shape[0]
-                c = torch.ones(Q.shape[1]).cuda(non_blocking=True) / (self.gpus * Q.shape[1])
+                # u = torch.zeros(q.shape[0]).cuda(non_blocking=True)
+                r = torch.ones(q.shape[0]).cuda(non_blocking=True) / q.shape[0]
+                c = torch.ones(q.shape[1]).cuda(non_blocking=True) / (self.gpus * q.shape[1])
             else:
-                u = torch.zeros(Q.shape[0])
-                r = torch.ones(Q.shape[0]) / Q.shape[0]
-                c = torch.ones(Q.shape[1]) / (self.gpus * Q.shape[1])
+                # u = torch.zeros(q.shape[0])
+                r = torch.ones(q.shape[0]) / q.shape[0]
+                c = torch.ones(q.shape[1]) / (self.gpus * q.shape[1])
 
-            curr_sum = torch.sum(Q, dim=1)
+            curr_sum = torch.sum(q, dim=1)
             dist.all_reduce(curr_sum)
 
-            for _ in range(nmb_iters):
+            for _ in range(num_iters):
                 u = curr_sum
-                Q *= (r / u).unsqueeze(1)
-                Q *= (c / torch.sum(Q, dim=0)).unsqueeze(0)
-                curr_sum = torch.sum(Q, dim=1)
+                q *= (r / u).unsqueeze(1)
+                q *= (c / torch.sum(q, dim=0)).unsqueeze(0)
+                curr_sum = torch.sum(q, dim=1)
                 dist.all_reduce(curr_sum)
-            return (Q / torch.sum(Q, dim=0, keepdim=True)).t().float()
+            return (q / torch.sum(q, dim=0, keepdim=True)).t().float()
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/swav_finetuner.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/swav_finetuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from argparse import ArgumentParser
 
 from pytorch_lightning import Trainer, seed_everything
 
 from pl_bolts.models.self_supervised.ssl_finetuner import SSLFineTuner
 from pl_bolts.models.self_supervised.swav.swav_module import SwAV
-from pl_bolts.models.self_supervised.swav.transforms import SwAVFinetuneTransform
 from pl_bolts.transforms.dataset_normalizations import imagenet_normalization, stl10_normalization
+from pl_bolts.transforms.self_supervised.swav_transforms import SwAVFinetuneTransform
 
 
 def cli_main():  # pragma: no cover
     from pl_bolts.datamodules import ImagenetDataModule, STL10DataModule
 
     seed_everything(1234)
 
@@ -102,15 +102,15 @@
 
     trainer = Trainer(
         gpus=args.gpus,
         num_nodes=1,
         precision=16,
         max_epochs=args.num_epochs,
         accelerator="ddp",
-        sync_batchnorm=True if args.gpus > 1 else False,
+        sync_batchnorm=args.gpus > 1,
     )
 
     trainer.fit(tuner, dm)
     trainer.test(datamodule=dm)
 
 
 if __name__ == "__main__":
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/swav_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/swav_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,60 +27,60 @@
         dataset: str,
         num_nodes: int = 1,
         arch: str = "resnet50",
         hidden_mlp: int = 2048,
         feat_dim: int = 128,
         warmup_epochs: int = 10,
         max_epochs: int = 100,
-        nmb_prototypes: int = 3000,
+        num_prototypes: int = 3000,
         freeze_prototypes_epochs: int = 1,
         temperature: float = 0.1,
         sinkhorn_iterations: int = 3,
         queue_length: int = 0,  # must be divisible by total batch-size
         queue_path: str = "queue",
         epoch_queue_starts: int = 15,
         crops_for_assign: tuple = (0, 1),
-        nmb_crops: tuple = (2, 6),
+        num_crops: tuple = (2, 6),
         first_conv: bool = True,
         maxpool1: bool = True,
         optimizer: str = "adam",
         exclude_bn_bias: bool = False,
         start_lr: float = 0.0,
         learning_rate: float = 1e-3,
         final_lr: float = 0.0,
         weight_decay: float = 1e-6,
         epsilon: float = 0.05,
         **kwargs
-    ):
+    ) -> None:
         """
         Args:
             gpus: number of gpus per node used in training, passed to SwAV module
                 to manage the queue and select distributed sinkhorn
             num_nodes: number of nodes to train on
             num_samples: number of image samples used for training
             batch_size: batch size per GPU in ddp
             dataset: dataset being used for train/val
             arch: encoder architecture used for pre-training
             hidden_mlp: hidden layer of non-linear projection head, set to 0
                 to use a linear projection head
             feat_dim: output dim of the projection head
             warmup_epochs: apply linear warmup for this many epochs
             max_epochs: epoch count for pre-training
-            nmb_prototypes: count of prototype vectors
+            num_prototypes: count of prototype vectors
             freeze_prototypes_epochs: epoch till which gradients of prototype layer
                 are frozen
             temperature: loss temperature
             sinkhorn_iterations: iterations for sinkhorn normalization
             queue_length: set queue when batch size is small,
                 must be divisible by total batch-size (i.e. total_gpus * batch_size),
                 set to 0 to remove the queue
             queue_path: folder within the logs directory
             epoch_queue_starts: start uing the queue after this epoch
             crops_for_assign: list of crop ids for computing assignment
-            nmb_crops: number of global and local crops, ex: [2, 6]
+            num_crops: number of global and local crops, ex: [2, 6]
             first_conv: keep first conv same as the original resnet architecture,
                 if set to false it is replace by a kernel 3, stride 1 conv (cifar-10)
             maxpool1: keep first maxpool layer same as the original resnet architecture,
                 if set to false, first maxpool is turned off (cifar10, maybe stl10)
             optimizer: optimizer to use
             exclude_bn_bias: exclude batchnorm and bias layers from weight decay in optimizers
             start_lr: starting lr for linear warmup
@@ -97,23 +97,23 @@
         self.arch = arch
         self.dataset = dataset
         self.num_samples = num_samples
         self.batch_size = batch_size
 
         self.hidden_mlp = hidden_mlp
         self.feat_dim = feat_dim
-        self.nmb_prototypes = nmb_prototypes
+        self.num_prototypes = num_prototypes
         self.freeze_prototypes_epochs = freeze_prototypes_epochs
         self.sinkhorn_iterations = sinkhorn_iterations
 
         self.queue_length = queue_length
         self.queue_path = queue_path
         self.epoch_queue_starts = epoch_queue_starts
         self.crops_for_assign = crops_for_assign
-        self.nmb_crops = nmb_crops
+        self.num_crops = num_crops
 
         self.first_conv = first_conv
         self.maxpool1 = maxpool1
 
         self.optim = optimizer
         self.exclude_bn_bias = exclude_bn_bias
         self.weight_decay = weight_decay
@@ -128,15 +128,15 @@
 
         self.model = self.init_model()
         self.criterion = SWAVLoss(
             gpus=self.gpus,
             num_nodes=self.num_nodes,
             temperature=self.temperature,
             crops_for_assign=self.crops_for_assign,
-            nmb_crops=self.nmb_crops,
+            num_crops=self.num_crops,
             sinkhorn_iterations=self.sinkhorn_iterations,
             epsilon=self.epsilon,
         )
         self.use_the_queue = None
         # compute iters per epoch
         global_batch_size = self.num_nodes * self.gpus * self.batch_size if self.gpus > 0 else self.batch_size
         self.train_iters_per_epoch = self.num_samples // global_batch_size
@@ -159,15 +159,15 @@
         elif self.arch == "resnet50":
             backbone = resnet50
 
         return backbone(
             normalize=True,
             hidden_mlp=self.hidden_mlp,
             output_dim=self.feat_dim,
-            nmb_prototypes=self.nmb_prototypes,
+            num_prototypes=self.num_prototypes,
             first_conv=self.first_conv,
             maxpool1=self.maxpool1,
         )
 
     def forward(self, x):
         # pass single batch from the resnet backbone
         return self.model.forward_backbone(x)
@@ -243,15 +243,15 @@
     def exclude_from_wt_decay(self, named_params, weight_decay, skip_list=("bias", "bn")):
         params = []
         excluded_params = []
 
         for name, param in named_params:
             if not param.requires_grad:
                 continue
-            elif any(layer_name in name for layer_name in skip_list):
+            if any(layer_name in name for layer_name in skip_list):
                 excluded_params.append(param)
             else:
                 params.append(param)
 
         return [{"params": params, "weight_decay": weight_decay}, {"params": excluded_params, "weight_decay": 0.0}]
 
     def configure_optimizers(self):
@@ -303,15 +303,15 @@
         parser.add_argument("--gaussian_blur", action="store_true", help="add gaussian blur")
         parser.add_argument("--jitter_strength", type=float, default=1.0, help="jitter strength")
         parser.add_argument("--dataset", type=str, default="stl10", help="stl10, cifar10")
         parser.add_argument("--data_dir", type=str, default=".", help="path to download data")
         parser.add_argument("--queue_path", type=str, default="queue", help="path for queue")
 
         parser.add_argument(
-            "--nmb_crops", type=int, default=[2, 4], nargs="+", help="list of number of crops (example: [2, 6])"
+            "--num_crops", type=int, default=[2, 4], nargs="+", help="list of number of crops (example: [2, 6])"
         )
         parser.add_argument(
             "--size_crops", type=int, default=[96, 36], nargs="+", help="crops resolutions (example: [224, 96])"
         )
         parser.add_argument(
             "--min_scale_crops",
             type=float,
@@ -355,15 +355,15 @@
         parser.add_argument("--temperature", default=0.1, type=float, help="temperature parameter in training loss")
         parser.add_argument(
             "--epsilon", default=0.05, type=float, help="regularization parameter for Sinkhorn-Knopp algorithm"
         )
         parser.add_argument(
             "--sinkhorn_iterations", default=3, type=int, help="number of iterations in Sinkhorn-Knopp algorithm"
         )
-        parser.add_argument("--nmb_prototypes", default=512, type=int, help="number of prototypes")
+        parser.add_argument("--num_prototypes", default=512, type=int, help="number of prototypes")
         parser.add_argument(
             "--queue_length",
             type=int,
             default=0,
             help="length of the queue (0 for no queue); must be divisible by total batch size",
         )
         parser.add_argument(
@@ -378,15 +378,15 @@
 
         return parser
 
 
 def cli_main():
     from pl_bolts.callbacks.ssl_online import SSLOnlineEvaluator
     from pl_bolts.datamodules import CIFAR10DataModule, ImagenetDataModule, STL10DataModule
-    from pl_bolts.models.self_supervised.swav.transforms import SwAVEvalDataTransform, SwAVTrainDataTransform
+    from pl_bolts.transforms.self_supervised.swav_transforms import SwAVEvalDataTransform, SwAVTrainDataTransform
 
     parser = ArgumentParser()
 
     # model args
     parser = SwAV.add_model_specific_args(parser)
     args = parser.parse_args()
 
@@ -411,23 +411,23 @@
         args.maxpool1 = False
         args.first_conv = False
 
         normalization = cifar10_normalization()
 
         # cifar10 specific params
         args.size_crops = [32, 16]
-        args.nmb_crops = [2, 1]
+        args.num_crops = [2, 1]
         args.gaussian_blur = False
     elif args.dataset == "imagenet":
         args.maxpool1 = True
         args.first_conv = True
         normalization = imagenet_normalization()
 
         args.size_crops = [224, 96]
-        args.nmb_crops = [2, 6]
+        args.num_crops = [2, 6]
         args.min_scale_crops = [0.14, 0.05]
         args.max_scale_crops = [1.0, 0.14]
         args.gaussian_blur = True
         args.jitter_strength = 1.0
 
         args.batch_size = 64
         args.num_nodes = 8
@@ -435,38 +435,38 @@
         args.max_epochs = 800
 
         args.optimizer = "lars"
         args.learning_rate = 4.8
         args.final_lr = 0.0048
         args.start_lr = 0.3
 
-        args.nmb_prototypes = 3000
+        args.num_prototypes = 3000
         args.online_ft = True
 
         dm = ImagenetDataModule(data_dir=args.data_dir, batch_size=args.batch_size, num_workers=args.num_workers)
 
         args.num_samples = dm.num_samples
         args.input_height = dm.dims[-1]
     else:
         raise NotImplementedError("other datasets have not been implemented till now")
 
     dm.train_transforms = SwAVTrainDataTransform(
         normalize=normalization,
         size_crops=args.size_crops,
-        nmb_crops=args.nmb_crops,
+        num_crops=args.num_crops,
         min_scale_crops=args.min_scale_crops,
         max_scale_crops=args.max_scale_crops,
         gaussian_blur=args.gaussian_blur,
         jitter_strength=args.jitter_strength,
     )
 
     dm.val_transforms = SwAVEvalDataTransform(
         normalize=normalization,
         size_crops=args.size_crops,
-        nmb_crops=args.nmb_crops,
+        num_crops=args.num_crops,
         min_scale_crops=args.min_scale_crops,
         max_scale_crops=args.max_scale_crops,
         gaussian_blur=args.gaussian_blur,
         jitter_strength=args.jitter_strength,
     )
 
     # swav model init
@@ -490,15 +490,15 @@
 
     trainer = Trainer(
         max_epochs=args.max_epochs,
         max_steps=None if args.max_steps == -1 else args.max_steps,
         gpus=args.gpus,
         num_nodes=args.num_nodes,
         accelerator="ddp" if args.gpus > 1 else None,
-        sync_batchnorm=True if args.gpus > 1 else False,
+        sync_batchnorm=args.gpus > 1,
         precision=32 if args.fp32 else 16,
         callbacks=callbacks,
         fast_dev_run=args.fast_dev_run,
     )
 
     trainer.fit(model, datamodule=dm)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/self_supervised/swav/swav_resnet.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/self_supervised/swav/swav_resnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         planes,
         stride=1,
         downsample=None,
         groups=1,
         base_width=64,
         dilation=1,
         norm_layer=None,
-    ):
+    ) -> None:
         super().__init__()
         if norm_layer is None:
             norm_layer = nn.BatchNorm2d
         if groups != 1 or base_width != 64:
             raise ValueError("BasicBlock only supports groups=1 and base_width=64")
         if dilation > 1:
             raise NotImplementedError("Dilation > 1 not supported in BasicBlock")
@@ -82,15 +82,15 @@
         planes,
         stride=1,
         downsample=None,
         groups=1,
         base_width=64,
         dilation=1,
         norm_layer=None,
-    ):
+    ) -> None:
         super().__init__()
         if norm_layer is None:
             norm_layer = nn.BatchNorm2d
         width = int(planes * (base_width / 64.0)) * groups
         # Both self.conv2 and self.downsample layers downsample the input when stride != 1
         self.conv1 = conv1x1(inplanes, width)
         self.bn1 = norm_layer(width)
@@ -135,19 +135,19 @@
         widen=1,
         width_per_group=64,
         replace_stride_with_dilation=None,
         norm_layer=None,
         normalize=False,
         output_dim=0,
         hidden_mlp=0,
-        nmb_prototypes=0,
+        num_prototypes=0,
         eval_mode=False,
         first_conv=True,
         maxpool1=True,
-    ):
+    ) -> None:
         super().__init__()
         if norm_layer is None:
             norm_layer = nn.BatchNorm2d
         self._norm_layer = norm_layer
 
         self.eval_mode = eval_mode
         self.padding = nn.ConstantPad2d(1, 0.0)
@@ -211,18 +211,18 @@
                 nn.BatchNorm1d(hidden_mlp),
                 nn.ReLU(inplace=True),
                 nn.Linear(hidden_mlp, output_dim),
             )
 
         # prototype layer
         self.prototypes = None
-        if isinstance(nmb_prototypes, list):
-            self.prototypes = MultiPrototypes(output_dim, nmb_prototypes)
-        elif nmb_prototypes > 0:
-            self.prototypes = nn.Linear(output_dim, nmb_prototypes, bias=False)
+        if isinstance(num_prototypes, list):
+            self.prototypes = MultiPrototypes(output_dim, num_prototypes)
+        elif num_prototypes > 0:
+            self.prototypes = nn.Linear(output_dim, num_prototypes, bias=False)
 
         for m in self.modules():
             if isinstance(m, nn.Conv2d):
                 nn.init.kaiming_normal_(m.weight, mode="fan_out", nonlinearity="relu")
             elif isinstance(m, (nn.BatchNorm2d, nn.GroupNorm)):
                 nn.init.constant_(m.weight, 1)
                 nn.init.constant_(m.bias, 0)
@@ -315,41 +315,38 @@
         idx_crops = torch.cumsum(
             torch.unique_consecutive(
                 torch.tensor([inp.shape[-1] for inp in inputs]),
                 return_counts=True,
             )[1],
             0,
         )
-        start_idx = 0
+        start_idx, output = 0, None
         for end_idx in idx_crops:
             _out = torch.cat(inputs[start_idx:end_idx])
 
             if "cuda" in str(self.conv1.weight.device):
                 _out = self.forward_backbone(_out.cuda(non_blocking=True))
             else:
                 _out = self.forward_backbone(_out)
 
-            if start_idx == 0:
-                output = _out
-            else:
-                output = torch.cat((output, _out))
+            output = _out if start_idx == 0 else torch.cat((output, _out))
             start_idx = end_idx
         return self.forward_head(output)
 
 
 class MultiPrototypes(nn.Module):
-    def __init__(self, output_dim, nmb_prototypes):
+    def __init__(self, output_dim, num_prototypes) -> None:
         super().__init__()
-        self.nmb_heads = len(nmb_prototypes)
-        for i, k in enumerate(nmb_prototypes):
+        self.num_heads = len(num_prototypes)
+        for i, k in enumerate(num_prototypes):
             self.add_module("prototypes" + str(i), nn.Linear(output_dim, k, bias=False))
 
     def forward(self, x):
         out = []
-        for i in range(self.nmb_heads):
+        for i in range(self.num_heads):
             out.append(getattr(self, "prototypes" + str(i))(x))
         return out
 
 
 def resnet18(**kwargs):
     return ResNet(BasicBlock, [2, 2, 2, 2], **kwargs)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/vision/image_gpt/gpt2.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/image_gpt/gpt2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from torch import nn
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class Block(nn.Module):
-    def __init__(self, embed_dim, heads):
+    def __init__(self, embed_dim, heads) -> None:
         super().__init__()
         self.ln_1 = nn.LayerNorm(embed_dim)
         self.ln_2 = nn.LayerNorm(embed_dim)
         self.attn = nn.MultiheadAttention(embed_dim, heads)
         self.mlp = nn.Sequential(
             nn.Linear(embed_dim, embed_dim * 4),
             nn.GELU(),
@@ -57,15 +57,15 @@
         self,
         embed_dim: int,
         heads: int,
         layers: int,
         num_positions: int,
         vocab_size: int,
         num_classes: int,
-    ):
+    ) -> None:
         super().__init__()
         self.save_hyperparameters()
 
         self._init_sos_token()
         self._init_embeddings()
         self._init_layers()
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/vision/image_gpt/igpt_module.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/image_gpt/igpt_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,25 @@
 
 from pl_bolts.models.vision.image_gpt.gpt2 import GPT2
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 def _shape_input(x):
-    """shape batch of images for input into GPT2 model."""
+    """Shape batch of images for input into GPT2 model."""
     x = x.view(x.shape[0], -1)  # flatten images into sequences
     x = x.transpose(0, 1).contiguous()  # to shape [seq len, batch]
     return x
 
 
 @under_review()
 class ImageGPT(LightningModule):
-    """
-    **Paper**: `Generative Pretraining from Pixels
-    <https://cdn.openai.com/papers/Generative_Pretraining_from_Pixels_V2.pdf>`_
-    [original paper `code <https://github.com/openai/image-gpt>`_].
+    """**Paper**: `Generative Pretraining from Pixels
+    <https://cdn.openai.com/papers/Generative_Pretraining_from_Pixels_V2.pdf>`_ [original paper `code
+    <https://github.com/openai/image-gpt>`_].
 
     **Paper by:** Mark Che, Alec Radford, Rewon Child, Jeff Wu, Heewoo Jun,
     Prafulla Dhariwal, David Luan, Ilya Sutskever
 
     **Implementation contributed by**:
 
         - `Teddy Koker <https://github.com/teddykoker>`_
@@ -111,15 +110,15 @@
         classify: bool = False,
         batch_size: int = 64,
         learning_rate: float = 1e-2,
         steps: int = 25_000,
         data_dir: str = ".",
         num_workers: int = 8,
         **kwargs,
-    ):
+    ) -> None:
         """
         Args:
             embed_dim: the embedding dim
             heads: number of attention heads
             layers: number of layers
             pixels: number of input pixels
             vocab_size: vocab size
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/vision/pixel_cnn.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/pixel_cnn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""
-PixelCNN
-Implemented by: William Falcon
-Reference: https://arxiv.org/pdf/1905.09272.pdf (page 15)
-Accessed: May 14, 2020
+"""PixelCNN.
+
+Implemented by: William Falcon Reference
+: https: //arxiv.org/pdf/1905.09272.pdf (page 15
+Accessed: May 14, 2020.
 """
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class PixelCNN(nn.Module):
     """Implementation of `Pixel CNN <https://arxiv.org/abs/1606.05328>`_.
@@ -30,15 +30,15 @@
         >>> x = torch.rand(5, 3, 64, 64)
         >>> out = model(x)
         ...
         >>> out.shape
         torch.Size([5, 3, 64, 64])
     """
 
-    def __init__(self, input_channels: int, hidden_channels: int = 256, num_blocks=5):
+    def __init__(self, input_channels: int, hidden_channels: int = 256, num_blocks=5) -> None:
         super().__init__()
         self.input_channels = input_channels
         self.hidden_channels = hidden_channels
 
         self.blocks = nn.ModuleList([self.conv_block(input_channels) for _ in range(num_blocks)])
 
     def conv_block(self, input_channels):
@@ -48,17 +48,15 @@
         pad = nn.ConstantPad2d((0, 0, 1, 0, 0, 0, 0, 0), 1)
         c3 = nn.Conv2d(
             in_channels=self.hidden_channels, out_channels=self.hidden_channels, kernel_size=(2, 1), padding=(0, 1)
         )
         act2 = nn.ReLU()
         c4 = nn.Conv2d(in_channels=self.hidden_channels, out_channels=input_channels, kernel_size=(1, 1))
 
-        block = nn.Sequential(c1, act1, c2, pad, c3, act2, c4)
-        return block
+        return nn.Sequential(c1, act1, c2, pad, c3, act2, c4)
 
     def forward(self, z):
         c = z
         for conv_block in self.blocks:
             c = c + conv_block(c)
 
-        c = F.relu(c)
-        return c
+        return F.relu(c)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/vision/segmentation.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser
 from typing import Any, Dict, Optional
 
 import torch
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from torch import Tensor
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.models.vision.unet import UNet
 
 
 class SemSegment(LightningModule):
     """Basic model for semantic segmentation. Uses UNet architecture by default.
 
@@ -40,15 +40,15 @@
         num_classes: int = 19,
         num_layers: int = 5,
         features_start: int = 64,
         bilinear: bool = False,
         ignore_index: Optional[int] = 250,
         lr: float = 0.01,
         **kwargs: Any
-    ):
+    ) -> None:
         """
         Args:
             num_classes: number of output classes (default 19)
             num_layers: number of layers in each side of U-net (default 5)
             features_start: number of features in first layer (default 64)
             bilinear: whether to use bilinear interpolation (True) or transposed convolutions (default) for upsampling.
             ignore_index: target value to be ignored in cross_entropy (default 250)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/models/vision/unet.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/models/vision/unet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch import Tensor, nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 
 class UNet(nn.Module):
     """Pytorch Lightning implementation of U-Net.
 
     Paper: `U-Net: Convolutional Networks for Biomedical Image Segmentation
     <https://arxiv.org/abs/1505.04597>`_
@@ -27,16 +27,15 @@
     def __init__(
         self,
         num_classes: int,
         input_channels: int = 3,
         num_layers: int = 5,
         features_start: int = 64,
         bilinear: bool = False,
-    ):
-
+    ) -> None:
         if num_layers < 1:
             raise ValueError(f"num_layers = {num_layers}, expected: num_layers > 0")
 
         super().__init__()
         self.num_layers = num_layers
 
         layers = [DoubleConv(input_channels, features_start)]
@@ -64,15 +63,15 @@
             xi[-1] = layer(xi[-1], xi[-2 - i])
         return self.layers[-1](xi[-1])
 
 
 class DoubleConv(nn.Module):
     """[ Conv2d => BatchNorm => ReLU ] x 2."""
 
-    def __init__(self, in_ch: int, out_ch: int):
+    def __init__(self, in_ch: int, out_ch: int) -> None:
         super().__init__()
         self.net = nn.Sequential(
             nn.Conv2d(in_ch, out_ch, kernel_size=3, padding=1, bias=False),
             nn.BatchNorm2d(out_ch),
             nn.ReLU(inplace=True),
             nn.Conv2d(out_ch, out_ch, kernel_size=3, padding=1, bias=False),
             nn.BatchNorm2d(out_ch),
@@ -82,27 +81,27 @@
     def forward(self, x: Tensor) -> Tensor:
         return self.net(x)
 
 
 class Down(nn.Module):
     """Downscale with MaxPool => DoubleConvolution block."""
 
-    def __init__(self, in_ch: int, out_ch: int):
+    def __init__(self, in_ch: int, out_ch: int) -> None:
         super().__init__()
         self.net = nn.Sequential(nn.MaxPool2d(kernel_size=2, stride=2), DoubleConv(in_ch, out_ch))
 
     def forward(self, x: Tensor) -> Tensor:
         return self.net(x)
 
 
 class Up(nn.Module):
     """Upsampling (by either bilinear interpolation or transpose convolutions) followed by concatenation of feature
     map from contracting path, followed by DoubleConv."""
 
-    def __init__(self, in_ch: int, out_ch: int, bilinear: bool = False):
+    def __init__(self, in_ch: int, out_ch: int, bilinear: bool = False) -> None:
         super().__init__()
         self.upsample = None
         if bilinear:
             self.upsample = nn.Sequential(
                 nn.Upsample(scale_factor=2, mode="bilinear", align_corners=True),
                 nn.Conv2d(in_ch, in_ch // 2, kernel_size=1),
             )
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/optimizers/lars.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/optimizers/lars.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,31 +64,31 @@
         lr=required,
         momentum=0,
         dampening=0,
         weight_decay=0,
         nesterov=False,
         trust_coefficient=0.001,
         eps=1e-8,
-    ):
+    ) -> None:
         if lr is not required and lr < 0.0:
             raise ValueError(f"Invalid learning rate: {lr}")
         if momentum < 0.0:
             raise ValueError(f"Invalid momentum value: {momentum}")
         if weight_decay < 0.0:
             raise ValueError(f"Invalid weight_decay value: {weight_decay}")
 
-        defaults = dict(
-            lr=lr,
-            momentum=momentum,
-            dampening=dampening,
-            weight_decay=weight_decay,
-            nesterov=nesterov,
-            trust_coefficient=trust_coefficient,
-            eps=eps,
-        )
+        defaults = {
+            "lr": lr,
+            "momentum": momentum,
+            "dampening": dampening,
+            "weight_decay": weight_decay,
+            "nesterov": nesterov,
+            "trust_coefficient": trust_coefficient,
+            "eps": eps,
+        }
         if nesterov and (momentum <= 0 or dampening != 0):
             raise ValueError("Nesterov momentum requires a momentum and zero dampening")
 
         super().__init__(params, defaults)
 
     def __setstate__(self, state):
         super().__setstate__(state)
@@ -121,31 +121,27 @@
                     continue
 
                 d_p = p.grad
                 p_norm = torch.norm(p.data)
                 g_norm = torch.norm(p.grad.data)
 
                 # lars scaling + weight decay part
-                if weight_decay != 0:
-                    if p_norm != 0 and g_norm != 0:
-                        lars_lr = p_norm / (g_norm + p_norm * weight_decay + group["eps"])
-                        lars_lr *= group["trust_coefficient"]
+                if weight_decay != 0 and p_norm != 0 and g_norm != 0:
+                    lars_lr = p_norm / (g_norm + p_norm * weight_decay + group["eps"])
+                    lars_lr *= group["trust_coefficient"]
 
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

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/optimizers/lr_scheduler.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/optimizers/lr_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import math
 import warnings
 from typing import List
 
-from torch import nn
-from torch.optim import Adam, Optimizer
+from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 
 from pl_bolts.utils.stability import under_review
 
 
 @under_review()
 class LinearWarmupCosineAnnealingLR(_LRScheduler):
@@ -23,24 +22,25 @@
         passing epoch to :func:`.step()` is being deprecated and comes with an EPOCH_DEPRECATION_WARNING.
         It calls the :func:`_get_closed_form_lr()` method for this scheduler instead of
         :func:`get_lr()`. Though this does not change the behavior of the scheduler, when passing
         epoch param to :func:`.step()`, the user should call the :func:`.step()` function before calling
         train and validation methods.
 
     Example:
+        >>> import torch.nn as nn
+        >>> from torch.optim import Adam
+        >>> #
         >>> layer = nn.Linear(10, 1)
         >>> optimizer = Adam(layer.parameters(), lr=0.02)
         >>> scheduler = LinearWarmupCosineAnnealingLR(optimizer, warmup_epochs=10, max_epochs=40)
-        >>> #
         >>> # the default case
         >>> for epoch in range(40):
         ...     # train(...)
         ...     # validate(...)
         ...     scheduler.step()
-        >>> #
         >>> # passing epoch param case
         >>> for epoch in range(40):
         ...     scheduler.step(epoch)
         ...     # train(...)
         ...     # validate(...)
     """
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/transforms/dataset_normalizations.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/dataset_normalizations.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,39 +11,36 @@
 
 def imagenet_normalization() -> Callable:
     if not _TORCHVISION_AVAILABLE:  # pragma: no cover
         raise ModuleNotFoundError(
             "You want to use `torchvision` which is not installed yet, install it with `pip install torchvision`."
         )
 
-    normalize = transforms.Normalize(mean=(0.485, 0.456, 0.406), std=(0.229, 0.224, 0.225))
-    return normalize
+    return transforms.Normalize(mean=(0.485, 0.456, 0.406), std=(0.229, 0.224, 0.225))
 
 
 def cifar10_normalization() -> Callable:
     if not _TORCHVISION_AVAILABLE:  # pragma: no cover
         raise ModuleNotFoundError(
             "You want to use `torchvision` which is not installed yet, install it with `pip install torchvision`."
         )
 
-    normalize = transforms.Normalize(
+    return transforms.Normalize(
         mean=[x / 255.0 for x in [125.3, 123.0, 113.9]],
         std=[x / 255.0 for x in [63.0, 62.1, 66.7]],
     )
-    return normalize
 
 
 def stl10_normalization() -> Callable:
     if not _TORCHVISION_AVAILABLE:  # pragma: no cover
         raise ModuleNotFoundError(
             "You want to use `torchvision` which is not installed yet, install it with `pip install torchvision`."
         )
 
-    normalize = transforms.Normalize(mean=(0.43, 0.42, 0.39), std=(0.27, 0.26, 0.27))
-    return normalize
+    return transforms.Normalize(mean=(0.43, 0.42, 0.39), std=(0.27, 0.26, 0.27))
 
 
 def emnist_normalization(split: str) -> Callable:
     if not _TORCHVISION_AVAILABLE:  # pragma: no cover
         raise ModuleNotFoundError(
             "You want to use `torchvision` which is not installed yet, install it with `pip install torchvision`."
         )
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/transforms/self_supervised/ssl_transforms.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/transforms/self_supervised/ssl_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 
 from pl_bolts.utils import _PIL_AVAILABLE
 from pl_bolts.utils.stability import under_review
 from pl_bolts.utils.warnings import warn_missing_pkg
 
 if _PIL_AVAILABLE:
     from PIL import Image
@@ -15,15 +15,15 @@
 class RandomTranslateWithReflect:
     """Translate image randomly Translate vertically and horizontally by n pixels where n is integer drawn
     uniformly independently for each axis from [-max_translation, max_translation].
 
     Fill the uncovered blank area with reflect padding.
     """
 
-    def __init__(self, max_translation):
+    def __init__(self, max_translation) -> None:
         if not _PIL_AVAILABLE:  # pragma: no cover
             raise ModuleNotFoundError("You want to use `Pillow` which is not installed yet.")
 
         self.max_translation = max_translation
 
     def __call__(self, old_image):
         xtranslation, ytranslation = np.random.randint(-self.max_translation, self.max_translation + 1, size=2)
@@ -53,27 +53,27 @@
             (xpad - xtranslation, ypad - ytranslation, xpad + xsize - xtranslation, ypad + ysize - ytranslation)
         )
         return new_image
 
 
 @under_review()
 class Patchify:
-    def __init__(self, patch_size, overlap_size):
+    def __init__(self, patch_size, overlap_size) -> None:
         self.patch_size = patch_size
         self.overlap_size = self.patch_size - overlap_size
 
     def __call__(self, x):
         x = x.unsqueeze(0)
         b, c, h, w = x.size()
 
         # patch up the images
         # (b, c, h, w) -> (b, c*patch_size, L)
         x = F.unfold(x, kernel_size=self.patch_size, stride=self.overlap_size)
 
-        # (b, c*patch_size, L) -> (b, nb_patches, width, height)
+        # (b, c*patch_size, L) -> (b, num_patches, width, height)
         x = x.transpose(2, 1).contiguous().view(b, -1, self.patch_size, self.patch_size)
 
         # reshape to have (b x patches, c, h, w)
         x = x.view(-1, c, self.patch_size, self.patch_size)
 
         x = x.squeeze(0)
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/utils/__init__.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import operator
+import platform
 
 import torch
 from lightning_utilities.core.imports import compare_version, module_available
 
 from pl_bolts.callbacks.verification.batch_gradient import BatchGradientVerification  # type: ignore
 
 _NATIVE_AMP_AVAILABLE: bool = module_available("torch.cuda.amp") and hasattr(torch.cuda.amp, "autocast")
-
+_IS_WINDOWS = platform.system() == "Windows"
+_TORCH_ORT_AVAILABLE = module_available("torch_ort")
+_TORCH_MAX_VERSION_SPARSEML = compare_version("torch", operator.lt, "1.11.0")
+_TORCH_MESHGRID_REQUIRES_INDEXING = compare_version("torch", operator.ge, "1.10.0")
 _TORCHVISION_AVAILABLE: bool = module_available("torchvision")
+_TORCHVISION_LESS_THAN_0_9_1: bool = compare_version("torchvision", operator.lt, "0.9.1")
+_TORCHVISION_LESS_THAN_0_13: bool = compare_version("torchvision", operator.le, "0.13.0")
+_TORCHMETRICS_DETECTION_AVAILABLE: bool = module_available("torchmetrics.detection")
+_PL_GREATER_EQUAL_1_4 = compare_version("pytorch_lightning", operator.ge, "1.4.0")
+_PL_GREATER_EQUAL_1_4_5 = compare_version("pytorch_lightning", operator.ge, "1.4.5")
 _GYM_AVAILABLE: bool = module_available("gym")
+_GYM_GREATER_EQUAL_0_20 = compare_version("gym", operator.ge, "0.20.0")
 _SKLEARN_AVAILABLE: bool = module_available("sklearn")
 _PIL_AVAILABLE: bool = module_available("PIL")
 _OPENCV_AVAILABLE: bool = module_available("cv2")
 _WANDB_AVAILABLE: bool = module_available("wandb")
 _MATPLOTLIB_AVAILABLE: bool = module_available("matplotlib")
-_TORCHVISION_LESS_THAN_0_9_1: bool = compare_version("torchvision", operator.lt, "0.9.1")
-_TORCHVISION_LESS_THAN_0_13: bool = compare_version("torchvision", operator.le, "0.13.0")
-_PL_GREATER_EQUAL_1_4 = compare_version("pytorch_lightning", operator.ge, "1.4.0")
-_PL_GREATER_EQUAL_1_4_5 = compare_version("pytorch_lightning", operator.ge, "1.4.5")
-_TORCH_ORT_AVAILABLE = module_available("torch_ort")
-_TORCH_MAX_VERSION_SPARSEML = compare_version("torch", operator.lt, "1.11.0")
 _SPARSEML_AVAILABLE = module_available("sparseml") and _PL_GREATER_EQUAL_1_4_5 and _TORCH_MAX_VERSION_SPARSEML
 _JSONARGPARSE_GREATER_THAN_4_16_0 = compare_version("jsonargparse", operator.gt, "4.16.0")
 
 
 __all__ = ["BatchGradientVerification"]
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/utils/arguments.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/utils/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def add_object_args(self, name: str, obj: Any) -> None:
         default_args = gather_lit_args(obj)
         self._default_obj_args[name] = default_args
         for arg in default_args:
             if arg.name in self._added_arg_names:
                 continue
             self._added_arg_names.append(arg.name)
-            kwargs = dict(type=arg.types[0])
+            kwargs = {"type": arg.types[0]}
             if arg.required and not self.ignore_required_init_args:
                 kwargs["required"] = True
             else:
                 kwargs["default"] = arg.default
             self.add_argument(f"--{arg.name}", **kwargs)
 
     def parse_lit_args(self, *args: Any, **kwargs: Any) -> Namespace:
@@ -86,22 +86,19 @@
         else:
             root_cls = cls
 
     blacklisted_args = ["self", "args", "kwargs"]
     arguments: List[LitArg] = []
     argument_names = []
     for obj in inspect.getmro(cls):
-
         if obj is root_cls and len(arguments) > 0:
             break
 
         if issubclass(obj, root_cls):
-
             default_params = inspect.signature(obj.__init__).parameters  # type: ignore
-
             for arg in default_params:
                 arg_type = default_params[arg].annotation
                 arg_default = default_params[arg].default
 
                 try:
                     arg_types = tuple(arg_type.__args__)
                 except AttributeError:
@@ -120,15 +117,15 @@
                 arg_is_positional = arg_default == inspect.Parameter.empty and not arg_is_missing_type_hint
                 # Kwargs have both a default + known type or types
                 arg_is_kwarg = arg_default != inspect.Parameter.empty and not arg_is_missing_type_hint
 
                 if do_skip_this_arg:
                     continue
 
-                elif arg_is_positional or arg_is_kwarg:
+                if arg_is_positional or arg_is_kwarg:
                     lit_arg = LitArg(
                         name=arg,
                         types=arg_types,
                         default=arg_default if arg_default != inspect.Parameter.empty else None,
                         required=arg_is_positional,
                         context=obj.__name__,
                     )
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/utils/pretrained_weights.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/utils/pretrained_weights.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/utils/self_supervised.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/utils/self_supervised.py`

 * *Files identical despite different names*

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/utils/semi_supervised.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/utils/semi_supervised.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,106 +32,100 @@
 
     def forward(self, x: Tensor) -> Tensor:
         return x
 
 
 @under_review()
 def balance_classes(
-    X: Union[Tensor, np.ndarray], Y: Union[Tensor, np.ndarray, Sequence[int]], batch_size: int
+    X: Union[Tensor, np.ndarray], y: Union[Tensor, np.ndarray, Sequence[int]], batch_size: int  # noqa: N803
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Makes sure each batch has an equal amount of data from each class. Perfect balance.
 
     Args:
         X: input features
-        Y: mixed labels (ints)
+        y: mixed labels (ints)
         batch_size: the ultimate batch size
     """
     if not _SKLEARN_AVAILABLE:  # pragma: no cover
         raise ModuleNotFoundError("You want to use `shuffle` function from `scikit-learn` which is not installed yet.")
 
-    nb_classes = len(set(Y))
-
-    nb_batches = math.ceil(len(Y) / batch_size)
-
+    num_classes = len(set(y))
+    num_batches = math.ceil(len(y) / batch_size)
     # sort by classes
-    final_batches_x: List[list] = [[] for i in range(nb_batches)]
-    final_batches_y: List[list] = [[] for i in range(nb_batches)]
+    final_batches_x: List[list] = [[] for i in range(num_batches)]
+    final_batches_y: List[list] = [[] for i in range(num_batches)]
 
     # Y needs to be np arr
-    Y = np.asarray(Y)
+    y = np.asarray(y)
 
     # pick chunk size for each class using the largest split
     chunk_sizes = []
-    for class_i in range(nb_classes):
-        mask = Y == class_i
-        y = Y[mask]
-        chunk_sizes.append(math.ceil(len(y) / nb_batches))
+    for class_i in range(num_classes):
+        mask = class_i == y
+        y_sub = y[mask]
+        chunk_sizes.append(math.ceil(len(y_sub) / num_batches))
     chunk_size = max(chunk_sizes)
     # force chunk size to be even
     if chunk_size % 2 != 0:
         chunk_size -= 1
 
     # divide each class into each batch
-    for class_i in range(nb_classes):
-        mask = Y == class_i
-        x = X[mask]
-        y = Y[mask]
+    for class_i in range(num_classes):
+        mask = class_i == y
+        x_sub = X[mask]
+        y_sub = y[mask]
 
         # shuffle items in the class
-        x, y = sk_shuffle(x, y, random_state=123)
+        x_sub, y_sub = sk_shuffle(x_sub, y_sub, random_state=123)
 
         # divide the class into the batches
-        for i_start in range(0, len(y), chunk_size):
+        for i_start in range(0, len(y_sub), chunk_size):
             batch_i = i_start // chunk_size
             i_end = i_start + chunk_size
 
             if len(final_batches_x) > batch_i:
-                final_batches_x[batch_i].append(x[i_start:i_end])
-                final_batches_y[batch_i].append(y[i_start:i_end])
+                final_batches_x[batch_i].append(x_sub[i_start:i_end])
+                final_batches_y[batch_i].append(y_sub[i_start:i_end])
 
     # merge into full dataset
-    final_batches_x = [np.concatenate(x, axis=0) for x in final_batches_x if len(x) > 0]
-    final_batches_x = np.concatenate(final_batches_x, axis=0)
-
-    final_batches_y = [np.concatenate(x, axis=0) for x in final_batches_y if len(x) > 0]
-    final_batches_y = np.concatenate(final_batches_y, axis=0)
-
+    final_batches_x = np.concatenate([np.concatenate(x, axis=0) for x in final_batches_x if len(x) > 0], axis=0)
+    final_batches_y = np.concatenate([np.concatenate(x, axis=0) for x in final_batches_y if len(x) > 0], axis=0)
     return final_batches_x, final_batches_y
 
 
 @under_review()
 def generate_half_labeled_batches(
-    smaller_set_X: np.ndarray,
-    smaller_set_Y: np.ndarray,
-    larger_set_X: np.ndarray,
-    larger_set_Y: np.ndarray,
+    smaller_set_x: np.ndarray,
+    smaller_set_y: np.ndarray,
+    larger_set_x: np.ndarray,
+    larger_set_y: np.ndarray,
     batch_size: int,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Given a labeled dataset and an unlabeled dataset, this function generates a joint pair where half the
     batches are labeled and the other half is not."""
-    X = []
-    Y = []
+    x = []
+    y = []
     half_batch = batch_size // 2
 
-    n_larger = len(larger_set_X)
-    n_smaller = len(smaller_set_X)
+    n_larger = len(larger_set_x)
+    n_smaller = len(smaller_set_x)
     for i_start in range(0, n_larger, half_batch):
         i_end = i_start + half_batch
 
-        X_larger = larger_set_X[i_start:i_end]
-        Y_larger = larger_set_Y[i_start:i_end]
+        x_larger = larger_set_x[i_start:i_end]
+        y_larger = larger_set_y[i_start:i_end]
 
         # pull out labeled part
         smaller_start = i_start % (n_smaller - half_batch)
         smaller_end = smaller_start + half_batch
 
-        X_small = smaller_set_X[smaller_start:smaller_end]
-        Y_small = smaller_set_Y[smaller_start:smaller_end]
+        x_small = smaller_set_x[smaller_start:smaller_end]
+        y_small = smaller_set_y[smaller_start:smaller_end]
 
-        X.extend([X_larger, X_small])
-        Y.extend([Y_larger, Y_small])
+        x.extend([x_larger, x_small])
+        y.extend([y_larger, y_small])
 
     # aggregate reshuffled at end of shuffling
-    X = np.concatenate(X, axis=0)
-    Y = np.concatenate(Y, axis=0)
+    x = np.concatenate(x, axis=0)
+    y = np.concatenate(y, axis=0)
 
-    return X, Y
+    return x, y
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/utils/stability.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/utils/stability.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 
 
 def _raise_review_warning(message: str, stacklevel: int = 6) -> None:
     rank_zero_warn(_create_full_message(message), stacklevel=stacklevel, category=UnderReviewWarning)
 
 
 def under_review():
-    """The under_review decorator is used to indicate that a particular feature is not properly reviewed and tested yet.
+    """The under_review decorator is used to indicate that a particular feature is not properly reviewed and tested
+    yet.
+
     A callable or type that has been marked as under_review will give a ``UnderReviewWarning`` when it is called or
     instantiated. This designation should be used following the description given in :ref:`stability`.
     Args:
         message: The message to include in the warning.
     Examples
     ________
     >>> from pytest import warns
```

### Comparing `lightning-bolts-0.6.0.post1/pl_bolts/utils/warnings.py` & `lightning-bolts-0.7.0rc0/src/pl_bolts/utils/warnings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import os
 import warnings
 from typing import Callable, Dict, Optional
 
-from pl_bolts.utils.stability import under_review
-
 MISSING_PACKAGE_WARNINGS: Dict[str, int] = {}
 
 WARN_MISSING_PACKAGE = int(os.environ.get("WARN_MISSING_PACKAGE", False))
 
 
-@under_review()
 def warn_missing_pkg(
     pkg_name: str,
     pypi_name: Optional[str] = None,
     extra_text: Optional[str] = None,
     stdout_func: Callable = warnings.warn,
 ) -> int:
     """Template for warning on missing packages, show them just once.
```

### Comparing `lightning-bolts-0.6.0.post1/setup.py` & `lightning-bolts-0.7.0rc0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,90 @@
 #!/usr/bin/env python
 
 import os
 import re
 from importlib.util import module_from_spec, spec_from_file_location
-from typing import List
 
 from setuptools import find_packages, setup
 
 _PATH_ROOT = os.path.realpath(os.path.dirname(__file__))
 _PATH_REQUIRE = os.path.join(_PATH_ROOT, "requirements")
+_FREEZE_REQUIREMENTS = bool(int(os.environ.get("FREEZE_REQUIREMENTS", 0)))
 
 
 def _load_py_module(fname, pkg="pl_bolts"):
-    spec = spec_from_file_location(os.path.join(pkg, fname), os.path.join(_PATH_ROOT, pkg, fname))
+    spec = spec_from_file_location(os.path.join(pkg, fname), os.path.join(_PATH_ROOT, "src", pkg, fname))
     py = module_from_spec(spec)
     spec.loader.exec_module(py)
     return py
 
 
-def _load_requirements(path_dir: str, file_name: str = "requirements.txt", comment_char: str = "#") -> List[str]:
-    """Load requirements from a file.
+def _augment_requirement(ln: str, comment_char: str = "#", unfreeze: bool = True) -> str:
+    """Adjust the upper version contrains.
 
-    >>> _load_requirements(_PATH_ROOT)  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-    ['pytorch-lightning...']
+    >>> _augment_requirement("arrow<=1.2.2,>=1.2.0  # anything", unfreeze=False)
+    'arrow<=1.2.2,>=1.2.0'
+    >>> _augment_requirement("arrow<=1.2.2,>=1.2.0  # strict", unfreeze=False)
+    'arrow<=1.2.2,>=1.2.0  # strict'
+    >>> _augment_requirement("arrow<=1.2.2,>=1.2.0  # my name", unfreeze=True)
+    'arrow>=1.2.0'
+    >>> _augment_requirement("arrow>=1.2.0, <=1.2.2  # strict", unfreeze=True)
+    'arrow>=1.2.0, <=1.2.2  # strict'
+    >>> _augment_requirement("arrow", unfreeze=True)
+    'arrow'
+    """
+    # filer all comments
+    if comment_char in ln:
+        comment = ln[ln.index(comment_char) :]
+        ln = ln[: ln.index(comment_char)]
+        is_strict = "strict" in comment
+    else:
+        is_strict = False
+    req = ln.strip()
+    # skip directly installed dependencies
+    if not req or (unfreeze and any(c in req for c in ["http:", "https:", "@"])):
+        return ""
+
+    # remove version restrictions unless they are strict
+    if unfreeze and "<" in req and not is_strict:
+        req = re.sub(r",? *<=? *[\d\.\*]+,? *", "", req).strip()
+
+    # adding strict back to the comment
+    if is_strict:
+        req += "  # strict"
+
+    return req
+
+
+def _load_requirements(path_dir: str, file_name: str, unfreeze: bool = not _FREEZE_REQUIREMENTS) -> list:
+    """Loading requirements from a file.
+
+    >>> path_req = os.path.join(_PATH_ROOT, "requirements")
+    >>> _load_requirements(path_req, "docs.txt")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
+    ['sphinx>=4.0', ...]
     """
     with open(os.path.join(path_dir, file_name)) as file:
         lines = [ln.strip() for ln in file.readlines()]
-    reqs = []
-    for ln in lines:
-        # filer all comments
-        if comment_char in ln:
-            ln = ln[: ln.index(comment_char)].strip()
-        # skip directly installed dependencies
-        if ln.startswith("http"):
-            continue
-        if ln:  # if requirement is not empty
-            reqs.append(ln)
+    reqs = [_augment_requirement(ln, unfreeze=unfreeze) for ln in lines]
+    reqs = [str(req) for req in reqs if req and not req.startswith("-r")]
+    if unfreeze:
+        # filter empty lines and containing @ which means redirect to some git/http
+        reqs = [req for req in reqs if not any(c in req for c in ["@", "http://", "https://"])]
     return reqs
 
 
 def _load_readme_description(path_dir: str, homepage: str, ver: str) -> str:
     """Load readme as decribtion.
 
     >>> _load_readme_description(_PATH_ROOT, "", "")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
     '<div align="center">...'
     """
     path_readme = os.path.join(path_dir, "README.md")
-    text = open(path_readme, encoding="utf-8").read()
+    with open(path_readme, encoding="utf-8") as fo:
+        text = fo.read()
 
     # drop images from readme
     text = text.replace("![PT to PL](docs/source/_images/general/pl_quick_start_full_compressed.gif)", "")
 
     # https://github.com/PyTorchLightning/pytorch-lightning/raw/master/docs/source/_images/lightning_module/pt_to_png
     github_source_url = os.path.join(homepage, "raw", ver)
     # replace relative repository path to absolute link to the release
@@ -78,14 +112,15 @@
 
 
 def _prepare_extras():
     extras = {
         "loggers": _load_requirements(path_dir=_PATH_REQUIRE, file_name="loggers.txt"),
         "models": _load_requirements(path_dir=_PATH_REQUIRE, file_name="models.txt"),
         "test": _load_requirements(path_dir=_PATH_REQUIRE, file_name="test.txt"),
+        "typing": _load_requirements(path_dir=_PATH_REQUIRE, file_name="typing.txt"),
     }
     extras["extra"] = extras["models"] + extras["loggers"]
     extras["dev"] = extras["extra"] + extras["test"]
     return extras
 
 
 about = _load_py_module("__about__.py")
@@ -105,23 +140,24 @@
     version=about.__version__,
     description=about.__docs__,
     author=about.__author__,
     author_email=about.__author_email__,
     url=about.__homepage__,
     download_url="https://github.com/PyTorchLightning/lightning-bolts",
     license=about.__license__,
-    packages=find_packages(exclude=["tests", "docs"]),
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     zip_safe=False,
     keywords=["deep learning", "pytorch", "AI"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     setup_requires=["wheel"],
-    install_requires=_load_requirements(_PATH_ROOT),
+    install_requires=_load_requirements(_PATH_REQUIRE, "base.txt"),
     extras_require=_prepare_extras(),
     project_urls={
         "Bug Tracker": "https://github.com/PyTorchLightning/lightning-bolts/issues",
         "Documentation": "https://lightning-bolts.rtfd.io/en/latest/",
         "Source Code": "https://github.com/PyTorchLightning/lightning-bolts",
     },
     classifiers=[
@@ -137,12 +173,12 @@
         "Topic :: Scientific/Engineering :: Information Analysis",
         # Pick your license as you wish
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 )
```

