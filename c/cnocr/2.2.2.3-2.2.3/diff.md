# Comparing `tmp/cnocr-2.2.2.3.tar.gz` & `tmp/cnocr-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnocr-2.2.2.3.tar", last modified: Tue Apr 11 15:22:31 2023, max compression
+gzip compressed data, was "cnocr-2.2.3.tar", last modified: Fri Jun 30 04:51:44 2023, max compression
```

## Comparing `cnocr-2.2.2.3.tar` & `cnocr-2.2.3.tar`

### file list

```diff
@@ -1,57 +1,65 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.343070 cnocr-2.2.2.3/
--rw-r--r--   0 king       (501) staff       (20)    19838 2023-04-11 15:22:31.342154 cnocr-2.2.2.3/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    15891 2023-02-11 15:49:08.000000 cnocr-2.2.2.3/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.211761 cnocr-2.2.2.3/cnocr/
--rw-r--r--   0 king       (501) staff       (20)     1259 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      893 2023-04-09 11:55:18.000000 cnocr-2.2.2.3/cnocr/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     7025 2022-10-24 08:33:21.000000 cnocr-2.2.2.3/cnocr/app.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.281894 cnocr-2.2.2.3/cnocr/classification/
--rw-r--r--   0 king       (501) staff       (20)      915 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/classification/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     5430 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/classification/dataset.py
--rw-r--r--   0 king       (501) staff       (20)     9801 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/classification/image_classifier.py
--rw-r--r--   0 king       (501) staff       (20)     8314 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/clf_cli.py
--rw-r--r--   0 king       (501) staff       (20)    18161 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/cli.py
--rw-r--r--   0 king       (501) staff       (20)    17817 2022-09-16 16:03:16.000000 cnocr-2.2.2.3/cnocr/cn_ocr.py
--rw-r--r--   0 king       (501) staff       (20)     7439 2022-07-25 14:40:28.000000 cnocr-2.2.2.3/cnocr/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.290602 cnocr-2.2.2.3/cnocr/data_utils/
--rw-r--r--   0 king       (501) staff       (20)        0 2019-03-02 15:15:34.000000 cnocr-2.2.2.3/cnocr/data_utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4128 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/data_utils/aug.py
--rw-r--r--   0 king       (501) staff       (20)     2221 2021-11-05 14:17:16.000000 cnocr-2.2.2.3/cnocr/data_utils/block_shuffle.py
--rw-r--r--   0 king       (501) staff       (20)     4393 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/data_utils/utils.py
--rw-r--r--   0 king       (501) staff       (20)     4295 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/dataset.py
--rw-r--r--   0 king       (501) staff       (20)    26689 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/label_cn.txt
--rwxr-xr-x   0 king       (501) staff       (20)     4596 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/line_split.py
--rw-r--r--   0 king       (501) staff       (20)     7573 2021-11-05 14:17:16.000000 cnocr-2.2.2.3/cnocr/lr_scheduler.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.301794 cnocr-2.2.2.3/cnocr/models/
--rw-r--r--   0 king       (501) staff       (20)        0 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/models/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     3788 2021-08-26 09:54:36.000000 cnocr-2.2.2.3/cnocr/models/ctc.py
--rw-r--r--   0 king       (501) staff       (20)     5032 2021-11-05 14:17:16.000000 cnocr-2.2.2.3/cnocr/models/densenet.py
--rw-r--r--   0 king       (501) staff       (20)     6877 2023-02-11 15:49:08.000000 cnocr-2.2.2.3/cnocr/models/mobilenet.py
--rw-r--r--   0 king       (501) staff       (20)    11059 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/models/ocr_model.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.312914 cnocr-2.2.2.3/cnocr/ppocr/
--rw-r--r--   0 king       (501) staff       (20)      222 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     1782 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.316938 cnocr-2.2.2.3/cnocr/ppocr/postprocess/
--rw-r--r--   0 king       (501) staff       (20)     2088 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/postprocess/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    26691 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/postprocess/rec_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)     9675 2023-02-11 15:48:37.000000 cnocr-2.2.2.3/cnocr/ppocr/pp_recognizer.py
--rw-r--r--   0 king       (501) staff       (20)    20044 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utility.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.326884 cnocr-2.2.2.3/cnocr/ppocr/utils/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    33443 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utils/chinese_cht_dict.txt
--rw-r--r--   0 king       (501) staff       (20)      190 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utils/en_dict.txt
--rw-r--r--   0 king       (501) staff       (20)    26249 2022-07-20 02:15:52.000000 cnocr-2.2.2.3/cnocr/ppocr/utils/ppocr_keys_v1.txt
--rw-r--r--   0 king       (501) staff       (20)    16147 2023-02-11 15:49:08.000000 cnocr-2.2.2.3/cnocr/recognizer.py
--rw-r--r--   0 king       (501) staff       (20)     1797 2022-09-01 02:35:51.000000 cnocr-2.2.2.3/cnocr/serve.py
--rw-r--r--   0 king       (501) staff       (20)    12496 2023-03-22 14:23:07.000000 cnocr-2.2.2.3/cnocr/trainer.py
--rw-r--r--   0 king       (501) staff       (20)    14819 2022-07-25 14:40:28.000000 cnocr-2.2.2.3/cnocr/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-04-11 15:22:31.276307 cnocr-2.2.2.3/cnocr.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    19838 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     1134 2023-04-11 15:22:31.000000 cnocr-2.2.2.3/cnocr.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       71 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2020-05-29 09:15:54.000000 cnocr-2.2.2.3/cnocr.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      233 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)        6 2023-04-11 15:22:30.000000 cnocr-2.2.2.3/cnocr.egg-info/top_level.txt
--rw-r--r--   0 king       (501) staff       (20)       38 2023-04-11 15:22:31.343265 cnocr-2.2.2.3/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     3190 2023-04-09 11:52:59.000000 cnocr-2.2.2.3/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.723543 cnocr-2.2.3/
+-rw-r--r--   0 king       (501) staff       (20)    41980 2019-03-26 07:39:48.000000 cnocr-2.2.3/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    16912 2023-06-30 04:51:44.716647 cnocr-2.2.3/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    15891 2023-05-11 02:09:18.000000 cnocr-2.2.3/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.466399 cnocr-2.2.3/cnocr/
+-rw-r--r--   0 king       (501) staff       (20)     1259 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      896 2023-06-30 03:34:48.000000 cnocr-2.2.3/cnocr/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     7025 2022-10-24 08:33:21.000000 cnocr-2.2.3/cnocr/app.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.500472 cnocr-2.2.3/cnocr/classification/
+-rw-r--r--   0 king       (501) staff       (20)      915 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/classification/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     5430 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/classification/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     9801 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/classification/image_classifier.py
+-rw-r--r--   0 king       (501) staff       (20)     8314 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/clf_cli.py
+-rw-r--r--   0 king       (501) staff       (20)    18161 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/cli.py
+-rw-r--r--   0 king       (501) staff       (20)    17817 2022-09-16 16:03:16.000000 cnocr-2.2.3/cnocr/cn_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)     7568 2023-06-30 03:59:34.000000 cnocr-2.2.3/cnocr/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.512887 cnocr-2.2.3/cnocr/data_utils/
+-rw-r--r--   0 king       (501) staff       (20)        0 2019-03-02 15:15:34.000000 cnocr-2.2.3/cnocr/data_utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4128 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/data_utils/aug.py
+-rw-r--r--   0 king       (501) staff       (20)     2221 2021-11-05 14:17:16.000000 cnocr-2.2.3/cnocr/data_utils/block_shuffle.py
+-rw-r--r--   0 king       (501) staff       (20)     4393 2021-08-26 09:54:36.000000 cnocr-2.2.3/cnocr/data_utils/utils.py
+-rw-r--r--   0 king       (501) staff       (20)     4295 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)    26689 2021-08-26 09:54:36.000000 cnocr-2.2.3/cnocr/label_cn.txt
+-rwxr-xr-x   0 king       (501) staff       (20)     4596 2021-08-26 09:54:36.000000 cnocr-2.2.3/cnocr/line_split.py
+-rw-r--r--   0 king       (501) staff       (20)     7573 2021-11-05 14:17:16.000000 cnocr-2.2.3/cnocr/lr_scheduler.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.563653 cnocr-2.2.3/cnocr/models/
+-rw-r--r--   0 king       (501) staff       (20)        0 2021-08-26 09:54:36.000000 cnocr-2.2.3/cnocr/models/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     3788 2021-08-26 09:54:36.000000 cnocr-2.2.3/cnocr/models/ctc.py
+-rw-r--r--   0 king       (501) staff       (20)     5032 2021-11-05 14:17:16.000000 cnocr-2.2.3/cnocr/models/densenet.py
+-rw-r--r--   0 king       (501) staff       (20)     6877 2023-05-11 02:09:18.000000 cnocr-2.2.3/cnocr/models/mobilenet.py
+-rw-r--r--   0 king       (501) staff       (20)    11059 2023-02-11 15:48:37.000000 cnocr-2.2.3/cnocr/models/ocr_model.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.649432 cnocr-2.2.3/cnocr/ppocr/
+-rw-r--r--   0 king       (501) staff       (20)      222 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     1782 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.661280 cnocr-2.2.3/cnocr/ppocr/postprocess/
+-rw-r--r--   0 king       (501) staff       (20)     2088 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/postprocess/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    26691 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/postprocess/rec_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)     9910 2023-06-30 04:42:08.000000 cnocr-2.2.3/cnocr/ppocr/pp_recognizer.py
+-rw-r--r--   0 king       (501) staff       (20)    20044 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/utility.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.702721 cnocr-2.2.3/cnocr/ppocr/utils/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    33443 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/utils/chinese_cht_dict.txt
+-rw-r--r--   0 king       (501) staff       (20)      190 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/utils/en_dict.txt
+-rw-r--r--   0 king       (501) staff       (20)    26249 2022-07-20 02:15:52.000000 cnocr-2.2.3/cnocr/ppocr/utils/ppocr_keys_v1.txt
+-rw-r--r--   0 king       (501) staff       (20)    16412 2023-06-30 04:42:19.000000 cnocr-2.2.3/cnocr/recognizer.py
+-rw-r--r--   0 king       (501) staff       (20)     1797 2022-09-01 02:35:51.000000 cnocr-2.2.3/cnocr/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    12521 2023-05-11 02:35:52.000000 cnocr-2.2.3/cnocr/trainer.py
+-rw-r--r--   0 king       (501) staff       (20)    13597 2023-06-30 04:42:29.000000 cnocr-2.2.3/cnocr/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.495410 cnocr-2.2.3/cnocr.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    16912 2023-06-30 04:51:44.000000 cnocr-2.2.3/cnocr.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     1269 2023-06-30 04:51:44.000000 cnocr-2.2.3/cnocr.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2023-06-30 04:51:44.000000 cnocr-2.2.3/cnocr.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       70 2023-06-30 04:51:44.000000 cnocr-2.2.3/cnocr.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2020-05-29 09:15:54.000000 cnocr-2.2.3/cnocr.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      233 2023-06-30 04:51:44.000000 cnocr-2.2.3/cnocr.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)        6 2023-06-30 04:51:44.000000 cnocr-2.2.3/cnocr.egg-info/top_level.txt
+-rw-r--r--   0 king       (501) staff       (20)       38 2023-06-30 04:51:44.728489 cnocr-2.2.3/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     3245 2023-06-30 04:42:38.000000 cnocr-2.2.3/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:51:44.713026 cnocr-2.2.3/tests/
+-rw-r--r--   0 king       (501) staff       (20)     9464 2022-07-25 14:40:29.000000 cnocr-2.2.3/tests/test_cnocr.py
+-rw-r--r--   0 king       (501) staff       (20)     1816 2022-07-25 14:40:29.000000 cnocr-2.2.3/tests/test_dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     4947 2021-11-05 14:17:16.000000 cnocr-2.2.3/tests/test_models.py
+-rw-r--r--   0 king       (501) staff       (20)     3102 2022-07-20 02:15:52.000000 cnocr-2.2.3/tests/test_ppocr.py
+-rw-r--r--   0 king       (501) staff       (20)     1297 2022-07-25 14:40:29.000000 cnocr-2.2.3/tests/test_pytorch.py
+-rw-r--r--   0 king       (501) staff       (20)     1698 2022-07-25 14:40:29.000000 cnocr-2.2.3/tests/test_trainer.py
```

### Comparing `cnocr-2.2.2.3/PKG-INFO` & `cnocr-2.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,399 +1,401 @@
 Metadata-Version: 2.1
 Name: cnocr
-Version: 2.2.2.3
+Version: 2.2.3
 Summary: Python3 package for Chinese/English OCR, with small pretrained models
 Home-page: https://github.com/breezedeus/cnocr
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
-Description: <div align="center">
-          <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
-          <div>&nbsp;</div>
-        
-        [![Downloads](https://static.pepy.tech/personalized-badge/cnocr?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnocr)
-        [![license](https://img.shields.io/github/license/breezedeus/cnocr)](./LICENSE)
-        [![Docs](https://readthedocs.org/projects/cnocr/badge/?version=latest)](https://cnocr.readthedocs.io/zh/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/cnocr.svg)](https://badge.fury.io/py/cnocr)
-        [![forks](https://img.shields.io/github/forks/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
-        [![stars](https://img.shields.io/github/stars/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
-        ![last-releast](https://img.shields.io/github/release-date/breezedeus/cnocr)
-        ![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnocr)
-        [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
-        
-        [📖 文档](https://cnocr.readthedocs.io/zh/latest/) |
-        [🛠️ 安装](https://cnocr.readthedocs.io/zh/latest/install/) |
-        [🧳 可用模型](https://cnocr.readthedocs.io/zh/latest/models/) |
-        [🕹 模型训练](https://cnocr.readthedocs.io/zh/latest/train/) |
-        [🛀🏻 在线Demo](https://huggingface.co/spaces/breezedeus/cnocr) |
-        [💬 交流群](https://cnocr.readthedocs.io/zh/latest/contact/)
-        
-        </div>
-        
-        <div align="center">
-        
-        [English](./README_en.md) | 中文
-        
-        </div>
-        
-        # CnOCR
-        <div align="center">
-        <strong>Tech should serve the people, not enslave them!</strong>
-        <br>
-        <strong>请勿将此项目用于文字审查！</strong>
-        <br>
-        ---
-        </div>
-        
-        [**CnOCR**](https://github.com/breezedeus/cnocr) 是 **Python 3** 下的**文字识别**（**Optical Character Recognition**，简称**OCR**）工具包，支持**简体中文**、**繁体中文**（部分模型）、**英文**和**数字**的常见字符识别，支持竖排文字的识别。自带了**20+个** [训练好的模型](https://cnocr.readthedocs.io/zh/latest/models/)，适用于不同应用场景，安装后即可直接使用。同时，CnOCR也提供简单的[训练命令](https://cnocr.readthedocs.io/zh/latest/train/)供使用者训练自己的模型。欢迎扫码加小助手为好友，备注 `ocr`，小助手会定期统一邀请大家入群：
-        
-        <div align="center">
-          <img src="https://huggingface.co/datasets/breezedeus/cnocr-wx-qr-code/resolve/main/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
-        </div>
-        
-        
-        作者也维护 **知识星球** [**CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**未公开的模型**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。此外，**私享群中作者每月提供两次免费特有数据的训练服务**。
-        
-        ## 详细文档
-        
-        见 [CnOCR在线文档](https://cnocr.readthedocs.io/) 。
-        
-        ## 使用说明
-        
-        **CnOCR** 从 **V2.2** 开始，内部自动调用文字检测引擎 **[CnSTD](https://github.com/breezedeus/cnstd)** 进行文字检测和定位。所以 **CnOCR** V2.2 不仅能识别排版简单的印刷体文字图片，如截图图片，扫描件等，也能识别**一般图片中的场景文字**。
-        
-        以下是一些不同场景的调用示例。
-        
-        ## 在 Cloud IDE 中预览
-        
-        [https://idegithub.com/breezedeus/CnOCR](https://idegithub.com/breezedeus/CnOCR)
-        
-        ## 不同场景的调用示例
-        
-        ### 常见的图片识别
-        
-        所有参数都使用默认值即可。如果发现效果不够好，多调整下各个参数看效果，最终往往能获得比较理想的精度。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/huochepiao.jpeg'
-        ocr = CnOcr()  # 所有参数都使用默认值
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        识别结果：
-        
-        <div align="center">
-          <img src="./docs/predict-outputs/huochepiao.jpeg-result.jpg" alt="火车票识别" width="800px"/>
-        </div>
-        
-        
-        ### 排版简单的印刷体截图图片识别
-        
-        针对 **排版简单的印刷体文字图片**，如截图图片，扫描件图片等，可使用 `det_model_name='naive_det'`，相当于不使用文本检测模型，而使用简单的规则进行分行。
-        
-        > **Note**
-        >
-        >  `det_model_name='naive_det'` 的效果相当于 `V2.2` 之前（`V2.0.*`, `V2.1.*`）的 CnOCR 版本。
-        
-        使用 `det_model_name='naive_det'` 的最大优势是**速度快**，劣势是对图片比较挑剔。如何判断是否该使用此检测模型呢？最简单的方式就是拿应用图片试试效果，效果好就用，不好就不用。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/multi-line_cn1.png'
-        ocr = CnOcr(det_model_name='naive_det') 
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        识别结果：
-        
-        <div align="center">
-        
-        | 图片                                                                      | OCR结果                                                                                                                         |
-        | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
-        | ![docs/examples/multi-line_cn1.png](./docs/examples/multi-line_cn1.png) | 网络支付并无本质的区别，因为<br />每一个手机号码和邮件地址背后<br />都会对应着一个账户--这个账<br />户可以是信用卡账户、借记卡账<br />户，也包括邮局汇款、手机代<br />收、电话代收、预付费卡和点卡<br />等多种形式。 |
-        
-        </div>
-        
-        
-        ### 竖排文字识别
-        
-        采用来自 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR)（之后简称 **ppocr**）的中文识别模型 `rec_model_name='ch_PP-OCRv3'` 进行识别。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/shupai.png'
-        ocr = CnOcr(rec_model_name='ch_PP-OCRv3')
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        识别结果：
-        <div align="center">
-          <img src="./docs/predict-outputs/shupai.png-result.jpg" alt="竖排文字识别" width="800px"/>
-        </div>
-        
-        
-        ### 英文识别
-        
-        虽然中文检测和识别模型也能识别英文，但**专为英文文字训练的检测器和识别器往往精度更高**。如果是纯英文的应用场景，建议使用来自 **ppocr** 的英文检测模型 `det_model_name='en_PP-OCRv3_det'`， 和英文识别模型 `rec_model_name='en_PP-OCRv3'` 。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/en_book1.jpeg'
-        ocr = CnOcr(det_model_name='en_PP-OCRv3_det', rec_model_name='en_PP-OCRv3')
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        识别结果：
-        
-        <div align="center">
-          <img src="./docs/predict-outputs/en_book1.jpeg-result.jpg" alt="英文识别" width="600px"/>
-        </div>
-        
-        
-        ### 繁体中文识别
-        
-        采用来自ppocr的繁体识别模型 `rec_model_name='chinese_cht_PP-OCRv3'` 进行识别。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/fanti.jpg'
-        ocr = CnOcr(rec_model_name='chinese_cht_PP-OCRv3')  # 识别模型使用繁体识别模型
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        使用此模型时请注意以下问题：
-        
-        * 识别精度一般，不是很好；
-        
-        * 除了繁体字，对标点、英文、数字的识别都不好；
-        
-        * 此模型不支持竖排文字的识别。
-        
-        识别结果：
-        <div align="center">
-          <img src="./docs/predict-outputs/fanti.jpg-result.jpg" alt="繁体中文识别" width="700px"/>
-        </div>
-        
-        
-        ### 单行文字的图片识别
-        
-        如果明确知道待识别的图片是单行文字图片（如下图），可以使用类函数 `CnOcr.ocr_for_single_line()` 进行识别。这样就省掉了文字检测的时间，速度会快一倍以上。
-        
-        <div align="center">
-          <img src="./docs/examples/helloworld.jpg" alt="单行文本识别" width="300px"/>
-        </div>
-        调用代码如下：
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/helloworld.jpg'
-        ocr = CnOcr()
-        out = ocr.ocr_for_single_line(img_fp)
-        print(out)
-        ```
-        
-        
-        
-        ### 更多应用示例
-        
-        * **核酸疫苗截图识别**
-        <div align="center">
-          <img src="./docs/predict-outputs/jiankangbao.jpeg-result.jpg" alt="核酸疫苗截图识别" width="500px"/>
-        </div>
-        
-        * **身份证识别**
-        <div align="center">
-          <img src="./docs/predict-outputs/aobama.webp-result.jpg" alt="身份证识别" width="700px"/>
-        </div>
-        
-        * **饭店小票识别**
-        <div align="center">
-          <img src="./docs/predict-outputs/fapiao.jpeg-result.jpg" alt="饭店小票识别" width="500px"/>
-        </div>
-          
-        
-          
-        
-        ## 安装
-        
-        嗯，顺利的话一行命令即可。
-        
-        ```bash
-        pip install cnocr
-        ```
-        
-        安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
-        
-        ```bash
-        pip install cnocr -i https://pypi.doubanio.com/simple
-        ```
-        
-        > **Note** 
-        >
-        > 请使用 **Python3**（3.6以及之后版本应该都行），没测过Python2下是否ok。
-        
-        更多说明可见 [安装文档](https://cnocr.readthedocs.io/zh/latest/install/)。
-        
-        > **Warning** 
-        >
-        > 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到问题，但一般都是常见问题，可以自行百度/Google解决。
-        
-        
-        
-        
-        
-        ## HTTP服务
-        
-        CnOCR **V2.2.1** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
-        
-        ```bash
-        pip install cnocr[serve]
-        ```
-        
-        
-        
-        安装完成后，可以通过以下命令启动HTTP服务（**`-p`** 后面的数字是**端口**，可以根据需要自行调整）：
-        
-        ```bash
-        cnocr serve -p 8501
-        ```
-        
-        
-        
-        服务开启后，可以使用以下方式调用服务。
-        
-        
-        
-        ### 命令行
-        
-        比如待识别文件为 `docs/examples/huochepiao.jpeg`，如下使用 curl 调用服务：
-        
-        ```bash
-        > curl -F image=@docs/examples/huochepiao.jpeg http://0.0.0.0:8501/ocr
-        ```
-        
-        
-        
-        ### Python
-        
-        使用如下方式调用服务：
-        
-        ```python
-        import requests
-        
-        image_fp = 'docs/examples/huochepiao.jpeg'
-        r = requests.post(
-            'http://0.0.0.0:8501/ocr', files={'image': (image_fp, open(image_fp, 'rb'), 'image/png')},
-        )
-        ocr_out = r.json()['results']
-        print(ocr_out)
-        ```
-        
-        
-        
-        具体也可参考文件 [scripts/screenshot_daemon_with_server.py](scripts/screenshot_daemon_with_server.py) 。 
-        
-        
-        
-        ### 其他语言
-        
-        请参照 curl 的调用方式自行实现。
-        
-        
-        
-        
-        
-        ## 可使用的模型
-        
-        ### 可使用的检测模型
-        
-        | `det_model_name`                                             | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                       | 是否支持竖排文字识别 |
-        | ------------------------------------------------------------ | ------------ | --------- | ------------ | ------------ | ------------------------------ | -------------------- |
-        | db_shufflenet_v2                                             | √            | X         | cnocr        | 18 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | **db_shufflenet_v2_small**                                   | √            | X         | cnocr        | 12 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | [db_shufflenet_v2_tiny](https://mp.weixin.qq.com/s/fHPNoGyo72EFApVhEgR6Nw) | √            | X         | cnocr        | 7.5 M        | 简体中文、繁体中文、英文、数字 | √                    |
-        | db_mobilenet_v3                                              | √            | X         | cnocr        | 16 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | db_mobilenet_v3_small                                        | √            | X         | cnocr        | 7.9 M        | 简体中文、繁体中文、英文、数字 | √                    |
-        | db_resnet34                                                  | √            | X         | cnocr        | 86 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | db_resnet18                                                  | √            | X         | cnocr        | 47 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | ch_PP-OCRv3_det                                              | X            | √         | ppocr        | 2.3 M        | 简体中文、繁体中文、英文、数字 | √                    |
-        | ch_PP-OCRv2_det                                              | X            | √         | ppocr        | 2.2 M        | 简体中文、繁体中文、英文、数字 | √                    |
-        | **en_PP-OCRv3_det**                                          | X            | √         | ppocr        | 2.3 M        | **英文**、数字                 | √                    |
-        
-        
-        
-        ### 可使用的识别模型
-        
-        | `rec_model_name`          | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                 | 是否支持竖排文字识别 |
-        | ------------------------- | ------------ | --------- | ------------ | ------------ | ------------------------ | -------------------- |
-        | densenet_lite_114-fc      | √            | √         | cnocr        | 4.9 M        | 简体中文、英文、数字     | X                    |
-        | densenet_lite_124-fc      | √            | √         | cnocr        | 5.1 M        | 简体中文、英文、数字     | X                    |
-        | densenet_lite_134-fc      | √            | √         | cnocr        | 5.4 M        | 简体中文、英文、数字     | X                    |
-        | densenet_lite_136-fc      | √            | √         | cnocr        | 5.9 M        | 简体中文、英文、数字     | X                    |
-        | densenet_lite_134-gru     | √            | X         | cnocr        | 11 M         | 简体中文、英文、数字     | X                    |
-        | densenet_lite_136-gru     | √            | X         | cnocr        | 12 M         | 简体中文、英文、数字     | X                    |
-        | ch_PP-OCRv3               | X            | √         | ppocr        | 10 M         | 简体中文、英文、数字     | √                    |
-        | ch_ppocr_mobile_v2.0      | X            | √         | ppocr        | 4.2 M        | 简体中文、英文、数字     | √                    |
-        | **en_PP-OCRv3**           | X            | √         | ppocr        | 8.5 M        | **英文**、数字           | √                    |
-        | **en_number_mobile_v2.0** | X            | √         | ppocr        | 1.8 M        | **英文**、数字           | √                    |
-        | **chinese_cht_PP-OCRv3**  | X            | √         | ppocr        | 11 M         | **繁体中文**、英文、数字 | X                    |
-        
-        ## 未来工作
-        
-        * [x] 支持图片包含多行文字 (`Done`)
-        * [x] crnn模型支持可变长预测，提升灵活性 (since `V1.0.0`)
-        * [x] 完善测试用例 (`Doing`)
-        * [x] 修bugs（目前代码还比较凌乱。。） (`Doing`)
-        * [x] 支持`空格`识别（since `V1.1.0`）
-        * [x] 尝试新模型，如 DenseNet，进一步提升识别准确率（since `V1.1.0`）
-        * [x] 优化训练集，去掉不合理的样本；在此基础上，重新训练各个模型
-        * [x] 由 MXNet 改为 PyTorch 架构（since `V2.0.0`）
-        * [x] 基于 PyTorch 训练更高效的模型
-        * [x] 支持列格式的文字识别
-        * [x] 打通与 [CnSTD](https://github.com/breezedeus/cnstd) 的无缝衔接（since `V2.2`）
-        * [ ] 支持更多的应用场景，如公式识别、表格识别、版面分析等
-        
-        
-        
-        ## 给作者来杯咖啡
-        
-        开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
-        
-        ---
-        
-        官方代码库：[https://github.com/breezedeus/cnocr](https://github.com/breezedeus/cnocr)。
-        
-        
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
-Provides-Extra: serve
 Provides-Extra: dev
+Provides-Extra: serve
+License-File: LICENSE
+
+<div align="center">
+  <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
+  <div>&nbsp;</div>
+
+[![Downloads](https://static.pepy.tech/personalized-badge/cnocr?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnocr)
+[![license](https://img.shields.io/github/license/breezedeus/cnocr)](./LICENSE)
+[![Docs](https://readthedocs.org/projects/cnocr/badge/?version=latest)](https://cnocr.readthedocs.io/zh/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/cnocr.svg)](https://badge.fury.io/py/cnocr)
+[![forks](https://img.shields.io/github/forks/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
+[![stars](https://img.shields.io/github/stars/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
+![last-releast](https://img.shields.io/github/release-date/breezedeus/cnocr)
+![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnocr)
+[![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
+
+[📖 文档](https://cnocr.readthedocs.io/zh/latest/) |
+[🛠️ 安装](https://cnocr.readthedocs.io/zh/latest/install/) |
+[🧳 可用模型](https://cnocr.readthedocs.io/zh/latest/models/) |
+[🕹 模型训练](https://cnocr.readthedocs.io/zh/latest/train/) |
+[🛀🏻 在线Demo](https://huggingface.co/spaces/breezedeus/cnocr) |
+[💬 交流群](https://cnocr.readthedocs.io/zh/latest/contact/)
+
+</div>
+
+<div align="center">
+
+[English](./README_en.md) | 中文
+
+</div>
+
+# CnOCR
+<div align="center">
+<strong>Tech should serve the people, not enslave them!</strong>
+<br>
+<strong>请勿将此项目用于文字审查！</strong>
+<br>
+---
+</div>
+
+[**CnOCR**](https://github.com/breezedeus/cnocr) 是 **Python 3** 下的**文字识别**（**Optical Character Recognition**，简称**OCR**）工具包，支持**简体中文**、**繁体中文**（部分模型）、**英文**和**数字**的常见字符识别，支持竖排文字的识别。自带了**20+个** [训练好的模型](https://cnocr.readthedocs.io/zh/latest/models/)，适用于不同应用场景，安装后即可直接使用。同时，CnOCR也提供简单的[训练命令](https://cnocr.readthedocs.io/zh/latest/train/)供使用者训练自己的模型。欢迎扫码加小助手为好友，备注 `ocr`，小助手会定期统一邀请大家入群：
+
+<div align="center">
+  <img src="https://huggingface.co/datasets/breezedeus/cnocr-wx-qr-code/resolve/main/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
+</div>
+
+
+作者也维护 **知识星球** [**CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**未公开的模型**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。此外，**私享群中作者每月提供两次免费特有数据的训练服务**。
+
+## 详细文档
+
+见 [CnOCR在线文档](https://cnocr.readthedocs.io/) 。
+
+## 使用说明
+
+**CnOCR** 从 **V2.2** 开始，内部自动调用文字检测引擎 **[CnSTD](https://github.com/breezedeus/cnstd)** 进行文字检测和定位。所以 **CnOCR** V2.2 不仅能识别排版简单的印刷体文字图片，如截图图片，扫描件等，也能识别**一般图片中的场景文字**。
+
+以下是一些不同场景的调用示例。
+
+## 在 Cloud IDE 中预览
+
+[https://idegithub.com/breezedeus/CnOCR](https://idegithub.com/breezedeus/CnOCR)
+
+## 不同场景的调用示例
+
+### 常见的图片识别
+
+所有参数都使用默认值即可。如果发现效果不够好，多调整下各个参数看效果，最终往往能获得比较理想的精度。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/huochepiao.jpeg'
+ocr = CnOcr()  # 所有参数都使用默认值
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+识别结果：
+
+<div align="center">
+  <img src="./docs/predict-outputs/huochepiao.jpeg-result.jpg" alt="火车票识别" width="800px"/>
+</div>
+
+
+### 排版简单的印刷体截图图片识别
+
+针对 **排版简单的印刷体文字图片**，如截图图片，扫描件图片等，可使用 `det_model_name='naive_det'`，相当于不使用文本检测模型，而使用简单的规则进行分行。
+
+> **Note**
+>
+>  `det_model_name='naive_det'` 的效果相当于 `V2.2` 之前（`V2.0.*`, `V2.1.*`）的 CnOCR 版本。
+
+使用 `det_model_name='naive_det'` 的最大优势是**速度快**，劣势是对图片比较挑剔。如何判断是否该使用此检测模型呢？最简单的方式就是拿应用图片试试效果，效果好就用，不好就不用。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/multi-line_cn1.png'
+ocr = CnOcr(det_model_name='naive_det') 
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+识别结果：
+
+<div align="center">
+
+| 图片                                                                      | OCR结果                                                                                                                         |
+| ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
+| ![docs/examples/multi-line_cn1.png](./docs/examples/multi-line_cn1.png) | 网络支付并无本质的区别，因为<br />每一个手机号码和邮件地址背后<br />都会对应着一个账户--这个账<br />户可以是信用卡账户、借记卡账<br />户，也包括邮局汇款、手机代<br />收、电话代收、预付费卡和点卡<br />等多种形式。 |
+
+</div>
+
+
+### 竖排文字识别
+
+采用来自 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR)（之后简称 **ppocr**）的中文识别模型 `rec_model_name='ch_PP-OCRv3'` 进行识别。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/shupai.png'
+ocr = CnOcr(rec_model_name='ch_PP-OCRv3')
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+识别结果：
+<div align="center">
+  <img src="./docs/predict-outputs/shupai.png-result.jpg" alt="竖排文字识别" width="800px"/>
+</div>
+
+
+### 英文识别
+
+虽然中文检测和识别模型也能识别英文，但**专为英文文字训练的检测器和识别器往往精度更高**。如果是纯英文的应用场景，建议使用来自 **ppocr** 的英文检测模型 `det_model_name='en_PP-OCRv3_det'`， 和英文识别模型 `rec_model_name='en_PP-OCRv3'` 。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/en_book1.jpeg'
+ocr = CnOcr(det_model_name='en_PP-OCRv3_det', rec_model_name='en_PP-OCRv3')
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+识别结果：
+
+<div align="center">
+  <img src="./docs/predict-outputs/en_book1.jpeg-result.jpg" alt="英文识别" width="600px"/>
+</div>
+
+
+### 繁体中文识别
+
+采用来自ppocr的繁体识别模型 `rec_model_name='chinese_cht_PP-OCRv3'` 进行识别。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/fanti.jpg'
+ocr = CnOcr(rec_model_name='chinese_cht_PP-OCRv3')  # 识别模型使用繁体识别模型
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+使用此模型时请注意以下问题：
+
+* 识别精度一般，不是很好；
+
+* 除了繁体字，对标点、英文、数字的识别都不好；
+
+* 此模型不支持竖排文字的识别。
+
+识别结果：
+<div align="center">
+  <img src="./docs/predict-outputs/fanti.jpg-result.jpg" alt="繁体中文识别" width="700px"/>
+</div>
+
+
+### 单行文字的图片识别
+
+如果明确知道待识别的图片是单行文字图片（如下图），可以使用类函数 `CnOcr.ocr_for_single_line()` 进行识别。这样就省掉了文字检测的时间，速度会快一倍以上。
+
+<div align="center">
+  <img src="./docs/examples/helloworld.jpg" alt="单行文本识别" width="300px"/>
+</div>
+调用代码如下：
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/helloworld.jpg'
+ocr = CnOcr()
+out = ocr.ocr_for_single_line(img_fp)
+print(out)
+```
+
+
+
+### 更多应用示例
+
+* **核酸疫苗截图识别**
+<div align="center">
+  <img src="./docs/predict-outputs/jiankangbao.jpeg-result.jpg" alt="核酸疫苗截图识别" width="500px"/>
+</div>
+
+* **身份证识别**
+<div align="center">
+  <img src="./docs/predict-outputs/aobama.webp-result.jpg" alt="身份证识别" width="700px"/>
+</div>
+
+* **饭店小票识别**
+<div align="center">
+  <img src="./docs/predict-outputs/fapiao.jpeg-result.jpg" alt="饭店小票识别" width="500px"/>
+</div>
+  
+
+  
+
+## 安装
+
+嗯，顺利的话一行命令即可。
+
+```bash
+pip install cnocr
+```
+
+安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
+
+```bash
+pip install cnocr -i https://pypi.doubanio.com/simple
+```
+
+> **Note** 
+>
+> 请使用 **Python3**（3.6以及之后版本应该都行），没测过Python2下是否ok。
+
+更多说明可见 [安装文档](https://cnocr.readthedocs.io/zh/latest/install/)。
+
+> **Warning** 
+>
+> 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到问题，但一般都是常见问题，可以自行百度/Google解决。
+
+
+
+
+
+## HTTP服务
+
+CnOCR **V2.2.1** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
+
+```bash
+pip install cnocr[serve]
+```
+
+
+
+安装完成后，可以通过以下命令启动HTTP服务（**`-p`** 后面的数字是**端口**，可以根据需要自行调整）：
+
+```bash
+cnocr serve -p 8501
+```
+
+
+
+服务开启后，可以使用以下方式调用服务。
+
+
+
+### 命令行
+
+比如待识别文件为 `docs/examples/huochepiao.jpeg`，如下使用 curl 调用服务：
+
+```bash
+> curl -F image=@docs/examples/huochepiao.jpeg http://0.0.0.0:8501/ocr
+```
+
+
+
+### Python
+
+使用如下方式调用服务：
+
+```python
+import requests
+
+image_fp = 'docs/examples/huochepiao.jpeg'
+r = requests.post(
+    'http://0.0.0.0:8501/ocr', files={'image': (image_fp, open(image_fp, 'rb'), 'image/png')},
+)
+ocr_out = r.json()['results']
+print(ocr_out)
+```
+
+
+
+具体也可参考文件 [scripts/screenshot_daemon_with_server.py](scripts/screenshot_daemon_with_server.py) 。 
+
+
+
+### 其他语言
+
+请参照 curl 的调用方式自行实现。
+
+
+
+
+
+## 可使用的模型
+
+### 可使用的检测模型
+
+| `det_model_name`                                             | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                       | 是否支持竖排文字识别 |
+| ------------------------------------------------------------ | ------------ | --------- | ------------ | ------------ | ------------------------------ | -------------------- |
+| db_shufflenet_v2                                             | √            | X         | cnocr        | 18 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| **db_shufflenet_v2_small**                                   | √            | X         | cnocr        | 12 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| [db_shufflenet_v2_tiny](https://mp.weixin.qq.com/s/fHPNoGyo72EFApVhEgR6Nw) | √            | X         | cnocr        | 7.5 M        | 简体中文、繁体中文、英文、数字 | √                    |
+| db_mobilenet_v3                                              | √            | X         | cnocr        | 16 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| db_mobilenet_v3_small                                        | √            | X         | cnocr        | 7.9 M        | 简体中文、繁体中文、英文、数字 | √                    |
+| db_resnet34                                                  | √            | X         | cnocr        | 86 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| db_resnet18                                                  | √            | X         | cnocr        | 47 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| ch_PP-OCRv3_det                                              | X            | √         | ppocr        | 2.3 M        | 简体中文、繁体中文、英文、数字 | √                    |
+| ch_PP-OCRv2_det                                              | X            | √         | ppocr        | 2.2 M        | 简体中文、繁体中文、英文、数字 | √                    |
+| **en_PP-OCRv3_det**                                          | X            | √         | ppocr        | 2.3 M        | **英文**、数字                 | √                    |
+
+
+
+### 可使用的识别模型
+
+| `rec_model_name`          | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                 | 是否支持竖排文字识别 |
+| ------------------------- | ------------ | --------- | ------------ | ------------ | ------------------------ | -------------------- |
+| densenet_lite_114-fc      | √            | √         | cnocr        | 4.9 M        | 简体中文、英文、数字     | X                    |
+| densenet_lite_124-fc      | √            | √         | cnocr        | 5.1 M        | 简体中文、英文、数字     | X                    |
+| densenet_lite_134-fc      | √            | √         | cnocr        | 5.4 M        | 简体中文、英文、数字     | X                    |
+| densenet_lite_136-fc      | √            | √         | cnocr        | 5.9 M        | 简体中文、英文、数字     | X                    |
+| densenet_lite_134-gru     | √            | X         | cnocr        | 11 M         | 简体中文、英文、数字     | X                    |
+| densenet_lite_136-gru     | √            | X         | cnocr        | 12 M         | 简体中文、英文、数字     | X                    |
+| ch_PP-OCRv3               | X            | √         | ppocr        | 10 M         | 简体中文、英文、数字     | √                    |
+| ch_ppocr_mobile_v2.0      | X            | √         | ppocr        | 4.2 M        | 简体中文、英文、数字     | √                    |
+| **en_PP-OCRv3**           | X            | √         | ppocr        | 8.5 M        | **英文**、数字           | √                    |
+| **en_number_mobile_v2.0** | X            | √         | ppocr        | 1.8 M        | **英文**、数字           | √                    |
+| **chinese_cht_PP-OCRv3**  | X            | √         | ppocr        | 11 M         | **繁体中文**、英文、数字 | X                    |
+
+## 未来工作
+
+* [x] 支持图片包含多行文字 (`Done`)
+* [x] crnn模型支持可变长预测，提升灵活性 (since `V1.0.0`)
+* [x] 完善测试用例 (`Doing`)
+* [x] 修bugs（目前代码还比较凌乱。。） (`Doing`)
+* [x] 支持`空格`识别（since `V1.1.0`）
+* [x] 尝试新模型，如 DenseNet，进一步提升识别准确率（since `V1.1.0`）
+* [x] 优化训练集，去掉不合理的样本；在此基础上，重新训练各个模型
+* [x] 由 MXNet 改为 PyTorch 架构（since `V2.0.0`）
+* [x] 基于 PyTorch 训练更高效的模型
+* [x] 支持列格式的文字识别
+* [x] 打通与 [CnSTD](https://github.com/breezedeus/cnstd) 的无缝衔接（since `V2.2`）
+* [ ] 支持更多的应用场景，如公式识别、表格识别、版面分析等
+
+
+
+## 给作者来杯咖啡
+
+开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
+
+---
+
+官方代码库：[https://github.com/breezedeus/cnocr](https://github.com/breezedeus/cnocr)。
+
```

### Comparing `cnocr-2.2.2.3/README.md` & `cnocr-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/__init__.py` & `cnocr-2.2.3/cnocr/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/__version__.py` & `cnocr-2.2.3/cnocr/__version__.py`

 * *Files 2% similar despite different names*

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
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-__version__ = '2.2.2.3'
+__version__ = '2.2.3'
```

### Comparing `cnocr-2.2.2.3/cnocr/app.py` & `cnocr-2.2.3/cnocr/app.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/classification/__init__.py` & `cnocr-2.2.3/cnocr/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/classification/dataset.py` & `cnocr-2.2.3/cnocr/classification/dataset.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/classification/image_classifier.py` & `cnocr-2.2.3/cnocr/classification/image_classifier.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/clf_cli.py` & `cnocr-2.2.3/cnocr/clf_cli.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/cli.py` & `cnocr-2.2.3/cnocr/cli.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/cn_ocr.py` & `cnocr-2.2.3/cnocr/cn_ocr.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/consts.py` & `cnocr-2.2.3/cnocr/consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,19 +104,27 @@
     'lstm': {'rnn_units': 128,},
     'gru': {'rnn_units': 128,},
     'fc': {'hidden_size': 128, 'dropout': 0.1,},
     'fcfull': {'hidden_size': 256, 'dropout': 0.3,},
 }
 
 
+HF_HUB_REPO_ID = "breezedeus/cnstd-cnocr-models"
+HF_HUB_SUBFOLDER = "models/cnocr/%s" % MODEL_VERSION
+
+
+def format_hf_hub_url(url: str) -> dict:
+    return {
+        'repo_id': HF_HUB_REPO_ID,
+        'subfolder': HF_HUB_SUBFOLDER,
+        'filename': url,
+    }
+
+
 class AvailableModels(object):
-    ROOT_URL = (
-        'https://huggingface.co/breezedeus/cnstd-cnocr-models/resolve/main/models/cnocr/%s/'
-        % MODEL_VERSION
-    )
     CNOCR_SPACE = '__cnocr__'
 
     # name: (epoch, url)
     CNOCR_MODELS = {
         ('densenet_lite_114-fc', 'pytorch'): (37, 'densenet_lite_114-fc.zip'),
         ('densenet_lite_124-fc', 'pytorch'): (39, 'densenet_lite_124-fc.zip'),
         ('densenet_lite_134-fc', 'pytorch'): (34, 'densenet_lite_134-fc.zip'),
@@ -169,25 +177,25 @@
             return None
 
     def get_epoch(self, model_name, model_backend) -> Optional[int]:
         if (model_name, model_backend) in self.CNOCR_MODELS:
             return self.CNOCR_MODELS[(model_name, model_backend)][0]
         return None
 
-    def get_url(self, model_name, model_backend) -> Optional[str]:
+    def get_url(self, model_name, model_backend) -> Optional[dict]:
         if (model_name, model_backend) in self.CNOCR_MODELS:
             url = self.CNOCR_MODELS[(model_name, model_backend)][1]
         elif (model_name, model_backend) in self.OUTER_MODELS:
             url = self.OUTER_MODELS[(model_name, model_backend)]['url']
         else:
             logger.warning(
                 'no url is found for model %s' % ((model_name, model_backend),)
             )
             return None
-        url = self.ROOT_URL + url
+        url = format_hf_hub_url(url)
         return url
 
 
 AVAILABLE_MODELS = AvailableModels()
 
 # 候选字符集合
 NUMBERS = string.digits + string.punctuation
```

### Comparing `cnocr-2.2.2.3/cnocr/data_utils/aug.py` & `cnocr-2.2.3/cnocr/data_utils/aug.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/data_utils/block_shuffle.py` & `cnocr-2.2.3/cnocr/data_utils/block_shuffle.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/data_utils/utils.py` & `cnocr-2.2.3/cnocr/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/dataset.py` & `cnocr-2.2.3/cnocr/dataset.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/label_cn.txt` & `cnocr-2.2.3/cnocr/label_cn.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/line_split.py` & `cnocr-2.2.3/cnocr/line_split.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/lr_scheduler.py` & `cnocr-2.2.3/cnocr/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/models/ctc.py` & `cnocr-2.2.3/cnocr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/models/densenet.py` & `cnocr-2.2.3/cnocr/models/densenet.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/models/mobilenet.py` & `cnocr-2.2.3/cnocr/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/models/ocr_model.py` & `cnocr-2.2.3/cnocr/models/ocr_model.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/ppocr/consts.py` & `cnocr-2.2.3/cnocr/ppocr/consts.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/ppocr/postprocess/__init__.py` & `cnocr-2.2.3/cnocr/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/ppocr/postprocess/rec_postprocess.py` & `cnocr-2.2.3/cnocr/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/ppocr/pp_recognizer.py` & `cnocr-2.2.3/cnocr/ppocr/pp_recognizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-# Copyright (C) 2022, [Breezedeus](https://github.com/breezedeus).
+# Copyright (C) 2022-2023, [Breezedeus](https://github.com/breezedeus).
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -22,22 +22,20 @@
 import logging
 from typing import Union, Optional, Collection, List, Tuple
 from pathlib import Path
 import math
 
 import numpy as np
 from PIL import Image
+from cnstd.utils import get_model_file
 
-from ..utils import resize_img, data_dir, get_model_file, read_img
+from ..utils import resize_img, data_dir, read_img
 from ..recognizer import Recognizer
 from .postprocess import build_post_process
-from .utility import (
-    get_image_file_list,
-    create_predictor,
-)
+from .utility import create_predictor
 from .consts import PP_SPACE
 from ..consts import MODEL_VERSION, AVAILABLE_MODELS
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -98,17 +96,21 @@
             return
 
         root = os.path.join(root, MODEL_VERSION)
         self._model_dir = os.path.join(root, PP_SPACE)
         model_fp = os.path.join(self._model_dir, '%s_rec_infer.onnx' % self._model_name)
         if not os.path.isfile(model_fp):
             logger.warning('can not find model file %s' % model_fp)
-            get_model_file(
-                self._model_name, self._model_backend, self._model_dir
-            )  # download the .zip file and unzip
+            if (self._model_name, self._model_backend) not in AVAILABLE_MODELS:
+                raise NotImplementedError(
+                    '%s is not a downloadable model'
+                    % ((self._model_name, self._model_backend),)
+                )
+            url = AVAILABLE_MODELS.get_url(self._model_name, self._model_backend)
+            get_model_file(url, self._model_dir)
 
         self._model_fp = model_fp
         logger.info('use model: %s' % self._model_fp)
 
     def resize_norm_img(self, img, max_wh_ratio):
         """
```

### Comparing `cnocr-2.2.2.3/cnocr/ppocr/utility.py` & `cnocr-2.2.3/cnocr/ppocr/utility.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/ppocr/utils/chinese_cht_dict.txt` & `cnocr-2.2.3/cnocr/ppocr/utils/chinese_cht_dict.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/ppocr/utils/ppocr_keys_v1.txt` & `cnocr-2.2.3/cnocr/ppocr/utils/ppocr_keys_v1.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/recognizer.py` & `cnocr-2.2.3/cnocr/recognizer.py`

 * *Files 2% similar despite different names*

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
@@ -22,20 +22,20 @@
 from glob import glob
 from typing import Union, List, Tuple, Optional, Collection
 from pathlib import Path
 
 import numpy as np
 from PIL import Image
 import torch
+from cnstd.utils import get_model_file
 
 from .consts import MODEL_VERSION, AVAILABLE_MODELS, VOCAB_FP
 from .models.ocr_model import OcrModel
 from .utils import (
     data_dir,
-    get_model_file,
     read_charset,
     check_model_name,
     check_context,
     read_img,
     load_model_params,
     resize_img,
     pad_img_seq,
@@ -161,17 +161,21 @@
         if len(fps) > 1:
             raise ValueError(
                 'multiple %s files are found in %s, not sure which one should be used'
                 % (model_ext, self._model_dir)
             )
         elif len(fps) < 1:
             logger.warning('no %s file is found in %s' % (model_ext, self._model_dir))
-            get_model_file(
-                self._model_name, self._model_backend, self._model_dir
-            )  # download the .zip file and unzip
+            if (self._model_name, self._model_backend) not in AVAILABLE_MODELS:
+                raise NotImplementedError(
+                    '%s is not a downloadable model'
+                    % ((self._model_name, self._model_backend),)
+                )
+            url = AVAILABLE_MODELS.get_url(self._model_name, self._model_backend)
+            get_model_file(url, self._model_dir)
             fps = glob(
                 '%s/%s*.%s' % (self._model_dir, self._model_file_prefix, model_ext)
             )
 
         self._model_fp = fps[0]
 
     def _get_model(self, context):
```

### Comparing `cnocr-2.2.2.3/cnocr/serve.py` & `cnocr-2.2.3/cnocr/serve.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.2.2.3/cnocr/trainer.py` & `cnocr-2.2.3/cnocr/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 class Metrics(object):
     def __init__(self, configs=None):
         configs = configs or {'accuracy': {}}
         self._metrics = dict()
         for name, _config in configs.items():
             if name not in METRIC_MAPPING:
                 logger.warning(f'metric {name} is not supported and will be ignored')
+                continue
             self._metrics[name] = METRIC_MAPPING[name](**_config)
         if len(self._metrics) < 1:
             raise RuntimeError(
                 'no available metric is set, please check you `train_config.json`'
             )
 
     @classmethod
```

### Comparing `cnocr-2.2.2.3/cnocr/utils.py` & `cnocr-2.2.3/cnocr/utils.py`

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
@@ -205,52 +205,14 @@
                 'If the "repo_url" is overridden, consider switching to '
                 'the default repo.'.format(fname)
             )
 
     return fname
 
 
-def get_model_file(model_name, model_backend, model_dir):
-    r"""Return location for the downloaded models on local file system.
-
-    This function will download from online model zoo when model cannot be found or has mismatch.
-    The root directory will be created if it doesn't exist.
-
-    Parameters
-    ----------
-    model_name : str
-    model_backend : str
-    model_dir : str, default $CNOCR_HOME
-        Location for keeping the model parameters.
-
-    Returns
-    -------
-    file_path
-        Path to the requested pretrained model file.
-    """
-    model_dir = os.path.expanduser(model_dir)
-    par_dir = os.path.dirname(model_dir)
-    os.makedirs(par_dir, exist_ok=True)
-
-    if (model_name, model_backend) not in AVAILABLE_MODELS:
-        raise NotImplementedError(
-            '%s is not a downloadable model' % ((model_name, model_backend),)
-        )
-    url = AVAILABLE_MODELS.get_url(model_name, model_backend)
-
-    zip_file_path = os.path.join(par_dir, os.path.basename(url))
-    if not os.path.exists(zip_file_path):
-        download(url, path=zip_file_path, overwrite=True)
-    with zipfile.ZipFile(zip_file_path) as zf:
-        zf.extractall(par_dir)
-    os.remove(zip_file_path)
-
-    return model_dir
-
-
 def read_charset(charset_fp):
     alphabet = []
     with open(charset_fp, encoding='utf-8') as fp:
         for line in fp:
             alphabet.append(line.rstrip('\n'))
     inv_alph_dict = {_char: idx for idx, _char in enumerate(alphabet)}
     if len(alphabet) != len(inv_alph_dict):
```

### Comparing `cnocr-2.2.2.3/cnocr.egg-info/PKG-INFO` & `cnocr-2.2.3/cnocr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,399 +1,401 @@
 Metadata-Version: 2.1
 Name: cnocr
-Version: 2.2.2.3
+Version: 2.2.3
 Summary: Python3 package for Chinese/English OCR, with small pretrained models
 Home-page: https://github.com/breezedeus/cnocr
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
-Description: <div align="center">
-          <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
-          <div>&nbsp;</div>
-        
-        [![Downloads](https://static.pepy.tech/personalized-badge/cnocr?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnocr)
-        [![license](https://img.shields.io/github/license/breezedeus/cnocr)](./LICENSE)
-        [![Docs](https://readthedocs.org/projects/cnocr/badge/?version=latest)](https://cnocr.readthedocs.io/zh/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/cnocr.svg)](https://badge.fury.io/py/cnocr)
-        [![forks](https://img.shields.io/github/forks/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
-        [![stars](https://img.shields.io/github/stars/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
-        ![last-releast](https://img.shields.io/github/release-date/breezedeus/cnocr)
-        ![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnocr)
-        [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
-        
-        [📖 文档](https://cnocr.readthedocs.io/zh/latest/) |
-        [🛠️ 安装](https://cnocr.readthedocs.io/zh/latest/install/) |
-        [🧳 可用模型](https://cnocr.readthedocs.io/zh/latest/models/) |
-        [🕹 模型训练](https://cnocr.readthedocs.io/zh/latest/train/) |
-        [🛀🏻 在线Demo](https://huggingface.co/spaces/breezedeus/cnocr) |
-        [💬 交流群](https://cnocr.readthedocs.io/zh/latest/contact/)
-        
-        </div>
-        
-        <div align="center">
-        
-        [English](./README_en.md) | 中文
-        
-        </div>
-        
-        # CnOCR
-        <div align="center">
-        <strong>Tech should serve the people, not enslave them!</strong>
-        <br>
-        <strong>请勿将此项目用于文字审查！</strong>
-        <br>
-        ---
-        </div>
-        
-        [**CnOCR**](https://github.com/breezedeus/cnocr) 是 **Python 3** 下的**文字识别**（**Optical Character Recognition**，简称**OCR**）工具包，支持**简体中文**、**繁体中文**（部分模型）、**英文**和**数字**的常见字符识别，支持竖排文字的识别。自带了**20+个** [训练好的模型](https://cnocr.readthedocs.io/zh/latest/models/)，适用于不同应用场景，安装后即可直接使用。同时，CnOCR也提供简单的[训练命令](https://cnocr.readthedocs.io/zh/latest/train/)供使用者训练自己的模型。欢迎扫码加小助手为好友，备注 `ocr`，小助手会定期统一邀请大家入群：
-        
-        <div align="center">
-          <img src="https://huggingface.co/datasets/breezedeus/cnocr-wx-qr-code/resolve/main/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
-        </div>
-        
-        
-        作者也维护 **知识星球** [**CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**未公开的模型**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。此外，**私享群中作者每月提供两次免费特有数据的训练服务**。
-        
-        ## 详细文档
-        
-        见 [CnOCR在线文档](https://cnocr.readthedocs.io/) 。
-        
-        ## 使用说明
-        
-        **CnOCR** 从 **V2.2** 开始，内部自动调用文字检测引擎 **[CnSTD](https://github.com/breezedeus/cnstd)** 进行文字检测和定位。所以 **CnOCR** V2.2 不仅能识别排版简单的印刷体文字图片，如截图图片，扫描件等，也能识别**一般图片中的场景文字**。
-        
-        以下是一些不同场景的调用示例。
-        
-        ## 在 Cloud IDE 中预览
-        
-        [https://idegithub.com/breezedeus/CnOCR](https://idegithub.com/breezedeus/CnOCR)
-        
-        ## 不同场景的调用示例
-        
-        ### 常见的图片识别
-        
-        所有参数都使用默认值即可。如果发现效果不够好，多调整下各个参数看效果，最终往往能获得比较理想的精度。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/huochepiao.jpeg'
-        ocr = CnOcr()  # 所有参数都使用默认值
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        识别结果：
-        
-        <div align="center">
-          <img src="./docs/predict-outputs/huochepiao.jpeg-result.jpg" alt="火车票识别" width="800px"/>
-        </div>
-        
-        
-        ### 排版简单的印刷体截图图片识别
-        
-        针对 **排版简单的印刷体文字图片**，如截图图片，扫描件图片等，可使用 `det_model_name='naive_det'`，相当于不使用文本检测模型，而使用简单的规则进行分行。
-        
-        > **Note**
-        >
-        >  `det_model_name='naive_det'` 的效果相当于 `V2.2` 之前（`V2.0.*`, `V2.1.*`）的 CnOCR 版本。
-        
-        使用 `det_model_name='naive_det'` 的最大优势是**速度快**，劣势是对图片比较挑剔。如何判断是否该使用此检测模型呢？最简单的方式就是拿应用图片试试效果，效果好就用，不好就不用。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/multi-line_cn1.png'
-        ocr = CnOcr(det_model_name='naive_det') 
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        识别结果：
-        
-        <div align="center">
-        
-        | 图片                                                                      | OCR结果                                                                                                                         |
-        | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
-        | ![docs/examples/multi-line_cn1.png](./docs/examples/multi-line_cn1.png) | 网络支付并无本质的区别，因为<br />每一个手机号码和邮件地址背后<br />都会对应着一个账户--这个账<br />户可以是信用卡账户、借记卡账<br />户，也包括邮局汇款、手机代<br />收、电话代收、预付费卡和点卡<br />等多种形式。 |
-        
-        </div>
-        
-        
-        ### 竖排文字识别
-        
-        采用来自 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR)（之后简称 **ppocr**）的中文识别模型 `rec_model_name='ch_PP-OCRv3'` 进行识别。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/shupai.png'
-        ocr = CnOcr(rec_model_name='ch_PP-OCRv3')
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        识别结果：
-        <div align="center">
-          <img src="./docs/predict-outputs/shupai.png-result.jpg" alt="竖排文字识别" width="800px"/>
-        </div>
-        
-        
-        ### 英文识别
-        
-        虽然中文检测和识别模型也能识别英文，但**专为英文文字训练的检测器和识别器往往精度更高**。如果是纯英文的应用场景，建议使用来自 **ppocr** 的英文检测模型 `det_model_name='en_PP-OCRv3_det'`， 和英文识别模型 `rec_model_name='en_PP-OCRv3'` 。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/en_book1.jpeg'
-        ocr = CnOcr(det_model_name='en_PP-OCRv3_det', rec_model_name='en_PP-OCRv3')
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        识别结果：
-        
-        <div align="center">
-          <img src="./docs/predict-outputs/en_book1.jpeg-result.jpg" alt="英文识别" width="600px"/>
-        </div>
-        
-        
-        ### 繁体中文识别
-        
-        采用来自ppocr的繁体识别模型 `rec_model_name='chinese_cht_PP-OCRv3'` 进行识别。
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/fanti.jpg'
-        ocr = CnOcr(rec_model_name='chinese_cht_PP-OCRv3')  # 识别模型使用繁体识别模型
-        out = ocr.ocr(img_fp)
-        
-        print(out)
-        ```
-        
-        使用此模型时请注意以下问题：
-        
-        * 识别精度一般，不是很好；
-        
-        * 除了繁体字，对标点、英文、数字的识别都不好；
-        
-        * 此模型不支持竖排文字的识别。
-        
-        识别结果：
-        <div align="center">
-          <img src="./docs/predict-outputs/fanti.jpg-result.jpg" alt="繁体中文识别" width="700px"/>
-        </div>
-        
-        
-        ### 单行文字的图片识别
-        
-        如果明确知道待识别的图片是单行文字图片（如下图），可以使用类函数 `CnOcr.ocr_for_single_line()` 进行识别。这样就省掉了文字检测的时间，速度会快一倍以上。
-        
-        <div align="center">
-          <img src="./docs/examples/helloworld.jpg" alt="单行文本识别" width="300px"/>
-        </div>
-        调用代码如下：
-        
-        ```python
-        from cnocr import CnOcr
-        
-        img_fp = './docs/examples/helloworld.jpg'
-        ocr = CnOcr()
-        out = ocr.ocr_for_single_line(img_fp)
-        print(out)
-        ```
-        
-        
-        
-        ### 更多应用示例
-        
-        * **核酸疫苗截图识别**
-        <div align="center">
-          <img src="./docs/predict-outputs/jiankangbao.jpeg-result.jpg" alt="核酸疫苗截图识别" width="500px"/>
-        </div>
-        
-        * **身份证识别**
-        <div align="center">
-          <img src="./docs/predict-outputs/aobama.webp-result.jpg" alt="身份证识别" width="700px"/>
-        </div>
-        
-        * **饭店小票识别**
-        <div align="center">
-          <img src="./docs/predict-outputs/fapiao.jpeg-result.jpg" alt="饭店小票识别" width="500px"/>
-        </div>
-          
-        
-          
-        
-        ## 安装
-        
-        嗯，顺利的话一行命令即可。
-        
-        ```bash
-        pip install cnocr
-        ```
-        
-        安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
-        
-        ```bash
-        pip install cnocr -i https://pypi.doubanio.com/simple
-        ```
-        
-        > **Note** 
-        >
-        > 请使用 **Python3**（3.6以及之后版本应该都行），没测过Python2下是否ok。
-        
-        更多说明可见 [安装文档](https://cnocr.readthedocs.io/zh/latest/install/)。
-        
-        > **Warning** 
-        >
-        > 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到问题，但一般都是常见问题，可以自行百度/Google解决。
-        
-        
-        
-        
-        
-        ## HTTP服务
-        
-        CnOCR **V2.2.1** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
-        
-        ```bash
-        pip install cnocr[serve]
-        ```
-        
-        
-        
-        安装完成后，可以通过以下命令启动HTTP服务（**`-p`** 后面的数字是**端口**，可以根据需要自行调整）：
-        
-        ```bash
-        cnocr serve -p 8501
-        ```
-        
-        
-        
-        服务开启后，可以使用以下方式调用服务。
-        
-        
-        
-        ### 命令行
-        
-        比如待识别文件为 `docs/examples/huochepiao.jpeg`，如下使用 curl 调用服务：
-        
-        ```bash
-        > curl -F image=@docs/examples/huochepiao.jpeg http://0.0.0.0:8501/ocr
-        ```
-        
-        
-        
-        ### Python
-        
-        使用如下方式调用服务：
-        
-        ```python
-        import requests
-        
-        image_fp = 'docs/examples/huochepiao.jpeg'
-        r = requests.post(
-            'http://0.0.0.0:8501/ocr', files={'image': (image_fp, open(image_fp, 'rb'), 'image/png')},
-        )
-        ocr_out = r.json()['results']
-        print(ocr_out)
-        ```
-        
-        
-        
-        具体也可参考文件 [scripts/screenshot_daemon_with_server.py](scripts/screenshot_daemon_with_server.py) 。 
-        
-        
-        
-        ### 其他语言
-        
-        请参照 curl 的调用方式自行实现。
-        
-        
-        
-        
-        
-        ## 可使用的模型
-        
-        ### 可使用的检测模型
-        
-        | `det_model_name`                                             | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                       | 是否支持竖排文字识别 |
-        | ------------------------------------------------------------ | ------------ | --------- | ------------ | ------------ | ------------------------------ | -------------------- |
-        | db_shufflenet_v2                                             | √            | X         | cnocr        | 18 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | **db_shufflenet_v2_small**                                   | √            | X         | cnocr        | 12 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | [db_shufflenet_v2_tiny](https://mp.weixin.qq.com/s/fHPNoGyo72EFApVhEgR6Nw) | √            | X         | cnocr        | 7.5 M        | 简体中文、繁体中文、英文、数字 | √                    |
-        | db_mobilenet_v3                                              | √            | X         | cnocr        | 16 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | db_mobilenet_v3_small                                        | √            | X         | cnocr        | 7.9 M        | 简体中文、繁体中文、英文、数字 | √                    |
-        | db_resnet34                                                  | √            | X         | cnocr        | 86 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | db_resnet18                                                  | √            | X         | cnocr        | 47 M         | 简体中文、繁体中文、英文、数字 | √                    |
-        | ch_PP-OCRv3_det                                              | X            | √         | ppocr        | 2.3 M        | 简体中文、繁体中文、英文、数字 | √                    |
-        | ch_PP-OCRv2_det                                              | X            | √         | ppocr        | 2.2 M        | 简体中文、繁体中文、英文、数字 | √                    |
-        | **en_PP-OCRv3_det**                                          | X            | √         | ppocr        | 2.3 M        | **英文**、数字                 | √                    |
-        
-        
-        
-        ### 可使用的识别模型
-        
-        | `rec_model_name`          | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                 | 是否支持竖排文字识别 |
-        | ------------------------- | ------------ | --------- | ------------ | ------------ | ------------------------ | -------------------- |
-        | densenet_lite_114-fc      | √            | √         | cnocr        | 4.9 M        | 简体中文、英文、数字     | X                    |
-        | densenet_lite_124-fc      | √            | √         | cnocr        | 5.1 M        | 简体中文、英文、数字     | X                    |
-        | densenet_lite_134-fc      | √            | √         | cnocr        | 5.4 M        | 简体中文、英文、数字     | X                    |
-        | densenet_lite_136-fc      | √            | √         | cnocr        | 5.9 M        | 简体中文、英文、数字     | X                    |
-        | densenet_lite_134-gru     | √            | X         | cnocr        | 11 M         | 简体中文、英文、数字     | X                    |
-        | densenet_lite_136-gru     | √            | X         | cnocr        | 12 M         | 简体中文、英文、数字     | X                    |
-        | ch_PP-OCRv3               | X            | √         | ppocr        | 10 M         | 简体中文、英文、数字     | √                    |
-        | ch_ppocr_mobile_v2.0      | X            | √         | ppocr        | 4.2 M        | 简体中文、英文、数字     | √                    |
-        | **en_PP-OCRv3**           | X            | √         | ppocr        | 8.5 M        | **英文**、数字           | √                    |
-        | **en_number_mobile_v2.0** | X            | √         | ppocr        | 1.8 M        | **英文**、数字           | √                    |
-        | **chinese_cht_PP-OCRv3**  | X            | √         | ppocr        | 11 M         | **繁体中文**、英文、数字 | X                    |
-        
-        ## 未来工作
-        
-        * [x] 支持图片包含多行文字 (`Done`)
-        * [x] crnn模型支持可变长预测，提升灵活性 (since `V1.0.0`)
-        * [x] 完善测试用例 (`Doing`)
-        * [x] 修bugs（目前代码还比较凌乱。。） (`Doing`)
-        * [x] 支持`空格`识别（since `V1.1.0`）
-        * [x] 尝试新模型，如 DenseNet，进一步提升识别准确率（since `V1.1.0`）
-        * [x] 优化训练集，去掉不合理的样本；在此基础上，重新训练各个模型
-        * [x] 由 MXNet 改为 PyTorch 架构（since `V2.0.0`）
-        * [x] 基于 PyTorch 训练更高效的模型
-        * [x] 支持列格式的文字识别
-        * [x] 打通与 [CnSTD](https://github.com/breezedeus/cnstd) 的无缝衔接（since `V2.2`）
-        * [ ] 支持更多的应用场景，如公式识别、表格识别、版面分析等
-        
-        
-        
-        ## 给作者来杯咖啡
-        
-        开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
-        
-        ---
-        
-        官方代码库：[https://github.com/breezedeus/cnocr](https://github.com/breezedeus/cnocr)。
-        
-        
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
-Provides-Extra: serve
 Provides-Extra: dev
+Provides-Extra: serve
+License-File: LICENSE
+
+<div align="center">
+  <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
+  <div>&nbsp;</div>
+
+[![Downloads](https://static.pepy.tech/personalized-badge/cnocr?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnocr)
+[![license](https://img.shields.io/github/license/breezedeus/cnocr)](./LICENSE)
+[![Docs](https://readthedocs.org/projects/cnocr/badge/?version=latest)](https://cnocr.readthedocs.io/zh/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/cnocr.svg)](https://badge.fury.io/py/cnocr)
+[![forks](https://img.shields.io/github/forks/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
+[![stars](https://img.shields.io/github/stars/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
+![last-releast](https://img.shields.io/github/release-date/breezedeus/cnocr)
+![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnocr)
+[![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
+
+[📖 文档](https://cnocr.readthedocs.io/zh/latest/) |
+[🛠️ 安装](https://cnocr.readthedocs.io/zh/latest/install/) |
+[🧳 可用模型](https://cnocr.readthedocs.io/zh/latest/models/) |
+[🕹 模型训练](https://cnocr.readthedocs.io/zh/latest/train/) |
+[🛀🏻 在线Demo](https://huggingface.co/spaces/breezedeus/cnocr) |
+[💬 交流群](https://cnocr.readthedocs.io/zh/latest/contact/)
+
+</div>
+
+<div align="center">
+
+[English](./README_en.md) | 中文
+
+</div>
+
+# CnOCR
+<div align="center">
+<strong>Tech should serve the people, not enslave them!</strong>
+<br>
+<strong>请勿将此项目用于文字审查！</strong>
+<br>
+---
+</div>
+
+[**CnOCR**](https://github.com/breezedeus/cnocr) 是 **Python 3** 下的**文字识别**（**Optical Character Recognition**，简称**OCR**）工具包，支持**简体中文**、**繁体中文**（部分模型）、**英文**和**数字**的常见字符识别，支持竖排文字的识别。自带了**20+个** [训练好的模型](https://cnocr.readthedocs.io/zh/latest/models/)，适用于不同应用场景，安装后即可直接使用。同时，CnOCR也提供简单的[训练命令](https://cnocr.readthedocs.io/zh/latest/train/)供使用者训练自己的模型。欢迎扫码加小助手为好友，备注 `ocr`，小助手会定期统一邀请大家入群：
+
+<div align="center">
+  <img src="https://huggingface.co/datasets/breezedeus/cnocr-wx-qr-code/resolve/main/wx-qr-code.JPG" alt="微信群二维码" width="300px"/>
+</div>
+
+
+作者也维护 **知识星球** [**CnOCR/CnSTD私享群**](https://t.zsxq.com/FEYZRJQ) ，这里面的提问会较快得到作者的回复，欢迎加入。**知识星球私享群**也会陆续发布一些CnOCR/CnSTD相关的私有资料，包括[**更详细的训练教程**](https://articles.zsxq.com/id_u6b4u0wrf46e.html)，**未公开的模型**，**不同应用场景的调用代码**，使用过程中遇到的难题解答等。本群也会发布OCR/STD相关的最新研究资料。此外，**私享群中作者每月提供两次免费特有数据的训练服务**。
+
+## 详细文档
+
+见 [CnOCR在线文档](https://cnocr.readthedocs.io/) 。
+
+## 使用说明
+
+**CnOCR** 从 **V2.2** 开始，内部自动调用文字检测引擎 **[CnSTD](https://github.com/breezedeus/cnstd)** 进行文字检测和定位。所以 **CnOCR** V2.2 不仅能识别排版简单的印刷体文字图片，如截图图片，扫描件等，也能识别**一般图片中的场景文字**。
+
+以下是一些不同场景的调用示例。
+
+## 在 Cloud IDE 中预览
+
+[https://idegithub.com/breezedeus/CnOCR](https://idegithub.com/breezedeus/CnOCR)
+
+## 不同场景的调用示例
+
+### 常见的图片识别
+
+所有参数都使用默认值即可。如果发现效果不够好，多调整下各个参数看效果，最终往往能获得比较理想的精度。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/huochepiao.jpeg'
+ocr = CnOcr()  # 所有参数都使用默认值
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+识别结果：
+
+<div align="center">
+  <img src="./docs/predict-outputs/huochepiao.jpeg-result.jpg" alt="火车票识别" width="800px"/>
+</div>
+
+
+### 排版简单的印刷体截图图片识别
+
+针对 **排版简单的印刷体文字图片**，如截图图片，扫描件图片等，可使用 `det_model_name='naive_det'`，相当于不使用文本检测模型，而使用简单的规则进行分行。
+
+> **Note**
+>
+>  `det_model_name='naive_det'` 的效果相当于 `V2.2` 之前（`V2.0.*`, `V2.1.*`）的 CnOCR 版本。
+
+使用 `det_model_name='naive_det'` 的最大优势是**速度快**，劣势是对图片比较挑剔。如何判断是否该使用此检测模型呢？最简单的方式就是拿应用图片试试效果，效果好就用，不好就不用。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/multi-line_cn1.png'
+ocr = CnOcr(det_model_name='naive_det') 
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+识别结果：
+
+<div align="center">
+
+| 图片                                                                      | OCR结果                                                                                                                         |
+| ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
+| ![docs/examples/multi-line_cn1.png](./docs/examples/multi-line_cn1.png) | 网络支付并无本质的区别，因为<br />每一个手机号码和邮件地址背后<br />都会对应着一个账户--这个账<br />户可以是信用卡账户、借记卡账<br />户，也包括邮局汇款、手机代<br />收、电话代收、预付费卡和点卡<br />等多种形式。 |
+
+</div>
+
+
+### 竖排文字识别
+
+采用来自 [**PaddleOCR**](https://github.com/PaddlePaddle/PaddleOCR)（之后简称 **ppocr**）的中文识别模型 `rec_model_name='ch_PP-OCRv3'` 进行识别。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/shupai.png'
+ocr = CnOcr(rec_model_name='ch_PP-OCRv3')
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+识别结果：
+<div align="center">
+  <img src="./docs/predict-outputs/shupai.png-result.jpg" alt="竖排文字识别" width="800px"/>
+</div>
+
+
+### 英文识别
+
+虽然中文检测和识别模型也能识别英文，但**专为英文文字训练的检测器和识别器往往精度更高**。如果是纯英文的应用场景，建议使用来自 **ppocr** 的英文检测模型 `det_model_name='en_PP-OCRv3_det'`， 和英文识别模型 `rec_model_name='en_PP-OCRv3'` 。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/en_book1.jpeg'
+ocr = CnOcr(det_model_name='en_PP-OCRv3_det', rec_model_name='en_PP-OCRv3')
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+识别结果：
+
+<div align="center">
+  <img src="./docs/predict-outputs/en_book1.jpeg-result.jpg" alt="英文识别" width="600px"/>
+</div>
+
+
+### 繁体中文识别
+
+采用来自ppocr的繁体识别模型 `rec_model_name='chinese_cht_PP-OCRv3'` 进行识别。
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/fanti.jpg'
+ocr = CnOcr(rec_model_name='chinese_cht_PP-OCRv3')  # 识别模型使用繁体识别模型
+out = ocr.ocr(img_fp)
+
+print(out)
+```
+
+使用此模型时请注意以下问题：
+
+* 识别精度一般，不是很好；
+
+* 除了繁体字，对标点、英文、数字的识别都不好；
+
+* 此模型不支持竖排文字的识别。
+
+识别结果：
+<div align="center">
+  <img src="./docs/predict-outputs/fanti.jpg-result.jpg" alt="繁体中文识别" width="700px"/>
+</div>
+
+
+### 单行文字的图片识别
+
+如果明确知道待识别的图片是单行文字图片（如下图），可以使用类函数 `CnOcr.ocr_for_single_line()` 进行识别。这样就省掉了文字检测的时间，速度会快一倍以上。
+
+<div align="center">
+  <img src="./docs/examples/helloworld.jpg" alt="单行文本识别" width="300px"/>
+</div>
+调用代码如下：
+
+```python
+from cnocr import CnOcr
+
+img_fp = './docs/examples/helloworld.jpg'
+ocr = CnOcr()
+out = ocr.ocr_for_single_line(img_fp)
+print(out)
+```
+
+
+
+### 更多应用示例
+
+* **核酸疫苗截图识别**
+<div align="center">
+  <img src="./docs/predict-outputs/jiankangbao.jpeg-result.jpg" alt="核酸疫苗截图识别" width="500px"/>
+</div>
+
+* **身份证识别**
+<div align="center">
+  <img src="./docs/predict-outputs/aobama.webp-result.jpg" alt="身份证识别" width="700px"/>
+</div>
+
+* **饭店小票识别**
+<div align="center">
+  <img src="./docs/predict-outputs/fapiao.jpeg-result.jpg" alt="饭店小票识别" width="500px"/>
+</div>
+  
+
+  
+
+## 安装
+
+嗯，顺利的话一行命令即可。
+
+```bash
+pip install cnocr
+```
+
+安装速度慢的话，可以指定国内的安装源，如使用豆瓣源：
+
+```bash
+pip install cnocr -i https://pypi.doubanio.com/simple
+```
+
+> **Note** 
+>
+> 请使用 **Python3**（3.6以及之后版本应该都行），没测过Python2下是否ok。
+
+更多说明可见 [安装文档](https://cnocr.readthedocs.io/zh/latest/install/)。
+
+> **Warning** 
+>
+> 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到问题，但一般都是常见问题，可以自行百度/Google解决。
+
+
+
+
+
+## HTTP服务
+
+CnOCR **V2.2.1** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
+
+```bash
+pip install cnocr[serve]
+```
+
+
+
+安装完成后，可以通过以下命令启动HTTP服务（**`-p`** 后面的数字是**端口**，可以根据需要自行调整）：
+
+```bash
+cnocr serve -p 8501
+```
+
+
+
+服务开启后，可以使用以下方式调用服务。
+
+
+
+### 命令行
+
+比如待识别文件为 `docs/examples/huochepiao.jpeg`，如下使用 curl 调用服务：
+
+```bash
+> curl -F image=@docs/examples/huochepiao.jpeg http://0.0.0.0:8501/ocr
+```
+
+
+
+### Python
+
+使用如下方式调用服务：
+
+```python
+import requests
+
+image_fp = 'docs/examples/huochepiao.jpeg'
+r = requests.post(
+    'http://0.0.0.0:8501/ocr', files={'image': (image_fp, open(image_fp, 'rb'), 'image/png')},
+)
+ocr_out = r.json()['results']
+print(ocr_out)
+```
+
+
+
+具体也可参考文件 [scripts/screenshot_daemon_with_server.py](scripts/screenshot_daemon_with_server.py) 。 
+
+
+
+### 其他语言
+
+请参照 curl 的调用方式自行实现。
+
+
+
+
+
+## 可使用的模型
+
+### 可使用的检测模型
+
+| `det_model_name`                                             | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                       | 是否支持竖排文字识别 |
+| ------------------------------------------------------------ | ------------ | --------- | ------------ | ------------ | ------------------------------ | -------------------- |
+| db_shufflenet_v2                                             | √            | X         | cnocr        | 18 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| **db_shufflenet_v2_small**                                   | √            | X         | cnocr        | 12 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| [db_shufflenet_v2_tiny](https://mp.weixin.qq.com/s/fHPNoGyo72EFApVhEgR6Nw) | √            | X         | cnocr        | 7.5 M        | 简体中文、繁体中文、英文、数字 | √                    |
+| db_mobilenet_v3                                              | √            | X         | cnocr        | 16 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| db_mobilenet_v3_small                                        | √            | X         | cnocr        | 7.9 M        | 简体中文、繁体中文、英文、数字 | √                    |
+| db_resnet34                                                  | √            | X         | cnocr        | 86 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| db_resnet18                                                  | √            | X         | cnocr        | 47 M         | 简体中文、繁体中文、英文、数字 | √                    |
+| ch_PP-OCRv3_det                                              | X            | √         | ppocr        | 2.3 M        | 简体中文、繁体中文、英文、数字 | √                    |
+| ch_PP-OCRv2_det                                              | X            | √         | ppocr        | 2.2 M        | 简体中文、繁体中文、英文、数字 | √                    |
+| **en_PP-OCRv3_det**                                          | X            | √         | ppocr        | 2.3 M        | **英文**、数字                 | √                    |
+
+
+
+### 可使用的识别模型
+
+| `rec_model_name`          | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                 | 是否支持竖排文字识别 |
+| ------------------------- | ------------ | --------- | ------------ | ------------ | ------------------------ | -------------------- |
+| densenet_lite_114-fc      | √            | √         | cnocr        | 4.9 M        | 简体中文、英文、数字     | X                    |
+| densenet_lite_124-fc      | √            | √         | cnocr        | 5.1 M        | 简体中文、英文、数字     | X                    |
+| densenet_lite_134-fc      | √            | √         | cnocr        | 5.4 M        | 简体中文、英文、数字     | X                    |
+| densenet_lite_136-fc      | √            | √         | cnocr        | 5.9 M        | 简体中文、英文、数字     | X                    |
+| densenet_lite_134-gru     | √            | X         | cnocr        | 11 M         | 简体中文、英文、数字     | X                    |
+| densenet_lite_136-gru     | √            | X         | cnocr        | 12 M         | 简体中文、英文、数字     | X                    |
+| ch_PP-OCRv3               | X            | √         | ppocr        | 10 M         | 简体中文、英文、数字     | √                    |
+| ch_ppocr_mobile_v2.0      | X            | √         | ppocr        | 4.2 M        | 简体中文、英文、数字     | √                    |
+| **en_PP-OCRv3**           | X            | √         | ppocr        | 8.5 M        | **英文**、数字           | √                    |
+| **en_number_mobile_v2.0** | X            | √         | ppocr        | 1.8 M        | **英文**、数字           | √                    |
+| **chinese_cht_PP-OCRv3**  | X            | √         | ppocr        | 11 M         | **繁体中文**、英文、数字 | X                    |
+
+## 未来工作
+
+* [x] 支持图片包含多行文字 (`Done`)
+* [x] crnn模型支持可变长预测，提升灵活性 (since `V1.0.0`)
+* [x] 完善测试用例 (`Doing`)
+* [x] 修bugs（目前代码还比较凌乱。。） (`Doing`)
+* [x] 支持`空格`识别（since `V1.1.0`）
+* [x] 尝试新模型，如 DenseNet，进一步提升识别准确率（since `V1.1.0`）
+* [x] 优化训练集，去掉不合理的样本；在此基础上，重新训练各个模型
+* [x] 由 MXNet 改为 PyTorch 架构（since `V2.0.0`）
+* [x] 基于 PyTorch 训练更高效的模型
+* [x] 支持列格式的文字识别
+* [x] 打通与 [CnSTD](https://github.com/breezedeus/cnstd) 的无缝衔接（since `V2.2`）
+* [ ] 支持更多的应用场景，如公式识别、表格识别、版面分析等
+
+
+
+## 给作者来杯咖啡
+
+开源不易，如果此项目对您有帮助，可以考虑 [给作者加点油🥤，鼓鼓气💪🏻](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
+
+---
+
+官方代码库：[https://github.com/breezedeus/cnocr](https://github.com/breezedeus/cnocr)。
+
```

### Comparing `cnocr-2.2.2.3/cnocr.egg-info/SOURCES.txt` & `cnocr-2.2.3/cnocr.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 cnocr/__init__.py
 cnocr/__version__.py
 cnocr/app.py
 cnocr/clf_cli.py
 cnocr/cli.py
@@ -39,8 +40,14 @@
 cnocr/ppocr/pp_recognizer.py
 cnocr/ppocr/utility.py
 cnocr/ppocr/postprocess/__init__.py
 cnocr/ppocr/postprocess/rec_postprocess.py
 cnocr/ppocr/utils/__init__.py
 cnocr/ppocr/utils/chinese_cht_dict.txt
 cnocr/ppocr/utils/en_dict.txt
-cnocr/ppocr/utils/ppocr_keys_v1.txt
+cnocr/ppocr/utils/ppocr_keys_v1.txt
+tests/test_cnocr.py
+tests/test_dataset.py
+tests/test_models.py
+tests/test_ppocr.py
+tests/test_pytorch.py
+tests/test_trainer.py
```

### Comparing `cnocr-2.2.2.3/setup.py` & `cnocr-2.2.3/setup.py`

 * *Files 2% similar despite different names*

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
@@ -92,13 +92,14 @@
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

