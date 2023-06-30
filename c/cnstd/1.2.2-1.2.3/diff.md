# Comparing `tmp/cnstd-1.2.2.tar.gz` & `tmp/cnstd-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnstd-1.2.2.tar", last modified: Sun Feb 19 03:21:01 2023, max compression
+gzip compressed data, was "cnstd-1.2.3.tar", last modified: Fri Jun 30 04:27:44 2023, max compression
```

## Comparing `cnstd-1.2.2.tar` & `cnstd-1.2.3.tar`

### file list

```diff
@@ -1,90 +1,98 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.902604 cnstd-1.2.2/
--rw-r--r--   0 king       (501) staff       (20)    31514 2023-02-19 03:21:01.901909 cnstd-1.2.2/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    25974 2023-02-19 03:16:03.000000 cnstd-1.2.2/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.360857 cnstd-1.2.2/cnstd/
--rw-r--r--   0 king       (501) staff       (20)     1025 2022-10-07 15:02:09.000000 cnstd-1.2.2/cnstd/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      891 2023-02-18 15:01:02.000000 cnstd-1.2.2/cnstd/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     4891 2022-07-06 05:54:12.000000 cnstd-1.2.2/cnstd/app.py
--rw-r--r--   0 king       (501) staff       (20)    13890 2023-02-19 02:44:43.000000 cnstd-1.2.2/cnstd/cli.py
--rw-r--r--   0 king       (501) staff       (20)    10018 2023-02-11 16:08:09.000000 cnstd-1.2.2/cnstd/cn_std.py
--rw-r--r--   0 king       (501) staff       (20)     8567 2023-02-08 07:47:10.000000 cnstd-1.2.2/cnstd/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.413679 cnstd-1.2.2/cnstd/datasets/
--rw-r--r--   0 king       (501) staff       (20)      916 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/datasets/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    10658 2022-06-30 13:44:51.000000 cnstd-1.2.2/cnstd/datasets/dataset.py
--rw-r--r--   0 king       (501) staff       (20)     8936 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/datasets/util.py
--rw-r--r--   0 king       (501) staff       (20)    12240 2022-07-31 07:00:29.000000 cnstd-1.2.2/cnstd/detector.py
--rw-r--r--   0 king       (501) staff       (20)     7573 2021-12-05 08:15:10.000000 cnstd-1.2.2/cnstd/lr_scheduler.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.432304 cnstd-1.2.2/cnstd/model/
--rw-r--r--   0 king       (501) staff       (20)     1733 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/model/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    15884 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/model/base.py
--rw-r--r--   0 king       (501) staff       (20)    10382 2022-07-05 04:55:42.000000 cnstd-1.2.2/cnstd/model/core.py
--rw-r--r--   0 king       (501) staff       (20)    10061 2021-12-05 08:14:50.000000 cnstd-1.2.2/cnstd/model/dbnet.py
--rw-r--r--   0 king       (501) staff       (20)     4061 2021-12-05 08:14:50.000000 cnstd-1.2.2/cnstd/model/fpn.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.452207 cnstd-1.2.2/cnstd/ppocr/
--rw-r--r--   0 king       (501) staff       (20)     1070 2022-07-02 11:56:46.000000 cnstd-1.2.2/cnstd/ppocr/__init__.py
--rwxr-xr-x   0 king       (501) staff       (20)     7586 2023-02-11 13:26:35.000000 cnstd-1.2.2/cnstd/ppocr/angle_classifier.py
--rw-r--r--   0 king       (501) staff       (20)     1192 2022-07-01 02:57:56.000000 cnstd-1.2.2/cnstd/ppocr/consts.py
--rw-r--r--   0 king       (501) staff       (20)    14517 2022-07-06 02:43:04.000000 cnstd-1.2.2/cnstd/ppocr/img_operators.py
--rw-r--r--   0 king       (501) staff       (20)     1856 2022-07-02 11:57:35.000000 cnstd-1.2.2/cnstd/ppocr/opt_utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.481497 cnstd-1.2.2/cnstd/ppocr/postprocess/
--rw-r--r--   0 king       (501) staff       (20)     1636 2022-07-02 11:55:21.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     1522 2022-07-02 11:55:40.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/cls_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)     8091 2022-07-05 02:34:41.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/db_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)     5103 2022-05-27 13:20:26.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/east_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)     5034 2022-05-02 05:59:45.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/locality_aware_nms.py
--rw-r--r--   0 king       (501) staff       (20)     1813 2022-05-02 05:59:45.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/pg_postprocess.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.484709 cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/
--rw-r--r--   0 king       (501) staff       (20)      654 2022-05-02 05:59:45.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/__init__.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.491636 cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/pse/
--rw-r--r--   0 king       (501) staff       (20)     1145 2022-05-02 05:59:45.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      326 2022-05-02 05:59:45.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/pse/setup.py
--rwxr-xr-x   0 king       (501) staff       (20)     4047 2022-05-02 05:59:45.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)    25211 2022-05-15 09:38:05.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/rec_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)    13673 2022-05-15 09:49:29.000000 cnstd-1.2.2/cnstd/ppocr/postprocess/sast_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)    11632 2023-02-18 14:58:36.000000 cnstd-1.2.2/cnstd/ppocr/pp_detector.py
--rwxr-xr-x   0 king       (501) staff       (20)    17083 2022-05-15 10:20:14.000000 cnstd-1.2.2/cnstd/ppocr/predict_rec.py
--rwxr-xr-x   0 king       (501) staff       (20)     8506 2022-07-02 10:58:02.000000 cnstd-1.2.2/cnstd/ppocr/predict_system.py
--rw-r--r--   0 king       (501) staff       (20)    18824 2022-07-06 03:52:50.000000 cnstd-1.2.2/cnstd/ppocr/utility.py
--rw-r--r--   0 king       (501) staff       (20)     8872 2021-12-05 08:14:50.000000 cnstd-1.2.2/cnstd/trainer.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.620599 cnstd-1.2.2/cnstd/transforms/
--rw-r--r--   0 king       (501) staff       (20)     1009 2021-12-05 08:14:50.000000 cnstd-1.2.2/cnstd/transforms/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4029 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/transforms/base.py
--rw-r--r--   0 king       (501) staff       (20)    11529 2021-12-05 08:14:50.000000 cnstd-1.2.2/cnstd/transforms/process_data.py
--rw-r--r--   0 king       (501) staff       (20)     2836 2021-12-05 08:14:50.000000 cnstd-1.2.2/cnstd/transforms/random_crop.py
--rw-r--r--   0 king       (501) staff       (20)     3018 2022-06-30 13:47:18.000000 cnstd-1.2.2/cnstd/transforms/resize.py
--rw-r--r--   0 king       (501) staff       (20)     4109 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/transforms/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.700437 cnstd-1.2.2/cnstd/utils/
--rw-r--r--   0 king       (501) staff       (20)     1043 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     9475 2023-02-01 06:21:40.000000 cnstd-1.2.2/cnstd/utils/_utils.py
--rw-r--r--   0 king       (501) staff       (20)     1236 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/utils/common_types.py
--rw-r--r--   0 king       (501) staff       (20)     4329 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/utils/geometry.py
--rw-r--r--   0 king       (501) staff       (20)    15158 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/utils/metrics.py
--rw-r--r--   0 king       (501) staff       (20)     2649 2021-08-26 09:54:14.000000 cnstd-1.2.2/cnstd/utils/repr.py
--rw-r--r--   0 king       (501) staff       (20)    15968 2023-02-18 15:24:02.000000 cnstd-1.2.2/cnstd/utils/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.893547 cnstd-1.2.2/cnstd/yolov7/
--rw-r--r--   0 king       (501) staff       (20)      869 2022-10-06 08:11:18.000000 cnstd-1.2.2/cnstd/yolov7/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     8109 2022-10-06 08:12:51.000000 cnstd-1.2.2/cnstd/yolov7/autoanchor.py
--rw-r--r--   0 king       (501) staff       (20)    85336 2022-10-06 08:12:58.000000 cnstd-1.2.2/cnstd/yolov7/common.py
--rw-r--r--   0 king       (501) staff       (20)     1300 2022-12-18 14:43:12.000000 cnstd-1.2.2/cnstd/yolov7/consts.py
--rw-r--r--   0 king       (501) staff       (20)    57174 2023-02-01 06:27:41.000000 cnstd-1.2.2/cnstd/yolov7/datasets.py
--rw-r--r--   0 king       (501) staff       (20)    11822 2022-10-06 08:14:21.000000 cnstd-1.2.2/cnstd/yolov7/experimental.py
--rw-r--r--   0 king       (501) staff       (20)    38670 2022-12-18 15:04:18.000000 cnstd-1.2.2/cnstd/yolov7/general.py
--rw-r--r--   0 king       (501) staff       (20)    13911 2023-02-19 02:09:32.000000 cnstd-1.2.2/cnstd/yolov7/layout_analyzer.py
--rw-r--r--   0 king       (501) staff       (20)    75901 2022-10-06 08:14:45.000000 cnstd-1.2.2/cnstd/yolov7/loss.py
--rw-r--r--   0 king       (501) staff       (20)    10277 2022-10-06 08:14:45.000000 cnstd-1.2.2/cnstd/yolov7/metrics.py
--rw-r--r--   0 king       (501) staff       (20)    22030 2022-10-13 04:28:33.000000 cnstd-1.2.2/cnstd/yolov7/plots.py
--rw-r--r--   0 king       (501) staff       (20)    16420 2022-12-18 14:21:22.000000 cnstd-1.2.2/cnstd/yolov7/torch_utils.py
--rw-r--r--   0 king       (501) staff       (20)    40992 2022-10-06 08:15:08.000000 cnstd-1.2.2/cnstd/yolov7/yolo.py
--rw-r--r--   0 king       (501) staff       (20)     5010 2023-02-08 07:45:10.000000 cnstd-1.2.2/cnstd/yolov7/yolov7-mfd.yaml
--rw-r--r--   0 king       (501) staff       (20)     5586 2022-10-06 08:15:22.000000 cnstd-1.2.2/cnstd/yolov7/yolov7-tiny-layout.yaml
--rw-r--r--   0 king       (501) staff       (20)     5630 2022-12-18 13:53:41.000000 cnstd-1.2.2/cnstd/yolov7/yolov7-tiny-mfd.yaml
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-02-19 03:21:01.407708 cnstd-1.2.2/cnstd.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    31514 2023-02-19 03:21:00.000000 cnstd-1.2.2/cnstd.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     2113 2023-02-19 03:21:00.000000 cnstd-1.2.2/cnstd.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2023-02-19 03:21:00.000000 cnstd-1.2.2/cnstd.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       41 2023-02-19 03:21:00.000000 cnstd-1.2.2/cnstd.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2020-05-31 06:07:08.000000 cnstd-1.2.2/cnstd.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      219 2023-02-19 03:21:00.000000 cnstd-1.2.2/cnstd.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)        6 2023-02-19 03:21:00.000000 cnstd-1.2.2/cnstd.egg-info/top_level.txt
--rw-r--r--   0 king       (501) staff       (20)       38 2023-02-19 03:21:01.910836 cnstd-1.2.2/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     3164 2023-02-18 15:37:20.000000 cnstd-1.2.2/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.426244 cnstd-1.2.3/
+-rw-r--r--   0 king       (501) staff       (20)    41980 2019-03-26 07:39:48.000000 cnstd-1.2.3/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    28335 2023-06-30 04:27:44.423622 cnstd-1.2.3/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    27254 2023-06-30 04:25:33.000000 cnstd-1.2.3/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.321058 cnstd-1.2.3/cnstd/
+-rw-r--r--   0 king       (501) staff       (20)     1025 2022-10-07 15:02:09.000000 cnstd-1.2.3/cnstd/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      896 2023-06-30 04:08:02.000000 cnstd-1.2.3/cnstd/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     4891 2022-07-06 05:54:12.000000 cnstd-1.2.3/cnstd/app.py
+-rw-r--r--   0 king       (501) staff       (20)    13890 2023-02-19 02:44:43.000000 cnstd-1.2.3/cnstd/cli.py
+-rw-r--r--   0 king       (501) staff       (20)    10018 2023-02-11 16:08:09.000000 cnstd-1.2.3/cnstd/cn_std.py
+-rw-r--r--   0 king       (501) staff       (20)     8753 2023-06-30 04:07:55.000000 cnstd-1.2.3/cnstd/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.331887 cnstd-1.2.3/cnstd/datasets/
+-rw-r--r--   0 king       (501) staff       (20)      916 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/datasets/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    10658 2022-06-30 13:44:51.000000 cnstd-1.2.3/cnstd/datasets/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     8936 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/datasets/util.py
+-rw-r--r--   0 king       (501) staff       (20)    12240 2022-07-31 07:00:29.000000 cnstd-1.2.3/cnstd/detector.py
+-rw-r--r--   0 king       (501) staff       (20)     7573 2021-12-05 08:15:10.000000 cnstd-1.2.3/cnstd/lr_scheduler.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.336797 cnstd-1.2.3/cnstd/model/
+-rw-r--r--   0 king       (501) staff       (20)     1733 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/model/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    15884 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/model/base.py
+-rw-r--r--   0 king       (501) staff       (20)    10382 2022-07-05 04:55:42.000000 cnstd-1.2.3/cnstd/model/core.py
+-rw-r--r--   0 king       (501) staff       (20)    10061 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/model/dbnet.py
+-rw-r--r--   0 king       (501) staff       (20)     4061 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/model/fpn.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.350460 cnstd-1.2.3/cnstd/ppocr/
+-rw-r--r--   0 king       (501) staff       (20)     1070 2022-07-02 11:56:46.000000 cnstd-1.2.3/cnstd/ppocr/__init__.py
+-rwxr-xr-x   0 king       (501) staff       (20)     7586 2023-02-11 13:26:35.000000 cnstd-1.2.3/cnstd/ppocr/angle_classifier.py
+-rw-r--r--   0 king       (501) staff       (20)     1192 2022-07-01 02:57:56.000000 cnstd-1.2.3/cnstd/ppocr/consts.py
+-rw-r--r--   0 king       (501) staff       (20)    14517 2022-07-06 02:43:04.000000 cnstd-1.2.3/cnstd/ppocr/img_operators.py
+-rw-r--r--   0 king       (501) staff       (20)     1856 2022-07-02 11:57:35.000000 cnstd-1.2.3/cnstd/ppocr/opt_utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.360363 cnstd-1.2.3/cnstd/ppocr/postprocess/
+-rw-r--r--   0 king       (501) staff       (20)     1636 2022-07-02 11:55:21.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     1522 2022-07-02 11:55:40.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/cls_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)     8091 2022-07-05 02:34:41.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/db_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)     5103 2022-05-27 13:20:26.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/east_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)     5034 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/locality_aware_nms.py
+-rw-r--r--   0 king       (501) staff       (20)     1813 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pg_postprocess.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.364259 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/
+-rw-r--r--   0 king       (501) staff       (20)      654 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/__init__.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.366442 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse/
+-rw-r--r--   0 king       (501) staff       (20)     1145 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      326 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse/setup.py
+-rwxr-xr-x   0 king       (501) staff       (20)     4047 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)    25211 2022-05-15 09:38:05.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/rec_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)    13673 2022-05-15 09:49:29.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/sast_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)    11632 2023-02-18 14:58:36.000000 cnstd-1.2.3/cnstd/ppocr/pp_detector.py
+-rwxr-xr-x   0 king       (501) staff       (20)    17083 2022-05-15 10:20:14.000000 cnstd-1.2.3/cnstd/ppocr/predict_rec.py
+-rwxr-xr-x   0 king       (501) staff       (20)     8506 2022-07-02 10:58:02.000000 cnstd-1.2.3/cnstd/ppocr/predict_system.py
+-rw-r--r--   0 king       (501) staff       (20)    18824 2022-07-06 03:52:50.000000 cnstd-1.2.3/cnstd/ppocr/utility.py
+-rw-r--r--   0 king       (501) staff       (20)     8872 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/trainer.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.372243 cnstd-1.2.3/cnstd/transforms/
+-rw-r--r--   0 king       (501) staff       (20)     1009 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/transforms/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4029 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/transforms/base.py
+-rw-r--r--   0 king       (501) staff       (20)    11529 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/transforms/process_data.py
+-rw-r--r--   0 king       (501) staff       (20)     2836 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/transforms/random_crop.py
+-rw-r--r--   0 king       (501) staff       (20)     3018 2022-06-30 13:47:18.000000 cnstd-1.2.3/cnstd/transforms/resize.py
+-rw-r--r--   0 king       (501) staff       (20)     4109 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/transforms/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.383505 cnstd-1.2.3/cnstd/utils/
+-rw-r--r--   0 king       (501) staff       (20)     1043 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     9475 2023-02-01 06:21:40.000000 cnstd-1.2.3/cnstd/utils/_utils.py
+-rw-r--r--   0 king       (501) staff       (20)     1236 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/common_types.py
+-rw-r--r--   0 king       (501) staff       (20)     4329 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/geometry.py
+-rw-r--r--   0 king       (501) staff       (20)    15158 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/metrics.py
+-rw-r--r--   0 king       (501) staff       (20)     2649 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/repr.py
+-rw-r--r--   0 king       (501) staff       (20)    15834 2023-06-30 02:47:39.000000 cnstd-1.2.3/cnstd/utils/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.406919 cnstd-1.2.3/cnstd/yolov7/
+-rw-r--r--   0 king       (501) staff       (20)      869 2022-10-06 08:11:18.000000 cnstd-1.2.3/cnstd/yolov7/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     8109 2022-10-06 08:12:51.000000 cnstd-1.2.3/cnstd/yolov7/autoanchor.py
+-rw-r--r--   0 king       (501) staff       (20)    85336 2022-10-06 08:12:58.000000 cnstd-1.2.3/cnstd/yolov7/common.py
+-rw-r--r--   0 king       (501) staff       (20)     1300 2022-12-18 14:43:12.000000 cnstd-1.2.3/cnstd/yolov7/consts.py
+-rw-r--r--   0 king       (501) staff       (20)    57174 2023-02-01 06:27:41.000000 cnstd-1.2.3/cnstd/yolov7/datasets.py
+-rw-r--r--   0 king       (501) staff       (20)    11822 2022-10-06 08:14:21.000000 cnstd-1.2.3/cnstd/yolov7/experimental.py
+-rw-r--r--   0 king       (501) staff       (20)    38670 2022-12-18 15:04:18.000000 cnstd-1.2.3/cnstd/yolov7/general.py
+-rw-r--r--   0 king       (501) staff       (20)    13911 2023-02-19 02:09:32.000000 cnstd-1.2.3/cnstd/yolov7/layout_analyzer.py
+-rw-r--r--   0 king       (501) staff       (20)    75901 2022-10-06 08:14:45.000000 cnstd-1.2.3/cnstd/yolov7/loss.py
+-rw-r--r--   0 king       (501) staff       (20)    10277 2022-10-06 08:14:45.000000 cnstd-1.2.3/cnstd/yolov7/metrics.py
+-rw-r--r--   0 king       (501) staff       (20)    22030 2022-10-13 04:28:33.000000 cnstd-1.2.3/cnstd/yolov7/plots.py
+-rw-r--r--   0 king       (501) staff       (20)    16420 2022-12-18 14:21:22.000000 cnstd-1.2.3/cnstd/yolov7/torch_utils.py
+-rw-r--r--   0 king       (501) staff       (20)    40992 2022-10-06 08:15:08.000000 cnstd-1.2.3/cnstd/yolov7/yolo.py
+-rw-r--r--   0 king       (501) staff       (20)     5010 2023-02-08 07:45:10.000000 cnstd-1.2.3/cnstd/yolov7/yolov7-mfd.yaml
+-rw-r--r--   0 king       (501) staff       (20)     5586 2022-10-06 08:15:22.000000 cnstd-1.2.3/cnstd/yolov7/yolov7-tiny-layout.yaml
+-rw-r--r--   0 king       (501) staff       (20)     5630 2022-12-18 13:53:41.000000 cnstd-1.2.3/cnstd/yolov7/yolov7-tiny-mfd.yaml
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.326361 cnstd-1.2.3/cnstd.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    28335 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     2256 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       40 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2020-05-31 06:07:08.000000 cnstd-1.2.3/cnstd.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      235 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)        6 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/top_level.txt
+-rw-r--r--   0 king       (501) staff       (20)       38 2023-06-30 04:27:44.426751 cnstd-1.2.3/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     3317 2023-06-30 04:04:58.000000 cnstd-1.2.3/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.418166 cnstd-1.2.3/tests/
+-rw-r--r--   0 king       (501) staff       (20)     1046 2022-07-06 06:05:27.000000 cnstd-1.2.3/tests/test_cnstd.py
+-rw-r--r--   0 king       (501) staff       (20)     1411 2021-12-05 08:14:50.000000 cnstd-1.2.3/tests/test_lr_schedulers.py
+-rw-r--r--   0 king       (501) staff       (20)      986 2021-12-05 08:14:50.000000 cnstd-1.2.3/tests/test_models.py
+-rw-r--r--   0 king       (501) staff       (20)      910 2021-08-26 09:54:14.000000 cnstd-1.2.3/tests/test_transforms.py
+-rw-r--r--   0 king       (501) staff       (20)      456 2023-02-18 14:57:29.000000 cnstd-1.2.3/tests/test_utils.py
+-rw-r--r--   0 king       (501) staff       (20)      281 2022-10-07 14:46:08.000000 cnstd-1.2.3/tests/test_yolov7.py
```

### Comparing `cnstd-1.2.2/PKG-INFO` & `cnstd-1.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,597 +1,605 @@
 Metadata-Version: 2.1
 Name: cnstd
-Version: 1.2.2
-Summary: Python3 package for Chinese/English STR (Scene Text Recognition), with small pretrained models
+Version: 1.2.3
+Summary: Python3 package for Chinese/English Scene Text Detection (STD), Mathematical Formula Detection (MFD), and Layout Analysis, with free pretrained models
 Home-page: https://github.com/breezedeus/cnstd
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
-Description: <div align="center">
-        	<img src="./docs/logo.png" width="250px"/>
-          <div>&nbsp;</div>
-        
-        [![Downloads](https://static.pepy.tech/personalized-badge/cnstd?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnstd)
-        [![license](https://img.shields.io/github/license/breezedeus/cnstd)](./LICENSE)
-        [![PyPI version](https://badge.fury.io/py/cnstd.svg)](https://badge.fury.io/py/cnstd)
-        [![forks](https://img.shields.io/github/forks/breezedeus/cnstd)](https://img.shields.io/github/forks/breezedeus/cnstd)
-        [![stars](https://img.shields.io/github/stars/breezedeus/cnstd)](https://github.com/breezedeus/cnocr)
-        ![last-releast](https://img.shields.io/github/release-date/breezedeus/cnstd?style=plastic)
-        ![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnstd)
-        [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
-        
-        </div>
-        
-        # CnSTD
-        
-        
-        # Update 2023.02.19：发布 V1.2.2
-        
-        主要变更：
-        * MFD训练了参数更多精度更高的模型，供 [P2T网页版](https://p2t.behye.com) 使用。
-        * 优化了检测出的boxes的排序算法，使得boxes的顺序更加符合人类的阅读习惯。
-        
-        了解更多：[RELEASE.md](./RELEASE.md) 。
-        
-        ---
-        
-        
-        
-        **CnSTD** 是 **Python 3** 下的**场景文字检测**（**Scene Text Detection**，简称**STD**）工具包，支持**中文**、**英文**等语言的文字检测，自带了多个训练好的检测模型，安装后即可直接使用。**CnSTD** 自 **V1.2.1** 版本开始，加入了**数学公式检测**（**Mathematical Formula Detection**，简称**MFD**）模型，并提供训练好的模型可直接用于检测图片中包含的数学公式（**行内公式** `embedding` 与**独立行公式** `isolated` ）。
-        
-        欢迎扫码加入微信交流群：
-        
-        <div align="center">
-          <img src="https://huggingface.co/datasets/breezedeus/cnocr-wx-qr-code/resolve/main/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
-        </div>
-        
-        作者也维护 **知识星球** [**CnOCR/CnSTD/P2T私享群**](https://t.zsxq.com/FEYZRJQ)，欢迎加入。**知识星球私享群**会陆续发布一些CnOCR/CnSTD/P2T相关的私有资料，包括**更详细的训练教程**，**未公开的模型**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。
-        
-        自 **V1.0.0** 版本开始，**CnSTD** 从之前基于 MXNet 实现转为基于 **PyTorch** 实现。新模型的训练合并了  **ICPR MTWI 2018**、**ICDAR RCTW-17** 和 **ICDAR2019-LSVT** 三个数据集，包括了 **`46447`** 个训练样本，和 **`1534`** 个测试样本。
-        
-        相较于之前版本， 新版本的变化主要包括：
-        
-        * 加入了对 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR) 检测模型的支持；
-        * 部分调整了检测结果中 `box` 的表达方式，统一为 `4` 个点的坐标值；  
-        * 修复了已知bugs。
-        
-        如需要识别文本框中的文字，可以结合 **OCR** 工具包 **[cnocr](https://github.com/breezedeus/cnocr)** 一起使用。
-        
-        
-        ## 示例
-        
-        ### 场景文字检测（STD）
-        
-        <div align="center">
-          <img src="./docs/cases.png" alt="STD效果" width="700px"/>
-        </div>
-        
-        ### 数学公式检测（MFD）
-        
-        MFD 模型检测图片中包含的数学公式，其中行内的公式检测为 `embedding` 类别，独立行的公式检测为 `isolated`。模型训练使用了英文 [IBEM](https://zenodo.org/record/4757865) 和中文 [CnMFD_Dataset](https://github.com/breezedeus/CnMFD_Dataset) 两个数据集。
-        
-        <div align="center">
-          <img src="./examples/mfd/out-zh4.jpg" alt="中文MFD效果" width="700px"/>
-        </div>  
-        <div align="center">
-          <img src="./examples/mfd/out-zh5.jpg" alt="中文MFD效果" width="700px"/>
-        </div>
-        <div align="center">
-          <img src="./examples/mfd/out-en2.jpg" alt="英文MFD效果" width="700px"/>
-        </div> 
-        
-        
-        ### 版面分析（Layout Analysis）
-        
-        版面分析模型识别图片中的不同排版元素。模型训练使用的是 [CDLA](https://github.com/buptlihang/CDLA) 数据集。可识别以下10中版面元素：
-        
-        |正文|标题|图片|图片标题|表格|表格标题|页眉|页脚|注释|公式|
-        |---|---|---|---|---|---|---|---|---|---|
-        |Text|Title|Figure|Figure caption|Table|Table caption|Header|Footer|Reference|Equation|
-        
-        <div align="center">
-          <img src="./examples/layout/out-zh.jpg" alt="版面分析效果" width="700px"/>
-        </div>  
-        
-        
-        ## 安装
-        
-        嗯，顺利的话很简单（bless）。
-        
-        ```bash
-        pip install cnstd
-        ```
-        
-        安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
-        
-        ```bash
-        pip install cnstd -i https://pypi.doubanio.com/simple
-        ```
-        
-        【注意】：
-        
-        * 请使用 **Python3** (3.6以及之后版本应该都行)，没测过Python2下是否ok。
-        * 依赖 **opencv**，所以可能需要额外安装opencv。
-        
-        ## 已有STD模型
-        
-        CnSTD 从 **V1.2** 开始，可直接使用的模型包含两类：1）CnSTD 自己训练的模型，通常会包含 PyTorch 和 ONNX 版本；2）从其他ocr引擎搬运过来的训练好的外部模型，ONNX化后用于 CnSTD 中。
-        
-        直接使用的模型都放在 [**cnstd-cnocr-models**](https://huggingface.co/breezedeus/cnstd-cnocr-models) 项目中，可免费下载使用。
-        
-        ### 1. CnSTD 自己训练的模型
-        
-        当前版本（Since **V1.1.0**）的文字检测模型使用的是 [**DBNet**](https://github.com/MhLiao/DB)，相较于 V0.1 使用的 [PSENet](https://github.com/whai362/PSENet) 模型， DBNet 的检测耗时几乎下降了一个量级，同时检测精度也得到了极大的提升。
-        
-        目前包含以下已训练好的模型：
-        
-        | 模型名称                       | 参数规模      | 模型文件大小    | 测试集精度（IoU） | 平均推断耗时<br />（秒/张） | 下载方式                                                      |
-        | -------------------------- | --------- | --------- | ---------- | ----------------- | --------------------------------------------------------- |
-        | db_resnet34                | 22.5 M    | 86 M      | **0.7322** | 3.11              | 自动                                                        |
-        | db_resnet18                | 12.3 M    | 47 M      | 0.7294     | 1.93              | 自动                                                        |
-        | db_mobilenet_v3            | 4.2 M     | 16 M      | **0.7269** | 1.76              | 自动                                                        |
-        | db_mobilenet_v3_small      | 2.0 M     | 7.9 M     | 0.7054     | 1.24              | 自动                                                        |
-        | db_shufflenet_v2           | 4.7 M     | 18 M      | 0.7238     | 1.73              | 自动                                                        |
-        | **db_shufflenet_v2_small** | 3.0 M     | 12 M      | 0.7190     | 1.29              | 自动                                                        |
-        | db_shufflenet_v2_tiny      | **1.9 M** | **7.5 M** | **0.7172** | **1.14**          | [下载链接](https://mp.weixin.qq.com/s/fHPNoGyo72EFApVhEgR6Nw) |
-        
-        > 上表耗时基于本地 Mac 获得，绝对值无太大参考价值，相对值可供参考。IoU的计算方式经过调整，仅相对值可供参考。
-        
-        相对于两个基于 **ResNet** 的模型，基于 **MobileNet** 和 **ShuffleNet** 的模型体积更小，速度更快，建议在轻量级场景使用。
-        
-        ### 2. 外部模型
-        
-        以下模型是 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR) 中模型的 **ONNX** 版本，所以不会依赖 **PaddlePaddle** 相关工具包，故而也不支持基于这些模型在自己的领域数据上继续精调模型。这些模型支持检测**竖排文字**。
-        
-        | `model_name`    | PyTorch 版本 | ONNX 版本 | 支持检测的语言    | 模型文件大小 |
-        | --------------- | ---------- | ------- | ---------- | ------ |
-        | ch_PP-OCRv3_det | X          | √       | 简体中问、英文、数字 | 2.3 M  |
-        | ch_PP-OCRv2_det | X          | √       | 简体中问、英文、数字 | 2.2 M  |
-        | en_PP-OCRv3_det | X          | √       | **英文**、数字  | 2.3 M  |
-        
-        更多模型可参考 [PaddleOCR/models_list.md](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/models_list.md) 。如有其他外语（如日、韩等）检测需求，可在 **知识星球** [**CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) 中向作者提出建议。
-        
-        ## 使用方法
-        
-        首次使用 **CnSTD** 时，系统会自动下载zip格式的模型压缩文件，并存放于 `~/.cnstd`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\cnstd`）。下载速度超快。下载后的zip文件代码会自动对其解压，然后把解压后的模型相关目录放于`~/.cnstd/1.2`目录中。
-        
-        如果系统无法自动成功下载zip文件，则需要手动从 [百度云盘](https://pan.baidu.com/s/1zDMzArCDrrXHWL0AWxwYQQ?pwd=nstd)（提取码为 `nstd`）下载对应的zip文件并把它存放于 `~/.cnstd/1.2`（Windows下为 `C:\Users\<username>\AppData\Roaming\cnstd\1.2`）目录中。模型也可从 **[cnstd-cnocr-models](https://huggingface.co/breezedeus/cnstd-cnocr-models)** 中下载。放置好zip文件后，后面的事代码就会自动执行了。
-        
-        ### 场景文字检测（STD）
-        
-        使用类 `CnStd` 进行场景文字的检测。类 `CnStd` 的初始化函数如下：
-        
-        ```python
-        class CnStd(object):
-            """
-            场景文字检测器（Scene Text Detection）。虽然名字中有个"Cn"（Chinese），但其实也可以轻松识别英文的。
-            """
-        
-            def __init__(
-                self,
-                model_name: str = 'ch_PP-OCRv3_det',
-                *,
-                auto_rotate_whole_image: bool = False,
-                rotated_bbox: bool = True,
-                context: str = 'cpu',
-                model_fp: Optional[str] = None,
-                model_backend: str = 'onnx',  # ['pytorch', 'onnx']
-                root: Union[str, Path] = data_dir(),
-                use_angle_clf: bool = False,
-                angle_clf_configs: Optional[dict] = None,
-                **kwargs,
-            ):
-        ```
-        
-        其中的几个参数含义如下：
-        
-        * `model_name`:  模型名称，即前面模型表格第一列中的值。默认为 **ch_PP-OCRv3_det** 。
-        
-        * `auto_rotate_whole_image`:  是否自动对整张图片进行旋转调整。默认为`False`。
-        
-        * `rotated_bbox`:  是否支持检测带角度的文本框；默认为 `True`，表示支持；取值为 `False` 时，只检测水平或垂直的文本。
-        
-        * `context`：预测使用的机器资源，可取值为字符串`cpu`、`gpu`、`cuda:0`。
-        
-        * `model_fp`:  如果不使用系统自带的模型，可以通过此参数直接指定所使用的模型文件（`.ckpt`文件）。
-        
-        * `model_backend` (str): 'pytorch', or 'onnx'。表明预测时是使用 PyTorch 版本模型，还是使用 ONNX 版本模型。  同样的模型，ONNX 版本的预测速度一般是 PyTorch 版本的2倍左右。默认为 `onnx`。
-        
-        * `root`: 模型文件所在的根目录。
-          
-          * Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/db_shufflenet_v2_small`。
-          * Windows下默认值为 `C:\Users\<username>\AppData\Roaming\cnstd`。
-        
-        * `use_angle_clf` (bool): 对于检测出的文本框，是否使用角度分类模型进行调整（检测出的文本框可能会存在倒转180度的情况）。默认为 `False`
-        
-        * `angle_clf_configs` (dict): 角度分类模型对应的参数取值，主要包含以下值：
-          
-          - `model_name`: 模型名称。默认为 'ch_ppocr_mobile_v2.0_cls'
-          - `model_fp`: 如果不使用系统自带的模型，可以通过此参数直接指定所使用的模型文件（'.onnx' 文件）。默认为 `None`。具体可参考类 `AngleClassifier` 的说明
-        
-        每个参数都有默认取值，所以可以不传入任何参数值进行初始化：`std = CnStd()`。
-        
-        文本检测使用类`CnOcr`的函数 **`detect()`**，以下是详细说明：
-        
-        #### 类函数`CnStd.detect()`
-        
-        ```python
-            def detect(
-                self,
-                img_list: Union[
-                    str,
-                    Path,
-                    Image.Image,
-                    np.ndarray,
-                    List[Union[str, Path, Image.Image, np.ndarray]],
-                ],
-                resized_shape: Union[int, Tuple[int, int]] = (768, 768),
-                preserve_aspect_ratio: bool = True,
-                min_box_size: int = 8,
-                box_score_thresh: float = 0.3,
-                batch_size: int = 20,
-                **kwargs,
-            ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
-        ```
-        
-        **函数说明**：
-        
-        函数输入参数包括：
-        
-        - `img_list`: 支持对单个图片或者多个图片（列表）的检测。每个值可以是图片路径，或者已经读取进来 `PIL.Image.Image` 或 `np.ndarray`,  格式应该是 `RGB` 3 通道，shape: `(height, width, 3)`, 取值范围：`[0, 255]`。
-        
-        - `resized_shape`: `int` or `tuple`, `tuple` 含义为 `(height, width)`, `int` 则表示高宽都为此值；  
-           检测前，先把原始图片resize到接近此大小（只是接近，未必相等）。默认为 `(768, 768)`。
-          
-          > **Note** **（注意）**
-          > 这个取值对检测结果的影响较大，可以针对自己的应用多尝试几组值，再选出最优值。例如 `(512, 768)`, `(768, 768)`, `(768, 1024)`等。
-        
-        - `preserve_aspect_ratio`: 对原始图片 resize 时是否保持高宽比不变。默认为 `True`。
-        
-        - `min_box_size`: 过滤掉高度或者宽度小于此值的文本框。默认为 `8`，也即高或者宽小于 `8` 的文本框会被过滤去掉。
-        
-        - `box_score_thresh`: 过滤掉得分低于此值的文本框。默认为 `0.3`。
-        
-        - `batch_size`: 待处理图片很多时，需要分批处理，每批图片的数量由此参数指定。默认为 `20`。
-        
-        - `kwargs`: 保留参数，目前未被使用。
-        
-        函数输出类型为`list`，其中每个元素是一个字典，对应一张图片的检测结果。字典中包含以下 `keys`：
-        
-        - `rotated_angle`: `float`, 整张图片旋转的角度。只有 `auto_rotate_whole_image==True` 才可能非 `0`。
-        
-        - `detected_texts`: `list`, 每个元素存储了检测出的一个框的信息，使用词典记录，包括以下几个值：
-          
-          - `box`：检测出的文字对应的矩形框；`np.ndarray`, shape: `(4, 2)`，对应 box 4个点的坐标值 `(x, y)`;
-          
-          - `score`：得分；`float` 类型；分数越高表示越可靠；
-          
-          - `croppped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
-          
-          - 示例:
-            
-            ```python
-              [{'box': array([[416,  77],
-                              [486,  13],
-                              [800, 325],
-                              [730, 390]], dtype=int32),
-                'score': 1.0, 
-                'cropped_img': array([[[25, 20, 24],
-                                       [26, 21, 25],
-                                       [25, 20, 24],
-                                      ...,
-                                       [11, 11, 13],
-                                       [11, 11, 13],
-                                       [11, 11, 13]]], dtype=uint8)},
-               ...
-              ]
-            ```
-        
-        #### 调用示例
-        
-        ```python
-        from cnstd import CnStd
-        std = CnStd()
-        box_info_list = std.detect('examples/taobao.jpg')
-        ```
-        
-        或：
-        
-        ```python
-        from PIL import Image
-        from cnstd import CnStd
-        
-        std = CnStd()
-        img_fp = 'examples/taobao.jpg'
-        img = Image.open(img_fp)
-        box_infos = std.detect(img)
-        ```
-        
-        ### 识别检测框中的文字（OCR）
-        
-        上面示例识别结果中"cropped_img"对应的值可以直接交由 **[cnocr](https://github.com/breezedeus/cnocr)** 中的 **`CnOcr`** 进行文字识别。如上例可以结合  **`CnOcr`** 进行文字识别：
-        
-        ```python
-        from cnstd import CnStd
-        from cnocr import CnOcr
-        
-        std = CnStd()
-        cn_ocr = CnOcr()
-        
-        box_infos = std.detect('examples/taobao.jpg')
-        
-        for box_info in box_infos['detected_texts']:
-            cropped_img = box_info['cropped_img']
-            ocr_res = cn_ocr.ocr_for_single_line(cropped_img)
-            print('ocr result: %s' % str(ocr_res))
-        ```
-        
-        注：运行上面示例需要先安装  **[cnocr](https://github.com/breezedeus/cnocr)** ：
-        
-        ```bash
-        pip install cnocr
-        ```
-        
-        
-        
-        ### 数学公式检测（MFD）与 版面分析（Layout Analysis）
-        
-        数学公式检测（MFD）与 版面分析（Layout Analysis）都是检测图片中感兴趣的元素，它们使用的都是基于YOLOv7的检测架构，在CnSTD都来源于相同的类 `LayoutAnalyzer`，差别只是训练模型使用的数据不同。
-        
-        > 这两个模型的训练代码在 [yolov7](https://github.com/breezedeus/yolov7) 中（Forked from [WongKinYiu/yolov7](https://github.com/WongKinYiu/yolov7)，感谢原作者。）
-        
-        
-        
-        类 `LayoutAnalyzer` 的初始化函数如下：
-        
-        ```python
-        class LayoutAnalyzer(object):
-            def __init__(
-                self,
-                model_name: str = 'mfd',  # 'layout' or 'mfd'
-                *,
-                model_type: str = 'yolov7_tiny',
-                model_backend: str = 'pytorch',
-                model_fp: Optional[str] = None,
-                root: Union[str, Path] = data_dir(),
-                device: str = 'cpu',
-                **kwargs,
-            ):
-        ```
-        
-        其中的参数含义如下：
-        
-        - `model_name`: 字符串类型，表示模型类型。可选值：'mfd' 表示数学公式检测；'layout' 表示版面分析。默认值：'mfd'
-        
-        - `model_type`: 字符串类型，表示模型类型。当前支持 'yolov7_tiny' 和 'yolov7'；默认值：'yolov7_tiny'
-        
-        - `model_backend`: 字符串类型，表示backend。当前仅支持: 'pytorch'；默认值：'pytorch'
-        
-        - `model_fp`: 字符串类型，表示模型文件的路径。默认值：`None`，表示使用默认的文件路径
-        
-        - `root`: 字符串或`Path`类型，表示模型文件所在的根目录。
-          - Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/analysis`
-          - Windows下默认值为 `C:/Users/<username>/AppData/Roaming/cnstd`。
-          
-        - `device`: 字符串类型，表示运行模型的设备，可选值：'cpu' 或 'gpu'；默认值：'cpu'
-        
-        - `**kwargs`: 额外的参数。
-        
-        
-        
-        函数输出结果为一个`list`，其中每个元素表示识别出的版面中的一个元素，包含以下信息：
-        
-        * type: 版面元素对应的类型；可选值来自：`self.categories` ;
-        * box: 版面元素对应的矩形框；`np.ndarray`, shape: (4, 2)，对应 box 4个点的坐标值 `(x, y)` ;
-        * score: 得分，越高表示越可信 。
-        
-        
-        
-        #### 类函数`LayoutAnalyzer.analyze()`
-        
-        对指定图片（列表）进行版面分析。
-        
-        ```python
-        def analyze(
-            self,
-            img_list: Union[
-                str,
-                Path,
-                Image.Image,
-                np.ndarray,
-                List[Union[str, Path, Image.Image, np.ndarray]],
-            ],
-            resized_shape: Union[int, Tuple[int, int]] = 700,
-            box_margin: int = 2,
-            conf_threshold: float = 0.25,
-            iou_threshold: float = 0.45,
-        ) -> Union[List[Dict[str, Any]], List[List[Dict[str, Any]]]]:
-        ```
-        
-        
-        
-        **函数说明**：
-        
-        函数输入参数包括：
-        
-        * `img_list` (str or list): 待识别图片或图片列表；如果是 `np.ndarray`，则应该是shape为 `[H, W, 3]` 的 RGB 格式数组
-        * `resized_shape` (int or tuple): (H, W); 把图片resize到此大小再做分析；默认值为 `700`
-        * `box_margin` (int): 对识别出的内容框往外扩展的像素大小；默认值为 `2`
-        * `conf_threshold` (float): 分数阈值；默认值为 `0.25`
-        * `iou_threshold` (float): IOU阈值；默认值为 `0.45`
-        * `**kwargs`: 额外的参数。
-        
-        
-        
-        #### 调用示例
-        
-        ```python
-        from cnstd import LayoutAnalyzer
-        img_fp = 'examples/mfd/zh5.jpg'
-        analyzer = LayoutAnalyzer('mfd')
-        out = analyzer.analyze(img_fp, resized_shape=700)
-        print(out)
-        ```
-        
-        
-        
-        
-        
-        ### 脚本使用
-        
-        **cnstd** 包含了几个命令行工具，安装 **cnstd** 后即可使用。
-        
-        #### STD 预测单个文件或文件夹中所有图片
-        
-        使用命令 **`cnstd predict`** 预测单个文件或文件夹中所有图片，以下是使用说明：
-        
-        ```bash
-        (venv) ➜  cnstd git:(master) ✗ cnstd predict -h
-        Usage: cnstd predict [OPTIONS]
-        
-          预测单个文件，或者指定目录下的所有图片
-        
-        Options:
-          -m, --model-name [ch_PP-OCRv2_det|ch_PP-OCRv3_det|db_mobilenet_v3|db_mobilenet_v3_small|db_resnet18|db_resnet34|db_shufflenet_v2|db_shufflenet_v2_small|db_shufflenet_v2_tiny|en_PP-OCRv3_det]
-                                          模型名称。默认值为 db_shufflenet_v2_small
-          -b, --model-backend [pytorch|onnx]
-                                          模型类型。默认值为 `onnx`
-          -p, --pretrained-model-fp TEXT  使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型
-          -r, --rotated-bbox              是否检测带角度（非水平和垂直）的文本框。默认为 `True`
-          --resized-shape TEXT            格式："height,width";
-                                          预测时把图片resize到此大小再进行预测。两个值都需要是32的倍数。默认为
-                                          `768,768`
-        
-          --box-score-thresh FLOAT        检测结果只保留分数大于此值的文本框。默认值为 `0.3`
-          --preserve-aspect-ratio BOOLEAN
-                                          resize时是否保留图片原始比例。默认值为 `True`
-          --context TEXT                  使用cpu还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`。默认为
-                                          `cpu`
-        
-          -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹
-          -o, --output-dir TEXT           检测结果存放的文件夹。默认为 `./predictions`
-          -h, --help                      Show this message and exit.
-        ```
-        
-        例如可以使用以下命令对图片 `examples/taobao.jpg`进行检测，并把检测结果存放在目录 `outputs`中：
-        
-        ```bash
-        cnstd predict -i examples/taobao.jpg -o outputs
-        ```
-        
-        具体使用也可参考文件 [Makefile](./Makefile) 。
-        
-        
-        
-        #### MFD or Layout Analysis 预测单个文件
-        
-        使用命令 **`cnstd analyze`** 获得单个文件的 MFD 或者 Layout Analysis 结果，以下是使用说明：
-        
-        ```bash
-        (venv) ➜  cnstd git:(master) ✗ cnstd analyze -h
-        Usage: cnstd analyze [OPTIONS]
-        
-          对给定图片进行 MFD 或者 版面分析。
-        
-        Options:
-          -m, --model-name [mfd|layout]   模型类型。`mfd` 表示数学公式检测，`layout`
-                                          表示版面分析；默认为：`mfd`
-          -t, --model-type TEXT           模型类型。当前支持 [`yolov7_tiny`, `yolov7`]
-          -b, --model-backend [pytorch|onnx]
-                                          模型后端架构。当前仅支持 `pytorch`
-          -p, --model-fp TEXT             使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型
-          --device TEXT                   cuda device, i.e. 0 or 0,1,2,3 or cpu
-          -i, --img-fp TEXT               待分析的图片路径或图片目录
-          -o, --output-fp TEXT            分析结果输出的图片路径。默认为 `None`，会存储在当前文件夹，文件名称为输入文件名称
-                                          前面增加`out-`；如输入文件名为 `img.jpg`, 输出文件名即为 `out-
-                                          img.jpg`；如果输入为目录，则此路径也应该是一个目录，会将输出文件存储在此目录下
-          --resized-shape INTEGER         分析时把图片resize到此大小再进行。默认为 `700`
-          --conf-thresh FLOAT             Confidence Threshold。默认值为 `0.25`
-          --iou-thresh FLOAT              IOU threshold for NMS。默认值为 `0.45`
-          -h, --help                      Show this message and exit.
-        ```
-        
-        例如可以使用以下命令对图片 `examples/mfd/zh.jpg` 进行 MFD，并把检测结果存放在文件 `out-zh.jpg` 中：
-        
-        ```bash
-        (venv) ➜  cnstd analyze -m mfd --conf-thresh 0.25 --resized-shape 800 -i examples/mfd/zh.jpg -o out-zh.jpg
-        ```
-        
-        具体使用也可参考文件 [Makefile](./Makefile) 。
-        
-        #### 模型训练
-        
-        使用命令 **`cnstd train`**  训练文本检测模型，以下是使用说明：
-        
-        ```bash
-        (venv) ➜  cnstd git:(master) ✗ cnstd train -h
-        Usage: cnstd train [OPTIONS]
-        
-          训练文本检测模型
-        
-        Options:
-          -m, --model-name [db_resnet50|db_resnet34|db_resnet18|db_mobilenet_v3|db_mobilenet_v3_small|db_shufflenet_v2|db_shufflenet_v2_small|db_shufflenet_v2_tiny]
-                                          模型名称。默认值为 `db_shufflenet_v2_small`
-          -i, --index-dir TEXT            索引文件所在的文件夹，会读取文件夹中的 `train.tsv` 和 `dev.tsv` 文件
-                                          [required]
-        
-          --train-config-fp TEXT          训练使用的json配置文件  [required]
-          -r, --resume-from-checkpoint TEXT
-                                          恢复此前中断的训练状态，继续训练
-          -p, --pretrained-model-fp TEXT  导入的训练好的模型，作为初始模型。优先级低于 "--restore-training-
-                                          fp"，当传入"--restore-training-fp"时，此传入失效
-        
-          -h, --help                      Show this message and exit.
-        ```
-        
-        具体使用可参考文件 [Makefile](./Makefile) 。
-        
-        #### 模型转存
-        
-        训练好的模型会存储训练状态，使用命令 **`cnstd resave`**  去掉与预测无关的数据，降低模型大小。
-        
-        ```bash
-        (venv) ➜  cnstd git:(master) ✗ cnstd resave -h
-        Usage: cnstd resave [OPTIONS]
-        
-          训练好的模型会存储训练状态，使用此命令去掉预测时无关的数据，降低模型大小
-        
-        Options:
-          -i, --input-model-fp TEXT   输入的模型文件路径  [required]
-          -o, --output-model-fp TEXT  输出的模型文件路径  [required]
-          -h, --help                  Show this message and exit.
-        ```
-        
-        ## 未来工作
-        
-        * [x] 进一步精简模型结构，降低模型大小
-        * [x] PSENet速度上还是比较慢，尝试更快的STD算法
-        * [x] 加入更多的训练数据
-        * [x] 加入对外部模型的支持
-        * [x] 加入数学公式检测（MFD）与 版面分析（Layout Analysis）模型
-        * [ ] 加入对文档结构与表格的检测
-        
-        
-        
-        ## 给作者来杯咖啡
-        
-        开源不易，如果此项目对您有帮助，可以考虑 [给作者来杯咖啡 ☕️](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
-        
-        ---
-        
-        官方代码库：[https://github.com/breezedeus/cnstd](https://github.com/breezedeus/cnstd)。
 Platform: Mac
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+<div align="center">
+	<img src="./docs/logo.png" width="250px"/>
+  <div>&nbsp;</div>
+
+[![Downloads](https://static.pepy.tech/personalized-badge/cnstd?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnstd)
+[![license](https://img.shields.io/github/license/breezedeus/cnstd)](./LICENSE)
+[![PyPI version](https://badge.fury.io/py/cnstd.svg)](https://badge.fury.io/py/cnstd)
+[![forks](https://img.shields.io/github/forks/breezedeus/cnstd)](https://img.shields.io/github/forks/breezedeus/cnstd)
+[![stars](https://img.shields.io/github/stars/breezedeus/cnstd)](https://github.com/breezedeus/cnocr)
+![last-releast](https://img.shields.io/github/release-date/breezedeus/cnstd?style=plastic)
+![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnstd)
+[![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
+
+</div>
+
+# CnSTD
+# Update 2023.06.30：发布 V1.2.3
+
+主要变更：
+* 修复了模型文件自动下载的功能。HuggingFace似乎对下载文件的逻辑做了调整，导致之前版本的自动下载失败，当前版本已修复。但由于HuggingFace国内被墙，国内下载仍需 **梯子（VPN）**。
+* 更新了各个依赖包的版本号。
+
+# Update 2023.06.20：
+
+主要变更：
+* 基于新标注的数据，重新训练了 **MFD YoloV7** 模型，目前新模型已部署到 [P2T网页版](https://p2t.behye.com) 。具体说明见：[Pix2Text (P2T) 新版公式检测模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230613) 。
+* 之前的 MFD YoloV7 模型已开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
+* 增加了一些Label Studio相关的脚本，见 [scripts](scripts) 。如：利用 CnSTD 自带的 MFD 模型对目录中的图片进行公式检测后生成可导入到Label Studio中的JSON文件；以及，Label Studio标注后把导出的JSON文件转换成训练 MFD 模型所需的数据格式。注意，MFD 模型的训练代码在 [yolov7](https://github.com/breezedeus/yolov7) （`dev` branch）中。
+
+了解更多：[RELEASE.md](./RELEASE.md) 。
+
+---
+
+
+
+**CnSTD** 是 **Python 3** 下的**场景文字检测**（**Scene Text Detection**，简称**STD**）工具包，支持**中文**、**英文**等语言的文字检测，自带了多个训练好的检测模型，安装后即可直接使用。**CnSTD** 自 **V1.2.1** 版本开始，加入了**数学公式检测**（**Mathematical Formula Detection**，简称**MFD**）模型，并提供训练好的模型可直接用于检测图片中包含的数学公式（**行内公式** `embedding` 与**独立行公式** `isolated` ）。
+
+欢迎扫码加入微信交流群：
+
+<div align="center">
+  <img src="https://huggingface.co/datasets/breezedeus/cnocr-wx-qr-code/resolve/main/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
+</div>
+
+作者也维护 **知识星球** [**CnOCR/CnSTD/P2T私享群**](https://t.zsxq.com/FEYZRJQ)，欢迎加入。**知识星球私享群**会陆续发布一些CnOCR/CnSTD/P2T相关的私有资料，包括**更详细的训练教程**，**未公开的模型**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。
+
+自 **V1.0.0** 版本开始，**CnSTD** 从之前基于 MXNet 实现转为基于 **PyTorch** 实现。新模型的训练合并了  **ICPR MTWI 2018**、**ICDAR RCTW-17** 和 **ICDAR2019-LSVT** 三个数据集，包括了 **`46447`** 个训练样本，和 **`1534`** 个测试样本。
+
+相较于之前版本， 新版本的变化主要包括：
+
+* 加入了对 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR) 检测模型的支持；
+* 部分调整了检测结果中 `box` 的表达方式，统一为 `4` 个点的坐标值；  
+* 修复了已知bugs。
+
+如需要识别文本框中的文字，可以结合 **OCR** 工具包 **[cnocr](https://github.com/breezedeus/cnocr)** 一起使用。
+
+
+## 示例
+
+### 场景文字检测（STD）
+
+<div align="center">
+  <img src="./docs/cases.png" alt="STD效果" width="700px"/>
+</div>
+
+### 数学公式检测（MFD）
+
+MFD 模型检测图片中包含的数学公式，其中行内的公式检测为 `embedding` 类别，独立行的公式检测为 `isolated`。模型训练使用了英文 [IBEM](https://zenodo.org/record/4757865) 和中文 [CnMFD_Dataset](https://github.com/breezedeus/CnMFD_Dataset) 两个数据集。
+
+<div align="center">
+  <img src="./examples/mfd/out-zh4.jpg" alt="中文MFD效果" width="700px"/>
+</div>  
+<div align="center">
+  <img src="./examples/mfd/out-zh5.jpg" alt="中文MFD效果" width="700px"/>
+</div>
+<div align="center">
+  <img src="./examples/mfd/out-en2.jpg" alt="英文MFD效果" width="700px"/>
+</div> 
+
+
+### 版面分析（Layout Analysis）
+
+版面分析模型识别图片中的不同排版元素。模型训练使用的是 [CDLA](https://github.com/buptlihang/CDLA) 数据集。可识别以下10中版面元素：
+
+|正文|标题|图片|图片标题|表格|表格标题|页眉|页脚|注释|公式|
+|---|---|---|---|---|---|---|---|---|---|
+|Text|Title|Figure|Figure caption|Table|Table caption|Header|Footer|Reference|Equation|
+
+<div align="center">
+  <img src="./examples/layout/out-zh.jpg" alt="版面分析效果" width="700px"/>
+</div>  
+
+
+## 安装
+
+嗯，顺利的话很简单（bless）。
+
+```bash
+pip install cnstd
+```
+
+安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
+
+```bash
+pip install cnstd -i https://pypi.doubanio.com/simple
+```
+
+【注意】：
+
+* 请使用 **Python3** (3.6以及之后版本应该都行)，没测过Python2下是否ok。
+* 依赖 **opencv**，所以可能需要额外安装opencv。
+
+## 已有STD模型
+
+CnSTD 从 **V1.2** 开始，可直接使用的模型包含两类：1）CnSTD 自己训练的模型，通常会包含 PyTorch 和 ONNX 版本；2）从其他ocr引擎搬运过来的训练好的外部模型，ONNX化后用于 CnSTD 中。
+
+直接使用的模型都放在 [**cnstd-cnocr-models**](https://huggingface.co/breezedeus/cnstd-cnocr-models) 项目中，可免费下载使用。
+
+### 1. CnSTD 自己训练的模型
+
+当前版本（Since **V1.1.0**）的文字检测模型使用的是 [**DBNet**](https://github.com/MhLiao/DB)，相较于 V0.1 使用的 [PSENet](https://github.com/whai362/PSENet) 模型， DBNet 的检测耗时几乎下降了一个量级，同时检测精度也得到了极大的提升。
+
+目前包含以下已训练好的模型：
+
+| 模型名称                       | 参数规模      | 模型文件大小    | 测试集精度（IoU） | 平均推断耗时<br />（秒/张） | 下载方式                                                      |
+| -------------------------- | --------- | --------- | ---------- | ----------------- | --------------------------------------------------------- |
+| db_resnet34                | 22.5 M    | 86 M      | **0.7322** | 3.11              | 自动                                                        |
+| db_resnet18                | 12.3 M    | 47 M      | 0.7294     | 1.93              | 自动                                                        |
+| db_mobilenet_v3            | 4.2 M     | 16 M      | **0.7269** | 1.76              | 自动                                                        |
+| db_mobilenet_v3_small      | 2.0 M     | 7.9 M     | 0.7054     | 1.24              | 自动                                                        |
+| db_shufflenet_v2           | 4.7 M     | 18 M      | 0.7238     | 1.73              | 自动                                                        |
+| **db_shufflenet_v2_small** | 3.0 M     | 12 M      | 0.7190     | 1.29              | 自动                                                        |
+| db_shufflenet_v2_tiny      | **1.9 M** | **7.5 M** | **0.7172** | **1.14**          | [下载链接](https://mp.weixin.qq.com/s/fHPNoGyo72EFApVhEgR6Nw) |
+
+> 上表耗时基于本地 Mac 获得，绝对值无太大参考价值，相对值可供参考。IoU的计算方式经过调整，仅相对值可供参考。
+
+相对于两个基于 **ResNet** 的模型，基于 **MobileNet** 和 **ShuffleNet** 的模型体积更小，速度更快，建议在轻量级场景使用。
+
+### 2. 外部模型
+
+以下模型是 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR) 中模型的 **ONNX** 版本，所以不会依赖 **PaddlePaddle** 相关工具包，故而也不支持基于这些模型在自己的领域数据上继续精调模型。这些模型支持检测**竖排文字**。
+
+| `model_name`    | PyTorch 版本 | ONNX 版本 | 支持检测的语言    | 模型文件大小 |
+| --------------- | ---------- | ------- | ---------- | ------ |
+| ch_PP-OCRv3_det | X          | √       | 简体中问、英文、数字 | 2.3 M  |
+| ch_PP-OCRv2_det | X          | √       | 简体中问、英文、数字 | 2.2 M  |
+| en_PP-OCRv3_det | X          | √       | **英文**、数字  | 2.3 M  |
+
+更多模型可参考 [PaddleOCR/models_list.md](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/models_list.md) 。如有其他外语（如日、韩等）检测需求，可在 **知识星球** [**CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) 中向作者提出建议。
+
+## 使用方法
+
+首次使用 **CnSTD** 时，系统会自动下载zip格式的模型压缩文件，并存放于 `~/.cnstd`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\cnstd`）。下载速度超快。下载后的zip文件代码会自动对其解压，然后把解压后的模型相关目录放于`~/.cnstd/1.2`目录中。
+
+如果系统无法自动成功下载zip文件，则需要手动从 [百度云盘](https://pan.baidu.com/s/1zDMzArCDrrXHWL0AWxwYQQ?pwd=nstd)（提取码为 `nstd`）下载对应的zip文件并把它存放于 `~/.cnstd/1.2`（Windows下为 `C:\Users\<username>\AppData\Roaming\cnstd\1.2`）目录中。模型也可从 **[cnstd-cnocr-models](https://huggingface.co/breezedeus/cnstd-cnocr-models)** 中下载。放置好zip文件后，后面的事代码就会自动执行了。
+
+### 场景文字检测（STD）
+
+使用类 `CnStd` 进行场景文字的检测。类 `CnStd` 的初始化函数如下：
+
+```python
+class CnStd(object):
+    """
+    场景文字检测器（Scene Text Detection）。虽然名字中有个"Cn"（Chinese），但其实也可以轻松识别英文的。
+    """
+
+    def __init__(
+        self,
+        model_name: str = 'ch_PP-OCRv3_det',
+        *,
+        auto_rotate_whole_image: bool = False,
+        rotated_bbox: bool = True,
+        context: str = 'cpu',
+        model_fp: Optional[str] = None,
+        model_backend: str = 'onnx',  # ['pytorch', 'onnx']
+        root: Union[str, Path] = data_dir(),
+        use_angle_clf: bool = False,
+        angle_clf_configs: Optional[dict] = None,
+        **kwargs,
+    ):
+```
+
+其中的几个参数含义如下：
+
+* `model_name`:  模型名称，即前面模型表格第一列中的值。默认为 **ch_PP-OCRv3_det** 。
+
+* `auto_rotate_whole_image`:  是否自动对整张图片进行旋转调整。默认为`False`。
+
+* `rotated_bbox`:  是否支持检测带角度的文本框；默认为 `True`，表示支持；取值为 `False` 时，只检测水平或垂直的文本。
+
+* `context`：预测使用的机器资源，可取值为字符串`cpu`、`gpu`、`cuda:0`。
+
+* `model_fp`:  如果不使用系统自带的模型，可以通过此参数直接指定所使用的模型文件（`.ckpt`文件）。
+
+* `model_backend` (str): 'pytorch', or 'onnx'。表明预测时是使用 PyTorch 版本模型，还是使用 ONNX 版本模型。  同样的模型，ONNX 版本的预测速度一般是 PyTorch 版本的2倍左右。默认为 `onnx`。
+
+* `root`: 模型文件所在的根目录。
+  
+  * Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/db_shufflenet_v2_small`。
+  * Windows下默认值为 `C:\Users\<username>\AppData\Roaming\cnstd`。
+
+* `use_angle_clf` (bool): 对于检测出的文本框，是否使用角度分类模型进行调整（检测出的文本框可能会存在倒转180度的情况）。默认为 `False`
+
+* `angle_clf_configs` (dict): 角度分类模型对应的参数取值，主要包含以下值：
+  
+  - `model_name`: 模型名称。默认为 'ch_ppocr_mobile_v2.0_cls'
+  - `model_fp`: 如果不使用系统自带的模型，可以通过此参数直接指定所使用的模型文件（'.onnx' 文件）。默认为 `None`。具体可参考类 `AngleClassifier` 的说明
+
+每个参数都有默认取值，所以可以不传入任何参数值进行初始化：`std = CnStd()`。
+
+文本检测使用类`CnOcr`的函数 **`detect()`**，以下是详细说明：
+
+#### 类函数`CnStd.detect()`
+
+```python
+    def detect(
+        self,
+        img_list: Union[
+            str,
+            Path,
+            Image.Image,
+            np.ndarray,
+            List[Union[str, Path, Image.Image, np.ndarray]],
+        ],
+        resized_shape: Union[int, Tuple[int, int]] = (768, 768),
+        preserve_aspect_ratio: bool = True,
+        min_box_size: int = 8,
+        box_score_thresh: float = 0.3,
+        batch_size: int = 20,
+        **kwargs,
+    ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
+```
+
+**函数说明**：
+
+函数输入参数包括：
+
+- `img_list`: 支持对单个图片或者多个图片（列表）的检测。每个值可以是图片路径，或者已经读取进来 `PIL.Image.Image` 或 `np.ndarray`,  格式应该是 `RGB` 3 通道，shape: `(height, width, 3)`, 取值范围：`[0, 255]`。
+
+- `resized_shape`: `int` or `tuple`, `tuple` 含义为 `(height, width)`, `int` 则表示高宽都为此值；  
+   检测前，先把原始图片resize到接近此大小（只是接近，未必相等）。默认为 `(768, 768)`。
+  
+  > **Note** **（注意）**
+  > 这个取值对检测结果的影响较大，可以针对自己的应用多尝试几组值，再选出最优值。例如 `(512, 768)`, `(768, 768)`, `(768, 1024)`等。
+
+- `preserve_aspect_ratio`: 对原始图片 resize 时是否保持高宽比不变。默认为 `True`。
+
+- `min_box_size`: 过滤掉高度或者宽度小于此值的文本框。默认为 `8`，也即高或者宽小于 `8` 的文本框会被过滤去掉。
+
+- `box_score_thresh`: 过滤掉得分低于此值的文本框。默认为 `0.3`。
+
+- `batch_size`: 待处理图片很多时，需要分批处理，每批图片的数量由此参数指定。默认为 `20`。
+
+- `kwargs`: 保留参数，目前未被使用。
+
+函数输出类型为`list`，其中每个元素是一个字典，对应一张图片的检测结果。字典中包含以下 `keys`：
+
+- `rotated_angle`: `float`, 整张图片旋转的角度。只有 `auto_rotate_whole_image==True` 才可能非 `0`。
+
+- `detected_texts`: `list`, 每个元素存储了检测出的一个框的信息，使用词典记录，包括以下几个值：
+  
+  - `box`：检测出的文字对应的矩形框；`np.ndarray`, shape: `(4, 2)`，对应 box 4个点的坐标值 `(x, y)`;
+  
+  - `score`：得分；`float` 类型；分数越高表示越可靠；
+  
+  - `croppped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
+  
+  - 示例:
+    
+    ```python
+      [{'box': array([[416,  77],
+                      [486,  13],
+                      [800, 325],
+                      [730, 390]], dtype=int32),
+        'score': 1.0, 
+        'cropped_img': array([[[25, 20, 24],
+                               [26, 21, 25],
+                               [25, 20, 24],
+                              ...,
+                               [11, 11, 13],
+                               [11, 11, 13],
+                               [11, 11, 13]]], dtype=uint8)},
+       ...
+      ]
+    ```
+
+#### 调用示例
+
+```python
+from cnstd import CnStd
+std = CnStd()
+box_info_list = std.detect('examples/taobao.jpg')
+```
+
+或：
+
+```python
+from PIL import Image
+from cnstd import CnStd
+
+std = CnStd()
+img_fp = 'examples/taobao.jpg'
+img = Image.open(img_fp)
+box_infos = std.detect(img)
+```
+
+### 识别检测框中的文字（OCR）
+
+上面示例识别结果中"cropped_img"对应的值可以直接交由 **[cnocr](https://github.com/breezedeus/cnocr)** 中的 **`CnOcr`** 进行文字识别。如上例可以结合  **`CnOcr`** 进行文字识别：
+
+```python
+from cnstd import CnStd
+from cnocr import CnOcr
+
+std = CnStd()
+cn_ocr = CnOcr()
+
+box_infos = std.detect('examples/taobao.jpg')
+
+for box_info in box_infos['detected_texts']:
+    cropped_img = box_info['cropped_img']
+    ocr_res = cn_ocr.ocr_for_single_line(cropped_img)
+    print('ocr result: %s' % str(ocr_res))
+```
+
+注：运行上面示例需要先安装  **[cnocr](https://github.com/breezedeus/cnocr)** ：
+
+```bash
+pip install cnocr
+```
+
+
+
+### 数学公式检测（MFD）与 版面分析（Layout Analysis）
+
+数学公式检测（MFD）与 版面分析（Layout Analysis）都是检测图片中感兴趣的元素，它们使用的都是基于YOLOv7的检测架构，在CnSTD都来源于相同的类 `LayoutAnalyzer`，差别只是训练模型使用的数据不同。
+
+> 这两个模型的训练代码在 [yolov7](https://github.com/breezedeus/yolov7) 中（Forked from [WongKinYiu/yolov7](https://github.com/WongKinYiu/yolov7)，感谢原作者。）
+
+
+
+类 `LayoutAnalyzer` 的初始化函数如下：
+
+```python
+class LayoutAnalyzer(object):
+    def __init__(
+        self,
+        model_name: str = 'mfd',  # 'layout' or 'mfd'
+        *,
+        model_type: str = 'yolov7_tiny',
+        model_backend: str = 'pytorch',
+        model_fp: Optional[str] = None,
+        root: Union[str, Path] = data_dir(),
+        device: str = 'cpu',
+        **kwargs,
+    ):
+```
+
+其中的参数含义如下：
+
+- `model_name`: 字符串类型，表示模型类型。可选值：'mfd' 表示数学公式检测；'layout' 表示版面分析。默认值：'mfd'
+
+- `model_type`: 字符串类型，表示模型类型。当前支持 'yolov7_tiny' 和 'yolov7'；默认值：'yolov7_tiny'。'yolov7' 模型暂不开源，当前仅开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
+
+- `model_backend`: 字符串类型，表示backend。当前仅支持: 'pytorch'；默认值：'pytorch'
+
+- `model_fp`: 字符串类型，表示模型文件的路径。默认值：`None`，表示使用默认的文件路径
+
+- `root`: 字符串或`Path`类型，表示模型文件所在的根目录。
+  - Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/analysis`
+  - Windows下默认值为 `C:/Users/<username>/AppData/Roaming/cnstd`。
+  
+- `device`: 字符串类型，表示运行模型的设备，可选值：'cpu' 或 'gpu'；默认值：'cpu'
+
+- `**kwargs`: 额外的参数。
+
+
+
+函数输出结果为一个`list`，其中每个元素表示识别出的版面中的一个元素，包含以下信息：
+
+* type: 版面元素对应的类型；可选值来自：`self.categories` ;
+* box: 版面元素对应的矩形框；`np.ndarray`, shape: (4, 2)，对应 box 4个点的坐标值 `(x, y)` ;
+* score: 得分，越高表示越可信 。
+
+
+
+#### 类函数`LayoutAnalyzer.analyze()`
+
+对指定图片（列表）进行版面分析。
+
+```python
+def analyze(
+    self,
+    img_list: Union[
+        str,
+        Path,
+        Image.Image,
+        np.ndarray,
+        List[Union[str, Path, Image.Image, np.ndarray]],
+    ],
+    resized_shape: Union[int, Tuple[int, int]] = 700,
+    box_margin: int = 2,
+    conf_threshold: float = 0.25,
+    iou_threshold: float = 0.45,
+) -> Union[List[Dict[str, Any]], List[List[Dict[str, Any]]]]:
+```
+
+
+
+**函数说明**：
+
+函数输入参数包括：
+
+* `img_list` (str or list): 待识别图片或图片列表；如果是 `np.ndarray`，则应该是shape为 `[H, W, 3]` 的 RGB 格式数组
+* `resized_shape` (int or tuple): (H, W); 把图片resize到此大小再做分析；默认值为 `700`
+* `box_margin` (int): 对识别出的内容框往外扩展的像素大小；默认值为 `2`
+* `conf_threshold` (float): 分数阈值；默认值为 `0.25`
+* `iou_threshold` (float): IOU阈值；默认值为 `0.45`
+* `**kwargs`: 额外的参数。
+
+
+
+#### 调用示例
+
+```python
+from cnstd import LayoutAnalyzer
+img_fp = 'examples/mfd/zh5.jpg'
+analyzer = LayoutAnalyzer('mfd')
+out = analyzer.analyze(img_fp, resized_shape=700)
+print(out)
+```
+
+
+
+
+
+### 脚本使用
+
+**cnstd** 包含了几个命令行工具，安装 **cnstd** 后即可使用。
+
+#### STD 预测单个文件或文件夹中所有图片
+
+使用命令 **`cnstd predict`** 预测单个文件或文件夹中所有图片，以下是使用说明：
+
+```bash
+(venv) ➜  cnstd git:(master) ✗ cnstd predict -h
+Usage: cnstd predict [OPTIONS]
+
+  预测单个文件，或者指定目录下的所有图片
+
+Options:
+  -m, --model-name [ch_PP-OCRv2_det|ch_PP-OCRv3_det|db_mobilenet_v3|db_mobilenet_v3_small|db_resnet18|db_resnet34|db_shufflenet_v2|db_shufflenet_v2_small|db_shufflenet_v2_tiny|en_PP-OCRv3_det]
+                                  模型名称。默认值为 db_shufflenet_v2_small
+  -b, --model-backend [pytorch|onnx]
+                                  模型类型。默认值为 `onnx`
+  -p, --pretrained-model-fp TEXT  使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型
+  -r, --rotated-bbox              是否检测带角度（非水平和垂直）的文本框。默认为 `True`
+  --resized-shape TEXT            格式："height,width";
+                                  预测时把图片resize到此大小再进行预测。两个值都需要是32的倍数。默认为
+                                  `768,768`
+
+  --box-score-thresh FLOAT        检测结果只保留分数大于此值的文本框。默认值为 `0.3`
+  --preserve-aspect-ratio BOOLEAN
+                                  resize时是否保留图片原始比例。默认值为 `True`
+  --context TEXT                  使用cpu还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`。默认为
+                                  `cpu`
+
+  -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹
+  -o, --output-dir TEXT           检测结果存放的文件夹。默认为 `./predictions`
+  -h, --help                      Show this message and exit.
+```
+
+例如可以使用以下命令对图片 `examples/taobao.jpg`进行检测，并把检测结果存放在目录 `outputs`中：
+
+```bash
+cnstd predict -i examples/taobao.jpg -o outputs
+```
+
+具体使用也可参考文件 [Makefile](./Makefile) 。
+
+
+
+#### MFD or Layout Analysis 预测单个文件
+
+使用命令 **`cnstd analyze`** 获得单个文件的 MFD 或者 Layout Analysis 结果，以下是使用说明：
+
+```bash
+(venv) ➜  cnstd git:(master) ✗ cnstd analyze -h
+Usage: cnstd analyze [OPTIONS]
+
+  对给定图片进行 MFD 或者 版面分析。
+
+Options:
+  -m, --model-name [mfd|layout]   模型类型。`mfd` 表示数学公式检测，`layout`
+                                  表示版面分析；默认为：`mfd`
+  -t, --model-type TEXT           模型类型。当前支持 [`yolov7_tiny`, `yolov7`]
+  -b, --model-backend [pytorch|onnx]
+                                  模型后端架构。当前仅支持 `pytorch`
+  -p, --model-fp TEXT             使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型
+  --device TEXT                   cuda device, i.e. 0 or 0,1,2,3 or cpu
+  -i, --img-fp TEXT               待分析的图片路径或图片目录
+  -o, --output-fp TEXT            分析结果输出的图片路径。默认为 `None`，会存储在当前文件夹，文件名称为输入文件名称
+                                  前面增加`out-`；如输入文件名为 `img.jpg`, 输出文件名即为 `out-
+                                  img.jpg`；如果输入为目录，则此路径也应该是一个目录，会将输出文件存储在此目录下
+  --resized-shape INTEGER         分析时把图片resize到此大小再进行。默认为 `700`
+  --conf-thresh FLOAT             Confidence Threshold。默认值为 `0.25`
+  --iou-thresh FLOAT              IOU threshold for NMS。默认值为 `0.45`
+  -h, --help                      Show this message and exit.
+```
+
+例如可以使用以下命令对图片 `examples/mfd/zh.jpg` 进行 MFD，并把检测结果存放在文件 `out-zh.jpg` 中：
+
+```bash
+(venv) ➜  cnstd analyze -m mfd --conf-thresh 0.25 --resized-shape 800 -i examples/mfd/zh.jpg -o out-zh.jpg
+```
+
+具体使用也可参考文件 [Makefile](./Makefile) 。
+
+#### 模型训练
+
+使用命令 **`cnstd train`**  训练文本检测模型，以下是使用说明：
+
+```bash
+(venv) ➜  cnstd git:(master) ✗ cnstd train -h
+Usage: cnstd train [OPTIONS]
+
+  训练文本检测模型
+
+Options:
+  -m, --model-name [db_resnet50|db_resnet34|db_resnet18|db_mobilenet_v3|db_mobilenet_v3_small|db_shufflenet_v2|db_shufflenet_v2_small|db_shufflenet_v2_tiny]
+                                  模型名称。默认值为 `db_shufflenet_v2_small`
+  -i, --index-dir TEXT            索引文件所在的文件夹，会读取文件夹中的 `train.tsv` 和 `dev.tsv` 文件
+                                  [required]
+
+  --train-config-fp TEXT          训练使用的json配置文件  [required]
+  -r, --resume-from-checkpoint TEXT
+                                  恢复此前中断的训练状态，继续训练
+  -p, --pretrained-model-fp TEXT  导入的训练好的模型，作为初始模型。优先级低于 "--restore-training-
+                                  fp"，当传入"--restore-training-fp"时，此传入失效
+
+  -h, --help                      Show this message and exit.
+```
+
+具体使用可参考文件 [Makefile](./Makefile) 。
+
+#### 模型转存
+
+训练好的模型会存储训练状态，使用命令 **`cnstd resave`**  去掉与预测无关的数据，降低模型大小。
+
+```bash
+(venv) ➜  cnstd git:(master) ✗ cnstd resave -h
+Usage: cnstd resave [OPTIONS]
+
+  训练好的模型会存储训练状态，使用此命令去掉预测时无关的数据，降低模型大小
+
+Options:
+  -i, --input-model-fp TEXT   输入的模型文件路径  [required]
+  -o, --output-model-fp TEXT  输出的模型文件路径  [required]
+  -h, --help                  Show this message and exit.
+```
+
+## 未来工作
+
+* [x] 进一步精简模型结构，降低模型大小
+* [x] PSENet速度上还是比较慢，尝试更快的STD算法
+* [x] 加入更多的训练数据
+* [x] 加入对外部模型的支持
+* [x] 加入数学公式检测（MFD）与 版面分析（Layout Analysis）模型
+* [ ] 加入对文档结构与表格的检测
+
+
+
+## 给作者来杯咖啡
+
+开源不易，如果此项目对您有帮助，可以考虑 [给作者来杯咖啡 ☕️](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
+
+---
+
+官方代码库：[https://github.com/breezedeus/cnstd](https://github.com/breezedeus/cnstd)。
```

### Comparing `cnstd-1.2.2/README.md` & `cnstd-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,26 @@
 ![last-releast](https://img.shields.io/github/release-date/breezedeus/cnstd?style=plastic)
 ![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnstd)
 [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
 
 </div>
 
 # CnSTD
+# Update 2023.06.30：发布 V1.2.3
 
+主要变更：
+* 修复了模型文件自动下载的功能。HuggingFace似乎对下载文件的逻辑做了调整，导致之前版本的自动下载失败，当前版本已修复。但由于HuggingFace国内被墙，国内下载仍需 **梯子（VPN）**。
+* 更新了各个依赖包的版本号。
 
-# Update 2023.02.19：发布 V1.2.2
+# Update 2023.06.20：
 
 主要变更：
-* MFD训练了参数更多精度更高的模型，供 [P2T网页版](https://p2t.behye.com) 使用。
-* 优化了检测出的boxes的排序算法，使得boxes的顺序更加符合人类的阅读习惯。
+* 基于新标注的数据，重新训练了 **MFD YoloV7** 模型，目前新模型已部署到 [P2T网页版](https://p2t.behye.com) 。具体说明见：[Pix2Text (P2T) 新版公式检测模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230613) 。
+* 之前的 MFD YoloV7 模型已开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
+* 增加了一些Label Studio相关的脚本，见 [scripts](scripts) 。如：利用 CnSTD 自带的 MFD 模型对目录中的图片进行公式检测后生成可导入到Label Studio中的JSON文件；以及，Label Studio标注后把导出的JSON文件转换成训练 MFD 模型所需的数据格式。注意，MFD 模型的训练代码在 [yolov7](https://github.com/breezedeus/yolov7) （`dev` branch）中。
 
 了解更多：[RELEASE.md](./RELEASE.md) 。
 
 ---
 
 
 
@@ -350,15 +355,15 @@
     ):
 ```
 
 其中的参数含义如下：
 
 - `model_name`: 字符串类型，表示模型类型。可选值：'mfd' 表示数学公式检测；'layout' 表示版面分析。默认值：'mfd'
 
-- `model_type`: 字符串类型，表示模型类型。当前支持 'yolov7_tiny' 和 'yolov7'；默认值：'yolov7_tiny'
+- `model_type`: 字符串类型，表示模型类型。当前支持 'yolov7_tiny' 和 'yolov7'；默认值：'yolov7_tiny'。'yolov7' 模型暂不开源，当前仅开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
 
 - `model_backend`: 字符串类型，表示backend。当前仅支持: 'pytorch'；默认值：'pytorch'
 
 - `model_fp`: 字符串类型，表示模型文件的路径。默认值：`None`，表示使用默认的文件路径
 
 - `root`: 字符串或`Path`类型，表示模型文件所在的根目录。
   - Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/analysis`
```

### Comparing `cnstd-1.2.2/cnstd/__init__.py` & `cnstd-1.2.3/cnstd/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/__version__.py` & `cnstd-1.2.3/cnstd/datasets/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-__version__ = '1.2.2'
+from .dataset import StdDataset, StdDataModule
```

### Comparing `cnstd-1.2.2/cnstd/app.py` & `cnstd-1.2.3/cnstd/app.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/cli.py` & `cnstd-1.2.3/cnstd/cli.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/cn_std.py` & `cnstd-1.2.3/cnstd/cn_std.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/consts.py` & `cnstd-1.2.3/cnstd/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-# Copyright (C) 2021, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2021-2023, [Breezedeus](https://github.com/breezedeus).
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -107,18 +107,24 @@
         'fpn_layers': ['maxpool', 'stage2', 'stage3', 'stage4'],
         'fpn_channels': [24, 116, 232, 464],
         'input_shape': (3, 768, 768),
         'url': None,
     },
 }
 
-ROOT_URL = (
-    'https://huggingface.co/breezedeus/cnstd-cnocr-models/resolve/main/models/cnstd/%s/'
-    % MODEL_VERSION
-)
+HF_HUB_REPO_ID = "breezedeus/cnstd-cnocr-models"
+HF_HUB_SUBFOLDER = "models/cnstd/%s" % MODEL_VERSION
+
+
+def format_hf_hub_url(url: str) -> dict:
+    return {
+        'repo_id': HF_HUB_REPO_ID,
+        'subfolder': HF_HUB_SUBFOLDER,
+        'filename': url,
+    }
 
 
 class AvailableModels(object):
     CNSTD_SPACE = '__cnstd__'
 
     # name: (epochs, url)
     # 免费模型
@@ -212,43 +218,43 @@
 
     def get_epoch(self, model_name, model_backend) -> Optional[int]:
         return self.get_value(model_name, model_backend, 'model_epoch')
 
     def get_fpn_type(self, model_name, model_backend) -> Optional[int]:
         return self.get_value(model_name, model_backend, 'fpn_type')
 
-    def get_url(self, model_name, model_backend) -> Optional[str]:
+    def get_url(self, model_name, model_backend) -> Optional[dict]:
         url = self.get_value(model_name, model_backend, 'url')
         if url:
-            url = ROOT_URL + url
+            url = format_hf_hub_url(url)
 
         return url
 
 
 AVAILABLE_MODELS = AvailableModels()
 
 ANGLE_CLF_SPACE = 'angle_clf'
 ANGLE_CLF_MODELS = {
     ('ch_ppocr_mobile_v2.0_cls', 'onnx'): {
-        'url': ROOT_URL + 'ch_ppocr_mobile_v2.0_cls_infer-onnx.zip'
+        'url': format_hf_hub_url('ch_ppocr_mobile_v2.0_cls_infer-onnx.zip')
     }
 }
 
 ANALYSIS_SPACE = 'analysis'
 ANALYSIS_MODELS = {
     'layout': {
         ('yolov7_tiny', 'pytorch'): {
-            'url': ROOT_URL + 'yolov7_tiny_layout-pytorch.zip',
+            'url': format_hf_hub_url('yolov7_tiny_layout-pytorch.zip'),
             'arch_yaml': Path(__file__).parent / 'yolov7' / 'yolov7-tiny-layout.yaml',
         }
     },
     'mfd': {
         ('yolov7_tiny', 'pytorch'): {
-            'url': ROOT_URL + 'yolov7_tiny_mfd-pytorch.zip',
+            'url': format_hf_hub_url('yolov7_tiny_mfd-pytorch.zip'),
             'arch_yaml': Path(__file__).parent / 'yolov7' / 'yolov7-tiny-mfd.yaml',
         },
         ('yolov7', 'pytorch'): {
-            'url': ROOT_URL + 'yolov7_mfd-pytorch.zip',
+            'url': format_hf_hub_url('yolov7_mfd-pytorch.zip'),
             'arch_yaml': Path(__file__).parent / 'yolov7' / 'yolov7-mfd.yaml',
-        }
+        },
     },
 }
```

### Comparing `cnstd-1.2.2/cnstd/datasets/__init__.py` & `cnstd-1.2.3/cnstd/yolov7/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-# Copyright (C) 2021, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2022, [Breezedeus](https://github.com/breezedeus).
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -13,8 +13,7 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-from .dataset import StdDataset, StdDataModule
```

### Comparing `cnstd-1.2.2/cnstd/datasets/dataset.py` & `cnstd-1.2.3/cnstd/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/datasets/util.py` & `cnstd-1.2.3/cnstd/datasets/util.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/detector.py` & `cnstd-1.2.3/cnstd/detector.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/lr_scheduler.py` & `cnstd-1.2.3/cnstd/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/model/__init__.py` & `cnstd-1.2.3/cnstd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/model/base.py` & `cnstd-1.2.3/cnstd/model/base.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/model/core.py` & `cnstd-1.2.3/cnstd/model/core.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/model/dbnet.py` & `cnstd-1.2.3/cnstd/model/dbnet.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/model/fpn.py` & `cnstd-1.2.3/cnstd/model/fpn.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/__init__.py` & `cnstd-1.2.3/cnstd/ppocr/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/angle_classifier.py` & `cnstd-1.2.3/cnstd/ppocr/angle_classifier.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/consts.py` & `cnstd-1.2.3/cnstd/ppocr/consts.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/img_operators.py` & `cnstd-1.2.3/cnstd/ppocr/img_operators.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/opt_utils.py` & `cnstd-1.2.3/cnstd/ppocr/opt_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/__init__.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/cls_postprocess.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/cls_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/db_postprocess.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/east_postprocess.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/east_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/locality_aware_nms.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/locality_aware_nms.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/pg_postprocess.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/pg_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/__init__.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/rec_postprocess.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/postprocess/sast_postprocess.py` & `cnstd-1.2.3/cnstd/ppocr/postprocess/sast_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/pp_detector.py` & `cnstd-1.2.3/cnstd/ppocr/pp_detector.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/predict_rec.py` & `cnstd-1.2.3/cnstd/ppocr/predict_rec.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/predict_system.py` & `cnstd-1.2.3/cnstd/ppocr/predict_system.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/ppocr/utility.py` & `cnstd-1.2.3/cnstd/ppocr/utility.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/trainer.py` & `cnstd-1.2.3/cnstd/trainer.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/transforms/__init__.py` & `cnstd-1.2.3/cnstd/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/transforms/base.py` & `cnstd-1.2.3/cnstd/transforms/base.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/transforms/process_data.py` & `cnstd-1.2.3/cnstd/transforms/process_data.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/transforms/random_crop.py` & `cnstd-1.2.3/cnstd/transforms/random_crop.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/transforms/resize.py` & `cnstd-1.2.3/cnstd/transforms/resize.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/transforms/utils.py` & `cnstd-1.2.3/cnstd/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/utils/__init__.py` & `cnstd-1.2.3/cnstd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/utils/_utils.py` & `cnstd-1.2.3/cnstd/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/utils/common_types.py` & `cnstd-1.2.3/cnstd/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/utils/geometry.py` & `cnstd-1.2.3/cnstd/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/utils/metrics.py` & `cnstd-1.2.3/cnstd/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/utils/repr.py` & `cnstd-1.2.3/cnstd/utils/repr.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/utils/utils.py` & `cnstd-1.2.3/cnstd/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-# Copyright (C) 2021, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2021-2023, [Breezedeus](https://github.com/breezedeus).
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -22,20 +22,23 @@
 import requests
 from pathlib import Path
 from typing import Tuple, Union, List, Dict, Any
 import logging
 import platform
 import zipfile
 from functools import cmp_to_key
+import shutil
+import tempfile
 
 from tqdm import tqdm
 import cv2
 import numpy as np
-from PIL import Image
+from PIL import Image, ImageOps
 import torch
+from huggingface_hub import hf_hub_download
 
 from ..consts import MODEL_VERSION, MODEL_CONFIGS, AVAILABLE_MODELS
 
 
 fmt = '[%(levelname)s %(asctime)s %(funcName)s:%(lineno)d] %(' 'message)s '
 logging.basicConfig(format=fmt)
 logging.captureWarnings(True)
@@ -126,109 +129,101 @@
 
     sha1_file = sha1.hexdigest()
     l = min(len(sha1_file), len(sha1_hash))
     return sha1.hexdigest()[0:l] == sha1_hash[0:l]
 
 
 def download(url, path=None, overwrite=False, sha1_hash=None):
-    """Download an given URL
+    """Download a given URL
     Parameters
     ----------
-    url : str
-        URL to download
+    url : dict, url for downloading the model, with keys:
+            repo_id, subfolder, filename
     path : str, optional
-        Destination path to store downloaded file. By default stores to the
+        Destination path to store downloaded file. By default, stores to the
         current directory with same name as in url.
     overwrite : bool, optional
         Whether to overwrite destination file if already exists.
     sha1_hash : str, optional
         Expected sha1 hash in hexadecimal digits. Will ignore existing file when hash is specified
         but doesn't match.
     Returns
     -------
     str
         The file path of the downloaded file.
     """
     if path is None:
-        fname = url.split('/')[-1]
+        fname = url['filename']
     else:
         path = os.path.expanduser(path)
         if os.path.isdir(path):
-            fname = os.path.join(path, url.split('/')[-1])
+            fname = os.path.join(path, url['filename'])
         else:
             fname = path
 
     if (
         overwrite
         or not os.path.exists(fname)
         or (sha1_hash and not check_sha1(fname, sha1_hash))
     ):
         dirname = os.path.dirname(os.path.abspath(os.path.expanduser(fname)))
         if not os.path.exists(dirname):
             os.makedirs(dirname)
 
         logger.info('Downloading %s from %s...' % (fname, url))
-        r = requests.get(url, stream=True)
-        if r.status_code != 200:
-            raise RuntimeError(
-                'Failed downloading url %s. Probably because this model is not free anymore.'
-                % url
-            )
-        total_length = r.headers.get('content-length')
-        with open(fname, 'wb') as f:
-            if total_length is None:  # no content length header
-                for chunk in r.iter_content(chunk_size=1024):
-                    if chunk:  # filter out keep-alive new chunks
-                        f.write(chunk)
-            else:
-                total_length = int(total_length)
-                for chunk in tqdm(
-                    r.iter_content(chunk_size=1024),
-                    total=int(total_length / 1024.0 + 0.5),
-                    unit='KB',
-                    unit_scale=False,
-                    dynamic_ncols=True,
-                ):
-                    f.write(chunk)
-
-        if sha1_hash and not check_sha1(fname, sha1_hash):
-            raise UserWarning(
-                'File {} is downloaded but the content hash does not match. '
-                'The repo may be outdated or download may be incomplete. '
-                'If the "repo_url" is overridden, consider switching to '
-                'the default repo.'.format(fname)
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            local_path = hf_hub_download(
+                repo_id=url["repo_id"],
+                subfolder=url["subfolder"],
+                filename=url["filename"],
+                repo_type="model",
+                cache_dir=tmp_dir,
             )
+            shutil.copy2(local_path, fname)
 
     return fname
 
 
+class ModelDownloadingError(Exception):
+    pass
+
+
 def get_model_file(url, model_dir):
     r"""Return location for the downloaded models on local file system.
 
     This function will download from online model zoo when model cannot be found or has mismatch.
     The root directory will be created if it doesn't exist.
 
     Parameters
     ----------
-    url: str, url for downloading the model
+    url : dict, url for downloading the model, with keys:
+            repo_id, subfolder, filename
     model_dir : str, default $CNSTD_HOME
         Location for keeping the model parameters.
 
     Returns
     -------
     file_path
         Path to the requested pretrained model file.
     """
     model_dir = os.path.expanduser(model_dir)
     par_dir = os.path.dirname(model_dir)
     os.makedirs(par_dir, exist_ok=True)
 
-    zip_file_path = os.path.join(par_dir, os.path.basename(url))
+    zip_file_path = os.path.join(par_dir, url['filename'])
     if not os.path.exists(zip_file_path):
-        download(url, path=zip_file_path, overwrite=True)
+        try:
+            download(url, path=zip_file_path, overwrite=True)
+        except Exception as e:
+            logger.error(e)
+            message = f'Failed to download model: {url["filename"]}.'
+            message += '\n\tPlease open your VPN and try again. \n\t' \
+                       'If this error persists, please follow the instruction at ' \
+                       '[CnSTD/CnOCR Doc](https://www.breezedeus.com/cnocr) to manually download the model files.'
+            raise ModelDownloadingError(message)
     with zipfile.ZipFile(zip_file_path) as zf:
         zf.extractall(par_dir)
     os.remove(zip_file_path)
 
     return model_dir
 
 
@@ -276,15 +271,17 @@
     """
     img_mean = RGB_MEAN.reshape(3, 1, 1) if img.shape[0] == 3 else RGB_MEAN
     img = img * 255 + img_mean
     return img.clip(0, 255).astype(np.uint8)
 
 
 def read_img(img_fp) -> Image.Image:
-    return Image.open(img_fp)
+    img = Image.open(img_fp)
+    img = ImageOps.exif_transpose(img).convert('RGB')  # 识别旋转后的图片（pillow不会自动识别）
+    return img
 
 
 def pil_to_numpy(img: Image.Image) -> np.ndarray:
     """
 
     Args:
         img: an Image.Image from `read_img()`
```

### Comparing `cnstd-1.2.2/cnstd/yolov7/__init__.py` & `cnstd-1.2.3/cnstd/__version__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-# Copyright (C) 2022, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2021-2023, [Breezedeus](https://github.com/breezedeus).
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -13,7 +13,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
+__version__ = '1.2.3'
```

### Comparing `cnstd-1.2.2/cnstd/yolov7/autoanchor.py` & `cnstd-1.2.3/cnstd/yolov7/autoanchor.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/common.py` & `cnstd-1.2.3/cnstd/yolov7/common.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/consts.py` & `cnstd-1.2.3/cnstd/yolov7/consts.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/datasets.py` & `cnstd-1.2.3/cnstd/yolov7/datasets.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/experimental.py` & `cnstd-1.2.3/cnstd/yolov7/experimental.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/general.py` & `cnstd-1.2.3/cnstd/yolov7/general.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/layout_analyzer.py` & `cnstd-1.2.3/cnstd/yolov7/layout_analyzer.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/loss.py` & `cnstd-1.2.3/cnstd/yolov7/loss.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/metrics.py` & `cnstd-1.2.3/cnstd/yolov7/metrics.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/plots.py` & `cnstd-1.2.3/cnstd/yolov7/plots.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/torch_utils.py` & `cnstd-1.2.3/cnstd/yolov7/torch_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/yolo.py` & `cnstd-1.2.3/cnstd/yolov7/yolo.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/yolov7-mfd.yaml` & `cnstd-1.2.3/cnstd/yolov7/yolov7-mfd.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/yolov7-tiny-layout.yaml` & `cnstd-1.2.3/cnstd/yolov7/yolov7-tiny-layout.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd/yolov7/yolov7-tiny-mfd.yaml` & `cnstd-1.2.3/cnstd/yolov7/yolov7-tiny-mfd.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.2/cnstd.egg-info/PKG-INFO` & `cnstd-1.2.3/cnstd.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,597 +1,605 @@
 Metadata-Version: 2.1
 Name: cnstd
-Version: 1.2.2
-Summary: Python3 package for Chinese/English STR (Scene Text Recognition), with small pretrained models
+Version: 1.2.3
+Summary: Python3 package for Chinese/English Scene Text Detection (STD), Mathematical Formula Detection (MFD), and Layout Analysis, with free pretrained models
 Home-page: https://github.com/breezedeus/cnstd
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
-Description: <div align="center">
-        	<img src="./docs/logo.png" width="250px"/>
-          <div>&nbsp;</div>
-        
-        [![Downloads](https://static.pepy.tech/personalized-badge/cnstd?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnstd)
-        [![license](https://img.shields.io/github/license/breezedeus/cnstd)](./LICENSE)
-        [![PyPI version](https://badge.fury.io/py/cnstd.svg)](https://badge.fury.io/py/cnstd)
-        [![forks](https://img.shields.io/github/forks/breezedeus/cnstd)](https://img.shields.io/github/forks/breezedeus/cnstd)
-        [![stars](https://img.shields.io/github/stars/breezedeus/cnstd)](https://github.com/breezedeus/cnocr)
-        ![last-releast](https://img.shields.io/github/release-date/breezedeus/cnstd?style=plastic)
-        ![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnstd)
-        [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
-        
-        </div>
-        
-        # CnSTD
-        
-        
-        # Update 2023.02.19：发布 V1.2.2
-        
-        主要变更：
-        * MFD训练了参数更多精度更高的模型，供 [P2T网页版](https://p2t.behye.com) 使用。
-        * 优化了检测出的boxes的排序算法，使得boxes的顺序更加符合人类的阅读习惯。
-        
-        了解更多：[RELEASE.md](./RELEASE.md) 。
-        
-        ---
-        
-        
-        
-        **CnSTD** 是 **Python 3** 下的**场景文字检测**（**Scene Text Detection**，简称**STD**）工具包，支持**中文**、**英文**等语言的文字检测，自带了多个训练好的检测模型，安装后即可直接使用。**CnSTD** 自 **V1.2.1** 版本开始，加入了**数学公式检测**（**Mathematical Formula Detection**，简称**MFD**）模型，并提供训练好的模型可直接用于检测图片中包含的数学公式（**行内公式** `embedding` 与**独立行公式** `isolated` ）。
-        
-        欢迎扫码加入微信交流群：
-        
-        <div align="center">
-          <img src="https://huggingface.co/datasets/breezedeus/cnocr-wx-qr-code/resolve/main/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
-        </div>
-        
-        作者也维护 **知识星球** [**CnOCR/CnSTD/P2T私享群**](https://t.zsxq.com/FEYZRJQ)，欢迎加入。**知识星球私享群**会陆续发布一些CnOCR/CnSTD/P2T相关的私有资料，包括**更详细的训练教程**，**未公开的模型**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。
-        
-        自 **V1.0.0** 版本开始，**CnSTD** 从之前基于 MXNet 实现转为基于 **PyTorch** 实现。新模型的训练合并了  **ICPR MTWI 2018**、**ICDAR RCTW-17** 和 **ICDAR2019-LSVT** 三个数据集，包括了 **`46447`** 个训练样本，和 **`1534`** 个测试样本。
-        
-        相较于之前版本， 新版本的变化主要包括：
-        
-        * 加入了对 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR) 检测模型的支持；
-        * 部分调整了检测结果中 `box` 的表达方式，统一为 `4` 个点的坐标值；  
-        * 修复了已知bugs。
-        
-        如需要识别文本框中的文字，可以结合 **OCR** 工具包 **[cnocr](https://github.com/breezedeus/cnocr)** 一起使用。
-        
-        
-        ## 示例
-        
-        ### 场景文字检测（STD）
-        
-        <div align="center">
-          <img src="./docs/cases.png" alt="STD效果" width="700px"/>
-        </div>
-        
-        ### 数学公式检测（MFD）
-        
-        MFD 模型检测图片中包含的数学公式，其中行内的公式检测为 `embedding` 类别，独立行的公式检测为 `isolated`。模型训练使用了英文 [IBEM](https://zenodo.org/record/4757865) 和中文 [CnMFD_Dataset](https://github.com/breezedeus/CnMFD_Dataset) 两个数据集。
-        
-        <div align="center">
-          <img src="./examples/mfd/out-zh4.jpg" alt="中文MFD效果" width="700px"/>
-        </div>  
-        <div align="center">
-          <img src="./examples/mfd/out-zh5.jpg" alt="中文MFD效果" width="700px"/>
-        </div>
-        <div align="center">
-          <img src="./examples/mfd/out-en2.jpg" alt="英文MFD效果" width="700px"/>
-        </div> 
-        
-        
-        ### 版面分析（Layout Analysis）
-        
-        版面分析模型识别图片中的不同排版元素。模型训练使用的是 [CDLA](https://github.com/buptlihang/CDLA) 数据集。可识别以下10中版面元素：
-        
-        |正文|标题|图片|图片标题|表格|表格标题|页眉|页脚|注释|公式|
-        |---|---|---|---|---|---|---|---|---|---|
-        |Text|Title|Figure|Figure caption|Table|Table caption|Header|Footer|Reference|Equation|
-        
-        <div align="center">
-          <img src="./examples/layout/out-zh.jpg" alt="版面分析效果" width="700px"/>
-        </div>  
-        
-        
-        ## 安装
-        
-        嗯，顺利的话很简单（bless）。
-        
-        ```bash
-        pip install cnstd
-        ```
-        
-        安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
-        
-        ```bash
-        pip install cnstd -i https://pypi.doubanio.com/simple
-        ```
-        
-        【注意】：
-        
-        * 请使用 **Python3** (3.6以及之后版本应该都行)，没测过Python2下是否ok。
-        * 依赖 **opencv**，所以可能需要额外安装opencv。
-        
-        ## 已有STD模型
-        
-        CnSTD 从 **V1.2** 开始，可直接使用的模型包含两类：1）CnSTD 自己训练的模型，通常会包含 PyTorch 和 ONNX 版本；2）从其他ocr引擎搬运过来的训练好的外部模型，ONNX化后用于 CnSTD 中。
-        
-        直接使用的模型都放在 [**cnstd-cnocr-models**](https://huggingface.co/breezedeus/cnstd-cnocr-models) 项目中，可免费下载使用。
-        
-        ### 1. CnSTD 自己训练的模型
-        
-        当前版本（Since **V1.1.0**）的文字检测模型使用的是 [**DBNet**](https://github.com/MhLiao/DB)，相较于 V0.1 使用的 [PSENet](https://github.com/whai362/PSENet) 模型， DBNet 的检测耗时几乎下降了一个量级，同时检测精度也得到了极大的提升。
-        
-        目前包含以下已训练好的模型：
-        
-        | 模型名称                       | 参数规模      | 模型文件大小    | 测试集精度（IoU） | 平均推断耗时<br />（秒/张） | 下载方式                                                      |
-        | -------------------------- | --------- | --------- | ---------- | ----------------- | --------------------------------------------------------- |
-        | db_resnet34                | 22.5 M    | 86 M      | **0.7322** | 3.11              | 自动                                                        |
-        | db_resnet18                | 12.3 M    | 47 M      | 0.7294     | 1.93              | 自动                                                        |
-        | db_mobilenet_v3            | 4.2 M     | 16 M      | **0.7269** | 1.76              | 自动                                                        |
-        | db_mobilenet_v3_small      | 2.0 M     | 7.9 M     | 0.7054     | 1.24              | 自动                                                        |
-        | db_shufflenet_v2           | 4.7 M     | 18 M      | 0.7238     | 1.73              | 自动                                                        |
-        | **db_shufflenet_v2_small** | 3.0 M     | 12 M      | 0.7190     | 1.29              | 自动                                                        |
-        | db_shufflenet_v2_tiny      | **1.9 M** | **7.5 M** | **0.7172** | **1.14**          | [下载链接](https://mp.weixin.qq.com/s/fHPNoGyo72EFApVhEgR6Nw) |
-        
-        > 上表耗时基于本地 Mac 获得，绝对值无太大参考价值，相对值可供参考。IoU的计算方式经过调整，仅相对值可供参考。
-        
-        相对于两个基于 **ResNet** 的模型，基于 **MobileNet** 和 **ShuffleNet** 的模型体积更小，速度更快，建议在轻量级场景使用。
-        
-        ### 2. 外部模型
-        
-        以下模型是 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR) 中模型的 **ONNX** 版本，所以不会依赖 **PaddlePaddle** 相关工具包，故而也不支持基于这些模型在自己的领域数据上继续精调模型。这些模型支持检测**竖排文字**。
-        
-        | `model_name`    | PyTorch 版本 | ONNX 版本 | 支持检测的语言    | 模型文件大小 |
-        | --------------- | ---------- | ------- | ---------- | ------ |
-        | ch_PP-OCRv3_det | X          | √       | 简体中问、英文、数字 | 2.3 M  |
-        | ch_PP-OCRv2_det | X          | √       | 简体中问、英文、数字 | 2.2 M  |
-        | en_PP-OCRv3_det | X          | √       | **英文**、数字  | 2.3 M  |
-        
-        更多模型可参考 [PaddleOCR/models_list.md](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/models_list.md) 。如有其他外语（如日、韩等）检测需求，可在 **知识星球** [**CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) 中向作者提出建议。
-        
-        ## 使用方法
-        
-        首次使用 **CnSTD** 时，系统会自动下载zip格式的模型压缩文件，并存放于 `~/.cnstd`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\cnstd`）。下载速度超快。下载后的zip文件代码会自动对其解压，然后把解压后的模型相关目录放于`~/.cnstd/1.2`目录中。
-        
-        如果系统无法自动成功下载zip文件，则需要手动从 [百度云盘](https://pan.baidu.com/s/1zDMzArCDrrXHWL0AWxwYQQ?pwd=nstd)（提取码为 `nstd`）下载对应的zip文件并把它存放于 `~/.cnstd/1.2`（Windows下为 `C:\Users\<username>\AppData\Roaming\cnstd\1.2`）目录中。模型也可从 **[cnstd-cnocr-models](https://huggingface.co/breezedeus/cnstd-cnocr-models)** 中下载。放置好zip文件后，后面的事代码就会自动执行了。
-        
-        ### 场景文字检测（STD）
-        
-        使用类 `CnStd` 进行场景文字的检测。类 `CnStd` 的初始化函数如下：
-        
-        ```python
-        class CnStd(object):
-            """
-            场景文字检测器（Scene Text Detection）。虽然名字中有个"Cn"（Chinese），但其实也可以轻松识别英文的。
-            """
-        
-            def __init__(
-                self,
-                model_name: str = 'ch_PP-OCRv3_det',
-                *,
-                auto_rotate_whole_image: bool = False,
-                rotated_bbox: bool = True,
-                context: str = 'cpu',
-                model_fp: Optional[str] = None,
-                model_backend: str = 'onnx',  # ['pytorch', 'onnx']
-                root: Union[str, Path] = data_dir(),
-                use_angle_clf: bool = False,
-                angle_clf_configs: Optional[dict] = None,
-                **kwargs,
-            ):
-        ```
-        
-        其中的几个参数含义如下：
-        
-        * `model_name`:  模型名称，即前面模型表格第一列中的值。默认为 **ch_PP-OCRv3_det** 。
-        
-        * `auto_rotate_whole_image`:  是否自动对整张图片进行旋转调整。默认为`False`。
-        
-        * `rotated_bbox`:  是否支持检测带角度的文本框；默认为 `True`，表示支持；取值为 `False` 时，只检测水平或垂直的文本。
-        
-        * `context`：预测使用的机器资源，可取值为字符串`cpu`、`gpu`、`cuda:0`。
-        
-        * `model_fp`:  如果不使用系统自带的模型，可以通过此参数直接指定所使用的模型文件（`.ckpt`文件）。
-        
-        * `model_backend` (str): 'pytorch', or 'onnx'。表明预测时是使用 PyTorch 版本模型，还是使用 ONNX 版本模型。  同样的模型，ONNX 版本的预测速度一般是 PyTorch 版本的2倍左右。默认为 `onnx`。
-        
-        * `root`: 模型文件所在的根目录。
-          
-          * Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/db_shufflenet_v2_small`。
-          * Windows下默认值为 `C:\Users\<username>\AppData\Roaming\cnstd`。
-        
-        * `use_angle_clf` (bool): 对于检测出的文本框，是否使用角度分类模型进行调整（检测出的文本框可能会存在倒转180度的情况）。默认为 `False`
-        
-        * `angle_clf_configs` (dict): 角度分类模型对应的参数取值，主要包含以下值：
-          
-          - `model_name`: 模型名称。默认为 'ch_ppocr_mobile_v2.0_cls'
-          - `model_fp`: 如果不使用系统自带的模型，可以通过此参数直接指定所使用的模型文件（'.onnx' 文件）。默认为 `None`。具体可参考类 `AngleClassifier` 的说明
-        
-        每个参数都有默认取值，所以可以不传入任何参数值进行初始化：`std = CnStd()`。
-        
-        文本检测使用类`CnOcr`的函数 **`detect()`**，以下是详细说明：
-        
-        #### 类函数`CnStd.detect()`
-        
-        ```python
-            def detect(
-                self,
-                img_list: Union[
-                    str,
-                    Path,
-                    Image.Image,
-                    np.ndarray,
-                    List[Union[str, Path, Image.Image, np.ndarray]],
-                ],
-                resized_shape: Union[int, Tuple[int, int]] = (768, 768),
-                preserve_aspect_ratio: bool = True,
-                min_box_size: int = 8,
-                box_score_thresh: float = 0.3,
-                batch_size: int = 20,
-                **kwargs,
-            ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
-        ```
-        
-        **函数说明**：
-        
-        函数输入参数包括：
-        
-        - `img_list`: 支持对单个图片或者多个图片（列表）的检测。每个值可以是图片路径，或者已经读取进来 `PIL.Image.Image` 或 `np.ndarray`,  格式应该是 `RGB` 3 通道，shape: `(height, width, 3)`, 取值范围：`[0, 255]`。
-        
-        - `resized_shape`: `int` or `tuple`, `tuple` 含义为 `(height, width)`, `int` 则表示高宽都为此值；  
-           检测前，先把原始图片resize到接近此大小（只是接近，未必相等）。默认为 `(768, 768)`。
-          
-          > **Note** **（注意）**
-          > 这个取值对检测结果的影响较大，可以针对自己的应用多尝试几组值，再选出最优值。例如 `(512, 768)`, `(768, 768)`, `(768, 1024)`等。
-        
-        - `preserve_aspect_ratio`: 对原始图片 resize 时是否保持高宽比不变。默认为 `True`。
-        
-        - `min_box_size`: 过滤掉高度或者宽度小于此值的文本框。默认为 `8`，也即高或者宽小于 `8` 的文本框会被过滤去掉。
-        
-        - `box_score_thresh`: 过滤掉得分低于此值的文本框。默认为 `0.3`。
-        
-        - `batch_size`: 待处理图片很多时，需要分批处理，每批图片的数量由此参数指定。默认为 `20`。
-        
-        - `kwargs`: 保留参数，目前未被使用。
-        
-        函数输出类型为`list`，其中每个元素是一个字典，对应一张图片的检测结果。字典中包含以下 `keys`：
-        
-        - `rotated_angle`: `float`, 整张图片旋转的角度。只有 `auto_rotate_whole_image==True` 才可能非 `0`。
-        
-        - `detected_texts`: `list`, 每个元素存储了检测出的一个框的信息，使用词典记录，包括以下几个值：
-          
-          - `box`：检测出的文字对应的矩形框；`np.ndarray`, shape: `(4, 2)`，对应 box 4个点的坐标值 `(x, y)`;
-          
-          - `score`：得分；`float` 类型；分数越高表示越可靠；
-          
-          - `croppped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
-          
-          - 示例:
-            
-            ```python
-              [{'box': array([[416,  77],
-                              [486,  13],
-                              [800, 325],
-                              [730, 390]], dtype=int32),
-                'score': 1.0, 
-                'cropped_img': array([[[25, 20, 24],
-                                       [26, 21, 25],
-                                       [25, 20, 24],
-                                      ...,
-                                       [11, 11, 13],
-                                       [11, 11, 13],
-                                       [11, 11, 13]]], dtype=uint8)},
-               ...
-              ]
-            ```
-        
-        #### 调用示例
-        
-        ```python
-        from cnstd import CnStd
-        std = CnStd()
-        box_info_list = std.detect('examples/taobao.jpg')
-        ```
-        
-        或：
-        
-        ```python
-        from PIL import Image
-        from cnstd import CnStd
-        
-        std = CnStd()
-        img_fp = 'examples/taobao.jpg'
-        img = Image.open(img_fp)
-        box_infos = std.detect(img)
-        ```
-        
-        ### 识别检测框中的文字（OCR）
-        
-        上面示例识别结果中"cropped_img"对应的值可以直接交由 **[cnocr](https://github.com/breezedeus/cnocr)** 中的 **`CnOcr`** 进行文字识别。如上例可以结合  **`CnOcr`** 进行文字识别：
-        
-        ```python
-        from cnstd import CnStd
-        from cnocr import CnOcr
-        
-        std = CnStd()
-        cn_ocr = CnOcr()
-        
-        box_infos = std.detect('examples/taobao.jpg')
-        
-        for box_info in box_infos['detected_texts']:
-            cropped_img = box_info['cropped_img']
-            ocr_res = cn_ocr.ocr_for_single_line(cropped_img)
-            print('ocr result: %s' % str(ocr_res))
-        ```
-        
-        注：运行上面示例需要先安装  **[cnocr](https://github.com/breezedeus/cnocr)** ：
-        
-        ```bash
-        pip install cnocr
-        ```
-        
-        
-        
-        ### 数学公式检测（MFD）与 版面分析（Layout Analysis）
-        
-        数学公式检测（MFD）与 版面分析（Layout Analysis）都是检测图片中感兴趣的元素，它们使用的都是基于YOLOv7的检测架构，在CnSTD都来源于相同的类 `LayoutAnalyzer`，差别只是训练模型使用的数据不同。
-        
-        > 这两个模型的训练代码在 [yolov7](https://github.com/breezedeus/yolov7) 中（Forked from [WongKinYiu/yolov7](https://github.com/WongKinYiu/yolov7)，感谢原作者。）
-        
-        
-        
-        类 `LayoutAnalyzer` 的初始化函数如下：
-        
-        ```python
-        class LayoutAnalyzer(object):
-            def __init__(
-                self,
-                model_name: str = 'mfd',  # 'layout' or 'mfd'
-                *,
-                model_type: str = 'yolov7_tiny',
-                model_backend: str = 'pytorch',
-                model_fp: Optional[str] = None,
-                root: Union[str, Path] = data_dir(),
-                device: str = 'cpu',
-                **kwargs,
-            ):
-        ```
-        
-        其中的参数含义如下：
-        
-        - `model_name`: 字符串类型，表示模型类型。可选值：'mfd' 表示数学公式检测；'layout' 表示版面分析。默认值：'mfd'
-        
-        - `model_type`: 字符串类型，表示模型类型。当前支持 'yolov7_tiny' 和 'yolov7'；默认值：'yolov7_tiny'
-        
-        - `model_backend`: 字符串类型，表示backend。当前仅支持: 'pytorch'；默认值：'pytorch'
-        
-        - `model_fp`: 字符串类型，表示模型文件的路径。默认值：`None`，表示使用默认的文件路径
-        
-        - `root`: 字符串或`Path`类型，表示模型文件所在的根目录。
-          - Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/analysis`
-          - Windows下默认值为 `C:/Users/<username>/AppData/Roaming/cnstd`。
-          
-        - `device`: 字符串类型，表示运行模型的设备，可选值：'cpu' 或 'gpu'；默认值：'cpu'
-        
-        - `**kwargs`: 额外的参数。
-        
-        
-        
-        函数输出结果为一个`list`，其中每个元素表示识别出的版面中的一个元素，包含以下信息：
-        
-        * type: 版面元素对应的类型；可选值来自：`self.categories` ;
-        * box: 版面元素对应的矩形框；`np.ndarray`, shape: (4, 2)，对应 box 4个点的坐标值 `(x, y)` ;
-        * score: 得分，越高表示越可信 。
-        
-        
-        
-        #### 类函数`LayoutAnalyzer.analyze()`
-        
-        对指定图片（列表）进行版面分析。
-        
-        ```python
-        def analyze(
-            self,
-            img_list: Union[
-                str,
-                Path,
-                Image.Image,
-                np.ndarray,
-                List[Union[str, Path, Image.Image, np.ndarray]],
-            ],
-            resized_shape: Union[int, Tuple[int, int]] = 700,
-            box_margin: int = 2,
-            conf_threshold: float = 0.25,
-            iou_threshold: float = 0.45,
-        ) -> Union[List[Dict[str, Any]], List[List[Dict[str, Any]]]]:
-        ```
-        
-        
-        
-        **函数说明**：
-        
-        函数输入参数包括：
-        
-        * `img_list` (str or list): 待识别图片或图片列表；如果是 `np.ndarray`，则应该是shape为 `[H, W, 3]` 的 RGB 格式数组
-        * `resized_shape` (int or tuple): (H, W); 把图片resize到此大小再做分析；默认值为 `700`
-        * `box_margin` (int): 对识别出的内容框往外扩展的像素大小；默认值为 `2`
-        * `conf_threshold` (float): 分数阈值；默认值为 `0.25`
-        * `iou_threshold` (float): IOU阈值；默认值为 `0.45`
-        * `**kwargs`: 额外的参数。
-        
-        
-        
-        #### 调用示例
-        
-        ```python
-        from cnstd import LayoutAnalyzer
-        img_fp = 'examples/mfd/zh5.jpg'
-        analyzer = LayoutAnalyzer('mfd')
-        out = analyzer.analyze(img_fp, resized_shape=700)
-        print(out)
-        ```
-        
-        
-        
-        
-        
-        ### 脚本使用
-        
-        **cnstd** 包含了几个命令行工具，安装 **cnstd** 后即可使用。
-        
-        #### STD 预测单个文件或文件夹中所有图片
-        
-        使用命令 **`cnstd predict`** 预测单个文件或文件夹中所有图片，以下是使用说明：
-        
-        ```bash
-        (venv) ➜  cnstd git:(master) ✗ cnstd predict -h
-        Usage: cnstd predict [OPTIONS]
-        
-          预测单个文件，或者指定目录下的所有图片
-        
-        Options:
-          -m, --model-name [ch_PP-OCRv2_det|ch_PP-OCRv3_det|db_mobilenet_v3|db_mobilenet_v3_small|db_resnet18|db_resnet34|db_shufflenet_v2|db_shufflenet_v2_small|db_shufflenet_v2_tiny|en_PP-OCRv3_det]
-                                          模型名称。默认值为 db_shufflenet_v2_small
-          -b, --model-backend [pytorch|onnx]
-                                          模型类型。默认值为 `onnx`
-          -p, --pretrained-model-fp TEXT  使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型
-          -r, --rotated-bbox              是否检测带角度（非水平和垂直）的文本框。默认为 `True`
-          --resized-shape TEXT            格式："height,width";
-                                          预测时把图片resize到此大小再进行预测。两个值都需要是32的倍数。默认为
-                                          `768,768`
-        
-          --box-score-thresh FLOAT        检测结果只保留分数大于此值的文本框。默认值为 `0.3`
-          --preserve-aspect-ratio BOOLEAN
-                                          resize时是否保留图片原始比例。默认值为 `True`
-          --context TEXT                  使用cpu还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`。默认为
-                                          `cpu`
-        
-          -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹
-          -o, --output-dir TEXT           检测结果存放的文件夹。默认为 `./predictions`
-          -h, --help                      Show this message and exit.
-        ```
-        
-        例如可以使用以下命令对图片 `examples/taobao.jpg`进行检测，并把检测结果存放在目录 `outputs`中：
-        
-        ```bash
-        cnstd predict -i examples/taobao.jpg -o outputs
-        ```
-        
-        具体使用也可参考文件 [Makefile](./Makefile) 。
-        
-        
-        
-        #### MFD or Layout Analysis 预测单个文件
-        
-        使用命令 **`cnstd analyze`** 获得单个文件的 MFD 或者 Layout Analysis 结果，以下是使用说明：
-        
-        ```bash
-        (venv) ➜  cnstd git:(master) ✗ cnstd analyze -h
-        Usage: cnstd analyze [OPTIONS]
-        
-          对给定图片进行 MFD 或者 版面分析。
-        
-        Options:
-          -m, --model-name [mfd|layout]   模型类型。`mfd` 表示数学公式检测，`layout`
-                                          表示版面分析；默认为：`mfd`
-          -t, --model-type TEXT           模型类型。当前支持 [`yolov7_tiny`, `yolov7`]
-          -b, --model-backend [pytorch|onnx]
-                                          模型后端架构。当前仅支持 `pytorch`
-          -p, --model-fp TEXT             使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型
-          --device TEXT                   cuda device, i.e. 0 or 0,1,2,3 or cpu
-          -i, --img-fp TEXT               待分析的图片路径或图片目录
-          -o, --output-fp TEXT            分析结果输出的图片路径。默认为 `None`，会存储在当前文件夹，文件名称为输入文件名称
-                                          前面增加`out-`；如输入文件名为 `img.jpg`, 输出文件名即为 `out-
-                                          img.jpg`；如果输入为目录，则此路径也应该是一个目录，会将输出文件存储在此目录下
-          --resized-shape INTEGER         分析时把图片resize到此大小再进行。默认为 `700`
-          --conf-thresh FLOAT             Confidence Threshold。默认值为 `0.25`
-          --iou-thresh FLOAT              IOU threshold for NMS。默认值为 `0.45`
-          -h, --help                      Show this message and exit.
-        ```
-        
-        例如可以使用以下命令对图片 `examples/mfd/zh.jpg` 进行 MFD，并把检测结果存放在文件 `out-zh.jpg` 中：
-        
-        ```bash
-        (venv) ➜  cnstd analyze -m mfd --conf-thresh 0.25 --resized-shape 800 -i examples/mfd/zh.jpg -o out-zh.jpg
-        ```
-        
-        具体使用也可参考文件 [Makefile](./Makefile) 。
-        
-        #### 模型训练
-        
-        使用命令 **`cnstd train`**  训练文本检测模型，以下是使用说明：
-        
-        ```bash
-        (venv) ➜  cnstd git:(master) ✗ cnstd train -h
-        Usage: cnstd train [OPTIONS]
-        
-          训练文本检测模型
-        
-        Options:
-          -m, --model-name [db_resnet50|db_resnet34|db_resnet18|db_mobilenet_v3|db_mobilenet_v3_small|db_shufflenet_v2|db_shufflenet_v2_small|db_shufflenet_v2_tiny]
-                                          模型名称。默认值为 `db_shufflenet_v2_small`
-          -i, --index-dir TEXT            索引文件所在的文件夹，会读取文件夹中的 `train.tsv` 和 `dev.tsv` 文件
-                                          [required]
-        
-          --train-config-fp TEXT          训练使用的json配置文件  [required]
-          -r, --resume-from-checkpoint TEXT
-                                          恢复此前中断的训练状态，继续训练
-          -p, --pretrained-model-fp TEXT  导入的训练好的模型，作为初始模型。优先级低于 "--restore-training-
-                                          fp"，当传入"--restore-training-fp"时，此传入失效
-        
-          -h, --help                      Show this message and exit.
-        ```
-        
-        具体使用可参考文件 [Makefile](./Makefile) 。
-        
-        #### 模型转存
-        
-        训练好的模型会存储训练状态，使用命令 **`cnstd resave`**  去掉与预测无关的数据，降低模型大小。
-        
-        ```bash
-        (venv) ➜  cnstd git:(master) ✗ cnstd resave -h
-        Usage: cnstd resave [OPTIONS]
-        
-          训练好的模型会存储训练状态，使用此命令去掉预测时无关的数据，降低模型大小
-        
-        Options:
-          -i, --input-model-fp TEXT   输入的模型文件路径  [required]
-          -o, --output-model-fp TEXT  输出的模型文件路径  [required]
-          -h, --help                  Show this message and exit.
-        ```
-        
-        ## 未来工作
-        
-        * [x] 进一步精简模型结构，降低模型大小
-        * [x] PSENet速度上还是比较慢，尝试更快的STD算法
-        * [x] 加入更多的训练数据
-        * [x] 加入对外部模型的支持
-        * [x] 加入数学公式检测（MFD）与 版面分析（Layout Analysis）模型
-        * [ ] 加入对文档结构与表格的检测
-        
-        
-        
-        ## 给作者来杯咖啡
-        
-        开源不易，如果此项目对您有帮助，可以考虑 [给作者来杯咖啡 ☕️](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
-        
-        ---
-        
-        官方代码库：[https://github.com/breezedeus/cnstd](https://github.com/breezedeus/cnstd)。
 Platform: Mac
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+<div align="center">
+	<img src="./docs/logo.png" width="250px"/>
+  <div>&nbsp;</div>
+
+[![Downloads](https://static.pepy.tech/personalized-badge/cnstd?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnstd)
+[![license](https://img.shields.io/github/license/breezedeus/cnstd)](./LICENSE)
+[![PyPI version](https://badge.fury.io/py/cnstd.svg)](https://badge.fury.io/py/cnstd)
+[![forks](https://img.shields.io/github/forks/breezedeus/cnstd)](https://img.shields.io/github/forks/breezedeus/cnstd)
+[![stars](https://img.shields.io/github/stars/breezedeus/cnstd)](https://github.com/breezedeus/cnocr)
+![last-releast](https://img.shields.io/github/release-date/breezedeus/cnstd?style=plastic)
+![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnstd)
+[![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
+
+</div>
+
+# CnSTD
+# Update 2023.06.30：发布 V1.2.3
+
+主要变更：
+* 修复了模型文件自动下载的功能。HuggingFace似乎对下载文件的逻辑做了调整，导致之前版本的自动下载失败，当前版本已修复。但由于HuggingFace国内被墙，国内下载仍需 **梯子（VPN）**。
+* 更新了各个依赖包的版本号。
+
+# Update 2023.06.20：
+
+主要变更：
+* 基于新标注的数据，重新训练了 **MFD YoloV7** 模型，目前新模型已部署到 [P2T网页版](https://p2t.behye.com) 。具体说明见：[Pix2Text (P2T) 新版公式检测模型 | Breezedeus.com](https://www.breezedeus.com/article/p2t-mfd-20230613) 。
+* 之前的 MFD YoloV7 模型已开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
+* 增加了一些Label Studio相关的脚本，见 [scripts](scripts) 。如：利用 CnSTD 自带的 MFD 模型对目录中的图片进行公式检测后生成可导入到Label Studio中的JSON文件；以及，Label Studio标注后把导出的JSON文件转换成训练 MFD 模型所需的数据格式。注意，MFD 模型的训练代码在 [yolov7](https://github.com/breezedeus/yolov7) （`dev` branch）中。
+
+了解更多：[RELEASE.md](./RELEASE.md) 。
+
+---
+
+
+
+**CnSTD** 是 **Python 3** 下的**场景文字检测**（**Scene Text Detection**，简称**STD**）工具包，支持**中文**、**英文**等语言的文字检测，自带了多个训练好的检测模型，安装后即可直接使用。**CnSTD** 自 **V1.2.1** 版本开始，加入了**数学公式检测**（**Mathematical Formula Detection**，简称**MFD**）模型，并提供训练好的模型可直接用于检测图片中包含的数学公式（**行内公式** `embedding` 与**独立行公式** `isolated` ）。
+
+欢迎扫码加入微信交流群：
+
+<div align="center">
+  <img src="https://huggingface.co/datasets/breezedeus/cnocr-wx-qr-code/resolve/main/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
+</div>
+
+作者也维护 **知识星球** [**CnOCR/CnSTD/P2T私享群**](https://t.zsxq.com/FEYZRJQ)，欢迎加入。**知识星球私享群**会陆续发布一些CnOCR/CnSTD/P2T相关的私有资料，包括**更详细的训练教程**，**未公开的模型**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。
+
+自 **V1.0.0** 版本开始，**CnSTD** 从之前基于 MXNet 实现转为基于 **PyTorch** 实现。新模型的训练合并了  **ICPR MTWI 2018**、**ICDAR RCTW-17** 和 **ICDAR2019-LSVT** 三个数据集，包括了 **`46447`** 个训练样本，和 **`1534`** 个测试样本。
+
+相较于之前版本， 新版本的变化主要包括：
+
+* 加入了对 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR) 检测模型的支持；
+* 部分调整了检测结果中 `box` 的表达方式，统一为 `4` 个点的坐标值；  
+* 修复了已知bugs。
+
+如需要识别文本框中的文字，可以结合 **OCR** 工具包 **[cnocr](https://github.com/breezedeus/cnocr)** 一起使用。
+
+
+## 示例
+
+### 场景文字检测（STD）
+
+<div align="center">
+  <img src="./docs/cases.png" alt="STD效果" width="700px"/>
+</div>
+
+### 数学公式检测（MFD）
+
+MFD 模型检测图片中包含的数学公式，其中行内的公式检测为 `embedding` 类别，独立行的公式检测为 `isolated`。模型训练使用了英文 [IBEM](https://zenodo.org/record/4757865) 和中文 [CnMFD_Dataset](https://github.com/breezedeus/CnMFD_Dataset) 两个数据集。
+
+<div align="center">
+  <img src="./examples/mfd/out-zh4.jpg" alt="中文MFD效果" width="700px"/>
+</div>  
+<div align="center">
+  <img src="./examples/mfd/out-zh5.jpg" alt="中文MFD效果" width="700px"/>
+</div>
+<div align="center">
+  <img src="./examples/mfd/out-en2.jpg" alt="英文MFD效果" width="700px"/>
+</div> 
+
+
+### 版面分析（Layout Analysis）
+
+版面分析模型识别图片中的不同排版元素。模型训练使用的是 [CDLA](https://github.com/buptlihang/CDLA) 数据集。可识别以下10中版面元素：
+
+|正文|标题|图片|图片标题|表格|表格标题|页眉|页脚|注释|公式|
+|---|---|---|---|---|---|---|---|---|---|
+|Text|Title|Figure|Figure caption|Table|Table caption|Header|Footer|Reference|Equation|
+
+<div align="center">
+  <img src="./examples/layout/out-zh.jpg" alt="版面分析效果" width="700px"/>
+</div>  
+
+
+## 安装
+
+嗯，顺利的话很简单（bless）。
+
+```bash
+pip install cnstd
+```
+
+安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
+
+```bash
+pip install cnstd -i https://pypi.doubanio.com/simple
+```
+
+【注意】：
+
+* 请使用 **Python3** (3.6以及之后版本应该都行)，没测过Python2下是否ok。
+* 依赖 **opencv**，所以可能需要额外安装opencv。
+
+## 已有STD模型
+
+CnSTD 从 **V1.2** 开始，可直接使用的模型包含两类：1）CnSTD 自己训练的模型，通常会包含 PyTorch 和 ONNX 版本；2）从其他ocr引擎搬运过来的训练好的外部模型，ONNX化后用于 CnSTD 中。
+
+直接使用的模型都放在 [**cnstd-cnocr-models**](https://huggingface.co/breezedeus/cnstd-cnocr-models) 项目中，可免费下载使用。
+
+### 1. CnSTD 自己训练的模型
+
+当前版本（Since **V1.1.0**）的文字检测模型使用的是 [**DBNet**](https://github.com/MhLiao/DB)，相较于 V0.1 使用的 [PSENet](https://github.com/whai362/PSENet) 模型， DBNet 的检测耗时几乎下降了一个量级，同时检测精度也得到了极大的提升。
+
+目前包含以下已训练好的模型：
+
+| 模型名称                       | 参数规模      | 模型文件大小    | 测试集精度（IoU） | 平均推断耗时<br />（秒/张） | 下载方式                                                      |
+| -------------------------- | --------- | --------- | ---------- | ----------------- | --------------------------------------------------------- |
+| db_resnet34                | 22.5 M    | 86 M      | **0.7322** | 3.11              | 自动                                                        |
+| db_resnet18                | 12.3 M    | 47 M      | 0.7294     | 1.93              | 自动                                                        |
+| db_mobilenet_v3            | 4.2 M     | 16 M      | **0.7269** | 1.76              | 自动                                                        |
+| db_mobilenet_v3_small      | 2.0 M     | 7.9 M     | 0.7054     | 1.24              | 自动                                                        |
+| db_shufflenet_v2           | 4.7 M     | 18 M      | 0.7238     | 1.73              | 自动                                                        |
+| **db_shufflenet_v2_small** | 3.0 M     | 12 M      | 0.7190     | 1.29              | 自动                                                        |
+| db_shufflenet_v2_tiny      | **1.9 M** | **7.5 M** | **0.7172** | **1.14**          | [下载链接](https://mp.weixin.qq.com/s/fHPNoGyo72EFApVhEgR6Nw) |
+
+> 上表耗时基于本地 Mac 获得，绝对值无太大参考价值，相对值可供参考。IoU的计算方式经过调整，仅相对值可供参考。
+
+相对于两个基于 **ResNet** 的模型，基于 **MobileNet** 和 **ShuffleNet** 的模型体积更小，速度更快，建议在轻量级场景使用。
+
+### 2. 外部模型
+
+以下模型是 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR) 中模型的 **ONNX** 版本，所以不会依赖 **PaddlePaddle** 相关工具包，故而也不支持基于这些模型在自己的领域数据上继续精调模型。这些模型支持检测**竖排文字**。
+
+| `model_name`    | PyTorch 版本 | ONNX 版本 | 支持检测的语言    | 模型文件大小 |
+| --------------- | ---------- | ------- | ---------- | ------ |
+| ch_PP-OCRv3_det | X          | √       | 简体中问、英文、数字 | 2.3 M  |
+| ch_PP-OCRv2_det | X          | √       | 简体中问、英文、数字 | 2.2 M  |
+| en_PP-OCRv3_det | X          | √       | **英文**、数字  | 2.3 M  |
+
+更多模型可参考 [PaddleOCR/models_list.md](https://github.com/PaddlePaddle/PaddleOCR/blob/release%2F2.5/doc/doc_ch/models_list.md) 。如有其他外语（如日、韩等）检测需求，可在 **知识星球** [**CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) 中向作者提出建议。
+
+## 使用方法
+
+首次使用 **CnSTD** 时，系统会自动下载zip格式的模型压缩文件，并存放于 `~/.cnstd`目录（Windows下默认路径为 `C:\Users\<username>\AppData\Roaming\cnstd`）。下载速度超快。下载后的zip文件代码会自动对其解压，然后把解压后的模型相关目录放于`~/.cnstd/1.2`目录中。
+
+如果系统无法自动成功下载zip文件，则需要手动从 [百度云盘](https://pan.baidu.com/s/1zDMzArCDrrXHWL0AWxwYQQ?pwd=nstd)（提取码为 `nstd`）下载对应的zip文件并把它存放于 `~/.cnstd/1.2`（Windows下为 `C:\Users\<username>\AppData\Roaming\cnstd\1.2`）目录中。模型也可从 **[cnstd-cnocr-models](https://huggingface.co/breezedeus/cnstd-cnocr-models)** 中下载。放置好zip文件后，后面的事代码就会自动执行了。
+
+### 场景文字检测（STD）
+
+使用类 `CnStd` 进行场景文字的检测。类 `CnStd` 的初始化函数如下：
+
+```python
+class CnStd(object):
+    """
+    场景文字检测器（Scene Text Detection）。虽然名字中有个"Cn"（Chinese），但其实也可以轻松识别英文的。
+    """
+
+    def __init__(
+        self,
+        model_name: str = 'ch_PP-OCRv3_det',
+        *,
+        auto_rotate_whole_image: bool = False,
+        rotated_bbox: bool = True,
+        context: str = 'cpu',
+        model_fp: Optional[str] = None,
+        model_backend: str = 'onnx',  # ['pytorch', 'onnx']
+        root: Union[str, Path] = data_dir(),
+        use_angle_clf: bool = False,
+        angle_clf_configs: Optional[dict] = None,
+        **kwargs,
+    ):
+```
+
+其中的几个参数含义如下：
+
+* `model_name`:  模型名称，即前面模型表格第一列中的值。默认为 **ch_PP-OCRv3_det** 。
+
+* `auto_rotate_whole_image`:  是否自动对整张图片进行旋转调整。默认为`False`。
+
+* `rotated_bbox`:  是否支持检测带角度的文本框；默认为 `True`，表示支持；取值为 `False` 时，只检测水平或垂直的文本。
+
+* `context`：预测使用的机器资源，可取值为字符串`cpu`、`gpu`、`cuda:0`。
+
+* `model_fp`:  如果不使用系统自带的模型，可以通过此参数直接指定所使用的模型文件（`.ckpt`文件）。
+
+* `model_backend` (str): 'pytorch', or 'onnx'。表明预测时是使用 PyTorch 版本模型，还是使用 ONNX 版本模型。  同样的模型，ONNX 版本的预测速度一般是 PyTorch 版本的2倍左右。默认为 `onnx`。
+
+* `root`: 模型文件所在的根目录。
+  
+  * Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/db_shufflenet_v2_small`。
+  * Windows下默认值为 `C:\Users\<username>\AppData\Roaming\cnstd`。
+
+* `use_angle_clf` (bool): 对于检测出的文本框，是否使用角度分类模型进行调整（检测出的文本框可能会存在倒转180度的情况）。默认为 `False`
+
+* `angle_clf_configs` (dict): 角度分类模型对应的参数取值，主要包含以下值：
+  
+  - `model_name`: 模型名称。默认为 'ch_ppocr_mobile_v2.0_cls'
+  - `model_fp`: 如果不使用系统自带的模型，可以通过此参数直接指定所使用的模型文件（'.onnx' 文件）。默认为 `None`。具体可参考类 `AngleClassifier` 的说明
+
+每个参数都有默认取值，所以可以不传入任何参数值进行初始化：`std = CnStd()`。
+
+文本检测使用类`CnOcr`的函数 **`detect()`**，以下是详细说明：
+
+#### 类函数`CnStd.detect()`
+
+```python
+    def detect(
+        self,
+        img_list: Union[
+            str,
+            Path,
+            Image.Image,
+            np.ndarray,
+            List[Union[str, Path, Image.Image, np.ndarray]],
+        ],
+        resized_shape: Union[int, Tuple[int, int]] = (768, 768),
+        preserve_aspect_ratio: bool = True,
+        min_box_size: int = 8,
+        box_score_thresh: float = 0.3,
+        batch_size: int = 20,
+        **kwargs,
+    ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
+```
+
+**函数说明**：
+
+函数输入参数包括：
+
+- `img_list`: 支持对单个图片或者多个图片（列表）的检测。每个值可以是图片路径，或者已经读取进来 `PIL.Image.Image` 或 `np.ndarray`,  格式应该是 `RGB` 3 通道，shape: `(height, width, 3)`, 取值范围：`[0, 255]`。
+
+- `resized_shape`: `int` or `tuple`, `tuple` 含义为 `(height, width)`, `int` 则表示高宽都为此值；  
+   检测前，先把原始图片resize到接近此大小（只是接近，未必相等）。默认为 `(768, 768)`。
+  
+  > **Note** **（注意）**
+  > 这个取值对检测结果的影响较大，可以针对自己的应用多尝试几组值，再选出最优值。例如 `(512, 768)`, `(768, 768)`, `(768, 1024)`等。
+
+- `preserve_aspect_ratio`: 对原始图片 resize 时是否保持高宽比不变。默认为 `True`。
+
+- `min_box_size`: 过滤掉高度或者宽度小于此值的文本框。默认为 `8`，也即高或者宽小于 `8` 的文本框会被过滤去掉。
+
+- `box_score_thresh`: 过滤掉得分低于此值的文本框。默认为 `0.3`。
+
+- `batch_size`: 待处理图片很多时，需要分批处理，每批图片的数量由此参数指定。默认为 `20`。
+
+- `kwargs`: 保留参数，目前未被使用。
+
+函数输出类型为`list`，其中每个元素是一个字典，对应一张图片的检测结果。字典中包含以下 `keys`：
+
+- `rotated_angle`: `float`, 整张图片旋转的角度。只有 `auto_rotate_whole_image==True` 才可能非 `0`。
+
+- `detected_texts`: `list`, 每个元素存储了检测出的一个框的信息，使用词典记录，包括以下几个值：
+  
+  - `box`：检测出的文字对应的矩形框；`np.ndarray`, shape: `(4, 2)`，对应 box 4个点的坐标值 `(x, y)`;
+  
+  - `score`：得分；`float` 类型；分数越高表示越可靠；
+  
+  - `croppped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
+  
+  - 示例:
+    
+    ```python
+      [{'box': array([[416,  77],
+                      [486,  13],
+                      [800, 325],
+                      [730, 390]], dtype=int32),
+        'score': 1.0, 
+        'cropped_img': array([[[25, 20, 24],
+                               [26, 21, 25],
+                               [25, 20, 24],
+                              ...,
+                               [11, 11, 13],
+                               [11, 11, 13],
+                               [11, 11, 13]]], dtype=uint8)},
+       ...
+      ]
+    ```
+
+#### 调用示例
+
+```python
+from cnstd import CnStd
+std = CnStd()
+box_info_list = std.detect('examples/taobao.jpg')
+```
+
+或：
+
+```python
+from PIL import Image
+from cnstd import CnStd
+
+std = CnStd()
+img_fp = 'examples/taobao.jpg'
+img = Image.open(img_fp)
+box_infos = std.detect(img)
+```
+
+### 识别检测框中的文字（OCR）
+
+上面示例识别结果中"cropped_img"对应的值可以直接交由 **[cnocr](https://github.com/breezedeus/cnocr)** 中的 **`CnOcr`** 进行文字识别。如上例可以结合  **`CnOcr`** 进行文字识别：
+
+```python
+from cnstd import CnStd
+from cnocr import CnOcr
+
+std = CnStd()
+cn_ocr = CnOcr()
+
+box_infos = std.detect('examples/taobao.jpg')
+
+for box_info in box_infos['detected_texts']:
+    cropped_img = box_info['cropped_img']
+    ocr_res = cn_ocr.ocr_for_single_line(cropped_img)
+    print('ocr result: %s' % str(ocr_res))
+```
+
+注：运行上面示例需要先安装  **[cnocr](https://github.com/breezedeus/cnocr)** ：
+
+```bash
+pip install cnocr
+```
+
+
+
+### 数学公式检测（MFD）与 版面分析（Layout Analysis）
+
+数学公式检测（MFD）与 版面分析（Layout Analysis）都是检测图片中感兴趣的元素，它们使用的都是基于YOLOv7的检测架构，在CnSTD都来源于相同的类 `LayoutAnalyzer`，差别只是训练模型使用的数据不同。
+
+> 这两个模型的训练代码在 [yolov7](https://github.com/breezedeus/yolov7) 中（Forked from [WongKinYiu/yolov7](https://github.com/WongKinYiu/yolov7)，感谢原作者。）
+
+
+
+类 `LayoutAnalyzer` 的初始化函数如下：
+
+```python
+class LayoutAnalyzer(object):
+    def __init__(
+        self,
+        model_name: str = 'mfd',  # 'layout' or 'mfd'
+        *,
+        model_type: str = 'yolov7_tiny',
+        model_backend: str = 'pytorch',
+        model_fp: Optional[str] = None,
+        root: Union[str, Path] = data_dir(),
+        device: str = 'cpu',
+        **kwargs,
+    ):
+```
+
+其中的参数含义如下：
+
+- `model_name`: 字符串类型，表示模型类型。可选值：'mfd' 表示数学公式检测；'layout' 表示版面分析。默认值：'mfd'
+
+- `model_type`: 字符串类型，表示模型类型。当前支持 'yolov7_tiny' 和 'yolov7'；默认值：'yolov7_tiny'。'yolov7' 模型暂不开源，当前仅开放给星球会员下载，具体说明见：[P2T YoloV7 数学公式检测模型开放给星球会员下载 | Breezedeus.com](https://www.breezedeus.com/article/p2t-yolov7-for-zsxq-20230619) 。
+
+- `model_backend`: 字符串类型，表示backend。当前仅支持: 'pytorch'；默认值：'pytorch'
+
+- `model_fp`: 字符串类型，表示模型文件的路径。默认值：`None`，表示使用默认的文件路径
+
+- `root`: 字符串或`Path`类型，表示模型文件所在的根目录。
+  - Linux/Mac下默认值为 `~/.cnstd`，表示模型文件所处文件夹类似 `~/.cnstd/1.2/analysis`
+  - Windows下默认值为 `C:/Users/<username>/AppData/Roaming/cnstd`。
+  
+- `device`: 字符串类型，表示运行模型的设备，可选值：'cpu' 或 'gpu'；默认值：'cpu'
+
+- `**kwargs`: 额外的参数。
+
+
+
+函数输出结果为一个`list`，其中每个元素表示识别出的版面中的一个元素，包含以下信息：
+
+* type: 版面元素对应的类型；可选值来自：`self.categories` ;
+* box: 版面元素对应的矩形框；`np.ndarray`, shape: (4, 2)，对应 box 4个点的坐标值 `(x, y)` ;
+* score: 得分，越高表示越可信 。
+
+
+
+#### 类函数`LayoutAnalyzer.analyze()`
+
+对指定图片（列表）进行版面分析。
+
+```python
+def analyze(
+    self,
+    img_list: Union[
+        str,
+        Path,
+        Image.Image,
+        np.ndarray,
+        List[Union[str, Path, Image.Image, np.ndarray]],
+    ],
+    resized_shape: Union[int, Tuple[int, int]] = 700,
+    box_margin: int = 2,
+    conf_threshold: float = 0.25,
+    iou_threshold: float = 0.45,
+) -> Union[List[Dict[str, Any]], List[List[Dict[str, Any]]]]:
+```
+
+
+
+**函数说明**：
+
+函数输入参数包括：
+
+* `img_list` (str or list): 待识别图片或图片列表；如果是 `np.ndarray`，则应该是shape为 `[H, W, 3]` 的 RGB 格式数组
+* `resized_shape` (int or tuple): (H, W); 把图片resize到此大小再做分析；默认值为 `700`
+* `box_margin` (int): 对识别出的内容框往外扩展的像素大小；默认值为 `2`
+* `conf_threshold` (float): 分数阈值；默认值为 `0.25`
+* `iou_threshold` (float): IOU阈值；默认值为 `0.45`
+* `**kwargs`: 额外的参数。
+
+
+
+#### 调用示例
+
+```python
+from cnstd import LayoutAnalyzer
+img_fp = 'examples/mfd/zh5.jpg'
+analyzer = LayoutAnalyzer('mfd')
+out = analyzer.analyze(img_fp, resized_shape=700)
+print(out)
+```
+
+
+
+
+
+### 脚本使用
+
+**cnstd** 包含了几个命令行工具，安装 **cnstd** 后即可使用。
+
+#### STD 预测单个文件或文件夹中所有图片
+
+使用命令 **`cnstd predict`** 预测单个文件或文件夹中所有图片，以下是使用说明：
+
+```bash
+(venv) ➜  cnstd git:(master) ✗ cnstd predict -h
+Usage: cnstd predict [OPTIONS]
+
+  预测单个文件，或者指定目录下的所有图片
+
+Options:
+  -m, --model-name [ch_PP-OCRv2_det|ch_PP-OCRv3_det|db_mobilenet_v3|db_mobilenet_v3_small|db_resnet18|db_resnet34|db_shufflenet_v2|db_shufflenet_v2_small|db_shufflenet_v2_tiny|en_PP-OCRv3_det]
+                                  模型名称。默认值为 db_shufflenet_v2_small
+  -b, --model-backend [pytorch|onnx]
+                                  模型类型。默认值为 `onnx`
+  -p, --pretrained-model-fp TEXT  使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型
+  -r, --rotated-bbox              是否检测带角度（非水平和垂直）的文本框。默认为 `True`
+  --resized-shape TEXT            格式："height,width";
+                                  预测时把图片resize到此大小再进行预测。两个值都需要是32的倍数。默认为
+                                  `768,768`
+
+  --box-score-thresh FLOAT        检测结果只保留分数大于此值的文本框。默认值为 `0.3`
+  --preserve-aspect-ratio BOOLEAN
+                                  resize时是否保留图片原始比例。默认值为 `True`
+  --context TEXT                  使用cpu还是 `gpu` 运行代码，也可指定为特定gpu，如`cuda:0`。默认为
+                                  `cpu`
+
+  -i, --img-file-or-dir TEXT      输入图片的文件路径或者指定的文件夹
+  -o, --output-dir TEXT           检测结果存放的文件夹。默认为 `./predictions`
+  -h, --help                      Show this message and exit.
+```
+
+例如可以使用以下命令对图片 `examples/taobao.jpg`进行检测，并把检测结果存放在目录 `outputs`中：
+
+```bash
+cnstd predict -i examples/taobao.jpg -o outputs
+```
+
+具体使用也可参考文件 [Makefile](./Makefile) 。
+
+
+
+#### MFD or Layout Analysis 预测单个文件
+
+使用命令 **`cnstd analyze`** 获得单个文件的 MFD 或者 Layout Analysis 结果，以下是使用说明：
+
+```bash
+(venv) ➜  cnstd git:(master) ✗ cnstd analyze -h
+Usage: cnstd analyze [OPTIONS]
+
+  对给定图片进行 MFD 或者 版面分析。
+
+Options:
+  -m, --model-name [mfd|layout]   模型类型。`mfd` 表示数学公式检测，`layout`
+                                  表示版面分析；默认为：`mfd`
+  -t, --model-type TEXT           模型类型。当前支持 [`yolov7_tiny`, `yolov7`]
+  -b, --model-backend [pytorch|onnx]
+                                  模型后端架构。当前仅支持 `pytorch`
+  -p, --model-fp TEXT             使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型
+  --device TEXT                   cuda device, i.e. 0 or 0,1,2,3 or cpu
+  -i, --img-fp TEXT               待分析的图片路径或图片目录
+  -o, --output-fp TEXT            分析结果输出的图片路径。默认为 `None`，会存储在当前文件夹，文件名称为输入文件名称
+                                  前面增加`out-`；如输入文件名为 `img.jpg`, 输出文件名即为 `out-
+                                  img.jpg`；如果输入为目录，则此路径也应该是一个目录，会将输出文件存储在此目录下
+  --resized-shape INTEGER         分析时把图片resize到此大小再进行。默认为 `700`
+  --conf-thresh FLOAT             Confidence Threshold。默认值为 `0.25`
+  --iou-thresh FLOAT              IOU threshold for NMS。默认值为 `0.45`
+  -h, --help                      Show this message and exit.
+```
+
+例如可以使用以下命令对图片 `examples/mfd/zh.jpg` 进行 MFD，并把检测结果存放在文件 `out-zh.jpg` 中：
+
+```bash
+(venv) ➜  cnstd analyze -m mfd --conf-thresh 0.25 --resized-shape 800 -i examples/mfd/zh.jpg -o out-zh.jpg
+```
+
+具体使用也可参考文件 [Makefile](./Makefile) 。
+
+#### 模型训练
+
+使用命令 **`cnstd train`**  训练文本检测模型，以下是使用说明：
+
+```bash
+(venv) ➜  cnstd git:(master) ✗ cnstd train -h
+Usage: cnstd train [OPTIONS]
+
+  训练文本检测模型
+
+Options:
+  -m, --model-name [db_resnet50|db_resnet34|db_resnet18|db_mobilenet_v3|db_mobilenet_v3_small|db_shufflenet_v2|db_shufflenet_v2_small|db_shufflenet_v2_tiny]
+                                  模型名称。默认值为 `db_shufflenet_v2_small`
+  -i, --index-dir TEXT            索引文件所在的文件夹，会读取文件夹中的 `train.tsv` 和 `dev.tsv` 文件
+                                  [required]
+
+  --train-config-fp TEXT          训练使用的json配置文件  [required]
+  -r, --resume-from-checkpoint TEXT
+                                  恢复此前中断的训练状态，继续训练
+  -p, --pretrained-model-fp TEXT  导入的训练好的模型，作为初始模型。优先级低于 "--restore-training-
+                                  fp"，当传入"--restore-training-fp"时，此传入失效
+
+  -h, --help                      Show this message and exit.
+```
+
+具体使用可参考文件 [Makefile](./Makefile) 。
+
+#### 模型转存
+
+训练好的模型会存储训练状态，使用命令 **`cnstd resave`**  去掉与预测无关的数据，降低模型大小。
+
+```bash
+(venv) ➜  cnstd git:(master) ✗ cnstd resave -h
+Usage: cnstd resave [OPTIONS]
+
+  训练好的模型会存储训练状态，使用此命令去掉预测时无关的数据，降低模型大小
+
+Options:
+  -i, --input-model-fp TEXT   输入的模型文件路径  [required]
+  -o, --output-model-fp TEXT  输出的模型文件路径  [required]
+  -h, --help                  Show this message and exit.
+```
+
+## 未来工作
+
+* [x] 进一步精简模型结构，降低模型大小
+* [x] PSENet速度上还是比较慢，尝试更快的STD算法
+* [x] 加入更多的训练数据
+* [x] 加入对外部模型的支持
+* [x] 加入数学公式检测（MFD）与 版面分析（Layout Analysis）模型
+* [ ] 加入对文档结构与表格的检测
+
+
+
+## 给作者来杯咖啡
+
+开源不易，如果此项目对您有帮助，可以考虑 [给作者来杯咖啡 ☕️](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
+
+---
+
+官方代码库：[https://github.com/breezedeus/cnstd](https://github.com/breezedeus/cnstd)。
```

### Comparing `cnstd-1.2.2/cnstd.egg-info/SOURCES.txt` & `cnstd-1.2.3/cnstd.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 cnstd/__init__.py
 cnstd/__version__.py
 cnstd/app.py
 cnstd/cli.py
 cnstd/cn_std.py
@@ -69,8 +70,14 @@
 cnstd/yolov7/loss.py
 cnstd/yolov7/metrics.py
 cnstd/yolov7/plots.py
 cnstd/yolov7/torch_utils.py
 cnstd/yolov7/yolo.py
 cnstd/yolov7/yolov7-mfd.yaml
 cnstd/yolov7/yolov7-tiny-layout.yaml
-cnstd/yolov7/yolov7-tiny-mfd.yaml
+cnstd/yolov7/yolov7-tiny-mfd.yaml
+tests/test_cnstd.py
+tests/test_lr_schedulers.py
+tests/test_models.py
+tests/test_transforms.py
+tests/test_utils.py
+tests/test_yolov7.py
```

### Comparing `cnstd-1.2.2/setup.py` & `cnstd-1.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # coding: utf-8
-# Copyright (C) 2021, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2021-2023, [Breezedeus](https://github.com/breezedeus).
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -52,29 +52,31 @@
     'shapely',
     'Polygon3',
     'pyclipper',
     'matplotlib',
     'seaborn',
     "onnx",
     "onnxruntime",
+    "huggingface_hub",
 ]
 
 extras_require = {
     "dev": ["pip-tools", "pytest"],
 }
 
 entry_points = """
 [console_scripts]
 cnstd = cnstd.cli:cli
 """
 
 setup(
     name=PACKAGE_NAME,
     version=about['__version__'],
-    description="Python3 package for Chinese/English STR (Scene Text Recognition), with small pretrained models",
+    description="Python3 package for Chinese/English Scene Text Detection (STD), Mathematical Formula Detection (MFD), "
+                "and Layout Analysis, with free pretrained models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='breezedeus',
     author_email='breezedeus@163.com',
     license='Apache 2.0',
     url='https://github.com/breezedeus/cnstd',
     platforms=["Mac", "Linux", "Windows"],
@@ -98,13 +100,14 @@
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
 )
```

