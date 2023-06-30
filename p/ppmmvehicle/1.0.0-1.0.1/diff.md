# Comparing `tmp/ppmmvehicle-1.0.0.tar.gz` & `tmp/ppmmvehicle-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppmmvehicle-1.0.0.tar", last modified: Fri Jun 30 02:27:42 2023, max compression
+gzip compressed data, was "ppmmvehicle-1.0.1.tar", last modified: Fri Jun 30 03:32:35 2023, max compression
```

## Comparing `ppmmvehicle-1.0.0.tar` & `ppmmvehicle-1.0.1.tar`

### file list

```diff
@@ -1,199 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 02:05:26.136921 ppmmvehicle-1.0.0/
--rw-rw-rw-   0        0        0     5624 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    34523 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      213 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    28644 2023-06-30 02:27:42.563912 ppmmvehicle-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    24548 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/README.md
--rw-rw-rw-   0        0        0    23524 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/README.zh-CN.md
-drwxrwxrwx   0        0        0        0 2023-06-30 02:27:42.533913 ppmmvehicle-1.0.0/ppmmvehicle.egg-info/
--rw-rw-rw-   0        0        0    28644 2023-06-30 02:27:42.000000 ppmmvehicle-1.0.0/ppmmvehicle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5620 2023-06-30 02:27:42.000000 ppmmvehicle-1.0.0/ppmmvehicle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 02:27:42.000000 ppmmvehicle-1.0.0/ppmmvehicle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-30 02:27:42.000000 ppmmvehicle-1.0.0/ppmmvehicle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      369 2023-06-30 02:27:42.000000 ppmmvehicle-1.0.0/ppmmvehicle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 02:27:42.000000 ppmmvehicle-1.0.0/ppmmvehicle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1129 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0      723 2023-06-30 02:27:42.564912 ppmmvehicle-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3137 2023-06-30 02:05:17.000000 ppmmvehicle-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.460448 ppmmvehicle-1.0.0/ultralytics/
--rw-rw-rw-   0        0        0      451 2023-06-30 01:47:25.000000 ppmmvehicle-1.0.0/ultralytics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.462453 ppmmvehicle-1.0.0/ultralytics/assets/
--rw-rw-rw-   0        0        0   137419 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/assets/bus.jpg
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.481448 ppmmvehicle-1.0.0/ultralytics/datasets/
--rw-rw-rw-   0        0        0     2751 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/Argoverse.yaml
--rw-rw-rw-   0        0        0     1986 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/GlobalWheat2020.yaml
--rw-rw-rw-   0        0        0    42439 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/datasets/ImageNet.yaml
--rw-rw-rw-   0        0        0     9270 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/Objects365.yaml
--rw-rw-rw-   0        0        0     2437 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/SKU-110K.yaml
--rw-rw-rw-   0        0        0     3512 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/VOC.yaml
--rw-rw-rw-   0        0        0     3012 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/VisDrone.yaml
--rw-rw-rw-   0        0        0     1547 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/coco-pose.yaml
--rw-rw-rw-   0        0        0     2526 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/coco.yaml
--rw-rw-rw-   0        0        0     1862 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/datasets/coco128-seg.yaml
--rw-rw-rw-   0        0        0     1846 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/datasets/coco128.yaml
--rw-rw-rw-   0        0        0      895 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/datasets/coco8-pose.yaml
--rw-rw-rw-   0        0        0     1797 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/datasets/coco8-seg.yaml
--rw-rw-rw-   0        0        0     1777 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/datasets/coco8.yaml
--rw-rw-rw-   0        0        0     5178 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/datasets/xView.yaml
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.487448 ppmmvehicle-1.0.0/ultralytics/hub/
--rw-rw-rw-   0        0        0     4225 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/hub/__init__.py
--rw-rw-rw-   0        0        0     5209 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/hub/auth.py
--rw-rw-rw-   0        0        0     8479 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/hub/session.py
--rw-rw-rw-   0        0        0     9157 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/hub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.427451 ppmmvehicle-1.0.0/ultralytics/models/
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.489449 ppmmvehicle-1.0.0/ultralytics/models/rt-detr/
--rw-rw-rw-   0        0        0     1970 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/rt-detr/rt-detr-l.yaml
--rw-rw-rw-   0        0        0     2177 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/rt-detr/rt-detr-x.yaml
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.494449 ppmmvehicle-1.0.0/ultralytics/models/v3/
--rw-rw-rw-   0        0        0     1550 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v3/yolov3-spp.yaml
--rw-rw-rw-   0        0        0     1252 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v3/yolov3-tiny.yaml
--rw-rw-rw-   0        0        0     1537 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v3/yolov3.yaml
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.496448 ppmmvehicle-1.0.0/ultralytics/models/v5/
--rw-rw-rw-   0        0        0     1923 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v5/yolov5-p6.yaml
--rw-rw-rw-   0        0        0     1550 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v5/yolov5.yaml
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.498448 ppmmvehicle-1.0.0/ultralytics/models/v6/
--rw-rw-rw-   0        0        0     1680 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v6/yolov6.yaml
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.508449 ppmmvehicle-1.0.0/ultralytics/models/v8/
--rw-rw-rw-   0        0        0      920 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-cls.yaml
--rw-rw-rw-   0        0        0     1751 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-p2.yaml
--rw-rw-rw-   0        0        0     1856 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-p6.yaml
--rw-rw-rw-   0        0        0     1946 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-rw-rw-   0        0        0     1580 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-pose.yaml
--rw-rw-rw-   0        0        0     1490 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-seg.yaml
--rw-rw-rw-   0        0        0     1913 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8.yaml
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.517450 ppmmvehicle-1.0.0/ultralytics/nn/
--rw-rw-rw-   0        0        0      555 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/nn/__init__.py
--rw-rw-rw-   0        0        0    24254 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/nn/autobackend.py
--rw-rw-rw-   0        0        0    12509 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/nn/autoshape.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.531449 ppmmvehicle-1.0.0/ultralytics/nn/modules/
--rw-rw-rw-   0        0        0     1587 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/nn/modules/__init__.py
--rw-rw-rw-   0        0        0    11816 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/nn/modules/block.py
--rw-rw-rw-   0        0        0    11647 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/nn/modules/conv.py
--rw-rw-rw-   0        0        0    17098 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/nn/modules/head.py
--rw-rw-rw-   0        0        0    16396 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/nn/modules/transformer.py
--rw-rw-rw-   0        0        0     3244 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/nn/modules/utils.py
--rw-rw-rw-   0        0        0    33967 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/nn/tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.537448 ppmmvehicle-1.0.0/ultralytics/tracker/
--rw-rw-rw-   0        0        0      202 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.540450 ppmmvehicle-1.0.0/ultralytics/tracker/cfg/
--rw-rw-rw-   0        0        0      890 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/cfg/botsort.yaml
--rw-rw-rw-   0        0        0      694 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/cfg/bytetrack.yaml
--rw-rw-rw-   0        0        0     2309 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/tracker/track.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.545448 ppmmvehicle-1.0.0/ultralytics/tracker/trackers/
--rw-rw-rw-   0        0        0      171 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/trackers/__init__.py
--rw-rw-rw-   0        0        0     1609 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/trackers/basetrack.py
--rw-rw-rw-   0        0        0     5684 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/trackers/bot_sort.py
--rw-rw-rw-   0        0        0    14448 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/trackers/byte_tracker.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.550448 ppmmvehicle-1.0.0/ultralytics/tracker/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/utils/__init__.py
--rw-rw-rw-   0        0        0    12214 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/tracker/utils/gmc.py
--rw-rw-rw-   0        0        0    18420 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/tracker/utils/kalman_filter.py
--rw-rw-rw-   0        0        0     8699 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/tracker/utils/matching.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.551448 ppmmvehicle-1.0.0/ultralytics/vit/
--rw-rw-rw-   0        0        0      149 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.562450 ppmmvehicle-1.0.0/ultralytics/vit/rtdetr/
--rw-rw-rw-   0        0        0      197 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/rtdetr/__init__.py
--rw-rw-rw-   0        0        0     5077 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/vit/rtdetr/model.py
--rw-rw-rw-   0        0        0     1902 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/vit/rtdetr/predict.py
--rw-rw-rw-   0        0        0     4790 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/vit/rtdetr/val.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.580448 ppmmvehicle-1.0.0/ultralytics/vit/sam/
--rw-rw-rw-   0        0        0      130 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/__init__.py
--rw-rw-rw-   0        0        0    13304 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/amg.py
--rw-rw-rw-   0        0        0     3878 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/autosize.py
--rw-rw-rw-   0        0        0     3781 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/build.py
--rw-rw-rw-   0        0        0     2274 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/model.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.589448 ppmmvehicle-1.0.0/ultralytics/vit/sam/modules/
--rw-rw-rw-   0        0        0        0 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/modules/__init__.py
--rw-rw-rw-   0        0        0     6351 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/modules/decoders.py
--rw-rw-rw-   0        0        0    22502 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/modules/encoders.py
--rw-rw-rw-   0        0        0    15250 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/modules/mask_generator.py
--rw-rw-rw-   0        0        0    11201 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-rw-rw-   0        0        0     7116 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/modules/sam.py
--rw-rw-rw-   0        0        0     8489 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/modules/transformer.py
--rw-rw-rw-   0        0        0     2139 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/vit/sam/predict.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.590448 ppmmvehicle-1.0.0/ultralytics/yolo/
--rw-rw-rw-   0        0        0       94 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.594448 ppmmvehicle-1.0.0/ultralytics/yolo/cfg/
--rw-rw-rw-   0        0        0    18051 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/yolo/cfg/__init__.py
--rw-rw-rw-   0        0        0     6356 2023-06-19 03:05:30.000000 ppmmvehicle-1.0.0/ultralytics/yolo/cfg/backup.yaml
--rw-rw-rw-   0        0        0     6365 2023-06-29 08:40:29.000000 ppmmvehicle-1.0.0/ultralytics/yolo/cfg/default.yaml
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.605448 ppmmvehicle-1.0.0/ultralytics/yolo/data/
--rw-rw-rw-   0        0        0     1068 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/__init__.py
--rw-rw-rw-   0        0        0     2339 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/annotator.py
--rw-rw-rw-   0        0        0    40327 2023-06-28 08:32:04.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/augment.py
--rw-rw-rw-   0        0        0    13410 2023-06-26 08:12:33.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/base.py
--rw-rw-rw-   0        0        0     6575 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/build.py
--rw-rw-rw-   0        0        0     9190 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/converter.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.609448 ppmmvehicle-1.0.0/ultralytics/yolo/data/dataloaders/
--rw-rw-rw-   0        0        0        0 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/dataloaders/__init__.py
--rw-rw-rw-   0        0        0    14905 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-rw-rw-   0        0        0    17646 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-rw-rw-   0        0        0    51260 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-rw-rw-   0        0        0    13372 2023-06-26 07:54:38.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/dataset.py
--rw-rw-rw-   0        0        0     1776 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/dataset_wrappers.py
--rw-rw-rw-   0        0        0    25030 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.618448 ppmmvehicle-1.0.0/ultralytics/yolo/engine/
--rw-rw-rw-   0        0        0        0 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/engine/__init__.py
--rw-rw-rw-   0        0        0    40964 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/engine/exporter.py
--rw-rw-rw-   0        0        0    22144 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/engine/model.py
--rw-rw-rw-   0        0        0    16204 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/engine/predictor.py
--rw-rw-rw-   0        0        0    24287 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/engine/results.py
--rw-rw-rw-   0        0        0    31199 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/engine/trainer.py
--rw-rw-rw-   0        0        0    11715 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/engine/validator.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.623450 ppmmvehicle-1.0.0/ultralytics/yolo/nas/
--rw-rw-rw-   0        0        0      179 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/nas/__init__.py
--rw-rw-rw-   0        0        0     4977 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/nas/model.py
--rw-rw-rw-   0        0        0     1465 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/nas/predict.py
--rw-rw-rw-   0        0        0      953 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/nas/val.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.648449 ppmmvehicle-1.0.0/ultralytics/yolo/utils/
--rw-rw-rw-   0        0        0    27955 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/__init__.py
--rw-rw-rw-   0        0        0     3846 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/autobatch.py
--rw-rw-rw-   0        0        0    15888 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/benchmarks.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.661450 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/
--rw-rw-rw-   0        0        0      214 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/__init__.py
--rw-rw-rw-   0        0        0     5593 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/base.py
--rw-rw-rw-   0        0        0     5902 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/clearml.py
--rw-rw-rw-   0        0        0    12978 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/comet.py
--rw-rw-rw-   0        0        0     4301 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/dvc.py
--rw-rw-rw-   0        0        0     3310 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/hub.py
--rw-rw-rw-   0        0        0     2493 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-rw-rw-   0        0        0     3679 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/neptune.py
--rw-rw-rw-   0        0        0      495 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/raytune.py
--rw-rw-rw-   0        0        0     1525 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-rw-rw-   0        0        0     2170 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/callbacks/wb.py
--rw-rw-rw-   0        0        0    17568 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/checks.py
--rw-rw-rw-   0        0        0     2596 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/dist.py
--rw-rw-rw-   0        0        0    12114 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/downloads.py
--rw-rw-rw-   0        0        0      317 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/errors.py
--rw-rw-rw-   0        0        0     3588 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/files.py
--rw-rw-rw-   0        0        0    14634 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/instance.py
--rw-rw-rw-   0        0        0    18090 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/loss.py
--rw-rw-rw-   0        0        0    43799 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/metrics.py
--rw-rw-rw-   0        0        0    28273 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/ops.py
--rw-rw-rw-   0        0        0     1241 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/patches.py
--rw-rw-rw-   0        0        0    24523 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/plotting.py
--rw-rw-rw-   0        0        0    13645 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/tal.py
--rw-rw-rw-   0        0        0    22231 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/torch_utils.py
--rw-rw-rw-   0        0        0     2300 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/yolo/utils/tuner.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.663449 ppmmvehicle-1.0.0/ultralytics/yolo/v8/
--rw-rw-rw-   0        0        0      158 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.668450 ppmmvehicle-1.0.0/ultralytics/yolo/v8/classify/
--rw-rw-rw-   0        0        0      391 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/classify/__init__.py
--rw-rw-rw-   0        0        0     1929 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/classify/predict.py
--rw-rw-rw-   0        0        0     6927 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/classify/train.py
--rw-rw-rw-   0        0        0     4676 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/classify/val.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.673449 ppmmvehicle-1.0.0/ultralytics/yolo/v8/detect/
--rw-rw-rw-   0        0        0      277 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/detect/__init__.py
--rw-rw-rw-   0        0        0     1854 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/detect/predict.py
--rw-rw-rw-   0        0        0     7199 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/detect/train.py
--rw-rw-rw-   0        0        0    14730 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/detect/val.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.679451 ppmmvehicle-1.0.0/ultralytics/yolo/v8/pose/
--rw-rw-rw-   0        0        0      247 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/pose/__init__.py
--rw-rw-rw-   0        0        0     2375 2023-06-27 09:07:15.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/pose/predict.py
--rw-rw-rw-   0        0        0     2790 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/pose/train.py
--rw-rw-rw-   0        0        0    10932 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/pose/val.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:50:07.685448 ppmmvehicle-1.0.0/ultralytics/yolo/v8/segment/
--rw-rw-rw-   0        0        0      295 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/segment/__init__.py
--rw-rw-rw-   0        0        0     2839 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/segment/predict.py
--rw-rw-rw-   0        0        0     2499 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/segment/train.py
--rw-rw-rw-   0        0        0    12906 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.0/ultralytics/yolo/v8/segment/val.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.275287 ppmmvehicle-1.0.1/
+-rw-rw-rw-   0        0        0     5624 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    34523 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      213 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    28644 2023-06-30 03:32:35.275287 ppmmvehicle-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    24548 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/README.md
+-rw-rw-rw-   0        0        0    23524 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/README.zh-CN.md
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.251288 ppmmvehicle-1.0.1/ppmmvehicle.egg-info/
+-rw-rw-rw-   0        0        0    28644 2023-06-30 03:32:35.000000 ppmmvehicle-1.0.1/ppmmvehicle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2023-06-30 03:32:35.000000 ppmmvehicle-1.0.1/ppmmvehicle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 03:32:35.000000 ppmmvehicle-1.0.1/ppmmvehicle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-30 03:32:35.000000 ppmmvehicle-1.0.1/ppmmvehicle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      369 2023-06-30 03:32:35.000000 ppmmvehicle-1.0.1/ppmmvehicle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 03:32:35.000000 ppmmvehicle-1.0.1/ppmmvehicle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1129 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0      723 2023-06-30 03:32:35.276287 ppmmvehicle-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3181 2023-06-30 03:15:19.000000 ppmmvehicle-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.251288 ppmmvehicle-1.0.1/ultralytics/
+-rw-rw-rw-   0        0        0      451 2023-06-30 03:20:59.000000 ppmmvehicle-1.0.1/ultralytics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.253288 ppmmvehicle-1.0.1/ultralytics/assets/
+-rw-rw-rw-   0        0        0   137419 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/assets/bus.jpg
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.262287 ppmmvehicle-1.0.1/ultralytics/datasets/
+-rw-rw-rw-   0        0        0     2751 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/Argoverse.yaml
+-rw-rw-rw-   0        0        0     1986 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-rw-rw-   0        0        0    42439 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/datasets/ImageNet.yaml
+-rw-rw-rw-   0        0        0     9270 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/Objects365.yaml
+-rw-rw-rw-   0        0        0     2437 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/SKU-110K.yaml
+-rw-rw-rw-   0        0        0     3512 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/VOC.yaml
+-rw-rw-rw-   0        0        0     3012 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/VisDrone.yaml
+-rw-rw-rw-   0        0        0     1547 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/coco-pose.yaml
+-rw-rw-rw-   0        0        0     2526 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/coco.yaml
+-rw-rw-rw-   0        0        0     1862 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/datasets/coco128-seg.yaml
+-rw-rw-rw-   0        0        0     1846 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/datasets/coco128.yaml
+-rw-rw-rw-   0        0        0      895 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/datasets/coco8-pose.yaml
+-rw-rw-rw-   0        0        0     1797 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/datasets/coco8-seg.yaml
+-rw-rw-rw-   0        0        0     1777 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/datasets/coco8.yaml
+-rw-rw-rw-   0        0        0     5178 2023-06-27 09:07:16.000000 ppmmvehicle-1.0.1/ultralytics/datasets/xView.yaml
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.238288 ppmmvehicle-1.0.1/ultralytics/models/
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.264287 ppmmvehicle-1.0.1/ultralytics/models/rt-detr/
+-rw-rw-rw-   0        0        0     1970 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/rt-detr/rt-detr-l.yaml
+-rw-rw-rw-   0        0        0     2177 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/rt-detr/rt-detr-x.yaml
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.266289 ppmmvehicle-1.0.1/ultralytics/models/v3/
+-rw-rw-rw-   0        0        0     1550 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v3/yolov3-spp.yaml
+-rw-rw-rw-   0        0        0     1252 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-rw-rw-   0        0        0     1537 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v3/yolov3.yaml
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.267288 ppmmvehicle-1.0.1/ultralytics/models/v5/
+-rw-rw-rw-   0        0        0     1923 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v5/yolov5-p6.yaml
+-rw-rw-rw-   0        0        0     1550 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v5/yolov5.yaml
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.268288 ppmmvehicle-1.0.1/ultralytics/models/v6/
+-rw-rw-rw-   0        0        0     1680 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v6/yolov6.yaml
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.272288 ppmmvehicle-1.0.1/ultralytics/models/v8/
+-rw-rw-rw-   0        0        0      920 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-cls.yaml
+-rw-rw-rw-   0        0        0     1751 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-p2.yaml
+-rw-rw-rw-   0        0        0     1856 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-p6.yaml
+-rw-rw-rw-   0        0        0     1946 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-rw-rw-   0        0        0     1580 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-pose.yaml
+-rw-rw-rw-   0        0        0     1490 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-seg.yaml
+-rw-rw-rw-   0        0        0     1913 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8.yaml
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.239290 ppmmvehicle-1.0.1/ultralytics/tracker/
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.273287 ppmmvehicle-1.0.1/ultralytics/tracker/cfg/
+-rw-rw-rw-   0        0        0      890 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/tracker/cfg/botsort.yaml
+-rw-rw-rw-   0        0        0      694 2023-06-11 18:39:32.000000 ppmmvehicle-1.0.1/ultralytics/tracker/cfg/bytetrack.yaml
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.239290 ppmmvehicle-1.0.1/ultralytics/yolo/
+drwxrwxrwx   0        0        0        0 2023-06-30 03:32:35.274288 ppmmvehicle-1.0.1/ultralytics/yolo/cfg/
+-rw-rw-rw-   0        0        0     6356 2023-06-19 03:05:30.000000 ppmmvehicle-1.0.1/ultralytics/yolo/cfg/backup.yaml
+-rw-rw-rw-   0        0        0     6365 2023-06-29 08:40:29.000000 ppmmvehicle-1.0.1/ultralytics/yolo/cfg/default.yaml
```

### Comparing `ppmmvehicle-1.0.0/CONTRIBUTING.md` & `ppmmvehicle-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/LICENSE` & `ppmmvehicle-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/PKG-INFO` & `ppmmvehicle-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppmmvehicle
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ppmmvehicle Version: 1.0.0 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ppmmvehicle Version: 1.0.1 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Home-page: https://github.com/
 ultralytics/ultralytics Author: Ultralytics Author-email: hello@ultralytics.com
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics Description:
    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-
```

### Comparing `ppmmvehicle-1.0.0/README.md` & `ppmmvehicle-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/README.zh-CN.md` & `ppmmvehicle-1.0.1/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ppmmvehicle.egg-info/PKG-INFO` & `ppmmvehicle-1.0.1/ppmmvehicle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppmmvehicle
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ppmmvehicle Version: 1.0.0 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ppmmvehicle Version: 1.0.1 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Home-page: https://github.com/
 ultralytics/ultralytics Author: Ultralytics Author-email: hello@ultralytics.com
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics Description:
    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-
```

### Comparing `ppmmvehicle-1.0.0/requirements.txt` & `ppmmvehicle-1.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/setup.cfg` & `ppmmvehicle-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/setup.py` & `ppmmvehicle-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     url='https://github.com/ultralytics/ultralytics',
     project_urls={
         'Bug Reports': 'https://github.com/ultralytics/ultralytics/issues',
         'Funding': 'https://ultralytics.com',
         'Source': 'https://github.com/ultralytics/ultralytics'},
     author='Ultralytics',
     author_email='hello@ultralytics.com',
-    packages=find_packages(),  # required
+    # packages=find_packages(),  # required
+    packages=["ultralytics"],  # required
     include_package_data=True,
     install_requires=REQUIREMENTS,
     extras_require={
         'dev': [
             'check-manifest',
             'pytest',
             'pytest-cov',
```

### Comparing `ppmmvehicle-1.0.0/ultralytics/assets/bus.jpg` & `ppmmvehicle-1.0.1/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/Argoverse.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/GlobalWheat2020.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/ImageNet.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/Objects365.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/SKU-110K.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/VOC.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/VisDrone.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/coco-pose.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/coco.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/coco128-seg.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/coco128.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/coco8-pose.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/coco8-seg.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/coco8.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/datasets/xView.yaml` & `ppmmvehicle-1.0.1/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/rt-detr/rt-detr-l.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/rt-detr/rt-detr-l.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/rt-detr/rt-detr-x.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/rt-detr/rt-detr-x.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v3/yolov3-spp.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v3/yolov3-tiny.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v3/yolov3.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v5/yolov5-p6.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v5/yolov5.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v6/yolov6.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-cls.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-p2.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-p6.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-pose.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8-seg.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/models/v8/yolov8.yaml` & `ppmmvehicle-1.0.1/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/tracker/cfg/botsort.yaml` & `ppmmvehicle-1.0.1/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/tracker/cfg/bytetrack.yaml` & `ppmmvehicle-1.0.1/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/yolo/cfg/backup.yaml` & `ppmmvehicle-1.0.1/ultralytics/yolo/cfg/backup.yaml`

 * *Files identical despite different names*

### Comparing `ppmmvehicle-1.0.0/ultralytics/yolo/cfg/default.yaml` & `ppmmvehicle-1.0.1/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

